# Tool-Use Risk Checklist for AI Agents

## Permission boundaries

- [ ] Agent tools are explicitly listed
- [ ] Each tool has allowed use cases
- [ ] Dangerous tools require confirmation
- [ ] Write actions are separated from read actions
- [ ] External API calls are logged

## Data exposure

- [ ] Sensitive data is masked where possible
- [ ] Tool inputs are reviewed for unnecessary data
- [ ] Tool outputs are not blindly exposed to users
- [ ] Logs avoid secrets and private content

## Action safety

- [ ] Agent cannot perform irreversible actions without approval
- [ ] Agent has a dry-run mode for risky workflows
- [ ] Agent handles tool errors gracefully
- [ ] Agent escalates when context is insufficient

## Auditability

- [ ] Tool call history is preserved
- [ ] Decision rationale is available at a safe summary level
- [ ] Failures are linked to test cases
- [ ] Regression suite covers known failure modes
