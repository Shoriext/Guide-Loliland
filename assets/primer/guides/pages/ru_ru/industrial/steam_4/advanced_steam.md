---
id: "primer:advanced-steam"
title: "Еще больше пара"
feedback: true
icon:
  item: "lolienergistics:industrial_steam_boiler"
  meta: 0
---

Когда одного котла уже не хватает, пар нужен в промышленных масштабах. На этой странице описан **промышленный паровой котёл**.

# Основная информация {#advanced-steam-info}

Промышленный паровой котёл – промышленная версия механизма <item id="lolienergistics:steam_boiler" />.

- Продукт: <item id="appliedenergistics2:item.ItemGasHolder" nbt='{G:"steam"}' />
- Побочный продукт: <item id="lolidimensions:salt_crystal" />

Во время работы в котле копится <tooltip content="Отложения, из которых получается побочный продукт">накипь</tooltip>. Из неё и получается побочный продукт.

:::callout{type="warning"}
Если уровень накипи дойдёт до 100%, котёл остановится.
:::

Мультиструктуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/par1.scene.json" caption="Промышленный паровой котёл"}
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>

<text key="energy">
Тут может быть любой источник энергии
</text>
:::

# Улучшения {#advanced-steam-upgrades}

Улучшения избавляют котёл от накипи и упрощают подачу воды.

:::item-card{item="lolienergistics:upgrade_demineralizer"}
Автоматически собирает накипь и превращает её в побочный продукт
:::

:::item-card{item="lolienergistics:upgrade_recycler"}
Автоматически уничтожает побочный продукт
:::

:::item-card{item="lolienergistics:upgrade_singular_buck"}
Увеличивает объём внутренних резервуаров
:::

:::item-card{item="lolienergistics:upgrade_resource_gen"}
Бесконечно наполняет внутренний резервуар водой
:::
