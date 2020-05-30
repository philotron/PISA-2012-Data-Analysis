# PISA 2012 Dataset Exploration
### by Phillip Schneider

## Files
- Data preprocessing - wrangle_pisa_data.ipynb
- Exploratory data analysis - slide_deck_pisa_data.ipynb
- Presentation of results - slide_deck_pisa_data.ipynb


## Dataset

The dataset for this project comes from the PISA study conducted in the year 2012. This large-scale, international study aims at assessing problem solving and cognition skills by testing students' scholastic performance in math, reading, and science. While the original dataset (https://s3.amazonaws.com/udacity-hosted-downloads/ud507/pisa2012.csv.zip) holds information for about 500000 students and over 600 observed variables, the prepared subset for this project consists of 299843 rows and 22 columns. The selected columns are as follows:
- country                           
- oecd                              
- gender                            
- age     
- at_home_computer                  
- at_home_internet               
- at_school_computer         
- at_school_internet     
- first_use_computer                
- first_use_internet              
- at_school_chatting              
- at_school_emailing             
- at_school_browsing               
- at_school_downloading         
- at_school_posting           
- at_home_computer_study_time  
- at_home_study_time             
- at_school_computer_study_time    
- avg_math_score                   
- avg_read_score                  
- avg_science_score              
- avg_total_score                


## Summary of Findings

During the exploratory data analysis, the investigation focused primarily on the influences of information and communication technology (ICT) on students' PISA test performance levels. In this regard, variables about the availability, type of activity, as well as frequency of ICT use were examined.

Concerning ICT availability, it became evident that a very large proportion of students have access to computers and the internet. In fact, the availability of such technologies in schools is even slightly better than in students' homes. Yet, despite this greater availability, the actual usage rate of ICT at school is seemingly lower than at home. Putting ICT availability in relation to scholastic performance, students coming from schools with such technical equipment do better than schools without computers and an internet connection. This phenomenon can be observed for both OECD and non-OECD countries.

Another interesting variable is the age of first exposure to ICT. The analysis showed that most students started to use computers and the internet at an age between 7-9 years. Only a very small percentage of students have never used either technology until their current age of 15-16 years. When comparing the age of first use with test scores, the earlier students start using ICT, the better their PISA test performance. Students who never used the technologies in question have by far the lowest average test scores.

As for the study time variable, the shape of the distribution of hours spent studying on the computer is highly right-skewed, meaning that very few students learn with computers for an excessive amount of time of over 25 hours, while the vast majority spends 0-5 hours studying on the computer at home. Furthermore, the correlational analyses disclosed a negative connection between study time on the computer and scores in each of the three test areas. The correlation coefficients take values of around -0.15. Inefficient studying techniques are assumed to be a main cause behind this observation.

The last part of the analysis looked at how students use ICT during their time in school. For the activities of browsing, emailing, chatting, and posting, there seems to be a negative relationship between use frequency and PISA test scores. The higher the frequency of ICT use at school, the lower are the achieved PISA test scores. Students who reported daily ICT usage perform the worst. However, the described effect of less ICT usage and higher test scores is not linear, but wears off after a lower than weekly use frequency. Besides, specific activities like chatting or posting, often connected with social media use, tend to affect test scores more negatively than activities like browsing or emailing. This can be observed across all levels of usage frequency. 

From all the insights above, certain main threads are selected for the final presentation, such as the positive effect of ICT resources in schools as well as the negative effect of time spent studying on computers. The provisionally created visualizations of the data exploration can thus be adopted. However, they need to be polished up in terms of simplification, improved color coding and labeling of the axes. Apart from that, no substantial changes have to be made. The final results are presented in the file "slide_deck_pisa_data.html".
