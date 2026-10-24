# AgentBuild — Autonomous Tool-Calling AI Assistant

> **Skill First Labs Internship Shortlisting — Milestone 2: AgentBuild**  
> *A high-trust, engineering-grade autonomous agent interface with tool calling, grounded catalog search, mathematical reasoning, and deep telemetry inspection.*

---

## 1. Project Overview

**AgentBuild** is an agentic AI assistant designed to execute complex reasoning pipelines by interleaving natural language understanding with deterministic tool execution. Built on top of high-speed Groq Cloud inference, AgentBuild implements an autonomous multi-turn ReAct loop that discovers products, inspects warehouse inventory, calculates prices and discounts, and generates grounded, factual responses.

---

## 2. Core Capabilities & Architecture

- **Autonomous Tool-Calling Loop:** Implements W3C-compliant tool invocation protocols with recursive model dispatch. The agent decides when to invoke external tools, evaluates outputs, and synthesizes answers with zero hallucination.
- **Product Catalog Lookup Engine:** Deterministic query resolution against an in-memory hardware & peripherals catalog (search_catalog), supporting SKU, category, price range, and multi-warehouse filters.
- **Mathematical Computation Engine:** Sandboxed expression calculator (calculate) for precise price tallying, discount computation, and inventory arithmetic.
- **Execution Telemetry & Trace Drawer:** Collapsible real-time inspection panel displaying JSON payloads, execution status dots, timestamps, and tool durations.
- **Persistent Conversation Management:** Local session state and conversation threading with instant history switching and context preservation.
- **Linear-Inspired Developer UI:** Crisp light-mode palette, Inter typography, Material Symbols, and responsive layout.

---

## 3. Technology Stack

- **Inference Engine:** Groq Cloud API (openai/gpt-oss-120b or configurable models)
- **Frontend Architecture:** Modern Vanilla HTML5 / ES6+ JavaScript / CSS
- **Styling & Design System:** Tailwind CSS with custom developer-grade tokens
- **Markdown & Security:** Marked.js for response rendering and DOMPurify for strict XSS sanitization

---

## 4. Getting Started

### Prerequisites
- Modern web browser (Chrome, Edge, Firefox, Safari)
- A Groq Cloud API key ([console.groq.com/keys](https://console.groq.com/keys))

### Installation & Run

1. **Clone the repository:**
   \\\ash
   git clone https://github.com/Abisheik-728/agentbuild.git
   cd agentbuild
   \\\

2. **Configure your API Key:**
   Copy \config.example.js\ to \config.js\ and add your Groq API key:
   \\\ash
   cp config.example.js config.js
   \\\
   Edit \config.js\:
   \\\javascript
   window.GROQ_API_KEY = 'your-groq-api-key-here';
   \\\
   *(Note: \config.js\ is included in \.gitignore\ to prevent accidental secret exposure).*

3. **Launch the web application:**
   You can serve the folder using any static HTTP server:
   \\\ash
   # Using Python
   python -m http.server 8080

   # Or using Node.js npx serve
   npx serve .
   \\\
   Open \http://localhost:8080\ in your browser.

4. **Alternative In-App Setup:**
   You can also enter or update your Groq API key directly via the in-app **Settings** dialog without editing files.

---

## 5. Security & Secret Hygiene

- No API keys or secrets are committed to version control.
- All credentials are kept in untracked local storage or ignored configuration files (\config.js\).
- Responses are sanitized with DOMPurify before DOM insertion to protect against cross-site scripting (XSS).

---

## 6. License

MIT License. Developed for Skill First Labs Internship — Milestone 2.
