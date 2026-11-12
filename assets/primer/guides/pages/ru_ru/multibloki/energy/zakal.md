---
id: "primer:zakal-1"
title: "Закалочная ванна"
feedback: true
icon:
  item: "lolienergistics:hardening_bath"
---

# Основная информация {#info_zakal}

**Закалочная ванна** – это промышленная версия инструмента <item id="lolienergistics:cauldron"/>, которая используется для производства <item id="uniresources:ingotSteel"/> и <item id="uniresources:blockSteel"/>, используя <item id="lolienergistics:hot_iron_ingot" /> и <item id="lolienergistics:hot_iron_block" /> соответственно.

Для работы закалочная ванна требует одну из трех вариантов охлаждающих жидкостей и EU. Скорость работы ванны зависит от уровня жидкости. Доступные варианты можно посмотреть, наведя курсор на бак в интефейсе механизма.

:::callout{type="tip"}
За один цикл работы закалочная ванна перерабатывает все ресурсы из своего буфера. При использовании жидкости третьего уровня, ванна работает мгновенно.
:::
 
## Постройка {#building_zakal}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/zakal-1.scene.json" caption="Пример мультиблочной структуры"}
<text key="energy">
Тут может быть любой источник энергии
</text>
<text key="Inter">
Тут может быть любой мэ интерфейс
</text>
:::

Необходимые ресурсы:
- <item id="lolienergistics:hardening_bath" count="1" />
- <item id="lolienergistics:niobium_tank" count="1" />
- <item id="lolienergistics:quantum_glass" count="8" />
- <item id="lolienergistics:niobium_plating" count="8" />

:::callout{type="tip"}
Данную структуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

