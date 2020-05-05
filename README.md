# COVID-19 Real World Worry Dataset

Papers on this dataset:

- [1]I. van der Vegt and B. Kleinberg, “Women worry about family, men about the economy: Gender differences in emotional responses to COVID-19,” arXiv:2004.08202 [cs], Apr. 2020, Accessed: Apr. 20, 2020. [Online]. Available: http://arxiv.org/abs/2004.08202.
- [2]B. Kleinberg, I. van der Vegt, and M. Mozes, “Measuring Emotions in the COVID-19 Real World Worry Dataset,” arXiv:2004.04225 [cs], Apr. 2020, Accessed: Apr. 10, 2020. [Online]. Available: http://arxiv.org/abs/2004.04225.

Contact: bennett.kleinberg [at] ucl.ac.uk

### Repo structure

- main
    - files
        - meta
        - texts
            - short (n=2500)
            - long (n=2500)
    - files_clean
        - liwc
        - meta
        - texts
            - short (n=2491)
            - long (n=2491)


_The directory "files" contains all 5000 texts, while "files_clean" contains those after the exclusion of 9 participants (as reported in the paper_

Note: the LIWC data were only extracted on the "cleaned" data.

-----

### Variable codebook


| Variable name             	| Type       	| Meaning                                                                                                	|
|---------------------------	|------------	|--------------------------------------------------------------------------------------------------------	|
| startdate                 	| time stamp 	| Time of starting the task                                                                              	|
| enddate                   	| time stamp 	| Time of submitting the task                                                                            	|
| duration                  	| numeric    	| Duration in seconds                                                                                    	|
| worry                     	| numeric    	| 9-point scale rating (1=low, 9=high)                                                                   	|
| chosen_emotion            	| string     	| Choice of emotion that best represented their feeling                                                  	|
| anger                     	| numeric    	| 9-point scale rating (1=low, 9=high)                                                                   	|
| disgust                   	| numeric    	| 9-point scale rating (1=low, 9=high)                                                                   	|
| fear                      	| numeric    	| 9-point scale rating (1=low, 9=high)                                                                   	|
| anxiety                   	| numeric    	| 9-point scale rating (1=low, 9=high)                                                                   	|
| sadness                   	| numeric    	| 9-point scale rating (1=low, 9=high)                                                                   	|
| happiness                 	| numeric    	| 9-point scale rating (1=low, 9=high)                                                                   	|
| relaxation                	| numeric    	| 9-point scale rating (1=low, 9=high)                                                                   	|
| desire                    	| numeric    	| 9-point scale rating (1=low, 9=high)                                                                   	|
| text_long                 	| string     	| Text input on long text (500 chars. minumum)                                                           	|
| text_short                	| string     	| Text input on Tweet-sized text (280 chars. maximum)                                                    	|
| self\_rating_general       	| numeric    	| 9-point scale rating (1=low, 9=high) - how well they could express their feelings in text in general   	|
| self\_rating_short         	| numeric    	| 9-point scale rating (1=low, 9=high) - how well they could express their feelings in the short text    	|
| self\_rating_long          	| numeric    	| 9-point scale rating (1=low, 9=high) - how well they could express their feelings in the long text     	|
| twitter\_general_often     	| numeric    	| 9-point scale rating (1=rarely, 9=very often) - how often they are on Twitter                          	|
| twitter\_tweet_often       	| numeric    	| 9-point scale rating (1=rarely, 9=very often) - how often they tweet on Twitter                        	|
| twitter\_participate_often 	| numeric    	| 9-point scale rating (1=rarely, 9=very often) - how often they participate in conversations on Twitter 	|
| eng_native                	| string     	| Whether English is their native language (Yes, No, No but fluent)                                      	|

