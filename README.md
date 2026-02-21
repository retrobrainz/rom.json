# rom.json

Portable game ROM metadata file specification

## File name

*.rom.json share same file name as rom files, but with different extension.

| File name | Description |
| --- | --- |
| Yu Yu Hakusho - Makyou Toitsusen (Japan).md | ROM |
| Yu Yu Hakusho - Makyou Toitsusen (Japan).rom.json | Metadata |
| Yu Yu Hakusho - Makyou Toitsusen (Japan).boxart.jpg/png | Boxart image |
| Yu Yu Hakusho - Makyou Toitsusen (Japan).snap.jpg/png | Screenshot image |
| Yu Yu Hakusho - Makyou Toitsusen (Japan).title.jpg/png | Titlescreen image |

## File format

Standard JSON format

```json
{
  "name": "Yu Yu Hakusho - Makyou Toitsusen (Japan)",
  "description": "...",
  "platform": "Sega - Mega Drive - Genesis",
  "regions": [ "Japan" ],
  "languages": [ "Ja" ],
  "genres": [ "Fighting" ],
  "developers": [ "Treasure" ],
  "publishers": [ "Sega" ],
  "releaseDate": "1994-09-30",
  "translations": [
    {
      "locale": "ja",
      "name": "幽遊白書 魔強統一戦 (日本)",
      "description": "..."
    },
    {
      "locale": "zh-CN",
      "name": "幽游白书 魔强统一战 (日本)",
      "description": "..."
    },
  ]
}
```
