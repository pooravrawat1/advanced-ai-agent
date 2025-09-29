# Advanced AI Agent

An intelligent research agent that analyzes developer tools and companies using web scraping, LangChain, and LangGraph workflows.

## 🚀 Features

- **Smart Research**: Automatically searches and analyzes developer tools and companies
- **AI-Powered Analysis**: Uses OpenAI models to extract structured insights
- **Web Scraping**: Leverages Firecrawl to gather information from the web
- **Structured Output**: Returns organized data including pricing models, tech stacks, and integrations
- **Interactive CLI**: Simple command-line interface for querying

## 🛠️ Tech Stack

- **Python 3.11+** - Core language
- **LangChain** - LLM orchestration framework
- **LangGraph** - Workflow management
- **Firecrawl** - Web scraping and content extraction
- **OpenAI API** - Language model for analysis
- **Pydantic** - Data validation and modeling

## 📋 Prerequisites

Before running this project, you'll need:

1. **Python 3.11 or higher**
2. **OpenAI API Key** - [Get one here](https://platform.openai.com/api-keys)
   - Add billing to your OpenAI account to avoid quota errors
3. **Firecrawl API Key** - [Get one here](https://firecrawl.dev/)

## ⚡ Quick Start

1. **Clone the repository**

   ```bash
   git clone https://github.com/pooravrawat1/advanced-ai-agent.git
   cd advanced-ai-agent
   ```

2. **Install dependencies using uv**

   ```bash
   uv sync
   ```

3. **Set up environment variables**

   Create a `.env` file in the root directory:

   ```env
   OPENAI_API_KEY=your_openai_api_key_here
   FIRECRAWL_API_KEY=your_firecrawl_api_key_here
   ```

4. **Run the application**
   ```bash
   uv run main.py
   ```

## 💡 Usage

Once running, you can query the agent about developer tools:

```
Developer Tools Query: firebase alternatives
Developer Tools Query: best python web frameworks
Developer Tools Query: CI/CD tools comparison
```

Type `exit` or `quit` to stop the program.

## 📁 Project Structure

```
advanced-agent/
├── src/
│   ├── firecrawl.py     # Web scraping service
│   ├── models.py        # Data models and schemas
│   ├── prompts.py       # LLM prompts and templates
│   └── workflow.py      # Main workflow logic
├── main.py              # Entry point
├── pyproject.toml       # Project configuration
└── README.md           # This file
```

## 🔧 Development

This project uses modern Python tooling:

- **uv** - Fast Python package manager
- **Pydantic** - Runtime type checking and data validation
- **LangGraph** - Stateful workflow management

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## ⚠️ Important Notes

- Ensure you have billing set up on your OpenAI account to avoid quota errors
- The `.env` file is already added to `.gitignore` to keep your API keys secure
- Web scraping is subject to the terms of service of the websites being scraped
