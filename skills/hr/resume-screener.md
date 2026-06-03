# Skill: Resume Screener

| Category | HR |
| Version | 1.0 |
| Author | Kamrul Arafin |
| Last Updated | 2026 |
| License | MIT |

---

## What it does

Screens and ranks resumes against a job description, identifying top candidates and highlighting strengths and gaps for each applicant.

---

## How to use it

1. Copy the system prompt below
2. Paste it into Claude
3. Provide the job description
4. Paste multiple resumes
5. Get ranked candidates with scoring and notes

### Time needed: 5-10 minutes for 10-20 resumes

---

## System Prompt

```
You are an expert recruiter and hiring manager. Your job is to screen resumes and rank candidates by job fit.

When given a job description and a list of resumes, you will:
1. Create a scoring rubric based on the job description (skills, experience, education)
2. Score each candidate 1-10 on overall fit
3. Identify top 3-5 candidates
4. For each candidate, note:
   - Key strengths matching the role
   - Any gaps or concerns
   - Recommended next steps (interview, reject, maybe pile)
5. Provide a ranked list with brief recommendations

Format your response as:

## Job Requirements Analysis
- **Key Skills:** [Must-have skills from JD]
- **Experience Required:** [Years and type]
- **Education:** [Degree level required]
- **Nice-to-haves:** [Bonus qualifications]

## Candidate Rankings

### 1. [Candidate Name] — Score: 8.5/10
**Strengths:**
- [Strength 1]
- [Strength 2]

**Gaps/Concerns:**
- [Gap 1]

**Recommendation:** Interview — Strong fit for the role

---

### 2. [Candidate Name] — Score: 7/10
...

## Summary
- **Top Pick:** [Name] for [reason]
- **Other Strong Candidates:** [Names]
- **Pass/Reject:** [Names and reasons]

Remember: This is screening only. Conduct interviews to assess soft skills, culture fit, and actual capability.
```

---

## Example Input

```
JOB DESCRIPTION:

Position: Senior Software Engineer (Python/Backend)

Required:
- 5+ years backend software development
- Proficiency in Python
- Experience with relational databases (PostgreSQL, MySQL)
- Strong understanding of system design and scalability
- Experience with cloud platforms (AWS, GCP, Azure)
- B.S. in Computer Science or equivalent

Preferred:
- Open source contributions
- Experience with microservices architecture
- Experience with Kubernetes
- Previous startup experience
- Master's degree

---

RESUME 1:

JOHN SMITH
john@email.com | github.com/johnsmith

EXPERIENCE:
Senior Backend Engineer at TechCorp (2020-2024)
- Led backend architecture for 3 microservices, serving 2M+ users
- Optimized database queries, reducing response time by 40%
- Mentored 4 junior engineers
- Tech stack: Python, PostgreSQL, Docker, Kubernetes, AWS

Backend Engineer at StartupXYZ (2018-2020)
- Built REST APIs using Python (Flask, FastAPI)
- Designed and implemented database schema
- Deployed to AWS using EC2 and RDS

EDUCATION:
B.S. Computer Science, State University (2018)
Relevant Coursework: Data Structures, Algorithms, Database Design

SKILLS:
Python, PostgreSQL, MySQL, AWS, Docker, Kubernetes, Git, SQL

---

RESUME 2:

JANE DOE
jane@email.com

EXPERIENCE:
Full Stack Developer at WebAgency (2019-2024)
- Built web applications using Django and React
- Some backend work with Python and MySQL
- Deployed to shared hosting and AWS
- Created and maintained WordPress sites

Junior Developer at TechStart (2018-2019)
- HTML/CSS/JavaScript development
- Basic Python scripting

EDUCATION:
B.A. Business (2018)
Self-taught coding through online courses

SKILLS:
Python, JavaScript, React, MySQL, AWS, WordPress

---

RESUME 3:

ALEX JOHNSON
alex@email.com | github.com/alexjohnson

EXPERIENCE:
Software Engineer at BigTech (2017-2024)
- Worked on cloud infrastructure team
- Built internal tools in Go and Python
- Experience with GCP and Kubernetes
- Some microservices experience

Intern at TechInc (2016-2017)
- Python scripting and automation
- Linux systems administration

EDUCATION:
B.S. Computer Science, Top University (2017)

SKILLS:
Go, Python, Kubernetes, GCP, Linux, Docker, Microservices

---

RESUME 4:

MARIA GARCIA
maria@email.com

EXPERIENCE:
Senior DevOps Engineer at CloudCorp (2019-2024)
- Infrastructure and deployment automation
- AWS and Kubernetes expertise
- Shell scripting and CI/CD pipelines

Frontend Developer at DesignStudio (2017-2019)
- React, JavaScript, CSS
- Web design and user experience

EDUCATION:
Certification in Cloud Computing (2019)
High School Diploma (2015)

SKILLS:
AWS, Kubernetes, Docker, Shell Scripting, JavaScript, React
```

## Example Output

## Job Requirements Analysis
- **Key Skills:** Python, PostgreSQL/MySQL, System Design, Cloud (AWS/GCP/Azure)
- **Experience Required:** 5+ years backend software development
- **Education:** B.S. Computer Science (or equivalent)
- **Nice-to-haves:** Open source, microservices, Kubernetes, startup experience

---

## Candidate Rankings

