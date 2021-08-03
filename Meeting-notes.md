# Meeting Notes

## Meeting 1 (18th July, 2021) - Exploring the problem space

### Key Takeaways - 1

* Need to answer 6 questions (5W1H) about the problem before starting to address it
  * How big is the problem?
  * Why is it a problem? - Root cause analysis
  * Who is the problem affecting?
  * What will change if we solve the problem?
  * Where are we currently and where we intend to reach? - Identifying the gap between Status Quo and ideal situation
  * When of the problem? - Time related aspects (Since when is this a problem, is this regular, seasonal or transient, and how long will it take to address it)?

> Also look at the SMART framework: Specific, Measurable, Action-oriented, Relevant and Time bound.

* Issues with existing media channels - social media or other channels like Television, news etc.
  * Information is very diffused, leads to information overload
  * Important problems often get overshadowed by posts made by popular accounts
  * Lack of updates on the status of a problem posted
  * Misuse of comment space for self-promotion, use by malicious actors and cyber-bullying
  * Lack of actionability and clarity on actions required and outcomes to expect
  * Hard to separate signal from noise
  * Misinformation - hard to know which posts are genuine
  * Lack of transparency and 2-way communication

### Next Steps (till 1st August, 2021)

* Building a basic pipeline to get inputs from social media channels (ingest using twitter api), storing in a database, scheduling requests and allocating to whatsapp accounts (send message via api)
  * Setting up a mongodb database to receive input from twitter api
  * Need to perform analysis on twitter data extracted from api
  * Create a dummy mongodb database and send message through whatsapp api
  * Identifying relevant public data sources and relevant points of contact (people and organizations, both)
  * Literature survey on citizen engagement in addressing social issues

### Areas identified

#### **Low difficulty, High Reward**

* Awareness about Health, Finance, Public Services, Govt facilities, career options
* Aligning educational outcomes with needs of industry and society
* Providing basic sanitation, food and health facilities
* Promoting critical thinking mindset in people to tackle misinformation
* Making people more responsible and accountable for their actions (maintaining cleanliness, pollution, social etiquette) - positive reinforcement instead of negative
* Creating social support system and communities for addressing mental health issues

#### **High difficulty, High Reward**

* Centralization of data in organizations for operational efficiency
* Approachability and transparency in public service interactions
* Modifying incentive structures in organizations to have motivated employees and better outcomes for the workers as well as customers
* Decentralization of essential services - instead of centralized multispeciality hospitals for larger radius, have multiple small emergency and essential care centres for smaller radii
* Increasing investment in research and promoting industry academia collaborations
* Changing people's mindset towards police and the justice system - when seeing something wrong happening people should collectively deal with the culprit instead of waiting for someone to take the first step. Make police and law more approachable
* Dealing with cybersecurity and misinformation
* Credibility checking of research and keeping a check on malicious actors

#### **Low difficulty, Low Reward**

* Enabling supportive social interactions

#### **High difficulty, Low Reward**

* Solving people's procrastination

## Meeting 2 (1st August, 2021) - Start defining MVP and core components

### Key Takeaways - 2

* Used the SPRINT framework by Google Ventures
* Dividing contributors across 4 verticals with leading members in each group

#### **User types**

| User type | Optimizing for | Inputs | Outputs | Challenges |
| ---------- | ------------| ------ | ------ | -------- |
| Post creator | Getting the right resources | 5W1H of the problem + any additional info like in Kaggle | Knowledge repo; Person of contact; Financial help | Incorrect/incomplete info; Need for anonymity, urgency/criticality of situation; Withdraws request/not responsive |
Solver | Maximizing impact | What can they offer (skill, time, money etc), and how much of it; Expectations/addtional requirements from the post creator | Problem info + other updated info on the current status | Acceptance and then cancellations, malicious actors, lack of expertise, not finding the right solver/ no solver available | location or authorization constraints |
| Funding orgs | ROI | TBD | TBD | TBD |
| Knowledge/expertise source | Recognition,; outreach; network | TBD | TBD | TBD |
|

#### **Essential components of our service/system**

* ***Verification/validation on the both ends (problem post creator and solving candidates)*** - Analogy with Uber/Ola can be useful - in team creation, can take inspiration from Uber Pool's dynamics
* Categorization of problems by criticality, volume, urgency etc. (If you're being chased by gangsters - creating a post not really feasible)
* Updation of status, and failure resolution mechanism (if post creator withdraws, or solver cancels etc., expected turn around time etc)
* Specifications and filters (localization, preference for anonymity etc)
* ***Review System*** (Feedback and accountability on both ends) to deal with malicious or incompetent candidates
* ***Finding experts for different categories*** Connect with experts in each domain who'll ensure we are approaching the problems in the appropriate way and minimize unintentional harm due to lack of expertise

### Next steps (till 15th August, 2021)

#### **Group 1: Post Creator**

* Create mockups for post creator user persona, taking into account the highlighed components from above

#### **Group 2: Solver**

* Create mockups for solver side persona, taking into account the highlighed components from above

#### **Group 3: Analytics**

* Identify low risk high volume category to attack first
* Connect with experts and identify knowledge repos for that category
* Define metrics to optimize, and design the evaluation experiment/study

#### **Group 4: Verification/validation/support**

* Study existing literature to find different mechanisms of verification/validation used by businesses and organizations - example - How just Ola perform the background check of the entities involved
* Automated techniques vs manual processes
* Design risk mitigation and failure resolution mechanisms
