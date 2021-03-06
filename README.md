## Description
Calendar extension for integration of external calendars with [iCalendar-format](https://en.wikipedia.org/wiki/ICalendar).

This module has **only been tested** in **Humhub v1.2.3 and v1.2.4** with the **calendar module version 0.6.3**!

**Be careful!**
some calendars are not intended for permanent synchronization. These do not send a "last_modified" timestamp. Please do not select the option `auto sync hourly` for these. It could slow down your system..

## Installation
First you have to activate the original calendar module for humhub.
The external_calendar module only works if it is activated!

copy this module to the modules-folder and activate the module in the admin menu.

By default, this module prevents the calendar events from being posted to the stream. You can change this by editing the settings in the admin area:
> administration->module->calendar extension->configuration


If you want to add external calendars, go to a specific space (or your own profile), activate the external_calendar module in the space settings (or profile settings) and start the configuration of the module here.

**If there is an error, something went wrong with your sync.**


*Hints*:
- When you try to add an external calendar, the module first checks whether the URL you added is correct and can be converted to an iCal file.
**Therefore you need a url with** `http://` or `https://`
For example:
```
Wrong: webcal://calendar.google.com/calendar/ical/....
Right: https://calendar.google.com/calendar/ical/...
```
## Informations
This module is in Beta and not tested with other external calendars than google (private) and mep24!
Please help to find a solution for the ["upcoming-events"-issue](https://github.com/staxDB/external_calendar/issues/1).
- only translated in german

## Tested Calendars
- Google Calendar ([private adress](https://support.google.com/calendar/answer/37648?hl=en) only)
- [MEP24 Calendar](https://www.mep24software.de/kalender-freigeben/)

__Module website:__ <https://github.com/staxDB/external_calendar.git>    
__Author:__ David Born    

## Changelog
<https://github.com/staxDB/external_calendar/commits/master>

## Bugtracker
<https://github.com/staxDB/external_calendar/issues>

## ToDos
- fix bug with calendar-widget "upcoming events"
- test other calendars than google (only private link tested)
- async delete / add / update events
- add more translations


This Module uses the Calendar UI Interface in v0.6 - [see dokumentation](https://github.com/humhub/humhub-modules-calendar/blob/master/docs/interface.md)
