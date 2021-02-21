# DSI-Project01

## Background
In United State, SAT and ACT are standardized tests in order to admittance to a US university along with others extracurricular activities, essays, athletics, and others.
The difference between SAT and ACT:
* SAT has two sections of the test: Evidence-Based Reading and Writing and Mathematics.
* ACT has 4 sections: English, Mathematics, Reading, and Science, with an additional optional writing section.

## Problem Statement
As United State government decided to funded ACT and SAT test for high school students in particular states with a limited budget in order to help student for higher education.  
For the best outcome, which states should they funded for ACT and SAT?

## Outside research
From outside research there are policy in some state that provide a free test for students in its state.

* For SAT there are 9 states in 2017 and incresed to 15 states in 2019.
* For ACT there are 17 states in 2017 and incresed to 20 states in 2019.


https://magoosh.com/hs/sat/states-provide-sat-free/  
https://magoosh.com/hs/act/states-provide-act-free/  
https://theolivebook.com/states-that-offer-the-act-or-sat-for-free/

## Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|**state**|*Object*|sat_test|The state name in USA.|
|**year**|*Integer*|sat_test|The year of test.|
|**participation**|*float*|sat_test|The propotion of students who take ACT in specific state.|
|**ebrw**|*Intrger*|sat_test|The mean of Evidence-based reading and writing section of SAT score in specific state.|
|**math**|*Intrger*|sat_test|The mean of Mathemetics section of SAT score in specific state.|
|**total**|*Intrger*|sat_test|The mean of total of SAT score in specific state.|
|**free_sat**|*Intrger*|sat_test|The indicator show state funded SAT test fee.|
|**state**|*Object*|act_test|The state name in USA.|
|**year**|*Integer*|act_test|The year of test.|
|**participation**|*float*|act_test|The propotion of students who take ACT in specific state.|
|**composite**|*float*|act_test|The mean of composite of ACT score in specific state.|
|**school**|*Object*|sat_act_by_college|The name of school/university.|
|**test_optional**|*Object*|sat_act_by_college|Specify that its required SAT/ACT or not.|
|**applies_class_year**|*Object*|sat_act_by_college|Specify that its not required SAT/ACT in which year.|
|**applies_class_year**|*Object*|sat_act_by_college|Specify that its not required SAT/ACT in which year.|
|**policy_details**|*Object*|sat_act_by_college|The details of optional requirement.|
|**number_of_applicantsl**|*Interger*|sat_act_by_college|Number of applicant.|
|**accept_rate**|*float*|sat_act_by_college|Acceptance rate.|
|**sat_25_percentile**|*float*|sat_act_by_college|SAT accept at 25th percentile.|
|**sat_75_percentile**|*float*|sat_act_by_college|SAT accept at 75th percentile.|
|**act_25_percentile**|*float*|sat_act_by_college|ACT accept at 25th percentile.|
|**act_75_percentile**|*float*|sat_act_by_college|ACT accept at 75th percentile.|

## Conclusions
Based on the data, major movements in participation rates are depended to the state policies.  
If a state were funded for all students to take SAT/ACT, the participation rate would increased to nearly 100%.  
And participation rates also related with average total/composite score in negative way.  
Therefore, prediction of new total/composite score when participation rate is 100%, is the way to ranked a states with high ability of student regardless to the differs of participation rate.

## Recommendations
As the result,  the government can decided to make funded to which states that have prediction of high average total/composite score while the participation rate is nearly to 100% which are:
* SAT funded for Massachusetts, Minnesota, Wisconsin, Virginia and South Dakota etc.
* ACT funded for Connecticut, Massachusetts, New Hampshire, Michigan and Illinois etc.
