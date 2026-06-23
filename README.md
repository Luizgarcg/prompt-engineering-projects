# 📱 Achados & Perdidos

> A mobile app that connects people who lost belongings with those who found them — built as a prompt engineering academic project.

---

## 📋 About the Project

**Achados & Perdidos** is a lost-and-found mobile application designed to solve the lack of a centralized, secure platform for recovering items in urban public spaces.

The project was developed for the **Prompt Engineering and AI Applications** course (1st semester — ADS/UNIPE), demonstrating how generative AI tools can support the full software development lifecycle — from UX wireframes to UML diagrams and technical documentation.

**Team:**
- Luis Eduardo
- Ana Manuela Ferreira
- Jéssica Maria Cordeiro Oliveira
- Jaciel de Paula Trajano

---

## 🚀 Live Prototype

🔗 **[Access the interactive prototype here](https://dwarf-crayon-48097759.figma.site/)**

Built with Figma Maker — navigate through all 15 screens of the app.

---

## 📁 Repository Files

| File | Description |
|---|---|
| `Relatorio_Tecnico_v6_final.pdf` | Full technical specification report — business rules, architecture, modules, and UML diagrams |
| `WIREFRAME_BAIXA_QUALIDADE.pdf` | Low-fidelity wireframes for all 15 screens, generated with Claude (Anthropic) |
| `IMG_7218.pdf` | UML sequence diagrams covering the 5 main system flows |

---

## 🖥️ App Screens (15 total)

| # | Screen | Main Feature |
|---|---|---|
| 1 | Login | Email/password auth + OAuth2 (Google, Facebook, iCloud) |
| 2 | Register | New user sign-up with email validation |
| 3 | Home | Feed of recent items with category filters |
| 4 | Messages | Conversation list with unread count |
| 5 | Chat | Item-linked messaging between users |
| 6 | Notifications | Alerts and system updates |
| 7 | Add Item | Publish lost or found item |
| 8 | Advanced Search | Combined filters + AI image search |
| 9 | Profile | User stats and settings |
| 10 | Support | FAQ and contact |
| 11 | Item Details | Full info + ownership claim button |
| 12 | History | Item list filtered by status |
| 13 | Settings | Notifications, appearance, security |
| 14 | Map | Geolocated view of nearby items |
| 15 | Ownership Validation | 3-step flow to confirm item ownership |

---

## 🤖 AI Tools Used

| Tool | Role in the Project |
|---|---|
| **Claude (Anthropic)** | Generated low-fidelity wireframes via descriptive prompts |
| **ChatGPT (OpenAI)** | Modeled UML sequence diagrams for the 5 main flows |
| **Gemini (Google)** | Validated requirements and supported technical writing |
| **Mermaid Live Editor** | Rendered and validated UML diagrams visually |

---

## 🏗️ Architecture Overview

- **Database:** PostgreSQL with SQLAlchemy ORM (Python)
- **Reason:** Strong relational dependencies (User → Items → Messages) require ACID-compliant transactions
- **Key relationships:** User has many Items (1:N) — Message belongs to a Chat linked to an Item (N:1)

**System Services:**
Authentication · Items · Search · Chat · Notifications · Profile · Storage · AI · Database

---

## 📌 Prompt Engineering Techniques Applied

| Prompt | Technique |
|---|---|
| Wireframe generation | Role-Prompting + Specification Prompting |
| UML sequence diagrams | Chain-of-Thought (CoT) |
| Geolocation concept study | Conceptual Prompting (Zero-shot) |
| Ownership validation logic | CoT + Specification Prompting |
| REST API endpoint mapping | Role-Prompting + Few-shot Prompting |

---

## 📚 Course

**Prompt Engineering and AI Applications** — 1st Semester  
ADS (Systems Analysis and Development) — UNIPE
