As Jade continues to expand its business, our Talent Acquisition (TA) process must evolve to keep pace. Traditionally, the TA process has been manual, tedious, and inefficient — resulting in lost productivity and delays in hiring the right talent.
This project leverages Workato Genie, Slack, and Agentic AI (powered by Anthropic Claude) to build a next-generation TA assistant that automates repetitive workflows, ensures consistency, and provides actionable insights.
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Introduction**

The Talent Acquisition team faces several challenges in hiring the right talent quickly and efficiently:
1. Resume Screening – Filtering hundreds of resumes against a job description is slow and inconsistent.
2. Resume Standardization – Client-facing resumes must follow Jade’s standard format, requiring cleanup, redaction, and formatting.
3. Interview Scheduling & Coordination – Manual coordination consumes significant effort in aligning schedules, handling reschedules, and sending reminders.
4. Post-Offer Candidate Engagement – Candidates must be kept “warm” until joining with personalized communications, onboarding material, and regular check-ins.

This project introduces an Agentic AI-driven TA Assistant that addresses these gaps by automating routine tasks, improving decision-making, and creating a seamless recruiter experience.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Representative Data**

1. Resumes: Unstructured PDF/Docx/Images (jpg, png etc) files submitted by candidates.
2. Job Descriptions (JD): Text files capturing role, skills, and experience requirements.
3. TA Process Data: Interview schedules, recruiter notes, panel feedback, and offer details.
4. Engagement Data: Email/Slack follow-ups, onboarding material, and candidate interaction logs.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Executive Driven Questions**

The solution helps leaders and recruiters answer questions like:
1. Which resumes best match a given JD?
2. Are candidate resumes client-ready (standardized, clean, consistent)?
3. What is the interview pipeline health (scheduled, pending feedback, no-shows)?
4. Which candidates are at risk of dropping off after offer rollout?
5. How much manual recruiter effort has been saved by automation?

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Analytical Framework**

The project uses a layered AI framework:
1. Resume Parsing & Screening

  -Workato Genie + LLM evaluates resumes against JD in real-time.
  -Candidate scoring based on skills, experience, and role fit.

2. Resume Standardization
  -Automatic removal of personal details.
  -Grammar/spelling correction and template formatting.

3. Interview Scheduling & Feedback Management
  -Slack integration for candidate/panel coordination.
  -Automated reminders and post-interview feedback collection.

4. Post-Offer Engagement
  -Automated, personalized Slack/Email follow-ups.
  -AI-driven engagement check-ins to reduce dropouts.

5. Knowledge Base
  -Centralized repository of JDs, candidate data, and recruiter insights.
  -AI uses this knowledge base to evaluate candidates dynamically and respond to runtime prompts.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
