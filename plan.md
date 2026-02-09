# The Plan

## Reasoning

### Goal

Land a spring 2027 co-op/internship as an ML Engineer or Data Scientist (Consumer) at a top-tier company (Meta, Google, Amazon, OpenAI, Anthropic, Airbnb, Palantir etc.). Build toward $270k/year total comp by May 2029.

### Target Roles

1. Machine Learning Engineer
2. ML Engineer (Recommendation Systems)
3. Data Scientist (Consumer)

### Weekly Schedule

19 hours/week. Every week. No exceptions.

| Day | Time | Focus |
|-----|------|-------|
| Monday | 12pm-3pm | Project |
| Tuesday | 12pm-3pm | Project |
| Wednesday | 12pm-3pm | Project |
| Thursday | 12pm-3pm | Networking |
| Friday | 12pm-3pm | HackerRank / LeetCode / DSA |
| Saturday | 1pm-3pm | Research + Retrieval |
| Sunday | 1pm-3pm | Catch-up buffer |

### Time Allocation

| Activity | % | Hrs/week |
|----------|---|----------|
| Building projects | 47% | 9 |
| Networking | 16% | 3 |
| HackerRank / LeetCode / DSA | 16% | 3 |
| Research + retrieval practice | 11% | 2 |
| Catch-up buffer | 10% | 2 |

### Lag Metrics

Track every week. Weekly execution score = (metrics hit / 7) x 100%. 85%+ = on track. Below 65% for 2 weeks = diagnose what's going wrong.

1. Hours on project work (target: 9)
2. Hours on networking (target: 3)
3. Hours on HackerRank/LeetCode/DSA (target: 3)
4. Hours on research + retrieval (target: 2)
5. Outreach messages sent — DMs, connection requests, coffee chat asks (target: 3)
6. Posts published across LinkedIn/X/GitHub (target: 2)
7. Active recall pass/fail — could you explain last week's code from memory? (target: pass)

### Rules

These come from practitioners who already have the jobs I want. Follow them exactly.

1. **Never cold apply.** Always get a referral first. Employees get paid for successful referrals — you're not just asking for a favor. (Sajjaad, $220k Amazon)
2. **Learn top-down, not bottom-up.** Start with a project. Hit a wall. Learn exactly what you need to get past it. Never watch 40 hours of lectures before building. (Gabriel, OpenAI)
3. **Every project ships as a live demo with a link.** You should be able to send someone a URL. A good demo communicates that you understand coding. (Gabriel, OpenAI)
4. **Recursive gap filling.** When AI writes code, go line by line through the core ML logic. When something is vague ("this helps the algorithm learn faster"), ask "what do you mean" recursively until you truly understand. Then explain it back to AI until it confirms you get it. (Gabriel, OpenAI)
5. **Active recall weekly.** A week after writing code, explain it from memory. If you can't, you were vibe coding. Get a refresher. (Victor, TikTok MLE)
6. **System design > LeetCode.** Ray Fu uses system design every day at work. He never uses LeetCode knowledge except the meta-skill of problem-solving. Both matter, but system design matters more. (Ray Fu)
7. **Reach out to engineers and hiring managers, not recruiters.** Recruiters aren't technical and go with safe bets. Engineers can look at your demo and actually evaluate you. (Gabriel, OpenAI)
8. **Document everything you build and its impact.** At the end of the year this is how you get promoted. (Ray Fu)
9. **Phone in another room during learning blocks.** Distraction/procrastination is the #1 obstacle.
10. **Track daily in Notion.** Log what you worked on and how many hours. Weekly review on Saturdays to check if you're hitting 19 hrs/week.

### Skills I'm Prioritizing (from 36 job postings)

| Skill | Frequency | How I'll Learn It |
|-------|-----------|-------------------|
| Python | 100% | Through every project |
| PyTorch | 78% | Primary framework for all ML projects |
| Distributed Systems / Spark | 50% | Through rec sys project at scale |
| A/B Testing / Experimentation | 42% | Through DS Consumer-focused project |
| Recommendation / Personalization | 39% | First project |
| Deep Learning | 39% | Through projects, top-down |
| SQL | 33% | Through data pipelines in projects |
| Data Visualization | 33% | Through project dashboards and analysis |

