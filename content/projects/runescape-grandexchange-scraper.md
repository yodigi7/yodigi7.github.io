---
title: "Runescape Grandexchange Scraper"
description: "This project combines my love for Runescape, AI, and programming to analyze Grand Exchange trends. It features a pyQt GUI, a Runescape API web scraper, and AI algorithms built with sklearn to predict item price trends."
---

# Summary

When I was an avid Runescape player I enjoyed the idea of making gold off of "flipping" which was very similar to the way the stock market works.
This interest intersected with my love for AI, ML, and programming in general.
I decided to make a tool to make this easier with a custom GUI and a predictive AI in the background.
The first step was to create a web scraper sending rest requests to the Runescape API for item prices and store in the database for record keeping.
I then built a GUI using pyQt to display the database in a more user friendly way.
I then setup a few simple AI algorithms with sklearn to try to predict the future trend of the item but unsurprisingly did not do very well.

Link to project: https://github.com/yodigi7/runescape-grand-exchange-data-analytics

# Tech Stack

* python3
* sqlite3
* sklearn
* requests
* pyQt
