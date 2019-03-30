### List All Surahs 

#### URL

```
GET /surahs
```

#### Parameters

None

#### Response

```json
{
    "data": [
        {
          "number": 1,
          "basmala": false,
          "revelation_place": "meccan",
          "ayah_count": 7,
          "name": {
            "arabic": "الفاتحة",
            "translation": "The Opening",
            "transliteration": "Al-Fatiha"
          }
        },
        {
          "number": 2,
          "basmala": true,
          "revelation_place": "medinan",
          "ayah_count": 286,
          "name": {
            "arabic": "البقرة",
            "translation": "The Cow",
            "transliteration": "Al-Baqara"
          }
        }
    ]
}
```

### Fetch a specific surah

#### URL

```
GET /surah
```

#### Parameters

| Name| Type | Description |
| --- | --- | --- |
| surah_number | integer | The number of a surah. |

#### Response

```json
{
    "data": {
        "number": 1,
        "basmala": false,
        "revelation_place": "meccan",
        "ayah_count": 7,
        "name": {
            "arabic": "الفاتحة",
            "translation": "The Opening",
            "transliteration": "Al-Fatiha"
        }
    }
}
```