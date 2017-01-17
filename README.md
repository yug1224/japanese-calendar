# japanese-calendar [![npm version](https://badge.fury.io/js/japanese-calendar.svg)](https://badge.fury.io/js/japanese-calendar)

This module is for converting Japanese calendar

[![NPM](https://nodei.co/npm/japanese-calendar.png?downloads=true&downloadRank=true&stars=true)](https://nodei.co/npm/japanese-calendar/)

## Install

### cli
```bash
npm install -g japanese-calendar
```

### js
```bash
npm install japanese-calendar
```

## Usage

### cli
```bash
Usage: japanese-calendar [options]

Options:

  -h, --help         output usage information
  -f, --from [from]  This flag specifies the calendar to convert.,
        Choose Calendar:
          c, Christian : Christian Era
          j, Japanese  : Japanese Calendar
  -t, --type [type]  This flag specifies the Japanese calendar to convert.
        Choose Calendar:
          m, Meiji  : Meiji
          t, Taisho : Taisho
          s, Showa  : Showa
          h, Heisei : Heisei
  -y, --year [year]  This flag specifies the year to be converted.

japanese-calendar -f christian -t heisei -y 2017
# 29

japanese-calendar -f japanese -t heisei -y 29
# 2017
```

### js

```js
const calendar = require('japanese-calendar');

console.log(calendar('christian', 'heisei', 2017));
// 29

console.log(calendar('japanese', 'heisei', 29));
// 2017
```

## License
[MIT](http://opensource.org/licenses/mit-license.php)

## Author
[YuG1224](https://github.com/YuG1224)
