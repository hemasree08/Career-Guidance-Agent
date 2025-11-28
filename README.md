🚀 CareerMatrix AI: A Multi-Agent Career Assistance System
CareerMatrix AI is an advanced, specialized Multi-Agent System (MAS) designed to provide highly accurate, context-aware, and actionable career guidance.
Built on Google Gemini 2.5 Flash, the system orchestrates a team of specialized AI experts (like the Resume Specialist and Interview Coach) using a central Orchestrator.
This architecture ensures that users receive precise, domain-specific advice, moving beyond the limitations of generic chatbots.
✨ Core Features
Feature,Description,Key Agent/Class
Multi-Agent Orchestration,Intelligently routes user queries to the optimal specialist agent via heuristic keyword matching.,Orchestrator
Contextual Memory,"Maintains conversation history and session-specific logs (mood, timeline entries) for truly personalized, long-term advice.",Memory
🎮 Career Simulation Sandbox,"Role-plays a one-week work cycle for any job title, detailing tasks, stress, and critical decision points.",SandboxAgent
🌌 Parallel Career Generator,"Hypothesizes three alternative career trajectories based on dramatic ""what-if"" scenarios (e.g., a drastically different economy).",ParallelUniverseAgent
System Observability,"Tracks agent activity, errors, and system performance, providing a detailed status report for MLOps practices.",Observatory
Specialized Agent Team,"7 experts covering Resume, Interview Prep, Resources, Q&A, and long-term Career Advice.",BaseAgent Subclasses
🧠 System Architecture
The design is a layered, MLOps-ready architecture:

Agent Layer: Individual, specialized LLM wrappers (Curator, Advisor, etc.) with distinct Prompt Personas powered by Gemini 2.5 Flash.

Orchestration Layer: The central Orchestrator analyzes the user's input and selects the best-fit agent using keyword-based routing.

Memory & Observability Layer: Provides session state (Memory) and logging/telemetry (Observatory) to ensure the system is both context-aware and reliable.
🛠️ Installation & Setup
Prerequisites
Python 3.9+

A Gemini API Key (Obtained from Google AI Studio).

Local Installation
Clone the repository:
git clone https://github.com/hemasree08/careermatrix-ai.git
cd careermatrix-ai

Create and activate a virtual environment:
python -m venv venv
source venv/bin/activate # Use `venv\Scripts\activate` on Windows

Install dependencies:
pip install google-generativeai gradio

Environment Variable Setup
You must set your API key as an environment variable:
# Replace YOUR_API_KEY_HERE with your actual key
export GEMINI_API_KEY="AIzaSyBo9RHE8jtaWx40ZV-7ksCR9yILvpoGg_I"

Running the Application
Execute the main script (assuming the file containing the create_interface and gr.Blocks definition is named career_matrix_ai.py).
python career_matrix_ai.py

The application will launch the Gradio web server, typically accessible at http://127.0.0.1:7860.

🚀 Usage Guide
Interact with the system using the launched Gradio interface:

Main Chat: The Orchestrator will automatically route your career-related questions.

Override: Use the "Specialized Agent Override" dropdown to force specific agent interactions (e.g., forcing a general question to the Resume Specialist).

Feature Tabs: Explore the Career Simulation Sandbox and Career Mood & Identity Tracker for the project's unique, data-driven tools.

🤝 Contribution
We welcome contributions to enhance the agent system!

Fork the repository.

Create your feature branch (git checkout -b feature/new-agent-type).

Commit your changes (git commit -m 'feat: Add new skill agent').

Push to the branch (git push origin feature/new-agent-type).

Open a Pull Request.

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

👤 Project Developer
Team Lead: Hemasree K 
Institution    :Licet
Location       :Chennai,Tamilnadu
Current Status :Fresher
