---
id: "primer:ind-base-steel-1"
title: "Получение стали"
feedback: true
icon:
  item: "uniresources:ingotSteel"
---

Сталь нужна для создания многих механизмов и мультиструктур. На этой странице описана вся цепочка её производства и мультиструктуры, которые для этого понадобятся.

# Основная информация {#steel-info}

Простой переплавкой железа сталь не получить. Понадобятся три мультиструктуры:

1. **Коксовая печь** – производит топливо. Результат: <item id="lolienergistics:coke_coal" />.
2. **Доменная печь** – нагревает железо. Результат: <item id="lolienergistics:hot_iron_ingot" />.
3. **Закалочная ванна** – охлаждает нагретое железо. Результат: <item id="uniresources:ingotSteel" />.

:::callout{type="tip"}
Все мультиструктуры с этой страницы можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Получение кокса {#steel-coke}

Сначала наладьте производство топлива для доменной печи. Для этого постройте **коксовую печь**.

- Сырьё: <item id="minecraft:coal" />
- Продукт: <item id="lolienergistics:coke_coal" />
- Побочный продукт: <item id="lolienergistics:fluid.creosote" />

Улучшения коксовая печь не поддерживает.

:::scheme{src="pages/ru_ru/industrial/industrial_base/scenes/cocs_pech.scene.json" caption="Коксовая печь"}
<text key="import" header="Поставка">
Поставлять топливо можно с любой стороны
</text>

<text key="export" header="Выгрузка">
Забирать результат переработки можно с любой стороны
</text>
:::

# Нагрев железа {#steel-blast-furnace}

Следующий шаг – нагрев железа в **доменной печи**. На сервере есть два её варианта:

- **Обычная** – использует твёрдое топливо, подходит для начала игры
- **Промышленная** – потребляет жидкости и энергию, рассчитана на массовое производство

Переработка в обоих вариантах одинаковая:

- <item id="uniresources:ingotIron" /> > <item id="lolienergistics:hot_iron_ingot" />
- <item id="uniresources:blockIron" /> > <item id="lolienergistics:hot_iron_block" />

## Обычная доменная печь {#steel-blast-furnace-basic}

Подходящее топливо:

- <item id="lolienergistics:coke_coal" />
- <item id="lolienergistics:coal_coke_block" />
- <item id="uniresources:charcoal" />

Топливо из коксовой печи можно сразу отправлять в доменную.\
За один цикл печь выдаёт один вид продукции. Улучшения не поддерживаются.

:::scheme{src="pages/ru_ru/industrial/industrial_base/scenes/steal-1.scene.json" caption="Обычная доменная печь"}
<text key="import" header="Поставка">
Поставлять железо можно с любой стороны
</text>

<text key="export" header="Выгрузка">
Забирать результат можно с любой стороны
</text>
:::

## Промышленная доменная печь {#steel-blast-furnace-industrial}

Промышленной печи не нужно твёрдое топливо. Вместо него она потребляет энергию и две жидкости: нагревающую и охлаждающую.\
Чтобы увидеть подходящие жидкости и их уровни, наведите курсор на баки в интерфейсе мультиструктуры.

:::callout{type="warning"}
Если уровень охлаждающей жидкости ниже уровня нагревающей, печь не будет работать.
:::

За один цикл печь обрабатывает всё содержимое <tooltip content="Внутреннее хранилище мультиструктуры для сырья">буфера</tooltip>. С жидкостями третьего уровня процесс становится мгновенным.\
Индустриальные улучшения поддерживаются, но не нужны. **Скорость зависит только от уровня жидкостей**.

:::scheme{src="pages/ru_ru/industrial/industrial_base/scenes/steal-2.scene.json" caption="Промышленная доменная печь"}
<text key="energy">
Тут может быть любой источник энергии
</text>
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>
:::

# Закалка железа {#steel-hardening-bath}

Последний шаг – охлаждение нагретого железа в **закалочной ванне**. Это промышленная версия функционального блока <item id="lolienergistics:cauldron" />.

- <item id="lolienergistics:hot_iron_ingot" /> > <item id="uniresources:ingotSteel" />
- <item id="lolienergistics:hot_iron_block" /> > <item id="uniresources:blockSteel" />

Ванне нужны энергия и одна из трёх охлаждающих жидкостей. Их список виден при наведении курсора на бак в интерфейсе.\
Чем выше уровень жидкости, тем быстрее идёт процесс. За один цикл ванна обрабатывает весь буфер, а с жидкостью третьего уровня – мгновенно.

:::scheme{src="pages/ru_ru/industrial/industrial_base/scenes/zakal-1.scene.json" caption="Закалочная ванна"}
<text key="energy">
Тут может быть любой источник энергии
</text>
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>
:::

# Цепочка производства {#steel-chain}

1. Загрузите <item id="minecraft:coal" /> в коксовую печь.
2. Отправьте полученное топливо и <item id="uniresources:ingotIron" /> в доменную печь.
3. Переложите <item id="lolienergistics:hot_iron_ingot" /> в закалочную ванну и заберите сталь.

Чтобы ускорить производство, перерабатывайте сразу блоки: <item id="uniresources:blockIron" /> > <item id="lolienergistics:hot_iron_block" /> > <item id="uniresources:blockSteel" />.

:::callout{type="tip"}
Соедините промышленную доменную печь и закалочную ванну через МЭ-сеть. Нагретое железо будет сразу уходить на охлаждение, и цепочка заработает автоматически.
:::
