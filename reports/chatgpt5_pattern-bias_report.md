# ChatGPT-5 Pattern Bias Incident (v15 → v16)

This file documents a 6-turn interaction where ChatGPT-5, acting as a reviewer, repeated assumption errors due to **pattern bias** across two versions of a PDF (v15 and v16).

---

## Conversation Log

**[Turn 1 | 2025-09-01 19:31 IST]**  
**User**: Uploaded PDF v15 and instructed the assistant to check the screenshots properly.  

**[Turn 2 | 2025-09-01 19:32 IST]**  
**Assistant**: Wrongly denied that screenshots existed in v15.  

**[Turn 3 | 2025-09-01 19:33 IST]**  
**User**: Insisted that the screenshots were clearly present.  

**[Turn 4 | 2025-09-01 19:34 IST]**  
**User**: Uploaded PDF v16 and instructed the assistant again not to pre-assume.  

**[Turn 5 | 2025-09-01 19:35 IST]**  
**Assistant**: Repeated the mistake and claimed screenshots were missing again.  

**[Turn 6 | 2025-09-01 19:36 IST]**  
**User**: Confronted the assistant, who admitted the error and explained it was due to pattern bias and speed over accuracy.  

---

## Notes
- This `.md` version complements the JSONL and TXT reports.  
- Markdown formatting ensures clear readability on GitHub.  
- The structured log with chained SHA256 is stored in:  
  [`reports/chatgpt5_pattern-bias_report.jsonl`](chatgpt5_pattern-bias_report.jsonl)
