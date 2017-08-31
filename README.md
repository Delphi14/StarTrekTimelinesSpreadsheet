# Star Trek Timelines Spreadsheet Tool
A tool to ease with crew management in Star Trek Timelines

**DISCLAIMER** This tool is provided "as is", without warranty of any kind. Use at your own risk! Make sure you read and understand [Disruptor Beam's Terms of Service](https://www.disruptorbeam.com/tos/). Star Trek Timelines content and materials are trademarks and copyrights of [Disruptor Beam](https://www.disruptorbeam.com/games/star-trek-timelines/); I have no affiliation with Disruptor Beam or any of its partners.

## Install and run the tool

I recommend you install the development environment and play with the source code yourself; make improvements and submit PRs to help your fellow players!

However, if you're only interested in installing and running the tool, head on to the [releases](https://github.com/IAmPicard/StarTrekTimelinesSpreadsheet/releases) page and pick a recent release to install.

## Features

### Crew management

![Screenshot tool](/Screenshot-Tool.png "Tool screenshot")

The first tab lets you manage your crew. You can sort by various fields, (un)group by rarity as well as export the data in Excel or plain CSV formats.

### Item management

![Screenshot Items](/Screenshot-Items.png "Items screenshot")

This tab lists out all the items you currently have, along with their quantity and type.

### Missions

![Screenshot Missions](/Screenshot-Missions.png "Missions screenshot")

This tab give an overview of all accepted missions, along with individual requirements and player stats for each quest and challenge.

### Cadet challenges

![Screenshot Cadet](/Screenshot-Cadet.png "Cadet screenshot")

Similar to the Missions tab, but for cadet challenged.

### Crew recommendations

![Screenshot CrewRecommendations](/Screenshot-CrewRecommendations.png "CrewRecommendations screenshot")

*Work in progress!*

This tab will make recommendations about which crew you can freeze or airlock, and which you need to keep in your active roster, primarily for cadet challenges.

### Gauntlet

![Screenshot Gauntlet](/Screenshot-Gauntlet.png "Gauntlet screenshot")

In this tab you can get recommendations for which crew to use in your next gauntlet (if you didn't already start it). Please see source code for details, the algorithm is still "hand-wavy" at this point and could use input from someone more experienced with statistic analysis.

## Get an access token
First, you need to obtain an access token. If you're running on a Windows PC, install the free Star Trek Timelines [Steam application](http://store.steampowered.com/app/600750/Star_Trek_Timelines/), then open it at least once to log in.

If you're not running on a Windows PC or don't want to install the Steam application, you can use the Facebook application through your browser. Please follow the steps below for obtaining an access token:

1. Open Chrome and hit F12 and switch to the Network tab in the debug pane that opens
2. Now navigate to [Star Trek Timelines](https://apps.facebook.com/sttimelines) on the page and wait until you get the "Play >>" link
3. Back in the debug page, enter "stt.disruptorbeam.com/player" in the Filter input. Select the first item in the list of requests.
4. On the right, you should see something like this:

![Screenshot](/screenshot.png "Screenshot")

5. Copy the access_token, which should be in this format: "123e4567-e89b-12d3-a456-426655440000"

*NOTE*: you need to repeat this process about once every 2 weeks, as the access token expires after a set period of time.

## Command line version of the tool
**NOTE:The command line version of the tool is deprecated, all new development happens in the GUI version!**


[See details here for the command line version of the tool](CLI.MD)

## GUI version of the tool
[See details here for the GUI version of the tool](gui/README.md)
