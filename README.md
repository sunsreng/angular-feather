## angular-feather

[![npm](https://img.shields.io/npm/v/angular-feather.svg?style=flat-square)]()
[![license](https://img.shields.io/npm/l/angular-feather.svg?style=flat-square)]()
[![stars](https://img.shields.io/github/stars/michaelbazos/angular-feather.svg?style=flat-square)]()
[![deps status](https://david-dm.org/michaelbazos/angular-feather/status.svg?style=flat-square)](https://david-dm.org/michaelbazos/angular-feather)

### Description

This package allows you to use the [Feather Icons](https://github.com/colebemis/feather) in your angular applications. The icons are designed by Cole Bemis.

Import only the icons that you need :)

<h3>
  <a href="https://stackblitz.com/edit/angular-feather?file=app%2Fapp.component.html">
    Live Demo
  </a>
</h3>

### Usage

_1. Install the package_

```sh
npm install angular-feather
```
  
_2. Import the icons you need_
  
Import the icons _a la carte_. Keep consistency by defining an `IconsModule`. As this angular module doesn't use the icons, it only uses the `exports` array property to export the icons your feature module need. Therefore you deal only with the aggregation `IconsModule` when you need to import icons in feature modules.

```ts  
import { NgModule } from '@angular/core';

import { IconLogIn, IconLogOut, IconUser } from 'angular-feather';

@NgModule({
  exports: [
    IconLogIn,
    IconLogOut,
    IconUser
  ]
})
export class IconsModule { }
```

_3. Use it in template_

```html
<i-log-in></i-log-in>
<i-log-out></i-log-out>
<i-user></i-user>
```
    
Refer to the table below for the list of all available icons.

|     | Symbol to import | Component selector |
| --- | ---------------- | ------------------ |
| ![activity](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/activity.svg) | `IconActivity` | `<i-activity>` |
| ![airplay](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/airplay.svg) | `IconAirplay` | `<i-airplay>` |
| ![alert-circle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/alert-circle.svg) | `IconAlertCircle` | `<i-alert-circle>` |
| ![alert-octagon](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/alert-octagon.svg) | `IconAlertOctagon` | `<i-alert-octagon>` |
| ![alert-triangle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/alert-triangle.svg) | `IconAlertTriangle` | `<i-alert-triangle>` |
| ![align-center](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/align-center.svg) | `IconAlignCenter` | `<i-align-center>` |
| ![align-justify](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/align-justify.svg) | `IconAlignJustify` | `<i-align-justify>` |
| ![align-left](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/align-left.svg) | `IconAlignLeft` | `<i-align-left>` |
| ![align-right](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/align-right.svg) | `IconAlignRight` | `<i-align-right>` |
| ![anchor](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/anchor.svg) | `IconAnchor` | `<i-anchor>` |
| ![aperture](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/aperture.svg) | `IconAperture` | `<i-aperture>` |
| ![arrow-down-circle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/arrow-down-circle.svg) | `IconArrowDownCircle` | `<i-arrow-down-circle>` |
| ![arrow-down-left](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/arrow-down-left.svg) | `IconArrowDownLeft` | `<i-arrow-down-left>` |
| ![arrow-down-right](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/arrow-down-right.svg) | `IconArrowDownRight` | `<i-arrow-down-right>` |
| ![arrow-down](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/arrow-down.svg) | `IconArrowDown` | `<i-arrow-down>` |
| ![arrow-left-circle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/arrow-left-circle.svg) | `IconArrowLeftCircle` | `<i-arrow-left-circle>` |
| ![arrow-left](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/arrow-left.svg) | `IconArrowLeft` | `<i-arrow-left>` |
| ![arrow-right-circle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/arrow-right-circle.svg) | `IconArrowRightCircle` | `<i-arrow-right-circle>` |
| ![arrow-right](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/arrow-right.svg) | `IconArrowRight` | `<i-arrow-right>` |
| ![arrow-up-circle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/arrow-up-circle.svg) | `IconArrowUpCircle` | `<i-arrow-up-circle>` |
| ![arrow-up-left](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/arrow-up-left.svg) | `IconArrowUpLeft` | `<i-arrow-up-left>` |
| ![arrow-up-right](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/arrow-up-right.svg) | `IconArrowUpRight` | `<i-arrow-up-right>` |
| ![arrow-up](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/arrow-up.svg) | `IconArrowUp` | `<i-arrow-up>` |
| ![at-sign](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/at-sign.svg) | `IconAtSign` | `<i-at-sign>` |
| ![award](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/award.svg) | `IconAward` | `<i-award>` |
| ![bar-chart-2](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/bar-chart-2.svg) | `IconBarChart2` | `<i-bar-chart-2>` |
| ![bar-chart](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/bar-chart.svg) | `IconBarChart` | `<i-bar-chart>` |
| ![battery-charging](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/battery-charging.svg) | `IconBatteryCharging` | `<i-battery-charging>` |
| ![battery](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/battery.svg) | `IconBattery` | `<i-battery>` |
| ![bell-off](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/bell-off.svg) | `IconBellOff` | `<i-bell-off>` |
| ![bell](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/bell.svg) | `IconBell` | `<i-bell>` |
| ![bluetooth](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/bluetooth.svg) | `IconBluetooth` | `<i-bluetooth>` |
| ![bold](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/bold.svg) | `IconBold` | `<i-bold>` |
| ![book-open](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/book-open.svg) | `IconBookOpen` | `<i-book-open>` |
| ![book](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/book.svg) | `IconBook` | `<i-book>` |
| ![bookmark](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/bookmark.svg) | `IconBookmark` | `<i-bookmark>` |
| ![box](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/box.svg) | `IconBox` | `<i-box>` |
| ![briefcase](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/briefcase.svg) | `IconBriefcase` | `<i-briefcase>` |
| ![calendar](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/calendar.svg) | `IconCalendar` | `<i-calendar>` |
| ![camera-off](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/camera-off.svg) | `IconCameraOff` | `<i-camera-off>` |
| ![camera](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/camera.svg) | `IconCamera` | `<i-camera>` |
| ![cast](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/cast.svg) | `IconCast` | `<i-cast>` |
| ![check-circle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/check-circle.svg) | `IconCheckCircle` | `<i-check-circle>` |
| ![check-square](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/check-square.svg) | `IconCheckSquare` | `<i-check-square>` |
| ![check](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/check.svg) | `IconCheck` | `<i-check>` |
| ![chevron-down](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/chevron-down.svg) | `IconChevronDown` | `<i-chevron-down>` |
| ![chevron-left](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/chevron-left.svg) | `IconChevronLeft` | `<i-chevron-left>` |
| ![chevron-right](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/chevron-right.svg) | `IconChevronRight` | `<i-chevron-right>` |
| ![chevron-up](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/chevron-up.svg) | `IconChevronUp` | `<i-chevron-up>` |
| ![chevrons-down](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/chevrons-down.svg) | `IconChevronsDown` | `<i-chevrons-down>` |
| ![chevrons-left](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/chevrons-left.svg) | `IconChevronsLeft` | `<i-chevrons-left>` |
| ![chevrons-right](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/chevrons-right.svg) | `IconChevronsRight` | `<i-chevrons-right>` |
| ![chevrons-up](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/chevrons-up.svg) | `IconChevronsUp` | `<i-chevrons-up>` |
| ![chrome](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/chrome.svg) | `IconChrome` | `<i-chrome>` |
| ![circle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/circle.svg) | `IconCircle` | `<i-circle>` |
| ![clipboard](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/clipboard.svg) | `IconClipboard` | `<i-clipboard>` |
| ![clock](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/clock.svg) | `IconClock` | `<i-clock>` |
| ![cloud-drizzle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/cloud-drizzle.svg) | `IconCloudDrizzle` | `<i-cloud-drizzle>` |
| ![cloud-lightning](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/cloud-lightning.svg) | `IconCloudLightning` | `<i-cloud-lightning>` |
| ![cloud-off](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/cloud-off.svg) | `IconCloudOff` | `<i-cloud-off>` |
| ![cloud-rain](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/cloud-rain.svg) | `IconCloudRain` | `<i-cloud-rain>` |
| ![cloud-snow](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/cloud-snow.svg) | `IconCloudSnow` | `<i-cloud-snow>` |
| ![cloud](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/cloud.svg) | `IconCloud` | `<i-cloud>` |
| ![code](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/code.svg) | `IconCode` | `<i-code>` |
| ![codepen](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/codepen.svg) | `IconCodepen` | `<i-codepen>` |
| ![command](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/command.svg) | `IconCommand` | `<i-command>` |
| ![compass](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/compass.svg) | `IconCompass` | `<i-compass>` |
| ![copy](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/copy.svg) | `IconCopy` | `<i-copy>` |
| ![corner-down-left](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/corner-down-left.svg) | `IconCornerDownLeft` | `<i-corner-down-left>` |
| ![corner-down-right](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/corner-down-right.svg) | `IconCornerDownRight` | `<i-corner-down-right>` |
| ![corner-left-down](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/corner-left-down.svg) | `IconCornerLeftDown` | `<i-corner-left-down>` |
| ![corner-left-up](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/corner-left-up.svg) | `IconCornerLeftUp` | `<i-corner-left-up>` |
| ![corner-right-down](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/corner-right-down.svg) | `IconCornerRightDown` | `<i-corner-right-down>` |
| ![corner-right-up](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/corner-right-up.svg) | `IconCornerRightUp` | `<i-corner-right-up>` |
| ![corner-up-left](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/corner-up-left.svg) | `IconCornerUpLeft` | `<i-corner-up-left>` |
| ![corner-up-right](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/corner-up-right.svg) | `IconCornerUpRight` | `<i-corner-up-right>` |
| ![cpu](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/cpu.svg) | `IconCpu` | `<i-cpu>` |
| ![credit-card](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/credit-card.svg) | `IconCreditCard` | `<i-credit-card>` |
| ![crop](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/crop.svg) | `IconCrop` | `<i-crop>` |
| ![crosshair](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/crosshair.svg) | `IconCrosshair` | `<i-crosshair>` |
| ![database](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/database.svg) | `IconDatabase` | `<i-database>` |
| ![delete](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/delete.svg) | `IconDelete` | `<i-delete>` |
| ![disc](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/disc.svg) | `IconDisc` | `<i-disc>` |
| ![dollar-sign](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/dollar-sign.svg) | `IconDollarSign` | `<i-dollar-sign>` |
| ![download-cloud](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/download-cloud.svg) | `IconDownloadCloud` | `<i-download-cloud>` |
| ![download](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/download.svg) | `IconDownload` | `<i-download>` |
| ![droplet](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/droplet.svg) | `IconDroplet` | `<i-droplet>` |
| ![edit-2](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/edit-2.svg) | `IconEdit2` | `<i-edit-2>` |
| ![edit-3](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/edit-3.svg) | `IconEdit3` | `<i-edit-3>` |
| ![edit](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/edit.svg) | `IconEdit` | `<i-edit>` |
| ![external-link](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/external-link.svg) | `IconExternalLink` | `<i-external-link>` |
| ![eye-off](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/eye-off.svg) | `IconEyeOff` | `<i-eye-off>` |
| ![eye](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/eye.svg) | `IconEye` | `<i-eye>` |
| ![facebook](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/facebook.svg) | `IconFacebook` | `<i-facebook>` |
| ![fast-forward](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/fast-forward.svg) | `IconFastForward` | `<i-fast-forward>` |
| ![feather](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/feather.svg) | `IconFeather` | `<i-feather>` |
| ![file-minus](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/file-minus.svg) | `IconFileMinus` | `<i-file-minus>` |
| ![file-plus](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/file-plus.svg) | `IconFilePlus` | `<i-file-plus>` |
| ![file-text](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/file-text.svg) | `IconFileText` | `<i-file-text>` |
| ![file](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/file.svg) | `IconFile` | `<i-file>` |
| ![film](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/film.svg) | `IconFilm` | `<i-film>` |
| ![filter](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/filter.svg) | `IconFilter` | `<i-filter>` |
| ![flag](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/flag.svg) | `IconFlag` | `<i-flag>` |
| ![folder-minus](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/folder-minus.svg) | `IconFolderMinus` | `<i-folder-minus>` |
| ![folder-plus](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/folder-plus.svg) | `IconFolderPlus` | `<i-folder-plus>` |
| ![folder](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/folder.svg) | `IconFolder` | `<i-folder>` |
| ![git-branch](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/git-branch.svg) | `IconGitBranch` | `<i-git-branch>` |
| ![git-commit](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/git-commit.svg) | `IconGitCommit` | `<i-git-commit>` |
| ![git-merge](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/git-merge.svg) | `IconGitMerge` | `<i-git-merge>` |
| ![git-pull-request](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/git-pull-request.svg) | `IconGitPullRequest` | `<i-git-pull-request>` |
| ![github](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/github.svg) | `IconGithub` | `<i-github>` |
| ![gitlab](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/gitlab.svg) | `IconGitlab` | `<i-gitlab>` |
| ![globe](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/globe.svg) | `IconGlobe` | `<i-globe>` |
| ![grid](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/grid.svg) | `IconGrid` | `<i-grid>` |
| ![hard-drive](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/hard-drive.svg) | `IconHardDrive` | `<i-hard-drive>` |
| ![hash](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/hash.svg) | `IconHash` | `<i-hash>` |
| ![headphones](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/headphones.svg) | `IconHeadphones` | `<i-headphones>` |
| ![heart](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/heart.svg) | `IconHeart` | `<i-heart>` |
| ![help-circle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/help-circle.svg) | `IconHelpCircle` | `<i-help-circle>` |
| ![home](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/home.svg) | `IconHome` | `<i-home>` |
| ![image](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/image.svg) | `IconImage` | `<i-image>` |
| ![inbox](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/inbox.svg) | `IconInbox` | `<i-inbox>` |
| ![info](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/info.svg) | `IconInfo` | `<i-info>` |
| ![instagram](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/instagram.svg) | `IconInstagram` | `<i-instagram>` |
| ![italic](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/italic.svg) | `IconItalic` | `<i-italic>` |
| ![layers](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/layers.svg) | `IconLayers` | `<i-layers>` |
| ![layout](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/layout.svg) | `IconLayout` | `<i-layout>` |
| ![life-buoy](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/life-buoy.svg) | `IconLifeBuoy` | `<i-life-buoy>` |
| ![link-2](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/link-2.svg) | `IconLink2` | `<i-link-2>` |
| ![link](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/link.svg) | `IconLink` | `<i-link>` |
| ![linkedin](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/linkedin.svg) | `IconLinkedin` | `<i-linkedin>` |
| ![list](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/list.svg) | `IconList` | `<i-list>` |
| ![loader](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/loader.svg) | `IconLoader` | `<i-loader>` |
| ![lock](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/lock.svg) | `IconLock` | `<i-lock>` |
| ![log-in](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/log-in.svg) | `IconLogIn` | `<i-log-in>` |
| ![log-out](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/log-out.svg) | `IconLogOut` | `<i-log-out>` |
| ![mail](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/mail.svg) | `IconMail` | `<i-mail>` |
| ![map-pin](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/map-pin.svg) | `IconMapPin` | `<i-map-pin>` |
| ![map](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/map.svg) | `IconMap` | `<i-map>` |
| ![maximize-2](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/maximize-2.svg) | `IconMaximize2` | `<i-maximize-2>` |
| ![maximize](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/maximize.svg) | `IconMaximize` | `<i-maximize>` |
| ![menu](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/menu.svg) | `IconMenu` | `<i-menu>` |
| ![message-circle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/message-circle.svg) | `IconMessageCircle` | `<i-message-circle>` |
| ![message-square](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/message-square.svg) | `IconMessageSquare` | `<i-message-square>` |
| ![mic-off](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/mic-off.svg) | `IconMicOff` | `<i-mic-off>` |
| ![mic](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/mic.svg) | `IconMic` | `<i-mic>` |
| ![minimize-2](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/minimize-2.svg) | `IconMinimize2` | `<i-minimize-2>` |
| ![minimize](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/minimize.svg) | `IconMinimize` | `<i-minimize>` |
| ![minus-circle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/minus-circle.svg) | `IconMinusCircle` | `<i-minus-circle>` |
| ![minus-square](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/minus-square.svg) | `IconMinusSquare` | `<i-minus-square>` |
| ![minus](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/minus.svg) | `IconMinus` | `<i-minus>` |
| ![monitor](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/monitor.svg) | `IconMonitor` | `<i-monitor>` |
| ![moon](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/moon.svg) | `IconMoon` | `<i-moon>` |
| ![more-horizontal](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/more-horizontal.svg) | `IconMoreHorizontal` | `<i-more-horizontal>` |
| ![more-vertical](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/more-vertical.svg) | `IconMoreVertical` | `<i-more-vertical>` |
| ![move](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/move.svg) | `IconMove` | `<i-move>` |
| ![music](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/music.svg) | `IconMusic` | `<i-music>` |
| ![navigation-2](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/navigation-2.svg) | `IconNavigation2` | `<i-navigation-2>` |
| ![navigation](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/navigation.svg) | `IconNavigation` | `<i-navigation>` |
| ![octagon](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/octagon.svg) | `IconOctagon` | `<i-octagon>` |
| ![package](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/package.svg) | `IconPackage` | `<i-package>` |
| ![paperclip](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/paperclip.svg) | `IconPaperclip` | `<i-paperclip>` |
| ![pause-circle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/pause-circle.svg) | `IconPauseCircle` | `<i-pause-circle>` |
| ![pause](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/pause.svg) | `IconPause` | `<i-pause>` |
| ![percent](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/percent.svg) | `IconPercent` | `<i-percent>` |
| ![phone-call](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/phone-call.svg) | `IconPhoneCall` | `<i-phone-call>` |
| ![phone-forwarded](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/phone-forwarded.svg) | `IconPhoneForwarded` | `<i-phone-forwarded>` |
| ![phone-incoming](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/phone-incoming.svg) | `IconPhoneIncoming` | `<i-phone-incoming>` |
| ![phone-missed](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/phone-missed.svg) | `IconPhoneMissed` | `<i-phone-missed>` |
| ![phone-off](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/phone-off.svg) | `IconPhoneOff` | `<i-phone-off>` |
| ![phone-outgoing](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/phone-outgoing.svg) | `IconPhoneOutgoing` | `<i-phone-outgoing>` |
| ![phone](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/phone.svg) | `IconPhone` | `<i-phone>` |
| ![pie-chart](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/pie-chart.svg) | `IconPieChart` | `<i-pie-chart>` |
| ![play-circle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/play-circle.svg) | `IconPlayCircle` | `<i-play-circle>` |
| ![play](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/play.svg) | `IconPlay` | `<i-play>` |
| ![plus-circle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/plus-circle.svg) | `IconPlusCircle` | `<i-plus-circle>` |
| ![plus-square](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/plus-square.svg) | `IconPlusSquare` | `<i-plus-square>` |
| ![plus](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/plus.svg) | `IconPlus` | `<i-plus>` |
| ![pocket](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/pocket.svg) | `IconPocket` | `<i-pocket>` |
| ![power](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/power.svg) | `IconPower` | `<i-power>` |
| ![printer](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/printer.svg) | `IconPrinter` | `<i-printer>` |
| ![radio](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/radio.svg) | `IconRadio` | `<i-radio>` |
| ![refresh-ccw](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/refresh-ccw.svg) | `IconRefreshCcw` | `<i-refresh-ccw>` |
| ![refresh-cw](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/refresh-cw.svg) | `IconRefreshCw` | `<i-refresh-cw>` |
| ![repeat](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/repeat.svg) | `IconRepeat` | `<i-repeat>` |
| ![rewind](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/rewind.svg) | `IconRewind` | `<i-rewind>` |
| ![rotate-ccw](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/rotate-ccw.svg) | `IconRotateCcw` | `<i-rotate-ccw>` |
| ![rotate-cw](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/rotate-cw.svg) | `IconRotateCw` | `<i-rotate-cw>` |
| ![rss](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/rss.svg) | `IconRss` | `<i-rss>` |
| ![save](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/save.svg) | `IconSave` | `<i-save>` |
| ![scissors](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/scissors.svg) | `IconScissors` | `<i-scissors>` |
| ![search](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/search.svg) | `IconSearch` | `<i-search>` |
| ![send](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/send.svg) | `IconSend` | `<i-send>` |
| ![server](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/server.svg) | `IconServer` | `<i-server>` |
| ![settings](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/settings.svg) | `IconSettings` | `<i-settings>` |
| ![share-2](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/share-2.svg) | `IconShare2` | `<i-share-2>` |
| ![share](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/share.svg) | `IconShare` | `<i-share>` |
| ![shield-off](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/shield-off.svg) | `IconShieldOff` | `<i-shield-off>` |
| ![shield](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/shield.svg) | `IconShield` | `<i-shield>` |
| ![shopping-bag](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/shopping-bag.svg) | `IconShoppingBag` | `<i-shopping-bag>` |
| ![shopping-cart](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/shopping-cart.svg) | `IconShoppingCart` | `<i-shopping-cart>` |
| ![shuffle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/shuffle.svg) | `IconShuffle` | `<i-shuffle>` |
| ![sidebar](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/sidebar.svg) | `IconSidebar` | `<i-sidebar>` |
| ![skip-back](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/skip-back.svg) | `IconSkipBack` | `<i-skip-back>` |
| ![skip-forward](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/skip-forward.svg) | `IconSkipForward` | `<i-skip-forward>` |
| ![slack](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/slack.svg) | `IconSlack` | `<i-slack>` |
| ![slash](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/slash.svg) | `IconSlash` | `<i-slash>` |
| ![sliders](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/sliders.svg) | `IconSliders` | `<i-sliders>` |
| ![smartphone](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/smartphone.svg) | `IconSmartphone` | `<i-smartphone>` |
| ![speaker](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/speaker.svg) | `IconSpeaker` | `<i-speaker>` |
| ![square](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/square.svg) | `IconSquare` | `<i-square>` |
| ![star](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/star.svg) | `IconStar` | `<i-star>` |
| ![stop-circle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/stop-circle.svg) | `IconStopCircle` | `<i-stop-circle>` |
| ![sun](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/sun.svg) | `IconSun` | `<i-sun>` |
| ![sunrise](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/sunrise.svg) | `IconSunrise` | `<i-sunrise>` |
| ![sunset](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/sunset.svg) | `IconSunset` | `<i-sunset>` |
| ![tablet](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/tablet.svg) | `IconTablet` | `<i-tablet>` |
| ![tag](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/tag.svg) | `IconTag` | `<i-tag>` |
| ![target](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/target.svg) | `IconTarget` | `<i-target>` |
| ![terminal](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/terminal.svg) | `IconTerminal` | `<i-terminal>` |
| ![thermometer](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/thermometer.svg) | `IconThermometer` | `<i-thermometer>` |
| ![thumbs-down](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/thumbs-down.svg) | `IconThumbsDown` | `<i-thumbs-down>` |
| ![thumbs-up](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/thumbs-up.svg) | `IconThumbsUp` | `<i-thumbs-up>` |
| ![toggle-left](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/toggle-left.svg) | `IconToggleLeft` | `<i-toggle-left>` |
| ![toggle-right](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/toggle-right.svg) | `IconToggleRight` | `<i-toggle-right>` |
| ![trash-2](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/trash-2.svg) | `IconTrash2` | `<i-trash-2>` |
| ![trash](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/trash.svg) | `IconTrash` | `<i-trash>` |
| ![trending-down](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/trending-down.svg) | `IconTrendingDown` | `<i-trending-down>` |
| ![trending-up](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/trending-up.svg) | `IconTrendingUp` | `<i-trending-up>` |
| ![triangle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/triangle.svg) | `IconTriangle` | `<i-triangle>` |
| ![truck](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/truck.svg) | `IconTruck` | `<i-truck>` |
| ![tv](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/tv.svg) | `IconTv` | `<i-tv>` |
| ![twitter](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/twitter.svg) | `IconTwitter` | `<i-twitter>` |
| ![type](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/type.svg) | `IconType` | `<i-type>` |
| ![umbrella](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/umbrella.svg) | `IconUmbrella` | `<i-umbrella>` |
| ![underline](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/underline.svg) | `IconUnderline` | `<i-underline>` |
| ![unlock](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/unlock.svg) | `IconUnlock` | `<i-unlock>` |
| ![upload-cloud](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/upload-cloud.svg) | `IconUploadCloud` | `<i-upload-cloud>` |
| ![upload](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/upload.svg) | `IconUpload` | `<i-upload>` |
| ![user-check](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/user-check.svg) | `IconUserCheck` | `<i-user-check>` |
| ![user-minus](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/user-minus.svg) | `IconUserMinus` | `<i-user-minus>` |
| ![user-plus](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/user-plus.svg) | `IconUserPlus` | `<i-user-plus>` |
| ![user-x](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/user-x.svg) | `IconUserX` | `<i-user-x>` |
| ![user](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/user.svg) | `IconUser` | `<i-user>` |
| ![users](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/users.svg) | `IconUsers` | `<i-users>` |
| ![video-off](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/video-off.svg) | `IconVideoOff` | `<i-video-off>` |
| ![video](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/video.svg) | `IconVideo` | `<i-video>` |
| ![voicemail](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/voicemail.svg) | `IconVoicemail` | `<i-voicemail>` |
| ![volume-1](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/volume-1.svg) | `IconVolume1` | `<i-volume-1>` |
| ![volume-2](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/volume-2.svg) | `IconVolume2` | `<i-volume-2>` |
| ![volume-x](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/volume-x.svg) | `IconVolumeX` | `<i-volume-x>` |
| ![volume](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/volume.svg) | `IconVolume` | `<i-volume>` |
| ![watch](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/watch.svg) | `IconWatch` | `<i-watch>` |
| ![wifi-off](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/wifi-off.svg) | `IconWifiOff` | `<i-wifi-off>` |
| ![wifi](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/wifi.svg) | `IconWifi` | `<i-wifi>` |
| ![wind](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/wind.svg) | `IconWind` | `<i-wind>` |
| ![x-circle](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/x-circle.svg) | `IconXCircle` | `<i-x-circle>` |
| ![x-square](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/x-square.svg) | `IconXSquare` | `<i-x-square>` |
| ![x](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/x.svg) | `IconX` | `<i-x>` |
| ![zap-off](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/zap-off.svg) | `IconZapOff` | `<i-zap-off>` |
| ![zap](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/zap.svg) | `IconZap` | `<i-zap>` |
| ![zoom-in](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/zoom-in.svg) | `IconZoomIn` | `<i-zoom-in>` |
| ![zoom-out](https://cdn.rawgit.com/michaelbazos/angular-feather/0183b1edfa41235532f4fd303256dd1e97ed7835/docs/icons/zoom-out.svg) | `IconZoomOut` | `<i-zoom-out>` |

### FAQ

_1. Can I import all icons at once?_

See [issue 1](https://github.com/michaelbazos/angular-feather/issues/1)

### License

MIT © [Michael Bazos](mailto:micabazos@gmail.com)
