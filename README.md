# rom.json

Portable game ROM metadata file specification

## File name

### Single-file ROM

*.rom.json share same file name as rom files, but with different extension.

| File name | Description |
| --- | --- |
| Yu Yu Hakusho - Makyou Toitsusen (Japan).md | ROM |
| Yu Yu Hakusho - Makyou Toitsusen (Japan).rom.json | Metadata |
| Yu Yu Hakusho - Makyou Toitsusen (Japan).boxart.jpg/png | Boxart image |
| Yu Yu Hakusho - Makyou Toitsusen (Japan).snap.jpg/png | Screenshot image |
| Yu Yu Hakusho - Makyou Toitsusen (Japan).title.jpg/png | Titlescreen image |

Some disc images are dumped as `.bin` file and `.cue` file. They are also treated as single file ROM, though two file :-)

| File name | Description |
| --- | --- |
| Crash Bandicoot (USA).bin | ROM data |
| Crash Bandicoot (USA).cue | ROM index |
| Crash Bandicoot (USA).rom.json | Metadata |
| Crash Bandicoot (USA).boxart.jpg/png | Boxart image |
| Crash Bandicoot (USA).snap.jpg/png | Screenshot image |
| Crash Bandicoot (USA).title.jpg/png | Titlescreen image |

### Extract ROM and multi-file ROM

In some cases, ROM is a folder that contains many files:

1. Unmerged arcade (MAME) ROM
2. Extracted ISO (Some emulators, like RPCS3, don't support ISO/CHD format, you have extract all files)

In this case, metadata file and image files should be placed directly under the ROM folder and named as following:

| File name | Description |
| --- | --- |
| rom.json | Metadata |
| boxart.jpg/png | Boxart image |
| snap.jpg/png | Screenshot image |
| title.jpg/png | Titlescreen image |

## File format

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
      "description": "...",
      "regions": [ "日本" ],
      "languages": [ "日本語" ],
      "genres": [ "対戦格闘" ]
    },
    {
      "locale": "zh-CN",
      "name": "幽游白书 魔强统一战 (日本)",
      "description": "...",
      "regions": [ "日本" ],
      "languages": [ "日语" ],
      "genres": [ "格斗" ]
    }
  ]
}
```
