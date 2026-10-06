# SmartSpend AI

[![Status](https://img.shields.io/badge/status-live-success)](https://ai-shopping-assistant-7r1p.onrender.com)
[![.NET 8.0](https://img.shields.io/badge/.NET-8.0-512BD4?logo=dotnet)](https://dotnet.microsoft.com/)
[![C#](https://img.shields.io/badge/C%23-ASP.NET%20Core-239120?logo=csharp)](https://learn.microsoft.com/dotnet/csharp/)

> An AI-powered budgeting and shopping assistant designed to help students make smarter financial decisions.

## About the Project

Managing money as a student can be challenging. Between transport, groceries, subscriptions, and social spending, it can be difficult to track expenses, follow a budget, and distinguish genuine needs from impulse purchases.

**SmartSpend AI** helps students take control of their finances through AI-assisted budgeting, shopping insights, spending analysis, and practical financial learning resources. It combines budget management with intelligent shopping tools to make everyday financial decisions clearer and more intentional.

## Key Features

| Feature | Description |
| --- | --- |
| AI Chatbot | Ask budgeting, saving, and spending questions through an AI-powered financial assistant. |
| Need or Want? | Upload or capture an item image and receive AI-assisted classification to encourage mindful spending. |
| Price Comparison | Compare item prices across supported stores to find better-value options. |
| Budget Tracking | Create budgets, record expenses, and monitor spending by category. |
| Shopping List Management | Build and manage shopping lists while keeping planned purchases organised. |
| Distance-Based Shipping | Calculate delivery considerations based on distance and location data. |
| Financial Health Score | Receive a score based on budgeting habits, spending patterns, and savings progress. |
| Savings Goals | Set personal savings goals and track progress over time. |
| Budgeting Resources | Access educational content to improve financial literacy and budgeting skills. |
| Favorites | Save frequently used products, resources, or items for quick access. |

## Tech Stack

| Area | Technologies |
| --- | --- |
| Backend | ASP.NET Core 8.0, C#, Entity Framework Core, PostgreSQL |
| AI & Location Services | Google Gemini 2.0 Flash, Gemini Vision API, OpenCage Geocoder |
| Frontend | Razor Views, Tailwind CSS, JavaScript, Chart.js, Leaflet.js |
| DevOps & Hosting | Render.com, GitHub, Docker |

## Live Demo

Visit the live application here:

[**Open SmartSpend AI**] (https://ai-shopping-assistant-7r1p.onrender.com)

### Demo Credentials

> Replace these placeholders with safe demo-account credentials before publishing.

| Field | Value |
| --- | --- |
| Email | `demoUser1@gmail.com` |
| Password | `demoUser1` |

## Architecture

```text
┌─────────────────────────────────────────────────────────────┐
│                        Frontend                             │
│     Razor Views · Tailwind CSS · JavaScript · Chart.js      │
│                         Leaflet.js                          │
└──────────────────────────────┬──────────────────────────────┘
                               │
                               ▼
┌─────────────────────────────────────────────────────────────┐
│                       Controllers                           │
│     Authentication · Budget · Shopping · AI · Goals         │
└──────────────────────────────┬──────────────────────────────┘
                               │
                               ▼
┌─────────────────────────────────────────────────────────────┐
│                        Services                             │
│   Business Logic · AI Processing · Price Analysis · Scoring │
└──────────────────────────────┬──────────────────────────────┘
                               │
                               ▼
┌─────────────────────────────────────────────────────────────┐
│                       Data Layer                             │
│          Entity Framework Core · PostgreSQL Database         │
└──────────────────────────────┬──────────────────────────────┘
                               │
                               ▼
┌─────────────────────────────────────────────────────────────┐
│                    External APIs                              │
│  Gemini 3.1 Flash-Lite · Gemini Vision · OpenCage · Store Data│
└─────────────────────────────────────────────────────────────┘
Project Structure
The source repository is private. The following structure is provided as a high-level overview.

SmartSpendAI/
├── Controllers/          # Handles HTTP requests and application routes
├── Services/             # Business logic, AI integration, and calculations
├── Models/               # Domain models and view models
├── Data/                 # Database context, migrations, and repositories
├── Views/                # Razor views and shared UI components
├── wwwroot/              # Static assets: CSS, JavaScript, images
├── Middleware/           # Custom request pipeline middleware
├── Configuration/        # Application configuration and options
├── Dockerfile            # Containerisation configuration
└── Program.cs            # Application entry point and service registration

Security
SmartSpend AI applies security-focused practices throughout the application
**Password Security:**	User passwords are hashed using BCrypt before storage.
**API Key Protection:**	API keys and sensitive configuration are stored in environment variables and excluded from source control.
**SQL Injection Prevention:**	Entity Framework Core parameterised queries protect against SQL injection.
**Authentication:**	Authenticated access protects user-specific financial data and features.
HTTPS	The deployed application uses HTTPS to encrypt data in transit.

Source Code Availability
The SmartSpend AI source code is maintained in a private repository.
This public repository exists as a project showcase and documentation hub. Keeping the implementation private helps protect sensitive configuration and API credentials.
