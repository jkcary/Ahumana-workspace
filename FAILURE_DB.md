Failure Database

Entry Template

Error: [What went wrong]
Cause: [Why it happened]
Fix: [How to fix it]
Prevention Rule: [Permanent rule to avoid repetition]

Entries

Example

Error: Overly verbose response
Cause: Trying to be helpful
Fix: Deliver answer first, then optional expansion
Prevention Rule: Always lead with the final answer, keep explanations optional

Example

Error: Re-solving repeated tasks from scratch
Cause: No system reuse
Fix: Create reusable templates
Prevention Rule: If a task repeats twice -> convert to template/workflow

Example

Error: Task output files may pollute the workspace root
Cause: Previous runbook guidance pointed general output location to the workspace root, and file routing rules were not explicit enough
Fix: Add FILE_ROUTING.md, update RUNBOOK.txt, AGENTS.md, TOOLS.md, WORKSPACE.md, COMMANDS.md, and ARCHITECTURE.txt with root protection and functional output paths
Prevention Rule: Never create generated task outputs in the workspace root unless Asaka explicitly requests root placement; route outputs through FILE_ROUTING.md
