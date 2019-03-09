# Web scraping with Python

Notebooks and documentation for a 3.5-hour session at NICAR 2019 on using Python to scrape the web.

### Link to this repo: [bit.ly/nicar19-scraping](http://bit.ly/nicar19-scraping)

- [Session details](#session-details)
- [Other rad Python classes to check out at #NICAR19](#other-rad-python-classes-to-check-out-at-nicar19)
- [Running these notebooks at home](#running-these-notebooks-at-home)
- [Starting a new scraping project using this setup](#starting-a-new-scraping-project-using-this-setup)

## Session details

**When and where:** [Saturday, March 9, from 2:15 - 5:45 p.m. in Salon 3](https://www.ire.org/events-and-training/event/3433/4395/)

**Description:** If you need data that's trapped on a website, writing some code to scrape the page could be your solution. This entry-level class will show you how to use the Python programming language to harvest information from websites into a data file. We'll introduce you to the command line and show you how to write enough code to fetch, parse and analyze web content.

**Class objectives:** Learn enough Python to get started scraping unstructured or semi-structured information on the web into structured data that you can analyze for journalistic purposes.

**Quick intro presentation**: [bit.ly/nicar19-scraping-prez](https://bit.ly/nicar19-scraping-prez)

**What we'll cover:** Common use cases for scraping, a few best practices, some basic Python syntax, fetching HTML with the `requests` library, parsing HTML with the `beautifulsoup` library and writing data to file. If we have time, we'll also talk about scraping paginated data and a few other more complex tasks.

**What we won't cover, probably:** Scraping dynamically rendered pages, pages that require authentication or pages that otherwise require you to keep track of session information.

## Other rad Python classes to check out at #NICAR19

[PyCAR](https://www.ire.org/events-and-training/event/3433/4086/) runs Thursday and Friday mornings from 9 a.m. - 12:30 p.m. (This session requires pre-registration and an additional fee to save a seat.)

| Day | Class | Room | Time | Pre-registration required? |
| --- | ---- | ----- | ---- | :--------------------------: |
| Thursday | [Python: Machine learning and natural language processing](https://www.ire.org/) | Copper Cove | 9-10 a.m. | |
| Thursday | [Python 101: An overview for total beginners](https://www.ire.org/events-and-training/event/3433/4192/) | Salon D | 11:30 a.m. - 12:30 p.m. | |
| Thursday | [Python 1: The fundamentals](https://www.ire.org/events-and-training/event/3433/4239/) | Salon 5 | 2:15 - 3:15 p.m. | |
| Thursday | [Python 2: Intro to data analysis using pandas](https://www.ire.org/events-and-training/event/3433/4240/) | Salon 5 | 3:30 - 4:30 p.m. | |
| Thursday | [Python 3: Data cleaning and visualization](https://www.ire.org/events-and-training/event/3433/4241/) | Salon 5 | 4:45 - 5:45 p.m. | |
| Friday | [First Python notebook: Data analysis on deadline](https://www.ire.org/events-and-training/event/3433/4094/) | Coral Cove | 9 a.m. - 5:45 p.m. | ✅ |
| Friday | [Python: Let's Scrape a Website](https://www.ire.org/events-and-training/event/3433/4246/) | Copper Cove | 2:15 - 3:15 p.m. | |
| Saturday | [Python: Let's Scrape a Website (repeat)](https://www.ire.org/events-and-training/event/3433/4287/) | Diamond Cove | 9-10 a.m. | |
| Saturday | [Write better Python code](https://www.ire.org/events-and-training/event/3433/4087/) (BYO laptop) | Mariner Cove | 9 a.m. - 12:30 p.m. | ✅ |
| Saturday | [Python: Data visualization with Altair](https://www.ire.org/events-and-training/event/3433/4204/) | Copper Cove | 3:30-4:30 p.m. | |
| Saturday | [Python: Writing tests for your code](https://www.ire.org/events-and-training/event/3433/4234/) | Copper Cove | 4:45-5:45 p.m. | |
| Sunday | [Web scraping with Python](https://www.ire.org/events-and-training/event/3433/4093/) | Coral Cove | 9 a.m.- 12:30 p.m. | ✅ |
| Sunday | [Python 1: The fundamentals (repeat)](https://www.ire.org/events-and-training/event/3433/4284/) | Salon 5 | 9-10 a.m. | |
| Sunday | [Python 2: Intro to data analysis using pandas (repeat)](https://www.ire.org/events-and-training/event/3433/4285/) | Salon 5 | 10:15-11:15 a.m. | |
| Sunday | [Python: Basic mapping and GIS](https://www.ire.org/events-and-training/event/3433/4248/) | Copper Cove | 10:15-11:15 a.m. | |
| Sunday | [Python 3: Data cleaning and visualization (repeat)](https://www.ire.org/events-and-training/event/3433/4286/) | Salon 5 | 11:30 a.m. - 12:30 p.m. | |

## Running these notebooks at home

### Step 1: Install Python and some other tools

There are many ways to install Python and the tools you need to get up and running. [Here's how we suggest doing it](https://docs.google.com/document/d/1cYmpfZEZ8r-09Q6Go917cKVcQk_d0P61gm0q8DAdIdg/edit?usp=sharing). Please feel free to email me if you run into any problems: [cody@ire.org](mailto:cody@ire.org).

### Step 2: Download or clone this repo

If you have git set up already, navigate to your terminal or command prompt and run this command: `git clone https://github.com/cjwinchester/nicar-2019-scraping`

If you don't have git set up, you can download the repo as a zipfile [here](https://github.com/cjwinchester/nicar-2019-scraping/archive/master.zip) and unzip it. Make note of where the folder lives on your computer.

### Step 3: Install the tools you need

This step assumes that you have already installed the latest version of Python 3 and pipenv.

Open a terminal or command prompt and move into the folder you cloned or downloaded using the `cd` command.

(Not sure what a terminal or command prompt is? If you're on OSX, it'll be a program called Terminal, typically in Applications → Utilities → Terminal, or you can just Spotlight search for it. If you're running windows, the program is called `cmd` -- just click the Windows button and search for `cmd`.)

If your folder lives at `Desktop/nicar-2019-scraping`, you would run the command `cd Desktop/nicar-2019-scraping`. Replace everything after `cd ` with the actual path to the folder you cloned or downloaded.

Next, make sure you're in the correct directory. If you're on a Mac, run this command: `ls`. If you're on a PC, run this command: `dir`. This will list the contents of the directory you're in -- you should see a `Pipfile` and the other files you see [here](https://github.com/cjwinchester/nicar-2019-scraping).

Finally, install the libraries you'll need: `pipenv install`.

### Step 4: Run the notebooks

Once everything has installed, run this command: `pipenv run jupyter notebook`.

This should launch the notebook server in your browser, and your terminal should start spitting out a bunch of information about the server it's running.

Work in your notebooks. When you're done, you can close out of the browser tab. To quit the server in your terminal, hit `Ctrl+C`. That's it!

## Starting a new scraping project using this setup

This example assumes that you already have Python and pipenv installed and you want to use `jupyter`, `requests` and `beautifulsoup`.

Open your command-line interface and create a directory for your project files: `mkdir your-cool-project`

Now move into that directory: `cd your-cool-project`

Next, install your dependencies: `pipenv install jupyter requests bs4`

Once your dependencies are done installing, run your notebook server: `pipenv run jupyter notebook`.

Create a new Python notebook and then you're off to the races.