# Root Protection Checklist

Before creating a new file:

1. Is it a system or control file?
2. Did Asaka explicitly ask for root placement?
3. If not, route it by FILE_ROUTING.md:
   - outputs -> artifacts/outputs/YYYY-MM-DD/
   - downloads -> artifacts/downloads/YYYY-MM-DD/
   - templates -> templates/
   - logs -> logs/
   - failures -> failures/
   - project files -> projects/
4. If the file is generated and temporary, avoid tracking it in git.
5. If the file may contain secrets or message bodies, keep it local and ignore it.

Git rule:
- Prefer tracking reusable system files.
- Prefer ignoring one-off generated deliverables unless Asaka explicitly wants them versioned.
