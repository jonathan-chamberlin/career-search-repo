# Metalearning Worksheet: Learning How to Learn ML Engineering

*"Before diving in, research how ML engineering is best learned and what the most important sub-skills are."*

---

## Target Roles (Job Categories I'm Pursuing)

1. **Machine Learning Engineer** - Building and deploying ML models at scale
2. **ML Engineer (Recommendation Systems)** - Personalization, ranking, and user modeling
3. **Data Scientist (Consumer)** - A/B testing, causal inference, product analytics
4. **Data Scientist (ML)** - Research-focused, deep learning, publishing papers

*These are the 4 job categories I'm optimizing for. All skills analysis and learning priorities below are based on job postings in these categories.*

---

**Time Investment:** Spend 5-10% of your total learning time on metalearning. For a 400-hour learning project, that's ~20-40 hours upfront.

**Date Started:** _______________
**Date Completed:** _______________

---

## Part 1: WHY - Clarifying Your Motivation

Understanding your motivation helps you prioritize what to learn and stay committed when things get hard.

### 1.1 Instrumental vs. Intrinsic Motivation

**Question:** Are you learning ML engineering primarily for an outcome (instrumental) or for the joy of learning itself (intrinsic)?

- [] Primarily instrumental (career, money, specific job)
- [ ] Primarily intrinsic (fascination with the field)
- [X] Both equally

**Your answer (explain):**
- ultimately i want to make $270k/year because this wod let me realistically save $50,000 for a bimax surgery in only 5 months.

### 1.2 Define Your Concrete Goal

**Question:** What specific outcome do you want? Be as precise as possible.

- **Job title you want:**
  -ML Engineer or Data Scientist (ML or Consumer)
- **Company type (startup/FAANG/research lab):**
  -Ultimately I want to work at a FANNG or top tier public company, like Meta, Google, Apple, Netflix, OpnAI, Anthropic, Perplexity, Airbnb, Intuit, Tesla, Amazon, Microsoft, Adobe, Linkedin, etc.
- **Salary range target:**
  - Eventually I want to hit $270k/year total comp.
- **Location/remote preference:**
  - Ideally San Francisco, LA, or remote.
- **Timeline to achieve this:**
  - By 1 year after graduation, or May 2029.

### 1.3 Why This Path?

**Question:** Why ML engineering or Data Science (ML or Consumer) specifically, rather than other tech roles?
- Because I already built 2 machine learning projects, agent-organism and lunar-lander, and had lots of fun making them. Additionally, for years I have really enjoyed tracking data. 

Data engineering, VR / immersive tech don't sound too interesting. AI engineering seems like something I would get good at naturally because I could integrate stuff to improve the products and systems I create. 

Robot Learning (ML Engineer for Robotics) has too high a barrier to entry - most roles require a PhD or 3-6+ years of experience deploying ML to physical robots, which I don't have. 

**Question:** What would you do if ML engineering jobs disappeared tomorrow?
- I would do analytics engineering. I could get really good at that since I've really enjoyed tracking and working with data my whole life. But it pays less than the ML engineering or DS roles.

*Suggestion: If your answer reveals a deeper interest (e.g., "I'd still want to build intelligent systems"), note that—it reveals your true motivation.*

---

## Part 2: WHAT - Mapping Knowledge Structure

Break down ML engineering & Data Science into concepts, facts, and procedures.

### 2.1 Concepts (Things to Understand Deeply)

Concepts require flexible understanding—you need to grasp the "why" and apply them in novel situations.

**Instructions:** For each concept, note your current level (1=none, 5=expert), priority (H/M/L), and any notes.

---

**1. Software Engineering Foundations** *(Learn first — prerequisite for everything)*
- **Object oriented programming**
  - Current level: Beginner
  - Priority: Fundamental
  - Notes: I used classes in my lunar lander project a bit so I do understand it to an extent. But I'd have trouble if I wrote it by hand.
- **Debugging**
  - Current level: Low. 
  - Priority: Fundamental
  - Notes: I have not really had to debug stuff since I just had AI fix it for me.
- **Deep Learning fundamentals**
  - Current level: medium
  - Priority: Fundamental
  - Notes: Did DDPG in agent-organism repo and TD3 in lunar-lander repo.
- **Loss functions & optimizers (SGD, Adam, learning rate schedules)**
  - Current level: Medium-low
  - Priority: Idk how important this is the machine learning
  - Notes: I used this in my lunar-lander repo.
- **Regularization techniques (dropout, batch norm, L1/L2)**
  - Current level: Idk what this is so 0
  - Priority:
  - Notes:
- **Hyperparameter tuning strategies**
  - Current level: Medium
  - Priority: Medium
  - Notes: In my lunar-lander I had a claude skill that had it setup and test hyperparameters and keep the highest ones.
- **Transfer learning / fine-tuning**
  - Current level: 0
  - Priority: Idk what this is
  - Notes:
- **Neural network architectures (CNNs, RNNs, Transformers)**
  - Current level: 0 
  - Priority: Idk what this is 
  - Notes:
- **Attention mechanisms**
  - Current level: 0 
  - Priority: Idk what this is 
  - Notes:
- **Bias-variance tradeoff**
  - Current level: 0
  - Priority: Idk what this is
  - Notes:

**Domain Areas**
- **Recommendation Systems**
  - Current level: 0
  - Priority: H (core skill for ML Engineer Rec Sys roles)
  - Notes:
- **User Modeling / Personalization**
  - Current level: 0
  - Priority: H (5/7 rec sys listings)
  - Notes: Building short-term and long-term user interest models
- **Ranking Systems (CTR/CVR Prediction)**
  - Current level: 0
  - Priority: H
  - Notes: Click-through rate and conversion rate prediction models
- **Candidate Generation / Content Retrieval**
  - Current level: 0
  - Priority: M
  - Notes: First stage of recommendation pipeline - retrieving candidates
- **Approximate Nearest Neighbors (ANN)**
  - Current level: 0
  - Priority: M
  - Notes: Efficient similarity search for recommendations at scale
- **NLP / Transformers**
  - Current level: 0
  - Priority: I'm not very interested in NLP specifically
  - Notes:
- **Computer Vision**
  - Current level: 0
  - Priority: Intuitively I'm more interested in RL learning, I know because I already did this, and recommendation systems (but that one I don't know because I've never tried it before).
  - Notes:
- **Reinforcement Learning**
  - Current level: Medium
  - Priority: idk
  - Notes: I've already done two projects with simulations using RL, one was a discrete environemnt I coded from scratch mostly by myself, another was a continuous environement which I vibe coded.

