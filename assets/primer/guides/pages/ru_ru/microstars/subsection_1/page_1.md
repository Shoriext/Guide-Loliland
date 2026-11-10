---
id: "primer:page-1"
title: "Микрозвезды"
feedback: true
icon:
  item: "lolienergistics:sun_core"
---
<item id="lolienergistics:astrolion_micro_star">Микрозвезды</item> – это обязательный компонент работы <item id="lolienergistics:thermonuclear_smelting_complex">плавильного комплекса</item>. Каждая звезда имеет свой <tooltip content="температуру поверхности">нагрев</tooltip>, от которого будет зависеть возможность переплавки ресурсов в <item id="lolienergistics:thermonuclear_smelting_complex" display="text">плавильном комплексе</item>


# Основы зарядки {#charge-basics icon-item="lolienergistics:upgrade_quantum_generator"}

Для преобразования <item id="lolienergistics:astrolion_core">ядер</item> в <item id="lolienergistics:astrolion_micro_star" nbt='{temperature:1.0E7f,energy:1000000000L}'>микрозвезды</item> и их последующего нагрева используется <item id="lolienergistics:heliospheric_charging_center">гелиосферный зарядный центр</item>
:::callout{type="tip"}
Для его постройки используйте <item id="loli_utility:structure_builder"/>
:::


<item id="lolienergistics:heliospheric_charging_center">Гелиосферный зарядный центр</item> потребляет 3 вида ресурсов:

- **Энергия**
- <item id="lolienergistics:star_matter"/>
- <item id="lolienergistics:fluid.phase_plasmoreactive">Плазмореактив</item>


А также имеет **2 слота** под <item id="lolienergistics:thermal_insulator1">улучшения термоизоляции</item>




## Преобразование ядер {#microstar-create}

:::item-card{item="lolienergistics:sun_core"}
У каждого ядра различные требования к **нагреву** и **энергии** для преобразования в микрозвезду
:::
**Максимальная** температура в <item id="lolienergistics:heliospheric_charging_center" display="text">гелиосферном зарядном центре</item> определяется тремя составляющими:

- **Типом** <item id="lolienergistics:fluid.phase_plasmoreactive">плазмореактива</item>
- **Количеством** и **уровенем** <item id="lolienergistics:thermal_insulator1">улучшений термоизоляции</item>
- **Уровенем** <item id="lolienergistics:thermal_induction_module1">тепловых индукционных модулей</item>


# Постепенная зарядка {#charge-steps icon-item="lolienergistics:portable_charging_module"}


## Астролион {#astrolion}
:::callout{type="tip"}
Наведите на звезду, чтобы узнать её **температуру**.
:::

| Этап нагрева | Следующий шаг |
|:---|:---|
| <item id="lolienergistics:astrolion_micro_star" nbt='{temperature:2.8E6f,energy:1000000000L}'/> | Создание <item id="lolienergistics:fluid.heliotropic_plasmoreactive">гелиотропного плазмореактива</item> |
| <item id="lolienergistics:astrolion_micro_star" nbt='{temperature:5.6E6f,energy:1000000000L}'/> | Создание <item id="lolienergistics:thermal_induction_module2" count="4">индукционных модулей 2го уровня</item> |
| <item id="lolienergistics:astrolion_micro_star" nbt='{temperature:7.2E6f,energy:1000000000L}'/> | Создание <item id="lolienergistics:fluid.luminescent_plasmoreactive">люминофазного плазмореактива</item> |
| <item id="lolienergistics:astrolion_micro_star" nbt='{temperature:1E7f,energy:1000000000L}'/> | Создание <item id="lolienergistics:thermal_insulator1" count="2">термоизоляторов 1го уровня</item> и <item id="lolienergistics:sun_core">ядра солнце</item> |


## Солнце {#sun}

| Этап нагрева | Следующий шаг |
|:---|:---|
| <item id="lolienergistics:sun_micro_star" nbt='{temperature:2.16E7f,energy:100000000000L}'/> | Создание <item id="lolienergistics:thermal_induction_module3" count="4">индукционных модулей 3го уровня</item> и <item id="lolienergistics:fluid.exothermic_plasmoreactive">экзотермического плазмореактива</item> |
| <item id="lolienergistics:sun_micro_star" nbt='{temperature:3E7f,energy:100000000000L}'/> | Создание <item id="lolienergistics:thermal_insulator2" count="2">термоизоляторов 2го уровня</item> и <item id="lolienergistics:sirius_core">ядра сириус</item> |

## Сириус {#sirius}

| Этап нагрева | Следующий шаг |
|:---|:---|
| <item id="lolienergistics:sirius_micro_star" nbt='{temperature:4.224E7f,energy:50000000000000L}'/> | Создание <item id="lolienergistics:fluid.quark_plasmoreactive">кваркового плазмореактива</item> |
| <item id="lolienergistics:sirius_micro_star" nbt='{temperature:6E7f,energy:50000000000000L}'/> | Создание <item id="lolienergistics:thermal_insulator2" count="2">термоизоляторов 3го уровня</item> и <item id="lolienergistics:thermal_induction_module4" count="4">индукционных модулей 4го уровня</item> |

## Зодиус {#zodius}
:::item-card{item="lolienergistics:zodius_micro_star" nbt='{temperature:1.2E8f,energy:1000000000000000L}'}
После создания последнего уровня <item id="lolienergistics:thermal_insulator2">модулей термоизоляции</item> и  <item id="lolienergistics:thermal_induction_module4" count="4">тепловых индукционных модулей</item>. Зарядите <item id="lolienergistics:zodius_core"/> до максимальных **50 000°C** температуры поверхности
:::