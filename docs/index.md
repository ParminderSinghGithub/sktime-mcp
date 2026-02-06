# sktime-mcp

<div class="hero-text">
  <h1>The Semantic Engine for Time-Series</h1>
  <p style="font-size: 1.2rem; margin-bottom: 2rem;">
    Empower Large Language Models to discover, reason about, and execute 
    sktime's advanced forecasting algorithms on real-world data.
  </p>
</div>

!!! success "Why sktime-mcp?"
    Bridging the gap between **LLM reasoning** and **time-series precision**. 
    Instead of hallucinating Python code, your agent interacts with a strictly typed, 
    safe, and stateful API to perform complex forecasting tasks.

---

## 🔥 Key Features

<div class="grid cards" markdown>

-   :material-compass-outline: **Semantic Discovery**
    ---
    Find the perfect estimator using semantic similarity and capability tags (e.g., "probabilistic forecaster that handles missing data").

-   :material-puzzle-outline: **Safe Composition**
    ---
    Build complex pipelines (Transformer → Forecaster) with built-in validation to ensure components are compatible before execution.

-   :material-database-outline: **Universal Data Loading**
    ---
    Seamlessly ingest data from **SQL Databases**, **Pandas DataFrames**, **Parquet**, **Excel**, and **CSV** files.

-   :material-flash-outline: **Execution Runtime**
    ---
    Stateful execution engine that manages object lifecycles, fitting, and predicting, all via simple JSON-RPC tools.

</div>

---

## ⚡ Quick Start

Get up and running in seconds. Use with **Claude Desktop**, **Cursor**, or any MCP-compatible client.

### 1. Install
```bash
pip install -e ".[all]"
```

### 2. Run
```bash
sktime-mcp
```

### 3. Connect (Claude Desktop Config)
Add this to your `claude_desktop_config.json`:
```json
{
  "mcpServers": {
    "sktime": {
      "command": "sktime-mcp"
    }
  }
}
```

---

## 📚 Documentation Map

| Section | Description |
| :--- | :--- |
| [**User Guide**](user-guide.md) | Comprehensive manual on using tools, workflows, and best practices. |
| [**Data Sources**](data-sources.md) | Deep dive into loading data from SQL, Files, and Pandas. |
| [**Architecture**](architecture.md) | High-level system design, data flow, and limitations. |
| [**Implementation**](implementation.md) | Detailed code walkthrough and file breakdown. |
| [**Developer Guide**](dev-guide.md) | Contributing guidelines, testing, and extending the server. |

---

## 🚀 Example Workflow

1.  **Discover**: "Find me a model that handles missing data."
2.  **Load**: "Load `sales_data.csv`."
3.  **Train**: "Fit an AutoARIMA model on the data."
4.  **Predict**: "Forecast the next 12 months."
5.  **Export**: "Give me the Python code to reproduce this."

[Get Started Now](user-guide.md){ .md-button .md-button--primary }
