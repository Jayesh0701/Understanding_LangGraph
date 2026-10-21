# LangGraph Learning Project

A set of Jupyter notebooks for learning how to build workflows with LangGraph, from basic state graphs to LLM-powered and parallel workflows.

## Learning progress

1. **Graph basics** — calculate and categorize BMI using state, nodes, and edges.
2. **First LLM workflow** — pass a question through a graph node and return a model response.
3. **Prompt chaining** — generate a blog outline, then use it to create a post.
4. **Parallel workflows** — calculate cricket statistics in parallel and combine them into a summary.
5. **Structured evaluation** — score an essay on multiple criteria in parallel, then combine the feedback and scores.

## What I have learned

- A `StateGraph` organizes work into nodes connected by edges.
- Typed state carries inputs and results between nodes.
- Compiling a graph creates a workflow that can be run with `invoke`.
- Sequential nodes support prompt chaining; parallel nodes can handle independent tasks.
- Structured model output and reducers help combine typed results from parallel evaluations.

## Run the notebooks

Install the listed dependencies:

```bash
pip install -r requirements.txt
```

For notebooks that use Google Gemini, add an `API_KEY` to a `.env` file in the project folder, then open and run the notebooks in order.

## Notebooks

- `00graph_working_concept.ipynb`
- `01first_llm_workflow.ipynb`
- `02llm_chaining_prompt.ipynb`
- `03cricket_stats_parallel_WF.ipynb`
- `04scorring_llm_workflow.ipynb`
