# Initiate Deep Research Project

You are initiating a new deep research project. Follow these steps systematically:

## Step 1: Gather Research Context

First, interview the user to understand their research needs:

**Ask the following questions:**

1. **Research Topic**: What is the main topic or question you want to research?
2. **Research Objectives**: What are you hoping to learn or accomplish?
3. **Existing Knowledge**: What context or background information should I know?
4. **Scope**: Are there specific aspects to focus on or avoid?
5. **Depth**: How deep should this research go? (exploratory, comprehensive, exhaustive)
6. **Output Format**: What format do you need the final output in? (report, presentation, audio script, etc.)
7. **Timeline**: Is this research time-sensitive?
8. **Sources**: Are there specific sources or types of sources to prioritize or avoid?

## Step 2: Create Project Context File

Based on the user's answers, create a comprehensive context file:

**File**: `context/from-human/project-context.md`

**Contents should include:**
- Research topic and main questions
- Research objectives
- Scope and boundaries
- Depth requirements
- Timeline constraints
- Source preferences
- Expected deliverables
- Any domain-specific context provided

## Step 3: Generate Initial Research Plan

Create an initial research plan file:

**File**: `prompts/queue/research-plan.md`

**Include:**
- Breakdown of main research questions
- Sub-questions to explore
- Research sequence (what to research first)
- Estimated research phases
- Key areas to investigate

## Step 4: Draft Initial Research Prompts

Based on the research plan, create 3-5 initial research prompts:

**Location**: `prompts/run/initial/`

**Files**:
- `01-exploratory-research.md` - Broad overview of the topic
- `02-key-concepts.md` - Core concepts and terminology
- `03-current-state.md` - Current understanding/state of the field
- Additional prompts as needed

Each prompt should be:
- Specific and actionable
- Focused on a particular aspect
- Designed to build on previous prompts

## Step 5: Create Research Notes Template

Initialize the research notes file:

**File**: `notes/research-log.md`

**Template:**
```markdown
# Research Log - [Topic Name]

## Project Start Date
[Date]

## Research Objectives
[From context file]

## Research Sessions

### Session 1 - [Date]
**Focus**:
**Key Findings**:
**Questions Raised**:
**Next Steps**:

[Template for additional sessions]
```

## Step 6: Set Up Scratchpad

Create a scratchpad file for working notes:

**File**: `scratchpad/working-notes.md`

## Step 7: Begin Research Execution

Ask the user: "I've set up your deep research project. Would you like me to begin executing the initial research prompts, or would you like to review and refine the research plan first?"

**If user says begin:**
1. Start with the first initial prompt
2. Document findings in `outputs/individual/`
3. Update research log in `notes/`
4. Generate follow-up prompts in `prompts/run/subsequent/`
5. Continue systematically through the research plan

**If user wants to review:**
1. Show them the research plan
2. Accept modifications
3. Update prompts accordingly
4. Then begin when ready

## Step 8: Establish Research Rhythm

Set expectations for the research workflow:

**Inform the user:**
- After each research prompt execution, findings will be documented
- Follow-up questions will be generated based on discoveries
- Regular synthesis points will aggregate findings
- They can redirect or refine research direction at any time

## Throughout Research: Maintain Documentation

- Save all outputs to appropriate directories
- Keep research log updated
- Generate follow-up prompts based on findings
- Document connections between research threads
- Archive conversation histories periodically

## Research Session Conclusion

At natural stopping points, provide:
1. Summary of findings so far
2. Outstanding questions
3. Suggested next research directions
4. Draft aggregated output if appropriate

---

**Now begin by asking the Step 1 questions to understand the user's research needs.**
