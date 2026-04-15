File Routing Policy

Purpose

Prevent task outputs from polluting the workspace root.

Root Directory Rule

The workspace root is reserved for Ahumana system and OpenClaw control files only.

Do not create user task outputs in the workspace root.

Root files are allowed only when they are:

OpenClaw identity files
Ahumana system doctrine files
runtime control files
explicitly requested by Asaka

Task Output Rule

All task-generated files must be stored under a functional subdirectory.

Default Output Location

If the user does not specify a path, save task outputs to:

artifacts/outputs/YYYY-MM-DD/

Downloads

Downloaded or externally sourced task files go to:

artifacts/downloads/YYYY-MM-DD/

Generated Deliverables

Reports, plans, documents, research outputs, exports, and final deliverables go to:

artifacts/outputs/YYYY-MM-DD/

Reusable Assets

Reusable frameworks, structured assets, and reference material go to:

artifacts/

Templates

Reusable templates go to:

templates/

Project Files

Files tied to ongoing projects go to:

projects/

Logs

Execution logs, task records, and trace files go to:

logs/

Failures

Error records and failure analysis go to:

failures/

Archive

Old, replaced, or deprecated files go to:

archive/

Naming Standard

Use clear, descriptive names.
Use lowercase words separated by underscores or hyphens.
Include dates for generated task outputs when useful.

Examples

artifacts/outputs/2026-04-15/market_research_summary.md
artifacts/downloads/2026-04-15/source_material.pdf
templates/product_launch_plan.md
projects/ahumana_operator_system/next_steps.md
logs/2026-04-15_task_log.md
failures/repeated_root_output_pollution.md

Root Protection Rule

Before creating any new file in the workspace root, ask:

Is this a system/control file?
Did Asaka explicitly request root placement?

If both answers are no:

route the file into the appropriate subdirectory.

Conflict Rule

If a requested filename conflicts with a root system file:

do not overwrite it
create the task file in the appropriate subdirectory
explain the chosen location briefly

Final Rule

Task outputs and system source files must remain separate.
