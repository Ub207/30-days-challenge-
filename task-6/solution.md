# Task 6 Solution: GitHub MCP Server Setup

## 1. Configuration Files

### `.env` File
Create a file named `.env` in your configuration directory (e.g., `C:\Users\Hp\.gemini\.env` or project root).

```env
GITHUB_PERSONAL_ACCESS_TOKEN=ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

### `settings.json` Configuration
Add the following to your `settings.json` (e.g., `C:\Users\Hp\.gemini\settings.json`):

```json
{
  "mcpServers": {
    "github": {
      "command": "npx",
      "args": [
        "-y",
        "@modelcontextprotocol/server-github"
      ],
      "env": {
        "GITHUB_PERSONAL_ACCESS_TOKEN": "${GITHUB_PERSONAL_ACCESS_TOKEN}"
      }
    }
  }
}
```

## 2. Verification Steps

### Step 1: Check MCP Servers
Run the following command in Gemini:
```
/mcp list
```
**Expected Output:**
```
✅ github (Tools: 90+)
```

### Step 2: Test GitHub Connection
Ask Gemini:
```
List my GitHub repositories
```
**Expected Output:**
Gemini should list your repositories, for example:
*   `Ub207/30-days-challenge-`
*   `Ub207/hakathone-02`
*   ...

## 3. Submission Evidence

> **Note:** Please verify these steps on your local machine and take the required screenshots for submission.

*   [ ] **.env Screenshot:** (Place screenshot here)
*   [ ] **settings.json Screenshot:** (Place screenshot here)
*   [ ] **MCP List Screenshot:** (Place screenshot here)
*   [ ] **Repo List Screenshot:** (Place screenshot here)
