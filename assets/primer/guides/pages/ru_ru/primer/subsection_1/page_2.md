---
id: "primer:page-2"
title: "Страница 2"
feedback: true
icon:
  item: "minecraft:chest"
---

Это вводный абзац. На этой странице предметы, клавиши, подсказки и плашки.

# Предметы {#items icon-item="minecraft:chest"}

Вот предмет: <item id="minecraft:chest" />. Наведите на него, и покажется рецепт.

Можно указать количество: <item id="minecraft:chest" count="4" />.\
Можно показать только иконку: <item id="minecraft:chest" display="icon" />\
А это мини-пинг: <item id="minecraft:chest" display="text" />. Видно только название, но на него всё ещё можно нажать.\
Можно написать свой текст вместо названия: <item id="minecraft:chest">Сундучок</item>.\
А это предмет с вариантом (meta): <item id="minecraft:anvil" meta="2" />.

# Клавиши {#hotkeys}

Нажмите <hotkey bind="key.use" /> по сундуку, чтобы открыть его.\
Комбинация клавиш: <hotkey bind="key.use" modifiers="shift" />.\
Клавиша без настройки в игре: <hotkey bind="Esc" />.

# Подсказки {#tooltips}

Наведите на <tooltip content="А вот тут пишем пояснение.\nМожно в две строки.">это слово</tooltip>, и появится пояснение.

# Плашки {#callouts}

:::callout{type="tip"}
Это совет. Сюда пишем что-то полезное.
:::

Тут обычный текст, чтобы плашки не шли подряд.

:::callout{type="warning"}
Это предупреждение. Сюда пишем, где можно ошибиться.
:::

А ниже плашка со ссылкой на дополнительную страницу.

:::callout{type="pinned"}
<item id="minecraft:book" display="icon" /> [Дополнительная страница](guide:primer:page-4)
:::
