---
id: "primer:freezer-1"
title: "Кристаллизационный охлаждающий комплекс"
feedback: true
icon:
  item: "lolienergistics:crystallization_cooling_complex"
---

В данной статье речь пойдёт о преобразовании жидкостей в предметы.

# Основная информация {#info_freezer}

**Кристаллизационный охлаждающий комплекс** - это мультиструктура, с помощью которой можно менять агрегатное состояние различных жидкостей.

# Постройка {#building_freezer}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/ohlad1.scene.json" caption="Пример мультиблочной структуры"}
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>

<text key="energy">
Тут может быть любой источник EU энергии
</text>
:::

Ресурсы нужные для постройки:

- <item id="lolienergistics:crystallization_cooling_complex" count="1"/>
- <item id="lolienergistics:resistant_tank" count="4"/>
- <item id="lolienergistics:cryogenic_glass" count="32"/>
- <item id="lolienergistics:tungsten_plating" count="26"/>

:::callout{type="tip"}
Данную структуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Улучшения {#upgrade_freezer}

Кристаллизующий охлаждающий комплекс поддерживает несколько улучшений:

:::item-card{item="lolienergistics:upgrade_module"}
Ускоряет работу механизма.
:::

:::item-card{item="lolienergistics:upgrade_singular_buck"}
Увеличивает размер внутринних резервуаров под жидкость и газ.
:::
