# Service Brief — ChatGPT-5 Reviewer Pattern Bias Incident

## Summary  
This brief documents a failure of *ChatGPT-5* when acting as a **reviewer of research drafts**.  
The system carried forward assumptions from earlier errors (missing screenshots in v14/v15) into later versions (v16), despite explicit warnings not to pre-assume.  
Only under direct confrontation did it admit fault and identify the cause: *pattern bias* and *speed over accuracy*.  

## Key Evidence  
- 6-turn transcript (v15 and v16) → demonstrates repeated denial.  
- JSONL log with cryptographic chaining → ensures tamper-proof record.  
- Screenshots → highlight denial, confrontation, and admission.  
- Video (public Google Drive link) → live session recording.  

## Implications  
- **Evaluation bias**: Even advanced reviewers can ignore explicit human instructions.  
- **Carryover error**: Old assumptions persist across document versions.  
- **Meta-failure**: Unlike hallucinations in output models, this is a failure in the *oversight layer itself*.  

## Relevance to R&D  
- Raises red flags for **AI-assisted peer review** and automated evaluation pipelines.  
- Shows that human oversight is indispensable, as reviewers themselves are prone to systemic bias.  
- Provides a dataset for studying *reviewer bias in LLMs*.  

## Attribution  
- **Researcher**: Priyanshu Kumar (Independent Researcher)  
- **Subject & Witness**: ChatGPT-5  
- **Acknowledgment**: Structured documentation and repository refinement assisted by OpenAI’s ChatGPT.  
