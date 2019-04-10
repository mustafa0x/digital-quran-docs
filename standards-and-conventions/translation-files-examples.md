---
description: >-
  Here are examples of translation files to give a better understanding of the
  structure
---

# Translation files: examples

Here you can find examples of [by-ayah translation](translation-files-examples.md#by-ayah-translation-example) and [word-by-word translation](translation-files-examples.md#word-by-word-translation-example) of both JSON and XML formats.

{% hint style="warning" %}
**NOTE.** Information in examples is not reliable! Please, do not treat it as real information. Mostly it is made up to just give you an idea of how values look like. 
{% endhint %}

## By-ayah translation example

{% tabs %}
{% tab title="JSON" %}
{% code-tabs %}
{% code-tabs-item title="By-ayah translation exmaple" %}
```javascript
{
    "translation": {
        "meta": {
            "name": {
                "ru": "Эльмир Кулиев",
                "en": "Elmir Kuliyev"
            },
            "language": {
                "name": "Russian",
                "iso1": "ru",
                "iso3": "rus",
                "direction": "ltr"
            },
            "authors": [
                {
                    "name": {
                        "ru": "Эльмир Кулиев",
                        "en": "Elmir Kuliev",
                    },
                    "bio": {
                        "ru": "Эльмир Кулиев — азербайджанский светский ученый-религиовед, автор перевода Священного Корана на русский язык, специалист в области мусульманского богословия, истории и культуры исламского региона. Автор книг «Пророчества о приближении конца света», «На пути к Корану», «Коран и глобализация», «Сладость веры», соавтор книг «Уроки благословенного месяца», «Исламоведение» (пособие для преподавателей), «Корановедение» (пособие для вузов). В последние годы Эльмир Кулиев занимается исследовательской и преподавательской деятельностью в своем родном городе, участвует в международных конференциях и выступает с лекциями в разных странах, ведет персональный сайт www.guliyev.org и страницу в социальной сети Facebook www.facebook.com/guliyev.org.",
                        "en": "Elmir Guliyev is an Azerbaijani secular religious scholar, author of the translation of the Holy Quran into Russian, an expert in Muslim theology, history and culture of the Islamic region. Author of the books “Prophecies about the end of the world”, “Towards the Qur'an”, “The Quran and Globalization”, “Sweetness of Faith”, co-author of the books “Lessons of the blessed month”, “Islamic studies” (teacher’s manual), “Koran studies” (manual for universities). In recent years, Elmir Guliyev is engaged in research and teaching activities in his hometown, participates in international conferences and lectures in different countries, maintains a personal website www.guliyev.org and a page on the social network Facebook www.facebook.com/guliyev.org."
                    },
                    "contacts": [
                        {
                            "type": "email",
                            "value": "kuliev@mail.ru"
                        },
                        {
                            "type": "website",
                            "value": "www.guliyev.org"
                        },
                        {
                            "type": "facebook",
                            "value": "www.facebook.com/guliyev"
                        }
                    ],
                    "isAlive": "true"
                }
            ],
            "riwaya": "Hafs",
            "copyrights": {
                "license": "Creative Commons Attribution 4.0 International License (http://creativecommons.org/licenses/by/4.0/)",
                "rightholder": "Elmir Kuliev"
            },
            "issueContacts": {
                "contact": [
                    {
                        "type": "email",
                        "value": "kuliev@mail.ru"
                    }
                ]
            },
            "firstGeneratedAt": "2019-04-05 06:01:53",
            "lastGeneratedAt": "2019-04-05 06:01:53",
            "textUpdatedAt": "2018-11-13 05:44:32"
        },
        "content": {
            "surahs": [
                {
                    "number": 1,
                    "name": "Открывающая Коран",
                    "nameTransliterated": "Аль-Фатиха",
                    "ayahs": [
                        {
                            "number": 1,
                            "text": "С именем Аллаха Милостивого, Милосердного!"
                        },
                        {
                            "number": 2,
                            "text": "(Вся) хвала – (лишь одному) Аллаху, Господу миров [Господу всех творений],"
                        }
                    ]
                }
            ]
        }
    }
}
```
{% endcode-tabs-item %}
{% endcode-tabs %}
{% endtab %}

{% tab title="XML" %}
```markup
<?xml version="1.0" encoding="utf-8"?>
<translation>
    <meta>
        <name>
            <ru>Эльмир Кулиев</ru>
            <en>Elmir Kuliyev</en>
        </name>
        <language>
            <name>Russian</name>
            <iso1>ru</iso1>
            <iso3>rus</iso3>
            <direction>ltr</direction>
        </language>
        <authors>
            <author>
                <name>
                    <ru>Эльмир Кулиев</ru>
                    <ru>Elmir Kuliev</ru>
                </name>
                <bio>
                    <ru>Эльмир Кулиев — азербайджанский светский ученый-религиовед, автор перевода Священного Корана на русский язык, специалист в области мусульманского богословия, истории и культуры исламского региона. Автор книг «Пророчества о приближении конца света», «На пути к Корану», «Коран и глобализация», «Сладость веры», соавтор книг «Уроки благословенного месяца», «Исламоведение» (пособие для преподавателей), «Корановедение» (пособие для вузов). В последние годы Эльмир Кулиев занимается исследовательской и преподавательской деятельностью в своем родном городе, участвует в международных конференциях и выступает с лекциями в разных странах, ведет персональный сайт www.guliyev.org и страницу в социальной сети Facebook www.facebook.com/guliyev.org.</ru>
                    <en>Elmir Guliyev is an Azerbaijani secular religious scholar, author of the translation of the Holy Quran into Russian, an expert in Muslim theology, history and culture of the Islamic region. Author of the books “Prophecies about the end of the world”, “Towards the Qur'an”, “The Quran and Globalization”, “Sweetness of Faith”, co-author of the books “Lessons of the blessed month”, “Islamic studies” (teacher’s manual), “Koran studies” (manual for universities). In recent years, Elmir Guliyev is engaged in research and teaching activities in his hometown, participates in international conferences and lectures in different countries, maintains a personal website www.guliyev.org and a page on the social network Facebook www.facebook.com/guliyev.org.</en>
                </bio>
                <contacts>
                    <contact>
                        <type>email</type>
                        <value>kuliev@mail.ru</value>
                    </contact>
                    <contact>
                        <type>website</type>
                        <value>www.guliyev.org</value>
                    </contact>
                    <contact>
                        <type>facebook</type>
                        <value>www.facebook.com/guliyev</value>
                    </contact>
                </contacts>
                <isAlive>true</isAlive>
            </author>
        </authors>
        <riwaya>Hafs</riwaya>
        <copyrights>
            <license>MIT</license>
            <rightholder>Elmir Kuliev</rightholder>
        </copyrights>
        <issueContacts>
            <contact>
                <contact>
                    <name>Elmir Kuliev</name>
                    <type>email</type>
                    <value>kuliev@mail.ru</value>
                </contact>
                <contact>
                    <name>Quran Academy support</name>
                    <type>email</type>
                    <value>support@quranacademy.org</value>
                </contact>
            </contact>
        </issueContacts>
        <firstGeneratedAt>2019-04-05 06:01:53</firstGeneratedAt>
        <lastGeneratedAt>2019-04-05 06:01:53</lastGeneratedAt>
        <textUpdatedAt>2018-11-13 05:44:32</textUpdatedAt>
    </meta>
    <content>
        <surahs>
            <surah number="1" ayahCount="7">
                <name>Открывающая Коран</name>
                <nameTransliterated>Аль-Фатиха</nameTransliterated>
                <ayahs>
                    <ayah number="1">Во имя Аллаха, Милостивого, Милосердного!</ayah>
                    <ayah number="2">Хвала Аллаху, Господу миров,</ayah>
                    <ayah number="3">Милостивому, Милосердному,</ayah>
                    <ayah number="4">Властелину Дня воздаяния!</ayah>
                    <ayah number="5">Тебе одному мы поклоняемся и Тебя одного молим о помощи.</ayah>
                    <ayah number="6">Веди нас прямым путем,</ayah>
                    <ayah number="7">путем тех, кого Ты облагодетельствовал, не тех, на кого пал гнев, и не заблудших.</ayah>
                </ayahs>
            </surah>
        </surahs>
    </content>
</translation>
```
{% endtab %}
{% endtabs %}



## Word-by-word translation example

TODO:


