---
id: "primer:first-steel"
title: "Первая сталь"
feedback: true
icon:
  item: "uniresources:ingotSteel"
  meta: 0
---

Сталь нужна для создания многих механизмов и мультиструктур. На этой странице описан самый простой способ её получить.

# Основная информация {#first-steel-info}

Простой переплавкой железа сталь не получить. Для первой стали понадобятся:

1. **Коксовая печь** – производит топливо. Результат: <item id="lolienergistics:coke_coal" />.
2. **Доменная печь** – нагревает железо. Результат: <item id="lolienergistics:hot_iron_ingot" />.
3. <item id="lolienergistics:cauldron" /> – охлаждает нагретое железо. Результат: <item id="uniresources:ingotSteel" />.

:::callout{type="tip"}
Обе мультиструктуры с этой страницы можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Получение кокса {#first-steel-coke}

Сначала наладьте производство топлива для доменной печи. Для этого постройте **коксовую печь**.

- Сырьё: <item id="minecraft:coal" />
- Продукт: <item id="lolienergistics:coke_coal" />
- Побочный продукт: <item id="lolienergistics:fluid.creosote" />

Улучшения коксовая печь не поддерживает.

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/cocs_pech.scene.json" caption="Коксовая печь"}
<text key="import" header="Поставка">
Поставлять топливо можно с любой стороны
</text>

<text key="export" header="Выгрузка">
Забирать результат переработки можно с любой стороны
</text>
:::

# Нагрев железа {#first-steel-blast-furnace}

Следующий шаг – нагрев железа в **доменной печи**.

| Сырьё                                | Результат                                    |
| :----------------------------------- | :------------------------------------------- |
| <item id="uniresources:ingotIron" /> | <item id="lolienergistics:hot_iron_ingot" /> |
| <item id="uniresources:blockIron" /> | <item id="lolienergistics:hot_iron_block" /> |

Подходящее топливо:

- <item id="lolienergistics:coke_coal" />
- <item id="lolienergistics:coal_coke_block" />
- <item id="uniresources:charcoal" />

Топливо из коксовой печи можно сразу отправлять в доменную.\
За один цикл печь выдаёт один вид продукции. Улучшения не поддерживаются.

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/steal-1.scene.json" caption="Доменная печь"}
<text key="import" header="Поставка">
Поставлять железо можно с любой стороны
</text>

<text key="export" header="Выгрузка">
Забирать результат можно с любой стороны
</text>
:::

# Закалка железа {#first-steel-cauldron}

Последний шаг – охлаждение нагретого железа. На раннем этапе для этого подойдёт функциональный блок <item id="lolienergistics:cauldron" />.

- Сырьё: <item id="lolienergistics:hot_iron_ingot" />
- Результат: <item id="uniresources:ingotSteel" />

Когда стали понадобится больше, переходите на промышленное производство. Оно описано на странице «Сталь в промышленных масштабах».
