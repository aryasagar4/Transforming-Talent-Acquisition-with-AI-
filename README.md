AI POWERED TALENT ACQUISITION: PnT Genie
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
As Jade continues to expand its business, our Talent Acquisition (TA) process must evolve to keep pace. Traditionally, the TA process has been manual, tedious, and inefficient — resulting in lost productivity and delays in hiring the right talent. This project leverages **Workato Genie (Agentic AI powered by Anthropic Claude)**, **Slack**, **Google Suite (Gmail + Calendar)**, and **Intelligent Document Processing (IDP)** in **Workato Apps** to build a next-generation TA assistant that automates repetitive workflows, ensures consistency, and provides actionable insights.

Side note- Zip File attached that is also known as Manifest, can be imported using recipe life cycle tool in Workato.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Introduction**

The Talent Acquisition team faces several challenges in hiring the right talent quickly and efficiently:
1. **Resume Screening** – Filtering hundreds of resumes against a job description is slow and inconsistent.
2. **Resume Standardization** – Client-facing resumes must follow Jade’s standard format, requiring cleanup, redaction, and formatting.
3. **Interview Scheduling & Coordination** – Manual coordination consumes significant effort in aligning schedules, handling reschedules, and sending reminders.
4. **Post-Offer Candidate Engagement** – Candidates must be kept “warm” until joining with personalized communications, onboarding material, and regular check-ins.

This project introduces an **Agentic AI-driven TA Assistant** that addresses these gaps by automating routine tasks, improving decision-making, and creating a seamless recruiter experience.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Representative Data**

1. **Resumes**: Unstructured PDF/Docx/Images (jpg, png etc) files.
2. **Job Descriptions** (JD): Text files capturing role, skills, and experience requirements.
3. **TA Process Data**: Interview schedules, recruiter notes, panel feedback, and offer details.
4. **Engagement Data**: Email follow-ups, onboarding material, and candidate interaction logs.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Executive Driven Questions**

The solution helps leaders and recruiters answer questions like:
1. Which resumes best match a given JD?
2. Are candidate resumes client-ready (standardized, clean, consistent)?
3. What is the interview pipeline health (scheduled, pending feedback, no-shows)?
4. Which candidates are at risk of dropping off after offer rollout?
5. How much manual recruiter effort has been saved by automation?

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Design Implementation**
<div align="center">

  <img width="3840" height="2161" alt="Untitled diagram _ Mermaid Chart-2025-09-14-151543" src="https://github.com/user-attachments/assets/2f5d24d1-ec22-40f9-9f68-9f30a421e82b" />

  <br>

  <img width="816" height="483" alt="AI-Powered Recruitment Automation System - visual selection" src="https://github.com/user-attachments/assets/eeb3d3f8-d089-49cf-9ab1-3e8226d696eb" />

</div>
 
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Analytical Framework**

The project uses a layered AI framework:
1. **Resume Parsing & Screening**: Workato Genie + LLM leveraged through/ using Slack evaluates resumes against JD in real-time. Candidate scoring based on skills, experience, and role fit.

2. **Resume Standardization**: Automated conversion of candidate resumes into Jade’s standard format, eliminating manual editing and ensuring consistency.

3. **Interview Scheduling & Feedback Management**: Slack integration for candidate/panel coordination with the help of Google Calender and GMail. Automated reminders to candidates reminding them of the scheduled interview.

4. **Post-Offer Engagement**: Automated, personalized Email follow-ups. AI-driven engagement check-ins to reduce dropouts.

5. **Knowledge Base**: Centralized repository of candidate data for recruiter insights and adding JD at run time. AI uses this knowledge base to evaluate candidates dynamically and respond to runtime prompts.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Knowledge Base**

The TA Genie uses a centralized Knowledge Base for candidate evaluation:

**Load Candidate data**: Knowledge base entry for resume parsing, backed by three recipes to handle resumes in different formats: PDF Resume Parser, DOCX Resume Parser, Image Resume Parser (OCR-enabled for scanned resumes/images).

This ensures every resume, regardless of format, is converted into structured data and stored in the Knowledge Base for evaluation.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Skills of the Genie**

The Genie has been equipped with multiple skills (Workato recipes) to automate recruiter workflows:

1. **Send Emails**: To internal PnT team, to candidates (acknowledgments, updates, follow-ups).

2. **Create Jade Resume**: Automatic conversion of raw resumes into Jade’s standard format.

3. **Read Attached File**: Intelligent parsing of resume files (PDF, DOCX, Image).

4. **Google Calendar Operations**: Create interview events, search available slots, update existing events.

Together, these skills allow the Genie to handle end-to-end TA workflows without manual intervention. 

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Working of the Model**

1. **Resume Intake**: Candidate resumes in PDF, DOCX, or Image formats are parsed using IDP recipes. Extracted structured data (skills, experience, education) is fed into the Knowledge Base.

2. **JD Processing**: Recruiter-uploaded JDs are parsed and stored in the Knowledge Base.

3. **Evaluation by Agentic AI**: Workato Genie powered by Anthropic Claude matches candidate resumes with JD requirements. Produces scores, shortlists, and Jade-standard resumes automatically.

4. **Workflow Orchestration**: AI triggers automation via Genie’s skills: Gmail → candidate/recruiter communications, Calendar → interview scheduling, updates, and reminders, Slack → recruiter interface for notifications and feedback.

5. **Feedback & Learning Loop**: Interview outcomes, recruiter feedback, and candidate engagement signals are stored back into the Knowledge Base. AI uses this updated data for runtime decision-making and future candidate evaluations.

---------------------------------------------------------

**Data Best Practices**

1. **Data Security**: Candidate personal data is redacted before AI processing.
2. **Data Consistency**: Standardized resume templates for client sharing.
3. **Data Governance**: Knowledge base segmented by JD, role, and candidate lifecycle stage.
4. **Runtime Processing**: AI can handle new resumes/JDs fed into the backend without retraining.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Insights and Impact**

1. **Efficiency**: Reduced recruiter time spent on resume screening and scheduling by >60%.
2. **Quality**: More consistent client-ready resumes with minimal manual effort.
3. **Speed**: Faster turnaround from resume submission to interview scheduling.
4. **Engagement**: Improved post-offer candidate connect, reducing dropout rates.
5. **Scalability**: AI scales seamlessly with increasing hiring volume without proportional recruiter overhead.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Tools Used**

1. **Workato Genie (Agentic AI powered by Anthropic Claude)** – Orchestration, automation, evaluation.

2. **Slack** – Recruiter/panel communication and bot interface.

3. **Google Suite** – Gmail → communication, Calendar → interview scheduling.

4. **Intelligent Document Processing (IDP)** – Parsing resumes in PDF, DOCX, and Image formats.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Conclusion**

This project transforms Jade’s TA process from a manual, reactive workflow into an AI-driven, proactive system. By combining Workato Genie, Slack, and Claude LLM, recruiters can focus on strategic hiring decisions while automation handles the heavy lifting.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
