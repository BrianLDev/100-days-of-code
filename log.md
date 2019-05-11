# 100 Days Of Code - Log

## Day 46: May 6, 2019 - Monday

**Today's Progress:**  
- Titanic Kaggle using ANN - Tweaking and testing the inputs to the ANN to see what impacts it

**Thoughts:**  
note - couldn't make it to ML bootcamp day 4 since I rented my car out on Turo.  

Made a few tweaks to the Titanic ANN inputs to see what affects the result.  Still not able to get results over 70% so will need to keep leaerning.

**Link(s) to work:**
1. [Titanic Kaggle using ANN - Tweaking and testing the inputs to the ANN to see what impacts it](n)

## Day 45: May 4, 2019 - Saturday

**Today's Progress:**  
*ML bootcamp - day 3 of 8*
- Intro to Deep Learning:
  - Titanic kaggle using artificial neural network (start)
  - Neural network strctures (perceptrons, neurons, etc)
- I completed the Titanic kaggle ANN using the Kaggle test data and submitted

**Thoughts:**  
Venkat switched up the agenda and instead of doing Advanced ML (time series, stock data, random forests), he skipped to Intro to Deep Learning.  Personally I was really looking forward to Advanced ML (time series, stock data, random forests) but will have to wait until next week.  

Artificial Neural Networks are very interesting and powerful and we barely scratched the surface here. Need to dive deeper in the future.  

Interestingly, the ANN only got 64% success rate on Titanic, where the simpler logistic regression previously got 74%.  Plan to tweak inputs and read about them to understand how to improve it.

