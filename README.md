# HR Chatbot - G2 (Howest HR)

Quick answers, better support. More time for people.

## About the project

A student team project for Howest HR. We plan to build a chatbot that answers common HR questions in plain language using Howest's own documents and always shows its sources. The chatbot supports personal HR services: sensitive or personal questions are referred to HR.

**Status:** introduction and planning phase. The repository currently contains the README and `.gitignore`; the application is not implemented yet. Technology choices and installation instructions will be added once the prototype is built.

## Team

- Max Drahomaretskyi
- Maksym Maliavko
- Viktor Sokorenko

## Client

Howest HR department, Howest University of Applied Sciences.

## Planned functionality

- Answer frequently asked HR questions in Dutch and English.
- Retrieve information from approved internal HR documents, including cross-language searches.
- Show the source document and relevant page or passage for each supported answer.
- Say when there is insufficient information and refer the employee to HR.
- Refer personal or sensitive questions, such as illness, conflicts or individual pay situations, to HR.
- Clearly tell users they are interacting with an AI.

## Planned approach

We will explore Retrieval-Augmented Generation (RAG):

1. Extract text from approved documents and use OCR where required.
2. Identify current document versions and retain source metadata.
3. Split text into passages and retrieve relevant information for a question.
4. Generate an answer based only on retrieved evidence, with source references.
5. Use an HR referral when the question cannot be answered safely.

We will create a Dutch/English question set together with HR and compare at least two approaches. Evaluation will cover answer correctness, source support, cross-language retrieval, fallback behavior and response time. Model hosting, chunking and retrieval choices are still to be decided and evaluated.

## Privacy and data

The source material consists of approximately 90 internal HR documents in Dutch and English. Some documents require OCR or exist in multiple versions.

- Use internal documents only within the project; do not publish them in this repository.
- Do not store personal information from conversations.
- Keep credentials, API keys and local configuration out of Git.
- Use only approved services for internal source material.

## Planning

Project work runs from **4 to 27 January 2027**. The **final presentation is on 27 January 2027**.

Only **Sprint 1 (4-8 January)** is planned in detail at this stage. It covers scope agreement, document inventory, project setup, an initial bilingual evaluation set and a small end-to-end RAG baseline with citations and HR fallback. Its proposed workload is 30 story points, to be reviewed by the team. Future work stays in the product backlog until later sprint planning.

## Trello

[Open the HR Chatbot - G2 board](https://trello.com/b/b4mI8Gou/hr-chatbot-g2-howest-hr)

The board uses the required workflow:

**Backlog -> Backlog Sprint -> In Progress -> Testing -> Done**

Use **Blocking** for work that cannot proceed. Backlog contains prioritized future work; Backlog Sprint contains the stories selected for the current week. Each story has acceptance criteria, category labels and an estimated complexity: **1 = easy, 3 = medium, 5 = complex, 7 = very complex**. Sprint tasks have deadlines. The Scrum master facilitates story selection with the team.

## Planned deliverables

- Working HR chatbot prototype.
- Source code and reproducible setup instructions.
- Project documentation, including architecture and privacy decisions.
- Evaluation question set, comparison of at least two approaches and known limitations.
- Short demo video and final presentation.

## Running the project

There is no runnable application yet. Setup commands, dependencies and configuration instructions will be documented here when implementation starts.
