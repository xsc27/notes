

## [Mind the platform execution gap](https://martinfowler.com/articles/platform-prerequisites.html)  
* _The platform team needs to think of the platform as a software product, needing dialog with its users, attention to reliable operations, and a healthy team environment._
* employees spend their time on value-adding activities ...  
  * One way to achieve this is to use SaaS to outsource functionality that isn’t part of their organisation’s core business.  
  * Another way is to consolidate infrastructure capabilities required by many teams and services into a digital platform  
* The purpose of a developer productivity platform is to allow teams who build end-user products concentrate on their core mission.
* Software engineering excellence
  Build small, simple pieces that you can change independently
  as defined by Kief Morris in his book Infrastructure as Code
* Healthy Teams
  * systems for planning work need to be mature.
     must have backlogs of items described in terms of their value and have processes for prioritisation
   * if too much of the team’s time is consumed with toil, then it will never have the capacity to invest in the improvement of its products
   * Teams should not try to manage too many platform products at once.

### Getting Started
* produce business value, be guided by product thinking, be implemented with operational and software engineering excellence and be backed by a team structure that can sustain the new platform service
* Small, focused platform services targeted at well-understood parts of your technology estate have a lower degree of difficulty.
&nbsp;
1. _what is the smallest thing  [[1]](https://martinfowler.com/articles/platform-prerequisites.html#footnote-tvp)  we can build_ that would help the product teams?
2. how could we upgrade or migrate away from this when the time comes?
   * If deprecating your platform service would require a painful transition over years, it is probably time to go back to the drawing board and simplify your product. 
   * factoring in a realistic lifetime (three to five years) and architectural seams for replacing solutions will force your designs to be simpler and more decoupled.

voluntary adoption of platform

* when product teams have the ability to opt out of platform services, it encourages you to keep your services loosely coupled
* when your platform organisation is dependent on product teams’ appreciation of the platform’s benefits, it puts a strong pressure on your platform organisation to keep customer delight at the forefront of their minds.
* Mandatory migration to the platform is a shortcut that has the long-term risk of eroding your team’s product thinking discipline.

&nbsp;
* platform teams will manage small portfolios of very effective products

**digital platforms succeed by reducing cognitive load on product development teams and accelerating an organisation’s innovation**

XP
* The difference between a team and a group of individuals are the existence of a common set of goals and values (the XP values are communication, simplicity, feedback, courage, and respect) as well as the presence of a high bandwidth, low latency medium that they use to communicate (Sit Together).
* ensure that information about the status of the work is visible at all times, which includes both progress on planned features and observability on running systems (Informative Workspace).
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjEyMDM3MDU5MywtNDk1NzkzOTYxLC0xMT
I0MDA5MTcyLC0xODU0MDAxMzY3XX0=
-->