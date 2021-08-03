# Effective-social-orgs-analysis

An open source platform to connect problems worth solving to people who have the will and means to solve them

## Key components

* Inputs
  * Interface to allow people to add problems to database (after verification): No junk policy, Twitter integration
  * People can add relevant organizations/funding orgs to the database
  * Could be used to fund independent research projects and allow collaborators to connect
    * Research could be funded to create content and then this content can be of demand in the external countries which can bring income to India and help find its place in the global world order
  * Create their profiles with the appropriate skillsets, interests, and time availability per week - Can connect with LinkedIn and other social media accounts
* Output
  * Notification and recommendations when a match is found
  * Community creation

## Notes

* Follow a test-driven development approach, so documentation and interface first, implementation later
* Keep a log of issues faced and how did you resolve those
* Create a database of relevant funding organizations
* For appropriately allocating problems and as inputs to the recommendation engine, use a small questionnaire like Netflix does to understand your interests. The choices will depend on our study of literature and the problems identified based on twitter data
* Ensure credibility and validation of both the problem and the problem solvers. Having a smaller volume but one you can trust is more powerful than having a large volume but you can't trust the posts or the people involved. This involves doing things that don't scale in the start.

* Define objective function
  * Need to define objective function for our platform. What are we optimizing for?
    * A lot of social media platforms are optimized for attention, which is not directly suited to actually solving problems
    * We need to define the parameters that will govern what aspects we need to focus on
      * **Higher scores good for platform**: Number of problems solved, number of people impacted by the problems solved, number of problem solvers getting engagement, for each person, the ratio of problems suggested to problems taken, the ratio of problems taken to problems solved, rate of resolving reported abuse issues etc.
      * **Lower scores good for platform**: Number of fake accounts and posts, number of reported abuses, number of spam problems, turn around time for resolving abuse, turn around time for problem clarification, time to find the appropriate candidates for solving the problem
  
## Resources

### Dev

* Python: <https://www.fullstackpython.com/table-of-contents.html>
