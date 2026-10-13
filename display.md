---
layout: boardlayout
title: airTEXT Display Board
---

# airTEXT Display Board

This is a simple webpage that can be shown on screens or incorporated in a webpage, the base URL is [airtext-jcd-display.onrender.com](https://airtext-jcd-display.onrender.com/).  The page shows forecast pollution episodes in the specified zone.  If there are no episodes forecast, informative screens are shown instead.

## Zone

Append **zone=<code>zone name</code>** to the query to show the pollution level
<code>Available values : Central London, North London, South London, East London, West London, Barnet, Bexley, Brent, Camden, Chelmsford, City of London, Colchester, Croydon, Ealing, Elmbridge, Enfield, Epsom and Ewell, Greenwich, Guildford, Hackney, Hammersmith and Fulham, Haringey, Harrow, Havering, Hillingdon, Hounslow, Islington, Kensington and Chelsea, Kingston upon Thames, Lambeth, Lewisham, Maldon, Merton, Mole Valley, Newham, Redbridge, Reigate and Banstead, Richmond upon Thames, Runnymede, Southwark, Spelthorne, Surrey Heath, Sutton, Tandridge, Tower Hamlets, Waltham Forest, Wandsworth, Waverley, Westminster, Woking<code>

e.g. <code>https://airtext-jcd-display.onrender.com/?zone=Southwark</code>

## Orientation

The image can be shown in either landscape or portrait, set **orientation=<code>landscape/portrait</code>**
<code>Available values : portrait, landscape<code>

**NOTE: Portrait shows the image rotated 90&deg; counter-clockwise.**

e.g. <code>https://airtext-jcd-display.onrender.com/?zone=Lambeth&orientation=landscape</code>

## Testing 

The [playground](display_playground.html) can be used to see the pages, including pages showing how they would look if there were pollution episodes.

## Further development


The code is open source, and can be found here [![GitHub Badge](https://img.shields.io/badge/GitHub-View%20Source-blue?logo=github)](https://github.com/CERCUK/airtext-jcd-display)

