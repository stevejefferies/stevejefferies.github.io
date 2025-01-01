# Evolution of a tester

Whilst writing a presentation for 2024's EuroSTAR conference in Stockholm, Sweden, I started examining the role a tester and how this has evolved over the past decade. The following post summarises this conference talk into a condensed blog post. You can also check-out a full recording of the presentation entitled "Becoming a Better Tester by Getting Involved in Everything" which was recorded as part of EuroSTAR's post-conference virtual event. This is available [here](https://www.youtube.com/watch?v=MtWtePxCfR4).

## Definition of a tester

What is the role of a tester? In overly simplistic terms, a testers role is to verify the requirements have been met. How this is achieved of course adds significant complexity to the definition of the role, but even this simplistic definition throws up questions:

1. How are we verifying? A huge field in its own right, we have changed our approaches to testing remarkably over the past decade, and I fully expect this to continue to change and evolve over the next 10 years, likely even more remarkably - but this is not a forward looking post...
2. How do we get our requirements? Today Agile methodologies reign supreme over the software development world. The Agile manifesto values "working software over extensive documentation", thats not to say that requirements dont exist, just not in the comprehensive way they once did back in a traditional waterfall project. With this change, a lot of the knowledge around what "working" means is now shifted into peoples heads. The tester role of "verifying requirements" therefore requires the tester to retain large volumes of data about the software, and using that effectively can be a challenge.

So we have an evolution in how we test, and we have a shift in what we define as being tested. Lets explore both in more detail.

## How we test

If you go back 15-20 years, the likelihood is you will find the bulk of software development teams practicing traditional waterfall techniques likely with large teams of testers performing test activities manually. Many teams have explored and have some level of unit testing but the emphasis for the most part is on manual verification using manual black box test techniques.

Back in the 00's and early 10's, many teams were starting to tackle web application development, single page apps were becoming the norm and the rise of Selenium-WebDriver as the defacto standard tool for web UI automation was cemented. Shortly after you had a boom in mobile app development, where Appium and others took a leaf from the Selenium-WebDriver book to focus on UI automation. In both mobile and web application it was common to see teams of testers upskilling with these UI automation tools to replace their manual regression tests.

At roughly the same time, teams were quickly realising that UI testing in general is not all its cracked up to be, its slow and flaky. API testing became increasingly important to reduce the reliance on expensive UI test techniques. We started pushing more testing lower down the test pyramid, with increasing technical complexity. This trend continues today, a modern microservice architecture will employ a huge range of test levels to effectively test a service at speed. A great example of this is [Tom Clemson and Martin Fowlers guide on microservice test strategies](https://martinfowler.com/articles/microservice-testing/). Whilst now 10 years old, this guide shows the heavy shift towards more complex technical testing strategies and mostly holds true today.

Alongside the technical test changes, the shift to Agile over the past 20 years has meant that work is being delivered by smaller teams who need to be able to deliver software end to end. Typical team make-up shifts from teams of developers and teams of testers to small teams of 6-8, including 1-2 testers. Rapid pace of development requires testing is built in continuously, you no longer have testing running weeks or months behind development. If you want to ship quickly, you need to test almost as soon as you make a change to the code. Teams high demand on testing has only added to the continuous pressure to deliver quicker test capabilities, using effecient test techniques, often at lower and more technical levels in the test pyramid.

## Shift Left

This shift towards earlier testing, lower down the test pyramid, is often associated with the term "Shift Left". Today the term is conflated to mean anything that can be shifted earlier in the lifecycle, but applied to testing it focuses on earlier test involvement and rapid, effective testing.

What about the role of a tester in a development team then? Well with this increased shifting in test focus to lower test levels, the expectation has become that testers need to be able to become more technical - undoubtedly we now expect testers to be involved in defining (and in many cases implementing) tests down to the unit level. Certainly reviewing PR's has become increasingly normalised in the role of a tester. There are very few test roles on the market today which do not come with some degree of technical code experience as a requirement.

## Shift Right

On the flip side of shift-left, we have realised that in this world of rapid software development we can't (and shouldn't) test everything. If we can ship software quicker, can we accept a level of risk by not testing everything and instead shifting some aspects of testing onto our production systems. This is the premise of shift-right - do things later (ie in production), such as monitor performance of a new feature when its in use, rather than extensive upfront testing.

This is great, it gets us closer to our customer and as testers, too much shift-left into technical low levels can be harmful - you loose the big picture. However shift-right comes with its own challenges, dealing with access to production systems, customer data sensitivities and correct data handling requires a tester to understand and practice safe use and operation of such systems and data.

## Shift Everywhere

So we have these competing priorities:
- **Shift-Left** - performing test activities earlier, often with higher degrees of technical understanding. Undoubtedly more effecient, but at the risk of loosing independence and big picture thinking
- **Shift-Right** - performing test activities later, using monitoring and testing in production systems. Increasing risk of introducing failures into production, but balancing this with quicker delivery.

In reality most teams today, certainly those working effectively are bridging both. We expect our testers to simultaneously be technically savvy, whilst also understand and be able to understand the big picture by testing in production.

Those testers who can effectively "shift everywhere" are in high demand, they are incredibly valuable to their team. 

Many of the issues experienced today by software development teams can be reduced or removed entirely by having suitable test resources on the project who have this "Shift Everywhere" mindset, For example:

- Not building the right thing, resulting in redesign and rework. Sure this is partly Agile but theres no excuse for fundamentally building the wrong thing. A tester able to get close to the customer, who can think like an end user can rapidly pick up on gaps in requirements or approach.
- Not understanding the level of risk and implementing and effective test strategy. A good tester should be able to design a well-rounded test approach taking into account technical detail (shift-left) and acceptable risk profiles (to allow shift-right)
- Slow delivery. A tester who cannot adapt to working in a "Shift Everywhere" approach will likely duplicate effort in testing or certainly not advocate for the right level of testing, resulting in slower CI and regression cycles, slowing down the delivery vehicle.

## What we Test

Alongside how we test, is the change in what we test

## Risk Heros

Extending the concept of "Shift Everywhere", testers today have become masters of risk. A good tester on a team can handle risks from different origins to help provide an effective test strategy. I describe this person as a "Risk Hero", someone who can take the key pillars of risk and apply them to any project. These testers are again incredibly valuable to the team and should be sought after and retained for effective software delivery. A tester looking to further their career should look to these risk pillars as a way to add additional value in an industry continually under scrutiny in terms of value add vs other software engineering roles.

### Risk Pillars

The four main risk pillars I see today:

1. **Business risk** - these are risks that your specific business is willing to accept (or not). The risk profile of a small start-up may be fairly risk tolerant, taking on more risks to enable them to move quickly in the market. Compare this to a large market-leader in an industry, who will commonly be risk-averse and will look for stability and high levels of quality, but often at a cost of quality.
1. **Client risk** - this is associated to the level of risk your client is willing to take on. Primarily delivering to end-users, at a low cost point? These users are likely to accept a lower level of stability and potentially quality in their product compared to a large enterprise client with a multi-million dollar contract. 
1. **Technical risk** - associated with the risks that stem from the technical implementation of the project. Knowing your technical risks will often require a tester to wade into conversations with architects, lead engineers etc.
1. **Regulatory risk** - industry specific, these are risks associated with regulations either in place today which you or your clients must adhere to, or are new regulatory changes on the horizon. A good tester keeps up with regulatory changes, dont wait for legal teams to push regulatory changes down, be proactive to the changes.

Becoming a risk hero requires you to master all four pillars with respect to your project and industry. Doing so creates an effective test approach for your project and makes the tester role incredibly valuable.

## Can I not just test?!

Much of the presentation and this blog post focuses on the broadening of the testing role. You may be asking yourself, wheres the time for "testing"? Answering this depends on your definition of testing though, as yes if you are thinking that testing today just involves things such as:

- writing test strategies, plans, scripts
- performing exploratory (experience based) testing
- raising and re-testing bugs
- performing regression teting
- writing test reports

Then yes, there is less scope for this in todays software tester role. However the role has shifted, an effective tester today focuses on value-add throughout the SDLC, with actvities such as:

- reviewing code, architecture, feature design
- implementing test tooling
- shadowing (and supporting) other teams in the business - sales, support, operations
- training on regulations
- conducting usability reviews
- coaching and mentoring developers

All these activities provide value to the business, whilst increasing the knowledge for the "core" test activities which today are evermore reliant on experience and broad knowledge levels.

## Want More?
 
This is a short summary of a presentation given at the EuroSTAR conference in Stockholm, Sweden in June 2024. There is a recording available of this talk which was given after the conference as part of the "EuroSTAR Virtual Days" which explores some of these themes in more detail. Click the link below.

[Becoming a Better Tester by Getting Involved in Everything](https://www.youtube.com/watch?v=MtWtePxCfR4)