<div align="center">
<img src="https://img.shields.io/badge/📋_Meeting_Summarizer-Local_LLM_Powered-blue?style=for-the-badge&labelColor=1a1a2e&color=16213e" alt="Project Banner" width="600"/>

<br/>

<img src="https://img.shields.io/badge/Gemma_4-Ollama-orange?style=flat-square&logo=google&logoColor=white" alt="Gemma 4"/>
<img src="https://img.shields.io/badge/Python-3.9+-blue?style=flat-square&logo=python&logoColor=white" alt="Python"/>
<img src="https://img.shields.io/badge/Streamlit-Web_UI-red?style=flat-square&logo=streamlit&logoColor=white" alt="Streamlit"/>
<img src="https://img.shields.io/badge/Click-CLI-green?style=flat-square&logo=gnu-bash&logoColor=white" alt="Click CLI"/>
<img src="https://img.shields.io/badge/License-MIT-yellow?style=flat-square" alt="License"/>

<br/><br/>

<strong>Part of <a href="https://github.com/kennedyraju55/90-local-llm-projects">90 Local LLM Projects</a> collection</strong>

</div>

<br/>
# 📋 Meeting Summarizer

![Python](https://img.shields.io/badge/Python-3.11+-blue?logo=python&logoColor=white)
![LLM](https://img.shields.io/badge/LLM-Gemma%204-orange)
![Ollama](https://img.shields.io/badge/Ollama-Local-green)
![Streamlit](https://img.shields.io/badge/UI-Streamlit-red?logo=streamlit)
![License](https://img.shields.io/badge/License-MIT-yellow)

Production-grade meeting transcript analyzer with speaker identification, action item tracking, decision logging, and follow-up reminders using a local LLM.

## ✨ Features

- **Attendee Extraction** — Identifies participants and their roles
- **Speaker Identification** — Profile speakers with contribution analysis
- **Action Item Tracking** — Tasks with assignee, description, and deadline
- **Decision Log** — Structured decision tracking with proposers and approvers
- **Follow-up Reminders** — Prioritized follow-ups with deadlines
- **Agenda Detection** — Topics covered in the meeting
- **Dual Interface** — CLI + Streamlit Web UI
- **File Export** — Save summaries to Markdown
- **Local & Private** — All data stays on your machine

## 🚀 Installation

```bash
cd 13-meeting-summarizer
pip install -r requirements.txt
ollama serve && ollama pull gemma4
```

## 📋 CLI Usage

```bash
# Full summary
python -m src.meeting_summarizer.cli summarize --transcript meeting.txt

# Save to file
python -m src.meeting_summarizer.cli summarize --transcript meeting.txt --output summary.md

# Speaker identification
python -m src.meeting_summarizer.cli speakers --transcript meeting.txt

# Decision log
python -m src.meeting_summarizer.cli decisions --transcript meeting.txt

# Follow-up reminders
python -m src.meeting_summarizer.cli followups --transcript meeting.txt
```

## 🌐 Web UI (Streamlit)

```bash
streamlit run src/meeting_summarizer/web_ui.py
```

Features: Transcript upload, summary tabs (decisions/actions/notes), speaker profiles, timeline.

## 🧪 Running Tests

```bash
python -m pytest tests/ -v
```

## 📁 Project Structure

```
13-meeting-summarizer/
├── src/meeting_summarizer/
│   ├── __init__.py, core.py, cli.py, web_ui.py, config.py, utils.py
├── tests/
│   ├── __init__.py, test_core.py, test_cli.py
├── config.yaml, setup.py, requirements.txt, Makefile, .env.example, README.md
```

## Part of

[90 Local LLM Projects](../README.md)

## 📸 Screenshots

<div align="center">
<table>
<tr>
<td><img src="https://via.placeholder.com/400x250/1a1a2e/e94560?text=CLI+Interface" alt="CLI Interface"/></td>
<td><img src="https://via.placeholder.com/400x250/16213e/e94560?text=Web+UI" alt="Web UI"/></td>
</tr>
<tr>
<td align="center"><em>CLI Interface</em></td>
<td align="center"><em>Streamlit Web UI</em></td>
</tr>
</table>
</div>
