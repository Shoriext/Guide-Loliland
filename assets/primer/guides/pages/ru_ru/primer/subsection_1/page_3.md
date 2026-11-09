---
id: "primer:page-3"
title: "Страница 3"
feedback: true
icon:
  item: "minecraft:furnace"
---

Это вводный абзац. Тут карточки, 3D-сцена, рецепт и таблицы.

# Карточки предметов {#item-cards icon-item="minecraft:chest"}

:::item-card{item="minecraft:chest"}
А вот тут можно сделать описание предмета.\
Вместимость: 27 слотов
:::

:::item-card{item="minecraft:hopper"}
Тут описание второго предмета. Карточки можно ставить подряд.
:::

# Карточка механизма {#block-card}

:::block-card{item="minecraft:furnace"}
А тут описание механизма. Карточка большая, поэтому ставим её редко.
:::

# 3D-сцена {#scene}

Вот пример МЭ-сети. Наведите на маркеры, чтобы увидеть подсказки.

:::scheme{src="pages/ru_ru/primer/subsection_1/scenes/ae2_example.scene.json" caption="Пример МЭ-сети"}
<text key="power">
Тут может быть любой источник энергии
</text>
<text key="storage">
Место для хранения ячеек
</text>
:::

# Карточка моба {#mob-card}

:::mob-card{entity="terra.ghost"}
А вот тут можно сделать описание моба.
:::

# Рецепт {#recipe}

:::recipe{item="minecraft:chest" type="crafting" caption="Крафт сундука"}
:::

# Таблицы {#tables}

| Предмет                                | Что делает  |
| :------------------------------------- | :---------- |
| <item id="minecraft:chest" />          | Хранит вещи |
| <item id="minecraft:furnace" />        | Плавит руду |
| <item id="minecraft:crafting_table" /> | Крафтит     |

## Таблица с настройкой столбцов {#table-widths}

:::table{widths="auto 1fr"}
| Предмет | Описание |
|:---|:---|
| <item id="minecraft:hopper" /> | Тут длинное описание, оно само переносится.<br>А тут перенос строки в ячейке. |
:::
