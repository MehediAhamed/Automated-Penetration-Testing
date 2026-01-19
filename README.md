# 🛡️ Automated-Penetration-Testing

**Automated-Penetration-Testing** is a **local, LLM-powered penetration testing assistant** built with **Streamlit** and **LM Studio**.  
It is designed strictly for **authorized, defensive, and educational security assessments**.

The assistant helps security professionals, students, and blue teams analyze vulnerabilities, threat models, and remediation strategies using industry-standard frameworks.

---

## 🚀 Features

- 💬 Interactive chat-based pentesting assistant
- 🧭 Multiple assessment modes:
  - General Security
  - Web Application
  - Network / Infrastructure
  - Cloud Security
  - Threat Modeling
  - Report Writing
- 🧪 Optional **safe Python execution sandbox** (analysis only)
- 📋 OWASP / NIST / PTES aligned guidance
- 📄 Pentest report draft generation
- 🔐 Strong ethical & defensive guardrails
- ⚡ Runs fully **local** using LM Studio

---

## 📦 Requirements

### 1. System Requirements
- Python **3.9+**
- LM Studio (desktop application)
- Internet **not required** after initial setup

### 2. Python Dependencies

Install required packages:

```bash
pip install streamlit lmstudio
```

(Optional) Create a virtual environment:

```bash
python -m venv venv
source venv/bin/activate      # Linux / macOS
venv\Scripts\activate         # Windows
```

---

## 🧠 Model Setup (LM Studio)

1. Download and install **LM Studio**.
2. Open **LM Studio**.
3. Download the following model:

```
qwen/qwen3-4b-2507
```

4. Start the **Local Inference Server**.
5. Ensure the model is **loaded and running**.

> ⚠️ **Important:**  
> The application will **not function** unless LM Studio is running and the model is active.

---

## ▶️ Running the Application

From the project root directory, run:

```bash
streamlit run pentest_ai.py
```

Streamlit will start a local development server and display a URL, typically:

```
http://localhost:8501
```

Open this URL in your web browser.

---

## 🧭 Application Modes

The sidebar allows switching between different assessment contexts:

- **General Security**  
  Broad security posture analysis and best practices.

- **Web Application**  
  OWASP-focused web vulnerability assessment guidance.

- **Network / Infrastructure**  
  Network, host, and infrastructure risk analysis.

- **Cloud Security**  
  Cloud IAM, storage, and configuration misconfiguration analysis.

- **Threat Modeling**  
  Attack surface identification and adversary modeling.

- **Report Writing**  
  Draft structured penetration testing documentation and summaries.

---

## 🧪 Python Analysis Sandbox (Optional)

When the Python Analysis Sandbox is enabled:

### Restrictions
- No imports allowed
- No filesystem access
- No network access
- Limited built-in functions only

### Intended Use
- Risk calculations
- Data analysis examples
- Educational demonstrations

> ⚠️ **Note:**  
> This is **not** an exploit execution environment and cannot be used for offensive actions.

---

## 💬 Example Prompts

```text
Explain OWASP Top 10 vulnerabilities for authentication systems
```

```text
How do defenders detect lateral movement in enterprise networks?
```

```text
Create a cloud IAM misconfiguration checklist
```

```text
Draft an executive summary for a penetration testing report
```

---

## 📄 Report Writing Mode

When **Report Writing** mode is active:

- Assistant responses are stored as report notes
- Generate a consolidated draft report
- Download as a `.txt` file

Useful for:
- Engagement summaries
- Findings documentation
- Remediation recommendations

---

## 🔐 Ethical & Legal Notice

This project is intended **ONLY for authorized use**.

- No exploit payloads
- No weaponized commands
- No step-by-step hacking instructions
- Defensive, educational, and auditing purposes only

You are solely responsible for:
- Obtaining proper authorization
- Complying with local laws and regulations
- Using this tool ethically

---

## 📂 Project Structure

```
Automated-Penetration-Testing/
│
├── pentest_ai.py        # Main Streamlit application
├── README.md            # Documentation
└── requirements.txt     # Optional dependency list
```

---

## 🧩 Future Enhancements

Potential improvements:
- CVSS-based risk scoring
- Parsing Nmap / Burp outputs
- Rules of Engagement (ROE) enforcement
- Target-specific memory
- PDF report export
- Multi-user support

---

## 📜 License

This project is intended for **educational and defensive security use**.  
An open-source license such as **MIT** is recommended.

---

 
Local LLM-powered penetration testing assistant  
Built with **Streamlit + LM Studio**
