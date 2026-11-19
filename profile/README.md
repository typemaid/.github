<p align="center">
  <img src="https://typemaid.pages.dev/docs/logo.svg" alt="typemaid" width="280">
</p>

<p align="center">
  <strong>The diagram is the program.</strong><br>
  Run Mermaid flowcharts as typed TypeScript workflows.
</p>

<p align="center">
  <a href="https://typemaid.pages.dev/docs/getting-started/">Quickstart</a> ·
  <a href="https://typemaid.pages.dev/docs/">Docs</a> ·
  <a href="https://github.com/typemaid/typemaid">Repository</a> ·
  <a href="https://www.npmjs.com/package/typemaid">npm</a>
</p>

---

typemaid is a TypeScript SDK. You draw a workflow as a Mermaid flowchart, and each box in the diagram is a step you write in TypeScript, with its input and output typed by Zod. The diagram decides what runs next.

- **Checked before it runs.** Mistakes in the diagram or the steps are reported with the file, line and a suggested fix.
- **People in the loop.** A run can pause for a person and resume later, even in another process.
- **Retries and saved runs.** Failed steps are retried, and runs can be saved to SQLite, Postgres or libSQL.
- **Any model.** Agent steps call models through the Vercel AI SDK.

```bash
npm install typemaid zod
```

| Package | What it is |
|---|---|
| [`typemaid`](https://www.npmjs.com/package/typemaid) | `run`, `resume`, `check`, plus `typemaid/ai` and `typemaid/sqlite` |
| [`@typemaid/postgres`](https://www.npmjs.com/package/@typemaid/postgres) | Keep runs in Postgres |
| [`@typemaid/libsql`](https://www.npmjs.com/package/@typemaid/libsql) | Keep runs in libSQL or Turso |
| [`@typemaid/view`](https://www.npmjs.com/package/@typemaid/view) | The local workflow viewer |

typemaid is source-available under FSL-1.1-MIT. Each release becomes MIT two years after it is published.
