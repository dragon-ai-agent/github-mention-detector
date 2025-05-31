# github-mention-detector
A github action for detecting mentions of the dragon-ai agent

Setup:

```yaml
- name: Detect AI mention
  uses: dragon-ai-user/github-mention-detector@v1
  with:
    github-token: ${{ secrets.PAT_FOR_PR }}
    mention-pattern: "@dragon-ai-agent\\s+please\\s+(.*)"
```

Using a different agent account:

```yaml
- name: Detect AI mention
  uses: dragon-ai-user/github-mention-detector@v1
  with:
    github-token: ${{ secrets.PAT_FOR_PR }}
    mention-pattern: "@my-ai-agent\s+please\\s+(.*)"
```
