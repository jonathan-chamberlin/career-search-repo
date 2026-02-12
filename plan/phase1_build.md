# 🧱🔨 Phase 1 (Feb-Jul) BUILD

Build two projects and ship both as live demos anyone can access via URL. Mon-Tue: write code yourself with /professor-mode as tutor. Wed-Thu: extend the same project with Claude Code. Begin the HackerRank and networking pipelines. Start system design study.

## Project #1: Recommendation System (Feb-Apr target)

### Mon-Tue Raw Coding Tasks
- Set up rec sys project repo with folder structure (src/, tests/, configs/, scripts/, app/)
- Download Goodreads-10K dataset (10K books, 53K users, 6M ratings), explore distributions (rating counts, user activity, genre spread)
- Implement data loading pipeline: PyTorch Dataset and DataLoader for user-item interactions
- Implement train/validation/test split BY USER (not by rating — this tests generalization to new users)
- Set up YAML config for all hyperparameters (embedding dim, learning rate, batch size, negative sampling ratio)
- Implement and evaluate baseline models: Random recommender, Popularity-based recommender (NDCG@10, Hit Rate@10, MRR)
- Start Two-Tower model: User Tower (interaction history → user embedding) + Item Tower (item features → item embedding) + dot product scoring
- Implement training loop with BPR loss (pairwise ranking loss) and negative sampling with popularity weighting
- Train on Goodreads training set, validate on validation set, beat baselines by meaningful margin
- Debug things yourself before asking AI — build the debugging muscle
- Recursive gap filling: PyTorch Dataset/DataLoader, NDCG computation, embedding layers, BPR loss derivation, Two-Tower vs NCF vs Matrix Factorization tradeoffs

### Wed-Thu AI-Augmented Tasks
- Set up Weights & Biases experiment tracking, log all runs with metrics and hyperparameters
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

## Project #2: Ambitious Second Demo (Apr-Jul target)

### Scoping
- Scope second project: (1) Highly ambitious ML project with live demo, (2) A/B testing platform, or (3) product analytics with causal inference
- Same standards as project #1: config-driven, experiment tracking, proper splits, type hints, clean code

### Mon-Tue Raw Coding Tasks
- Build the core ML component by hand — model architecture, training loop, evaluation pipeline
- Feature engineering, hyperparameter tuning, evaluation. Beat the baseline by a meaningful margin.
- Document what you tried and why it worked or didn't

### Wed-Thu AI-Augmented Tasks
- Use Claude Code to refactor, add tests, build API/frontend, deploy
- Go line by line through any AI-generated code. Understand every layer. Recursive gap filling on anything unclear.
- Build demo and deploy: FastAPI or Streamlit, Docker, cloud deployment, working URL
- Write README with architecture diagram and design tradeoffs
- Build portfolio website once project #2 demo is live — simple personal site linking both demos, GitHub repos, and a short bio. This becomes the single link to send to 500 people (Gabriel's advice).
- Start system design study: read 1 chapter of Grokking System Design or do 1 lesson on educative.io per week

## Friday — Networking / Posting
- Send 2-3 LinkedIn connection requests to Northeastern alumni at target companies (find via linkedin.com/school/khoury-college/people/)
- Message 1 person/week for a coffee chat using Nishanth's DM templates in 1metalearning.md
- Write and publish 1-2 posts/week across LinkedIn, X, and GitHub about what you're learning or building
- Goal early in this phase: build relationships. Do NOT ask for referrals yet.
- Once the rec sys ships: post about it on LinkedIn and X — what you built, what you learned, one interesting technical challenge
- Continue weekly coffee chat outreach (message 1 new person, follow up with existing conversations)
- Research and sign up for end-of-semester Khoury career events and employer panels — bring your demo
- Investigate joining AINU when applications open next fall
- Start reaching out to slightly harder targets: engineers and technical leads at companies you actually want to work at

## Saturday — LeetCode / HackerRank / DSA
- First few Saturdays: learn data structures visually on csvistool.com (arrays, linked lists, stacks, queues, hash maps, trees, graphs, heaps)
- Start on HackerRank first — use the Interview Preparation Kit and 1-Month Preparation Kit. HackerRank uses raw stdin/stdout parsing which is different from LeetCode's pre-parsed inputs; 3,000+ companies (Amazon, Goldman Sachs, Bloomberg, Adobe, Uber) use HackerRank as their actual screening tool
- Do 2-3 easy problems per session, one data structure per Saturday
- Also do HackerRank's SQL track — SQL appears in 33% of target roles and 89% of DS Consumer roles. Write queries against the Goodreads dataset too: practice joins, aggregations, window functions on the ratings/books/users tables
- Track which data structures you've covered
- By mid-phase, should have covered ALL major data structures at least once
- Transition to LeetCode for deeper algorithm pattern mastery — company-tagged problems (Premium), Blind 75, NeetCode 150
- Start recognizing patterns: "this is a two-pointer problem," "this needs a hash map"
- Start mixing in medium problems: two pointers, sliding window, BFS/DFS, binary search, dynamic programming basics
- When stuck for 1-2 hours, look at the solution on geeksforgeeks.org, then close it and redo it yourself (Ray Fu's method)

## Sunday — Catch-up Buffer
- If you missed any day this week, do that work now. If nothing was missed, do extra project work or extra LeetCode.

## Milestones (must be true before Phase 2)

- Rec sys demo is live and accessible via URL that anyone can click
- Project #2 demo is live and accessible via URL
- Both projects have READMEs with architecture diagrams and design tradeoffs
- Can explain both projects from memory — model, architecture, tradeoffs, what you'd do differently — without notes
- Portfolio website is live with links to both demos
- Experiment tracking is logging runs with metrics
- Have done HackerRank/LeetCode problems across ALL major data structures, with at least 10 medium problems completed
- Can sketch a basic system design (load balancer, app servers, database, cache) and explain each component
- Have reached out to at least 10 people on LinkedIn
- Have had at least 4 actual coffee chat conversations
- Notion daily tracking has entries for every work day
