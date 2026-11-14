---
id: "primer:dril-1"
title: "Буровая установка"
feedback: true
icon:
  item: "lolienergistics:drill_bit"
  meta: 1
---

В данной статье речь пойдёт об автономной добыче руды.

# Основная информация {#info_drill_bit}

**Буровая установка** – это мультиструктура, позволяющая получать руды в промышленных масштабах.

Буровая установка имеет 5 уровней и улучшается внутри своего интерфейса.

# Сборка {#build }

1. Поставьте <item id="lolienergistics:drill" /> .
2. Подключите энергию проводами.
3. Забирайте руду со стороны выходного шлюза.

# Установка 2 уровня {#scene-level-2 }

:::scheme{src="pages/ru_ru/multibloki/energy/scenes/drill_2.scene.json" caption="Буровая установка 2 уровня"}
<text key="energy" header="Энергия">
Сюда подключается энергия
</text>
<text key="interface" header="Выгрузка">
Сюда установка выгружает добытые руды
</text>
:::

:::callout{type="tip"}
Данную структуру можно построить при помощи жезла <item id="loli_utility:structure_builder" />.
:::

# Истощение жилы {#vein-depletion }

Убрать истощение жилы можно двумя способами.

1. Перенесите установку. Менять место необязательно: достаточно забрать её и поставить обратно. Поставить обратно можно с помощью <item id="loli_utility:structure_builder" />.
2. Положите в установку улучшение <item id="lolienergistics:oreglow_coating">напыление из рудноцвета</item>. Подавайте ману в установку через <item id="Botania:spreader">распространитель маны</item> и выше или через <item id="lolimagically:asgard_upgrade">улучшение Асгард</item>.

:::callout{type="warning"}
При переносе все улучшения сохраняются в буровой коронке, так что не теряйте её.
:::

# Улучшения {#extra-upgrades }

**Буровая устоновка** поддерживает несколько улучшений:
:::item-card{item="lolienergistics:oreglow_coating"}
Востанавливает жилу за счёт маны.
:::

:::item-card{item="lolimagically:asgard_upgrade"}
Убирает затраты маны.
:::

:::item-card{item="lolienergistics:upgrade_quantum_generator"}
Обеспечивает механизм EU энергией.
:::
