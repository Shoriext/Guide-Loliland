---
id: "primer:energon_preob-1"
title: "Преобразователь энегона"
feedback: true
icon:
  item: "lolienergistics:energon_converter_core"
---

В данной статье речь пойдёт о преобразовании энергона.

# Основная информация {#info_energon_preob}

**Энергонный преобразователь** – это мультиструктура, которая преобразует энергон в жидкую форму:

- <item id="lolienergistics:red_energon" /> в <item id="appliedenergistics2:item.ItemFluidHolder" nbt='{F:"red_energonium"}' />
- <item id="lolienergistics:dark_energon" /> в <item id="appliedenergistics2:item.ItemFluidHolder" nbt='{F:"dark_energonium"}' />

:::callout{type="tip"}
Преобразование энергона – очень энергоемкий процесс. Перед запуском убедитесь, что располагаете необходимым количеством EU энергии.
:::

# Постройка {#building_energon_preob}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/energon_preob-1.scene.json" caption="Пример мультиблочной структуры"}
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>

<text key="energy">
Тут может быть любой источник EU энергии
</text>
:::

Необходимые ресурсы:

- <item id="lolienergistics:energon_converter_core" />
- <item id="lolienergistics:quantum_glass" count="8" />
- <item id="lolienergistics:energon_plating" count="18" />

# Улучшения {#upgrade_energon_preob}

:::callout{type="tip"}
Данный механизм поддерживает все индустриальные улучшения.
:::