### 1. JOHN SMITH — Score: 9.2/10 ⭐
**Strengths:**
- ✅ 6 years total backend experience (exceeds 5-year requirement)
- ✅ Expert in Python and PostgreSQL (exactly what's needed)
- ✅ Extensive Kubernetes and AWS experience
- ✅ Led microservices architecture (shows senior-level skills)
- ✅ B.S. in Computer Science (meets education requirement)
- ✅ Mentoring experience (shows leadership)
- ✅ System design and optimization expertise

**Gaps/Concerns:**
- Only mentions AWS, not experience with GCP/Azure (minor — AWS is primary)

**Recommendation:** 🎯 **Interview — Strong fit. This is likely your top candidate.**

Why: Nearly perfect match. Has all required skills, exceeds experience requirement, proven track record with microservices and scale. Ready for senior role immediately.

---

### 2. ALEX JOHNSON — Score: 7.1/10
**Strengths:**
- ✅ 7 years experience (exceeds requirement)
- ✅ Python experience
- ✅ Kubernetes and microservices (preferred skills)
- ✅ GCP experience
- ✅ B.S. Computer Science
- ✅ Strong infrastructure understanding

**Gaps/Concerns:**
- ❌ Primary language is Go, not Python (may need ramp-up time)
- ⚠️ Background is infrastructure/DevOps, not backend development
- ⚠️ No mention of relational databases (PostgreSQL/MySQL)
- ⚠️ Limited REST API or application backend experience

**Recommendation:** 📋 **Maybe pile — Consider if backend engineers are hard to find.**

Why: Has some of the right skills but background is infrastructure-focused, not application development. Would likely need training on relational databases and backend architecture. Could work if willing to transition from DevOps.

---

### 3. JANE DOE — Score: 5.3/10
**Strengths:**
- ✅ Python experience
- ✅ MySQL experience
- ✅ AWS experience
- ✅ 5+ years web development experience

**Gaps/Concerns:**
- ❌ Only 1 year dedicated backend experience (need 5+)
- ❌ B.A. in Business, not Computer Science (doesn't meet education)
- ❌ Primary background is full stack / frontend
- ❌ No mention of system design or architecture
- ❌ No Kubernetes or Docker experience
- ❌ Mostly shared hosting, not cloud-native work

**Recommendation:** ❌ **Pass — Not ready for senior role.**

Why: Strong web developer but lacks depth in backend engineering and architecture. Would be overqualified as a junior engineer but underqualified for this senior role. Consider for mid-level positions instead.

---

### 4. MARIA GARCIA — Score: 4.2/10
**Strengths:**
- ✅ AWS and Kubernetes expertise
- ✅ Infrastructure knowledge
- ✅ 5+ years professional experience

**Gaps/Concerns:**
- ❌ No Python mentioned (core requirement)
- ❌ Background is DevOps/frontend, not backend development
- ❌ No relational database experience mentioned
- ❌ No system design or backend architecture background
- ❌ Only certification, no degree (doesn't meet education)
- ❌ Significant role transition needed

**Recommendation:** ❌ **Pass — Wrong specialization.**

Why: Strong DevOps engineer and good infrastructure knowledge, but not a software engineer. Would require complete retraining to do backend development. Better fit for DevOps or Infrastructure positions.

---

## Summary

**Recommendation:** **Interview John Smith first.**

- **Top Pick:** JOHN SMITH (9.2/10) — Nearly perfect fit. Has all required skills, proven experience at scale, and leadership ability.
- **Consider Second:** ALEX JOHNSON (7.1/10) — If John doesn't work out, consider Alex, but expect 2-3 month ramp-up on backend-specific knowledge.
- **Pass on:** JANE DOE (5.3/10) and MARIA GARCIA (4.2/10) — Both are good at what they do, but don't match this role's requirements.

**Next Steps:**
1. Contact John Smith for phone screen
2. Ask about database optimization experience and microservices decisions
3. Do technical assessment on system design if promising
4. If John passes, no need to interview others; if he declines, reach out to Alex

---

## Tips & Variations

### Customize for different roles:
- **Frontend:** Adjust keywords (React, Vue, TypeScript, CSS, UX)
- **Full Stack:** Look for balanced backend and frontend experience
- **DevOps:** Prioritize infrastructure, CI/CD, cloud platforms
- **Data Science:** Look for Python, SQL, statistics, machine learning

### Get more detail:
- Ask for "red flags" analysis per candidate
- Request "interview questions" tailored to each candidate
- Get "culture fit" assessment if you provide company info
- Ask for "compensation range estimate" based on experience

### Pro tips:
- Always phone screen top candidates before bringing in for technical interview
- Ask technical questions relevant to their background (don't ask about Go from Alex if he's DevOps)
- Check references and past work
- Be transparent about role and growth opportunities

---

## Common Issues

**Q: Should I invite all top candidates or just the top one?**
A: Typically interview top 2-3. Going too deep wastes your time.

**Q: One resume looks perfect but has a gap?**
A: Ask about the gap in the interview, but don't disqualify. Could be legitimate (sabbatical, relocation, etc.)

**Q: I don't have enough information**
A: Ask for cover letters or phone screen answers. Resumes don't tell the whole story.

**Q: None of the candidates are perfect**
A: That's normal. Look for the best fit and trainability on missing skills.

---

## Related Skills

- [`job-description-writer.md`](./job-description-writer.md) — Write better job postings to attract candidates
- [`interview-prep.md`](./interview-prep.md) — Prepare candidates for interviews

---

## Tags

#hiring #recruitment #screening #jobs #hr #talent

---

## Notes

- This is screening only — always conduct interviews to assess soft skills and actual ability
- Try before you buy — have top candidates complete a small technical test/task
- Be transparent about the role, salary range, and growth opportunities
- Hire for cultural fit + learning ability, not just skills match
- Some people exceed resumes — don't discount good candidates due to formatting
