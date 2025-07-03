# Incident Dataset for Frontend Integration

This repository contains a structured JSON dataset representing a full incident lifecycle, including metadata, technical details, war room logs, and resolution notes. The data is intended to simulate a real-world SRE incident postmortem and is formatted for consumption via frontend tools, mock UIs, or internal engineering dashboards.

---

## Contents

- `incident_INC9269346.json` — A detailed JSON file capturing the timeline, actions, impact analysis, involved teams, and post-resolution notes from a major incident (`INC9269346`).
- Contains technical bridge notes, Slack/Teams logs, error signatures, escalation history, timestamps, and ownership mapping.
- Ideal for building or testing:
  - UI components (incident viewers, timelines)
  - Internal engineering tools
  - Incident response simulators

---

## Purpose

This dataset is useful for:

- Prototyping incident response UIs or postmortem visualizations.
- Creating mock dashboards for SRE tooling or DevOps portals.
- Testing state handling in frontend applications using real-time operational data.

---

## How to Use

You can fetch the JSON file in your frontend application using `fetch` or `axios`:

### Example with `fetch()`:

```js
fetch("https://raw.githubusercontent.com/<your-username>/<repo-name>/main/incident_INC9269346.json")
  .then(res => res.json())
  .then(data => {
    console.log("Incident Data:", data);
  });
```

### Example with `axios`:
```
import axios from "axios";

axios.get("https://raw.githubusercontent.com/<your-username>/<repo-name>/main/incident_INC9269346.json")
  .then(response => {
    console.log("Incident Data:", response.data);
  });
```
