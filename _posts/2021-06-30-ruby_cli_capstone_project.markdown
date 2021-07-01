---
layout: post
title:      "Ruby CLI Capstone Project"
date:       2021-07-01 01:26:37 +0000
permalink:  ruby_cli_capstone_project
---


Dungeons & Dragons is a big passion of mine, and trying to find online games to play it during the pandemic was a big time sink for me. So when the opportunity arose to create a CLI that scrapes a website for data on mutliple levels, my mind immediately went to Roll20 and how a Ruby gem could make the process of looking so much easier.

However, once the time came to do the project, I ran into several obstacles. This is supposed to be the first big milestone in my course and I wanted to make sure I could devote the appropriate amount of time and do it right. Life had other ideas: my wife got a new job; I quit my job to devote all my time to this career change; and my daughter was finishing her school year.

So what was supposed to be a project given its due, instead turned into a projects of fits and starts. A few lines here, some outlining there. Three weeks after starting my outline, I was finally able to devote the hours necessary to get the project started in earnest.

My first step was outlining how the program would flow for the user:
* Greet the user;
* Scrape the initial Roll20 listing page;
* While scraping that top layer, follow each game's link to its full page and scrape the additional information;
* List the games in numerical order;
* Allow the user to select a game by number;
* Display the selected game's full information;
* Allow the user to re-access the list, or quit out.

Due to the long delays between my availability to code around work, every time I sat back down, I felt like I had to restart and rewrite almost all of it--what was originally logical and concise became unwiedy and obtsue on review. Once I could finally sit down for several days for several hours each, I found myself getting into a rhythm that allowed me to better see how the CLI class's overall structure should mirror its basic `call` method. I was also able to get rid of an extra class and pare down the `scraper` class to one method that instatiated a new instance of `meetup`. 

Then it came down to the actual scraping and formatting. Two of my favorite success were in this step. First, formatting the time and date from UNIX to a readable form took some research and finangling, but turned out simpler than I though. The second success was getting a deeper understanding of how the CSS selectors worked, specifically using `[#]` following a selector to choose a specific child, when that child did not have any unique selectors.

All-in-all I am happy with this program. There is likely some repitition that could be eliminated, so I am looking forward to my review session to get some tips and feedback to make it even better.