### What I'm NOT Spending Time On

- DS (ML) research track — requires PhD, not targeting this for first job
- NLP and Computer Vision as standalone study — not interested, low overlap with targets
- Mathematical proofs and derivations — understand intuition, don't derive
- TensorFlow and JAX — go deep on PyTorch only
- C++ and CUDA — light exposure only, 10-20 hours total
- Heavy Kubernetes / MLOps — learn Docker and simple deployment, skip deep K8s
- Video lectures and courses — use AI as tutor instead
- Textbooks cover-to-cover — use AI summaries, only open books when AI isn't clear enough

---

## 🧱🔨 Phase 1 (Feb-Apr) FOUNDATIONS + FIRST DEMO

Build the rec sys project and ship it as a live demo anyone can access via URL. Use /professor-mode to write and understand code myself. Begin the HackerRank and networking pipelines.

### Weekly Activities

#### 🛠️ Monday, Tuesday, Wednesday — Project: Build + Ship Recommendation System
- Set up rec sys project repo with folder structure (src/, tests/, configs/, scripts/, app/)
- Download Goodreads-10K dataset (10K books, 53K users, 6M ratings), explore distributions (rating counts, user activity, genre spread)
- Implement data loading pipeline: PyTorch Dataset and DataLoader for user-item interactions
- Implement train/validation/test split BY USER (not by rating — this tests generalization to new users)
- Set up YAML config for all hyperparameters (embedding dim, learning rate, batch size, negative sampling ratio)
- Set up Weights & Biases experiment tracking, log all runs with metrics and hyperparameters
- Implement and evaluate baseline models: Random recommender, Popularity-based recommender (NDCG@10, Hit Rate@10, MRR)
- Start Two-Tower model: User Tower (interaction history → user embedding) + Item Tower (item features → item embedding) + dot product scoring
- Implement training loop with BPR loss (pairwise ranking loss) and negative sampling with popularity weighting
- Train on Goodreads training set, validate on validation set, beat baselines by meaningful margin
- Debug things yourself before asking AI — build the debugging muscle
- Recursive gap filling: PyTorch Dataset/DataLoader, NDCG computation, embedding layers, BPR loss derivation, Two-Tower vs NCF vs Matrix Factorization tradeoffs
- Finish Two-Tower model: hyperparameter tuning (embedding dimension, learning rate, batch size, negative sampling ratio), log all experiments to W&B with model checkpoints
- If Two-Tower training is unstable: fallback to NCF (simpler architecture, same evaluation pipeline)
- Add content feature hybrid for explainability: extract genre tags, author, publication year, description keywords from Goodreads metadata
- For each recommendation, generate human-readable explanations: find top-3 similar books from user's liked set (genre overlap, author overlap, embedding distance), format as "Recommended because you liked [Book X] and [Book Y]. Shared genres: Science Fiction, Philosophy."
- Implement cold-start handling: test synthetic users with only 5 ratings, add popularity-weighted fallback for users with <10 ratings if needed
- Build FastAPI backend: POST /onboarding (receive ratings, return initial recs), POST /feedback (updated rating, re-ranked recs), GET /recommend/{user_id} (top-K with explanations + confidence), GET /health (model version, dataset version, commit hash). Input validation, error handling, log inference latency. Target <500ms per request.
- Build React frontend with shadcn/ui + Tailwind: onboarding screen (grid of ~30 books with covers, rate 5-10 books 1-5 stars), results screen (ranked list with cover, title, author, predicted rating, explanation, confidence), feedback loop (rate any rec, refresh re-ranks), model info panel, "Run example" button with pre-filled ratings
- Fallback: if React eats too much time, switch to Streamlit — a working Streamlit demo beats an unfinished React app
- Run final offline evaluation on test set, report all metrics vs all baselines with deltas
- Conduct user studies: recruit 5-10 people, have them rate 10-15 books, rate recommendation quality 1-5, collect qualitative feedback on failure modes
- Implement simulated A/B test: split test users into Group A (Two-Tower) and Group B (Popularity baseline), compare NDCG@10, report effect size, 95% CI, p-value, create visualization (cut this first if behind schedule)
- Write unit tests: data transforms, model inference (deterministic output given fixed input), API endpoints, edge cases (1 rating, all 5-star, all 1-star)
- Dockerize backend and frontend, deploy to Railway or Render (free tier), verify live URL works end-to-end
- Write README: problem statement, architecture diagram (Two-Tower + content hybrid), model explanation, evaluation results with visualizations, design tradeoffs (why Two-Tower over NCF, why explicit ratings, why books-only), known limitations, next steps

