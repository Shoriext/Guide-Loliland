---
id: "primer:convertor-energon"
title: "Работа с энергоном"
feedback: true
icon:
  item: "lolienergistics:energon_converter_core"
  meta: 0
---

Энергон используется для создания различных предметов. На этой странице описано, как перевести его в жидкую форму и как применить.

# Основная информация {#convertor-energon-info}

Для работы с энергоном понадобятся две мультиструктуры:

1. **Энергонный преобразователь** – переводит энергон в жидкую форму.
2. **Энергонный синтезатор** – создаёт предметы из жидкого энергона.

:::callout{type="tip"}
Обе мультиструктуры можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Энергонный преобразователь {#convertor-energon-converter}

Преобразователь переводит твёрдый энергон в жидкий:

| Сырьё                                     | Результат                                                                         |
| :---------------------------------------- | :-------------------------------------------------------------------------------- |
| <item id="lolienergistics:red_energon" /> | <item id="appliedenergistics2:item.ItemFluidHolder" nbt='{F:"red_energonium"}' />  |
| <item id="lolienergistics:dark_energon" /> | <item id="appliedenergistics2:item.ItemFluidHolder" nbt='{F:"dark_energonium"}' /> |

Преобразование требует очень много энергии. Перед запуском убедитесь, что её запаса хватит.\
Преобразователь поддерживает все индустриальные улучшения.

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/energon_preob-1.scene.json" caption="Энергонный преобразователь"}
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>

<text key="energy">
Тут может быть любой источник энергии
</text>
:::

# Энергонный синтезатор {#convertor-energon-synthesizer}

Синтезатор создаёт различные предметы. Для работы ему нужны энергия и жидкий энергон:

- <item id="appliedenergistics2:item.ItemFluidHolder" nbt='{F:"red_energonium"}' />
- <item id="appliedenergistics2:item.ItemFluidHolder" nbt='{F:"dark_energonium"}' />

Синтезатор поддерживает все индустриальные улучшения.

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/energon_sintez-1.scene.json" caption="Энергонный синтезатор"}
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>

<text key="energy">
Тут может быть любой источник энергии
</text>
:::
