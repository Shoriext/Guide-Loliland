---
id: "primer:gemo-1"
title: "Гемотрансмутатор"
feedback: true
icon:
  item: "lolienergistics:hemontransmutator"
---

В данной статье речь пойдёт об альтернативном способе получения крови драконов.

# Основная информация {#info_gemo}

**Гемотрансмутатор** – мультиструктура, которая позволяет получать кровь драконов из их сердец.

Для работы гемотрансмутатора требуется <item id="lolienergistics:dust_primordial_chaos" /> и <item id="lolienergistics:fluid.hemolymph" />, а также EU энергия. Также в качестве побочной продукции мы получаем <item id="lolienergistics:petrified_heart" />.

:::callout{type="tip"}
Для готовой продукции необходима <item id="lolidimensions:empty_dragon_blood_vessel" />. Другим способом извечь ее не получится.
:::

# Постройка {#building_gemob}

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/gemo-1.scene.json" caption="Пример мультиблочной структуры"}
<text key="energy">
Тут может быть любой источник EU энергии
</text>
<text key="Inter">
Тут может быть любой МЭ интерфейс
</text>
:::

Необходимые реусрсы:

- <item id="lolienergistics:hemontransmutator" />
- <item id="lolienergistics:cryogenic_glass" count="6" />
- <item id="lolienergistics:resistant_tank" count="2" />
- <item id="lolienergistics:tungsten_plating" count="18" />

:::callout{type="tip"}
Данную структуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Улучшения {#upgrade_gemo}

**Гемотрансмутатор** поддерживает 3 вида улучшений:

:::item-card{item="lolienergistics:upgrade_cardiacamplifier"}
Увеличивает скорость работы, эффект нескольких улучшений складывается.
:::
:::item-card{item="lolienergistics:upgrade_recycler"}
Автоматически уничтожает побочную продукцию.
:::
:::item-card{item="lolienergistics:upgrade_quantum_generator"}
Обеспечивает механизм EU энергией.
:::
