# Daily News Brief
An AI-powered automated news website that fetches the latest Indian and World news from multiple RSS feeds, summarizes the articles using Google's Gemini AI, generates a modern HTML news portal, and automatically deploys it to GitHub Pages every day using n8n.

---

## Features
* Fetches Indian and World news
* Collects news from multiple trusted RSS feeds
* AI-generated summaries using Google Gemini
* Displays article images when available
* Includes upcoming events in India
* Generates a responsive newspaper-style website
* Automatically updates GitHub Pages
* Scheduled execution every day at 6:00 AM

---

## News Sources

### Hindustan Times
* India News
* World News
* Entertainment

### India Today
* Home
* India
* World

---

## Tech Stack
* n8n
* Google Gemini API
* GitHub API
* RSS Feeds
* HTML5
* CSS3
* JavaScript
* GitHub Pages

---

## Project Structure
```text
daily-news-brief/
│
├── index.html
├── README.md
└── n8n-workflows/
    └── News Summarizer Website Final Draft.json
```

---

## Workflow
```text
Schedule Trigger (6 AM)
        │
        ▼
Fetch RSS Feeds
        │
        ▼
Fetch Events
        │
        ▼
Merge All Data
        │
        ▼
Gemini AI Summarization
        │
        ▼
Generate HTML Website
        │
        ▼
Get GitHub File SHA
        │
        ▼
Update index.html
        │
        ▼
GitHub Pages Deployment
```

---

## Website Features
* Responsive newspaper-style layout
* Indian News section
* World News section
* News grouped by publication
* AI-generated summaries
* Direct links to original articles
* Images (when available)
* Upcoming Events section
* Automatic daily updates

---

## Environment Setup
Configure the following credentials in n8n:

### Google Gemini API
Add your Google Gemini API key.

### GitHub
Create a GitHub Personal Access Token with the following permissions:

* `repo`
* `workflow` (optional)

Connect it as a GitHub credential in n8n.

---

## Installation
Clone the repository:

```bash
git clone https://github.com/Vinaykumar1311/daily-news-brief.git
```

Navigate into the project directory:

```bash
cd daily-news-brief
```

Import the workflow into n8n:

```text
News Summarizer Website Final Draft.json
```

Configure your Google Gemini API and GitHub credentials, then run the workflow.
---

## Deployment
The workflow automatically updates the `index.html` file using the GitHub Contents API. GitHub Pages serves the latest generated version of the website.
---

## Automation
Every day the workflow:
1. Fetches RSS feeds.
2. Fetches upcoming events.
3. Merges all collected data.
4. Uses Google Gemini to summarize the articles.
5. Generates the HTML website.
6. Updates `index.html` in the GitHub repository.
7. GitHub Pages publishes the latest version automatically.

---

## Author
**Vinay Kumar**
GitHub: https://github.com/Vinaykumar1311


