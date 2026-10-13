---
layout: boardlayout
title: airTEXT Display Board
---

# airTEXT Display Board [![GitHub Badge](https://img.shields.io/badge/GitHub-View%20Source-blue?logo=github)](https://github.com/CERCUK/airtext-jcd-display)

This is a simple display board that shows the airTEXT forecast for the next 24 hours. It is designed for a JCDecaux Roadside Digital 6-sheet display board (1080 x 1920), but can be used in any setting that supports HTML and JavaScript.

[URL](https://airtext-jcd-display.onrender.com/)

The [playground](display_playground.html) can be used to see the results

## Zone

Append zone=<zone name> to the query to show the pollution level

e.g. https://airtext-jcd-display.onrender.com/?zone=Southwark

## Orientation

The image can be shown in either landscape or portrait, set the orientation=<landscape/portrait>

e.g. https://airtext-jcd-display.onrender.com/?zone=Lambeth&orientation=landscape

## Testing 

Append `dummy=[scenario]` to the URL to test the different scenarios. The following scenarios are available:

- `normal` (i.e. low pollution and low pollen)
- `veryHighPollutionToday`
- `highPollutionToday`
- `moderatePollutionToday`
- `veryHighPollenToday`
- `highPollenToday`
- `moderatePollenToday`
- `highPollutionTomorrow`
- `moderatePollutionTomorrow`

Append `?dummy=normal&info=[template]` to the URL to test the different info templates. The following templates are available:

- `subscription-actionable`
- `subscription-reflexive`
- `educational`

