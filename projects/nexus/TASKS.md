# Nexus Tasks

## Active

| ID | Task | Status | Verification |
|---|---|---|---|
| NEX-001 | Review and verify the Vault foundation | in-review | Confirm expected files, registries, and project content through GitHub readback |
| NEX-002 | Restore application dependency installation | blocked | `npm install` succeeds using a working public registry or approved package source |
| NEX-003 | Execute Foundation MVP checks | blocked | Tests, repository-local lint check, and Vite build pass after NEX-002 |
| NEX-004 | Verify application project listing against the Vault | pending | `/api/v1/projects` returns the Nexus registry row without AI |

## Next

| ID | Task | Status | Verification |
|---|---|---|---|
| NEX-005 | Specify controlled Vault writes | proposed | Approved conflict, validation, audit, and rollback rules |
| NEX-006 | Add project creation workflow | proposed | A project can be created from the standard contract with registry updates |
| NEX-007 | Add NVIDIA reasoning | proposed | Reasoning operates only on selected context and exposes its context sources |
| NEX-008 | Add daily planning | proposed | `planning/TODAY.md` is produced from real tasks, projects, and daily records |

## Task Rules

- `proposed` is not approved implementation scope.
- A pull request is not proof that a task is verified or completed.
- Blocked tasks must name the blocking evidence.
- Completed tasks should retain verification evidence in the project changelog or linked decision record.
