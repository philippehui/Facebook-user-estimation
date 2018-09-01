# Facebook-user-estimation

## 1. Why I have this question:
- Facebook is the biggest social network company in the world.
- The number of users are one of the most significant metrics for stakeholders. The company disclose number of users in four regions( US and Canada, Europe, Asia and Pacific, Rest of World ) quarterly.
- In the last half year, Facebook stock price has experienced two sharp falls because of market concerns about user growth.(one by Cambridge Analytica scandal, the other by General Data Protection Regulation (GDPR) compliance).<br>
![screen shot 2018-08-31 at 3 12 06 pm](https://user-images.githubusercontent.com/31684373/44950007-1f159880-adf2-11e8-9aa3-328dea31b128.png)

Articles link to this theme:<br>
https://www.nytimes.com/2018/03/19/technology/facebook-cambridge-analytica-explained.html <br>
https://qz.com/1234414/should-you-delete-facebook-what-are-the-alternatives/<br>
<br>
Background Knowledge: 

- Daily Active User(DAU): Facebook defines a daily active user as a registered Facebook user who logged in and visited Facebook through Facebook website or a mobile device, or used facebook Messenger application (and is also a registered Facebook user), on a given day. 

The definition of DAU by Facebook is relatively more strict in social network industry.


## 2. US people have more and more Leisure Time<br>
![screen shot 2018-09-01 at 2 30 31 pm](https://user-images.githubusercontent.com/31684373/44950067-a1eb2300-adf3-11e8-91c7-752976ee3d1e.png)
<br>

## 3. How we spend leisure time?<br>
![screen shot 2018-09-01 at 2 31 43 pm](https://user-images.githubusercontent.com/31684373/44950085-c8a95980-adf3-11e8-867b-b845ef55da8c.png)
<br>

## 4. Which social platform might benefit most?<br>
![screen shot 2018-09-01 at 9 00 17 am](https://user-images.githubusercontent.com/31684373/44950164-ccd67680-adf5-11e8-86fa-9a745bf93fee.png)
<br>
![screen shot 2018-09-01 at 2 48 36 pm](https://user-images.githubusercontent.com/31684373/44950176-22128800-adf6-11e8-9bc0-f0d124f947f2.png)
<br>

## 5. How I simulate users growth?
### 5.1 My understanding of Facebook user growth in the next 5 years
- Based on improving algorithm and data scientists' research, user experience gets better and better.
- Social network has a special attribute: the more connected people in this network, the easier to join, and the harder to leave.
- In most part of world, Facebook has no similar size opponent and no scalable competition.

### 5.2 Two stages of user growth simulation
Based on my understanding of Facebook user growth, I divide the user growth into two stages.
> **5.2.1 User growth before saturation**<br>
Users increase very fast at the beginning, and acceleration slows down when the user base becomes bigger and bigger, and then stagnates at the peak. This user acquisition pace seems perfectly fit the left part of open faced two degree polynomial curve. The basic function is: <br>
$y=b\left(x-a\right)^2+c$ <br>
In this equation, a is the limit time, and c is limit peak, b determines the user increase rate.<br>
If we go further with the equation: <br>
$y=bx^2-2abx+ba^2+c$

> **5.2.2 User growth after saturation**<br>
When users increase stagnates, the popularization rate stay same, and the user increases as the population increases naturally. So I calculate the users number as popularization rate times the whole population.

### 5.3 Some assumptions based on consideration of reality factors
- The US and Canada market is saturated now in terms of number of users. The popularization rate is really high(More than half of the population are Facebook users).
- The Europe, Asia and Pacific and Rest of World market are still not saturated. I assume they will reach saturation at the end of 2021(three years from now). The assumption I made here may be not accurate but reasonable.
- I also assume that the popularization rate in Europe, Asia and Pacific and Rest of World after saturation will be lower than one in US and Canada by 10%, 30%, 25%. The assumption I made here is conservative.

![screen shot 2018-08-31 at 10 43 37 am](https://user-images.githubusercontent.com/31684373/44950190-7a498a00-adf6-11e8-94bd-932533640f14.png)


