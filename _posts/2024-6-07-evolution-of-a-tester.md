# Evolution of a tester

Whilst recently writing a presentation for this years EuroSTAR conference I started examining the role a tester and how this has evolved over the past decade. The following post summarises these thoughts, for a full version of this, check-out my presentation from EuroSTAR which will be livestreamed on 25th July at 2pm BST.

## Definition of a tester

What is the role of a tester? In overly simplistic terms, a testers role is to validate the requirements have been met. How this is achieved of course adds significant complexity to the definition of the role, but even this simplistic definition throws up questions:

1. How are we validating? A huge field in its own right, we have changed our approaches to testing remarkably over the past decade, and I fully expect this to continue to change and evolve over the next 10 years, likely even more remarkably - but this is not a forward looking post...
2. How do we get our requirements? Today Agile methodologies reign supreme over the software development world. The Agile manifesto values "working software over extensive documentation", thats not to say that requirements dont exist, just not in the comprehensive way they once did back in a traditional Waterfall project. With this change, a lot of the knowledge around what "working" means is now shifted into peoples heads. The tester role of "validating requirements" therefore requires the tester to retain large volumes of data about the software, and using that effectively can be a challenge.

So we have an evolution in how we test, and we have a shift in what we define as being tested. Lets explore both in more detail.

## How we test

If you go back 10-15 years, the likelihood is you will find the bulk of software development teams practicing traditional waterfall techniques likely with large teams of testers performing manual test activities. Many teams have explored and have some level of unit testing but the emphasis for the most part is on manual validation using manual black box test techniques.

Back in the late 00's and early 10's, many teams were starting to tackle web application development, single page apps were becoming the norm and the rise of Selenium-WebDriver as the defacto standard tool for web UI automation was cemented. At the same time you had a boom in mobile app development, where Appium and others took a leaf from the Selenium-WebDriver book to focus on UI automation. In both mobile and web application it was common to see teams of testers upskilling with these UI automation tools to replace their manual regression tests.

At roughly the same sort of time, teams were quickly realising that UI testing is not all its cracked up to be, its slow and flaky. API testing became increasingly important to reduce the reliance on expensive UI test techniques.

Alongside the technical test changes, the shift to Agile has meant that work is being delivered by smaller teams who need to be able to deliver software end to end. Typical team make-up shifts from teams of developers and teams of testers to small teams of 6-8, including 1-2 testers. Rapid pace of testing means that  