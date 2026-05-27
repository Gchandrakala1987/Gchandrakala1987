<h1 align="center">Hi, I'm Chandrakala 👋</h1>

<p align="center">
  <em>Engineer focused on AI-assisted automation, browser testing, and the .NET / Azure stack.</em>
</p>

<p align="center">
  <a href="https://github.com/Gchandrakala1987?tab=repositories"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-Gchandrakala1987-181717?logo=github"></a>
  <a href="mailto:gchandrakala1987@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-gchandrakala1987%40gmail.com-D14836?logo=gmail&logoColor=white"></a>
</p>

---

## 🚀 Featured project

### [Synth](https://github.com/Gchandrakala1987/synth) — AI-generated synthetic browser tests, in plain English

Plain-English in, structured bug report out. The agent opens a real browser, drives an OpenAI tool-calling loop through `navigate / click / fill / read_page / assert`, and streams every step to the UI over SignalR.

```
"Test the checkout flow with a guest user."
         │
         ▼
React UI → ASP.NET Core API → Background worker → OpenAI tool loop
                                                      ├── Playwright (Chromium)
                                                      └── SignalR fan-out → live progress
                                  ↓
                            structured BugReport
```

**Why it matters:** collapses the "write a script for every flow" treadmill that makes UI testing expensive. One natural-language instruction, one disposable agent per request.

**Built with:** `C#` `.NET 10` `ASP.NET Core` `SignalR` `Playwright` `OpenAI` `Azure OpenAI` `React 18` `TypeScript` `Vite` `Bicep` `GitHub Actions` `Docker`

**Engineering highlights:**

- Tool-calling loop with hard step / time / concurrency ceilings — bounded by design.
- Accessibility-tree snapshots as the model's view of the page (~10× cheaper than DOM HTML, far more stable).
- Pluggable everywhere — `ITestRunStore`, `IAgentChatClientFactory`, `IBrowserToolbox`, `IProgressPublisher` are all interfaces.
- Full IaC: Bicep deploys App Service + Azure OpenAI + Log Analytics + App Insights + ACR.
- CI/CD with typecheck, lint, build, test, Docker cache; OIDC-based deploy to Azure (no long-lived secrets).

→ **[Read the architecture](https://github.com/Gchandrakala1987/synth/blob/main/docs/ARCHITECTURE.md)** · **[Read the agent design](https://github.com/Gchandrakala1987/synth/blob/main/docs/AGENT_DESIGN.md)**

---

## 🛠 Tech I work with

```
Languages   C# · TypeScript · Python · SQL
Backend     ASP.NET Core · SignalR · REST · gRPC · background workers
AI / LLM    OpenAI · Azure OpenAI · tool-calling · agentic loops · prompt design
Testing     Playwright · xUnit · Jest · agent-driven QA
Frontend    React · Vite · TypeScript
Cloud       Azure (App Service · Functions · OpenAI · App Insights · Service Bus · Cosmos)
DevOps      GitHub Actions · Docker · Bicep · OIDC federated identity
```

---

## 💼 What I'm looking for

Roles where I can pair **AI** with **automation** — QA automation engineering, applied-AI / agent engineering, test platform / developer-productivity teams. Open to remote and hybrid.

If you're hiring for any of the above, [let's talk](mailto:gchandrakala1987@gmail.com).

---

## 📈 Activity

<p align="center">
  <img alt="GitHub stats" src="https://github-readme-stats.vercel.app/api?username=Gchandrakala1987&show_icons=true&hide_border=true&theme=tokyonight">
  <img alt="Top languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Gchandrakala1987&layout=compact&hide_border=true&theme=tokyonight">
</p>
