---
id: "primer:mixer"
title: "Работа со смесителем"
feedback: true
icon:
  item: "lolienergistics:mixer_core"
  meta: 0
---

Многие жидкости нельзя получить напрямую, их нужно смешать из других. Для этого используется **промышленный смеситель**.

# Основная информация {#mixer-info}

Промышленный смеситель – мультиструктура, которая создаёт новые жидкости из комбинации других. Для работы ему нужна энергия.

# Постройка {#mixer-building}

Мультиструктуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/mixer1.scene.json" caption="Промышленный смеситель"}
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>

<text key="energy">
Тут может быть любой источник энергии
</text>
:::

# Улучшения {#mixer-upgrades}

Смеситель поддерживает только одно улучшение.

:::item-card{item="lolienergistics:upgrade_singular_buck"}
Увеличивает объём внутренних резервуаров
:::
