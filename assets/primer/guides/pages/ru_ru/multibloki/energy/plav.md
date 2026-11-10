---
id: "primer:plav-1"
title: "Плавильный комплекс"
feedback: true
icon:
  item: "lolienergistics:thermonuclear_smelting_complex"
---

Плавильный комплекс открывает вам возможность расплавить даже самые твёрдые материалы.

# Основная информация {#info_boiler}

Данная структура позволяет плавить различные материалы. Температура плавления зависит от вставленной карманной звезды. Всего существует четыре вида таких звёзд, и у каждой своя температура.

| Звезда                                             | Температурный диапазон |
| :------------------------------------------------- | :--------------------- |
| <item id="lolienergistics:astrolion_micro_star" /> | 1120-4000              |
| <item id="lolienergistics:sun_micro_star" />       | 6000-12000             |
| <item id="lolienergistics:sirius_micro_star" />    | 20000-30000            |
| <item id="lolienergistics:zodius_micro_star" />    | 33400-50000            |

При работе звезда начинает остывать и разряжаться. Если звезда остынет или сядет, она перестанет плавить предметы. Чтобы она могла работать автономно, предусмотрено два улучшения.
:::item-card{item="lolienergistics:portable_charging_module"}
Позволяет звезде заряжаться внутри плавильного комплекса.
:::
:::item-card{item="lolienergistics:thermal_insulator1"}
Позволяет звезде терять температуру медленнее. Существует три уровня улучшения, при этом полную потерю температуры устраняет только третий уровень.
:::
Также поддерживает <item id="lolienergistics:upgrade_singular_buck" />
:::item-card{item="lolienergistics:upgrade_singular_buck"}
Данное улучшение позволяет расширить внутренние резервуары. Всего существует три уровня улучшения.
:::

# Постройка {#building_boiler}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/plav.scene.json" caption="Пример мультиблочной структуры"}
<text key="inv">
Тут может быть любой мэ интерфейс
</text>

<text key="eng">
Тут может быть любой источник энергии
</text>
:::

Ресурсы нужные для постройки:

- <item id="lolienergistics:thermonuclear_smelting_complex" count="1"/>
- <item id="lolienergistics:resistant_tank" count="4"/>
- <item id="lolienergistics:heat_resistant_glass" count="80"/>
- <item id="lolienergistics:tungsten_plating" count="50"/>

:::callout{type="tip"}
Данную структуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::
