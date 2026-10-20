# RepoGates

RepoGates checks what you or your AI agent is about to install (a GitHub repository, a Hugging Face model, a GitLab project, a VS Code or Docker Desktop extension, an agent skill or a Claude Code plugin) before its code reaches your machine.

- **In the browser:** a trust score on repository pages, and a download gate that holds a release-asset or Download ZIP download until the verdict is in.
- **For agents:** an MCP server and a Claude Code plugin, so the agent asks before it fetches. VS Code and Docker Desktop extensions and agent skills are answered through the MCP server and the plugin, not in the browser.

What it does not do: the browser extension does not see `git clone`, package managers or other command-line fetches. Inside Claude Code the plugin sees Bash tool calls in that one client and refuses a clone or install that names a blocked repository; it does not see anything else. We say that on every page where we offer it.

**Install and docs:** https://repogates.com  
**Research:** https://repogates.com/intel/fakegit.html · https://repogates.com/intel/malicious-skills.html  
**Contact:** support@repogates.com

RepoGates is built by Shuky Bendek through CISO Consultants Pty Ltd, Australia. This account holds no source code; everything installs from repogates.com.
