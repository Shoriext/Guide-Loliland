---
id: "primer:par-1"
title: "Промышленный паровой котёл"
feedback: true
icon:
  item: "lolienergistics:industrial_steam_boiler"
---

Промышленный паровой котёл - это мультиблочная структура, позволяющая получать пар в промышленных масштабах.

# Основная информация {#info_boiler}

Данная структура служит улучшенной версией механизма <item id="lolienergistics:steam_boiler" />, которая позволяет получать <item id="lolidimensions:salt_crystal" />, помимо большого количества пара. В данном механизме присутсвует механника накопления накипи. Для её сбороса есть кнопка в интерфейсе, а также специальные улучщения, про которые вы можете прочитать чуть ниже.

# Постройка {#building_boiler}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/par1.scene.json" caption="Пример МЭ-сети"}
<text key="Inter">
Тут может быть любой мэ интерфейс
</text>

<text key="energy">
Тут может быть любой источник энергии
</text>
:::

Промышленный паровой котёл строится при помощи строителя мультиструктур.

Ресурсы унжные для постройки:

- <item id="lolienergistics:industrial_steam_boiler" count="1"/>
- <item id="lolienergistics:niobium_tank" count="2"/>
- <item id="lolienergistics:quantum_glass" count="9"/>
- <item id="lolienergistics:niobium_plating" count="33"/>

# Улучшения {#upgrade_boiler}

<item id="lolienergistics:steam_boiler" /> поддерживает 4 вида улучшений
:::item-card{item="lolienergistics:upgrade_demineralizer"}
Автоматически собирает накипь, производя <item id="lolidimensions:salt_crystal" />.
:::
:::item-card{item="lolienergistics:upgrade_recycler"}
Автоматически сбрасывает накипь, уничтожая вторичную продукцию.
:::
:::item-card{item="lolienergistics:upgrade_singular_buck"}
Увеличивает размер внутринних резервуаров под жидкость и газ.
:::
:::item-card{item="lolienergistics:upgrade_resource_gen"}
Бесконечно генерирует воду в внутреннем резервуаре.
:::
