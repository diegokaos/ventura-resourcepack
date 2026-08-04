# VenturaFishing Resource Pack

Готовый resource-pack для плагина **VenturaFishing**: уникальные рыбы, мусор и две особые удочки без ItemsAdder или Oraxen.

![Превью текстур](texture-preview.png)

## Скачать и установить

1. Скачайте [последний ZIP](https://github.com/diegokaos/ventura-resourcepack/releases/latest/download/VenturaFishing-ResourcePack-1.21.x.zip).
2. Загрузите ZIP на сервер или используйте прямую ссылку GitHub Releases.
3. Вставьте настройки из [`server.properties.example`](server.properties.example) в `server.properties`.
4. Полностью перезапустите сервер.

```properties
resource-pack=https://github.com/diegokaos/ventura-resourcepack/releases/latest/download/VenturaFishing-ResourcePack-1.21.x.zip
resource-pack-sha1=400b80de9185f3bd3757d8adffe5f8deb6a3a85d
require-resource-pack=true
```

## Совместимость

Один ZIP поддерживает все релизные версии Minecraft Java от `1.21` до `1.21.11`.

| Версии клиента | Формат моделей |
| --- | --- |
| `1.21`–`1.21.3` | legacy `models/item` и `overrides` |
| `1.21.4`–`1.21.11` | современные item models из overlay |

## Модели

| ID | Предмет | model-data |
| --- | --- | ---: |
| `rainbow_fish` | Радужная рыба | 1101 |
| `crystal_fish` | Кристальная рыба | 1102 |
| `salmon_king` | Королевский лосось | 1103 |
| `golden_carp` | Золотой карп | 1104 |
| `shark` | Акула | 1105 |
| `old_boot` | Старый сапог | 1199 |
| `summer_tide` | Сезонная удочка | 2101 |
| `abyssal` | Лимитированная удочка | 2102 |

## Шаблоны для своей текстуры

В папке [`templates`](templates) лежат PSD, PNG-сетка 64×64 и инструкция на русском. Экспортируйте текстуры в `PNG-24` с прозрачностью и не используйте одну пару `material + model-data` дважды.

После изменения ZIP пересчитайте SHA-1 и замените его в `server.properties`.
