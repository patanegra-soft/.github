## PATANEGRA Soft

Open-source modules for Odoo Community 14.0 to 20.0. Apache 2.0. Site: [patanegra.com](https://www.patanegra.com/).

### AI inside Odoo Community

| Module | For whom |
| :--- | :--- |
| [**Chatboo**](https://github.com/patanegra-soft/pns_ai_chatboo) | Everyone. The AI chat inside Odoo: ask about your records, draw tables and charts, drop a vendor's bill and get a draft to confirm. **Start here**: installing it brings the engine. |
| [**PNS AI Engine**](https://github.com/patanegra-soft/pns_ai_mcp) | IT. Providers, agents, skills and the MCP server. Alone it serves Cursor, Claude or any MCP client. |

Install from git. Each Odoo series is a branch (`14.0`, `15.0`, `16.0`, `17.0`, `18.0`, `19.0`, `20.0`):

```bash
mkdir -p ~/odoo/pns && cd ~/odoo/pns
for r in pns_base pns_ai_mcp pns_ai_chatboo; do
  git clone -b 20.0 --depth 1 https://github.com/patanegra-soft/$r
done
```

Add each clone to `addons_path`, update the Apps list and install **Chatboo**. Details in its [Getting started](https://github.com/patanegra-soft/pns_ai_chatboo#getting-started).

### Tools

| Module | What it does |
| :--- | :--- |
| [**PNS Ribbon**](https://github.com/patanegra-soft/pns_ribbon) | Corner banner so a test database is not mistaken for production. |
| [**PNS Base**](https://github.com/patanegra-soft/pns_base) | Shared layer of the PNS modules. You install it as a dependency. |
