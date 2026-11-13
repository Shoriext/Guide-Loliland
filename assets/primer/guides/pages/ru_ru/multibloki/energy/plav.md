---
id: "primer:plav-1"
title: "Термоядерный плавильный комплекс"
feedback: true
icon:
  item: "lolienergistics:thermonuclear_smelting_complex"
---

В данной статье речь пойдёт о ток, как использовать Термоядерный плавильный комплекс.

# Основная информация {#osnovnaya-informaciya}

**Термоядерный плавильный комплекс** – это мультиструктура, которая позволяет мощь звёзд, для плавления некоторых материалов.

Всего существует 4 вида звёзд с различной темереатурой поверхности.

| Звезда                                             | Температурный диапазон |
| :------------------------------------------------- | :--------------------- |
| <item id="lolienergistics:astrolion_micro_star" /> | 1120-4000              |
| <item id="lolienergistics:sun_micro_star" />       | 6000-12 000            |
| <item id="lolienergistics:sirius_micro_star" />    | 20 000-30 000          |
| <item id="lolienergistics:zodius_micro_star" />    | 33 400-50 000          |

При работе звезда начинает терять температуру и энергию.
:::callout{type="warning"}
Если звезда потеряет энергию и остныет слишком сильно, она погаснет.
:::

# Постройка {#building_boiler}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/plav.scene.json" caption="Пример мультиблочной структуры"}
<text key="inv">
Тут может быть любой МЭ интерфейс
</text>

<text key="eng">
Тут может быть любой источник EU энергии
</text>
:::

Необходимые ресурсы:

- <item id="lolienergistics:thermonuclear_smelting_complex" count="1"/>
- <item id="lolienergistics:resistant_tank" count="4"/>
- <item id="lolienergistics:heat_resistant_glass" count="80"/>
- <item id="lolienergistics:tungsten_plating" count="50"/>

:::callout{type="tip"}
Данную структуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Улучшения {#uluchshenie}

**Термоядерный плавильный комплекс** поддержживает несколько улучшений:

:::item-card{item="lolienergistics:portable_charging_module"}
Убирает потери энергии звезды.
:::

:::item-card{item="lolienergistics:thermal_insulator1"}
Уменьшает скорость потери температуры звезды. Улучшение третьего уровня устраняет потери температуры.
:::

:::item-card{item="lolienergistics:upgrade_singular_buck"}
Увеличивает объём внутреннего резервуара.
:::
