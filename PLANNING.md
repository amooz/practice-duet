# Practice Duet Planning

This document tracks discovery questions and answers for the Practice Duet platform.

**How to use this file**
- Each question has an **Answer** section.
- If unanswered, keep `TBD`.
- When answered, replace `TBD` with the agreed decision (and optionally date/notes).
- After each answer, update `README.md` to reflect the latest understanding.


## Decision Update Template

When recording an answer, use this compact format:

- **Answer:** <decision>
- **Date:** YYYY-MM-DD
- **Notes (optional):** <tradeoffs/context>

---

## 1) Product scope & users

### 1. Who are the primary users at launch?
- Individual candidates practicing solo
- Interviewers running live sessions
- Companies/admins managing question banks
**Answer:** TBD

### 2. Is v1 focused on practice mode only, or also live interviewer-candidate sessions?
**Answer:** TBD

### 3. Do you want account tiers (free/pro), or is monetization out of scope for now?
**Answer:** TBD

### 4. Should candidates have a persistent profile/history across attempts?
**Answer:** TBD

---

## 2) “Universal language” definition

### 5. Which languages must be supported in v1? (e.g., Python, JS/TS, Java, C++, Go, Rust, Ruby, C#)
**Answer:** TBD

### 6. Do you need language-specific runtime execution (run/tests), or editor-only coding + AI review of code text?
**Answer:** TBD

### 7. If execution is needed: should each language run in isolated per-attempt containers?
**Answer:** TBD

### 8. Any languages you explicitly do not want to support due to security/runtime complexity?
**Answer:** TBD

---

## 3) Interview question model

### 9. Should questions include: prompt only; prompt + starter code; prompt + hidden/public tests; expected complexity constraints?
**Answer:** TBD

### 10. Do you want difficulty levels + topics/tags (arrays, graphs, DP, system design)?
**Answer:** TBD

### 11. Will you provide your own question bank, or should we seed from a curated open set?
**Answer:** TBD

### 12. Should candidates be timed with visible countdown?
**Answer:** TBD

### 13. Do you want “follow-up” questions (like real interviews) generated dynamically by AI?
**Answer:** TBD

---

## 4) AI evaluation behavior

### 14. What should AI feedback include? correctness, code quality/readability, algorithmic complexity, edge cases missed, suggested improvements
**Answer:** TBD

### 15. Should AI give a numeric score/rubric or qualitative feedback only?
**Answer:** TBD

### 16. Should AI evaluation compare against hidden tests when available?
**Answer:** TBD

### 17. Which LLM provider(s) do you prefer (OpenAI, Anthropic, Azure OpenAI, local)?
**Answer:** TBD

### 18. Do you want configurable model/provider by environment?
**Answer:** TBD

### 19. Should feedback be immediate after submit, or also stream in real-time while coding?
**Answer:** TBD

### 20. Do you want anti-cheating detection (copy/paste patterns, suspicious latency, AI-generated style)?
**Answer:** TBD

---

## 5) Collaboration / pair-programming experience

### 21. Is “pair programming” in v1 simulated (AI interviewer only), or true real-time shared editor between two humans?
**Answer:** TBD

### 22. If real-time collaboration is needed, do you want shared cursor presence, voice/video integration, chat, interviewer controls (read-only/take-over)?
**Answer:** TBD

### 23. Should sessions be recordable/replayable?
**Answer:** TBD

---

## 6) VS Code-based editor specifics

### 24. By “based on VS Code,” do you mean Monaco editor in browser, or full code-server / VS Code Web embedding?
**Answer:** TBD

### 25. Do you need support for VS Code extensions in-browser?
**Answer:** TBD

### 26. Should users be able to open multi-file projects, or single-file challenge workspace?
**Answer:** TBD

### 27. Need terminal access in-browser for candidates?
**Answer:** TBD

### 28. Need linting/formatting/autocomplete per language in v1, or keep minimal first?
**Answer:** TBD

---

## 7) Rails + realtime framework clarification

### 29. You mentioned Ruby on Rails with Livewire. Did you mean Hotwire (Turbo + Stimulus) for Rails, or a different Rails realtime approach (ActionCable + StimulusReflex/AnyCable)?
**Answer:** TBD

### 30. Are you committed to Rails 8 (if stable for your timeline) or Rails 7.x?
**Answer:** TBD

### 31. DB preference: PostgreSQL?
**Answer:** TBD

### 32. Background jobs preference: Sidekiq + Redis?
**Answer:** TBD

---

## 8) Dockerization & environments

### 33. For development, do you want one-command startup via `docker compose up` with web, worker, db, redis, and language runner service(s)?
**Answer:** TBD

### 34. For production runtime, target platform: Kubernetes, ECS/Fargate, Render/Fly/Heroku-style, or self-hosted Docker?
**Answer:** TBD

### 35. Do you need separate container image builds per service?
**Answer:** TBD

### 36. Any CI/CD preference (GitHub Actions, GitLab CI, etc.)?
**Answer:** TBD

### 37. Should we include infra-as-code in repo (Terraform/Helm) now or later?
**Answer:** TBD

---

## 9) Security, sandboxing, and compliance

### 38. Executing untrusted code requires sandboxing: are isolated ephemeral containers with strict CPU/memory/time/network limits acceptable?
**Answer:** TBD

### 39. Should user code execution have no outbound internet by default?
**Answer:** TBD

### 40. Any compliance/security requirements (SOC2, GDPR, data retention rules)?
**Answer:** TBD

### 41. Should we store candidate code attempts indefinitely or time-limited?
**Answer:** TBD

### 42. Need audit logs for interviewer/admin actions?
**Answer:** TBD

---

## 10) UX details

### 43. What is the ideal candidate flow?
- pick language → read prompt → code → run tests → submit → get AI feedback
**Answer:** TBD

### 44. Should candidates be allowed multiple submissions per question?
**Answer:** TBD

### 45. Do you want hint system (manual hints or AI-generated hints)?
**Answer:** TBD

### 46. Should there be “official solution” reveal, and under what conditions?
**Answer:** TBD

### 47. Should feedback be downloadable/shareable (PDF/report link)?
**Answer:** TBD

---

## 11) Admin/authoring tools

### 48. Do you need an internal admin UI to create/edit questions, test cases, and evaluation rubrics?
**Answer:** TBD

### 49. Should admins define language-specific starter templates and test harnesses?
**Answer:** TBD

### 50. Need A/B control over prompts/LLM settings per question?
**Answer:** TBD

---

## 12) Metrics & success criteria

### 51. What are launch KPIs? (e.g., D1 retention, completion rate, average score improvement, paid conversion)
**Answer:** TBD

### 52. Any performance targets? (e.g., editor load time, feedback latency, concurrent session target)
**Answer:** TBD

---

## 13) Timeline & delivery expectations

### 53. Are you expecting architecture + technical plan only, clickable prototype, or production-ready MVP?
**Answer:** TBD

### 54. What’s the timeline for v1?
**Answer:** TBD

### 55. Team composition (number of engineers/designers/devops) so scope can be sized realistically?
**Answer:** TBD

---

## Change Log

- Initial planning questionnaire and answer slots created.
