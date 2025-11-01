# Claude Deep Research Template

[![Claude Code](https://img.shields.io/badge/Claude-Code-8A2BE2?logo=anthropic&logoColor=white)](https://claude.ai/claude-code)
[![Claude Code Projects](https://img.shields.io/badge/Claude_Code-Projects_Index-blue?logo=github)](https://github.com/danielrosehill/Claude-Code-Repos-Index)
[![GitHub Master Index](https://img.shields.io/badge/GitHub-Master_Index-green?logo=github)](https://github.com/danielrosehill/Github-Master-Index)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A production-ready template for conducting systematic, comprehensive research using Claude Code. This implementation leverages an organized flow of data from previous outputs into persistent context, enabling iterative and cumulative research workflows.

## What is This?

This template provides a complete, structured workflow for using Claude Code as a deep research assistant. Instead of ad-hoc conversations, this approach:

- **Systematizes research** with clear phases and workflows
- **Documents everything** in organized directories
- **Generates reusable outputs** in multiple formats
- **Builds on previous work** through structured context
- **Scales from quick investigations to comprehensive studies**

## Background and Concept

**Planning and Development Notes**: [Claude-Deep-Research-Model Repository](https://github.com/danielrosehill/Claude-Deep-Research-Model)
This repository contains my planning and development notes for the concept behind this implementation, which attempts to leverage an organized flow of data from previous outputs into persistent context, among other features.

**Concept Discussion Podcast**: [Listen on Spotify](https://open.spotify.com/episode/0AuchKOm47XdKSGDePfEJq?si=4Q2Gl12sQtej6eT1oo9RDQ)
Audio discussion explaining the concept in detail.

## Quick Start

### 1. Use This Template

Click "Use this template" on GitHub or clone locally:

```bash
git clone https://github.com/danielrosehill/Claude-Deep-Research-Template.git my-research-project
cd my-research-project
```

### 2. Initialize Your Research

Open the repository in Claude Code and run:

```bash
/initiate-research
```

Claude will interview you about your research needs and set up your project.

### 3. Start Researching

Follow Claude's guidance through the research workflow:
- Context gathering
- Prompt planning
- Research execution
- Output synthesis

## Directory Structure

```
├── .claude/
│   ├── commands/          # Slash commands (e.g., /initiate-research)
│   └── agents/            # Specialized research agents
├── context/               # Research context and source materials
│   ├── from-internet/    # Web research, papers, articles
│   ├── from-human/       # Your context and requirements
│   └── from-history/     # Previous conversation histories
├── prompts/              # Research prompts by stage
│   ├── drafting/         # Draft prompts
│   ├── queue/            # Prompts ready to execute
│   └── run/              # Executed prompts
│       ├── initial/      # Starting prompts
│       └── subsequent/   # Follow-up prompts
├── outputs/              # Research outputs
│   ├── individual/       # Single-topic outputs
│   ├── aggregated/       # Synthesized reports
│   └── reformatted/      # Alternative formats (TTS, SSML)
├── pipeline/             # Workflow automation
├── notes/                # Research notes and logs
└── scratchpad/          # Working area for experiments
```

## How It Works

### Research Workflow

1. **Context Gathering** - Provide background, objectives, and constraints
2. **Prompt Planning** - Claude generates research questions systematically
3. **Research Execution** - Execute prompts, document findings, generate follow-ups
4. **Output Synthesis** - Aggregate findings into comprehensive reports
5. **Iteration** - Build on previous research in subsequent sessions

### Specialized Agents

The template includes three specialized agents:

- **Research Coordinator** - Orchestrates the overall workflow
- **Prompt Generator** - Creates effective research questions
- **Research Synthesizer** - Aggregates findings into reports

## Key Features

### Systematic Research
- Structured phases from exploration to synthesis
- Clear progression through research depth
- Built-in quality checkpoints

### Comprehensive Documentation
- All findings automatically documented
- Research log tracks progress
- Conversation histories archived

### Multiple Output Formats
- Markdown reports
- PDF documents
- TTS-safe text
- SSML for voice synthesis

### Reusable Context
- Build on previous research sessions
- Archive and reference past work
- Continuous knowledge accumulation

## Slash Commands

- `/initiate-research` - Start a new deep research project

Add your own custom commands in `.claude/commands/`

## Use Cases

This template works for:

- **Academic Research** - Literature reviews, topic exploration
- **Market Research** - Industry analysis, competitive intelligence
- **Technical Investigation** - Technology evaluation, architecture research
- **Strategic Planning** - Trend analysis, scenario planning
- **Content Creation** - Research for articles, presentations, reports
- **Learning** - Deep dives into new subjects

## Configuration

### CLAUDE.md

The `CLAUDE.md` file contains instructions for Claude on how to operate in this repository. Customize it for your specific needs.

### Custom Slash Commands

Create new slash commands in `.claude/commands/`:

```bash
.claude/commands/my-command.md
```

### Custom Agents

Define specialized agents in `.claude/agents/`:

```bash
.claude/agents/my-agent.md
```

## Best Practices

1. **Start with /initiate-research** - Let Claude set up your project properly
2. **Provide rich context** - The more context, the better the research
3. **Review and refine** - Check Claude's research plan before execution
4. **Synthesize regularly** - Don't wait until the end to aggregate
5. **Archive conversations** - Save conversation histories for future reference

## Tips for Deep Research

- **Be specific about objectives** - Clear goals lead to focused research
- **Iterate on prompts** - Refine research questions based on findings
- **Use the scratchpad** - Experiment without cluttering main outputs
- **Document methodology** - Note how you arrived at conclusions
- **Build incrementally** - Research in sessions, build on previous work

## Example Workflow

```bash
# 1. Clone template
git clone <template-url> my-research

# 2. Open in Claude Code
cd my-research
claude-code .

# 3. Initialize research
/initiate-research

# 4. Provide context when prompted
# - Research topic
# - Objectives
# - Scope and depth
# - Output requirements

# 5. Review generated research plan
# - Approve or refine

# 6. Let Claude execute research
# - Findings documented automatically
# - Follow-up prompts generated
# - Progress tracked

# 7. Generate synthesis
# - Request aggregated report
# - Multiple formats created

# 8. Continue or conclude
# - Archive session
# - Plan next session
# - Or finalize deliverables
```

## Contributing

Suggestions and improvements welcome! This template is designed to evolve based on real-world usage.

## Related Projects

- [Claude Deep Research Model](https://github.com/danielrosehill/Claude-Deep-Research-Model) - Concept and model notes
- [Claude Code Projects Index](https://github.com/danielrosehill/Claude-Code-Repos-Index) - More Claude Code projects

## License

MIT License - See LICENSE file for details

## Author

**Daniel Rosehill**
- Website: [danielrosehill.com](https://danielrosehill.com)
- Email: public@danielrosehill.com
- GitHub: [@danielrosehill](https://github.com/danielrosehill)

---

## Acknowledgments

Based on the Claude Deep Research Model concept. Special thanks to the Claude Code team at Anthropic for creating such a powerful research tool.
