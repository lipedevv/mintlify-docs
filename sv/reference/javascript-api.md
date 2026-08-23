---
title: "JavaScript API-referens"
description: "Alla symboler finns globalt och via objektet Nexora. Asynkrona operationer återgår säkert till workspace-runtime."
icon: book-open
---

## Kärna

| Symbol | Returns | Capability |
| --- | --- | --- |
| on(name, callback, options?) | Disposable | minecraft.players |
| command(name, definition) | Disposable | minecraft.commands |
| item(material, options?) | ItemStack | minecraft.inventory |
| gui.chest(definition) | Gui | minecraft.inventory |

## Schemaläggare

| Symbol | Returns | Capability |
| --- | --- | --- |
| scheduler.nextTick(callback) | Task | — |
| scheduler.delay(ticks, callback) | Task | — |
| scheduler.repeat(intervalTicks, callback, delayTicks?) | Task | — |
| task.cancel() / task.dispose() | void | — |

## Lagring

| Symbol | Returns | Capability |
| --- | --- | --- |
| storage.get(key, fallback?) | Promise&lt;T &#124; undefined&gt; | filesystem.workspace |
| storage.set(key, value) | Promise&lt;void&gt; | filesystem.workspace |
| storage.delete(key) | Promise&lt;boolean&gt; | filesystem.workspace |
| storage.keys(prefix?) | Promise&lt;string[]&gt; | filesystem.workspace |

## SQLite

| Symbol | Returns | Capability |
| --- | --- | --- |
| database.query(sql, parameters?) | Promise&lt;Row[]&gt; | database |
| database.execute(sql, parameters?) | Promise&lt;&#123; affectedRows &#125;&gt; | database |
| database.transaction(statements) | Promise&lt;&#123; affectedRows[] &#125;&gt; | database |

## HTTP

| Symbol | Returns | Capability |
| --- | --- | --- |
| http.get(url, options?) | Promise&lt;HttpResponse&gt; | http |
| http.post(url, body?, options?) | Promise&lt;HttpResponse&gt; | http |
| http.put(url, body?, options?) | Promise&lt;HttpResponse&gt; | http |
| http.delete(url, options?) | Promise&lt;HttpResponse&gt; | http |

## Server och loggning

| Symbol | Returns | Capability |
| --- | --- | --- |
| server.onlinePlayers | Player[] | minecraft.players |
| server.getPlayer(nameOrUuid) | Player &#124; null | minecraft.players |
| server.broadcast(miniMessage) | void | minecraft.players |
| server.mainThread(callback) | Promise&lt;T&gt; | — |
| log.debug/info/warn(message, context?) | void | — |
| log.error(message, error?) | void | — |

## Spelare

| Symbol | Returns | Capability |
| --- | --- | --- |
| player.name / uuid / online | string / boolean | minecraft.players |
| player.health / maxHealth | number | minecraft.players |
| player.gamemode | GameMode | minecraft.players |
| player.location | Location | minecraft.players |
| player.send(message) | void | minecraft.players |
| player.heal(amount?) / damage(amount) | void | minecraft.players |
| player.teleport(location) | void | minecraft.players |
| player.give(...items) | void | minecraft.inventory |
| player.hasPermission(permission) | boolean | minecraft.players |
| player.kick(message?) | void | minecraft.players |
| player.playSound(sound, volume?, pitch?) | void | minecraft.players |
| player.showTitle(...) / showActionBar(message) | void | minecraft.players |
| player.openGui(gui) | void | minecraft.inventory |

## Inventory

| Symbol | Returns | Capability |
| --- | --- | --- |
| inventory.size | number | minecraft.inventory |
| inventory.get(slot) | ItemStack &#124; null | minecraft.inventory |
| inventory.set(slot, item) | void | minecraft.inventory |
| inventory.add(...items) | void | minecraft.inventory |
| inventory.canFit(...items) | boolean | minecraft.inventory |
| inventory.tryAdd(...items) | boolean | minecraft.inventory |
| inventory.clear() | void | minecraft.inventory |

## GUI

| Symbol | Returns | Capability |
| --- | --- | --- |
| gui.slot(index, item, onClick?) | Gui | minecraft.inventory |
| gui.components(map) | Gui | minecraft.inventory |
| gui.on(open&#124;close&#124;click&#124;drag, callback) | Gui | minecraft.inventory |
| gui.open(player) | void | minecraft.inventory |
| gui.snapshot() | GuiSnapshot | minecraft.inventory |
| gui.dispose() | void | minecraft.inventory |

## Nativ åtkomst

| Symbol | Returns | Capability |
| --- | --- | --- |
| native.paper(className) | Java Class | native.paper + Native Mode |
| native.plugin(name) | Plugin &#124; null | native.paper + Native Mode |

## ItemOptions

| Field | Type | Status / behavior |
| --- | --- | --- |
| material | string | required |
| amount | number | implemented |
| name | MiniMessage | implemented |
| lore | MiniMessage[] | implemented |
| enchanted | boolean | implemented |
| customModelData | number | implemented |
| component | string | snapshot metadata |
| serialized | string | opaque exact ItemStack restore |
| enchantments | Record&lt;string, number&gt; | applied through the Bukkit enchantment registry |
| unbreakable | boolean | implemented |
| durability | number | item damage value, clamped to the material maximum |
| flags | string[] | validated Bukkit item flags |
| persistentData | Record&lt;string, primitive&gt; | stored only in the nexora namespace |
| playerHead | string | player name or UUID for PLAYER_HEAD |
