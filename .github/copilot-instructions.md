# Copilot Review Guidance

When reviewing changes in this repository, prioritize:

- Correctness and regressions over style nits.
- Security, input validation, and authorization checks.
- UI behavior in the static frontend and API behavior in the FastAPI backend.
- Data flow between the frontend, routers, and database layer.
- Missing or weak tests when behavior changes.

Keep review comments:

- Specific, actionable, and concise.
- Focused on the changed lines and nearby code paths.
- Backed by the observed behavior, expected contract, or test impact.

Project context:

- The backend lives under `src/backend/` and the API entrypoint is `src/app.py`.
- The frontend lives under `src/static/`.
- Favor small, local fixes that preserve the existing structure unless a broader change is clearly required.