# my-mcp-server

MCP server template I base new tools on

Small but I use it weekly.

## Installation

```bash
pip install -r requirements.txt
```

## Highlights

- Three tools: add / get / list notes
- Includes Claude Desktop config snippet
- FastMCP style: decorators, zero boilerplate
- State persisted to a JSON file in the home dir

## Examples

```bash
# claude_desktop_config.json
# {
#   "mcpServers": {
#     "notes-box": {"command": "python", "args": ["server.py"]}
#   }
# }
python server.py
```

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   ├── dependabot.yml
│   └── pull_request_template.md
├── docs/
│   ├── faq.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .editorconfig
├── .gitignore
├── CONTRIBUTING.md
├── LICENSE
├── Makefile
├── SECURITY.md
├── requirements.txt
└── server.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## Development

```bash
# run the test suite
pytest -q   # or npm test / go test ./...
```

## License

MIT licensed, see LICENSE.
