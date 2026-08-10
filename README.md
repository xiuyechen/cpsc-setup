# cpsc-setup

Workshop setup pages for using Claude Code on the course LLM gateway.

- **`index.html`** — student-facing walkthrough.
  Published at https://xiuyechen.github.io/cpsc-setup/
- **`agent-setup.txt`** — instructions Claude Code fetches and follows to do the
  setup. Students paste one line pointing at this file plus their own API key.
  Served at https://xiuyechen.github.io/cpsc-setup/agent-setup.txt

No API keys are stored in this repo. Each student supplies their own at setup time.

Note for maintainers: the Portkey config referenced in `agent-setup.txt` must not
contain a `"cache": {"mode": "simple"}` block — it disables Anthropic prompt
caching and multiplies per-turn cost.
