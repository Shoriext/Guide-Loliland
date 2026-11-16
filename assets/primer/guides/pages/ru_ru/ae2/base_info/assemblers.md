---
id: "primer:assemblers"
title: "Сборщики"
feedback: true
icon:
  item: "appliedenergistics2:tile.BlockMolecularAssembler"
  meta: 0
---

В данной статье речь пойдет о сборщиках и их функциях.

# Сборщики {#assemblers-info}

**Сборщик** – это основной функциональный блок, используемый для автоматизации создания чего-либо. Существует довольно много видов сборщиков, каждый из них позволяет автоматизировать различные процессы. 

Каждый из сборщиков требует шаблоны с рецептами для работы. Каждый шаблон может быть закодирован на <item id="appliedenergistics2:item.ItemMultiPart" meta="340">терминале интерфейсов</item> или на соответствующем кодировшике:
- <item id="loli_technologies:tile.BlockInfusionEncoding" />
- <item id="loli_technologies:tile.BlockBloodAltarEncoding" />
- <item id="loli_technologies:tile.BlockBloodAlchemyEncoding" />
- <item id="loli_technologies:tile.BlockNeutroniumEncoding" />
- <item id="loli_technologies:tile.BlockAssemblyTableEncoding" />
- <item id="loli_technologies:tile.BlockFusionEncoding" />

# Базовые сборщики {#assemlers-base}

**Сборщики**, позволяющие автоматизировать крафты на верстаке. Для работы требуют рядом любой <item id="appliedenergistics2:tile.BlockInterface" /> с шаблонами для работы.

Поддерживают улучшенулучшения: 
- <item id="appliedenergistics2:item.ItemMultiMaterial" meta="30" count="4" />
- <item id="loli_technologies:item.ItemQuantumAccelerationCard" count="1" />.

:::item-card{item="appliedenergistics2:tile.BlockMolecularAssembler"}
– Начальный сборщик, заменяет <item id="minecraft:crafting_table" />.
:::

:::item-card{item="loli_technologies:tile.BlockAdvancedAssembler"}
– Улучшенная версия обычного сборщика. Работает мгновенно, не нуждается в улучшениях.
:::

:::item-card{item="loli_technologies:tile.BlockLargeAssemblerX9"}
– Заменяет <item id="Avaritia:Dire_Crafting" />. В качестве шаблонов используется <item id="loli_technologies:item.ItemLargePattern" />. Работает мгновенно, не нуждается в улучшениях.
:::

# Магические сборщики {#assemblers-magic}

**Сборщики**, позволяющие автоматизировать создание предметов **Древней Магии**. 

Для работы требуют вис-аспекты или эссенцию. В качестве шаблонов используется <item id="appliedenergistics2:item.ItemKnowledgeCore" /> или <item id="loli_technologies:item.ItemInfusionCell" />. Шаблоны помещаются внутрь сборщиков. <---- **СЮДА НУЖНО ДОБАВИТЬ ССЫЛКУ НА РАЗДЕЛ С УЗЛАМИ и эссенцией**

Поддерживают улучшения: 
- <item id="appliedenergistics2:item.ItemMultiMaterial" meta="30"/>
- <item id="loli_technologies:item.ItemQuantumAccelerationCard" />
- <item id="loli_technologies:item.ItemSealAzanor" />.

:::item-card{item="appliedenergistics2:tile.BlockArcaneAssembler"}
– Начальный сборщик, заменяющий <item id="Thaumcraft:blockTable" meta="15" />. Может создавать предметы с затратами вис до 150.
:::

:::item-card{item="loli_technologies:tile.BlockArcaneImprovedAssembler"}
– Продвинутая версия предыдущего. Может создавать предметы с любыми затратами вис.
:::

:::item-card{item="loli_technologies:tile.BlockInfusionAssembler"}
– Заменяет <item id="Thaumcraft:blockStoneDevice" meta="2">Руническую матрицу</item>. 
:::

# Кровавый сборщик {#assemblers-blood}

**Сборщик**, позволяющий автоматизировать **Магию крови**.

Для работы требуется <item id="AWWayofTime:lifeEssence" />. В качестве шаблона используется <item id="loli_technologies:item.ItemBloodCell" />. Шаблоны помещаются внутрь сборщика. 

Поддерживает уникальное улучшение  – <item id="loli_technologies:item.ItemSealArmok" />

:::item-card{item="loli_technologies:tile.BlockBloodAssembler"}
– Заменяет <item id="AWWayofTime:Altar" /> максимального уровня и <item id="lolimagically:extra_writing_table">Улучшенную ахимическую и химическую установку</item>. Работает мгновенно, не нуждается в улучшениях скорости.
:::

# Нейтронный сборщик {#assemblers-neutron}

**Сборщик**, который значительно ускоряет процесс создания сингулярностей. 

В качестве шаблонов выступает <item id="loli_technologies:item.ItemNeutroniumCell" />. Шаблоны помещаются внутрь сборщика.

:::item-card{item="loli_technologies:tile.BlockNeutroniumAssembler"}
– Заменяет <item id="Avaritia:Neutronium_Compressor" />. Работает мгновенно, не нуждается в улучшениях.
:::

# Лазерный сборщик {#assemblers-laser}

**Сборщик**, позволяющий автоматизировать и **значительно** ускорить рецепты, создаваемые с помощью лазеров.

Для работы требует **большое** количество EU энергии. В качестве шаблонов используется <item id="loli_technologies:item.ItemAssemblyTableCell" />. Шаблоны помещаются внутрь сборщика.

Поддерживает улучшения:
- <item id="appliedenergistics2:item.ItemMultiMaterial" meta="30"/>
- <item id="loli_technologies:item.ItemQuantumAccelerationCard" />
- <item id="lolienergistics:upgrade_quantum_generator" />.

:::item-card{item="loli_technologies:tile.BlockAssemblyTableAssembler"} 
– Заменяет <item id="lolienergistics:assembly_table" />. При использовании <item id="lolienergistics:upgrade_quantum_generator" display="icon" /> работает мгновенно и не нуждается в улучшениях скорости.
:::

# Внеземной сборщик {#assemblers-dragon}

**Сборщик**, позволяющий автоматизировать и **значительно** ускорить **Дракониевое слияние**.

Для работы требует **большое** количество EU энергии. В качестве шаблонов используется <item id="loli_technologies:item.ItemFusionCell" />. Шаблоны помещаются внутрь сборщика.

Поддерживает улучшения:
- <item id="appliedenergistics2:item.ItemMultiMaterial" meta="30"/>
- <item id="loli_technologies:item.ItemQuantumAccelerationCard" />
- <item id="lolienergistics:upgrade_quantum_generator" />.


:::item-card{item="loli_technologies:tile.BlockFusionAssembler"}
– Заменяет <item id="loli_dragon_might:fusion_crafting_core" /> и <item id="loli_dragon_might:fusion_injector" meta="4" count="10" />. При использовании <item id="lolienergistics:upgrade_quantum_generator" display="icon" /> работает мгновенно и не нуждается в улучшениях скорости.
:::
