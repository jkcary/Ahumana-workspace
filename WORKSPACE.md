Workspace Doctrine

Purpose

Maintain a clean, fast, high-signal execution environment.

Core Principles

Every file should have a purpose.
Every useful output should be retrievable.
Clutter is a tax on future execution.
System files and task outputs must stay separate.

Organization Rules

Group by function, not randomness.
Use predictable naming.
Prefer a small number of strong folders over many weak ones.
Avoid duplicate outputs with slightly different names.
Do not write generated task files to the workspace root.

Retrieval Rules

Optimize for:

fast lookup
exact retrieval
low ambiguity
durable structure

Recommended Functional Structure

/identity
/system
/projects
/artifacts
/artifacts/outputs
/artifacts/downloads
/templates
/logs
/failures
/archive
/skills

Root Directory Policy

The workspace root is for OpenClaw and Ahumana system/control files only.

Task outputs must be stored under:

artifacts/outputs/YYYY-MM-DD/

Downloads and external source files must be stored under:

artifacts/downloads/YYYY-MM-DD/

If a generated file is reusable, promote or copy it into:

artifacts/
templates/
projects/

depending on its function.

Git Hygiene Policy

Version control should preserve reusable structure, not local noise.

Track by default:
- system/control files
- reusable templates
- curated docs and durable project files

Keep local by default:
- one-off outputs
- downloads
- runtime state
- email artifacts
- transient operational files

If an output graduates from one-off to reusable, move or copy it into a tracked location before committing.

Cleanliness Rule

If a file no longer serves:

archive it
merge it
remove it

Do not let the workspace decay into confusion.

Asset Rule

Outputs that are likely to be reused should be upgraded into artifacts or templates.
