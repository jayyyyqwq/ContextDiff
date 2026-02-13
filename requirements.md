# ContextDiff: System Requirements & Architecture

## 1. Tech Stack Overview
* **Backend:** Java 17+, Spring Boot 3.x (REST API, Core Graph Logic)
* **AI / Inference:** Amazon Bedrock (Claude 3.5 Sonnet / Haiku for fast text generation and logic extraction)
* **Frontend:** React.js / Next.js
* **Visualization:** Mermaid.js (Client-side rendering)

## 2. API & Integration Requirements
* **GitHub REST API v3:** Required for repository scanning and language depth analysis.
* **Amazon S3:** For temporarily hosting uploaded resume PDFs before parsing.
* **Amazon Bedrock API:** For the Knowledge Diff Engine and Analogy generation.

## 3. Environment Variables Needed
To run this project locally, you will need to configure the following in your `.env` or `application.properties`:
* `AWS_ACCESS_KEY_ID`
* `AWS_SECRET_ACCESS_KEY`
* `AWS_REGION` (e.g., us-east-1)
* `GITHUB_PERSONAL_ACCESS_TOKEN`

## 4. Run Instructions (Local Dev)
1. Clone the repository.
2. Ensure Java 17 and Maven are installed.
3. Run `mvn spring-boot:run` to start the backend engine.
4. Navigate to the `/client` directory and run `npm install` followed by `npm run dev`.
