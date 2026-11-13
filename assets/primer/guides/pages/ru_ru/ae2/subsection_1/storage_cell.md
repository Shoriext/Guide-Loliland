---
id: "primer:storage-cell"
title: "Ячейки"
feedback: true
icon:
  item: "appliedenergistics2:item.ItemBasicStorageCell.1k"
  meta: 0
---

В данной статье вы сможете ознакомится про механнику ячеек.

# Что такое ячейка {#chto-takoe-yacheyka}

Ячейка это что то похожее на флеш карту или жёский диск компьютера, она даёт МЭ-системе возможность храннить рессурсы. У ячеек есть три параметра:

- Вид ячейки
- Кол-во типов
- Кол-во байтов

# Что такое байты {#chto-takoe-bayty}

Байт - в случае с ячейками это единица измерения вместимости: количества предметов, которое ячейка может хранить. Что бы не волноваться о байтах есть <item id="loli_technologies:item.ItemStorageCell" meta="2" />, но типы у неё всё рано будут огранничены.

:::callout{type="tip"}
Если закончаться байты, то ячейка переснает принимать предметы
:::

# Что такое тип {#chto-takoe-tip}

Тип — это количество уникальных предметов, хранящихся в ячейке. У каждой ячейки есть своё ограниченное количество типов. Как для байтов несуществует бесконечного решения, так что отслеживайте сколько типов остаётся в МЭ-системе.

:::callout{type="tip"}
Если закончаться типы, то ячейка переснает принимать новые уникальные предметы
:::

# Какие виды ячеек существуют {#kakie-vidy-yacheek-suschestvuyut}

Для каждого вида предмета нужна ячейка определенного вида. К сожалению нет особенной ячеки, которя может хранить всё разом. Всего их существует 4 вида:

- Предметная, например <item id="appliedenergistics2:item.ItemBasicStorageCell.1k" />
- Жидкостная, например <item id="appliedenergistics2:item.ItemBasicStorageCell.fluid1k" />
- Газовая, например <item id="appliedenergistics2:item.ItemBasicStorageCell.gas1k" />
- Эссенций, например <item id="appliedenergistics2:item.ItemBasicStorageCell.aspect1k" />

# Творческая МЭ ячейка хранения эссенций {#item icon-item="appliedenergistics2:item.ItemCreativeStorageCell.aspect"}

<item id="appliedenergistics2:item.ItemCreativeStorageCell.aspect" display="text" /> унникальная ячейка, для получения бесконечного колличества аспектов в МЭ-системе. Что бы в ней появитлись аспекты требуется разметить ячейку используя <item id="appliedenergistics2:tile.BlockCellWorkbench" />, размечается она при помощи<item id="Thaumcraft:ItemWispEssence" />

# Разметка ячеек {#razmetka-yacheek}

Любую ячейку можно разметить на <item id="appliedenergistics2:tile.BlockCellWorkbench" />, это даёт возможность ячейке хранить только определённый список предметов, которые будут указаны при разметке на <item id="appliedenergistics2:tile.BlockCellWorkbench" />.
