<h1 align="center">Osama Quttenh</h1>

<p align="center">
  <b>Backend Software Engineer</b> · Python · FastAPI · SQLAlchemy · PostgreSQL
  <br>
  <sub>Jerusalem, Palestine · B.Sc. Computer Science, Birzeit University (2026)</sub>
</p>

<p align="center">
  <a href="https://osamazuhdi.com"><img alt="Website" src="https://img.shields.io/badge/osamazuhdi.com-111827?style=flat-square&logo=googlechrome&logoColor=white"></a>
  <a href="https://linkedin.com/in/osama-zuhdi"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white"></a>
  <a href="mailto:osamaps5181346@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-111827?style=flat-square&logo=gmail&logoColor=white"></a>
  <a href="https://osamazuhdi.com/osama-quttenh-cv.pdf"><img alt="CV" src="https://img.shields.io/badge/CV-PDF-111827?style=flat-square&logo=readthedocs&logoColor=white"></a>
</p>

---

I build backend systems in Python: APIs, data models, and the tests and pipelines that keep them working. I contribute to **[Advanced Alchemy](https://github.com/litestar-org/advanced-alchemy)**, the SQLAlchemy toolkit for Litestar and FastAPI, and most of what I build for myself is Arabic-first, which keeps leading me into search problems.

**Open to backend engineering roles.**

## Open source

**[Advanced Alchemy](https://github.com/litestar-org/advanced-alchemy)** · 5 merged pull requests

| PR | What changed |
| --- | --- |
| [#856](https://github.com/litestar-org/advanced-alchemy/pull/856) | **OpenTelemetry support.** Found why OpenTelemetry's SQLAlchemy instrumentation silently missed the library's engines (engine factories were bound at import time, before the instrumentor patched them). Resolved them at call time across sync, async and read-replica configs, and wrote the integration docs. |
| [#839](https://github.com/litestar-org/advanced-alchemy/pull/839), [#840](https://github.com/litestar-org/advanced-alchemy/pull/840) | **Specific errors on Oracle and SQL Server.** Constraint violations now raise `DuplicateKeyError` and `ForeignKeyError` instead of a generic `IntegrityError`, tested against real Oracle 23ai and SQL Server 2022. |
| [#869](https://github.com/litestar-org/advanced-alchemy/pull/869) | **Litestar query services.** Fixed service providers that failed every request for query and async read services, with typed overloads. |
| [#865](https://github.com/litestar-org/advanced-alchemy/pull/865) | **Cache protocols.** Exported the cache-region protocols on the public API. |

## Projects

### [Souq Al-Balad](https://github.com/osamaps518/souq_al_balad) · سوق البلد

A peer-to-peer marketplace for the local Palestinian community. My graduation project. The interface is Arabic, right-to-left and mobile-first.

- A FastAPI modular monolith with modules for listings, messaging, sale coordination, reputation and admin moderation, plus the full React/TypeScript frontend.
- Hybrid keyword and semantic search for Arabic listings (Meilisearch with Gemini embeddings), and real-time messaging and notifications over Socket.IO.
- An AI listing assistant that suggests a category, drafts an Arabic description and flags prohibited items from product photos.
- Deployed as Docker containers on Azure App Service, with Supabase for auth, storage and PostgreSQL. GitHub Actions runs 1,000+ tests (Pytest, Vitest, Playwright) and Alembic drift checks, then deploys to staging.

<sub>FastAPI · SQLAlchemy · PostgreSQL · React · TypeScript · Meilisearch · Socket.IO · Docker · Azure · Supabase</sub>

### [Mutabiq](https://github.com/osamaps518/Mutabiq) · مطابق <sub>`in progress`</sub>

A library that makes Arabic search work in your own PostgreSQL database. The same Arabic word gets written many ways (أرز, إرز, آرز, ارز), so Mutabiq turns them into one form, with the rules implemented in both Python and SQL and tested to give the same output. It adds alias packs for words that differ by region (بندورة and طماطم), a `doctor` command that checks a database, and a `bench` command that measures search quality on labelled queries.

<sub>Python · PostgreSQL · uv · Pytest</sub>

### [GHBot](https://github.com/osamaps518/GHBot) <sub>`in progress`</sub>

An Arabic-first training and nutrition app for people who train: food logging with daily totals, synced to the server. A FastAPI backend split into modules with a Flutter Android app that mirrors them. It will be Mutabiq's first user, for Arabic food search.

<sub>FastAPI · SQLAlchemy · PostgreSQL · Flutter · Dart</sub>

## Tech

<p>
  <img alt="Python, FastAPI, Django, PostgreSQL, TypeScript, React, Docker, Azure, GitHub Actions, Linux, Bash, Git" src="https://skillicons.dev/icons?i=py,fastapi,django,postgres,ts,react,docker,azure,githubactions,linux,bash,git&perline=12">
</p>

Also: SQLAlchemy · Alembic · Django REST Framework · Pytest · Vitest · Playwright · Java · SQL

</details>
