<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <img alt="Mohamed Mire. Computer Science at Brunel, software engineering placement at Accenture. I build tools that try to break code before users do." src="assets/banner-light.svg" width="100%">
</picture>

<p align="center">
  <b>BSc Computer Science, Brunel University London</b> · graduating 2028<br>
  Software engineer on a year-long placement at <b>Accenture</b>, London<br>
  <b>Looking for graduate software engineering roles from 2028</b>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/mohamedmirie/"><img alt="LinkedIn: mohamedmirie" src="https://img.shields.io/badge/LinkedIn-mohamedmirie-161616?style=flat-square&logo=linkedin&logoColor=white"></a>
  <a href="mailto:mohamedmirie@gmail.com"><img alt="Email: mohamedmirie@gmail.com" src="https://img.shields.io/badge/Email-mohamedmirie%40gmail.com-161616?style=flat-square&logo=gmail&logoColor=white"></a>
</p>

I like the part of software most people skip: tests, tooling, and the question **"how do we actually know this
works?"** With AI writing more and more code, I build the checks that keep it honest.

<br>

### Currently building

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/tracefix-logo-reversed.svg">
  <img alt="Tracefix" src="assets/tracefix-logo.svg" height="44">
</picture>

**Tracefix checks whether a bug fix really fixes the bug, then tries to break it.**

Give it a fix, written by a coding agent or a person, and it produces a **Fix Receipt**: evidence from real test
runs that the bug existed, that the fix removes it and that the tests guard it. Then **Break My Fix** throws
generated inputs at the fixed code and reports the one that still breaks it, or exactly how many it tried.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/receipt-dark.svg">
  <img alt="A recorded Tracefix run on a partial fix: nine stages, then a COUNTEREXAMPLE: parse_port(raw='') raises ValueError, found among 420 generated inputs." src="assets/receipt-light.svg" width="100%">
</picture>

- **AI proposes, code decides.** Models write tests and suggest attacks. Every pass or fail comes from code that
  actually ran, never from a model's opinion.
- **Attacks, not just checks.** Hundreds of generated inputs hunt for one that still breaks the fix
  (property-based testing with Hypothesis), and mutation testing checks that the tests really guard it.
- **Works where developers work.** A command-line tool, plus a GitHub Action that posts the receipt on the pull
  request.

<details>
<summary><b>Technical details</b></summary>
<br>

- **Untrusted code, contained.** Generated tests run in throwaway copies, sandboxed with bubblewrap on Linux, with
  whole-process-tree kills and tamper detection around every run.
- **Before and after.** The same generated inputs run on the old and the fixed code; every change in behaviour is
  listed and labelled as intended or not.
- **Benchmarked on real fixes.** 200+ runs against real-world bug fixes, including patches written by AI coding
  agents. The release gates are still open, which is why it isn't public yet.
- **Engineering.** Python with `mypy --strict`, 1,600+ tests, CI on Linux and Windows.

</details>

<sub>In active development. Private until it passes its own release gates.</sub>

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
