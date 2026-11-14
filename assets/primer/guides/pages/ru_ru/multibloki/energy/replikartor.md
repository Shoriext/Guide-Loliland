---
id: "primer:replikartor-1"
title: "Легендарный репликатор"
feedback: true
icon:
  item: "lolienergistics:legendary_replicator_core"
---

В данной статье речь пойдёт о Легендарном репликаторе.

# Основная информация {#info_replikartor}

**Легендарный репликатор** – это мультиструктура, которая является промышленной версией механизма <item id="lolienergistics:BlockQuantumReplicator" /> и обладает парой отличительных особенностей:

- Генерирует до 9 стаков указыных предметов за раз
- <item id="IC2:fluidUuMatter" /> тратится в два раза медленне

# Постройка {#building_replikartor}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/replicator.scene.json" caption="Легендарный репликатор"}
<text key="import">
Тут может быть подача материи
</text>

<text key="energy">
Тут может быть любой источник EU энергии
</text>

<text key="export">
Тут может быть любой МЭ интерфейс
</text>
:::

Необходимые ресурсы:

- <item id="lolienergistics:legendary_replicator_core" count="1" />
- <item id="lolienergistics:quantum_glass" count="8" />
- <item id="lolienergistics:niobium_plating" count="18" />

:::callout{type="tip"}
Данную структуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Улучшения {#upgrade_replikartor}

**Легендарный репликатор** поддерживает 3 вида улучшений:

:::item-card{item="lolienergistics:upgrade_quantum_generator"}
Обеспечивает механизм EU энергией.
:::

:::item-card{item="lolienergistics:upgrade_singular_buck"}
Увеличивает объём внутреннего резервуара.
:::

:::item-card{item="lolienergistics:upgrade_module"}
Ускоряет работу механизма. Эффект от нескольких улучшений складывается.
:::
