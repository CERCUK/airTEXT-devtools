---
layout: boardlayout
title: airTEXT Display Board
---

# Displaying airTEXT Forecasts on Digital Signage

## Overview

The Air Quality Forecast service can be integrated with compatible digital signage systems to display timely, locally relevant public health information in GP surgeries, pharmacies, hospitals, community centres and other public spaces.

The service provides a URL for a selected geographical zone. Based on the forecast conditions for the next two days, the URL automatically displays the most appropriate information screen.

Where moderate or higher air pollution or pollen levels are predicted, the service displays a screen relevant to the forecast level, including guidance on appropriate actions and precautions.

Where all forecast levels remain low, a general information screen is displayed instead.

This allows screens to present relevant, actionable health information when it is needed, without requiring staff to monitor forecasts or manually change the displayed content.

## URL

**Base URL:** [airtext-jcd-display.onrender.com](https://airtext-jcd-display.onrender.com/)

The display is configured using URL query parameters, allowing the geographical zone and screen orientation to be specified.

### Zone

Use the <code>zone</code> query parameter to select the geographical zone for which the forecast infromation should be displayed

#### Example:

<code>https://airtext-jcd-display.onrender.com/?zone=Southwark</code>

#### Available values

<code>Central London, North London, South London, East London, West London, Barnet, Bexley, Brent, Camden, Chelmsford, City of London, Colchester, Croydon, Ealing, Elmbridge, Enfield, Epsom and Ewell, Greenwich, Guildford, Hackney, Hammersmith and Fulham, Haringey, Harrow, Havering, Hillingdon, Hounslow, Islington, Kensington and Chelsea, Kingston upon Thames, Lambeth, Lewisham, Maldon, Merton, Mole Valley, Newham, Redbridge, Reigate and Banstead, Richmond upon Thames, Runnymede, Southwark, Spelthorne, Surrey Heath, Sutton, Tandridge, Tower Hamlets, Waltham Forest, Wandsworth, Waverley, Westminster, Woking</code>

### Orientation

Use the orientation query parameter to specify the display orientation.  If this omitted it will show in landscape.

#### Example:

<code>https://airtext-jcd-display.onrender.com/?zone=Lambeth&orientation=portrait</code>

#### Available values

<code>portrait, landscape</code>

**NOTE:** Portrait shows the image rotated 90&deg; counter-clockwise.

## Using the display with digital signage
The display URL can be added to a compatible digital signage system as a web page or browser-based content item.

- Select the required geographical zone.
- Construct the URL using the appropriate query parameters.
- Add the URL to the signage platform's content playlist.
- Configure the duration and refresh behaviour according to the platform's capabilities and the service's requirements.
  
The display can then run alongside other content in the screen rotation. The service determines which information screen to show based on the forecast, so staff do not need to select individual pollution or information screens manually.

Digital signage platforms differ in their support for external web pages. Check that the chosen platform can display externally hosted web content before deployment.

## Testing and previewing

The [playground](display_playground.html) can be used to see the pages, including pages showing how they would look if there were pollution episodes.

Use the playground to review the appearance of the content before configuring a live digital signage installation.

## Further development

The code is open source, and can be found here 
[![GitHub Badge](https://img.shields.io/badge/GitHub-View%20Source-blue?logo=github)](https://github.com/CERCUK/airtext-jcd-display)

