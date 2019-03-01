# The News Reading Dataset

This dataset was created to support research on modeling  **User Behavior, Preference,  Satisfaction**. We conducted a user study in **Online News Reading Scenario** on the **Mobile Devices**. User's interactions and explicit feedback were collected during user study.

## User Preference in Multi-Phases

**Before-Read Preference**

As soon as the user clicks a news snippet, we ask for his/her expected preference for the news, before he/she sees the content.

**After-Read Preference**

After the user decides to end reading the content of news, we ask for his/her experience in reading the news. 

**Post-Task Preference**

After user finishing the task, we shuffle the news shown to the user, and ask for his/her actual preference. 	

## Data Description

|         | #users | #tasks | #news | #clicks |
| ------- | ------ | ------ | ----- | ------- |
| Dataset | 32     | 352    | 5280  | 1603    |

*logs.csv*

| Measures               | Description                              |
| ---------------------- | ---------------------------------------- |
| userid                 | user identity                            |
| newsid                 | news identity                            |
| taskid                 | task identity                            |
| topic                  | the topic of the news                    |
| topic_pref             | user's interest in the topic of the news |
| equality               | expert quality of the news               |
| imp_position           | position of the news in the recommendation list |
| viewport_time          | the time user spend reading the snippet of the news |
| dwell_time             | the time user spend reading the content of the news |
| read_ratio             | the percentage of content user read      |
| read_speed             | the speed of user's reading (pixel/s)    |
| direction_change_times | the times user changes his scroll direction |
| pre_pref               | user preference in before-read phase     |
| read_pref              | user preference in after-read phase      |
| post_pref              | user preference in post-task phase       |

*tasks.csv*

|              | description             |
| ------------ | ----------------------- |
| userid       | user identity           |
| taskid       | task identity           |
| satisfaction | task-level satisfaction |



## How to get the detailed dataset

We provide the [data]() used in the [paper](http://www.thuir.cn/group/~mzhang/publications/SIGIR2018-LHY.pdf) we published at the SIGIR 2018 conference. For the whole dataset that contains the detailed user behavior, you need to contact with us. After signing an application forum online, we can send you the data.

## Citation

If you use this dataset in your research, please add the following bibtex citation in your references. A preprint of this paper can be found [here](http://www.thuir.cn/group/~mzhang/publications/SIGIR2018-LHY.pdf). 

```tex
@inproceedings{Lu:2018:CSS:3209978.3210007,
 author = {Lu, Hongyu and Zhang, Min and Ma, Shaoping},
 title = {Between Clicks and Satisfaction: Study on Multi-Phase User Preferences and Satisfaction for Online News Reading},
 booktitle = {The 41st International ACM SIGIR Conference on Research \&\#38; Development in Information Retrieval},
 series = {SIGIR '18},
 year = {2018},
 isbn = {978-1-4503-5657-2},
 location = {Ann Arbor, MI, USA},
 pages = {435--444},
 numpages = {10},
 url = {http://doi.acm.org/10.1145/3209978.3210007},
 doi = {10.1145/3209978.3210007},
 acmid = {3210007},
 publisher = {ACM},
 address = {New York, NY, USA},
 keywords = {click-through rate, item-level preference, multi-phase user preference, user behavior analysis, user satisfaction},
} 
```

