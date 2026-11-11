---
id: "primer:freezer-1"
title: "Охлаждающий комплекс"
feedback: true
icon:
  item: "lolienergistics:crystallization_cooling_complex"
---

Если вы случайно расплавили ресурс и не знаете, как его восстановить, эта статья точно для вас.

# Основная информация {#info_freezer}

Кристаллизующий охлаждающий комплекс позволяет изменять состояние предмета, превращая его из жидкого состояния обратно в твёрдое. Также он обладает уникальными крафтами.

# Постройка {#building_freezer}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/ohlad1.scene.json" caption="Пример мультиблочной структуры"}
<text key="Inter">
Тут может быть любой мэ интерфейс
</text>

<text key="energy">
Тут может быть любой источник энергии
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
