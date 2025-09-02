# JavaScript Hijri/Gregorian Datepicker Library

[![DOI: 10.5281/zenodo.2600133](https://zenodo.org/badge/doi/10.5281/zenodo.2600133.svg)](https://zenodo.org/record/2600133)

## Demo
Demo [here](https://mo7mud.github.io/Hijri-Datepicker/).

## Dependencies
- HijriDate.js which allows the use of
[`HijriDate`](https://mo7mud.github.io/Hijri-Datepicker/HijriDate.js/) objects, JS library to calculates Hijri dates in the same way as built-in
`Date` object calculates Gregorian dates.

- w3css, originally forked from [CSS Framework](https://github.com/JaniRefsnes/w3css) by
[Jan Egil Refsnes](https://github.com/JaniRefsnes) for styling this widget. 

## Usage
Simply put this code snippet to anywhere you want in the body of your html file:

### Offline
```html
<div id="datepicker"></div>
<link rel="stylesheet" href="../w3css/w3.css" />
<script type="text/javascript" src="../HijriDate.js/hijri-date.js"></script>
<script type="text/javascript" src="datepicker.js"></script>
<script type="text/javascript">
    let datepicker = new Datepicker();
    document.getElementById('datepicker').appendChild(datepicker.getElement());
    // or use
    // datepicker.attachTo(document.getElementById('datepicker'));
    // other code
</script>
```

### Online
```html
<div id="datepicker"></div>
<link rel="stylesheet" href="w3css/w3.css" />
<script type="text/javascript" src="HijriDate.js/hijri-date.js"></script>
<script type="text/javascript" src="datepicker.js"></script>
<script type="text/javascript">
    let datepicker = new Datepicker();
    document.getElementById('datepicker').appendChild(datepicker.getElement());
    // or use
    // datepicker.attachTo(document.getElementById('datepicker'));
    // other code
</script>
```

## Supported Languages
Languages currently supported are:
- Arabic (`"ar"`)
- English (`"en"`)
- Indonesian (`"id"`)

You can extend with your own language by adding this code snippet (assume your language is English):
```javascript
Datepicker.language["en"] = {
    isRTL: false,             // or true for right to left language
    eraSuffix: ["AD", "BC"],  // suffix for Gregorian era
    hEraSuffix: ["H", "BH"],  // suffix for Hijri era
    monthNames: [
        "January",
        "February",
        "March",
        "April",
        "May",
        "June",
        "July",
        "August",
        "September",
        "October",
        "November",
        "December"
    ],
    weekdayNames: [
        "Sunday",
        "Monday",
        "Tuesday",
        "Wednesday",
        "Thursday",
        "Friday",
        "Saturday"
    ],
    weekdayShortNames: ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
    hMonthNames: [
        "Muharram",
        "Safar",
        "Rabi'ul-Awwal",
        "Rabi'ul-Akhir",
        "Jumadal-Ula",
        "Jumadal-Akhir",
        "Rajab","Sha'ban",
        "Ramadan",
        "Syawwal",
        "Dhul-Qa'da",
        "Dhul-Hijja"
    ];
};
```
You are very welcomed to contribute your language to add to the library

## API Documentation
API doc [here](datepicker-api-doc.md).

&nbsp;

&nbsp;

&nbsp;

---
#### Designed By ZulNs
##### @Gorontalo, 8 January 2019

### Development continued in 2025 By Mohammad Ahmad
#### @Mo7mud, 3 September 2025
---
