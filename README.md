# Radiation FX Overhaul

A mod for **S.T.A.L.K.E.R. Anomaly G.A.M.M.A.** by Expand.

**[Download the latest version](https://github.com/expand0501/radiation-fx-overhaul/releases/latest)** · [Русский](#русский)

You only know how much radiation there is if you carry a working geiger counter. Standalone: needs no other
radiation mod.

## Features

- Geiger clicks play only while you carry a geiger counter with a charged battery. Separate options for your own
  dose and for radiation fields around you; optionally only with the geiger in the detector slot.
- No radiation film grain on screen (can be brought back in MCM, with strength following the radiation).
- Without a charged geiger counter the HUD radiation bar shows 0 and the inventory tooltip shows "???" instead of
  the dose.
- Five modes for the HUD radiation icon, including "only with charged geiger".
- Optional integration with DAR Dosimeter Enhanced (its dosimeter modes pick which clicks you hear).
- Works with or without: DAR Dosimeter Enhanced, Grain RGB & Psi Color Effects Remover, G_FLAT's Msv Above Radiation
  Icon, G.A.M.M.A. Minimalist HUD, UI Rework G.A.M.M.A. Style.

## Installation (Mod Organizer 2)

1. Install the zip from [Releases](https://github.com/expand0501/radiation-fx-overhaul/releases) as a new mod.
2. Any position in the load order. "Radiation_Overhaul - Silent Radiation" and "No geiger sound in my head" can be
   disabled; this mod replaces them.
3. In game: MCM > Radiation FX Overhaul. No new game needed.

The full manual is in [`src/readme.md`](src/readme.md) (also inside the zip).
Changes per version: [`CHANGELOG.md`](CHANGELOG.md).

## Bug reports

Open an [issue](https://github.com/expand0501/radiation-fx-overhaul/issues) with the lines starting with
`[zzz_rad_geiger_overhaul]` from `Anomaly\appdata\logs\xray_*.log` and describe what you saw.

---

## Русский

Мод для **S.T.A.L.K.E.R. Anomaly G.A.M.M.A.**, автор Expand.

**[Скачать последнюю версию](https://github.com/expand0501/radiation-fx-overhaul/releases/latest)**

Сколько вокруг радиации, вы узнаете только с рабочим счётчиком Гейгера. Самостоятельный мод: другие моды на
радиацию не нужны.

### Возможности

- Щелчки счётчика Гейгера слышны, только пока у вас есть счётчик с заряженной батареей. Отдельные настройки для
  вашей дозы и для радиации вокруг; по желанию — только со счётчиком в слоте детектора.
- Никакой радиационной зернистости на экране (её можно вернуть в MCM, сила зависит от радиации).
- Без заряженного счётчика полоска радиации на HUD показывает 0, а в подсказке инвентаря вместо дозы — «???».
- Пять режимов иконки радиации на HUD, в том числе «только с заряженным счётчиком».
- Необязательная поддержка DAR Dosimeter Enhanced (его режимы дозиметра выбирают, какие щелчки слышны).
- Работает с этими модами и без них: DAR Dosimeter Enhanced, Grain RGB & Psi Color Effects Remover, G_FLAT's Msv
  Above Radiation Icon, G.A.M.M.A. Minimalist HUD, UI Rework G.A.M.M.A. Style.

### Установка (Mod Organizer 2)

1. Установите zip из [Releases](https://github.com/expand0501/radiation-fx-overhaul/releases) как новый мод.
2. Любое место в порядке загрузки. "Radiation_Overhaul - Silent Radiation" и "No geiger sound in my head" можно
   отключить: этот мод их заменяет.
3. В игре: MCM > Radiation FX Overhaul. Новая игра не нужна.

Полное описание (на английском) — в [`src/readme.md`](src/readme.md), он же лежит в архиве.

### Сообщить об ошибке

Создайте [issue](https://github.com/expand0501/radiation-fx-overhaul/issues), приложите строки, начинающиеся с
`[zzz_rad_geiger_overhaul]`, из `Anomaly\appdata\logs\xray_*.log` и опишите, что произошло.
