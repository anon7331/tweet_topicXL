# TweetTopicXL dataset
This a topic classification dataset on Twitter with 19 labels. The datasets includes tweets in 4 languages, English (en), Spanish (es), Greek (gr), and Japanese (ja).
There are 1,000 tweets per language (4,000 in total).

# Labels
| <span style="font-weight:normal">0: arts_&_culture</span>           | <span style="font-weight:normal">5: fashion_&_style</span>   | <span style="font-weight:normal">10: learning_&_educational</span>  | <span style="font-weight:normal">15: science_&_technology</span>  |
|-----------------------------|---------------------|----------------------------|--------------------------|
| 1: business_&_entrepreneurs | 6: film_tv_&_video  | 11: music                  | 16: sports               |
| 2: celebrity_&_pop_culture  | 7: fitness_&_health | 12: news_&_social_concern  | 17: travel_&_adventure   |
| 3: diaries_&_daily_life     | 8: food_&_dining    | 13: other_hobbies          | 18: youth_&_student_life |
| 4: family                   | 9: gaming           | 14: relationships          |                          |


# Files 
In each language folder (en, es, ja, gr):

* A cross validation folder (cross_validation) containing all the splits for 5-fold cross-validation with:
   * {lang}_train_{i}.jsonl: 720 tweets
   * {lang}_test_{i}.jsonl: 200 tweets
   * {lang}_validation_{i}.jsonl: 80 tweets
* {lang}_1000.jsonl: containing all the new tweets collected (1,000 tweets)
* {lang}_test.jsonl: the test set to be used (800 tweets)
* {lang}_train.jsonl: the train set to be used (180 tweets)
* {lang}_validation.jsonl: the validation set to be used (20 tweets)

For the aggregatation a label is assigned if at least two coders aggree on it.


All the annotations are also included:
- en_all.csv
- es_all.csv
- gr_all.csv
- ja_all.csv
