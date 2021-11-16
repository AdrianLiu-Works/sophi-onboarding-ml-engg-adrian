# Hello!
We cannot wait to have you on-board in our team, but before that, we have designed a ticket, with exact similar structure of what we have in our Jira board for the team. This will help you to know more about us, too. You can imagine the future-you to take one or more of these tickets in every sprint.  

## Ticket name: SOPHI-1234: Design and develop Article Management System

### Goal:
Your project should catalog and organize the news articles present on the Sophi system for the journalists to consume.

### Background: 
The background behind this task is to see how comfortable you are with respect to system design. It also gives a chance to measure your programming skills and ability to design and develop modular code.

### Technical Notes:
* You are expected to do the following:
    - Design a article cataloging system.
    - Assume that the data is being populated into the tables by a data ingesstion system which is not in the scope of this task.
    - The attributes that are available as part of artile are as follows:
      ```
      article_id (string)
      headline (string)
      published_time (datetime)
      publisher_timezone (string) (timezone names from database. ex: America/Toronto)
      article_content (string)
      entities (map<string, list<string>>) (the entities found within the article. An example, entities map would look like below
                                                  {
                                                    'cities': ['Toronto', 'Montreal'],
                                                    'organizations': ['Pfizer', 'RAMQ'],
                                                    'topics': ['health', 'vaccine', 'covid-19']
                                                  }
                                           )
                                           
      ```
    - Address the following functional requirements:
      - Tagging the articles which may be of interest to the domain (like business, crime etc) which the journalist is interested in. Tags are public with-in the system.
      - Searching for news articles. The search is a free text search and additional filters as per the tags that the article is tagged with.
      - The return list of articles should be in the chronological order (or reverse chronological order) of the published time.

    - Following are the non-functional requirements
      - Our service needs to be highly available.
      - Acceptable latency of the system is 1sec for search results.
      - Consistency can take a hit (in the interest of availability); if a user doesn’t see a recent published article for a while, it should be fine.


### Expected Deliverables:
#### Required
* High level system design.
* System APIs in the language of choice.
* Working codebases of the modules and sub-moduels.
* A `docker-compose` file to run the modules.

#### Good to Have
* High level documentation of how you have solved the various problems like scalability, functionality etc.
* Markdown documentation, describing the necessary things, i.e. How to run the code.

### Solution Submission:
* Please fork this repository as a _private_ repository. It is important to keep your solution in a _private_ repository to avoid other potential candidates accessing your solutions.
* Whenever feeling comfortable, you can create a pull request in _your_ repository and add *skbeathanabhotla* as the reviewer.
* When you submit your pull request, *skbeathanabhotla* will add some other team members. The team will review your code. We try to keep our comments limited.
* You have the choice of addressing the comments and squashing your commits into one. The way you handle the comments is important to us.
 
### Good luck!