#### 🤝 Thursday — Networking
- Send 2-3 LinkedIn connection requests to Northeastern alumni at target companies (find via linkedin.com/school/khoury-college/people/)
- Message 1 person/week for a coffee chat using Nishanth's DM templates in 1metalearning.md
- Write and publish 2 posts/week across LinkedIn, X, and GitHub about what you're learning or building
- Goal early in this phase: build relationships. Do NOT ask for referrals yet.
- Once the rec sys ships: post about it on LinkedIn and X — what you built, what you learned, one interesting technical challenge
- Continue weekly coffee chat outreach (message 1 new person, follow up with existing conversations)
- Research and sign up for end-of-semester Khoury career events and employer panels — bring your demo
- Investigate joining AINU when applications open next fall

#### 🧩 Friday — HackerRank / LeetCode / Data Structures & Algorithms
- First 2-3 Fridays: learn data structures visually on csvistool.com (arrays, linked lists, stacks, queues, hash maps, trees, graphs, heaps)
- Start on HackerRank first — use the Interview Preparation Kit and 1-Month Preparation Kit. HackerRank uses raw stdin/stdout parsing which is different from LeetCode's pre-parsed inputs; 3,000+ companies (Amazon, Goldman Sachs, Bloomberg, Adobe, Uber) use HackerRank as their actual screening tool
- Do 2-3 easy problems per session, one data structure per Friday
- Also do HackerRank's SQL track — SQL appears in 33% of target roles and 89% of DS Consumer roles. Write queries against the Goodreads dataset too: practice joins, aggregations, window functions on the ratings/books/users tables
- Track which data structures you've covered
- By end of this phase, should have covered ALL major data structures at least once
- Transition to LeetCode for deeper algorithm pattern mastery — company-tagged problems (Premium), Blind 75, NeetCode 150
- Start recognizing patterns: "this is a two-pointer problem," "this needs a hash map"
- Continue SQL practice: HackerRank SQL track + writing queries against your project's data

#### 🧠 Saturday — Research + Retrieval
- First hour: explain what you built this week from memory without looking at code. Draw the architecture. Explain the loss function. If you can't, study it, close it, try again.
- Second hour: recursive gap filling on the hardest concept from the week. Once the model is shipped, research for project #2 — what are the key concepts? Use AI to explain the intuition.

#### 🔄 Sunday — Catch-up buffer
- If you missed any day this week, do that work now. If nothing was missed, do extra project work or extra LeetCode.

### Milestones (must be true before Phase 2)

- All tools from section 4.2 are installed and working (Python env, PyTorch, Docker, Git, VS Code, experiment tracking, Notion)
- Rec sys demo is live and accessible via URL that anyone can click
- README explains the problem, setup, model, and design tradeoffs with architecture diagram
- Can explain how the model works, why you chose the architecture, and what tradeoffs you made — from memory, without notes
- Experiment tracking is logging runs with metrics
- Have done HackerRank/LeetCode easy problems across ALL major data structures (arrays, linked lists, stacks, queues, hash maps, trees, graphs, heaps)
- Have reached out to at least 6 people on LinkedIn (not necessarily gotten responses)
- Have had at least 2 actual coffee chat conversations (not just sent DMs)
- Notion daily tracking has entries for every work day

---

