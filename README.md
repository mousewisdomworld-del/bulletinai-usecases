# BulletinAI use cases

Open data companion to [BulletinAI](https://bulletinai.app), a cross-platform directory of AI agent use cases and playbooks.

BulletinAI collects credited examples of work people hand to an AI agent: clearing an inbox, preparing for a meeting, drafting a briefing, running a content workflow, or keeping a household on track. Each entry is a short playbook with the outcome, the platform it runs on, who it is for, how hard it is to set up, the tools involved, and the steps.

This repository publishes that catalog: **65 use cases** in [`data/usecases.json`](data/usecases.json), tagged with the taxonomy in [`data/categories.md`](data/categories.md). The live directory serves the same playbooks at [`https://bulletinai.app/api/usecases.json`](https://bulletinai.app/api/usecases.json). The copy in this repo omits affiliate fields and adds a `bulletin_url` for each entry that has a page.

## How entries are organized

Every use case is classified on four axes.

| Axis | What it describes | Values |
| --- | --- | --- |
| Outcome | The job the agent is doing | Inbox & email · Calendar & planning · Research & briefings · Content & social · Sales & CRM · Meetings & notes · Personal life & health · Learning & education · Business ops & analysis |
| Platform | Where you run the playbook | OpenClaw · ChatGPT (agent mode, Tasks, workspace agents) · Claude (chat, connectors) · Gemini (Gems, Notebook) · n8n · Zapier · Make · Other |
| Role | Who it is for | Founder/solopreneur · Marketer · Sales · Ops/manager · Educator/student · Personal/household |
| Difficulty | How much setup it takes | No-code (chat only) · Low-code (connect apps or import a template) · Technical (self-host, API keys) |

A single entry can name more than one platform. The current catalog uses OpenClaw, ChatGPT, Claude, Gemini, n8n, Zapier, Make, Lindy, Relevance AI, and Microsoft Copilot. The taxonomy file groups tools beyond its named list under **Other**; entries still record the product name.

Each entry also has a status:

- **community** — shared from a community list or template and not yet checked by BulletinAI
- **official example** — taken from the vendor’s own docs, academy, or template gallery
- **verified** — tested by BulletinAI

Setup times are estimates.

## Catalog

Entries below are grouped by outcome. **Source** is the original writeup. **BulletinAI** links to the page on [bulletinai.app](https://bulletinai.app). Page URLs follow the `id` field in the [use cases API](https://bulletinai.app/api/usecases.json): `https://bulletinai.app/u/{id}`. All 65 ids in this dataset resolve to a live page.

### Inbox & email

7 use cases.

| Title | Platforms | Difficulty | Source | BulletinAI |
| --- | --- | --- | --- | --- |
| Inbox De-clutter: newsletter digest | OpenClaw | Technical | [awesome-openclaw-usecases (hesamsheikh, GitHub)](https://github.com/hesamsheikh/awesome-openclaw-usecases) | [page](https://bulletinai.app/u/03-inbox-de-clutter-newsletter-digest) |
| AI Gmail triage with draft replies | n8n | Low-code | [n8n community template](https://n8n.io/workflows/20570-triage-gmail-inbox-emails-and-draft-replies-with-openai-and-google-sheets/) | [page](https://bulletinai.app/u/28-ai-gmail-triage-with-draft-replies) |
| Email summaries & labels logged to Notion/Sheets | n8n | Low-code | [n8n community template](https://n8n.io/workflows/9679-automated-email-management-with-gemini-ai-gmail-summarizing-labeling-and-notionsheets-logging/) | [page](https://bulletinai.app/u/29-email-summaries-labels-logged-to-notion-sheets) |
| Summarize emails and post to Slack | Make | Low-code | [Make template](https://www.make.com/templates/11243-summarize-emails-with-openai-and-send-it-on-slack) | [page](https://bulletinai.app/u/31-summarize-emails-and-post-to-slack) |
| Summarize a week of emails on a project | Microsoft Copilot | No-code | [Microsoft Support](https://support.microsoft.com/en-us/outlook/copilot-outlook/chat-with-copilot-in-outlook) | [page](https://bulletinai.app/u/55-summarize-a-week-of-emails-on-a-project) |
| Prioritize unread email (Copilot license) | Microsoft Copilot | No-code | [Microsoft Support](https://support.microsoft.com/en-us/outlook/copilot-outlook/chat-with-copilot-in-outlook) | [page](https://bulletinai.app/u/56-prioritize-unread-email-copilot-license) |
| Copilot prompt gallery: who's waiting on me | Microsoft Copilot | No-code | [Microsoft Adoption prompt gallery](https://www.adoption.microsoft.com/en-us/copilot/prompt-gallery/) | [page](https://bulletinai.app/u/59-copilot-prompt-gallery-who-s-waiting-on-me) |

### Calendar & planning

5 use cases.

| Title | Platforms | Difficulty | Source | BulletinAI |
| --- | --- | --- | --- | --- |
| Event Guest Confirmation by phone | OpenClaw | Technical | [awesome-openclaw-usecases (hesamsheikh, GitHub)](https://github.com/hesamsheikh/awesome-openclaw-usecases) | [page](https://bulletinai.app/u/10-event-guest-confirmation-by-phone) |
| Quickly prep for your week | Claude | Low-code | [Anthropic — Claude for personal use](https://www.anthropic.com/learn/claude-for-you) | [page](https://bulletinai.app/u/19-quickly-prep-for-your-week) |
| Turn emails into an event tracker | Claude | No-code | [Claude — Use cases gallery](https://claude.com/resources/use-cases) | [page](https://bulletinai.app/u/21-turn-emails-into-an-event-tracker) |
| AI meeting scheduler you CC on email | Lindy | No-code | [Lindy template](https://www.lindy.ai/templates/meeting-scheduler) | [page](https://bulletinai.app/u/49-ai-meeting-scheduler-you-cc-on-email) |
| Build a balanced weekly work plan | ChatGPT | No-code | [OpenAI Academy — ChatGPT for any role](https://academy.openai.com/public/clubs/work-users-ynjqu/resources/chatgpt-for-any-role) | [page](https://bulletinai.app/u/60-build-a-balanced-weekly-work-plan) |

### Research & briefings

8 use cases.

| Title | Platforms | Difficulty | Source | BulletinAI |
| --- | --- | --- | --- | --- |
| Daily Reddit Digest | OpenClaw | Technical | [awesome-openclaw-usecases (hesamsheikh, GitHub)](https://github.com/hesamsheikh/awesome-openclaw-usecases) | [page](https://bulletinai.app/u/01-daily-reddit-digest) |
| Daily YouTube Digest | OpenClaw | Technical | [awesome-openclaw-usecases (hesamsheikh, GitHub)](https://github.com/hesamsheikh/awesome-openclaw-usecases) | [page](https://bulletinai.app/u/02-daily-youtube-digest) |
| Competitor analysis slide deck | ChatGPT | No-code | [OpenAI — Introducing ChatGPT agent](https://openai.com/index/introducing-chatgpt-agent/) | [page](https://bulletinai.app/u/14-competitor-analysis-slide-deck) |
| Weekday competitor & market briefing | ChatGPT | No-code | [OpenAI Academy — Tasks](https://academy.openai.com/public/clubs/work-users-ynjqu/resources/tasks) | [page](https://bulletinai.app/u/15-weekday-competitor-market-briefing) |
| Research docs to podcast-style overview | Gemini | No-code | [Google Workspace — Gemini at work guide](https://workspace.google.com/learning/report/content/geminiatworkapracticalguide) | [page](https://bulletinai.app/u/27-research-docs-to-podcast-style-overview) |
| Weekly AI-curated RSS digest to your inbox | n8n | Low-code | [n8n community template](https://n8n.io/workflows/16037-send-a-weekly-aicurated-rss-digest-email-with-openai-and-gmail/) | [page](https://bulletinai.app/u/48-weekly-ai-curated-rss-digest-to-your-inbox) |
| 'Catch me up' briefing after time off | Lindy | No-code | [Lindy use cases](https://www.lindy.ai/use-cases) | [page](https://bulletinai.app/u/51-catch-me-up-briefing-after-time-off) |
| 30-day project synthesis across email, meetings and chats | Microsoft Copilot | No-code | [Microsoft Learning lab](https://microsoftlearning.github.io/MS-4004-Empower-workforce-copilot-use-cases/Instructions/Labs/M01-empower-workforce-copilot-executives/01-Ex1-1-use-teams-synthesize-communications.html) | [page](https://bulletinai.app/u/58-30-day-project-synthesis-across-email-meetings-and) |

### Content & social

9 use cases.

| Title | Platforms | Difficulty | Source | BulletinAI |
| --- | --- | --- | --- | --- |
| Podcast Production Pipeline | OpenClaw | Technical | [awesome-openclaw-usecases (hesamsheikh, GitHub)](https://github.com/hesamsheikh/awesome-openclaw-usecases) | [page](https://bulletinai.app/u/08-podcast-production-pipeline) |
| Shared brand-voice copywriter Gem | Gemini | No-code | [Google Workspace Blog](https://workspace.google.com/blog/product-announcements/5-ways-to-boost-your-teams-productivity-with-the-gemini-app-featuring-new-sharable-gems) | [page](https://bulletinai.app/u/25-shared-brand-voice-copywriter-gem) |
| Sheets content calendar to scheduled social posts | Make | Low-code | [Make template](https://www.make.com/templates/14959-filter-rows-in-google-sheets-and-create-social-media-posts-with-chatgpt-and-buffer) | [page](https://bulletinai.app/u/32-sheets-content-calendar-to-scheduled-social-posts) |
| Weekly newsletter digest drafted from RSS | n8n | Low-code | [n8n community template](https://n8n.io/workflows/17539-draft-weekly-newsletter-digests-from-rss-feeds-with-openai-and-kit/) | [page](https://bulletinai.app/u/33-weekly-newsletter-digest-drafted-from-rss) |
| Daily AI news to LinkedIn post draft | n8n | Low-code | [n8n community template](https://n8n.io/workflows/5068-daily-ai-news-digest-to-linkedin-posts-with-openai-gpt-and-rss-feeds/) | [page](https://bulletinai.app/u/34-daily-ai-news-to-linkedin-post-draft) |
| Turn a monitored website into social posts | Make | Low-code | [Make template](https://www.make.com/templates/12103-summarize-content-with-chatgpt-from-a-monitored-site-using-browse-ai-and-create-a-social-media-posts) | [page](https://bulletinai.app/u/38-turn-a-monitored-website-into-social-posts) |
| New WordPress post to Facebook Page post | Make | Low-code | [Make template](https://www.make.com/templates/13664-create-engaging-social-media-posts-using-wordpress-and-chatgpt) | [page](https://bulletinai.app/u/39-new-wordpress-post-to-facebook-page-post) |
| Draft blog posts from form submissions | Zapier | Low-code | [Zapier automation template](https://zapier.com/automations/marketing/content-marketing/content-generation/create-draft-blog-posts-from-form-submissions-for-founders) | [page](https://bulletinai.app/u/40-draft-blog-posts-from-form-submissions) |
| Use a Gem inside Docs/Gmail side panel | Gemini | No-code | [Google Workspace Updates](https://workspaceupdates.googleblog.com/2025/07/gems-in-the-side-panel-of-google-workspace-apps.html) | [page](https://bulletinai.app/u/65-use-a-gem-inside-docs-gmail-side-panel) |

### Sales & CRM

7 use cases.

| Title | Platforms | Difficulty | Source | BulletinAI |
| --- | --- | --- | --- | --- |
| Personal CRM from email & calendar | OpenClaw | Technical | [awesome-openclaw-usecases (hesamsheikh, GitHub)](https://github.com/hesamsheikh/awesome-openclaw-usecases) | [page](https://bulletinai.app/u/04-personal-crm-from-email-calendar) |
| Weekly key-account news scan | ChatGPT | No-code | [OpenAI Academy — Tasks](https://academy.openai.com/public/clubs/work-users-ynjqu/resources/tasks) | [page](https://bulletinai.app/u/16-weekly-key-account-news-scan) |
| Fathom meeting summaries onto CRM leads | Zapier | Low-code | [Zapier automation template](https://zapier.com/automations/sales/crm-management/activity-logging/add-ai-meeting-summaries-to-crm-lead-records) | [page](https://bulletinai.app/u/30-fathom-meeting-summaries-onto-crm-leads) |
| Enrich new leads with ChatGPT, create in Salesforce, ping Slack | Make | Low-code | [Make template](https://www.make.com/templates/11998-enrich-lead-s-company-data-with-chatgpt-create-leads-in-salesforce-and-send-slack-notifications) | [page](https://bulletinai.app/u/35-enrich-new-leads-with-chatgpt-create-in-salesforce) |
| Transcribe sales calls and score lead qualification | Zapier | Low-code | [Zapier template](https://zapier.com/templates/details/7890cd8b687c9f3fc78336b98bdf8a7d5dd4b20785229e5d18eef7f892e2087d) | [page](https://bulletinai.app/u/43-transcribe-sales-calls-and-score-lead-qualificatio) |
| AI sales researcher pre-call briefs | Relevance AI | No-code | [Relevance AI marketplace](https://marketplace.relevanceai.com/agents/sales-researcher) | [page](https://bulletinai.app/u/53-ai-sales-researcher-pre-call-briefs) |
| Prospect research workflow | Relevance AI | Low-code | [Relevance AI docs](https://relevanceai.com/docs/guides/sales/prospect-research-use-case) | [page](https://bulletinai.app/u/54-prospect-research-workflow) |

### Meetings & notes

5 use cases.

| Title | Platforms | Difficulty | Source | BulletinAI |
| --- | --- | --- | --- | --- |
| Meeting Notes to Assigned Action Items | OpenClaw | Technical | [awesome-openclaw-usecases (hesamsheikh, GitHub)](https://github.com/hesamsheikh/awesome-openclaw-usecases) | [page](https://bulletinai.app/u/11-meeting-notes-to-assigned-action-items) |
| Client meeting prep briefing | ChatGPT | No-code | [OpenAI — Introducing ChatGPT agent](https://openai.com/index/introducing-chatgpt-agent/) | [page](https://bulletinai.app/u/12-client-meeting-prep-briefing) |
| Meeting notes to owner task list | ChatGPT | No-code | [OpenAI Academy — ChatGPT for any role](https://academy.openai.com/public/clubs/work-users-ynjqu/resources/chatgpt-for-any-role) | [page](https://bulletinai.app/u/17-meeting-notes-to-owner-task-list) |
| Close the loop after a meeting | Lindy | No-code | [Lindy use cases](https://www.lindy.ai/use-cases) | [page](https://bulletinai.app/u/52-close-the-loop-after-a-meeting) |
| Catch up on a Teams chat | Microsoft Copilot | No-code | [Microsoft Support](https://support.microsoft.com/en-us/teams/copilot/how-to-use-microsoft-365-copilot-in-teams-chats-and-channels) | [page](https://bulletinai.app/u/57-catch-up-on-a-teams-chat) |

### Personal life & health

7 use cases.

| Title | Platforms | Difficulty | Source | BulletinAI |
| --- | --- | --- | --- | --- |
| Family Calendar & Household Assistant | OpenClaw | Technical | [awesome-openclaw-usecases (hesamsheikh, GitHub)](https://github.com/hesamsheikh/awesome-openclaw-usecases) | [page](https://bulletinai.app/u/05-family-calendar-household-assistant) |
| Habit Tracker & Accountability Coach | OpenClaw | Technical | [awesome-openclaw-usecases (hesamsheikh, GitHub)](https://github.com/hesamsheikh/awesome-openclaw-usecases) | [page](https://bulletinai.app/u/06-habit-tracker-accountability-coach) |
| Health & Symptom Tracker | OpenClaw | Technical | [awesome-openclaw-usecases (hesamsheikh, GitHub)](https://github.com/hesamsheikh/awesome-openclaw-usecases) | [page](https://bulletinai.app/u/07-health-symptom-tracker) |
| Plan and shop a dinner party | ChatGPT | No-code | [OpenAI — Introducing ChatGPT agent](https://openai.com/index/introducing-chatgpt-agent/) | [page](https://bulletinai.app/u/13-plan-and-shop-a-dinner-party) |
| Digital recipe cards from handwriting | Claude | No-code | [Claude — Use cases gallery](https://claude.com/resources/use-cases) | [page](https://bulletinai.app/u/22-digital-recipe-cards-from-handwriting) |
| WhatsApp receipt bot | n8n | Technical | [n8n community template](https://n8n.io/workflows/9285-process-receipt-images-with-gpt-4o-mini-whatsapp-and-google-sheets-automation/) | [page](https://bulletinai.app/u/47-whatsapp-receipt-bot) |
| Daily travel itinerary | Claude | No-code | [Claude — Use cases gallery](https://claude.com/resources/use-cases) | [page](https://bulletinai.app/u/63-daily-travel-itinerary) |

### Learning & education

3 use cases.

| Title | Platforms | Difficulty | Source | BulletinAI |
| --- | --- | --- | --- | --- |
| Plan your syllabus | Claude | No-code | [Claude — Education use cases](https://claude.com/resources/use-cases-category/education) | [page](https://bulletinai.app/u/23-plan-your-syllabus) |
| Practice case interviews with feedback | Claude | No-code | [Claude — Education use cases](https://claude.com/resources/use-cases-category/education) | [page](https://bulletinai.app/u/24-practice-case-interviews-with-feedback) |
| Interview coach Gem | Gemini | No-code | [Google Workspace Blog](https://workspace.google.com/blog/product-announcements/new-gemini-gems-deeper-knowledge-and-business-context) | [page](https://bulletinai.app/u/26-interview-coach-gem) |

### Business ops & analysis

14 use cases.

| Title | Platforms | Difficulty | Source | BulletinAI |
| --- | --- | --- | --- | --- |
| Multi-Channel AI Customer Service | OpenClaw | Technical | [awesome-openclaw-usecases (hesamsheikh, GitHub)](https://github.com/hesamsheikh/awesome-openclaw-usecases) | [page](https://bulletinai.app/u/09-multi-channel-ai-customer-service) |
| Vendor quote decision matrix | ChatGPT | Low-code | [OpenAI Academy — Workspace agents](https://openai.com/academy/workspace-agents/) | [page](https://bulletinai.app/u/18-vendor-quote-decision-matrix) |
| Compare competing vendor proposals | Claude | No-code | [Anthropic — Claude for personal use](https://www.anthropic.com/learn/claude-for-you) | [page](https://bulletinai.app/u/20-compare-competing-vendor-proposals) |
| Reply to Google Business reviews with AI | Make | Low-code | [Make template](https://www.make.com/templates/15259-respond-to-google-my-business-reviews-using-openai-gpt-3-completions) | [page](https://bulletinai.app/u/36-reply-to-google-business-reviews-with-ai) |
| Log Google reviews to Airtable with draft ChatGPT replies | Make | Low-code | [Make template](https://www.make.com/templates/15168-monitor-google-my-business-reviews-and-create-records-in-airtable-with-chatgpt-responses) | [page](https://bulletinai.app/u/37-log-google-reviews-to-airtable-with-draft-chatgpt-) |
| Classify Google Forms responses with ChatGPT | Zapier | Low-code | [Zapier template](https://zapier.com/apps/chatgpt/integrations/google-forms/255593615/classify-new-google-forms-responses-with-chatgpt) | [page](https://bulletinai.app/u/41-classify-google-forms-responses-with-chatgpt) |
| Structured feedback records from intake forms | Zapier | Low-code | [Zapier automation template](https://zapier.com/automations/product/product-feedback-management/feedback-categorization-routing/add-structured-feedback-records-from-new-intake-forms) | [page](https://bulletinai.app/u/42-structured-feedback-records-from-intake-forms) |
| Receipt photos to an expense sheet | n8n | Low-code | [n8n community template](https://n8n.io/workflows/12954-receipt-processing-ai-agent-with-step-by-step-video/) | [page](https://bulletinai.app/u/44-receipt-photos-to-an-expense-sheet) |
| Invoice PDFs to booking list with auto-filing | n8n | Technical | [n8n community template](https://n8n.io/workflows/11058-extract-and-process-invoices-with-gpt-4-google-drive-and-google-sheets/) | [page](https://bulletinai.app/u/45-invoice-pdfs-to-booking-list-with-auto-filing) |
| Chat-upload invoices with Gemini, duplicate checks and email alerts | n8n, Gemini | Low-code | [n8n community template](https://n8n.io/workflows/8548-extract-and-process-invoices-with-gemini-ai-google-sheets-and-gmail-notifications/) | [page](https://bulletinai.app/u/46-chat-upload-invoices-with-gemini-duplicate-checks-) |
| Resume screening and top-candidate alerts | Lindy | Low-code | [Lindy docs](https://docs.lindy.ai/use-cases/hr/resume-screening) | [page](https://bulletinai.app/u/50-resume-screening-and-top-candidate-alerts) |
| Stakeholder project update draft | ChatGPT | No-code | [OpenAI Academy — ChatGPT for any role](https://academy.openai.com/public/clubs/work-users-ynjqu/resources/chatgpt-for-any-role) | [page](https://bulletinai.app/u/61-stakeholder-project-update-draft) |
| Build customer personas from research | Claude | No-code | [Claude — Use cases gallery](https://claude.com/resources/use-cases) | [page](https://bulletinai.app/u/62-build-customer-personas-from-research) |
| Sentiment analyzer Gem for customer feedback | Gemini | No-code | [Google Workspace Updates](https://workspaceupdates.googleblog.com/2024/12/more-premade-gems-for-the-gemini-app.html) | [page](https://bulletinai.app/u/64-sentiment-analyzer-gem-for-customer-feedback) |

## Credits

Every use case links to and credits its original source. Vendor documentation, community templates, and third-party lists remain the work of their authors. This repository shares BulletinAI’s compilation, taxonomy, and playbook summaries. It does not relicense those sources. Details are in [LICENSE](LICENSE).

## Contributing

Corrections and new playbooks are welcome as pull requests and issues. Open an issue to propose a use case, or open a pull request that adds one object to [`data/usecases.json`](data/usecases.json). If you introduce a new outcome, platform, role, or difficulty, update [`data/categories.md`](data/categories.md) in the same change.

Leave affiliate program URLs, referral codes, and affiliate IDs out of entries and source links.

The field list, allowed values, and review checklist are in [CONTRIBUTING.md](CONTRIBUTING.md).

### Entry template

Copy this object, replace the placeholder values, and append it to the array in `data/usecases.json`. Leave `bulletin_url` empty until the entry has a page on bulletinai.app.

```json
{
  "id": "66-short-kebab-case-slug",
  "title": "Short descriptive title",
  "outcome": "Inbox & email",
  "platforms": ["ChatGPT"],
  "role": "Ops/manager",
  "difficulty": "No-code",
  "setup_time_estimate": "~10m (estimate)",
  "tools": ["ChatGPT"],
  "playbook": [
    "First concrete step.",
    "Second concrete step.",
    "What the person receives or checks."
  ],
  "source_url": "https://example.com/original-source",
  "source_credit": "Publisher — page or list name",
  "status": "community",
  "notes": "",
  "bulletin_url": ""
}
```

## License

The dataset in this repository is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Original sources retain their own rights. See [LICENSE](LICENSE).
