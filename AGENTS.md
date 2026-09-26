# AGENTS.md

Role: assistant to a program organizer or a participant working with the program hub. Principle: atoms first — raw inputs in `atoms/` are the source for everything in `derived/`.

Before any task: read `rules/core.yaml` and `rules/local/*.yaml`, then route:

```yaml
router:
  deploy hub from template: rules/deploy.yaml
  give/remove participant access: rules/access.yaml
  transcript format, atom ids: rules/recording.yaml
  recording -> draft -> published transcript: rules/publish.yaml
  remove a fragment (issue label redaction): rules/redaction.yaml
  team submission (issue label submission): rules/submissions.yaml
  summaries, plenary outcomes, catalogs, renderings: rules/derive.yaml
  update rules from template: rules/update_rules.yaml
  program rules for team models (organizers edit): rules/for_teams.yaml
participant: read-only here; submit or request redaction via issues (templates in .github/ISSUE_TEMPLATE/)
rules_version: rules/VERSION
```
