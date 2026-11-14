---
id: "primer:use-matter"
title: "Использование жидкой материи"
feedback: true
icon:
  item: "IC2:blockMachine2"
  meta: 5
---

Жидкая материя нужна для копирования предметов. На этой странице описан **легендарный репликатор** – мультиструктура для массового копирования.

# Основная информация {#use-matter-info}

Легендарный репликатор – промышленная версия механизма <item id="lolienergistics:BlockQuantumReplicator" />. Для работы ему нужны энергия и <item id="IC2:fluidUuMatter" />.

Отличия от обычного механизма:

- Создаёт до 9 стаков выбранных предметов за раз
- Материя расходуется в два раза медленнее

# Постройка {#use-matter-building}

Мультиструктуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/replicator.scene.json" caption="Легендарный репликатор"}
<text key="import">
Тут может быть подача материи
</text>

<text key="energy">
Тут может быть любой источник энергии
</text>

<text key="export">
Тут может быть любой МЭ интерфейс
</text>
:::

# Улучшения {#use-matter-upgrades}

:::item-card{item="lolienergistics:upgrade_quantum_generator"}
Снабжает репликатор энергией
:::

:::item-card{item="lolienergistics:upgrade_singular_buck"}
Увеличивает объём внутреннего резервуара
:::

:::item-card{item="lolienergistics:upgrade_module"}
Ускоряет работу репликатора. \
Эффект нескольких улучшений суммируется
:::
