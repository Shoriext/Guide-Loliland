---
id: "primer:oil-rig-1"
title: "Нефтедобывающая вышка"
feedback: true
icon:
  item: "lolienergistics:oil_derrick_core_1"
---

В данной статье речь пойдёт о том, как добывается <item id="lolienergistics:fluid.crude_oil" />.

# Основная информация {#info_oil}

**Нефтедобывающая вышка** - это мультиструктура, с помощью которой добывается <item id="lolienergistics:fluid.crude_oil" />. Для её работы требуется EU энергия, а также [месторождения нефти](guide:primer:ind-base-oil-1).

:::callout{type="warning"}
Следите за количеством нефти в выбранных месторождениях, так как они не бесконечны.
:::

# Постройка {#building_oil}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/nefte1.scene.json" caption="Пример мультиблочной структуры"}
<text key="inv">
Тут может быть любой МЭ интерфейс
</text>

<text key="energy">
Тут может быть любой источник EU энергии
</text>
:::

Необходимые ресурсы:

- <item id="lolienergistics:oil_derrick_core_1" count="1"/>
- <item id="lolienergistics:tungsten_tank" count="12"/>
- <item id="lolienergistics:tungsten_plating" count="43"/>
- <item id="lolienergistics:niobium_plating" count="30"/>

:::callout{type="tip"}
Данную структуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Улучшение {#upgrade_oil}

Улучшаестся нефтянаная вышка внутри своего интерфейса.
Всего есть три ветки улучшений:

- Уровень вышки
- Скорость
- Эффективность

| Уровень вышки           | Макс месторождение  | Макс скорость | Макс эффективность |
| :---------------------- | :------------------ | :------------ | :----------------- |
| Уровень 1 (изначальный) | Месторождение альфа | 3             | 1                  |
| Уровень 2               | Месторождение бетта | 6             | 2                  |
| Уровень 3               | Месторождение гамма | 10            | 3                  |

:::callout{type="tip"}
Со второго уровня открывается возможность автоматической очереди для добычи.
:::
