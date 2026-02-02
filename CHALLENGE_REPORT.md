# TRP 1 - MCP Setup Challenge Report

## What I Did
- **Task 1: Setup** - Configured the Tenx MCP server in VS Code by adding the server details to `.vscode/mcp.json` with the required URL (`https://mcppulse.10academy.org/proxy`), type (`http`), and headers (X-Device: windows, X-Coding-Tool: vscode). Enabled the MCP Servers experimental feature in VS Code settings. Started the server via Copilot Chat → Agents → Tools, and authenticated with GitHub. The connection is active, logging interactions automatically.
- **Task 2: Research & Configure** - Researched Boris Cherny's workflow thread on X (Twitter) for Claude Code best practices. Incorporated community recommendations from GitHub docs, developer blogs, and forums. Updated `.github/copilot-instructions.md` with enhanced rules, adding sections for Dependencies & Libraries, Security & Performance, and more specific coding standards (e.g., Airbnb style, TypeScript strict mode). Tested AI behavior by prompting for code changes and observing more structured, secure outputs.
- **Task 3: Documentation** - Created this report documenting the process, successes, challenges, and insights. Ensured the repository is public and contains all artifacts (rules file, this report, README.md, etc.).

## What Worked
- MCP server setup was successful after enabling the experimental flag and authenticating. The server appears in Copilot Chat Tools, and interactions are logged.
- Rules file updates led to better AI responses: more consistent error handling, security suggestions, and adherence to clean code. For example, AI now prioritizes Jest tests and avoids insecure patterns.
- Git push worked after switching to SSH authentication with the personal key.
- Research from Cherny's thread provided actionable insights, like structuring rules hierarchically and emphasizing incremental changes.

## What Didn't Work
- Initial MCP setup failed due to the experimental flag not being enabled—resolved by toggling it and reloading VS Code.
- Git push initially failed with permission denied (HTTPS auth issues)—fixed by switching to SSH with proper key configuration.
- Some community sources had outdated info; filtered for recent, relevant practices.
- No major failures in rules testing, but AI occasionally suggested unverified libraries—mitigated by adding restrictions in the rules.

## Insights Gained
- Rules significantly align AI behavior with my intent by providing clear constraints (e.g., "prefer simple solutions" reduces over-engineering). They act as a "constitution," making the AI more reliable and less prone to hallucinations.
- From Cherny, iterative rule updates based on feedback improve outcomes—AI becomes a better pair programmer when guided on standards and collaboration.
- MCP logging enhances awareness of interaction patterns, showing how rules reduce vague responses and encourage proactive testing.
- Overall, configuring AI tools like MCP and rules fosters a more efficient, secure coding environment, aligning with modern AI-assisted development best practices.