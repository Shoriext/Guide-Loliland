---
id: "primer:interfaces"
title: "Интерфейсы"
feedback: true
icon:
  item: "appliedenergistics2:tile.BlockInterface"
  meta: 0
---

В данной статье речь пойдет о МЭ интерфейсах, их функциях и возможностях.

# Интерфейсы {#interfaces-base}

**Интерфейсы** – один из основных функциональных блоков, используемых в МЭ-системе.

Обладает несколькими основными функциями:

- Поставляет шаблоны для [сборщиков](guide:primer:assemblers) и механизмов.
- Поддерживает 2 вида шаблонов
  - <item id="appliedenergistics2:item.ItemEncodedPattern" />
  - <item id="loli_technologies:item.ItemLargePattern" />
- Принимает и отправляет в систему ресурсы из механизмов, которые имеют автоматическое выталкивание.
- При соответствующей настройке могут поставлять ресурсы в механизмы с функцией затягивания.

:::callout{type="tip"}
Обратите внимание, что буфер интерфейса сильно больше визуального. Он может принимать огромное количество ресурсов за раз.
:::

# Виды интерфейсов {#interfaces-types}

Всего существует несколько видов интерфейсов, которые отличаются только количеством поддерживаемых шаблонов:

- <item id="appliedenergistics2:tile.BlockInterface" /> – поддерживает 9 шаблонов
- <item id="loli_technologies:tile.BlockCraftingInterfaceX2" /> – поддерживает 18 шаблонов
- <item id="loli_technologies:tile.BlockCraftingInterfaceX3" /> – поддерживает 27 шаблонов
- <item id="loli_technologies:tile.BlockCraftingInterfaceX4" /> – поддерживает 36 шаблонов

Также <item id="loli_technologies:tile.BlockCraftingInterfaceX4" display="icon" /> имеет несколько декоративных аналогов, которые отличаются только визуально:

- <item id="loli_technologies:tile.BlockGoldCraftingInterface" />
- <item id="loli_technologies:tile.BlockInfiniteCraftingInterface" />
- <item id="loli_technologies:tile.BlockDemonicCraftingInterface" />

Для каждого **интерфейса** существует плоский аналог – <item id="appliedenergistics2:item.ItemMultiPart" meta="440" />. Он занимает меньше места. В один блок может быть установлено до четырех штук.

# Интерфейс Вис-реле {#interfaces-vis}

<item id="appliedenergistics2:item.ItemMultiPart" meta="600" /> – особый вид интерфейса, который используется для передачи вис-аспектов из [пробужденного узла](guide:primer:awakening-node-3) в <item id="appliedenergistics2:tile.BlockArcaneAssembler" /> или <item id="loli_technologies:tile.BlockArcaneImprovedAssembler" />.