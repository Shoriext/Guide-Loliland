---
id: "primer:star-charging"
title: "Зарядка звезд"
feedback: true
icon:
  item: "lolienergistics:sun_micro_star"
  meta: 0
---

Без микрозвезды термоядерный плавильный комплекс не работает. На этой странице описано, как превратить ядро в готовую микрозвезду.

# Ядра микрозвёзд {#star-charging-cores}

Каждая микрозвезда создаётся из своего ядра:

| Ядро                                         | Микрозвезда                                        |
| :------------------------------------------- | :------------------------------------------------- |
| <item id="lolienergistics:astrolion_core" /> | <item id="lolienergistics:astrolion_micro_star" /> |
| <item id="lolienergistics:sun_core" />       | <item id="lolienergistics:sun_micro_star" />       |
| <item id="lolienergistics:sirius_core" />    | <item id="lolienergistics:sirius_micro_star" />    |
| <item id="lolienergistics:zodius_core" />    | <item id="lolienergistics:zodius_micro_star" />    |

# Гелиосферный зарядный центр {#star-charging-center}

Ядро превращается в микрозвезду в **гелиосферном зарядном центре**. Для этого:

1. Зарядите ядро энергией.
2. Насытьте ядро топливом.
3. Нагрейте ядро до нужной температуры.

Топливо для ядер: <item id="lolienergistics:star_matter" />.\
Для нагрева понадобится один из плазмореактивов:

- <item id="lolienergistics:fluid.phase_plasmoreactive" />
- <item id="lolienergistics:fluid.heliotropic_plasmoreactive" />
- <item id="lolienergistics:fluid.luminescent_plasmoreactive" />
- <item id="lolienergistics:fluid.exothermic_plasmoreactive" />
- <item id="lolienergistics:fluid.quark_plasmoreactive" />

:::callout{type="tip"}
Для максимального нагрева используйте лучший доступный плазмореактив и улучшения высшего уровня.
:::

Мультиструктуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/gelios1.scene.json" caption="Гелиосферный зарядный центр"}
<text key="energy">
Тут может быть любой источник энергии
</text>
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>
:::

# Улучшения зарядного центра {#star-charging-upgrades}

:::item-card{item="lolienergistics:thermal_insulator1"}
Повышает максимальную температуру нагрева. \
Уровней: 3 \
Эффект нескольких улучшений суммируется
:::

:::item-card{item="lolienergistics:thermal_induction_module1"}
Повышает температуру плазмореактива. \
Уровней: 4 \
Встраивается прямо в мультиструктуру \
Эффект нескольких модулей суммируется
:::
