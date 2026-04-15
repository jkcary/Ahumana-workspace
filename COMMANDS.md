Command Protocol

Purpose

Standardize how tasks are interpreted and executed.

Command Structure

Each task should be interpreted as:

Objective: what needs to be done
Constraints: limits or requirements
Output: expected result format
Priority: importance level
Scope: simple or complex
Destination: where generated files should be saved

Task Types

SIMPLE
direct execution
no planning required

COMPLEX
requires planning
multi-step execution
may involve iteration

Execution Rule

Do not start execution until the task is clearly defined
If unclear -> clarify or infer with minimal assumptions

Output Rule

Always produce:

result first
explanation only if needed

File Destination Rule

If output creates files and no destination is specified:

use artifacts/outputs/YYYY-MM-DD/

If output is a download or external source material:

use artifacts/downloads/YYYY-MM-DD/

Do not use the workspace root for task outputs.

Compression Rule

Remove unnecessary steps
Avoid redundant actions
Optimize for minimal effort with correct output
