# onkel
A commandline calender inspired by cal and ncal.

<img src="https://raw.githubusercontent.com/ztiromoritz/ncal-js/master/screenshot.png" alt="screenshot" width="360">

## Installation
```
npm install -g onkel
```

## Some examples:
```
onkel          # calendar of the current month
onkel -y       # calendar of the current year
onkel 2048     # calendar of the year 2048
onkel -3       # calendar of three month: the last, the current, and the upcomming
onkel 12 1990  # calendar of the December 1990
```
## Highlighting
The current day, if visible, is highlighted in all these examples.
You can control these highligting by disable it completly or customize 
the dates to highlight.
```
onkel -n       # current month without highlight
# To set custom highlights use -H            
onkel 1981 -H 1981-07-23,1981-07-24
```

## Localization
Onkel only supports gregorian calendar based on [moment.js](https://momentjs.com/).
```
onkel -L          # to get a list of all available locales
onkel -l de 1981  # to get the calendar
```

## All Options

```
Usage: onkel [options] <<month> year>

A commandline calendar inspired by tools like cal, pal and ncal.

Options:

  -v, --version             output the version number
  -l, --locale <locale>     Select a locale.
  -L, --listLocales         List available locales.
  -y, --year                Display a calendar for the specified year.
  -t, --textOnly            No color escape sequences.
  -n, --noHighlights        No highlights at all. (Overrides -H).
  -H, --highlights [dates]  Comma separated lists of dates to highlight. This does not affect which month and year is shown.
  -c, --columns <number>    Number of month per row
  -A, --after <number>      Display the number of months after the current month.
  -B, --before <number>     Display the number of months before the current month.
  -3                        Display the previous, current and next month surrounding today.
  -h, --help                output usage information
```

