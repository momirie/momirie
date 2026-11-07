<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <img alt="Mohamed Mirie. Computer Science, London. I build developer tools that prove code works." src="assets/banner-light.svg" width="100%">
</picture>

<p align="center">
  <a href="https://www.linkedin.com/in/mohamedmirie/"><img alt="LinkedIn: mohamedmirie" src="https://img.shields.io/badge/LinkedIn-mohamedmirie-161616?style=flat-square&logo=linkedin&logoColor=white"></a>
  <a href="mailto:mohamedmirie@gmail.com"><img alt="Email: mohamedmirie@gmail.com" src="https://img.shields.io/badge/Email-mohamedmirie%40gmail.com-161616?style=flat-square&logo=gmail&logoColor=white"></a>
  <img alt="Based in London" src="https://img.shields.io/badge/Based_in-London-161616?style=flat-square">
</p>

I'm a Computer Science student in London. I like the part of software most people skip: tests, tooling,
and the question **"how do we actually know this works?"** With AI writing more and more code, I build the
checks that keep it honest.

<br>

### Currently building

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/tracefix-logo-reversed.svg">
  <img alt="Tracefix" src="assets/tracefix-logo.svg" height="44">
</picture>

An independent **fix verifier** for Python. Give it a bug fix, written by a coding agent or a person, and it
produces a **Fix Receipt**: executed evidence that the bug existed, that the fix removes it and that the tests
guard it. Then it attacks the fix with generated inputs (**Break My Fix**) and reports the input that breaks it,
or exactly how many it tried.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/receipt-dark.svg">
  <img alt="A recorded Tracefix run on a partial fix: nine stages, then a COUNTEREXAMPLE: parse_port(raw='') raises ValueError, found among 420 generated inputs." src="assets/receipt-light.svg" width="100%">
</picture>

- **AI proposes, code decides.** Models write tests and propose attacks. Every verdict comes from an exit code,
  a diff or a counter, never from a model's opinion.
- **Untrusted code, contained.** Generated tests run in throwaway copies, sandboxed with bubblewrap on Linux,
  with whole-process-tree kills and tamper detection around every run.
- **Attacks, not just checks.** Property-based inputs with Hypothesis, mutation testing to prove the tests guard
  the fix, and a before/after behaviour diff on the same inputs.
- **Fits the workflow.** A CLI and a GitHub Action that posts a Check Run and a PR comment with the receipt.
- **Measured, not claimed.** Benchmarked on 200+ runs against real-world bug fixes, including patches written by
  AI coding agents, with release gates it must pass before launch.
- **Built carefully.** 22k lines of typed Python (`mypy --strict`), 1,600+ tests, CI on Linux and Windows.

<sub>Pre-alpha. The repository opens once Tracefix passes its own release gates.</sub>

<br>

### Toolbox

<p>
  <img alt="Python" src="https://img.shields.io/badge/Python-161616?style=flat-square&logo=python&logoColor=white">
  <img alt="Java" src="https://img.shields.io/badge/Java-161616?style=flat-square&logo=openjdk&logoColor=white">
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-161616?style=flat-square&logo=typescript&logoColor=white">
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-161616?style=flat-square&logo=javascript&logoColor=white">
  <img alt="pytest" src="https://img.shields.io/badge/pytest-161616?style=flat-square&logo=pytest&logoColor=white">
  <img alt="Hypothesis" src="https://img.shields.io/badge/Hypothesis-161616?style=flat-square">
  <img alt="Git" src="https://img.shields.io/badge/Git-161616?style=flat-square&logo=git&logoColor=white">
  <img alt="GitHub Actions" src="https://img.shields.io/badge/GitHub_Actions-161616?style=flat-square&logo=githubactions&logoColor=white">
  <img alt="Docker" src="https://img.shields.io/badge/Docker-161616?style=flat-square&logo=docker&logoColor=white">
  <img alt="Linux" src="https://img.shields.io/badge/Linux-161616?style=flat-square&logo=linux&logoColor=white">
</p>

<br>

<p align="center"><sub><code>$ tracefix verify --repo github.com/momirie</code> &nbsp;→&nbsp; receipt written · exit 0</sub></p>
