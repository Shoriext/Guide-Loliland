---
id: "primer:steal-1"
title: "Доменные печи"
feedback: true
icon:
  item: "lolienergistics:industrial_blast_furnace"
---

# Основная информация {#osnovnaya-informaciya}

**Доменная печь** – это мультиблочная структура, с помощью которой можно создавать <item id="lolienergistics:hot_iron_ingot" /> и <item id="lolienergistics:hot_iron_block"/>, используя <item id="uniresources:ingotIron" /> и <item id="uniresources:blockIron" /> соответственно.

На сервере доменная печь представлена двумя мультиблочными структурами:

  - **Обычная доменная печь**
  - **Промышленная доменная печь**



# Доменная печь {#info_steal_1}

Для работы данная структура требует топливо. Им может являться:
  - <item id="lolienergistics:coke_coal"/>
  - <item id="lolienergistics:coal_coke_block"/>
  - <item id="uniresources:charcoal" />.

:::callout{type="tip"}
За один цикл работы доменная печь производит по 1 виду продукции и не поддерживает улучшения.
:::

## Постройка {#building_steal_1}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/steal-1.scene.json" caption="Пример мультиблочной структуры"}
<text key="energy">
Шина импорта
</text>
<text key="Inter">
Шина экспорта
</text>
:::

Необходимые ресурсы:
  - <item id="lolienergistics:blast_furnace_brick" count="27"/>

:::callout{type="tip"}
Данную структуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::



# Промышленная доменная печь {#info_steal_2}

Промышленная печь, в отличие от обычной, в качестве топлива требует два вида жидкости – нагревающую и охлаждающую, а также EU. Доступные жидкости и их уровни можно посмотреть, наведя курсор на баки в интерфейсе структуры.

:::callout{type="warning"}
Если уровень охлаждающей жидкости ниже уровня нагревающей, то печь не будет работать.
:::

:::callout{type="tip"}
За один цикл работы промышленная доменная печь перерабатывает все ресурсы из своего буфера. При использовании комбинации жидкостей третьего уровня, печь работает мгновенно.
:::

## Постройка {#building_steal_2}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/steal-2.scene.json" caption="Пример мультиблочной структуры"}
<text key="energy">
Тут может быть любой источник энергии
</text>
<text key="Inter">
Тут может быть любой мэ интерфейс
</text>
:::

Необходимые ресурсы:
- <item id="lolienergistics:industrial_blast_furnace" count="1"/>
- <item id="lolienergistics:blast_furnace_brick" count="29"/>
- <item id="lolienergistics:niobium_plating" count="12"/>
- <item id="lolienergistics:niobium_tank" count="8"/>
- <item id="lolienergistics:niobium_coil" count="5"/>

:::callout{type="tip"}
Данную структуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

## Улучшения {#upgrade_steal_2}

:::callout{type="tip"}
Промышленная доменная печь поддерживает все индустриальные улучшения, но не нуждается в них. **Скорость ее работы зависит только от уровня жидкостей**. 
:::