**Link(s) to work:**
1. [Created repo for Titanic Kaggle](https://github.com/BrianLeip/Kaggle_Titanic)
2. [Titanic Kaggle using Artificial Neural Network (ANN) - In class model training, converted to Jupyter notebook](https://github.com/BrianLeip/Kaggle_Titanic/blob/d4def6e8eb4deb06e893f31d4cd97847fd1c9b0d/Titanic%20ANN%20v1%20(2019-BL).ipynb)
3. [Titanic Kaggle using Artificial Neural Network (ANN) - Ran ANN on Kaggle test data, submitted results](https://github.com/BrianLeip/Kaggle_Titanic/blob/dc2cf459fe6e9a3c11ee19f307ca4d7e26b3d779/Titanic%20ANN%20v1%20(2019-BL).ipynb)

## Day 44: May 3, 2019 - Friday

**Today's Progress:**  
*Hands-On ML Book*
- Updated README.MD, updated 01-NOTES.MD for improved formatting, nested lists

**Thoughts:**  
Light day - will have a bigger one tomorrow with ML bootcamp

**Link(s) to work:**
1. [Updated notes from ch 01 - Hands on ML book](https://github.com/BrianLeip/Hands_On_Machine_Learning/blob/e3db1e99b2a890cea1587d2d60d572c7839af3f8/01-The%20ML%20Landscape/01-NOTES.MD)

## Day 43: May 2, 2019 - Thursday

**Today's Progress:**  
*Hands-On ML Book*
- Read through chapter 1 and part of chapter 2
- Took notes on chapter 1 using markdown `01-NOTES.MD`
- Re-ran original source code from Ch 1 and part of Ch 2 in Jupyter notebook
- Started working through the CA Housing Price regression notebook from Ch 2

**Thoughts:**  
Still liking the hands on ML book as a more in-depth tie in with the ML Academy bootcamp.  But I'm not a big fan of the coding style so far.  Funny how someone can have such a readable and approachable and clean English writing style and then their coding style is less so.  

**Link(s) to work:**
1. [Took notes on ch 1, going through Jupyter notebooks from ch1 and 2](https://github.com/BrianLeip/Hands_On_Machine_Learning/blob/dcf8a62c11b8d449f14fd446808b2364995baab0/01-The%20ML%20Landscape/01-NOTES.MD)

## Day 42: May 1, 2019 - Wednesday

**Today's Progress:**  
*Hands On ML Book*
- Set up git repo and downloaded source code from official github
- Read Ch 1 and part of Ch2
- Took notes of important points in Chapter 1

**Thoughts:**  
This book is amazing...  Very readable, and packed with real life hands on applications of Machine Learning and Deep Learning.  Hands-On is always the way that I learn best so I'm going to continue working through this book during the weekdays (as time permits of course) and go through the in-class examples at the ML bootcamp, which is more of a surface level overview and interactive workshop compared to how deep and detailed the book is. They will be good complements to each other.

**Link(s) to work:**
1. [Hands On ML Book - Set up git repo and downloaded source code from official github, read Ch 1 and part of Ch2](https://github.com/BrianLeip/Hands_On_Machine_Learning/tree/715587fb98f9c10fd98eda28e1266f7d928202c1/00-handson-ml-master)
2. [Hands On ML Book - Notes from Chapter 1](https://github.com/BrianLeip/Hands_On_Machine_Learning/blob/715587fb98f9c10fd98eda28e1266f7d928202c1/01-The%20ML%20Landscape/01-NOTES.MD)

## Day 41: April 30, 2019 - Tuesday

**Today's Progress:**  
Figured out how to filter out large files (100MB+) from previous git commits

**Thoughts:**  
Github was giving me an error message when I pushed my previous commits including a large 100MB+ file to github, saying the file was too large.  Deleting it from the current folder and repo wasn't working because Git saves all historic files.  So I had 2 options: 
1. Revert to a previous commit and re-add the new files including a zipped version of the MNIST data.  The downside of this is that I would lose my commit history from 4/28
2. Filter out / prune that file from my commit history

After some google-fu and searching through Stack overflow, a few different solutions came up, and the one below was the best.

`git filter-branch --index-filter 'git rm -r --cached --ignore-unmatch <file/dir>' HEAD`

**Link(s) to work:**
1. [Figured out how to filter over large files (100MB+) from previous git commits - MNISTdata.csv](https://github.com/BrianLeip/ML_and_DL_Bootcamp_2019/tree/1b6aca805b9715cb2b1b613abf295eb71d2c6d5d/01-Intro%20to%20ML)
2. [Stack Overflow - How to remove large files from git commit history](https://stackoverflow.com/questions/19573031/cant-push-to-github-because-of-large-file-which-i-already-deleted)

## Day 40: April 28, 2019 - Sunday

**Today's Progress:**  
### Day 2 of 8 - ML and DL bootcamp
- In class walkthrough of the MNIST handwritten numbers / digits recognition and classification Jupyter Notebook
- Google Cloud Platform (GCP) Course 2: Module 1 - Completed

**Thoughts:**  
This was similar to what I covered in previous weekend course with ML Academy (I had done the 1st of 4 weekends, and then scheduling conflicts meant I had to complete the other 3 weeks later). 

MNIST handwritten number recognition done in class, but this was very surface level as well.  Will need to dig deeper during my "free time" to really understand everything.

We also ended up spending a lot of class time on starting the Google Cloud Platform certification course, which is a separate course that Venkatesh teaches and being heavily promoted by Google (I went to another meetup that granted free access to this course, $300 in free credits, etc).  While it's interesting and was cool to see our Housing Price prediction ML algorithm integrated into a web app, at the same time it felt like a distraction from the ML and DL course that we are actually focused on.  Venkatesh encouraged all of us to get GCP certified, which if I had the time I would do, but since time is a rare commodity these days I have to narrow my focus to only the core things I want to hone in on right now.  And that is ML and DL.  

**Link(s) to work:**
1. [MNIST Classification Jupyter Notebook (handwritten digit recognition) - Completed](https://github.com/BrianLeip/ML_and_DL_Bootcamp_2019/blob/61637fdf5eb5fed057ec6b518cb3cdbd1b07d517/01-Intro%20to%20ML/MNIST_Simple.ipynb)
2. [Architecting with Google Cloud Platform (GCP) Coursera Course - Course 2: Module 1 - Completed](https://www.coursera.org/learn/gcp-infrastructure-foundation/home/welcome)

## Day 39: April 27, 2019 - Saturday

**Today's Progress:**  
### Day 1 of 8 - ML and DL bootcamp
- We walked through the End to End Titanic Data Cleaning and ML Kaggle competition
- Unscrambled a version of the Titanic Jupyter notebook that had all steps in mixed up orders.  Challenge for class
- As a class we walked through the CA house price linear regression Jupyter Notebook

**Thoughts:**  
Most of this was review from the previous sessions that I've had with ML Academy and Venkatesh.  Where I left off last time was starting in on Housing Prices / MNIST handwritten digit recognition.  

The CA House price linear regression was most interesting to me, and unfortunately we only did a surface level overview of in in class.  But there is a book that Venkatesh used for this entire course that dives into this example in much more depth so I plan to do that when time permits.  Book is called [Hands-On Machine Learning with Scikit-Learn and TensorFlow: Concepts, Tools, and Techniques to Build Intelligent Systems](https://www.amazon.com/Hands-Machine-Learning-Scikit-Learn-TensorFlow-ebook/dp/B06XNKV5TS/) and it's wideley regarded as one of the best books out there to grok Machine Learning and Deep Learning.  As of today it's ranked 4.4/5 with 268 reviews on Amazon.  [The 2nd edition of Hands-On ML](https://www.amazon.com/Hands-Machine-Learning-Scikit-Learn-TensorFlow/dp/1492032646) is in the works and is expected to be released Aug 4, 2019.  I'll stick with the 1st edition for now and then wait for the Kindle edition.

**Link(s) to work:**
1. [End to End Titanic ML Kaggle competition - Completed ](https://github.com/BrianLeip/ML_and_DL_Bootcamp_2019/blob/3824bef06dda07fa61c39e45d7625fffc9d76050/01-Intro%20to%20ML/End_to_End_Titanic_(4).ipynb)
2. [Titanic unscramble challenge - Completed](https://github.com/BrianLeip/ML_and_DL_Bootcamp_2019/blob/3824bef06dda07fa61c39e45d7625fffc9d76050/01-Intro%20to%20ML/Titanic_Kaggle_Jumbled_Challenge.ipynb)
3. [CA house price linear regression in-class walkthrough - Completed](https://github.com/BrianLeip/ML_and_DL_Bootcamp_2019/blob/3824bef06dda07fa61c39e45d7625fffc9d76050/01-Intro%20to%20ML/CA_House_Pricing.ipynb)

## Day 38: April 26, 2019 - Friday

**Today's Progress:**  
Created git repo and folder structure for the upcoming Machine Learning and Deep Learning bootcamp (4 weekends)

**Thoughts:**  
Work has been rough lately with a few late nights, one to 4am, but with the upcoming ML and DL bootcamp coming up I'm excited to get back into coding.

**Link(s) to work:**
1. [Set up git repo and README.MD for upcoming ML and DL bootcamp](https://github.com/BrianLeip/ML_and_DL_Bootcamp_2019/tree/b3a7bc7cc406fcba48f702106d557ab6244e57b6)

## Day 37: April 17, 2019 - Wednesday

**Today's Progress:**  
Started Python for Financial Analysis and Algo Trading course:
06-Pandas With Time Series

**Thoughts:**  
Starting in on the Pandas w/ Time Series section.  Getting very busy with deadlines at work so won't have much time to work on this in the near future.

**Link(s) to work:**
1. [Python for Financial Analysis and Algo Trading 06-Pandas With Time Series - Started](https://github.com/BrianLeip/Python_For_Finance/tree/e68ad5c3731c6331ebffd77232b2ae679b30a326/06-Pandas-with-Time-Series)

## Day 36: April 15, 2019 - Monday

**Today's Progress:**  
Completed Python for Financial Analysis and Algo Trading course:
05-Data Sources

**Thoughts:**  
Quick section but a useful one to get access to free Python data sources that have stock data, housing data, Federal Reserve, etc.  2 main options: Pandas Datareader, and Quandl.  The Quandl Wiki EOD stock prices free data is no longer available so I'll use Pandas Datareader and access IEX for stock data instead.

**Link(s) to work:**
1. [Python for Financial Analysis and Algo Trading 05-Data Sources - Completed](https://github.com/BrianLeip/Python_For_Finance/tree/6ec4e21fc8b31f891a1eca63c74e71f4c0a6e0bf/06-Data-Sources)

## Day 35: April 13, 2019 - Saturday

**Today's Progress:**  
Completed Python for Financial Analysis and Algo Trading course:
04-02-Pandas Visualization

**Thoughts:**  
Good day, spent about 3-4 hours on this, taking detailed notes and practicing all the different Pandas data viz.  Area plots, box plots, scatter plots, hex bin plots. Different styles of data viz (personal favorite is 'seaborn-deep').  Colormap styles (favorite here is 'coolwarm').  Saving figures to files like JPG, PNG, and PDF.  And visualizing time series stock data.  Loved all of this and will be using this often in both work and personal.

**Link(s) to work:**
1. [Python for Financial Analysis and Algo Trading 04-01-Pandas Visualization - Completed](https://github.com/BrianLeip/Python_For_Finance/tree/abb8860b17a31bf0660bc86c9cbc0238da9390ae/04-Visualization-Matplotlib-Pandas/04-02-Pandas%20Visualization)
2. [Example of Area Plot with semi transparency, legend outside of figure, and saved to JPG](https://raw.githubusercontent.com/BrianLeip/Python_For_Finance/90f76ce1df5a869dcd5362d72bba2c23db170e00/04-Visualization-Matplotlib-Pandas/04-02-Pandas%20Visualization/AreaPlot.jpg)
---

## Day 34: April 12, 2019 - Friday

**Today's Progress:**  
Completed Python for Financial Analysis and Algo Trading course:
04-01-Matplotlib

**Thoughts:**  
Busy time at work with quarter end deadlines, not much time to code, but back at it now.  
Matplotlib is a universal data viz library for Python and this section barely scratched the surface.  The course focused too much on watching examples and not enough on actual coding which is where you actually learn, so I'll have to spend more time doing that on my own.

**Link(s) to work:**
1. [Python for Financial Analysis and Algo Trading 04-01-Matplotlib - Completed](https://github.com/BrianLeip/Python_For_Finance/tree/86950623fc5dbc09fc5a7ba2e3e01347232be136/04-Visualization-Matplotlib-Pandas/04-01-Matplotlib)
---

## Day 33: March 31, 2019 - Sunday

**Today's Progress:**  
Completed Python for Financial Analysis and Algo Trading course:
03-DataFrames

**Thoughts:**  
This was a big section compared to the previous 2 and I wanted to dive deep enough to really understand Pandas, and use all the methods, data imports/exports, data selction, .apply, lambda functions, and pivot tables.  Learned quite a bit and got great hands on experience. Going to continue practicing with Pandas, recreating Excel work in Pandas.

**Link(s) to work:**
1. [Python for Financial Analysis and Algo Trading 03 - Pandas - Completed](https://github.com/BrianLeip/Python_For_Finance/tree/89fe1a71a13c4870fa47c4dcce5929ac900c816f/03-%20General%20Pandas)
---

## Day 32: March 30, 2019 - Saturday

**Today's Progress:**  
Completed most of Python for Financial Analysis and Algo Trading course:
03-DataFrames

**Thoughts:**  
DataFrames are a super important part of Pandas (which is the Python version of Excel), so I want to know them inside and out until I can use Pandas as well or better than I've been able to use Excel over the 16 years using it.
I'm taking detailed notes in EverNote as I go along and want to find a lot of DataFrame challenges (online or in a book) to keep practicing.
Then the next thing I want to do is to take any work that I do in Excel, and recreate it in Pandas

**Link(s) to work:**
1. [Python for Financial Analysis and Algo Trading 03 - Pandas - Mostly completed](https://github.com/BrianLeip/Python_For_Finance/tree/a644e0dcb0b9e35951f31e58e20c5f30216bbb7b/03-%20General%20Pandas)
---

## Day 31: March 29, 2019 - Friday

**Today's Progress:**  
Started in on Python for Financial Analysis and Algo Trading course:
03-DataFrames

**Thoughts:**  
Been a busy week at work, working late (until 2am on Thu) but want to keep moving on this too.  
Starting in on DataFrames

**Link(s) to work:**
1. [Python for Financial Analysis and Algo Trading 03 - Pandas - Started](https://github.com/BrianLeip/Python_For_Finance/tree/12675c460d4abd7108c310aa58cf4e557660536e/03-%20General%20Pandas)
---

## Day 30: March 27, 2019 - Wednesday

**Today's Progress:**  
Completed another section and examples of Python for Financial Analysis and Algo Trading course:
02-NumPy

**Thoughts:**  
Cruising along and taking notes in Evernote as I go for future reference in Python, Numpy, and Pandas

**Link(s) to work:**
1. [Python for Financial Analysis and Algo Trading 02 - NumPy - Completed](https://github.com/BrianLeip/Python_For_Finance/tree/79507c031186126d19963db9623a68003d2f7e5d/02-NumPy)
---

## Day 29: March 25, 2019 - Monday

**Today's Progress:**  
Completed the first chapter and exercises for the Python for Financial Analysis and Algo Trading course.  01-Python Crash Course.  

**Thoughts:**  
After talking about all the different coding options with the guys at Py and Beer, I decided that my best and most relevant option at the moment is Python for Financial Analysis and Algo trading (Udemy course).  It's something that I actually started a while back and have been watching videos while I shower on my ipad, but this is a very hands on course and need to get my hands dirty in the code.  So far I'm actually really liking the course and going to keep rolling forward on it.

**Link(s) to work:**
1. [Python for Financial Analysis and Algo Trading 01 Python Crash Course - Completed](https://github.com/BrianLeip/Python_For_Finance/tree/master/01-Python-Crash-Course)
---

## Day 28: March 24, 2019 - Sunday

**Today's Progress:**  
Went to Py and Beer meetup with Connor and crew.  Talked about a few Python projects, met some people and created some repos for Python challenges and Python Cookbook.

**Thoughts:**  
More of a networking / social day than a pure coding one but important to have those every now and then and connect with other people that are getitng into coding Python.

**Link(s) to work:**
1. [Python Cookbook repo setup and sample code downloaded](https://github.com/BrianLeip/Python_Cookbook)
2. [PyBites Challenges repo set up and code downloaded](https://github.com/BrianLeip/PyBites_Challenges)
---

## Day 27: March 23, 2019 - Saturday

**Today's Progress:**  
Completed the last available challenges from Python Project night at Yelp - Beginner SIG.  String Manipulation, args and kwargs.

**Thoughts:**  
These were great challenges, and I learned quite a bit, even from fixing the small bugs that happened when Simeon rushed to create this for everyone.  String manipulation funcitons are important and ubiquitous so that was a great one. Using args and kwargs in functions to allow dynamic inputs is challenging for most people at first, so I made sure I did it multiple times to better understand it.

**Link(s) to work:**
1. [Python Beginner SIG - Redid basic logic: looping & iteration to use while and for loops](https://github.com/BrianLeip/2019-03-20_Python_Project_Night_Yelp/blob/396d96b43b47631a4b843d0ad3e1ee364cd10d67/basic_logic/looping_and_iteration.py)
2. [Python Beginner SIG - String Manipulation completed](https://github.com/BrianLeip/2019-03-20_Python_Project_Night_Yelp/blob/10f37f78f73c23f2f6b731ada26ff5bd1768c6ff/strings/string_manipulation.py)
3. [Python Beginner SIG - args and kwargs completed](https://github.com/BrianLeip/2019-03-20_Python_Project_Night_Yelp/blob/41fe060da35af3b73960695c594ee4ea9bc3422c/intermediate/args_and_kwargs.py)
---

## Day 26: March 22, 2019 - Friday

**Today's Progress:**  
Continued with Python Project night at Yelp - Beginner SIG.  Completed basic logic: looping & iteration

**Thoughts:**  
Completed this using the most efficient string methods I was aware of.  But realized after that Simeon's intention was to do it using while and for loops to improve understanding of loops, so I redid the functions using while and for loops.  Was more challenging to get the syntax to work right but gave me a better understanding.

**Link(s) to work:**
1. [Python Beginner SIG - Completed basic logic: looping & iteration](https://github.com/BrianLeip/2019-03-20_Python_Project_Night_Yelp/blob/396d96b43b47631a4b843d0ad3e1ee364cd10d67/basic_logic/looping_and_iteration.py)
---

## Day 25: March 21, 2019 - Thursday

**Today's Progress:**  
Continued with Python Project night at Yelp - Beginner SIG.  Completed basic logic: operators_and_if and indexing challenges (actually finished later that night on 3/20)

**Thoughts:**  
Loving these challenges.  Going to keep working through them all until I finish what Simeon has created so far (he's creating them on the fly and it's a WIP)

**Link(s) to work:**
1. [Python Beginner SIG - Completed basic logic: operators_and_if and indexing challenges](https://github.com/BrianLeip/2019-03-20_Python_Project_Night_Yelp/commit/efb84624ebebecacb3697404f18801b102d05096)
---

## Day 24: March 20, 2019 - Wednesday

**Today's Progress:**  
Python Project night at Yelp - Beginner SIG.  Set up repo, completed the 2 Gtting Started challenges - getting_started.py and basic_functions.py.

**Thoughts:**  
Jumping back in to 100 days of code after a break to focus on a major project at work.
Python Project night at Yelp - Went to the Beginner Special Interest Group (SIG) led by Simeon Franklin.  This was actually really good and a fresh, hands-on approach to learning code.  All interactive challenges are actual python programs that you run in terminal, and you create the functions that will make all the tests pass.  Paired up with a guy that was a little less familiat with github, git, and python than I am so it was also helpful to teach someone how to work through some of the challenges.  Like Richard Feinman says, "When 1 person teaches another, 2 people learn."

**Link(s) to work:**
1. [Python Beginner SIG - first 2 challenges completed](https://github.com/BrianLeip/2019-03-20_Python_Project_Night_Yelp/commit/ac326302726b21820c3f7b10048a3ecbf388ceed)
---

## Day 23: February 24, 2019 - Sunday

**Today's Progress:**  
Completed Kaggle's Data Cleaning Challenge day 5 of 5 - Inconsistent Data Entry

**Thoughts:**  
Another interesting and useful one.  Using fuzzywuzzy library to find similar text matches with fuzzy logic matching, and then replace incorrect spelling is going to be super useful in the future.  Save this one.

**Link(s) to work:**
1. [Data Cleaning Challenge Day 5 - Inconsistent Data Entry](https://github.com/BrianLeip/data_cleaning_Kaggle/blob/d3a3a51e515a81a43b1485c0bdd7a7a5912edbdc/Data%20Cleaning%2005-Inconsistent%20Data%20Entry.ipynb)
---

## Day 22: February 23, 2019 - Saturday

**Today's Progress:**  
Completed Kaggle's Data Cleaning Challenge day 4 of 5 - Character Encodings

**Thoughts:**  
This one was a little dull but important to know if data isn't loading properly and how to find and fix the encoding issue.

**Link(s) to work:**
1. [Data Cleaning Challenge Day 4 - Character Encodings](https://github.com/BrianLeip/data_cleaning_Kaggle/blob/fa8c525918026f92d2f1d8f963f24fd9ac2b78d4/Data%20Cleaning%2004-Character%20Encodings.ipynb)
---

## Day 21: February 20, 2019 - Wednesday

**Today's Progress:**  
Completed Kaggle's Data Cleaning Challenge day 3 of 5 - Parsing Dates

**Thoughts:**  
Another good one.  Save for future reference and practice on other data.

**Link(s) to work:**
1. [Data Cleaning Challenge Day 3 - Parsing Dates](https://github.com/BrianLeip/data_cleaning_Kaggle/blob/be3345c99b9cc21dfa18698c0fb66770bc5b4d64/Data%20Cleaning%2003-Parsing%20Dates.ipynb)
---

## Day 20: February 17, 2019 - Sunday

**Today's Progress:**  
Started and completed Kaggle's Data Cleaning Challenge day 2 of 5 - Scale and Normalize data

**Thoughts:**  
Missed a few days but won't let that deter me.
The scale and normalize data challenge was an excellent one and combined data cleaning, statistics, and data viz.  Save for future reference

**Link(s) to work:**
1. [Data Cleaning Challenge Day 2 - Scale and Normalize Data](https://github.com/BrianLeip/data_cleaning_Kaggle/blob/60baea302104c7ae04535b2550c104d891c7cc23/Data%20Cleaning%2002-Scale%20and%20Normalize%20Data.ipynb)
---

## Day 19: February 12, 2019 - Tuesday

**Today's Progress:**  
Completed Kaggle's Data Cleaning Challenge day 1 of 5 - Handling Missing Values.

**Thoughts:**  
Want to focus on improving my Data Cleaning and Pandas experience, this is a good and quick 5 day challege to facilitate that.

**Link(s) to work:**
1. [Data Cleaning Challenge Day 1 - Hangling Missing Values](https://github.com/BrianLeip/data_cleaning_Kaggle/blob/master/Data%20Cleaning%2001-Handling%20Missing%20Values.ipynb)
---

## Day 18: February 11, 2019 - Monday

**Today's Progress:**  
Made a lot of progress on my Kaggle Petfinder notebook. Laid out structure of the notebook with all 7 steps of the Machine Learning Process, completed 3 of them, and working on step 4 - Feature Engineering and Data Cleansing.

**Thoughts:**  
Got back on the wagon today and cranked out a couple hours worth of work.  Feels good and want to keep the streak going again.

**Link(s) to work:**
1. [Big update to Petfinder Notebook - completed steps 1-3 and working on step 4](https://github.com/BrianLeip/Kaggle_Petfinder/blob/7fa37f3e17379641a31f4f1d9996ca83189ea596/Petfinder_Kaggle.ipynb)
---

## Day 17: February 8, 2019 - Friday

**Today's Progress:**  
more EDA on the Petfinder DataSet

**Thoughts:**  
Busy but moving forward

**Link(s) to work:**
1. [more EDA on the Petfinder DataSet](https://github.com/BrianLeip/Kaggle_Petfinder/blob/6499e453530d0d178b8b3a2b7a180a5fed23589b/Petfinder_Kaggle.ipynb)
---

## Day 16: February 6, 2019 - Wednesday

**Today's Progress:**  
some EDA on the Petfinder DataSet

**Thoughts:**  
Busy but moving forward

**Link(s) to work:**
1. [some EDA on the Petfinder DataSet](https://github.com/BrianLeip/Kaggle_Petfinder/blob/d3c690049f0f1f7d11b85e55a13cf9304d6d0371/Petfinder_Kaggle.ipynb)
---

## Day 15: February 5, 2019 - Tuesday

**Today's Progress:**  
Unemployment TimeSeries viz-added filters

**Thoughts:**  
Busy but moving forward

**Link(s) to work:**
1. [Unemployment TimeSeries viz-added filters](https://github.com/BrianLeip/TableauAtoZ/commit/90e3ec586556bd7c71b4b0fb63dda5dc55b75495)
---

## Day 14: February 3, 2019 - Sunday

**Today's Progress:**  
Tried getting the Kaggle API set up with Google Colab but there were a lot of issues with the kaggle.json credentials file and Googling that issue shows that almost everyone has problems with it.  Changed to instead use Dropbox and github, but remove the image DataSets since those are the largest by far.  Got it working and now can successfully use both Github and Colab by downloading the files from my Dropbox folder.

**Thoughts:**  
It was a frustrating day getting this set up and wish I could have spent that time coding.  But now that the setup part is done, future days can be spent analyzing the datasets and doing ML.

**Link(s) to work:**
1. [Kaggle Petfinder folder with DataSets - images excluded](https://github.com/BrianLeip/Kaggle_Petfinder/tree/d72238cbeded1c0fd45f3313795238c8c25851d2/DataSets)
---

## Day 13: February 2, 2019 - Saturday

**Today's Progress:**  
Set up Colab notebook for the Kaggle petfinder competition that I'm planning to tag team with a coder I met on Twitter. Tried to push the DataSet to github but it's too big.

**Thoughts:**  
The DataSet was too big to sync to github, so I also looked into other ways to make this work - possibly use the Kaggle API?

**Link(s) to work:**
1. [Kaggle Petfinder Colab](https://colab.research.google.com/drive/14oaWM71SXiiOWr-2ncHZlH4AwBTSlrtU)
---

## Day 12: February 1, 2019 - Friday

**Today's Progress:**  
Completed Tableau AtoZ section 03 - Time Series, Aggregation using Unemployment statistics.

**Thoughts:**  
This was an important one for me since I work with a lot of stock data which is considered time series data.  Will continue to play around and experiment with it to continue improving.

**Link(s) to work:**
1. [Tableau AtoZ 03 - Time Series, Aggregation using Unemployment statistics](https://github.com/BrianLeip/TableauAtoZ/commit/a4c8cdf9ca3c3df5cdf70f1202da6b7bb10fa647)
---

## Day 11: January 31, 2019 - Thursday

**Today's Progress:**  
Continued Tableau AtoZ course - Downloaded all course DataSources and instructor vizzes, created folder structure, then started on section 3.

**Thoughts:**  
Relatively short day but making progress every day

**Link(s) to work:**
1. [Downloaded all DataSets and instructor vizzes for the course, started on section 3](https://github.com/BrianLeip/TableauAtoZ/commit/ad0ec494f41c6101420ab40630e4e1a2e4458ae7)
---

## Day 10: January 30, 2019 - Wednesday

**Today's Progress:**  
Back to the Tableau A to Z course since it will be crucial to my new job.  Completed 02-Business Challenge - Sales by rep by region data viz. *

**Thoughts:**  
I haven't heard back from my Kaggle petfinder partner in a bit, and since Data Viz (Tableau especially) is going to be crucial in my new job, I'm focusing my attention on that.  Really love the program and the Udemy course too, going to keep moving on this and finish as fast as possible and then jump back to Kaggle and Machine Learning.

**Link(s) to work:**
1. [Tableau AtoZ 02-Business Challenge - Sales by rep by region](https://github.com/BrianLeip/TableauAtoZ/commit/0eeb9bb6cce21ae74b154ad8015bc42b778ce21d)
---

## Day 09: January 29, 2019 - Tuesday

**Today's Progress:**  
Busy day but I connected with a fellow coder doing 100 Days of code on Twitter who is taking on the Kaggle Pet Finder pet adoption challenge.  Joined the challenge, downloaded the data and started digging in.

**Thoughts:**  
I have a lot going on with my new job, but want to keep pushing forward on 100 Days of Code as much as possible. Also it's fun to collaborate with someone else on a Kaggle competition and even though it involves some things that are more complex (natural language processing, sentiment analysis, image recognition, etc.), sometimes the best way to learn is to get in a little over your head and force yourself to figure it out.

**Link(s) to work:**
1. [Started the Kaggle Petfinder competition](https://github.com/BrianLeip/Kaggle_Petfinder/commits/master)
---

## Day 08: January 27, 2019 - Sunday

**Today's Progress:**  
Day 2 of Intro to Machine Learning Bootcamp.  
- Delved into ML statistics, linear regressions, recapped confusion matrix.
- Completed the ML Outline (Titanic reshuffle) where all the key Titanic linear code lines are shuffled in the wrong order.  Re-order them in the correction sections of the 7 step Machine Learning process
- K Means clustering
- MINST handwritten number image recognition

**Thoughts:**  
Good day, much better than day 1.  But a lot of the topics we covered are quite deep and will require some deep dives in the future to truly grok everything.

**Link(s) to work:**
1. [ML Outline (Titanic Reshuffled)](https://github.com/BrianLeip/Intro_to_ML_Bootcamp_2019-01-26/blob/426e308406f15bd6ee1b8e6cd75348d8d84f5a89/ML%20Outline%20(Titanic%20reshuffle).ipynb)
2. [K Means Clustering](https://github.com/BrianLeip/Intro_to_ML_Bootcamp_2019-01-26/blob/4f5633556df0970a307aff71c897823a74f58bc1/K%20Means%20Clustering.ipynb)
3. [MINST - handwritten number image recognition](https://github.com/BrianLeip/Intro_to_ML_Bootcamp_2019-01-26/blob/4b651d347af2156b9fef1ba6c74cdd0392fd0172/MNIST%20-%20Simple.ipynb)
---

## Day 07: January 26, 2019 - Saturday

**Today's Progress:**  
Day 1 of Intro to Machine Learning Bootcamp.  Covered Python, Pandas, and Linear Regression confusion matrix in the AM.  Titanic (again) from 12pm to 2pm. Housing price prediction from 2pm to 4:30pm.

**Thoughts:**  
Unfortunately I've already learned most of this at the other meetup and weekend bootcamp.  This wasn't the best or most focused course I've taken yet, hopefully tomorrow will be better.

**Link(s) to work:**
1. [Intro to ML day 1 files: PDF about ML, Mini Titanic Jupyter notebook, Housing price prediction notebook](https://github.com/BrianLeip/Intro_to_ML_Bootcamp_2019-01-26/commit/d6bd142b0e16a92169f8241b07cdf2f40d23d138)
---

## SKIPPED: January 25, 2019 - Friday
Busy day at work at the new job and then after work event to welcome new hires until midnight.

---

## Day 06: January 24, 2019 - Thursday

**Today's Progress:**  
Tableau A to Z - 2nd data set - business challenge

**Thoughts:**  
Short one today, was very busy with work

**Link(s) to work:**
1. [Tableau - Business Challenge - dataset](https://github.com/BrianLeip/TableauAtoZ/commit/c336b61aa8a6d4f07c94fe397d2974dba910e905)
---

## Day 05: January 23, 2019 - Wednesday

**Today's Progress:**  
Started Tableau A to Z (Data Visualization) course on Udemy.  Installed Tableau, downloaded first data set and created first dat Viz.

**Thoughts:**  
I'm really enjoying this so far and Tableau / Data Viz in general will be hugely important at my new job and for personal projects in the future.

**Link(s) to work:**
1. [Tableau - SuperStore exercise - dataset and viz](https://github.com/BrianLeip/TableauAtoZ/tree/master/01-SuperStore%20Exercise)
---

## Day 04: January 22, 2019 - Tuesday

**Today's Progress:**  
Created Titanic v5 which removes all items that require the internet (e.g. !wget) over to a Jupyter notebook that pulls the data from the Titanic folder.  The new version will also work with Google Colab so it's cross compatible.  Now an internet connection is no longer required and can be worked on at anytime including while I ride the train.  Also looked into potential visualizations for the linear regression covariable weights, and started coding one.  Will need to finalize in the future.

**Thoughts:**  
Today was my first day starting my role as Controller at Sentieo.  So with that being my primary focus, I only was able to spend about 30 minutes coding while I was on the train commuting to/from work, and a bit after I got home.

**Link(s) to work:**
1. [Titanic v5 - no longer requires internet and Google Colab](https://github.com/BrianLeip/PythonMLBootcamp2019-01-19/blob/master/Titanic/Titanic%20(2019-BL)%20v5.ipynb)
---

## Day 03: January 21, 2019 - Monday

**Today's Progress:**  
Updated the Titanic Jupyter notebook - created a section that displayed the weights given to each of the features in the linear regression formula, sorted by the largest impact.  By far, being a man is the #1 way to die if you are on a sinking ship.  

**Thoughts:**  
Quick one today, but an important one.  by seeing the actual weights associated with each feature, that gives me clues on how to improve the model in the future.  Next I would like to create a visual for those weights using either matplotlib or seaborn, and then take steps to improve my prediction above 75%

**Link(s) to work:**
1. [Titanic v4 - display weights of linear regression, sorted by biggest impact (section 5)](https://github.com/BrianLeip/PythonMLBootcamp2019-01-19/blob/master/Titanic/End_to_End_Titanic%20(2019-01)%20BL%20Updates%20v4.ipynb)
---

## Day 02: January 20, 2019 - Sunday
*NOTE - I'll be writing quick notes from here on out. The focus of 100 days of code is on the code, not the daily log, so most of my time and energy will be focused accordingly.*

**Today's Progress:**  
Completed day 2 of 2 of the Python for Data Science bootcamp. Submitted my first Kaggle competition (Titanic)! 75% accurate, would like to get 80% or above in the future. Improved on Venkatesh's original version by using the mean age for each Pclass to fill in any null values, instead of a fixed 28.  Also learned more about Pandas.

**Thoughts:**  
Excited to have completed my first Kaggle competition from start to finish.  Will be taking on more in the future and challenging myself to score higher and build my Kaggle ranking.

**Link(s) to work:**
1. [Completed Kaggle Titanic v3 - Jupyter notebook](https://github.com/BrianLeip/PythonMLBootcamp2019-01-19/blob/9e50c88ed0d8874c1859a3dcdec19134c48159df/Titanic/End_to_End_Titanic%20V3-BL%20Updates%20(2019-01).ipynb)
2. [10 Minutes to Pandas - Jupyter Notebook](https://github.com/BrianLeip/PythonMLBootcamp2019-01-19/blob/9e50c88ed0d8874c1859a3dcdec19134c48159df/Pandas/10-minutes-to-pandas.ipynb)
---

## Day 01: January 19, 2019 - Saturday
**Today's Progress:**  
Jumping back into 100 Days of Code and 100 Days of ML Code.  Going to spend the 100 days focused on HANDS-ON (avoid videos when possible) Machine Learning, Data Science, and Data Visualization.

Completed day 1 of 2 on the Python for Data Science bootcamp - hosted on the Google campus in Mountain View and taught by Venkatesh Tadinada.  9am through 4:30pm.  For the most part, this was almost the same as the previous Meetup I had with him where he did a walkthrough of the Titanic Kaggle competition and his in depth Jupyter/Colab notebook for each step.  In addition, he did some Python tutorials and some Pandas as well.  It was a good refresher, and I pushed myself to dig deeper into the steps, modifying things along the way like filling the NaN items in the 'Age' feature with the mean instead of a fixed number, and then attempting to sub-fill them by taking the mean for each class 1, 2, 3.  Ran into an pandas error on the complex nested formula that it was referencing a copy of the data and not updating the original.  Since day 2 of the bootcamp is for Pandas, I'm going to hold off until tomorrow and revisit.  

Venkatesh put a challenge to the group that if any of us could go to Hacker Rank, complete the following data type challenges: easy-all, medium-a few, hard-one.  If we do that, he'll give us 50% off a future ML/DS course which I am interested in.  The ML one next weekend is normally $300 so that would save $150.  Jumping on to HackerRank now and will chip away until it's time to sleep.

**Thoughts:**  
Feels great to be getting back into 100 days of coding and being surrounded by smart, motivated people all wanting to do the same.  Time has been and always been the biggest challenge to keeping the streak going, and I expect it will likely be my biggest challenge when I start my new job on Tuesday.  But as much as I'm able, I'm going to keep this going.

**Link(s) to work:**
1. [Python - Folder of Jupyter notebooks](https://github.com/BrianLeip/PythonMLBootcamp2019-01-19/tree/9e50c88ed0d8874c1859a3dcdec19134c48159df/Python)
2. [Titanic Kaggle competition notebook - starting point v2](https://github.com/BrianLeip/PythonMLBootcamp2019-01-19/blob/9e50c88ed0d8874c1859a3dcdec19134c48159df/Titanic/End_to_End_Titanic%20V2%20(2019-01).ipynb)
---
