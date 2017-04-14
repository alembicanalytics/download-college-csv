## arguments:
* -v, --verbose : to run in the verbose mode (debug logger)
* -c, --college : pass in the college id. e.g. -c 1,2 - scrape college no 1 and college no 2.

To scrape all colleges pass in: 
**-c all** or don't do **-c** at all
</br>
How to get college ids, it's as simple as running the script with this argument:
**--print-college** or **-p**
</br>
* -s, --screen-capture : to save a screenshot of the browser before the csv file is downloaded
* -p, --print-college : to print all available colleges with their ids. ids are used to pass as an argument when we want to
scrape only a specific college.
* -r, --retry : to set how many times the script will retry to scrape/download data. by default is set to 3.

## Installation
* https://www.python.org/downloads/release/python-2713/
* run command line as administrator: **pip instal -U selenium**

## Examples:
``` python run.py -l -r 10 -v -s``` - scrape all colleges, log into a file in the verbose mode, 
retry up 10 times to scrape data and save a screencap right before the export to csv is cliked upon
</br>
```python run.py -c 15``` - scrape the college with an id of 15
</br>
```pyton run.py -print-college -l``` - open up the url, get the list of all colleges and print it out
