---
id: "primer:mixer-1"
title: "Промышленный смеситель"
feedback: true
icon:
  item: "lolienergistics:mixer_core"
---

В данной статье речь пойдёт о том, как смешивать различные жидкости.

# Основная информация {#info_smesitel}

**Промышленный смеситель** – это мультистуктура, которая позволяет создавать различные жидкости из комбинации других.

# Постройка {#building_smesitel}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/mixer1.scene.json" caption="Пример мультиблочной структуры"}
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>

<text key="energy">
Тут может быть любой источник EU энергии
</text>
:::

Необходимые ресурсы:

- <item id="lolienergistics:mixer_core" count="1"/>
- <item id="lolienergistics:niobium_tank" count="2"/>
- <item id="lolienergistics:quantum_glass" count="24"/>
- <item id="lolienergistics:niobium_plating" count="18"/>

:::callout{type="tip"}
Данную структуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Улучшения {#upgrade_smesitel}

**Промышленный смеситель** поддерживает только один вид улучшений.
:::item-card{item="lolienergistics:upgrade_singular_buck"}
Увеличивает объём внутренних резервуаров.
:::
