---
id: "primer:mixer-1"
title: "Смеситель"
feedback: true
icon:
  item: "lolienergistics:mixer_core"
---

Если вы хотите создать новые жидкости, но не знаете, как это сделать, данная статья точно для вас.

# Основная информация {#info_smesitel}

Промышленный смеситель - это одна из важнейших многоблочных структур, которые существуют. С его помощью вы сможете соединять несколько жидкостей, смешивать их и получать новые уникальные жидкости.

# Постройка {#building_smesitel}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/mixer1.scene.json" caption="Пример мультиблочной структуры"}
<text key="Inter">
Тут может быть любой мэ интерфейс
</text>

<text key="energy">
Тут может быть любой источник энергии
</text>
:::

Ресурсы нужные для постройки:

- <item id="lolienergistics:mixer_core" count="1"/>
- <item id="lolienergistics:niobium_tank" count="2"/>
- <item id="lolienergistics:quantum_glass" count="24"/>
- <item id="lolienergistics:niobium_plating" count="18"/>

:::callout{type="tip"}
Данную структуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Улучшения {#upgrade_smesitel}

Промышленный смеситель поддерживает только одно улучшение, а именно <item id="lolienergistics:upgrade_singular_buck" />.

:::item-card{item="lolienergistics:upgrade_singular_buck"}
Увеличивает размер внутринних резервуаров под жидкость и газ.
:::