**ML Engineer Concepts**
- **Distributed Training (DDP, FSDP, DeepSpeed)**
  - Current level: low
  - Priority:
  - Notes:
- **MLOps / CI-CD for ML**
  - Current level: 0
  - Priority:
  - Notes:
- **HPC Infrastructure**
  - Current level: 0
  - Priority:
  - Notes:
- **Model Optimization**
  - Current level: low-medium
  - Priority:
  - Notes:
- **Model serving / inference optimization**
  - Current level: 0
  - Priority:
  - Notes:
- **Batch vs real-time inference**
  - Current level: 0
  - Priority:
  - Notes:
- **Model monitoring (drift detection, performance decay)**
  - Current level: 0
  - Priority:
  - Notes:
- **Data pipelines for ML**
  - Current level: 0
  - Priority:
  - Notes:

**Data Scientist (Consumer) Concepts**
- **A/B Testing & Experimentation**
  - Current level: medium
  - Priority:
  - Notes: I did A/B testing in my lunar-lander project, hyperparameter tuning
- **Causal Inference**
  - Current level: 0 
  - Priority:
  - Notes:
- **Statistical hypothesis testing**
  - Current level: medium
  - Priority:
  - Notes: I did this in my lunar lander project
- **Experiment design**
  - Current level: medium
  - Priority:
  - Notes: Did in my lunar lander project
- **Feature engineering**
  - Current level: 0 
  - Priority:
  - Notes:
- **Data Visualization & Storytelling**
  - Current level: medium
  - Priority:
  - Notes: I did this in my sales org project and my uber-trips-analysis project.

**Research/Advanced (DS-ML)**
- **Generative Models (GANs, VAEs, Diffusion models)**
  - Current level: 0
  - Priority:
  - Notes:
- **Self-supervised learning**
  - Current level: 0
  - Priority:
  - Notes:
- **LLM fine-tuning (LoRA, RLHF)**
  - Current level: 0
  - Priority:
  - Notes:
- **Research Methods & Paper Reading**
  - Current level: 0
  - Priority:
  - Notes:

**System Design**
- **ML system design patterns**
  - Current level: low
  - Priority:
  - Notes:
- **Latency vs throughput tradeoffs**
  - Current level: 0
  - Priority:
  - Notes:
- **Scalability for ML systems**
  - Current level: 0
  - Priority:
  - Notes:

**Interview & Problem-Solving**
- **Data structures and algorithms**
  - Current level: 1
  - Priority:
  - Notes:
- **Problem-solving principles (pattern recognition, not giving up)**
  - Current level: 2-3
  - Priority:
  - Notes:

**Software Engineering**
- **Context efficiency**
  - Current level: medium
  - Priority:
  - Notes:
- **Version control (worktrees, PRs, pushing)**
  - Current level: low-medium
  - Priority:
  - Notes:
- **Object oriented programming**
  - Current level: low-medium
  - Priority:
  - Notes:
- **CLIs**
  - Current level: 0
  - Priority:
  - Notes:
- **MCPs**
  - Current level: low
  - Priority:
  - Notes:
- **Deployment & hosting**
  - Current level: low
  - Priority:
  - Notes:
- **Agents calling subagents**
  - Current level: 0
  - Priority:
  - Notes:
- **IDEs (VS Code, Cursor, etc.)**
  - Current level: low-medium
  - Priority:
  - Notes:
- **AI coding assistants (Claude Code, Cursor, Codex)**
  - Current level: medoium
  - Priority:
  - Notes:
- **Code review**
  - Current level: almost 0
  - Priority:
  - Notes:
- **Design choices at beginning of project**
  - Current level: low
  - Priority:
  - Notes:
- **Cloud computing**
  - Current level: 0
  - Priority:
  - Notes:
- **Type checking & type safety**
  - Current level: 0
  - Priority:
  - Notes:

**(Add your own)**
-
  - Current level:
  - Priority:
  - Notes:

**Question:** Which 3 concepts will be hardest for you to learn? Why?

1. **Hardest concept:** ML Ops.
   - Why: I have no experience deploying stuff.
2. **Second hardest:** Recommendation Systems
   - Why: I've no experience with this either.
3. **Third hardest:** Code Review
   - Why: Requires me to have a level of understandiung of the code I read

### 2.2 Facts (Things to Memorize)

Facts are information you need to recall without derivation. All of the following:

- [ ] **Framework comparisons:** PyTorch vs TensorFlow vs JAX (when to use each)
- [ ] **Algorithm tradeoffs:** When to use DQN vs PPO vs SAC, etc.
- [ ] **Cloud services:** AWS vs GCP vs Azure equivalents
- [ ] **Tool purposes:** What Docker, Kubernetes, Airflow, MLflow each do
- [ ] **API patterns:** Common PyTorch/TensorFlow idioms
- [ ] **Acronyms:** DDP, FSDP, RLHF, RAG, MLP, CNN, RNN, etc.
- [ ] **Git terminology:** rebase, cherry-pick, worktrees, etc.
- [ ] **Security vulnerabilities:** Common ML attack vectors
- [ ] **LLM/Agent comparisons:** Use cases, strengths, and weaknesses of each LLM and agent
- [ ] **Programming language comparisons:** Use cases, strengths, and weaknesses of each programming language
- [ ] **Available tools:** Software, libraries, connections to improve workflows
- [ ] **Job positions:** Different roles and what they entail
- [ ] **Important skills:** List of skills and problems to solve according to founders, hiring managers, executives
- [ ] **npm:** What npm does
- [ ] **Type checking:** Best way to type check code
- [ ] **OOP terminology:** class, method, object, attribute

**Recommendation Systems Knowledge:**
- [ ] **RecSys architectures:** Two-tower models, multi-stage retrieval + ranking, real-time vs batch
- [ ] **Ranking metrics:** CTR, CVR, NDCG, MRR, diversity metrics
- [ ] **Cold start problem:** Solutions for new users and new items
- [ ] **Embedding techniques:** Matrix factorization, neural collaborative filtering, item2vec
- [ ] **Feature stores:** What Feast, Tecton, and other feature stores do
- [ ] **ANN algorithms:** HNSW, Faiss, ScaNN for approximate nearest neighbor search

**Books to study from:**
- [ ] Cracking the Coding Interview
- [ ] Programming Interviews in Python
- [ ] Grokking System Design

