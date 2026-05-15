# Opencode CLI

AI-powered coding assistant CLI tool.

## Installation

```bash
npm install
npm run build
npm link  # Global install to use the command
```

## Usage

```bash
# Display help
opencode --help
opencode help

# Authentication
opencode login                    # Login via browser
opencode login --token <token>    # Login with API token

# Initialize project
opencode init                     # Initialize with default template
opencode init -n my-project       # Specify project name
opencode init -t typescript       # Use specific template

# Manage AI models
opencode model --list             # List available models
opencode model --set gpt-4        # Set default model
opencode model --info gpt-4       # Show model info

# Other commands
opencode clear                    # Clear screen
opencode clear --cache            # Clear cache
opencode clear --history          # Clear command history
opencode chat                     # Start interactive chat
opencode chat "Hello!"            # Send a message
opencode status                   # Check system status
```

## Available Commands

| Command | Description | Options |
|---------|-------------|---------|
| `help` | Show help information | - |
| `login` | Authenticate with your account | `--token` |
| `init` | Initialize a new project | `-t, --template`, `-n, --name` |
| `model` | Manage AI models | `-l, --list`, `-s, --set`, `-i, --info` |
| `clear` | Clear screen or cache | `--cache`, `--history` |
| `chat` | Start interactive chat session | `[message]` |
| `status` | Check system status | - |

## Examples

```bash
# Login and check status
opencode login
opencode status

# Initialize a new project
opencode init -n my-app -t react

# List and switch models
opencode model --list
opencode model --set claude-3

# Chat with AI
opencode chat "How do I create a React component?"
```

## Development

```bash
# Run in dev mode
npm run dev -- help

# Build
npm run build

# Run built version
npm start
```

## Project Structure

```
my-agent-node-cli/
├── src/
│   └── cli.ts          # CLI entry point
├── dist/               # Compiled output
├── package.json
├── tsconfig.json
└── README.md
```

## Publish to npm

```bash
npm login
npm publish
```

After publishing, users can install globally:
```bash
npm install -g my-agent-node-cli
opencode help
```
