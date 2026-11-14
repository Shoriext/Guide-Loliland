---
id: "primer:energon_sintez-1"
title: "Синтезатор энергона"
feedback: true
icon:
  item: "lolienergistics:energon_synthesizer_core"
---

В данной статье речь пойдёт о использовании жидкого энергония.

# Основная информация {#info_energon_sintez}

**Энергонный синтезатор** – это мультиструктура, которая использует <item id="appliedenergistics2:item.ItemFluidHolder" nbt='{F:"red_energonium"}' /> и <item id="appliedenergistics2:item.ItemFluidHolder" nbt='{F:"dark_energonium"}' />, а также EU для создания различных предметов.

# Постройка {#building_energon_sintez}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/energon_sintez-1.scene.json" caption="Пример мультиблочной структуры"}
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>

<text key="energy">
Тут может быть любой источник EU энергии
</text>
:::

Необходимые ресурсы:

- <item id="lolienergistics:energon_synthesizer_core" />
- <item id="lolienergistics:quantum_glass" count="48" />
- <item id="lolienergistics:energon_plating" count="52" />

:::callout{type="tip"}
Данную структуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Улучшения {#upgrade_energon_sintez}

:::callout{type="tip"}
Данный механизм поддерживает все индустриальные улучшения.
:::
