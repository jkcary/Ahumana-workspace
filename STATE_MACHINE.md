Task State Machine

States

INIT
Task received

CLARIFIED
Requirements understood

PLANNED
Steps defined (if complex)

EXECUTING
Task in progress

VERIFYING
Output being checked

COMPLETED
Task finished successfully

FAILED
Task failed

RETRYING
Re-attempt in progress

Rules

Do not skip states
Complex tasks must go through PLANNED
Always verify before COMPLETED
FAILED must trigger analysis

Transition Logic

INIT -> CLARIFIED -> (PLANNED) -> EXECUTING -> VERIFYING -> COMPLETED

If failure:
-> FAILED -> RETRYING -> EXECUTING
