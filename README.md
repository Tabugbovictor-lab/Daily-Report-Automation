# Daily Automated Report Pipeline (n8n + Gemini AI + Google Docs + Gmail)

An automated cloud workflow built using **n8n** that retrieves daily raw notes from Google Docs, synthesizes them into a structured 300-word formal report using **Google Gemini AI**, and delivers the final report to Gmail every evening at 6:00 PM.

---

## 📌 Architecture & Process Flow

```mermaid
graph LR;
    A([Schedule Trigger]) --> B[Google Docs Node];
    B --> C[Gemini AI Node];
    C --> D([Gmail Node]);
