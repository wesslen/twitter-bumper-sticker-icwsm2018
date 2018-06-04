## Paper

Wesslen, R., Nandu, S., Eltayeby, O., Gallicano, T., Levens, S., Jiang, M., and Shaikh, S. (2018). [Bumper Stickers on the Twitter Highway: Analyzing the Speed and Substance of Profile Changes](https://github.com/wesslen/twitter-bumper-sticker-icwsm2018/raw/master/wesslen-bumper-sticker-icwsm2018.pdf). ICWSM 2018 Poster Paper.

~~~
@inproceedings{twitterbumpersticker,
  title = {Bumper Stickers on the Twitter Highway: Analyzing the Speed and Substance of Profile Changes},
  author = {Wesslen, Ryan and Nandu, Sagar, and Eltayeby, Omar and Gallicano, Tiffany and Levens, Sara and Jiang, Min and Shaikh, Samira}, 
  booktitle = {Proceedings of the 12th International AAAI Conference on Web and Social Media},
  series = {ICWSM '18},
  year = {2018},
  location = {Palo Alto, California}
  }
~~~

## Instructions to run

The code is written in R 3.4.3 or higher. Highly recommend using RStudio 1.1.383 or higher.

Open the file twitter-bumper-sticker-icwsm-2018.Rproj.

1) Twitter API and tweetscores package code to run the experiment ([Rmd](./01-run-experiment.Rmd) / [HTML](https://htmlpreview.github.io/?https://github.com/wesslen/twitter-bumper-sticker-icwsm2018/blob/master/01-run-experiment.html))
2) Topic Modeling on profile summaries to get groups ([Rmd](./02-topicmodeling.Rmd) / [HTML](https://htmlpreview.github.io/?https://github.com/wesslen/twitter-bumper-sticker-icwsm2018/blob/master/02-topicmodeling.html))
3) Word probabilities (raw and FREX) for labeling topic groups ([Rmd](./03-topicmodel-labeling.Rmd) / [HTML](https://htmlpreview.github.io/?https://github.com/wesslen/twitter-bumper-sticker-icwsm2018/blob/master/03-topicmodel-labeling.html))
4) Plots used in the paper ([Rmd](./04-plots.Rmd) / [HTML](https://htmlpreview.github.io/?https://github.com/wesslen/twitter-bumper-sticker-icwsm2018/blob/master/04-plots.html))

## Data

Due to Twitter's Terms-of-Services, we are not able to provide the experiment data publicly. However, please email <rwesslen@uncc.edu> if you are interested in obtaining the dataset for research purposes only.

The dataset pulled a 24 hour 1\% sample of Tweets (3.4MM tweets) on September 28, 2017. Using that dataset, we identified 2.58MM unique Twitter profile ID's (actor.id). Using the [`tweetscores`](https://github.com/pablobarbera/twitter_ideology) package, we then received a snapshot of each Twitter profile over a two week period. Each snapshot (i.e., 2.58MM profiles) took approximately 36 hours, thus yielding 9 snapshots of profiles over a two week period.

