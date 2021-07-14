# the dataset structure

the dataset contains(2389217) record and (29) features
some of them looks like a combination of two features of them like
Deptime - CRSDep = Depdelay
ArrTime - CRSArrtime = Arrival delay

understanding some features meaning

ElapsedTime = time taken (as by a boat or automobile in traveling over a racecourse) this means that the Air time doesnt count the time of taking off or the landing
Elapsed Time: The time computed from gate departure time to gate arrival time.

"NAS" are the type of weather delays that could be reduced with corrective action by the airports or the Federal Aviation Administration.

carrier delay are: aircraft cleaning, aircraft damage, awaiting the arrival of connecting passengers or crew, baggage, bird strike, cargo loading, catering, computer, outage-carrier equipment, crew legality (pilot or attendant rest), damage by hazardous goods

aircraft delay is a result of the late arrival of the previous flight that utilized the same plane that will be departing. This causes the current flight to take off late and creates a domino effect

# main questions
I am more interested in<br>
1)the contribution of the Air carrier on the delay<br>
2)the contribution of the Air carrier on the cancellation<br>
3)when is the worst time and best time of the year regarding the delays<br>
4)what causes the most departure delay and elapsed delay<br>

# A summary of your findings and steps taken in your analysis.

the dataset coveres alot of flights in short distance , the long distance flights are fewer that those for short distance<br>
thursday has the highest arrival delay and departure delay , which indicates that its the busiest day of the week<br>
tuesday and surprisingly friday are the best days to travel without delays<br>
february has the highest arrival delay and departure delay<br>
january score is expected as its a busy time of the year due to holidays<br>
this relationship shows that in some records eventhough there were departure delay some planes arrived early or on time<br>
distance is highly corr with airtime<br>

**correllation**
departure delay and arrival delay are highly corr<br>
departure delay and elapsed delay are negatively correlated<br>
**carrier delays**
AQ and HA carriers arrives early and departure early this can be problematic for late passengers however the bording protocol of the passenger makes them board the plane early they are just early in a range of 0.5 to 2.5 minuits<br>
AA is the worst regarding arrival delay<br>
UA is the worst regrding Departure delay<br>
**cancellation**
WN is the most frequesnt carrier<br>
F9 carrier never cancels<br>
the highest cancellation percentage with 6% is YV<br>

**delay causes**
weather delay and carrier delay are the main causes of the high departure delay<br>
nasdelay and late aircraft delay causes the departure delay but not alot of time like weather and carrier delay<br><br>

the main reason of elapsed delay is the nas delay which is strange as the weather delay is very small<br>

this relationship can be explained as the time taken to prepare the plane to fly in harsh weather makes the delay because of weather small while the nas delay high<br>

also the carrier delay looks to have alot of outliers this can be explained as the carriers varies alot with unbalanced numbers of frequency for each carrier in the dataset<br>

also the airport making nas protocol to be able to fly in harsh weather this means that there is a bad weather that causes troubles in taking off and landing or sometimes flying hence, the high elapsed delay<br>


# Key points discovered in your exploratory file.


in the slide show i focused on the answeres of the main questions 
the slideshow startes with the distribution of the cancelled flights to the not cancelled  then the distance distributions in the dataset , followed by answering third question using a line plot to know the best time to travel regarding the delays ,  then the relation between arrival delay and departure delay were invistigated which didnt end up to be linear as expected to be instead some points showed even if there is departure delay the plane can arrive early
later in the carrier plots these  points showed in AQ & HA carriers , then the fourth question was answered using pointplot