**Interview knowledge:**
- [ ] Big companies look for problem-solving (data structures & algorithms); startups look for software development skills
- [ ] Employees get paid for successful referrals
- [ ] Common LeetCode problem patterns and which data structure/algorithm to use

### 2.3 Procedures (Things to Practice Until Automatic)

Procedures are skills that require hands-on repetition.

**Instructions:** For each procedure, note your current ability (1-5) and priority (H/M/L).

**Languages & Frameworks**
- **Python (production-quality)**
  - Current ability: 3
  - Priority: H (11/11 listings)
- **C++**
  - Current ability: 1
  - Priority: M (6/11 listings)
- **PyTorch**
  - Current ability: 2
  - Priority: H (9/11 listings, preferred framework)
- **TensorFlow**
  - Current ability: 1
  - Priority: M (9/11 listings, but PyTorch preferred)
- **JAX**
  - Current ability: 1
  - Priority: L (rare in listings)
- **CUDA**
  - Current ability: 1
  - Priority: M (3/11 listings)

**DevOps & Infrastructure**
- **Docker containerization**
  - Current ability: 1
  - Priority:
- **Kubernetes deployment**
  - Current ability: 1
  - Priority:
- **Setting up cloud ML environments (AWS/GCP)**
  - Current ability: 1
  - Priority: M (3/7 rec sys listings mention AWS)
- **CI/CD pipeline creation**
  - Current ability: 1
  - Priority:
- **Distributed systems for ML**
  - Current ability:
  - Priority: H (6/7 rec sys listings)
- **Deep learning model training & deployment**
  - Current ability:
  - Priority: H (4/7 rec sys listings)

**Version Control & Tooling**
- **Git workflows (branches, PRs, merges)**
  - Current ability: 3
  - Priority:
- **Gitlab (version control used at many big companies)**
  - Current ability: 1
  - Priority:
- **Downloading repos**
  - Current ability: 1
  - Priority:
- **Copying remote files into a repo**
  - Current ability: 1
  - Priority:
- **Creating a new repo**
  - Current ability: 4
  - Priority:
- **Create a new worktree**
  - Current ability: 2
  - Priority:
- **Multiple worktrees with agents, then merging**
  - Current ability: 2
  - Priority:
- **Using VSCode (shortcuts, settings, tools, interface)**
  - Current ability: 2
  - Priority:

**ML Development**
- **Debugging ML models**
  - Current ability: 2
  - Priority:
- **Writing tests for ML code**
  - Current ability: 2
  - Priority:
- **Experiment tracking setup**
  - Current ability: 3
  - Priority:
- **Reading and implementing papers**
  - Current ability: 1
  - Priority:

**Recommendation Systems Development**
- **Building ranking models (CTR/CVR prediction)**
  - Current ability:
  - Priority: H (core rec sys skill)
- **User embedding / representation learning**
  - Current ability:
  - Priority: H (5/7 listings)
- **Real-time feature engineering**
  - Current ability:
  - Priority: M (2/7 listings)
- **Building candidate retrieval systems**
  - Current ability:
  - Priority: M
- **A/B testing for recommendations**
  - Current ability:
  - Priority: H (4/7 listings)
- **Working with Spark for large-scale data**
  - Current ability:
  - Priority: M (3/7 listings)
- **Building data pipelines for ML**
  - Current ability:
  - Priority: M (3/7 listings)
- **Causal inference for recommendation evaluation**
  - Current ability:
  - Priority: M (2/7 listings)

**AI-Augmented Development**
- **Agent workflows**
  - Current ability: 2
  - Priority:
- **Debugging agents**
  - Current ability: 3
  - Priority:
- **Getting agents to write type-checked code**
  - Current ability: 1
  - Priority:
- **Code review with Greptile**
  - Current ability:1
  - Priority:

**Portfolio & Documentation**
- **Writing a great README**
  - Current ability:2
  - Priority:
- **Creating a compelling portfolio**
  - Current ability:2
  - Priority:
- **Documenting what you build and its impact (for promotions)**
  - Current ability:1
  - Priority:

**Networking & Job Search**
- **Reaching out for coffee chats**
  - Current ability:2
  - Priority:
- **Contributing to existing codebases**
  - Current ability:1
  - Priority:
- **Being useful in programmer discords (providing solutions/resources)**
  - Current ability:1
  - Priority:
- **Spending time in GitHub issues tab**
  - Current ability:1
  - Priority:
- **Answering questions in Theo's discord or on X**
  - Current ability:1
  - Priority:
- **Attending conferences and job fairs**
  - Current ability:3
  - Priority:
- **Outreach to recruiters**
  - Current ability:2
  - Priority:
- **Asking for referrals from network**
  - Current ability:2
  - Priority:
- **Connecting with software engineers on LinkedIn**
  - Current ability:1
  - Priority:
- **Building and posting about your journey online (post twice/week on LinkedIn)**
  - Current ability:2
  - Priority:

**Interview Prep**
- **Mock interviews with people who got the job or hire others**
  - Current ability:1
  - Priority:
- **LeetCode problems (work 1-2 hours, look at solution, redo yourself)**
  - Current ability:1
  - Priority:
- **System design practice using Excalidraw or Lucidchart ("design Airbnb")**
  - Current ability:2
  - Priority:

### 2.4 What do you already know?
- I'm already comfortable with statistics, linear algebra, calculus, algebra, artihmatic, and probability.


---

## Part 3: HOW - Research Learning Methods

### 3.1 The Benchmark Method

Research how others successfully learned ML engineering.

#### University Curricula

**Question:** What do top ML programs (Stanford CS229, CMU ML, MIT) teach and in what order?

