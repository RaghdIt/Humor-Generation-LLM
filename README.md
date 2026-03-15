# Topic-Guided Humor Generation using Large Language Models

This project studies whether a large language model can generate humorous text that adapts to different topics or social contexts.

Instead of focusing on humor classification, the project focuses on **controlled text generation** and evaluates whether generated jokes are:

- funny
- fluent
- relevant to the requested topic

The experiment compares humor generation across multiple topics such as technology, work, relationships, school, and politics.

---

# Project Goal

The goal of this project is to examine whether a generative language model can produce jokes that change depending on the requested topic.

By controlling the generation conditions and changing only the topic, we can analyze how humor quality varies across different social contexts.

---

# Research Questions

The project answers three main research questions.

### RQ1
Can the model generate jokes that are understandable and humorous?

Evaluation criteria:
- funniness
- fluency

### RQ2
Does humor quality change across topics?

Evaluation criteria:
- comparison of scores across topics

### RQ3
Can the model generate jokes that match the requested topic?

Evaluation criteria:
- topic relevance

---

# Project Pipeline

The project follows a structured pipeline.

1. Define the research goal and questions  
2. Reduce the dataset to a manageable subset  
3. Discover common topics in the joke dataset  
4. Select a final set of topics for generation  
5. Design controlled prompts for generation  
6. Generate jokes for each topic  
7. Evaluate generated jokes using human ratings  
8. Analyze results across topics

---

# Topics Used in the Experiment

Example topics used for generation:

- Technology
- Work
- Relationships
- School
- Politics
- Daily Life

Each topic represents a different social context for humor generation.

---

# Controlled Generation Design

To ensure fair comparison, the experiment keeps all generation settings fixed except the topic.

Fixed conditions:

- same language model
- same prompt structure
- same audience description
- same output style
- same number of generated jokes

Example prompt template:

Generate one short original joke about [TOPIC].

Audience: general adults  
Style: one-line joke  
Use natural language and avoid offensive content.

---

# Generation Setup

Each topic receives the same number of generated jokes.

Example setup:

Technology – 20 jokes  
Work – 20 jokes  
Relationships – 20 jokes  
School – 20 jokes  
Politics – 20 jokes  
Daily Life – 20 jokes  

Total generated jokes: **120**

---

# Human Evaluation

Generated jokes are evaluated by human judges using three criteria.

| Criterion | Description | Scale |
|----------|-------------|------|
| Funniness | How amusing the joke is | 1–5 |
| Fluency | Language clarity and readability | 1–5 |
| Topic Relevance | Whether the joke matches the topic | 1–5 |

Scores are averaged for final analysis.

---

# Technologies Used

- Python
- Google Colab / Jupyter Notebook
- OpenAI API
- Pandas
- Human evaluation methodology

---

# Key Idea

This project explores how well a language model can adapt humor generation to different topics while maintaining:

- humor quality
- linguistic fluency
- topic relevance
