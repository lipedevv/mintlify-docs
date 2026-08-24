---
title: "AI development"
description: "Official machine-readable Nexora documentation for ChatGPT, Claude, Cursor, Codex, and other coding agents."
icon: "bot"
---

# Develop Nexora workspaces with AI

Use these official endpoints as context before asking an AI agent to create, review, or debug a Nexora workspace.

<CardGroup cols={2}>
  <Card title="llms.txt" icon="list-tree" href="https://nexora.mintlify.site/llms.txt">
    Compact documentation index. Use it to locate the correct guide or API reference.
  </Card>
  <Card title="llms-full.txt" icon="file-text" href="https://nexora.mintlify.site/llms-full.txt">
    Complete English documentation in one machine-readable context file.
  </Card>
  <Card title="skill.md" icon="sparkles" href="https://nexora.mintlify.site/skill.md">
    Nexora capabilities, constraints, and reliable development workflow for AI agents.
  </Card>
  <Card title="Agent skills discovery" icon="radar" href="https://nexora.mintlify.site/.well-known/agent-skills/index.json">
    Machine-readable index of the specialized Nexora skills.
  </Card>
</CardGroup>

## Install the Nexora skills

Agents compatible with the Agent Skills standard can install the published skills directly from the documentation site.

```bash
npx skills add https://nexora.mintlify.site
```

## Recommended prompt

```text
Read https://nexora.mintlify.site/llms.txt and the relevant Nexora skill before editing.
Create a Safe Mode JavaScript workspace for Nexora 1.0.0.
Use only documented APIs and capabilities. Do not use TypeScript, Node.js packages,
a build step, or manual deployment. Validate database and inventory operations for
atomicity and explain how to test the result on Paper.
```

<Warning>
  AI-generated code must not invent Nexora APIs. If a symbol is absent from the JavaScript API reference, treat it as unsupported.
</Warning>

## Regras essenciais em português

- Use JavaScript (`.js` ou `.mjs`), nunca TypeScript.
- Salve diretamente em `plugins/NexoraEngine/workspaces/<id>`; o recarregamento é automático.
- Prefira Safe Mode. Native Mode exige necessidade explícita e capability declarada.
- Em economia, lojas e inventários, use transações e reembolso quando a entrega falhar.
- Consulte a referência da API antes de utilizar qualquer método ou evento.
