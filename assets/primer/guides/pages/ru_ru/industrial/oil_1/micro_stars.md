---
id: "primer:ind-base-micro-stars-1"
title: "Микрозвёзды"
feedback: true
icon:
  item: "lolienergistics:sun_micro_star"
---

Микрозвёзды нужны для плавки некоторых материалов. На этой странице описано, как создать микрозвезду и как её использовать.

# Основная информация {#micro-star-info}

Работа с микрозвёздами состоит из двух шагов:

1. **Гелиосферный зарядный центр** – превращает ядро в микрозвезду.
2. **Термоядерный плавильный комплекс** – нагревает материалы жаром микрозвезды.

:::callout{type="tip"}
Обе мультиструктуры можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Ядра микрозвёзд {#micro-star-cores}

Каждая микрозвезда создаётся из своего ядра:

| Ядро                                         | Микрозвезда                                        |
| :------------------------------------------- | :------------------------------------------------- |
| <item id="lolienergistics:astrolion_core" /> | <item id="lolienergistics:astrolion_micro_star" /> |
| <item id="lolienergistics:sun_core" />       | <item id="lolienergistics:sun_micro_star" />       |
| <item id="lolienergistics:sirius_core" />    | <item id="lolienergistics:sirius_micro_star" />    |
| <item id="lolienergistics:zodius_core" />    | <item id="lolienergistics:zodius_micro_star" />    |

# Создание микрозвезды {#micro-star-creation}

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

:::scheme{src="pages/ru_ru/industrial/industrial_base/scenes/gelios1.scene.json" caption="Гелиосферный зарядный центр"}
<text key="energy">
Тут может быть любой источник энергии
</text>
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>
:::

:::callout{type="tip"}
Для максимального нагрева используйте лучший доступный плазмореактив и улучшения высшего уровня.
:::

## Улучшения зарядного центра {#micro-star-charging-upgrades}

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

# Использование микрозвезды {#micro-star-usage}

Готовую микрозвезду поместите в **термоядерный плавильный комплекс**. Комплекс нагревает материалы её жаром.\
У каждой микрозвезды свой диапазон температуры:

| Микрозвезда                                        | Температура     |
| :------------------------------------------------- | :-------------- |
| <item id="lolienergistics:astrolion_micro_star" /> | 1120 - 4000     |
| <item id="lolienergistics:sun_micro_star" />       | 6000 - 12 000   |
| <item id="lolienergistics:sirius_micro_star" />    | 20 000 - 30 000 |
| <item id="lolienergistics:zodius_micro_star" />    | 33 400 - 50 000 |

Во время работы микрозвезда постепенно теряет температуру и энергию.

:::callout{type="warning"}
Если микрозвезда потеряет энергию и слишком остынет, она погаснет.
:::

:::scheme{src="pages/ru_ru/industrial/industrial_base/scenes/plav.scene.json" caption="Термоядерный плавильный комплекс"}
<text key="inv">
Тут может быть любой МЭ интерфейс
</text>

<text key="eng">
Тут может быть любой источник энергии
</text>
:::

## Улучшения плавильного комплекса {#micro-star-smelting-upgrades}

Улучшения комплекса помогают дольше сохранять микрозвезду активной.

:::item-card{item="lolienergistics:portable_charging_module"}
Убирает потерю энергии микрозвезды
:::

:::item-card{item="lolienergistics:thermal_insulator1"}
Замедляет остывание микрозвезды. \
На третьем уровне остывание прекращается
:::

:::item-card{item="lolienergistics:upgrade_singular_buck"}
Увеличивает объём внутреннего резервуара
:::
