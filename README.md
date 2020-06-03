
# Twitter Covid-19 UnBDC2020
**Contributors**: Stuart Martin, Jenney Ren, Riju Sikdar, Joyce Li

## Introduction
As the COVID-19 pandemic continues to ravage the globe, many political leaders are encouraging or enforcing social distancing to limit the spread of the virus. In the United States, social distancing is largely voluntary. As such, public opinion on the necessity of self-isolation directly affects the number of COVID-19 cases in the area.

In our best interest, our study uses sentiment analysis on state governors’ Tweets to determine whether communications vary between Republican and Democrat governors. We used open resources such as [Twitter Developer Labs](https://developer.twitter.com/en) and [Python 3](https://www.python.org/download/releases/3.0/), to collect all governor Tweets throughout the pandemic and perform automated sentiment analysis.

## Methodology
Tweets were only collected between March 13, 2020 and May 30, 2020. From the gathered data, the total Tweets made per day was calculated and plotted on a bar graph. A word cloud was made for each governor to show typical keywords and the importance of each word used by the governor. To evaluate the overall sentiment of the governor’s Tweets, a bar graph that showed the number of positive, neutral, and negative Tweets was created. Two scatter plots, Subjectivity vs. Polarity and Polarity vs. Time, displayed the overall subjectivity and changes in polarity of the governor’s Tweets. In addition, a graph bar-line graph was made to further visualize the polarity of the governor’s Tweets as the total COVID-19 cases and total deaths in the respective state grew in numbers. The total COVID-19 cases and total deaths were collected from [The COVID Tracking Project](https://covidtracking.com/) website.

The subjectivity and polarity are calculated upon function call from the [TextBlob](https://textblob.readthedocs.io/en/dev/quickstart.html#sentiment-analysis) package. The functions average the overall sentiment of each word, while interpreting the word with the full sentence. The subjectivity function returns a value within the range [0.0, 1.0], where 0.0 represents objectivity and 1.0 represents subjectivity. The polarity function returns a value within the range [−1.0, 1.0], where −1.0 is absolutely negative and 1.0 is absolutely positive. For each governor, the total subjectivity, total polarity, total Tweets of the entire period, total positive Tweets, total negative Tweets, total neutral Tweets, and average Tweets made per day were calculated.

## Results & Discussion
In conclusion, compared to Democrat governors, Republican governors had a higher proportion of positive and neutral posts and a lower proportion of negative posts. On average, Twitter posts from both parties were equally subjective and Republican posts were more positive. Given prior literature on the effects of communications from political leaders on the public, we conclude that a unified political stance on social distancing would increase the effectiveness of social distancing orders.

## Demo It Yourself
To try the model yourself, you must enter your own Twitter API authorization codes and clone the repository by entering:

```bash
git clone https://github.com/joyglitch/Twitter-Covid-19-UnBDC2020
```
Then, run the `GovernorTweetAnalysis.ipynb` file in Jupyter Notebook.


## Contributions
If you would like to make a pull request, feel free to contribute. For any significant changes, please open an issue on the repository. Stay safe!
