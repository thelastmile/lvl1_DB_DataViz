==================================================
KEYWORDS FOR DATASET: Medical, Biology, Physiology
==================================================

===============================================================
ACCOMPANYING DATA PROVIDED BY: Alan Garfinkel, PhD
                               UCLA, Department of Physiology
===============================================================

================================
GENERAL EXPLANATION OF THE STUDY
================================
This data is from a study that was trying to determine if a drug called 
"dobutamine" could be used effectively in a test for measuring a 
patient's risk of having a heart attack, or "cardiac event."  For younger 
patients, a typical test of this risk is called "Stress Echocardiography." 
It involves raising the patient's heart rate by exercise--often by having
the patient run on a treadmill--and then taking various measurements, such 
as heart rate and blood pressure, as well as more complicated 
measurements of the heart.  The problem with this test is that it often 
cannot be used on older patients whose bodies can't take the stress of hard 
exercise.  The key to assessing risk, however, is putting stress on the heart 
before taking the relevant measurements.  While exercise can't be used to 
create this stress for older patients, the drug dobutamine can. This study, 
then, was partly an attempt to see if the stress echocardiography test was 
still effective in predicting cardiac events when the stress on the heart 
was produced by dobutamine instead of exercise. More specifically, though,
the study sought to pinpoint which measurements taken during the 
stress echocardiography test were most helpful in predicting whether or not
a patient suffered a cardiac event over the next year. The complete
citation for the journal in which the results of the study were published
is as follows:

Garfinkel, Alan, et. al.  "Prognostic Value of Dobutamine Stress 
  Echocardiography in Predicting Cardiac Events in Patients
        With Known or Suspected Coronary Artery Disease." 
  Journal of the American College of Cardiology 33.3 (1999) 708-16. 

=============================
BRIEF DESCRIPTION OF THE DATA          
=============================
The accompanying data file contains the complete data for the final
study population, which included 220 men and 338 women. The data collected
on each subject is explained below.

========================
HOW TO USE THE DATA FILE
========================
The actual data file is a comma delimited text file. The first row contains
the abbreviations for the information recorded on each subject. The remaining 
rows each represent a single patient's corresponding information. 

For the purposes of the study, the "cardiac events" that the "Dobutamine
Stress Echocardiography" was attempting to predict were broken down into 
four categories:
        
   CARDIAC EVENTS: (1) myocardial infarction (MI)
                   (2) revascularization by percutaneous transluminal
                       coronary angioplasty (PTCA)
                   (3) coronary artery bypass grafting surgery (CABG) 
                   (4) cardiac death

If you're not familiar with medical jargon, you can simply think of these 
as four things that can go wrong with your heart, and that the test was 
trying to predict. In the datafile you can see whether or not a patient 
suffered one of these cardiac events in the year following the patient's
test by looking in the columns marked "newMI", "newPTCA", "newCABG", and
"death".  Note that, contrary to statistical convention, a "1" means that 
the patient DID NOT suffer the corresponding cardiac event, and a "0" means
that he DID. 

The other variables are explained below.       

==============================================================
EXPLANATION OF DATA MEASUREMENT ABBREVIATIONS IN THE DATA FILE
==============================================================

bhr   BASAL HEART RATE  
basebp    BASAL BLOOD PRESSURE  
basedp          BASAL DOUBLE PRODUCT (= bhr x basebp)
pkhr          PEAK HEART RATE
sbp         SYSTOLIC BLOOD PRESSURE
dp          DOUBLE PRODUCT (= pkhr x sbp)
dose          DOSE OF DOBUTAMINE GIVEN
maxhr         MAXIMUM HEART RATE
%mphr(b)  % OF MAXIMUM PREDICTED HEART RATE ACHIEVED BY PATIENT
mbp         MAXIMUM BLOOD PRESSURE
dpmaxdo         DOUBLE PRODUCT ON MAXIMUM DOBUTAMINE DOSE
dobdose         DOBUTAMINE DOSE AT WHICH MAXIMUM DOUBLE PRODUCT OCCURED
age         PATIENT'S AGE
gender          PATIENT'S GENDER (male = 0)
baseEF          BASELINE CARDIAC EJECTION FRACTION (a measure of 
                the heart's pumping efficiency) 
dobEF         EJECTION FRACTION ON DOBUTAMINE
chestpain 0 MEANS THE PATIENT EXPERIENCED CHEST PAIN
posECG          SIGNS OF HEART ATTACK ON ECG (0 = yes)
equivecg  ECG IS EQUIVOCAL (0 = yes)
restwma         CARDIOLOGIST SEES WALL MOTION ANAMOLY ON ECHOCARDIOGRAM
                (0 = yes)
posSE         STRESS ECHOCARDIOGRAM WAS POSITIVE (0 = yes)
newMI         NEW MYOCARDIAL INFARCTION, OR HEART ATTACK (0 = yes)
newPTCA         RECENT ANGIOPLASTY (0 = yes)
newCABG         RECENT BYPASS SURGERY (0 = yes)
death         THE PATIENT DIED (0 = yes)
hxofHT          PATIENT HAS HISTORY OF HYPERTENSION (0 = yes)
hxofdm          PATIENT HAS HISTORY OF DIABETES (0 = yes)
hxofcig         PATIENT HAS HISTORY OF SMOKING (0 = yes)
hxofMI          PATIENT HAS HISTORY OF HEART ATTACK (0 = yes)
hxofPTCA  PATIENT HAS HISTORY OF ANGIOPLASTY (0 = yes)
hxofCABG  PATIENT HAS HISTORY OF BYPASS SURGERY (0 = yes)
any event THIS IS THE OUTCOME VARIABLE. IT IS DEFINED AS 
                "death OR newMI OR newPTCA OR newCABG". IF ANY OF 
                THESE VARIABLES IS POSITIVE (= 0) THEN "ANY EVENT"
                IS ALSO POSTIVE (= 0).

     ************************************************************
     *  THE FOLLOWING REMAINING VARIABLES ARE THE RESEARCHER'S  *
     *      TECHNICAL CALCULATIONS AND THEY MAY BE IGNORED      *  
     ************************************************************
               
phat  
event(#)  
mics  
deltaEF 
newpkmphr 
gdpkmphr  
gdmaxmphr 
gddpeakdp 
gdmaxdp hardness

================================================
STATISTICAL TESTS AND ANALYSES USED IN THE STUDY
================================================
1) Two-sample z-test (or p-test) for difference in mean.
2) Chi-square test for independence.
3) Logistic regression analysis.
4) the Hosmer/Lemeshow "goodness of fit" test.
5) CART analysis (Classification and regression tree analysis).