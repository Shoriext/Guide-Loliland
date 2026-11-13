---
id: "primer:par-1"
title: "Промышленный паровой котёл"
feedback: true
icon:
  item: "lolienergistics:industrial_steam_boiler"
---

В данной статье речь пойдёт о том, как получать <item id="appliedenergistics2:item.ItemGasHolder" nbt='{G:"steam"}' /> в промышленных масштабах.

# Основная информация {#info_boiler}

**Промышленный паровой котёл** – это мультиструктура, которая является промышленной версией механизма <item id="lolienergistics:steam_boiler" /> и позволяет получать <item id="appliedenergistics2:item.ItemGasHolder" nbt='{G:"steam"}' />, а также <item id="lolidimensions:salt_crystal" /> в качестве побочного продукта, получаемого из накипи.
:::callout{type="warning"}
Если уровень накипи дойдёт до 100%, работа мультиструктуры остановится.
:::

# Постройка {#building_boiler}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/par1.scene.json" caption="Пример мультиблочной структуры"}
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>

<text key="energy">
Тут может быть любой источник EU энергии
</text>
:::

Необходимые ресурсы:

- <item id="lolienergistics:industrial_steam_boiler" count="1"/>
- <item id="lolienergistics:niobium_tank" count="2"/>
- <item id="lolienergistics:quantum_glass" count="9"/>
- <item id="lolienergistics:niobium_plating" count="33"/>

:::callout{type="tip"}
Данную структуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Улучшения {#upgrade_boiler}

**Промышленный паровой котёл** поддерживает несколько улучшений:
:::item-card{item="lolienergistics:upgrade_demineralizer"}
Автоматически собирает накипь, производя <item id="lolidimensions:salt_crystal" />.
:::
:::item-card{item="lolienergistics:upgrade_recycler"}
Автоматически уничтожает производимый <item id="lolidimensions:salt_crystal" />.
:::
:::item-card{item="lolienergistics:upgrade_singular_buck"}
Увеличивает размер внутринних резервуаров.
:::
:::item-card{item="lolienergistics:upgrade_resource_gen"}
Бесконечно генерирует воду в внутреннем резервуаре.
:::
