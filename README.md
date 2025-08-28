# zsh-config


### Others

#### Homebrew
~~~
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
~~~

#### docker
~~~
brew install docker docker-buildx docker-compose colima uv
~~~

#### iStat Menus
https://bjango.com/mac/istatmenus/

### Claude
1. Install Node.js
    - https://nodejs.org/ko/download
2. Install Claude CLI
    - npm install -g @anthropic-ai/claude-code
3. Install Claude Code Usage Tracker
    - npm install -g ccusage
4. Register Model Context Protocol (MCP) plugins
    - claude mcp add context7 -- npx -y @upstash/context7-mcp --api-key
    - claude mcp add sequential-thinking -- npx -y @modelcontextprotocol/server-sequential-thinking
    - claude mcp add github -- npx -y @modelcontextprotocol/server-github --api-key