- **Stanford CS229:** [cs229.stanford.edu](https://cs229.stanford.edu/)
  - **Course progression:**
    1. Supervised Learning (LMS, Logistic Regression, SVMs, Neural Networks)
    2. Learning Theory (Bias/Variance tradeoffs, practical debugging advice)
    3. Deep Learning (Neural Networks, Backpropagation, Vectorization)
    4. Unsupervised Learning (K-means, EM, PCA, ICA)
    5. Reinforcement Learning (MDPs, Q-learning, Policy Search)
  - **Strengths:** Taught by Andrew Ng (original); strong mathematical foundations; covers theory AND practical debugging advice; excellent lecture notes freely available; gold standard for ML fundamentals
  - **Weaknesses:** Graduate-level math heavy (requires linear algebra, probability, calculus); detailed syllabus restricted to Stanford students; less focus on modern deep learning compared to specialized courses
  - **Source:** [Stanford Engineering Everywhere](https://see.stanford.edu/course/cs229), [CS229 Lecture Notes](https://cs229.stanford.edu/main_notes.pdf)

- **CMU ML:** [ml.cmu.edu](https://www.ml.cmu.edu/academics/machine-learning-masters-curriculum)
  - **Course progression (Master's curriculum):**
    1. 10-701 Intro to ML OR 10-715 Advanced Intro to ML
    2. 10-617 Intermediate Deep Learning OR 10-703 Deep RL OR 10-707 Advanced Deep Learning
    3. 10-708 Probabilistic Graphical Models
    4. 10-718 Machine Learning in Practice
    5. 10-725 Optimization for Machine Learning
    6. 36-700/705 Probability and Statistics
    + 3 electives + practicum/internship
  - **Strengths:** Dedicated ML department (not just CS); rigorous theory (10-715 prepares for research); strong probabilistic/Bayesian focus; required practicum ensures real-world experience
  - **Weaknesses:** 10-715 is PhD-level intensity ("HEAVY and FAST"); requires strong prerequisites (algorithms, linear algebra, probability); less accessible for self-study
  - **Source:** [CMU ML Masters Curriculum](https://ml.cmu.edu/academics/machine-learning-masters-curriculum), [10-715 Course Page](https://www.cs.cmu.edu/~epxing/Class/10715/about.html)

- **MIT 6.036/6.867:** [ocw.mit.edu](https://ocw.mit.edu/courses/6-036-introduction-to-machine-learning-fall-2020/)
  - **Course progression:**
    1. 6.036 Intro to ML (undergrad): Classification, regression, neural networks, reinforcement learning, clustering, recommender systems
    2. 6.867 Machine Learning (grad): Deeper theory - boosting, SVMs, HMMs, Bayesian networks
    3. 6.862 Applied ML (grad): Same as 6.036 + semester project
  - **Strengths:** Freely available on MIT OpenCourseWare; taught by Leslie Kaelbling (RL pioneer); good balance of theory and application; undergraduate accessible (6.036)
  - **Weaknesses:** 6.867 materials are older (2006); less comprehensive than Stanford/CMU for production ML; graduate courses restricted
  - **Source:** [MIT OCW 6.036](https://ocw.mit.edu/courses/6-036-introduction-to-machine-learning-fall-2020/), [MIT Open Learning Library](https://openlearninglibrary.mit.edu/courses/course-v1:MITx+6.036+1T2019/about)

- **Key takeaways:**
  - All programs start with supervised learning fundamentals before unsupervised/RL
  - Math prerequisites are consistent: linear algebra, probability, calculus, algorithms
  - Stanford CS229 is best for self-study (free materials); CMU is most rigorous; MIT most accessible
  - None focus heavily on MLOps/production - that requires separate coursework

#### Online Courses

**Question:** What are the most recommended courses/resources? (FastAI, Coursera, etc.)

- **Course 1: Machine Learning Specialization (Andrew Ng / Stanford / Coursera)**
  - Link: [coursera.org/specializations/machine-learning-introduction](https://www.coursera.org/specializations/machine-learning-introduction)
  - What it covers: 3-course specialization covering supervised learning (regression, classification, neural networks), unsupervised learning (clustering, anomaly detection), recommender systems, and reinforcement learning. Rebuilt in 2022 with Python/TensorFlow (previously MATLAB).
  - Recommended by: Universally recommended as THE starting point for ML beginners; Andrew Ng is co-founder of Coursera and former Google Brain/Baidu AI lead
  - Your interest (1-5):

- **Course 2: Deep Learning Specialization (Andrew Ng / DeepLearning.AI / Coursera)**
  - Link: [coursera.org/specializations/deep-learning](https://www.coursera.org/specializations/deep-learning)
  - What it covers: 5-course specialization - Neural Networks basics, Improving Deep Neural Networks (hyperparameter tuning, regularization, optimization), Structuring ML Projects, CNNs, Sequence Models (RNNs, LSTMs, Transformers). Rated 4.9/5 by 120K+ learners.
  - Recommended by: Industry standard for deep learning foundations; prepares you to "set technical direction for an AI team"
  - Your interest (1-5):

- **Course 3: Practical Deep Learning for Coders (FastAI)**
  - Link: [course.fast.ai](https://course.fast.ai/)
  - What it covers: 9 lessons (~90 min each) covering computer vision, NLP, tabular data using PyTorch + fastai library. Top-down approach: build working models first, then learn theory. Part 2 covers diffusion models, DDPM/DDIM, Dreambooth.
  - Recommended by: FastAI alumni have gone to Google Brain, OpenAI, Adobe, Amazon, Tesla; published at NeurIPS. Free, no special hardware needed. Best for "learn by doing" style.
  - Your interest (1-5):

- **Course 4: Full Stack Deep Learning**
  - Link: [fullstackdeeplearning.com](https://fullstackdeeplearning.com/)
  - What it covers: MLOps and production ML - infrastructure/tooling, data management, experiment tracking, model deployment, monitoring, CI/CD, ML team organization. Teaches how to build AI-powered products end-to-end.
  - Recommended by: Started as UC Berkeley bootcamp; fills the gap between "train a model" and "deploy to production"; free and open
  - Your interest (1-5):

- **Course 5: MLOps Zoomcamp (DataTalks.Club)**
  - Link: [datatalks.club/blog/mlops-zoomcamp.html](https://datatalks.club/blog/mlops-zoomcamp.html)
  - What it covers: Free 3-month hands-on MLOps course - Docker, AWS, MLflow experiment tracking, Mage orchestration, model deployment (batch/real-time/streaming), Prometheus + Evidently monitoring, CI/CD. Community-driven with peer support.
  - Recommended by: Highly practical, project-based; all materials on GitHub; good for learning deployment skills missing from academic courses
  - Your interest (1-5):

- **Course 6: Made With ML**
  - Link: [madewithml.com](https://madewithml.com/)
  - What it covers: End-to-end ML system development - connects MLOps components (tracking, testing, serving, orchestration) as you build a complete system. Focus on going from development to production with mature CI/CD workflows.
  - Recommended by: Created by Goku Mohandas; practical focus on production ML; free and open-source
  - Your interest (1-5):

#### Practitioner Interviews

**Question:** Find 3-5 ML engineers on LinkedIn/Twitter with jobs you want. What was their path?

- **Person 1:**
  - Name/handle: Ray Fu
  - Current role:
  - Their learning path: He had a friend who he hungout with everyday who already did technical interviews, and they would code together (I could do this with Kenny).
  - Key insights:
    - They said books like Cracking the Coding Interview and Programming Interviews in Python
    - Mock Interviews with People who got the job or hire other people (I could use Casey for this, or Griffin or Marco [ I'd have to find their instas or get their numbers from Matt]).
    - He says the biggest thing is asking people in your network for referals. Remember that employees get paid if they refer someone who gets hired. I could ask Olivia Gagan for a referal, or if there is a software engineer I could get an introduction to to have a coffee chat with. A secondary tactic is going to linkedin, searching 'software engineer' then connecting with as many as possible. 
    - Sending your resumes to application sites doesn't really work because there are 10,000 other people doing the same.
    - Start building and posting about your journey online (I could make a task to post twice per week on linkedin something about what I'm building).
    - People in tech are so nice and want to help new people. Ask people for help.
    - At startups people look for software development, but bigger companies look for your knowledge of problem solving, especially solving data structures and algorithms problems. You don't really need to know how to create an API endpoint, for example, because you could quickly pick that up on the job. 
- you just need to know the principles and be really good at problem-solving. part of that is researching how people have solve problems before.
- one of those problem-solving principles is to not give up. Be stubborn about solving it. Said in a way that's more actionable, if there's a concept that's hard to understand, keep working on it until you do understand it. You can do it.
- this guy also did 300 leet code problems. he said you should work on a problem for 1 to 2 hours, and if you don't get it after two hours, look at the solution, then restart and do the problem by yourself.
- leet code is good for learning data structures and algorithms, and builds your skill of pattern recognition when it comes to deciding what data structure or algorithm you should use to solve a problem.
- think of leet code like th SAT for coding. as a student you never actually do SAT problems in college, but its like an IQ test fo you software knowledge. so i should practice data structure and algorithm problems, an leet code is one option to do that. 
- system design is an important concept. He recommends the book Grokking system design. he recommends using excalidraw or lucidchart to "design Airbnb" fo system design. sutem design he says is way more importnat than leetcode. he doesnt use anything he learned through leetcode except the meta skill of problem solving, but he usees system design all the time.
- when on a team, document what you build and its impact, so at the end of the year you are much more likely to get a promotion. 
  - https://www.youtube.com/watch?v=h3td0TPxZAc
- **Person 2:**  https://www.youtube.com/watch?v=vq5WhoPCWQ8Gabriel
https://x.com/gabriel1
  - Name/handle: Gabriel Petersen
  - Current role: open ai researcher on sora (video model)
  - Their learning path: started selling a ecom recommendation system code door to door to businesses. First he made a super simple java pokemon clone. then he made a udemy python course an made a simple 2d shooter game. When you have a real problem to solve, like integrating a product recommedation system with his client's website, its so much clearer what you need you need to get good at. having unlimited time is a bad idea for learning. 
  - Key insight: the best way to learn is to start top down. meaning start with s problem or project. then break it into subproblems recursively. you can ask chatgpt what project you should build. and ask it to explain the intution behind how something works. learning bottom up (like fundamentals first) is a BAD IDEA TO AVOID. He says you can learn diffussion models, for example, in 3 days top down, but it takes 6 years to learn bottom up (academia)
  - to learn using AI, you can ask it to make a quiz. You can also ask it what are the most fundamental concepts in ML, for example. You can have AI write code, then go through line by line to understand what each line does. For example, if it tells you "this help the algorithm learn faster,' you should ask it, 'what do you mean it makes it learn faster.' Then once you have understanding, explain it to the AI and keep doing this until the AI confirms you understand it. He calls it 'recursive gap filling.' The key is knowing what gaps are in your knowledge, and what parts you don't really understand.
    - Build the reflect of 'everytime you have a problem or question, ask AI right away.' He emphasizes this is really important. 
    - you can ask ai to explain something like you're 12. you can ask for 10 ideas about how to improve your codebase. you can ask it about research papers that would help you improve your codebase. 'Give me a list of exactly what this paper tried differently.' 
    - he emphasizes that you can learn anything and get into anything even without college.  
    - If you want to build something like ML, he believes it is really important to read the code that's generating. Ultimately you want to develop an understanding.
    - He kept finding the best teams, learn from them, work as closely with them as possible. Show appreciation for people who review your code because that means they'll give you more and better feedback. If your manager reviews your code, you should ask to hop on a call to go over every comment.  
    - He first joined a startup like airtable. He worked very closely with a really skilled engineer who cared about perfect code and gave him 100 comments per pull request. (Action: when i'm writing code, my ai agent reviewing it should care about perfect code and give me tons of comments.)
    - when you go to an event, or asking for a referal, make sure to mention something impressive you've built. Like a good demo. A good demo communicates that you understand coding and are a good developer. Making demos is super important. He emphasizes you should be able to send someone a link to your demo.
    - Also your portfolio should be a link where it is a story about yourself that demonstrates high agency. Then send it to 500 people.
    - He said avoid company recruiter because they are not technical. They don't want to look bad if the hire doesn't work out, so they will go with safe bets like 'they went to the top school.' Instead reach out to technical leads, hiring managers, or executives at startups. Those people, when looking at your demo, could actaully understand that you can do the job. 
    - Every single startup wants to hire people with high agency who can learn things.
    - Gabriel says you will meet interesting people at college, but you'll meet many more much more interesting people if you go to SF or start working in a company. 
    -His exact learning professor ML prompt workflow:
        bounce what to make, code it, debug it so it works, explain parts, explain intuition why it works, explain the math intution, explain to me like i'm 12, go into all details
- **Person 3:**
  - Name/handle: Sajjaad Khader 
  - Current role: Landed first software engineering role at 20 making $220k/yr at amazon. He helps students land in big tech.
  Video 1: https://www.youtube.com/watch?v=yUQbl9J3kJU
    - Key insight: Start by working on projects. Machine learning project. You can get datasets from kaggle. Clean data using pandas or numpy. Then lean SKlearn library, and use the fit and predict functions to test and train your model. Create visualization using matplotlib and get performance metrics.
    - Remove start date of college. Remove high school experiences unless it's super technical
    - Add 20-30 people on linkedin at a certain company by searching '{job_title} at {company_name}'. Then send them this message:
        Hey! My name is Jonathan. I'm a data science major at Northeastern University. I have X experience and I have Y interest. Would you be down to hop on a 15-minute call to talk about your experiences at the company?
        I'd want to do this at (1) Meta, Google, and (2) Uper, Amazon, OpenAI, Anthropic, xAI.
        - Once you hop on a call, establish rapport, an eventually ask 'Hey would you be down to give me a referal for the upcoming coop/internship program?
        He emphasizes to DO NOT apply without a referal. Absolutly don't do it.
        Behavioral interviews:
            - During interviews, you want to answer behavioral questions by telling a story about an item on your resume. Tie it into one of the company's core values. For example, if amazon asks you something, you could tie it into how you're customer obsessed. Or if amazon asks you your biggest weakness, say that you sometimes dive too deep into problems and don't see the bigger picture.
        - Technical interviews.
            Options are online assessments, online video interviews, and whiteboard interviews. 
            These target data structures and algorithms problems and Leet code. 
            Learn data structures before using leet code by using the website https://csvistool.com/
            After learning that, use leetcode and start with easy questions. Start by doing a few easy problems of one data structure, then a few easy problems of another data structure, etc. Covering all the data structures (meaning doing problems for each) is more important than doing harder leetcode problems.
            If you get stuck on a leetcode practice problem, use https://www.geeksforgeeks.org/, because it has optimal solutions for leetcode problems with explanations.
            For an internship, do not ever negotiate your salary unless you have a really good competing offer.
            1-2 months before your internship, ask the recruiter to put you in touch with your maanger, ask to get on a 1 on 1, and learn what you'll do and what tools you use so you can perhaps take a coursera course if they use a tool you aren't used to
        Video 2: https://www.youtube.com/watch?v=Xt1T2UAEq0Q
            - Value went from who is the strongest, to who is the smartest (who can use the new technology the best), to now agency is the most important thing. Agency is how good you are at using AI. The premis of the value is how good you are using at agents. 'How can i use ai to reach my goals.' Context engineering is important where you provide the info that AI needs to succeed. I should put an example of my creative context engineering on my resume.

- **Person 4:**
  - Name/handle: Yvonne Wang https://www.youtube.com/watch?v=R8udhb7m398
  - Current role: Senior technical recruiter at amazon
  - Their learning path:
  - Key insight: Reviewed 50k applicants. Rejected 95% of them. At amazon, if you don't do well in an interview, there is a cooloff period where if they apply to another role they are automatically rejected. This cooloff period can be 6-24 months.
  - Apply to no more than 2 jobs. If you don't meet the basic qualifications, you will likely be rejected.
  - Biggest resume red flag is if information on your resume and linkedin don't match (like job dates). They also do a background check, so make sure the dates are real.
  - She said you definetly shouldn't apply to a job if you don't meet the basic qualifications you shouldn't apply, unless you get a referal or network with someone in person.
  - Etracuriculars do help on your resume, especially something that shows you can communicate. So my sales role does demonstrate value.
  - You should message recruiters. Big tech companies usually have a specific recruiter looking for a role, so find the recruiter assigned for that role, and DM them on linkedin, link the role, and explain your qualificaitons.
  - Utilize your university's career services department.
  - Attending college events will help a lot with getting a job. 
  - You have to have a really clear idea of what role you want when talking to ta recruiter.
  - The recruiter is always on your side because they get paid to choose people who accept job offers.
  - University career services is a really good idea when it comes to finding a recruiter. 
  - Ask your recruiter if the company has an resources to help you pass the 'OA (online assessment)'
  - She emphasizes multiple times to utilize campus resources. So a component of my ultralearning plan should be investigating and using my university career services here at northeastern university.
  - She also said that joining a professional organization or club with professionals will help a lot, because networking helps a ton when it comes to getting an internship. I could apply for AINU when applications open next fall. She emphasizes you should go to the events of these organizations.
- **Person 5:**
  - Name/handle: Victor Luo
  - Video link: https://www.youtube.com/watch?v=ajYJZAigrPs
  - Current role: Was SWE at Amazon, and now   Tiktok ML Engineer
  - Their learning path:
  - Key insight: ML engineering is designing models where it can make accurate predictions based off troves of data.
  - Another role is a platform engineer. Since tiktok has so many users pinging the model, these engineers make sure that the model can handle the volume of pings.
- Their process is to identify a problem, then do liturature reading (understanding state of the art ways that problem has been solved before)
- ML engineers need both a business udnerstanding and a engineering understanding. Business understanding because they only have limited resources in terms of GPUs the model can run on, or number of expiriments you can test at a time, so you want to pick high impact expiriments. 
- He did a startup as a non-technical founder, but decided that he needs to develop a technical understanding. He self studied for a few months, but then decided to do a bootcamp and he said that was super beneficial. This youtube interview was done by the person running the bootcamp, so this interview was clearly marketing. 
- After the bootcamp called codesmith, he got an internship at amazon. 
- He says autonomous problem solving is the most important skill.
- Work on projects that you feel like are outside your ability.
- One drill he did that i should implement is that a week after writing code, i should explain it (active recall). If I can't , I need to get a refresher.
- He tracked what he did every hour. I should track what I do every day.(My interpreation: I should somehow record waht I work on in terms of ML engineering, and make 1-2 posts on linkedin every week explaining what I did)
- He joined a team where they were building a project together where they tied together LLMs in a way where they could collaborate.

- **Person 5:**
- Name: Theo t3
- Video: https://www.youtube.com/shorts/x71Rm0MWVHY
Role: Software CEO helping devs making applications and coding using AI.
Insight: he said even if you have a software role, you should be interviewing at least every 6 months. Maybe at your current company you are a junior but should be a senior. Plus having an offer at another company will help you negotiate to increase your salary at your current role. There is no reason to not interview other than 'youre boss says you shouldn't.'

- **Person 6:**
- Name: Cyrus Yari. This video was not useful so disreguard.
- Video: https://www.youtube.com/watch?v=QSkzA3Dk6fo
- Role: Senior Software Engineer at Tesla
- Insight: He started in investment banking after college. He then did product management and had a startup but it didn't take off.  
- Companies value soft skills. Luckily I'm already highly skilled at charisma, public speaking, leadership, and sales.

- **Person 7:**
- Name: Maddy Zhang
- Video 1: https://www.youtube.com/watch?v=e6JisS9tEtY
    - Role: SWE google. (interned at: xIBM, xMicrosoft, xAmazon.)
    - Insight: Read about the principles and mission of the company you're interested in to see if you're actually a good fit.
    - It's really good if you know people inside the company and ask for referals. 
    - OpenAI tested her on a leetcode problem during the technical phone screen. They recommended python but you can use any language.
    - They also ask her system design questions. Core concepts include scalability, availability, reliabablity, and CAP theorum. I should add these as concepts above. I should be familiair with concepts like networking (technical term), security, and performance best practices. And web/cloud architecture and distributed systems design.
    - When building a project, include system design flowchart. This is to test if you can explain the system logically. 
    - Be able to explain tradeoffs for design descisions you made.
    - To learn system design, do this course: https://www.educative.io/courses/grokking-the-system-design-interview
    - Practice explaining technical concepts to non-technical friends.
    - Prepare stories demonstrating collabortation and handling ambiguity.
- Video2: https://www.youtube.com/watch?v=opP_Ng76t1g
    - Medium and smaller tech companies are generally are generally more okay with you working remotly than big tech.
    - You can apply to the google summer of code program. It's bascially a remote internship that gives you a great opportunity to collaborate and work on a real team. Applications open in march but you should apply earlier. 'start contributing to participating organizations now. pick 3 organizations, start fixing bugs, engage with mentors on discord, and be part of the team.' <claude> Do research on what she probably means when she says that, and how i can take action on her advice.

- **Person 8:**
- Name: Nishanth
- Role: Intern at citadel
- Path:
- Insights: 
- go to linkedin for software company > people, people > search northeastern.
You'll see that amazon has top 5 northeasrtern students. THen if you search northeasrtern in that menu, you can see alum who work at that company. Itook pics on my phone of good messag eexamples (https://www.linkedin.com/company/amazon/people/?keywords=northeastern)
Or go to khoury in linkedin, go to alumni, see where they go to work. (https://www.linkedin.com/school/khoury-college/people/)
- Then you can see 


#### Job Postings Analysis - COMBINED (All Target Roles)

**Question:** Analyze job postings for ALL target roles. What tools/skills appear most frequently?

*Based on analysis of 36 job listings across all 4 target categories from job_listings.xlsx and skills_aggregate2.md*

| Skill | Frequency | Your Level |
|-------|-----------|------------|
| Python | 36/36 (100%) | |
| PyTorch/TensorFlow | 28/36 (78%) | |
| Distributed Systems/Spark | 18/36 (50%) | |
| A/B Testing/Experimentation | 15/36 (42%) | |
| Recommendation/Personalization | 14/36 (39%) | |
| Deep Learning | 14/36 (39%) | |
| Machine Learning | 13/36 (36%) | |
| SQL | 12/36 (33%) | |
| Data Visualization | 12/36 (33%) | |
| C++ | 11/36 (31%) | |
| Causal Inference | 9/36 (25%) | |
| Statistical Analysis | 9/36 (25%) | |
| NLP | 8/36 (22%) | |
| Cloud (AWS/GCP/Azure) | 5/36 (14%) | |

---

#### Breakdown by Job Category

**Machine Learning Engineer (11 roles)**
| Skill | Frequency |
|-------|-----------|
| Python | 11/11 |
| PyTorch/TensorFlow | 9/11 |
| C++ | 6/11 |
| Recommendation/Personalization | 5/11 |
| Distributed Systems/Spark | 5/11 |

**ML Engineer (Recommendation Systems) (7 roles)**
| Skill | Frequency |
|-------|-----------|
| Python | 7/7 |
| PyTorch/TensorFlow | 8/7 |
| Distributed Systems/Spark | 9/7 |
| Recommendation/Personalization | 7/7 |
| A/B Testing/Experimentation | 4/7 |

**Data Scientist (Consumer) (9 roles)**
| Skill | Frequency |
|-------|-----------|
| Python | 9/9 |
| A/B Testing/Experimentation | 9/9 |
| SQL | 8/9 |
| Data Visualization | 12/9 |
| Causal Inference | 7/9 |
| Statistical Analysis | 6/9 |

**Data Scientist (ML) (9 roles)**
| Skill | Frequency |
|-------|-----------|
| Python | 9/9 |
| PyTorch/TensorFlow | 11/9 |
| Deep Learning | 6/9 |
| Machine Learning | 4/9 |
| NLP | 4/9 |

### 3.2 The Include/Exclude Method

Customize the benchmark approach for your specific goals.

#### What to INCLUDE (emphasize more than standard)
[LEFT OFF]
**Question:** Based on your goals, what should you spend MORE time on than a typical curriculum suggests?

- **Topic/Skill 1:**
  - Why emphasize this:
- **Topic/Skill 2:**
  - Why emphasize this:
- **Topic/Skill 3:**
  - Why emphasize this:

#### What to EXCLUDE (de-emphasize or skip)

**Question:** What can you spend LESS time on or skip entirely?

- **Topic/Skill 1:**
  - Why de-emphasize:
- **Topic/Skill 2:**
  - Why de-emphasize:
- **Topic/Skill 3:**
  - Why de-emphasize:

*Suggestion: Be ruthless here. You can't learn everything. What's truly unnecessary for YOUR goal?*

#### What to MODIFY

**Question:** How will you learn differently than the standard approach?

- **Standard approach: Watch video lectures**
  - Your modification:
  - Why:
- **Standard approach: Do course exercises**
  - Your modification:
  - Why:
- **Standard approach: Read textbooks**
  - Your modification:
  - Why:
- **Standard approach: (add your own)**
  - Your modification:
  - Why:
---

## Part 4: Resource Inventory

### 4.1 Learning Resources

**Instructions:** List specific resources you'll use for each category.

- **Courses:**
  - Resource 1:
    - URL:
    - Priority:
  - Resource 2:
    - URL:
    - Priority:
  - Resource 3:
    - URL:
    - Priority:
- **Books:**
  - Resource 1:
    - Priority:
  - Resource 2:
    - Priority:
- **Documentation:**
  - Resource 1:
    - URL:
    - Priority:
  - Resource 2:
    - URL:
    - Priority:
- **YouTube Channels:**
  - Channel 1:
    - Priority:
  - Channel 2:
    - Priority:
- **Blogs/Newsletters:**
  - Resource 1:
    - URL:
    - Priority:
  - Resource 2:
    - URL:
    - Priority:
- **Communities:**
  - Community 1:
    - Platform:
    - Priority:
  - Community 2:
    - Platform:
    - Priority:
- **Study Tools:**
    - Hackerrank (wayfair uses this to interview technical people)
    - Leetcode

### 4.2 Tools to Set Up

**Instructions:** Check off once set up and working.

- [ ] Python environment (conda/venv)
- [ ] PyTorch installed and tested
- [ ] Docker installed
- [ ] Cloud account (AWS/GCP) with free tier configured
- [ ] Git + GitHub configured
- [ ] IDE set up (VS Code + extensions)
- [ ] AI coding assistant (Claude Code / Cursor)
- [ ] Experiment tracking (W&B / MLflow)
- [ ] Note-taking system (Notion / Obsidian)
- [ ] Spaced repetition app (Anki)

---

## Part 5: Time & Schedule Planning

### 5.1 Available Time Audit

**Question:** How many hours per week can you realistically dedicate?

- **Monday:**
  - Available hours:
  - Best time of day:
  - Notes:
- **Tuesday:**
  - Available hours:
  - Best time of day:
  - Notes:
- **Wednesday:**
  - Available hours:
  - Best time of day:
  - Notes:
- **Thursday:**
  - Available hours:
  - Best time of day:
  - Notes:
- **Friday:**
  - Available hours:
  - Best time of day:
  - Notes:
- **Saturday:**
  - Available hours:
  - Best time of day:
  - Notes:
- **Sunday:**
  - Available hours:
  - Best time of day:
  - Notes:
- **TOTAL:**
  - Hours per week:

### 5.2 Time Allocation

**Question:** How will you split your time across activities?

- **Building projects:**
  - % of time:
  - Hours/week:
- **Drilling weak skills:**
  - % of time:
  - Hours/week:
- **Reading/research:**
  - % of time:
  - Hours/week:
- **Retrieval practice:**
  - % of time:
  - Hours/week:
- **Community/networking:**
  - % of time:
  - Hours/week:
- **TOTAL:**
  - Should equal 100%:
  - Total hours/week:

*Suggestion: Projects should be 50-70% of time for project-based learning.*

---

## Part 6: Potential Obstacles

### 6.1 Identify Challenges

**Question:** What might derail your learning?

- **Obstacle 1: (Example: Burnout)**
  - Likelihood (H/M/L):
  - Mitigation strategy:
- **Obstacle 2:**
  - Likelihood (H/M/L):
  - Mitigation strategy:
- **Obstacle 3:**
  - Likelihood (H/M/L):
  - Mitigation strategy:
- **Obstacle 4:**
  - Likelihood (H/M/L):
  - Mitigation strategy:

### 6.2 Accountability

**Question:** How will you stay accountable?

- [ ] **Learning partner/study group:**
  - Who:
- [ ] **Public commitment (blog, Twitter):**
  - Where:
- [ ] **Regular check-ins with mentor:**
  - Who:
- [ ] **Progress tracking system:**
  - What:
- [ ] **Other:**
  - What:

---

## Part 7: Expert Consultation (Optional but Recommended)

### 7.1 Questions for Experts

**Instructions:** Prepare questions for ML engineers you can reach out to.
- Casey Brown
- Liam Kaufman
- Mario from vegas
- Jonathan Parra from Vegas
- Jai Senthil Kumar
- Sebastian Sepulveda
- Nishanth
- Marco & Griffin from Phi Delt

Draft 5 specific questions:

1.
2.
3.
4.
5.

### 7.2 People to Contact

- **Person 1:**
  - Name:
  - How to reach:
  - What to ask:
  - Status:
- **Person 2:**
  - Name:
  - How to reach:
  - What to ask:
  - Status:
- **Person 3:**
  - Name:
  - How to reach:
  - What to ask:
  - Status:


### 7.3 Referals I could ask for 
    - Taylor from MOA who used to sell google cloud
    - Engingineers above
    - Olivia Gagan (uni recruiter for fidelity)

---

## Action Items Checklist

### Immediate (This Week)
- [ ] Complete Parts 1-2 of this worksheet (Why and What)
- [ ] Analyze 10 job postings and fill in the skills frequency section
- [ ] Set up all tools in section 4.2
- [ ] Identify 3 practitioners to study/contact

### Short-term (Next 2 Weeks)
- [ ] Complete Parts 3-4 (How and Resources)
- [ ] Research 3 university curricula and note structure
- [ ] Find and bookmark primary learning resources
- [ ] Reach out to at least 1 practitioner for advice
- [ ] Complete Parts 5-6 (Time and Obstacles)

### Before Starting Main Learning
- [ ] Finalize your personalized curriculum (include/exclude decisions made)
- [ ] Create weekly schedule template
- [ ] Set up accountability system
- [ ] Complete Part 7 (at least 1 expert consultation)
- [ ] Review this worksheet and refine based on new information

---

ONCE YOU FINISH FILLING THIS OUT, run this prompt

Okay I finished filling out 1metalearning.md. Now I want you to identify any places I have not yet filled in.

## Summary: Your Metalearning Map

*Complete this section after finishing the worksheet.*

### Target Roles:
1. Machine Learning Engineer
2. ML Engineer (Recommendation Systems)
3. Data Scientist (Consumer)
4. Data Scientist (ML)

### My Goal in One Sentence:
-

### Top 5 Skills to Prioritize (based on 36 job postings):
1. Python (100% of roles)
2. PyTorch/TensorFlow (78% of roles)
3. Distributed Systems/Spark (50% of roles)
4. A/B Testing/Experimentation (42% of roles)
5. Recommendation/Personalization + Deep Learning (39% each)

### Top 3 Resources I'll Use:
1.
2.
3.

### My Weekly Commitment:
- Hours per week:
- For how many months:

### My First Project Will Be:
-

### How I'll Know I'm Ready for Jobs:
-

---

## Review Schedule

- [ ] **Week 2:** Review this worksheet and adjust based on early learning
- [ ] **Month 1:** Major review—is the plan working? Adjust as needed
- [ ] **Month 3:** Check progress against goals, update priorities
- [ ] **Month 6:** Comprehensive review, potentially redo Parts 2-3

*Remember: The map is not the territory. Update this document as you learn more about what works for you.*


 

 

# Once the ones i want are selected, run this prompt.

Awesome now keeping all those in mind, regenerate ultralearning_swe.md to accurately reflect my preferences, goal, the concepts, facts, and procedures I deemed important, and the principles.

**Important files to reference:**
- `ultralearning-worksheets/demo-guidelines.md` - Checklist for what makes a good ML demo (critical for portfolio projects)
- `skills_aggregated2.md` - Actual job posting requirements
- The "Practitioner Interviews" section above (Ray Fu, Gabriel Petersen, Sajjaad Khader)
- Casey Brown's advice from introduction.md

Prioritize information from these sources since they come from actual job postings and experts who have done this successfully.