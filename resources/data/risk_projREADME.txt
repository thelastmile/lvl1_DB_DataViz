================================================
KEYWORDS FOR DATASET: Risk perception
================================================

=======================================================
ACCOMPANYING DATA PROVIDED BY: Dr. Christina G.S. Palmer
             UCLA, Dept. of Psychiatry
             and Biobehavioral Sciences 
=======================================================

================================
GENERAL EXPLANATION OF THE STUDY
================================

Psychologists are interested in finding ways of measuring 
perception of risk, since it is an important component in 
any decision-making process.  There are two general approaches 
to measuring risk perception.  There is an objective approach, 
where participants are asked to evaluate prescribed levels of 
risk for different activities, and there is a subjective 
approach, where participants are asked to provide their own 
levels of risk for an activity.  This data set is from a study 
that combines these two different methods of measuring risk 
and compares participants¹ responses to both types of risk models.
 
This study was published: Carlstrom, Lisa K., Woodward, J. Arthur, 
and Palmer, Christina G.S., Evaluating the Simplified Conjoint 
Expected Risk Model: Comparing the Use of Objective and Subjective 
Information, Risk Analysis, Vol. 20, No. 3, 2000.
 
The data provided here are from the subjective part of the study.  
There were 611 participants who completed the survey.  They 
were asked to provide a numerical value of risk on 22 financial 
and health-related activities using a scale from 0-100 (100 being 
high risk).  They were also asked questions to identify their world 
view.  In general, there are five classifications for world view: 
hierarchists, individualists, egalitarians, fatalists and hermits.  
For this study, participants were either classified into one of the 
first three groups, or they remained unclassifiable.  

From this data set, it is possible to compare how different groups, 
such men and women, perceive risk.  It is also possible to compare 
levels of risk for people of different ethnic backgrounds and for 
people with different world views. 


=============================
BRIEF DESCRIPTION OF THE DATA          
=============================

Participants in this study were recruited between 1997-1998 from five 
sources: UCLA psychology undergraduate classes, campus and community 
organizations, community and college newspaper advertisements, a paid 
consultant, and posted flyers.  The following are the label names for 
each of the 22 activities (all grouped under the variable, ACTIVE):
 
Financial Activities:
 
MED80:  Invest 80% of savings in new medical research firm
MED20:  Invest 20% of savings in new medical research firm
STK80:  Invest 80% of savings in blue chip stock
STK20:  Invest 20% of savings in blue chip stock
GOLD:   Invest in one ounce of gold: now worth about $383
SILV:   Invest in one ounce of silver: now worth about $5
 
Health Activities:
 
DOC:    Work as a family physician in rural area
SWAT:   Work as a member of a SWAT police team
BIKE:   Ride bicycle one mile each day in an urban area
FLU:    Receive annual flu preventative vaccine
CAR:    Drive automobile 10 miles each day in an urban area
POOL:   Swim in indoor public pool each weekend
NUC:    Live near nuclear power station
XRAY:   Receive diagnostic x-rays every 6 months
PLANE:  Fly on commercial airplanes every month
APPL:   Use household appliances
HEART:  Tested for gene that predisposes to heart disease
DIAB:   Tested for gene that predisposes to diabetes
BRCA:   Tested for gene that predisposes to breast cancer
OVCA:   Tested for gene that predisposes to ovarian cancer 
        (females only)
PRCA:   Tested for gene that predisposes to prostate cancer 
        (males only)
GREY:   Tested for gene that predisposes to premature grey hair

  
========================
HOW TO USE THE DATA FILE
========================

The data file is tab delimited text.  The first row contains the list
of variables and each remaining row contains the corresponding data for
one risk judgement.  Please note that these data are stored longitudinally, 
that is, for each observation there is only one activity for which there is 
a risk judgement.  Therefore, for 611 participants, there are a total of 
13,442 observations (611 x 22).  Missing data are indicated by a period.  
Explanations for all variable abbreviations are given below.  
 
The variables are:
 
SUBID......ID of subject
 
RISK.......This is the risk value given to one of the 22 
           activities listed above, on a scale from 0-100 (100 high)
 
ETHNIC.....1=Caucasion, 2=African-American, 3=Mexican-American,     
           4=Taiwanese-American
 
GENDER.....0=Female, 1=Male
 
AGE........Age of participant
 
ACTIVE.....This is the name of the activity, for which the participant is 
           applying a risk judgement.
 
WVCAT......World View Category: 0= Unclassifiable, 1=Individualist, 
           2=Hierarchicalist, 3=Egalitarian


================================================
STATISTICAL TESTS AND ANALYSES USED
================================================
1. T-tests between males and females, on risk levels 
2. Anova, using Ethnicity and World View, on risk levels
3. Chi-squared on Ethnicity and World View, Gender and World View