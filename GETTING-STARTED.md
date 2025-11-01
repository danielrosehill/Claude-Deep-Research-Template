# Getting Started with Claude Deep Research

## Understanding the Concept

Before diving into setup, you may want to learn about the conceptual framework:

- **Planning Notes Repository**: [Claude-Deep-Research-Model Repository](https://github.com/danielrosehill/Claude-Deep-Research-Model) - Planning and development notes for the concept behind this implementation
- **Audio Explanation**: [Spotify Podcast Episode](https://open.spotify.com/episode/0AuchKOm47XdKSGDePfEJq?si=4Q2Gl12sQtej6eT1oo9RDQ) - Listen to a detailed discussion of the concept

## First Time Setup

### Prerequisites

- Claude Code CLI installed
- Git configured
- Basic familiarity with markdown

### Initial Setup

1. **Create your research project from this template:**

   ```bash
   # Using GitHub's template feature (recommended)
   # Click "Use this template" on GitHub

   # Or clone and remove git history
   git clone https://github.com/danielrosehill/Claude-Deep-Research-Template.git my-research
   cd my-research
   rm -rf .git
   git init
   ```

2. **Open in Claude Code:**

   ```bash
   claude-code .
   ```

3. **Run the initialization command:**

   ```
   /initiate-research
   ```

## Your First Research Session

### Step 1: Answer Claude's Questions

Claude will ask you about:
- Your research topic
- Your objectives
- How deep you want to go
- What output formats you need
- Any specific constraints

**Example responses:**

```
Research Topic: "The impact of AI on software development practices"

Objectives:
- Understand current state of AI coding assistants
- Identify best practices for integration
- Assess productivity impacts
- Identify potential risks

Depth: Comprehensive - I want a thorough investigation

Output: Final report in markdown and PDF, plus audio script version

Timeline: Not urgent, thorough research is priority

Sources: Technical blogs, academic papers, industry reports
```

### Step 2: Review the Research Plan

Claude will generate:
- A project context file in `context/from-human/`
- A research plan in `prompts/queue/`
- Initial research prompts in `prompts/run/initial/`

Review these and provide feedback. You can:
- Request modifications
- Add specific areas to investigate
- Remove or refine prompts

### Step 3: Begin Research

When you're ready, tell Claude to proceed. Claude will:
1. Execute the first research prompt
2. Document findings in `outputs/individual/`
3. Generate follow-up questions
4. Continue systematically

### Step 4: Monitor Progress

During research, Claude will:
- Update the research log in `notes/`
- Show you interesting findings
- Ask for your input at decision points
- Suggest when to synthesize

## Understanding the Structure

### Where Things Go

**Context files** (`context/`):
- `from-human/` - Your input, requirements, domain knowledge
- `from-internet/` - Research materials Claude gathers
- `from-history/` - Previous session transcripts

**Prompts** (`prompts/`):
- `drafting/` - Claude's prompt experiments
- `queue/` - Ready-to-run prompts
- `run/initial/` - Broad exploratory prompts
- `run/subsequent/` - Focused follow-up prompts

**Outputs** (`outputs/`):
- `individual/` - Single research topics
- `aggregated/` - Combined reports
- `reformatted/` - Different formats (TTS, SSML, PDF)

**Notes** (`notes/`):
- Research log
- Methodology notes
- Observations and insights

**Scratchpad** (`scratchpad/`):
- Working area
- Experiments
- Temporary notes

## Common Workflows

### Quick Investigation

```
/initiate-research
[Answer questions with narrow scope]
[Let Claude research for 30-60 minutes]
[Request synthesis]
[Done!]
```

### Deep Research Project

```
/initiate-research
[Provide comprehensive context]
[Review and refine research plan]
[Session 1: Exploratory research]
[Review findings, adjust direction]
[Session 2-3: Deep dives on key areas]
[Periodic synthesis of findings]
[Session 4: Gap filling]
[Final synthesis and report generation]
```

### Iterative Research

```
Session 1:
- Initialize project
- Conduct initial research
- Archive conversation

Session 2:
- Review previous findings in context/from-history/
- Define new questions based on session 1
- Continue research
- Archive conversation

[Repeat as needed]
```

## Tips for Success

### Providing Good Context

✅ **Do:**
- Be specific about your goals
- Share domain knowledge
- Mention what you already know
- Clarify what matters most
- Set clear boundaries

❌ **Don't:**
- Give vague objectives like "learn about AI"
- Assume Claude knows your specific context
- Skip the initialization interview
- Forget to mention constraints

### Working with Claude

✅ **Do:**
- Review and refine the research plan
- Provide feedback during research
- Ask Claude to go deeper on interesting areas
- Request synthesis at logical points
- Archive sessions regularly

❌ **Don't:**
- Let Claude research without direction
- Ignore the suggested workflow
- Delete conversation histories
- Skip documentation steps
- Rush to synthesis too early

### Organizing Your Research

✅ **Do:**
- Use descriptive filenames with dates
- Keep related materials together
- Archive completed sessions
- Maintain the directory structure
- Update the research log

❌ **Don't:**
- Create ad-hoc directories
- Mix different research projects
- Delete intermediate outputs
- Ignore naming conventions
- Skip documentation

## Troubleshooting

### "Claude isn't following the workflow"

Make sure CLAUDE.md is present and Claude has read it. You can explicitly say:
```
Please read CLAUDE.md and follow the deep research workflow
```

### "The directory structure is confusing"

Focus on these key locations:
- Put your context in `context/from-human/`
- Check outputs in `outputs/individual/`
- Read the research log in `notes/research-log.md`

Everything else is supporting structure.

### "I want to customize the workflow"

Edit `CLAUDE.md` to change how Claude operates:
- Add custom instructions
- Modify the workflow
- Define different output formats
- Add project-specific rules

### "Research is too broad/narrow"

During initialization or any time during research:
```
Let's refocus on [specific aspect]
```

Or:
```
Let's broaden this to also cover [related areas]
```

## Next Steps

After your first successful research session:

1. **Try different research depths**
   - Quick investigation
   - Moderate research
   - Exhaustive deep dive

2. **Experiment with output formats**
   - Different synthesis styles
   - Multiple formats
   - Custom templates

3. **Create custom slash commands**
   - Add commands for your recurring needs
   - See `.claude/commands/` for examples

4. **Develop specialized agents**
   - Create agents for your domain
   - See `.claude/agents/` for examples

## Getting Help

- Review the main [README.md](README.md)
- Check [CLAUDE.md](CLAUDE.md) for workflow details
- See the [concept repository](https://github.com/danielrosehill/Claude-Deep-Research-Model) for background
- Ask Claude! It understands this system and can guide you

## Example Research Projects

**Technical Investigation:**
```
Topic: "Evaluating vector databases for RAG applications"
Depth: Comprehensive
Focus: Performance, cost, ease of use, scalability
Output: Technical comparison report + decision matrix
```

**Market Research:**
```
Topic: "AI-assisted coding tools market landscape"
Depth: Moderate
Focus: Key players, pricing, features, trends
Output: Market overview report + presentation deck
```

**Academic Research:**
```
Topic: "Literature review on transformer architectures"
Depth: Exhaustive
Focus: Evolution, variants, applications, future directions
Output: Academic-style literature review + bibliography
```

---

Ready to start your first deep research project? Run `/initiate-research` and let Claude guide you through the process!
