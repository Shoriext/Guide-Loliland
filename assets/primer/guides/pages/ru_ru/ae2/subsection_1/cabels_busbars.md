---
id: "primer:cabels_busbars"
title: "Кабели и шины"
feedback: true
icon:
  item: "appliedenergistics2:item.ItemMultiPart"
  meta: 0
---

В этом разделе речь пойдет о кабелях, шинах и их функциях.

# Кабели {#cabel_info}

**МЭ кабели** – это вспомогательные компоненты МЭ-сети, которые используются для соединения МЭ механизмов в систему. Каждый из них подключает механизм и запитывает его. Кабели бывают нескольких типов и отличаются количеством проводимых [каналов](guide:primer:info#canals).

- <item id="appliedenergistics2:item.ItemMultiPart"/> - 16 каналов
- <item id="appliedenergistics2:item.ItemMultiPart" meta="20" /> – 16 каналов
- <item id="loli_technologies:item.ItemMultiPart" meta="20" /> – 64 канала
- <item id="loli_technologies:item.ItemMultiPart" meta="40" /> – 128 каналов
- <item id="loli_technologies:item.ItemMultiPart" meta="60" /> – 256 каналов

:::callout{type="tip"}
Кабели разного цвета не будут соединятся друг с другом. Чтобы их покрасить, используйте <item id="loli_utility:painting_table" /> или <item id="loli_utility:brush">кисточку</item>
:::

# Шины {#busbars_info}

**МЭ шины** – это компоненты МЭ-системы, которые используются для перемещения и сортировки предметов и не только. Шины бывают нескольких типов и отличаются по своему функционалу. В этом разделе будет представлены функции следующих механизмов:

- <item id="appliedenergistics2:item.ItemMultiPart" meta="260" />
- <item id="appliedenergistics2:item.ItemMultiPart" meta="240" />
- <item id="appliedenergistics2:item.ItemMultiPart" meta="220" />
- <item id="appliedenergistics2:item.ItemMultiPart" meta="320" />
- <item id="appliedenergistics2:item.ItemMultiPart" meta="300" />
- <item id="appliedenergistics2:item.ItemMultiPart" meta="100" />
- <item id="appliedenergistics2:item.ItemMultiPart" meta="80" />


# Логистика {#busbars_logistics}

За логистику отвечают 3 вида шин:

:::item-card{item="appliedenergistics2:item.ItemMultiPart" meta="260"}
– Поставляет указанные ресурсы в буфер. Поддерживает 18 слотов.
:::
:::item-card{item="appliedenergistics2:item.ItemMultiPart" meta="240"}
– Забирает выбранные ресурсы из буфера. Поддерживает 18 слотов. Если оставить интерфейс шины пустым, она будет забирать все предметы.
:::
:::block-card{item="appliedenergistics2:item.ItemMultiPart" meta="220"}
– Делает подключенный буфер частью МЭ-системы хранения. Мгновенно отправляет или забирает из него указанные ресурсы. Поддерживает 18 слотов. Если оставить интерфейс пустым, шина будет поддерживать любые предметы.
:::

# Взаимодействие с миром {#busbars_ploskost}

Плоскости – инструменты, которые позволяют МЭ-системе взаимодействовать с миром

:::item-card{item="appliedenergistics2:item.ItemMultiPart" meta="320"}
– Позволяет ставить блоки перед собой. Имеет 3 режима работы. Поддерживает 18 слотов.
:::
:::item-card{item="appliedenergistics2:item.ItemMultiPart" meta="300"}
– Позволяет ломать блоки перед собой, автоматически собирая их в систему. Не имеет интерфейса.
:::

# Дополнительные возможности {#busbars_features}

Шины переключения – вспомогательные инструменты, которые позволяют настаривать МЭ-систему с помощью сигнала красного камня.

:::item-card{item="appliedenergistics2:item.ItemMultiPart" meta="100"}
– Ставится между кабелями и разъединяет их при подаче сигнала красного камня. Не имеет интерфейса.
:::
:::item-card{item="appliedenergistics2:item.ItemMultiPart" meta="80"}
– Ставится между кабелями и соединяет их при подаче сигнала красного камня. Не имеет интерфейса.
:::


# Улучшения {#busbars_upgrades}

:::item-card{item="appliedenergistics2:item.ItemMultiMaterial" meta="27"}
– Увеличивает количество допустимых предметов в шины на 9. Поддерживается до пяти улучшений.
:::

:::item-card{item="appliedenergistics2:item.ItemMultiMaterial" meta="53"}
– Позволяет механизму создавать указанные предметы для подачи в буфер. Добавляет 2 режима создания.
:::

:::item-card{item="appliedenergistics2:item.ItemMultiMaterial" meta="26"}
– Добавляет шине режим работы от красного камня.
:::

:::item-card{item="appliedenergistics2:item.ItemMultiMaterial" meta="29"}
– Добавляет возможность игнорировать внутренние параметры предмета (NBT).
:::

:::item-card{item="appliedenergistics2:item.ItemMultiMaterial" meta="31"}
– При использовании меняет «белый список шины» на «черный».
:::

:::item-card{item="appliedenergistics2:item.ItemMultiMaterial" meta="30"}
– Ускоряет работу механизма. Поддерживается до четырех улучшений.
:::

:::item-card{item="loli_technologies:item.ItemQuantumAccelerationCard"}
– Улучшенная версия карты ускорения. Поддерживается одно улучшение
:::