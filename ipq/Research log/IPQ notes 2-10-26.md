recognise opposite arguments, perfuse them? 
don't wanna just regurgitate facts, u wanna analyse synthesise implications arugments evidences from diff sources, discuss, argue, criticise, evaluate, etc.

essay should be skillful and persuasive

higher lvl of reading and noting, research, uni prep basically 

reading, note taking, organisation, higher cognitive abilities 

read purposefully, skim and scan rather than word for word, important to write down what questions u want research to answer, more time to process idea

avoid superficiality, depth is better, criticise and evaluate always, analyze 

generate own ideas while reading 

add own thoughts to things that u read, prevents plagirisaion? 

reflection of our own thinking  

organise work in a way where u can easily tap into them and be able to retrieve the, and produce immediate improvements

dont have to read books cover to cover, just read the things u need
relevant material
dont waste time

radio coaching ban from singapore 2014 - lifted at german gp 2016

maybe compare during ban and after + preban? 
but then cars are very diff
pre ban can only rlly compare rosberg and hamilton cus only them stayed tgt from 2013-14, but then in 14 they were fighting for title so adds another factor which is hard to adjust for
post german gp 2016 only 9 rounds left in 2016, so we can also use that data

so first 14 rounds of 2014 (rounds 1-13) and last 9 rounds of 2016: no driver ban, 23 races total

This restriction was introduced to enforce the sporting regulation that "the driver must drive the car alone and unaided," Article 20.1 (or Article 27.1 in later versions) of fia sporting conduct
Gear selection and braking points.
Racing lines and car set-up adjustments.
Direct technical questions (e.g., torque map settings)

dropped in 2016: no limit in race, apart from period between start and formation lap and start of race
stricter ban for first 11 races of 2016, separate group
6 races in 2014 and 19 races in 2015 radio ban, 25
36 total races wit radio ban compared to 23 wit no radio ban

banning radio coaching would make gap between worse driver even worse and make races less exciting and competitive

green flag laps only, no lap 1, no pit laps, safety car laps, wet races. 

comparing shifts in gaps between teammates

wet races 2014-2016: 
https://www.reddit.com/r/formula1/comments/g0plkr/list_of_wet_weather_races_and_wins_by_driver/
2 in 2014: hungary and japan
2 in 2015: gb and usa
3 in 2016:  monaco, gb and brazil
22 coaching races and 30 no coaching races when accounted for rain

merc line up same 2014-2016 nico and hamilton
williams same lineup 2014-2016 massa and bottas
force india same 2014-2016 perez and hulk
ferrari same 2015-2016 seb and kimi

Saturday's data = real standard deviation. If  shift is smaller than the thresholds above, report the result as inconclusive. 

problems with the plan that was synthesized on 09-09-2026
- huge regulation change from 2013-2014, chassis, engine, etc. one of the largest regulation changes in f1 history. change in gap could have occured from cars, not from driver coaching
- 2014 ban started in singapore gp, round 14/19, so only 6 races of sample data, which is not a large enough sample size to get reliable data
- only 2 pair of drivers stayed together from 2013-2014, hamilton and rosberg in mercedes, bianchi and chilton in marussia. the pair of marussia split in 2014, so only really 1 pair of drivers. 
- hamilton and rosberg were also heavily involved in the title fight in 2014. this could have caused drivers to push considerably harder and take more risks than normal, or the races could have been influenced by team orders more often than without a title fight involved.

i would pull data from jolpica and fastf1api about driver lap times and the gap between the lap times between drivers, as well as run a permutations test, which is where i check whether the difference that i measured between the shift in lap times is bigger than random shuffling would be

how permutations test would run:
- take the 2013 merc and marussia drivers, compare and calculate difference in median lap times to 2014 merc and marussia drivers. 
- then we pool these values and assign them randomly to the 2 groups
- recalculate the difference in median lap times
- repeat a few thousand times
- the p value is the % of the shuffles that produced a difference at least  as large as my real comparison
- e

if the lap time gap numbers, the shift in the gap and the permutation test are not final by Sun 25-10-2026, drop the 2013 baseline first, as it would put me behind schedule.