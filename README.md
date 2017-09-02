### You Need
These programs / packages:
* [Python 3.6.x](https://www.python.org/downloads/) (use 64-bit version if running on Windows 10)
* [Latest pandas](https://pandas.pydata.org/pandas-docs/stable/install.html)
* Chrome / Firefox / Safari with internet access

These files:
* leaderboard.html
* streak.html
* report.css
* report.js
* make_report.sh
* make_report_csv.py
* test_make_report_csv.py
* [reddit_posts_2016_09_week_1.csv.gz](https://storage.googleapis.com/data_interview/reddit_posts_2016_09_week1/reddit_posts_2016_09_week_1.csv.gz)

### Run
Put all the files within a ```.../9gag/``` directory, then:
* for macOS, in terminal do:
``` bash
$ cd .../9gag/
$ . make_report.sh
```
* for Windows, in cmd do (please wait for each command to finish):
```batch
> cd ...\9gag
> python make_report_csv.py
> python -m http.server
```

### View the reports

Once you see the following in cmd / terminal:
```
Serving HTTP on 0.0.0.0 port 8000 ...
```
Head over to
* ```localhost:8000/leaderboard.html``` for the leaderboard report.
* ```localhost:8000/streak.html``` for the submission streak report.

### Tests
Run
``` bash
python test_make_report_csv.py
```
