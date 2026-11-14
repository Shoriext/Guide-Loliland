---
id: "primer:ind-base-steel-1"
title: "Получение стали"
feedback: true
icon:
  item: "uniresources:ingotSteel"
---

В данной статье речь пойдёт о том, как получить <item id="uniresources:ingotSteel" /> и <item id="uniresources:blockSteel" />, и какие мультиструктуры для этого понадобятся.

# Основная информация {#info-steel}

**Сталь** – один из основных материалов, который понадобится для создания множества механизмов и мультиструктур. Её нельзя получить простой переплавкой железа – для производства придётся построить цепочку из нескольких мультиструктур:

1. **Коксовая печь** – производит <item id="lolienergistics:coke_coal" />, который служит топливом.
2. **Доменная печь** – нагревает <item id="uniresources:ingotIron" /> до состояния <item id="lolienergistics:hot_iron_ingot" />.
3. **Закалочная ванна** – закаляет <item id="lolienergistics:hot_iron_ingot" /> и превращает его в <item id="uniresources:ingotSteel" />.

| Этап   | Мультиструктура  | Сырьё                                                                                      | Результат                                                                                  |
| :----- | :--------------- | :----------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------- |
| Первый | Коксовая печь    | Уголь                                                                                      | <item id="lolienergistics:coke_coal" />                                                    |
| Второй | Доменная печь    | <item id="uniresources:ingotIron" />, <item id="uniresources:blockIron" />                 | <item id="lolienergistics:hot_iron_ingot" />, <item id="lolienergistics:hot_iron_block" /> |
| Третий | Закалочная ванна | <item id="lolienergistics:hot_iron_ingot" />, <item id="lolienergistics:hot_iron_block" /> | <item id="uniresources:ingotSteel" />, <item id="uniresources:blockSteel" />               |

