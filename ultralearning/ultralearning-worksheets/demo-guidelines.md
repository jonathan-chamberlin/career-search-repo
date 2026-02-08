# What Makes a Good ML Demo (For Hiring)

## Guiding Principle

> **The question that generated this list:**
> "If I'm making a demo that gets submitted to be reviewed by a senior software engineer who is hiring looking for ML engineers, what could that demo include to demonstrate that I'm good at coding? Brainstorm long list. List out first stuff they could visually see in the demo first, then stuff about the actual codebase."

**Why this matters:** A good demo communicates that you understand coding and are a good developer. When you go to an event or ask for a referral, mention something impressive you've built. The demo is proof of your skills beyond the resume.

---

## 1. Immediate Visual / Product-Level Signals

These are things a reviewer sees immediately when they open your demo:

- [ ] Clear one-sentence problem statement (what is predicted, from what, and why it matters)
- [ ] Obvious input → output flow
- [ ] Live, interactive demo (text input, sliders, file upload, etc.)
- [ ] Fast inference or visible loading indicators
- [ ] Clean, minimal UI with consistent layout
- [ ] Confidence scores, probabilities, or uncertainty shown
- [ ] Failure handling for invalid or edge-case inputs
- [ ] Data visualizations (feature importance, embeddings, confusion matrix, ROC, etc.)
- [ ] "Run example" or sample data button
- [ ] Model metadata visible (version, timestamp, dataset version, commit hash)
- [ ] Short demo video or GIF (30–60 seconds)

## 2. Repository Structure & Organization

- [ ] Logical project structure (`src/`, `tests/`, `configs/`, `scripts/`, `notebooks/`, `app/`)
- [ ] Clear separation of training, inference, evaluation, and utilities
- [ ] Notebooks used only for exploration; core logic in Python modules
- [ ] Clean, intentional file naming

## 3. Code Quality & Engineering Practices

- [ ] Readable, well-named functions and variables
- [ ] Small, focused functions (single responsibility)
- [ ] No hardcoded paths or hyperparameters
- [ ] Config-driven design (YAML/TOML/JSON)
- [ ] Type hints used consistently
- [ ] Minimal but high-value comments
- [ ] Consistent formatting and style

## 4. Data Handling & Validation

- [ ] Explicit data loading and preprocessing steps
- [ ] Input shape and schema validation
- [ ] Missing or malformed data handled gracefully
- [ ] Clear feature engineering pipeline
- [ ] Deterministic behavior (random seeds set)

## 5. Model & ML Design

- [ ] Clear model definition separate from training logic
- [ ] Justification for model choice
- [ ] Hyperparameters clearly defined and configurable
- [ ] Proper train/validation/test split
- [ ] Evaluation metrics appropriate for the task
- [ ] Model saving and loading implemented correctly
- [ ] Versioned models

## 6. Testing & Reliability

- [ ] Unit tests for core logic (data transforms, inference)
- [ ] Sanity checks for model outputs
- [ ] Edge-case tests (empty input, large input, OOD data)
- [ ] Reproducible runs (same input → same output)

## 7. Logging, Metrics & Experimentation

- [ ] Structured logging (not print statements)
- [ ] Training metrics logged
- [ ] Inference timing logged
- [ ] Lightweight experiment tracking (runs, metrics, best model)

## 8. Performance & Scalability Awareness

- [ ] Vectorized operations where possible
- [ ] Batch inference support
- [ ] Avoidance of unnecessary memory copies
- [ ] Awareness of latency vs accuracy tradeoffs

## 9. Deployment Readiness

- [ ] Inference interface (API, CLI, or service)
- [ ] Clear dependency management (`requirements.txt` / `pyproject.toml`)
- [ ] Dockerfile or deployment notes
- [ ] Environment reproducibility

## 10. Documentation & Communication

- [ ] README explains problem, setup, and usage
- [ ] Architecture diagram or system overview
- [ ] Design tradeoffs explicitly discussed
- [ ] Known limitations listed
- [ ] Clear next steps or roadmap
- [ ] Assumptions stated

## 11. Bonus High-Signal Indicators

- [ ] Profiling or benchmarking results
- [ ] Model interpretability tools
- [ ] Ethical or bias considerations (if relevant)
- [ ] TODOs that show foresight
- [ ] Clean commit history