## 🚀🎯 Phase 2 (May-Jul) PORTFOLIO + SECOND DEMO + BUILDING WITH AGENTS + SYSTEM DESIGN

Build portfolio website. Scope and build highly ambitious project #2 as a live demo. Start studying system design. Level up AI-augmented development — the method of building becomes a learning objective itself.

### Weekly Activities

#### 🛠️ Monday, Tuesday, Wednesday — Project (Built with Agentic Workflows)
- Scope second project: (1) Highly ambitious ML project with live demo, (2) A/B testing platform, or (3) product analytics with causal inference
- Build project #2's core ML component. Same standards as project #1: config-driven, experiment tracking, proper splits, type hints, clean code.
- **Build this project using sophisticated agentic workflows, not just chatting with AI:**
  - Set up Claude Code and Codex with custom skills, hooks, and MCP servers tailored to project #2's domain (e.g., a skill for running experiments, a skill for evaluating model output, a hook that auto-lints on save)
  - Delegate work to OpenClaw
  - Use worktree-based parallel agent workflows — spin up multiple branches with agents working on independent features simultaneously, then merge
  - Get agents writing type-checked, tested code from the start — configure type hints, pytest, and linting as non-negotiable agent outputs, not afterthoughts
  - Build custom MCP servers or tools that accelerate development (e.g., a tool that queries your W&B runs, a tool that fetches dataset stats)
  - Practice context engineering: craft CLAUDE.md files, skill prompts, and project-level instructions that make agents productive without hand-holding
  - Set up Greptile or similar AI code review on every PR — get feedback on code quality, patterns, and potential issues even without a human reviewer
- Go line by line through any AI-generated code. Understand every layer. Recursive gap filling on anything unclear.
- Feature engineering, hyperparameter tuning, evaluation. Beat the baseline by a meaningful margin.
- Document what you tried and why it worked or didn't
- Build demo and deploy: FastAPI or Streamlit, Docker, cloud deployment, working URL
- Write README with architecture diagram and design tradeoffs
- Add a "How I Built This" section to README or portfolio documenting your agentic workflow — what skills/tools you created, how you orchestrated agents, what context engineering decisions you made. This is the differentiator Sajjaad and Casey described.
- Start system design study: read 1 chapter of Grokking System Design or do 1 lesson on educative.io

#### 🤝 Thursday — Networking
- Post 2x/week about project #2 progress and concepts you're learning on LinkedIn and X
- Post about your AI-augmented development workflow — what tools you built, how agents accelerated your work. This content stands out because most people just use AI passively.
- Continue weekly coffee chat outreach — now you have 2 real demos to show people
- Start reaching out to slightly harder targets: engineers and technical leads at companies you actually want to work at
- Build portfolio website once project #2 demo is live — simple personal site linking both demos, GitHub repos, and a short bio. This becomes the single link to send to 500 people (Gabriel's advice).

