# Automated AI Intelligence Agent

An end-to-end AI agent that collects YouTube content, analyzes trends using LLMs, generates executive-style PDF reports, and delivers them automatically via email.

## 1 Minute Project Overview

**Problem**  
Keeping up with fast-moving AI and tech content required hours of manual effort every week. Information was scattered across multiple platforms, making it difficult to extract meaningful insights and trends.

**Context & Realisation**  
While exploring automation and AI tools, I realized that most existing solutions either provided raw links or surface-level summaries. There was no system that converted unstructured content into actionable, decision-ready insights.

**Solution**  
I designed and built an autonomous AI agent using n8n and JavaScript that collects content, analyzes it using LLMs, generates structured reports, converts them into PDFs, and delivers them automatically via email. The system runs without manual effort using n8n, JavaScript, LLM APIs, and PDF automation

**Result**  
- Reduced manual research time by 90%
- Delivered consistent, high-quality weekly reports
- Created a scalable and reusable intelligence system
  
**if you want to see more, keep scrolling :)**
---


## Problem Statement

Staying updated with fast moving AI content on YouTube and blogs is time consuming. Most professionals don’t have time to watch hours of videos every week.
There was no simple way to:
- Collect relevant content
- Analyze it
- Summarize insights
- Deliver it in a clean format
I wanted to solve this using automation and AI.

---

## Key Challenges

- Research required significant time investment
- Insights lacked structure and consistency
- All processes were manual
- System couldn't scale efficiently

This created a need for an automated intelligence pipeline.

---

## Solution

I designed an AI agent that automates the entire research and reporting pipeline.

The system performs the following functions:

1. Automatically collects fresh content
2. Filters recent and relevant data
3. Structures raw inputs
4. Uses LLMs for analysis
5. Generates professional reports
6. Sends outputs via email

The goal was to build a system that works reliably with minimal maintenance.
---

## System Architecture:
<img width="1695" height="711" alt="Screenshot 2026-02-04 at 4 33 46 PM" src="https://github.com/user-attachments/assets/4e1b6992-5586-4cd2-b03d-710d0d57200a" />

### **Workflow Overview**

1. Scheduler: Triggers weekly execution
2. RSS Feeds: Content ingestion
3. XML Parser: Data conversion
4. JavaScript Nodes: Data processing
5. LLM APIs: Insight generation
6. Gmail API: Distribution

## Implementation Details:
### **Data Ingestion**

The system fetches data using RSS feeds and filters entries based on publication dates to ensure only recent content is processed.

Custom logic was implemented to handle inconsistent metadata and missing fields.

### **Data Processing**

Using JavaScript nodes, the pipeline:

- Normalizes data formats
- Extracts relevant attributes
- Removes duplicates
- Prepares structured prompts

### **AI Integration**

Prompt engineering was a critical component.

Each request to the LLM includes:

- Contextual data
- Formatting instructions
- Output structure
- Analysis requirements

This ensures consistent and high quality outputs.

 **Sample Output**

The system generates weekly reports that resemble internal intelligence briefs.
<img width="1990" height="1126" alt="Screenshot 2026-02-04 at 4 37 58 PM" src="https://github.com/user-attachments/assets/535b8bcd-a6d1-4622-ae5a-b207bdbce261" /> <img width="1440" height="900" alt="Screenshot 2026-02-04 at 4 39 40 PM" src="https://github.com/user-attachments/assets/932196dc-c6fe-4de4-9ce4-62f67d4b370a" />

---

## **Impact:**

### **Quantitative Impact**

- Reduced manual research by 90%
- Automated weekly insights
- Zero manual intervention

### **Qualitative Impact**

- Improved consistency
- Faster understanding of trends
- Better information quality
- Scalable knowledge system
---
## **Challenges & Iterations**

### **Major Challenges**

- API quota limits
- JSON formatting errors
- Data inconsistencies
- Debugging multi-node workflows

### **How I Solved Them**

- Added fallback logic
- Implemented retries
- Optimized prompts
- Improved parsing logic
---
