---
id: "primer:page-1"
title: "Буровая установка"
feedback: true
icon:
  item: "lolienergistics:drill_bit"
  meta: 1 
---

Если вы дошли до этапа, когда нужны руды в больших количествах, данная статья точно для вас.

# Основная информация {#info_drill_bit}

Буровая установка - это мультиблочная структура, позволяющая получать руды в промышленных масштабах.

# Сборка {#build icon-item="lolienergistics:drill_bit"}

1. Поставьте <item id="lolienergistics:drill" /> .
2. Подключите энергию проводами.
3. Забирайте руду со стороны выходного шлюза.

# Перенос установки {#moving icon-item="lolienergistics:drill_bit"}

Установка хранит свои характеристики в буровой коронке. Поэтому при переносе забирайте её вместе с коронкой.

:::callout{type="warning"}
- Главное при переносе не потерять главный блок <item id="lolienergistics:drill_bit" />. Без неё уровень и улучшения придётся прокачивать и ставить заново.
- Ресурсы, потраченные на прокачку и улучшения, вернуть нельзя.
:::
# Установка 2 уровня {#scene-level-2 icon-item="lolienergistics:drill_bit"}

:::scheme{src="pages/ru_ru/primer/subsection_1/scenes/drill_2.scene.scene.json" caption="Буровая установка 2 уровня"}
<text key="energy" header="Энергия">
Сюда подключается энергия.
</text>
<text key="exporting" header="Выгрузка">
Отсюда установка выгружает добытые руды.
</text>
:::

# Истощение жилы {#vein-depletion icon-item="lolienergistics:oreglow_coating"}
Убрать истощение жилы можно двумя способами.

1. [Перенесите установку](guide:primer:page-1#moving). Менять место необязательно: достаточно забрать её и поставить обратно. Поставить обратно можно с помощью <item id="loli_utility:structure_builder" />.
2. Положите в установку улучшение <item id="lolienergistics:oreglow_coating">напыление из рудноцвета</item>. Подавайте ману в установку через <item id="Botania:spreader">распространитель маны</item> и выше или через <item id="lolimagically:asgard_upgrade">улучшение Асгард</item>.

# Уровни коронок {#levels icon-item="lolienergistics:drill_bit_upgrade_2"}

Коронок 5 уровней. Чем выше уровень, тем больше видов руд. Чтобы повысить уровень, откройте установку, перейдите в раздел улучшения и вложите улучшение с указанными ресурсами.

- <item id="lolienergistics:drill_bit_upgrade_2" /> для 2 уровня
- <item id="lolienergistics:drill_bit_upgrade_3" /> для 3 уровня
- <item id="lolienergistics:drill_bit_upgrade_4" /> для 4 уровня
- <item id="lolienergistics:drill_bit_upgrade_5" /> для 5 уровня

# Улучшения установки {#extra-upgrades icon-item="lolienergistics:oreglow_coating"}

В установку можно положить дополнительные улучшения:

- <item id="lolienergistics:oreglow_coating">Напыление из рудноцвета</item> убирает проблему с истощением жилы.
- <item id="lolimagically:asgard_upgrade">Улучшение Асгард</item> даёт бесконечную ману в буровую установку.
- <item id="lolienergistics:upgrade_quantum_generator">Улучшение «Квантовый генератор»</item> даёт бесконечную энергию в буровую установку.

Если вы используете <item id="lolienergistics:oreglow_coating" />, подавайте ману в установку через <item id="Botania:spreader">распространитель маны</item> и выше или же через <item id="lolimagically:asgard_upgrade">Улучшение Асгард</item>
