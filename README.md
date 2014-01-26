giveMeCode()
==========

giveMeCode() seeks to provide an academic environment which allows developers to learn from each other through code submissions and peer review.

Features
========
- Submit questions related to code.
- Provide solutions to posted questions in any language.
- Rate and discuss solutions.

User Stories
============
- [ ] As an anonymous user, I can see recent questions, recent solutions, recent questions by requested language, recent solutions by language, and most active questions.
- [ ] As an anonymous user, I can create a profile based on Google authentication (more providers if possible)
- [ ] As any member, I can post a question with requested languages using markdown syntax.
- [ ] As any member, I can post any number of solutions to any question in any language.
- [ ] As any member, I can up-vote any single solution to a question except my own.  The idea behind voting is to choose your one single answer that you favor the most based on accuracy, readability, and scalability.  A member may change his vote, but should be prompted before doing so.

Opportunities
============
- Learn new programming techniques and solutions through cross language discussion.
- Data analysis can show trends in language use.
- Provide a system for teams and organizations to pre-screen and/or look for candidates to fill positions.

Security Concerns
=================
- Duplicate voting.  IP address, timestamp, and user will be associated with every vote.  Periodic analysis will be needed identify and remove duplicate votes and, if necessary, ban accounts.
- SPAM. At some point, detection of automated spam posting may be required. Disgus will be used for the commenting system with the assumption that Disgus has systems in place to combat spam.
 
Technology Stack
================
What technologies are used in this solution?

Rub on Rails - Server side web API and templating
-------------------------------------------------
Why Ruby on Rails? Based on a quick scan for open positions (particularly on weworkremotely), RoR appears to be quite popular. Ruby claims to be a language built to make programmer's jobs easier. I want to see what the fuss is about.  Also, RoR is supported on both Windows and Nix servers, increasing hosting flexibility.

Heroku - Application Host
-------------------------
Heroku is a PAAS provider with free entry-level hosting that can easily be scaled, should this project take off.  Heroku provides application templates with git-based deployment.  Both of these features help to expedite application startup and ongoing maintenance.

Database - PostGres
-------------------
PostGres is a mature, cross-platform RDBS, and is supported by Heroku and other hosts. As much as I want to play with MongoDB, I feel the number of relationships in this application to be more suitable for a RDBS.

References
==========
Ruby on Rails Tutorial, Hartl, 2014 http://ruby.railstutorial.org/ruby-on-rails-tutorial-book




