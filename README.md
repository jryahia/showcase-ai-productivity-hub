# AI Productivity Hub

**Pulls notes, meetings and tasks from Apple Notes, Notion, Airtable, Gmail, Calendly and Fireflies.ai into one dashboard with automation rules.**

> **This is a proprietary project. Source code is private. This page showcases the system's architecture and results.**

**Case study page:** [https://jryahia.github.io/showcase-ai-productivity-hub/](https://jryahia.github.io/showcase-ai-productivity-hub/)

![AI Productivity Hub](assets/00-dashboard.png)

## Problem it solves

Notes, meetings and tasks live in six different tools. This hub syncs them into one place, turns meeting action items into tasks automatically, and tags content, with or without an AI key.

## Architecture

![Architecture](assets/architecture.svg)

1. Scheduled syncs fetch, normalize and upsert items from each platform.
2. Automation rules react to triggers such as completed meetings or keywords.
3. Items are tagged and summarized, with local fallbacks when no AI key is set.
4. Everything shows on one dashboard with sync health.

## Key features

- Six platform connectors
- Rule engine with five triggers and four actions
- Credentials encrypted at rest
- Degrades gracefully without an AI key
- Kanban and table task views
- Full config backup and restore

## Tech stack

![Python](https://img.shields.io/badge/Python-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![FastAPI](https://img.shields.io/badge/FastAPI-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![SQLModel](https://img.shields.io/badge/SQLModel-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![APScheduler](https://img.shields.io/badge/APScheduler-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![Fernet encryption](https://img.shields.io/badge/Fernet%20encryption-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![Jinja2](https://img.shields.io/badge/Jinja2-161b22?style=for-the-badge&labelColor=161b22&color=161b22)

## What it does in practice

- Meeting action items become tracked tasks without copy-pasting.

## Screenshots

**Cross-platform dashboard after sync**

![Cross-platform dashboard after sync](assets/00-dashboard.png)

---

Built by [Yahya Jarray](https://github.com/jryahia). Interested in a similar system? [Get in touch](mailto:yahiajarray43@gmail.com).
