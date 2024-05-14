The goal of this exercise is to determine when people will accept coupons sent to their phone while driving.

Here is a summary of key findings from this data set:

60% of those who make more than 50k, and go to the bar more than 4 times per month, accepted the coupon. How about 100k?

65% accepted the coupon who visit the bar monthly and make 100k or more a year. How about low wage earners?

68% of those who make <12.5k accepted the coupon. Next, lets's look at bar visits per month vs acceptance

53% of those who never go to the bar, accepted the coupon

62% of those who go to the bar between 1 and 3 times per month accepted the coupon

64% of those who go the bar between 4 and 8 times per month accepted the coupon

People who visit the bar eight times per month, accepted coupons 58% of the time. This is lower than the other groups who visit the bar less. It would be a good follow up question to determine why this group accepts coupons less (assumably they are focused more on drinking than eating, so the type of coupon would be important. Let's next look at people who visit higher end restaurants eight times per month.

People who ate at resturants from 20-50 dollars a meal, accepted the coupon 66% percent of the time. I would assume this group has discretionary income and this is why acceptance is higher (they eat and drink out a lot more than the bar groups). Let's next look at the relationship between income and bar visits.

In general, alcoholism (visiting a bar greater than 8 times per month) is common across all income groups. Lower to middle class wage earners were more likely to never visit bars than the higher earners. This could be due to more discretionary income, which is certainly another question I'd look into, in future endeavours.

This visualization shows that the women in this group are more likely to go the bar eight times a month, the more educated they are. For men, those who didn't go to college or are in college without a degree were more likely to go to the bar eight times a month.

How does income and occupation affect acceptance of coupons for each group?

Largely, people who make less than $62.5k accept coupons at the higher rates than their peers in higher earning groups. Interestingly, the 100k group accepted coupons much higher than the middle income groups. It would be good to normalize this chart, to make sure we are not underestimating the strength of a smaller group. Let's look closer at the 100k group versus education and occupation.

Of the high earners, computer and math along with business and financial roles, we're more likely to accept coupons in general. Coffee house coupons were accepted at a higher rate than all other coupon types.

Of those that made less than $12.5k accepted coupons, students and unemployed people accepted coupons at a much higher rate than other professions.

For the middle income group, student, unemployed and computer/math professions accepted coupons the most. It would be interesting to look deeper into why these groups are more willing to accept coupons. The most accepted coupons are for low cost restaurants and coffee shops. This would correlate well with a student lifestyle. The bar coupon group was fairly well rounded across the group at this income range, which does make sense: our culture is quite intermixed with alcohol use.




Prompt for exercise for reference:
Will a Customer Accept the Coupon?
Context

Imagine driving through town and a coupon is delivered to your cell phone for a restaraunt near where you are driving. Would you accept that coupon and take a short detour to the restaraunt? Would you accept the coupon but use it on a sunbsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaraunt? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

Overview

The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

Data

This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’. There are five different types of coupons -- less expensive restaurants (under $20), coffee houses, carry out & take away, bar, and more expensive restaurants ($20 - $50).

Deliverables

Your final product should be a brief report that highlights the differences between customers who did and did not accept the coupons. To explore the data you will utilize your knowledge of plotting, statistical summaries, and visualization using Python. You will publish your findings in a public facing github repository as your first portfolio piece.

Data Description
Keep in mind that these values mentioned below are average values.

The attributes of this data set include:

User attributes

Gender: male, female
Age: below 21, 21 to 25, 26 to 30, etc.
Marital Status: single, married partner, unmarried partner, or widowed
Number of children: 0, 1, or more than 1
Education: high school, bachelors degree, associates degree, or graduate degree
Occupation: architecture & engineering, business & financial, etc.
Annual income: less than $12500, $12500 - $24999, $25000 - $37499, etc.
Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
Number of times that he/she buys takeaway food: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
Number of times that he/she goes to a coffee house: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
Number of times that he/she eats at a restaurant with average expense less than $20 per person: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
Contextual attributes

Driving destination: home, work, or no urgent destination
Location of user, coupon and destination: we provide a map to show the geographical location of the user, destination, and the venue, and we mark the distance between each two places with time of driving. The user can see whether the venue is in the same direction as the destination.
Weather: sunny, rainy, or snowy
Temperature: 30F, 55F, or 80F
Time: 10AM, 2PM, or 6PM
Passenger: alone, partner, kid(s), or friend(s)
Coupon attributes

time before it expires: 2 hours or one day
