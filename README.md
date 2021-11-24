# The COVID-19 Real World Worry Datasets

This repo contains the data and variable descriptions on the Real World Worry Datasets.

Papers on this dataset:

- [1]M. Mozes, I. van der Vegt, and B. Kleinberg, ‘A repeated-measures study on emotional responses after a year in the pandemic’, arXiv:2107.03466 [cs], Nov. 2021, Accessed: Nov. 24, 2021. [Online]. Available: http://arxiv.org/abs/2107.03466 (in press at _Scientific Reports_)
- [2]B. Kleinberg, I. van der Vegt, and M. Mozes, ‘Measuring Emotions in the COVID-19 Real World Worry Dataset’, presented at the ACL-NLP-COVID19 2020, Online, Jul. 2020. Accessed: Nov. 02, 2020. [Online]. Available: https://www.aclweb.org/anthology/2020.nlpcovid19-acl.11
- [3]I. van der Vegt and B. Kleinberg, ‘Women Worry About Family, Men About the Economy: Gender Differences in Emotional Responses to COVID-19’, in Social Informatics, vol. 12467, S. Aref, K. Bontcheva, M. Braghieri, F. Dignum, F. Giannotti, F. Grisolia, and D. Pedreschi, Eds. Cham: Springer, 2020, pp. 397–409. doi: 10.1007/978-3-030-60975-7_29.


_Contact: bennett.kleinberg [at] tilburguniversity.edu_

These projects are also available with on the [World Pandemic Research Network](https://wprn.org/#about-us):


- _Measuring emotional responses to COVID-19_ [https://wprn.org/item/459652](https://wprn.org/item/459652); [Presentation on YouTube](https://www.youtube.com/watch?v=ftDKiCrND0k)
- _Gender Differences in Emotional Responses to COVID-19_ [https://wprn.org/item/547252](https://wprn.org/item/547252); [Presentation on YouTube](https://www.youtube.com/watch?v=30M8PFF-TMw)
- _Worry, coping and resignation - A repeated-measures study on emotional responses after a year in the pandemic_ [https://wprn.org/item/545152](https://wprn.org/item/545152); [Presentation on YouTube](https://www.youtube.com/watch?v=Q37Vmq9X6d0)

-------



### Repo structure


- main
    - data_phase_1
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
    - data_repeated_measures
        - meta (n=1698)
        - texts
            - phase1
                - long
                - short
            - phase2
                - long
                - short


_The directory `./data_phase_1/files` contains all 5000 texts, while `./data_phase_1/files_clean` contains those after the exclusion of 9 participants (as reported in the paper). Note: the LIWC data were only extracted on the "cleaned" data._

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

**Note: in the repeated measures version of the dataset, the variables from phase 1 (April 2020) are denoted as "[VARIABLE]_wave1" and those from phase 2 (April 2021) as "[VARIABLE]_wave2". The "delta" variables are the difference between the values from these two measurements (i.e. phase 2 - phase 1).**