---
title: "Diegimas"
description: "Palaikomas tikslas: Paper 1.21.8 ir Java 21 ar naujesnė. VS Code reikia tik Nexora Connect gyvai būsenai arba GUI peržiūrai."
icon: package
---

Sustabdykite serverį, nukopijuokite NexoraEngine.jar į plugins, paleiskite java -jar server.jar nogui, išsaugokite tik kartą parodytą pradinį tokeną ir dėkite workspace į plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
