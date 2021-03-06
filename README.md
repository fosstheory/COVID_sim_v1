# COVID_sim_v1
17-parameter simulation of COVID-19 spread in a region, starting Mar 13th, 2020.  Daily stats predicted.

Most probable scenarios #1 or #3 have more than 40M deaths, after we run out of hospital space in mid-April.
Make sure to read the results summary text file.

SCRIER.org has created a deterministic state-machine simulation of the COVID spread in a region.
You can use this as an engine to drive a GUI, or for results to communicate to your policy-maker.
Nice whizzy graphs, and real-time updates, will be available at scrier.org .


Please send supporting thank-yous to gofundme.com/f/scrier  .  

GET STARTED:
1.  Download and unzip the repository.
2.  Code is written in basic C-style C++ in ONE FILE, main.cpp, for brain-dead simple caveman portability.
    Put main.cpp and parameters.h in the same directory, and compile them with your favorite C / C++ compiler.
    Then execute the results.
3.  We have included the output here because it's too important to not publicize.
4.  Current params file is best guess for entire America as of Mar 15 '20.
    The apocalypse is proceeding almost exactly as predicted, so no new updates needed here as of Mar 24 '20.
5.  Alternate params file jparameters.h is for best guess params on the nation of Japan.
    Swap out #include "parameters.h"  with #include "jparameters.h"
6.  Because the engine is almost all agnostic on parameters, you can set up the params
    for any state, any region, any other country, and they should work reasonably well.
    Forgot that the first couple of days' data initialization is hardwired inside main.
    This will not matter any, as ALL OF THE EXPANSION COMES FROM THE EXPONENTIAL EXPLOSION.
    It really hardly matters where you start.
    
 Contributions: 
1. Day-by-day breakdown prediction of how many Known (official) infections.  This is important to establish credibility--we are boldly predicting totals weeks ahead of time.  So far it's scarily accurate.
2. Assumptions about hospital and ventilator saturations on deaths.
 
 LEAVES OUT:
 350,000 pregnant births EACH MONTH in America, will have to stay at home.
 
 MAJOR ASSUMPTIONS:
1.  If a person is so severely sick that they need a hospital bed or die, and if turned away from hosp, then they'll die (in a few days)
2. 20% of infecteds are Severe or Critical, that's 15% Severe, 5% Critical
3. 50% of Criticals on ventilators die after a week; 50% live after 6 weeks on ventilator
4. 1,000,000 Hospital Beds (staffed), and 200,000 ventilators (staffed).  For America.
5. Ventilators come w/ own separate bed (not included in Hospital Beds total).  If this is wrong, we're hosed further.
6. Soft quarantine knocks down the spread factor but is largely ineffective for completely preventing spread.  People still go out to the grocery store, the gym, the pharmacy, or pick up packages from delivery folk, and get infected at a background level--then bring those infections home to everyone else in their household.  Round v.1.4 should dynamically adjust the number of available adults in the population if strict quarantining actually works.
7.  Note:  Since actual infections are probably somewhere between 500,000 and 5M at this moment, because they are lagged by 1-2 weeks (that's a factor of 10-100) behind known infections, even with strict quarantining we're probably still hosed.
8.  Other countries such as Japan and Germany are maybe two weeks behind America.  Learn from the example of others, and it might be good to avoid repeating their mistakes.  You can use this code to run numbers for your region, too!  
 
 RECOMMENDATIONS:
 As of Tues Mar 24 '20 we have 14 days before known infections hit definite 5M, another 7 days before probable 50M.
 Make all the paper bunny suits you can in 14 days.  Make extras out of garbage bags.
 Set up gymnasiums, enclosed stadiums, church halls, hotels, to deal with 10M-30M severely sick people by mid-April.
 Set up ice rinks as temporary morgues to deal with a couple million dead people happening in two weeks.
 
 TELL EVERYONE TO **STAY THE #### HOME AND NOT GO OUT *