#### 🧩 Friday — HackerRank / LeetCode / DSA
- Start mixing in medium problems
- Focus on common patterns: two pointers, sliding window, BFS/DFS, binary search, dynamic programming basics
- When stuck for 1-2 hours, look at the solution on geeksforgeeks.org, then close it and redo it yourself (Ray Fu's method)

#### 🧠 Saturday — Research + Retrieval
- First hour: active recall on project #2 code and concepts
- Second hour: alternate weeks between (1) system design practice — pick a system ("design a recommendation feed," "design Uber") and sketch the architecture in Excalidraw, practice explaining it out loud, and (2) agent workflow practice — experiment with multi-agent orchestration patterns, build a new skill or MCP server, try a new context engineering technique, study how production teams use agentic tools

#### 🔄 Sunday — Catch-up buffer

### Milestones (must be true before Phase 3)

- Project #2 demo is live and accessible via URL
- Both projects have READMEs with architecture diagrams and design tradeoffs
- Can explain both projects from memory — model, architecture, tradeoffs, what you'd do differently
- Portfolio website is live with links to both demos
- Have completed at least 10 medium HackerRank/LeetCode problems
- Can sketch a basic system design (load balancer, app servers, database, cache) and explain each component
- Have had at least 4 total coffee chats since Phase 1
- Can demonstrate a sophisticated agentic development workflow: custom skills, MCP servers, multi-agent orchestration, and context engineering — and explain the decisions behind it

---

## 🏗️⚡ Phase 3 (Aug-Sep) INTERVIEW PREP + REFERRAL PUSH

Get interview-ready. Reach out to EVERYONE in the referral list. Start mock interviews.

### Weekly Activities

#### 🛠️ Monday, Tuesday, Wednesday — Project + Interview Prep
- Start a third project or improve existing ones (add features, improve performance, add tests, polish demos)
- Active GitHub commits during this period show you're still building while applying
- System design practice: 1 full design exercise per week in Excalidraw ("design Netflix recommendations," "design a URL shortener," "design a real-time chat app"). Cover scalability, availability, reliability, CAP theorem.
- Practice explaining both projects as if in an interview — time yourself, 3-5 minutes per project. Include: problem, approach, architecture, tradeoffs, results, what you'd do differently.
- Practice behavioral stories tied to company values (Amazon: customer obsession. Google: impact at scale. Meta: move fast.)
- Mock interviews with Casey, Griffin, Marco every 2 weeks

#### 🤝 Thursday — Networking (REFERRAL PUSH)
- **This is the most important networking period of the entire plan.**
- Reach out to ALL people in the referral list for real conversations: Taylor (Google Cloud), Casey Brown, Olivia Gagan (Fidelity), Nishanth (Citadel), Greg Schafer (Scale.ai), Marco, Griffin, Liam Kaufman, Mario, Jonathan Parra, Jai Senthil Kumar, Sebastian Sepulveda
- Show them your portfolio site and demos. At the end of each conversation, ask: "Would you be down to give me a referral for the upcoming spring co-op cycle?"
- Continue posting 2x/week on LinkedIn, X, and GitHub about your interview prep journey
- Apply to 1-2 companies you don't care about for real interview reps — this is practice, not the real push (Prime's advice)

#### 🧩 Friday — HackerRank / LeetCode / DSA
- Ramp up to 4-5 problems per session
- Focus on medium problems and common patterns: dynamic programming, graph problems, tree traversals, string manipulation
- Goal is pattern recognition: see a problem, know which approach to use

#### 🧠 Saturday — Research + Retrieval
- First hour: active recall on interview topics. Can you explain system design components from memory? Can you walk through your projects without notes?
- Second hour: research target companies. Read their engineering blogs, understand what teams work on, identify which roles match your skills.

#### 🔄 Sunday — Catch-up buffer

### Milestones (must be true before Phase 4)

- Have done at least 4 mock interviews (behavioral + technical)
- Can explain both projects fluently in 3-5 minutes each without notes
- Can design a system on Excalidraw and explain it in 15-20 minutes
- Have completed at least 30 medium HackerRank/LeetCode problems total
- Have reached out to ALL people on the referral list
- Have at least 3 confirmed referrals lined up for applications
- Have prepared 3-4 behavioral stories tied to target company values
- Have done 1-2 throwaway interviews at companies you don't care about

---

## 📨🎯 Phase 4 (Oct-Nov) ACTIVE APPLICATIONS

Apply to spring 2027 co-ops with referrals. Interview. Get offers.

### Weekly Activities

