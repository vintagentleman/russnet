---
layout: page
title: Источники и методы
permalink: /sources/
---

## Методика построения RussNet

Разработка структуры RussNet идет по лексико-семантическим группам. Из частотного словаря С. А. Шарова отбираются лексемы, подходящие для выбранной группы. В корпусе современных текстов для этих лексем определяется полная совокупность контекстов, мощность которой (M) будет использована в дальнейшем для вычисления индекса ipm. Менеджер корпуса позволяет построить выборочные совокупности контекстов; стандартный объем такой совокупности равен 100. Контексты размечаются по статьям из МАС как схемам дифференциации значений и их оттенков. Если в контекстах встречаются отсутствующие в МАС значения, они добавляются к схеме.

Доли контекстов (_D<sub>i</sub>_), представляющих компоненты схемы, в размеченной совокупности используются для частотной упорядоченности значений; при этом нумерация и набор значений может как частично совпадать, так и полностью не совпадать с исходной статьей МАС. Для каждого значения вычисляется его экстраполированная частота в ipm: _f<sub>ipm</sub> = D<sub>i</sub> × M ÷ 21_. Из этого набора значений отбираются те, которые явным образом через дефиницию значения соотносятся с заданной семантической областью. При разметке контекстов по значениям дополнительно фиксируются контекстные маркеры, подтверждающие «принятие решения» исследователем. Эти контекстные маркеры обобщаются и записываются в виде рамок валентностей; эти структуры будут описаны в следующем разделе. Там же будет показано, как контекстная информация влияет на структурирование значений.

## Источники информации

В качестве источников в методике WordNet-словарей предусмотрено использование корпуса текстов. В нашем проекте корпус текстов относится к источникам первого порядка, т. е. непосредственным текстовым данным, не прошедшим специальной лексикографической обработки. На момент начала работ у нас не было возможности использовать общенациональные корпусы текстов, поэтому мы создали собственный корпус современных текстов и задали в нем принципы отбора текстов и его баланс следующим образом. Мы отбирали тексты из источников начиная с 1985 г., предполагая, что распад CCCР неизбежно отразился на статистическом распределении лексем, особенно в письменных источниках. Это не значит, что в отобранных текстах совершенно не представлена лексика советского периода, поскольку в статьях могли цитироваться фрагменты текстов предыдущих периодов. Основная часть текстов (около 60 %) — статьи из журналов, газет, интернет-источников на разные темы, чтобы обеспечить тематическое разнообразие текстов корпуса. Помимо этой части в корпус входит небольшая часть литературно-художественных текстов (15 %), научно-технических текстов (15 %), текстов законов как представителей деловых текстов (10 %). Общий объем корпуса составляет примерно 21 млн словоупотреблений.

Корпус текстов используется в методике RussNet для вычисления частотности значений полисемантичного слова и, следовательно, нумерации значений в тезаурусе в соответствии с этой частотой. В WordNet-проектах подобная оценка получается за счет размеченных по значению корпусов текстов, однако составление такого корпуса необходимого объема (несколько миллионов словоупотреблений) — нереальная задача в нашем случае отсутствия материальных ресурсов. Более подробно методику разметки значений по частотности мы опишем ниже.

Еще одним источником первого порядка является Русский ассоциативный словарь (в 2 т. / Ю. Н. Караулов, Г. А. Черкасова, Н. В. Уфимцева, Ю. А. Сорокин, Е. Ф. Тарасов. Т. I. От стимула к реакции: Ок. 7000 стимулов. М.: АСТ-Астрель, 2002. 784 с. Т. II. От реакции к стимулу: Более 100 000 реакций. М.: АСТ-Астрель, 2002. 992 с.), который представлен в электронном виде на [сайте РАС](http://tesaurus.ru/dict/dict.php). Несмотря на очевидную обработку данных (проведение экспериментов «стимул — реакция», отбор новых стимулов), данные представлены лишь с указанием частоты реакции на стимул; в этом смысле они подтверждают данные корпусных исследований, показывая, что некоторые связи присутствуют в лексической организации современного молодого человека.

Незначительное количество научных и деловых текстов, с нашей точки зрения, обеспечивает нетерминологический характер лексики в RussNet. Первоначально мы считали, что некоторые слова, которые используются терминологически, могут получать «терминологические расширения», однако первые эксперименты с подобными расширениями показали, что последние имеют иную систему организации, что закономерно, поскольку терминологические системы отражают научную картину мира, а RussNet ориентирован на наивную (языковую) картину мира.

Источники второго порядка — это лингвистические словари, которые имеют собственные цели и методику подготовки, а также построены на собственных текстовых данных. Однако как средство первоначальной схемы дифференциации значений они необходимы. В ходе работ оказалось, что МАС (Словарь русского языка: В 4-х тт. / АН СССР, Ин-т рус. яз.; под ред. А. П. Евгеньевой. 2-е изд., испр. и доп. М.: Русский язык, 1981–1984.) подходит для нашей методики, поскольку в словаре существенное внимание уделяется синтаксическим характеристикам употребления слова.

Также используются синонимические и идеографические словари: Словарь синонимов русского языка / под ред. А. П. Евгеньевой. Л.: Наука, 1970; Новый объяснительный словарь синонимов. 2-е изд., испр. и доп. / под рук. Ю. Д. Апресяна. М.: Школа «Языки славянской культуры», 2003 (НОСС); Толковый словарь русских глаголов. Идеографическое описание. Английские эквиваленты. Синонимы. Антонимы / под ред. Л. Г. Бабенко. М.: Аст-Пресс, 1999 (ТСРГ).

Частотные словари необходимы для отбора частотной лексики. Для частотного словаря весьма важен объем обработанных текстов, их баланс и периодизация. В силу этих факторов был выбран Частотный словарь С. А. Шарова ([2-я версия частотного списка](http://www.artint.ru/projects/frqlist.php)). Эта версия удобна тем, что предлагает 5000 наиболее частотных лемм основных частей речи.