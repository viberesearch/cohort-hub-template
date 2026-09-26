# rules/local — this hub's settings (never overwritten by template updates)

Create `hub.yaml`:

```yaml
org: <github-org>
hub: <repo-name>
hub_documents_language: ru
review_window_hours: 48
asr: {engine: "", diarization: "", where: local | cloud}
audio_storage: "<cloud folder link>"
participants: []        # [{login: "", team: ""}]
organizers: []          # [{login: ""}]
```
