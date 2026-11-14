---
id: "primer:ways-melting"
title: "Способы плавления материалов"
feedback: true
icon:
  item: "lolienergistics:thermonuclear_smelting_complex"
  meta: 0
---

Некоторые материалы не плавятся в обычных печах. Для них нужен жар микрозвезды и **термоядерный плавильный комплекс**.

# Основная информация {#ways-melting-info}

Термоядерный плавильный комплекс – мультиструктура, которая нагревает материалы жаром микрозвезды. Без микрозвезды внутри комплекс не работает.\
Как получить микрозвезду, описано на странице «Зарядка звезд».

:::callout{type="tip"}
Мультиструктуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Микрозвёзды {#ways-melting-stars}

Всего есть 4 вида микрозвёзд. У каждой свой диапазон температуры:

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

# Постройка {#ways-melting-building}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/plav.scene.json" caption="Термоядерный плавильный комплекс"}
<text key="inv">
Тут может быть любой МЭ интерфейс
</text>

<text key="eng">
Тут может быть любой источник энергии
</text>
:::

# Улучшения {#ways-melting-upgrades}

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