#### 🛠️ Monday, Tuesday, Wednesday — Project + Interview Prep
- Keep building or improving projects between interviews. Active GitHub commits show you're still working.
- Fix anything that came up during interviews ("we noticed your demo doesn't handle X"). Polish demos.
- Drill weak areas exposed by real interviews — if system design was weak, do more Excalidraw. If LeetCode was weak, target that pattern.
- After every interview, write down what went well and what you struggled with. Fix the weak spots immediately.
- Practice company-specific question types: Amazon (leadership principles + system design), Google (LeetCode + system design), Meta (LeetCode + system design + behavioral), OpenAI (technical depth + LeetCode)
- Continue mock interviews with Casey, Griffin, Marco — keep drilling weak areas exposed by real interviews
- Practice explaining technical concepts to non-technical friends (Maddy Zhang's advice) — this directly preps for behavioral rounds where you explain your projects to non-ML interviewers

#### 🤝 Thursday — Networking
- Apply to target companies WITH referrals: Amazon, Meta, Google, Uber, OpenAI, Anthropic, xAI, Scale.ai, Airbnb, Intuit, Adobe, LinkedIn
- Apply to no more than 2 roles per company (Amazon cooldown is 6-24 months if you bomb one)
- Message the specific recruiter assigned to each role on LinkedIn — link the role, explain your qualifications (Yvonne's advice)
- Ask recruiters if the company has resources to help you pass the online assessment
- Use Northeastern career services for resume review and interview prep
- Check NUWorks for spring 2027 co-op postings
- Post 2x/week on LinkedIn and X about your application journey
- Contribute to 1-2 open source ML projects (PyTorch, Hugging Face, or Ray) — fix bugs, engage with maintainers on Discord. This builds real codebase experience (reading other people's code, code review, debugging) and looks great on a resume (Maddy Zhang's advice re: Google Summer of Code)

#### 🧩 Friday — HackerRank / LeetCode / DSA
- Maintain sharpness. Continue medium problems, attempt 1-2 hard problems per week.
- Focus on problems similar to what you've seen in real interviews

#### 🧠 Saturday — Research + Retrieval
- First hour: active recall
- Second hour: research companies you're interviewing with next week. Read their engineering blogs, recent product launches, team structures.

#### 🔄 Sunday — Catch-up buffer

### Milestones (must be true before Phase 5)

- Have applied to at least 8 target companies with referrals
- Have completed at least 4 real interviews
- Have written post-interview notes for every interview identifying weak areas
- Have a system for tracking application status (applied, phone screen, onsite, offer, rejected)
- HackerRank/LeetCode total: at least 50 medium + 5 hard problems completed
- Have made at least 1 meaningful open source contribution (merged PR or active engagement with maintainers)

---

## 🏆🎉 Phase 5 (Dec-Jan) SECURE OFFER + PREP FOR DAY 1

Accept an offer. Prepare to hit the ground running on day 1.

### Weekly Activities

#### 🛠️ Monday, Tuesday, Wednesday — Co-op Prep
- Final interview rounds if still in process
- If offer accepted: ask recruiter to connect you with your future manager. Get on a 1-on-1 call to learn what you'll work on and what tools/frameworks the team uses (Sajjaad's advice).
- If the team uses unfamiliar tools (Spark, Kafka, internal frameworks), take a targeted Coursera course or build a small project with it — just enough to not be lost on day 1
- Read about the company's principles, mission, and recent technical blog posts. Understand what your team ships and how they measure success (Maddy Zhang's advice).
- Only negotiate salary with a competing offer for internships (Sajjaad's advice)

#### 🤝 Thursday — Networking
- Thank everyone who gave you referrals, regardless of outcome. Update them on where you landed. These relationships matter for the rest of your career.
- Post about landing the co-op on LinkedIn and X — this closes the loop on the "building in public" story
- Connect with future teammates on LinkedIn if possible

#### 🧩 Friday — HackerRank / LeetCode / DSA
- Maintenance mode. 2-3 problems to stay sharp. These skills atrophy if you stop completely.

#### 🧠 Saturday — Research + Retrieval
- Review what you've learned about the team's stack
- Practice explaining your projects one more time — you'll likely be asked about them by new teammates

#### 🔄 Sunday — Catch-up buffer

### Milestones (end of plan)

- Have accepted a co-op/internship offer for spring 2027
- Have spoken with future manager and know what team/tools to expect
- Have studied any unfamiliar tools the team uses
- Have read the company's engineering blog and understand the team's domain
- Start co-op in January 2027
- On day 1: document everything you build and its impact from the start — this is how you get a return offer or promotion (Ray Fu's advice)
- Ask your manager to review your code on calls and show appreciation for every comment — this gets you more and better feedback (Gabriel's advice)
