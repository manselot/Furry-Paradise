---
tags: [правила, yarn]
---

# Конвенции Yarn

## Спикеры и текст

- **Имя ГГ:** `{$username}` (в [[chapter1]] — `гг:`; унифицировать при правках).
- **Мысли:** `Мысли:` или `{$username}:*действие*`.
- **Действия** — в `*звёздочках*`.

## Команды

```yarn
<<character CharacterControl <id> "show"|"hide">>
<<bg RoomManager <bg>>>
```

| Что | Значения |
|---|---|
| `id` персонажа | `courtney`, `kara`, `eva`, `cassie` |
| `bg` фон | `shop1`, `"park"` |

## Локализация

`#line:<7 hex>` на строках в [[scene_03]], [[scene_04]], [[scene_06]].

> [!warning]
> Новые строки получают уникальные id. Существующие **не менять**.

## Переменные

Объявлять через `<<declare>>`.

| Переменная | Где ставится |
|---|---|
| `$username` | имя игрока |
| `$isYouTalkedWithCourtney` | [[scene_03]], читается в [[scene_04]] |
| `$gwen_doverie` | [[chapter1]] |
| `$gwen_interes` | [[chapter1]] |
| `$secret_publichen` | [[chapter1]] |

## Структура ноды

```yarn
title: имя_ноды
position: x,y
---
текст
===
```
