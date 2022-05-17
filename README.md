[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/it-works-why.svg)](https://forthebadge.com)

* ALPHA IS A PRE DEVELOPMENT BRANCH, DO NOT EXPECT USER FACING ISSUES TO BE ADDRESSED IN THIS BRANCH!


* Udemy Coupon Grabber & Course Enroller: Grab FREE Coupons!

Do you want to LEARN NEW STUFF for FREE? Don't worry, with the power of
web-scraping and automation, this script will find the necessary Udemy Coupons
&amp; enroll you to PAID UDEMY COURSES, ABSOLUTELY FREE!

**NOTE: THIS PROJECT IS NOT AFFILIATED WITH UDEMY.**

**NOTE: THIS PROJECT WILL NOT WORK WITH NON ENGLISH UDEMY.**

The code scrapes course links and coupons from:

 - [tutorialbar.com](https://tutorialbar.com)
 - [discudemy.com](https://discudemy.com)
 - [coursevania.com](https://coursevania.com)
 - [freebiesglobal.com](https://freebiesglobal.com) -> _New_



** **_Disclaimer & WARNINGS:_**

1. **Use** this ONLY for **Educational Purposes!** By using this code you agree
   that **I'm not responsible for any kind of trouble** caused by the code. **THIS PROJECT IS NOT AFFILIATED WITH UDEMY.**
2. **Make sure web-scraping is legal in your region.**
3. This is **NOT a hacking script**, i.e., it can't enroll you for a specific
   course! Instead it finds courses that provide coupon links to make the
   transaction free and then LEGALLY enroll you to the course!

---

** Requirements:

*** How to Install the Requirements?

**Required Python version:** [Python 3.8+](https://www.python.org/downloads/)

**(Windows users only) Required Microsoft Visual C++ 14.0+ version:** [Microsoft Visual C++ 14.0+](https://visualstudio.microsoft.com/visual-cpp-build-tools/)

![alt text](https://docs.microsoft.com/answers/storage/attachments/34873-10262.png)

**You must have pip or poetry installed. Please look up how to install them in your OS.**

Download a release of this project or clone the repository then navigate to the
folder where you placed the files on. Type `pip install -r requirements.txt` to
get all the requirements installed in one go. Similar instructions applies for poetry.

---

** Instructions

1 . Install from PyPI `pip install udemy-enroller`

-   Run the script and the cli will guide you through the settings required
-   If you decide to save the settings they will be stored in your home directory: <br>
    **Windows**:
    C:/Users/CurrentUserName/.udemy_enroller<br>
    **Linux**:
    /home/username/.udemy_enroller
    **The values in settings.yaml should be in the same language as the site you are browsing on**

2 . The script can be passed arguments:

- `--help`: View full list of arguments available
- `--browser=<BROWSER_NAME>`: Run with a specific browser 
- `--discudemy`: Run the discudemy scraper only
- `--coursevania`: Run the coursevania scraper only
- `--tutorialbar`: Run the tutorialbar scraper only
- `--freebiesglobal`: Run the freebiesglobal scraper only _[New]_ 
- `--max-pages=<NUMBER>`: Max number of pages to scrape from sites before exiting the script (default is 5)
- `--delete-settings`: Delete existing settings file
- `--delete-cookie`: Delete the cookie file if it exists _[New]_
- `--debug`: Enable debug logging


3 . Run the script in terminal with your target browser:

- `udemy_enroller --browser=firefox`
- `udemy_enroller --browser=chrome`
- `udemy_enroller --browser=chromium`

4 . The bot starts scraping the course links from the first **All Courses** page
on [Tutorial Bar](https://www.tutorialbar.com/all-courses/page/1), [DiscUdemy](https://www.discudemy.com/all), [Coursevania](https://coursevania.com) and [FreebiesGlobal](https://freebiesglobal.com) and starts
enrolling you to Udemy courses. After it has enrolled you to courses from the
first page, it then moves to the next site page and the cycle continues.

-   Stop the script by pressing ctrl+c in terminal to stop the enrollment process.

5 . _[New]_ At the end of process a detailed result is shown:

```
================== Run Statistics ==================

Enrolled:                   56
Unwanted Category:          0
Unwanted Language:          1
Already Claimed:            93
Expired:                    7
Total Enrolments:           1705
Savings:                    €2674.44
================== Run Statistics ==================
```
	

---

## FAQs

*** 1. Can I get a specific course for free with this script?

Unfortunately no, but let me assure you that you may be lucky enough to get a
particular course for free when the instructor posts its coupon code in order
to promote it. Also, over time you would build a library of courses by running
the script often and have all the required courses in your collection. In fact,
I made this course after completing a
[Python automation course](https://www.udemy.com/course/automate/) and selenium,
which of course I got for free! :)

*** 2. How does the bot work?

The bot retrieves coupon links from Tutorial Bar, DiscUdemy and Coursevania's lists to cut the prices and
then uses REST requests to authenticate and enroll to the
courses. Think of it this way: Epic Games & other clients like Steam provide you
a handful of games each week, for free; Only in this case, we need a coupon code
to make those courses free.

*** 3. How frequently should you run the script?

Daily, at least once! I've painstakingly amassed over 4000
courses in the last four years! And out of those 4000, I've only paid for 4 of
these courses.

So, a mere **0.001%** of courses are **actually paid** in my collection!
Thankfully, you can get more than what I gathered in 4 years, in a matter of
weeks! 🙌🏻

*** 4. Why did I create this?

It used to be my daily habit to redeem courses and it was an extremely tedious
task that took around 15 minutes, for 10 courses. And then I suddenly got the
idea to automate it, after I found the automation course mentioned above. I bet,
it will save your precious time too! :)

*** 5. The code compiles successfully, but it's taking too long to work! IS there any way to fix that?

Since we are heavily dependent on a third-party site to retrieve coupons links,
there may be issues when the site is down. Needless to mention the connectivity
issues too. If everything is working fine, you can see the courses being
retrieved in the Python console/shell, which may take a while.

*** 6. Which is the best way to run the script?

It is recommended to run the script using your terminal and system python.

*** 7. Which branch to commit against?

Pull request should be made on "develop" branch.

*** 8. What's the roadmap?

---

** Support & Maintenance Notice

By using this repo/script, you agree that the authors and contributors are under no obligation to provide support for the script and can discontinue it's development, as and when necessary, without prior notice.

---

** Supporters
