# Norton DeskTop for Windows 2.0 Archive

> Архив файлов **Norton DeskTop for Windows 2.0** и DOS-утилит Norton, сохраненный как набор с floppy disk.

[![Archive](https://img.shields.io/badge/type-software%20archive-2f80ed)](#содержимое)
[![Platform](https://img.shields.io/badge/platform-DOS%20%2F%20Windows%203.x-lightgrey)](#как-использовать)
[![Version](https://img.shields.io/badge/version-2.0-green)](#о-репозитории)
[![Status](https://img.shields.io/badge/status-preserved-yellow)](#дисклеймер)

## О репозитории

Репозиторий хранит компактный набор файлов **Norton DeskTop for Windows 2.0**: исполняемые DOS-утилиты, системные компоненты, сжатые Windows-файлы и служебный `NORTON.INI`.

Архив полезен для сохранения legacy-софта, восстановления старых окружений, работы в DOSBox/виртуальных машинах и изучения состава старых дискетных комплектов Norton.

## Содержимое

| Файл | Назначение |
| --- | --- |
| `NAV.EXE` | Norton AntiVirus / основная утилита NAV |
| `NDD.EXE` | Norton Disk Doctor |
| `SPEEDISK.EXE` | утилита оптимизации/дефрагментации диска |
| `UNERASE.EXE` | восстановление удаленных файлов |
| `UNFORMAT.EXE` | восстановление после форматирования |
| `NPACK.EXE` | служебная утилита Norton |
| `NAV&.SYS`, `NAV_.SYS` | системные компоненты NAV |
| `NAVDLL.DL$`, `NAVPOPUP.EX$`, `VNAVD.38$` | сжатые Windows-компоненты |
| `NORTON.INI` | служебный INI/данные конфигурации |

Подробная карта файлов находится в [`FILES.md`](FILES.md).

## Структура

```text
.
├── CHECKSUMS.txt
├── FILES.md
├── README.md
└── Norton DeskTop for Windows 2.0/
    ├── NAV.EXE
    ├── NDD.EXE
    ├── SPEEDISK.EXE
    ├── UNERASE.EXE
    ├── UNFORMAT.EXE
    ├── NPACK.EXE
    ├── NAV&.SYS
    ├── NAV_.SYS
    ├── NAVDLL.DL$
    ├── NAVPOPUP.EX$
    ├── VNAVD.38$
    └── NORTON.INI
```

## Как использовать

1. Работайте только в изолированной среде: DOSBox, виртуальная машина или тестовая Windows 3.x / DOS-система.
2. Перед запуском проверьте файлы по [`CHECKSUMS.txt`](CHECKSUMS.txt).
3. Основные исполняемые файлы находятся в папке:

```text
Norton DeskTop for Windows 2.0/
```

4. Для экспериментов с утилитами запускайте нужный `.EXE` внутри DOS/Windows 3.x-совместимой среды.

## Контрольные суммы

Проверить отдельный файл в PowerShell:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath "Norton DeskTop for Windows 2.0\NAV.EXE"
```

Полный список SHA-256 находится в [`CHECKSUMS.txt`](CHECKSUMS.txt).

## Дисклеймер

Репозиторий является архивной копией старого программного обеспечения. Файлы предоставлены для сохранения, изучения и восстановления legacy-сред. Все права на Norton DeskTop, Norton Utilities, Norton AntiVirus, документацию и торговые марки принадлежат их законным правообладателям.

Запускайте старые исполняемые файлы только в безопасной изолированной среде.
