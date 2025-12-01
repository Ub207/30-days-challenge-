# Task 6: GitHub MCP Server Setup

**Goal:** Connect Gemini to your GitHub account using the Model Context Protocol (MCP).

## Requirements

1.  **Step 1: Get Your GitHub Personal Access Token (PAT)**
    *   Go to GitHub Settings -> Developer Settings -> Personal Access Tokens -> Tokens (classic).
    *   Generate a new token with **`repo`** scope (Full control of private repositories).
    *   Copy the token.

2.  **Step 2: Store Your Token Securely**
    *   Create a `.env` file in your project root (or user home directory, depending on setup).
    *   Add `GITHUB_PERSONAL_ACCESS_TOKEN=your_token_here`.

3.  **Step 3: Configure Gemini to Use GitHub MCP Server**
    *   Open or create `settings.json` (usually in `~/.gemini/` or `%USERPROFILE%\.gemini\`).
    *   Add the GitHub MCP server configuration.

4.  **Step 4: Verify Connection**
    *   Restart Gemini CLI.
    *   Run `/mcp list` to see if `github` is listed.

5.  **Step 5: Test the Server**
    *   Ask Gemini: "List my GitHub repositories".
    *   Verify it returns your repos.

## Submission
*   [ ] Screenshot of `.env` file (token blurred).
*   [ ] Screenshot of `settings.json`.
*   [ ] Screenshot of `/mcp list` result.
*   [ ] Screenshot of GitHub repo list output.
