---
id: "primer:gelio-1"
title: "Гелиосферный зарядный центр"
feedback: true
icon:
  item: "lolienergistics:heliospheric_charging_center"
---

В данной статье речь пойдёт о создании микрозвезд.

# Основная информация {#info_boiler}

**Гелиосферный зарядный центр** - это мультиструктура, которая требуется для превращения ядер микрозвезд в полноценные микрозвезды. Всего есть 4 ядра мирковзведы:

- <item id="lolienergistics:astrolion_core" />
- <item id="lolienergistics:sun_core" />
- <item id="lolienergistics:sirius_core" />
- <item id="lolienergistics:zodius_core" />

# Постройка {#building_boiler}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/gelios1.scene.json" caption="Пример мультиблочной структуры"}
<text key="energy">
Тут может быть любой источник EU энергии
</text>
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>
:::

Необходимые ресурсы:

- <item id="lolienergistics:heliospheric_charging_center"/>
- <item id="lolienergistics:tungsten_plating" count="67"/>
- <item id="lolienergistics:heliospheric_stabilizer" count="48"/>
- <item id="lolienergistics:niobium_coil" count="8"/>
- <item id="lolienergistics:thermal_induction_module1" count="4"/>

:::callout{type="tip"}
Данную структуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Разогрев звёзд {#razogrev-zvezd}

Для превращения ядра в звезду требуется:

- Зарядить звезду EU энергией
- Насытить топливом
- Нагреть до указанной температуры

В качестве топлива для ядер микрозвёзд используется <item id="lolienergistics:star_matter" />.

Для разогрева ядра миркозвезды требуется один из четырёх плазмореактивов:

- <item id="lolienergistics:fluid.phase_plasmoreactive" />
- <item id="lolienergistics:fluid.heliotropic_plasmoreactive" />
- <item id="lolienergistics:fluid.luminescent_plasmoreactive" />
- <item id="lolienergistics:fluid.exothermic_plasmoreactive" />
- <item id="lolienergistics:fluid.quark_plasmoreactive" />

:::callout{type="tip"}
Для максимального разогрева актуальной звезды, требуются максимальные доступные улучшения и лучший из доступных плазмореактивов.
:::

# Улучшения {#upgrade_boiler}

**Гелиосферный зарядный центр** поддерживает два вида улучшений:
:::item-card{item="lolienergistics:thermal_insulator1"}
Даёт бонус к максимальной температуре. Имеет три уровня. Эффект от нескольких улучшений сумируется.
:::

:::item-card{item="lolienergistics:thermal_induction_module1"}
Увеличивает температуру плазмореактива. Имеет 4 уровня. Встраивается напрямую в мультиструктуру. Эффект от нескольких улучшений сумируется.
:::
