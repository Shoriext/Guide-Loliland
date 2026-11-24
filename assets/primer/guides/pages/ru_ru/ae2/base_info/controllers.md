---
id: "primer:controllers"
title: "Контроллер"
feedback: true
icon:
  item: "appliedenergistics2:tile.BlockController"
  meta: 0
---

В данной статье речь пойдет о контроллерах и их функциях.

# Контроллер {#controller-info}

**Контроллер** – это главный хаб любой МЭ-системы. Он отвечает за питание и объединение [каналов](guide:primer:info#canals). 

Каждый <item id="appliedenergistics2:tile.BlockController" /> поддерживает бесконечное количество каналов. Требует EU энергию.

МЭ-система может иметь только один <tooltip content="Два и более объединенных МЭ-контроллера, стоящих впритык">кластер</tooltip> контроллеров. Максимальный размер кластера составляет 10×10×10 блоков. 

:::scheme{src="pages/ru_ru/ae2/base_info/scenes/controller1.scene.json" caption="Максимальный куб контроллеров"}
:::

:::callout{type="tip"}
Контроллер не обязан иметь правильную форму. Если размер не превышает лимит, то в его рамках можно придать кластеру любую форму.
:::

:::scheme{src="pages/ru_ru/ae2/base_info/scenes/controller2.scene.json" caption="Максимальный куб контроллеров"}
:::

# Виды контроллеров {#controller-types}

<item id="appliedenergistics2:tile.BlockController" /> представлен несколькими видами:

- <item id="appliedenergistics2:tile.BlockController" />
- <item id="loli_technologies:tile.BlockGoldController" />
- <item id="loli_technologies:tile.BlockInfiniteController" />
- <item id="loli_technologies:tile.BlockDemonicController" />

Все они имеют одинаковые функции и откличаются только визуально.

# Энергетические ячейки {#ontroller-troubles}

Чем больше МЭ-система, тем больше EU энергии она потребляет. Если энергии не хватает, система может «моргать», отключаться или **полностью перестать работать**. 

**Энергетические ячейки** – это решение этой проблемы. Они представленными несколькиими видами:

:::item-card{item="appliedenergistics2:tile.BlockEnergyCell"}
– Базовая ячейка, хранит небольшое количество энергии.
:::

:::item-card{item="appliedenergistics2:tile.BlockDenseEnergyCell"}
– Улучшенная версия предыдущей ячейки, хранит весомое количество энергии. Как правило будет достаточно всего нескольких штук.
:::

:::item-card{item="appliedenergistics2:tile.BlockCreativeEnergyCell"}
– Уникальная ячейка, обладающая бесконечным запасом энергии.
:::

:::callout{type="warning"}
Следите за питанием контроллера. Если EU энергии не хватит, система отключится, и вы можете потерять доступ к ресурсам до тех пор, пока не восстановите энергоснабжение.
:::