:::callout{type="tip"}
Все мультиструктуры из этой статьи можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Этап 1. Коксовая печь {#steel-step-1}

Первым делом нужно добыть топливо для доменной печи. Для этого используется **коксовая печь** – мультиструктура, которая позволяет получать <item id="lolienergistics:coke_coal" /> и производит <item id="lolienergistics:fluid.creosote" /> в качестве побочного продукта.

:::callout{type="tip"}
Коксовая печь **не поддерживает** улучшения.
:::

## Постройка {#building-steel-cocs}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/cocs_pech.scene.json" caption="Коксовая печь"}
<text key="import" header="Поставка">
Поставлять топливо можно с любой стороны
</text>

<text key="export" header="Выгрузка">
Забирать результат переработки можно с любой стороны
</text>
:::

Необходимые ресурсы:

- <item id="lolienergistics:coke_oven_brick" count="27" />

# Этап 2. Доменная печь {#steel-step-2}

Следующий этап – нагрев железа. **Доменная печь** – это мультиструктура, с помощью которой можно создавать <item id="lolienergistics:hot_iron_ingot" /> и <item id="lolienergistics:hot_iron_block"/>, используя <item id="uniresources:ingotIron" /> и <item id="uniresources:blockIron" /> соответственно.

На сервере доменная печь представлена в двух вариантах:

- **Обычная доменная печь** – работает на твёрдом топливе, подходит для начала игры.
- **Промышленная доменная печь** – работает на жидкостях и энергии EU, подходит для массового производства.

## Обычная доменная печь {#steel-blast-1}

Для работы обычная доменная печь требует топливо. Им может являться:

- <item id="lolienergistics:coke_coal"/>
- <item id="lolienergistics:coal_coke_block"/>
- <item id="uniresources:charcoal" />

:::callout{type="tip"}
<item id="lolienergistics:coke_coal" />, полученный в коксовой печи, можно сразу отправлять в доменную печь в качестве топлива.
:::

:::callout{type="tip"}
За один цикл работы доменная печь производит по 1 виду продукции и не поддерживает улучшения.
:::

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/steal-1.scene.json" caption="Обычная доменная печь"}
<text key="import" header="Поставка">
Поставлять железо можно с любой стороны
</text>

<text key="export" header="Выгрузка">
Забирать результат можно с любой стороны
</text>
:::

Необходимые ресурсы:

- <item id="lolienergistics:blast_furnace_brick" count="27"/>

## Промышленная доменная печь {#steel-blast-2}

**Промышленная доменная печь**, в отличие от обычной, в качестве топлива требует два вида жидкости – нагревающую и охлаждающую, а также энергию EU. Доступные жидкости и их уровни можно посмотреть, наведя курсор на баки в интерфейсе структуры.

:::callout{type="warning"}
Если уровень охлаждающей жидкости ниже уровня нагревающей, то печь не будет работать.
:::

:::callout{type="tip"}
За один цикл работы промышленная доменная печь перерабатывает все ресурсы из своего буфера. При использовании комбинации жидкостей третьего уровня, печь работает мгновенно.
:::

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/steal-2.scene.json" caption="Промышленная доменная печь"}
<text key="energy">
Тут может быть любой источник EU энергии
</text>
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>
:::

Необходимые ресурсы:

- <item id="lolienergistics:industrial_blast_furnace" count="1"/>
- <item id="lolienergistics:blast_furnace_brick" count="29"/>
- <item id="lolienergistics:niobium_plating" count="12"/>
- <item id="lolienergistics:niobium_tank" count="8"/>
- <item id="lolienergistics:niobium_coil" count="5"/>

:::callout{type="tip"}
Промышленная доменная печь поддерживает все индустриальные улучшения, но не нуждается в них. **Скорость ее работы зависит только от уровня жидкостей**.
:::

# Этап 3. Закалочная ванна {#steel-step-3}

Последний этап – закалка раскалённого железа. **Закалочная ванна** – это промышленная версия функционального блока <item id="lolienergistics:cauldron"/>, которая используется для производства <item id="uniresources:ingotSteel"/> и <item id="uniresources:blockSteel"/>, используя <item id="lolienergistics:hot_iron_ingot" /> и <item id="lolienergistics:hot_iron_block" /> соответственно.

Для работы закалочная ванна требует одну из трёх охлаждающих жидкостей и энергию EU. Скорость работы ванны зависит от уровня жидкости. Доступные варианты можно посмотреть, наведя курсор на бак в интерфейсе механизма.

:::callout{type="tip"}
За один цикл работы закалочная ванна перерабатывает все ресурсы из своего буфера. При использовании жидкости третьего уровня, ванна работает мгновенно.
:::

## Постройка {#building-steel-zakal}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/zakal-1.scene.json" caption="Закалочная ванна"}
<text key="energy">
Тут может быть любой источник EU энергии
</text>
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>
:::

Необходимые ресурсы:

- <item id="lolienergistics:hardening_bath" count="1" />
- <item id="lolienergistics:niobium_tank" count="1" />
- <item id="lolienergistics:quantum_glass" count="8" />
- <item id="lolienergistics:niobium_plating" count="8" />

# Итог {#steel-summary}

Полная цепочка производства стали выглядит так:

1. Загрузите уголь в **коксовую печь** и получите <item id="lolienergistics:coke_coal" />.
2. Загрузите <item id="lolienergistics:coke_coal" /> и <item id="uniresources:ingotIron" /> в **доменную печь** и получите <item id="lolienergistics:hot_iron_ingot" />.
3. Загрузите <item id="lolienergistics:hot_iron_ingot" /> в **закалочную ванну** и получите <item id="uniresources:ingotSteel" />.

:::callout{type="tip"}
Для ускорения производства используйте блоки: <item id="uniresources:blockIron" /> превращается в <item id="lolienergistics:hot_iron_block" />, а затем в <item id="uniresources:blockSteel" />.
:::

:::callout{type="tip"}
Соедините промышленную доменную печь и закалочную ванну через МЭ-сеть, чтобы раскалённое железо сразу отправлялось на закалку, – так вся цепочка будет работать автоматически.
:::
