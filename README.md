# 🤖 AI Job Application Automator

An intelligent multi-agent AI system built with **LangGraph** that automatically searches for real jobs, writes custom cover letters, and sends applications via Gmail — all with human approval before sending!

## 🚀 Demo

🚀 AI Job Application Automator Starting...

- 🤖 Supervisor: Starting workflow...
   - Job Role : Python Developer
   - Applicant: Jimi Patel

📌 Running Research Subgraph...
- 🔍 Searching real jobs with Tavily...
   - ✅ Found 3 real jobs!
 - 🏢 Researching companies...
   - ✅ Researched: TCS, Infosys, Wipro

📌 Running Content Subgraph...
- 📄 Tailoring resumes...
   - ✅ All resumes tailored!
- ✍️  Writing cover letters...
   - ✅ All cover letters written!


🛑 HUMAN APPROVAL REQUIRED

  1. Senior Python Developer at TCS (Ahmedabad)
  2. Python Developer at Infosys (Bangalore)
  3. Python Lead at Wipro (Remote)

✅ Auto Approved!

📌 Running Apply Subgraph...
- 📧 Sending real emails...
   - ✅ Email sent to hr@tcs.com!
   - ✅ Email sent to careers@infosys.com!
   - ✅ Email sent to jobs@wipro.com!
- 📊 Excel tracker saved!

🎉 FINAL RESULTS
- ✅ Real Emails Sent : 3
- ✅ Tracker Saved   : outputs/applications.xlsx
- ✅ Cover Letters   : outputs/cover_letters/

## ✨ Features

- **Real Job Search** — Tavily MCP searches actual job listings from web
- **AI Cover Letters** — Groq LLM writes custom cover letter for each job
- **Resume Tailoring** — AI customizes resume summary for each company
- **Real Email Sending** — Gmail SMTP sends actual application emails
- **Human Approval** — Reviews jobs before applying
- **Excel Tracker** — Tracks all applications automatically
- **Checkpointing** — Resume workflow if interrupted
- **100% Free** — Uses Groq API + Tavily free tier

## 🧠 LangGraph Architecture

<img width="468" height="804" alt="Screenshot (96)" src="https://github.com/user-attachments/assets/107d973e-95ff-4411-ba53-c553d4ab63d0" />

### Subgraphs Detail:

- Research Subgraph:
  job_search_node        ← Tavily web search
  company_research_node  ← Company background

- Content Subgraph:
  tailor_resume_node     ← AI resume customization
  cover_letter_node      ← AI cover letter writing

- Apply Subgraph:
  send_applications_node ← Gmail SMTP
  save_tracker_node      ← Excel file

## 🛠️ Tech Stack

- **LangGraph** -> Multi-agent workflow orchestration 
- **LangChain** -> AI framework and tool integration 
- **Groq API** -> Free LLM (Llama 3.3 70B) 
- **Tavily API** -> Real-time web job search 
- **Gmail SMTP** -> Real email sending 
- **openpyxl** -> Excel tracker generation 
- **MemorySaver** -> Workflow checkpointing 
- **Python 3.10+** -> Programming language
  
## 🆕 Advanced Concepts Used

- **Subgraphs** -> 3 mini graphs inside main graph 
- **Supervisor Pattern** -> Boss agent coordinates workers 
- **Human-in-the-Loop** -> Approval before applying 
- **Checkpointing** -> MemorySaver for state persistence 
- **MCP Integration** -> Real tools via Tavily + Gmail 
- **State Management** -> TypedDict shared state 


## 📊 Output Files

### applications.xlsx 

<img width="1432" height="298" alt="Screenshot (99)" src="https://github.com/user-attachments/assets/256fe268-e333-4f3d-8c17-68387e426a8e" />

### cover_letters

<img width="1022" height="419" alt="Screenshot (100)" src="https://github.com/user-attachments/assets/1b5ada44-b7a2-4c3b-9a03-b1180f40be0d" />

## 🔮 Future Improvements

- [ ] LinkedIn job search integration
- [ ] Naukri.com scraping support
- [ ] PDF resume attachment in email
- [ ] Streamlit web interface
- [ ] Interview scheduler
- [ ] Application status tracker
- [ ] WhatsApp notification on apply

---

## ⚠️ Important Notes

1. Use this tool responsibly
2. Only apply to jobs you are genuinely interested in
3. Review cover letters before sending
4. Keep your API keys secure — never upload .env file
5. Tavily free tier = 1000 searches/month
6. Groq free tier = generous daily limits

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Open an issue for bugs
- Submit a pull request
- Suggest new features


## ⭐ Support

If this project helped you land a job or saved your time, please give it a **star** on GitHub! ⭐

Share it with friends who are job hunting! 🚀

*Built with ❤️ using LangGraph + LangChain + Groq + Tavily*
