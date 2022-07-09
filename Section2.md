# Section 2: Review  (2000 words)

## Review of current stage of project work
200 words

_Begin the account of how you feel the project is going. This is not an analysis and evaluation of the work that you have already reported in the earlier sections: this is your reflection on the process you have been going through and what you have achieved. It should include your thoughts on what went well/badly, and you how you would do things differently another time. : as an understanding of the process can be just as important to your personal development as it is to future projects you are involved with._

_Critically review how you have tackled the project.
Has clearly identified examples of effective work and factors that frustrate effective work and considered how they have been managed._

_**Be critical**_

As a whole, I think the project is progressing quite well and I feel in a good position with a few months left. I am mostly proud of creating a working application in React Native, having no prior experience in this framework. The majority of stories from the initial scope have been completed, apart from two, and when interacting with the system, it appears to work with few bugs. 


* how much effort you made*

* What went well? What can I learn from that for the rest of my work on this module?
* What didn’t go so well? How did I recover from my problems? What can I learn from that for the rest of my work on this module?


Another learning has been stakeholder communication. 
* Reflection on process you have been going through
    * requirement gathering
        * learning not to ask so many questions
    * github
        * having each sub task in a card which can have unlimited notes/ images/ tabbles/ adding
        * all in mark down so can copy and paste into assigment
        * the board which makes it easy to move cards and prioritised them
        * cards can have labels, added labels for s/m/l
        * milestones act as the stages
        * helped making me effective
        * so useful to look back at, pull in evidence for various tma's
    * architecture
        * prototype
        * class diagram
            * assocaitions
    * HCI/ mockups
        * lucid chart worked well 
        * could copy paste easily, has lots of components to use
        * helped view what could be reused
    * extra step needed to find resources
        * high risk resources not focusing on
            * What went badly
            * not having data 
            * not having found api for frost dates upfront
    * implementation
        * longer to learn vue than expected
            * What went badly
            * a lot of research dduring the implementation of astory as language was unknown
            * slowing down development
            * could have had dedicated two weeks to learning react
            * was learning on the go
        * story planning
            * meant stories were ready to go
            * technically a agile step to get stories "ready"
            * in analysis requirements meant each story was clear when it came to picking it up, with a mock up, test, acceptance criteria, texual description etc
            * helped influence prgress made
        * postman
            * a quick way of testing the api without thining about front end implementation
            * automatic documentation
            * a tool used in work to better define interfaces
            * could play around with params, urls, check what responses are returned
        * front-end / back-end seperate
            * with back end stories no worries or concerns as confident in rails development
    * testing
        * should have done ,more as went along
    * feedback
        * having friends and family to prioritise stories, and provide feedback

* Right at the end of your work on the module another useful question is: What would I do differently if I did the project again?

* How you would do things differently another time
    * dedicated time to learn vue
    * dedicated time to find resources
        * hard when your not 100% what you need though until implementing
    * think about non-functional requirements more and add stories for them
        * didnt add story about adding ux thruogh. involved researching and choosing a library, testing etc
        * could split out research stories about which library to use
    * although a app was prefered from initial requirements, could have spent more time looking into other options
        * web app might have been easier but wouldnt have learnt vue
        * web apps are now websites just displayed on decive in a good way which could have worked  
    * lifecycles
        * discussed in section ..
    * plan before project start date
        * time between start and tma01, although short, dont feel like i did lots
        * but i did get a prototoe of the vue or cordova request to rails data which was good to fundamentally see it working



## Project Management
1530/500 words

Review your project management. Identify those elements of your plan that have not progressed as satisfactorily as you expected and briefly record the reason(s)

**LO9**: Plan and organise your project work appropriately, and keep systematic records of plans, progress and outcomes.
**Has a clear plan and makes an accurate assessment of progress in relation to the original plan. Understands what has gone well and what has not gone to plan.**


### Lifecycle

Initially, I started the project following a KanBan approach (ref). However, the process felt to big for complex for a person project with too many moving parts, as there could be multiple tasks at play at any one time, left me feeling overwhelmed. After some research. I found WaterScrumFall, a hybrid Agile method which combines Waterfall and Scrum, where Scrum is inserted into the middle of the Watefall cycle. Appendix 24 provides a comparison table of the other lifecycle approaches which were considered and tested. 

As WaterScrumFall has three distinct phrases, the first being "Water", it provided the upfront structure of Waterfall, which I wanted as I was closely folling TM354 Case Study steps which were in a Waterfall approach. I was able to gather and analysis requirements, design the database and HCI designs and complete as much upfront preparation as possible which the project benefitted from. 

The "Scrum" approach to implementation allowed me to develop an MVP, which took four weeks. I was able to have users verfiy the system, provde feedback (as shown in Appendix ...). From this, I generated the "Improvement", or "Version 2" stories. This has been great becuase although I get upfront requirements, users don't know exactly what they would like until they have sometime to test and look at. On think I haven't dont much of is testing, as I have felt the pressure to get a working software, which is something I'm going to work on over the next iteration. I now have a small group of stories which I will discuess in section x, as part of the upcoming plan. 

The final "Fall" phrase, will be the "release" the the software. I will again gather feedback from users. As a whole, I think WaterScrumFall has been a well suited and efficent process for this project. More discussion of its effectiveness will be included in the final report. 

### Plan

From MVP feedback, 15 new stories were created. For each story I gave it a size: Small, Medium or Large, where I would expect small to take less than a day, medium a day, and large over a day. After sizing them up, and putting them in order. To decide on this priority order, I noted how many times a feature was mentioned by users, and then considered the size and value of the stories. With small cost and high value first. I added them to the original Gantt Chart (appendix ..) under TMA02 and before report. However, there was not enough days to complete them all, before starting the critical start date of EMA writing. 

The stories which are high cost in time, low in value have been moved to the back log. (The large tag is still on them, and the order will remain, so if any spare time I can go and pick one up, however this is very unlikely.) This leaves 10 remaining stories: five small, two medium and three large. Six of these stories are relative simple UI changes which will made a big difference to the usability of the application, for little effort, such as adding colour, text description and images. For example, adding a button to add a vegetable from the plot screen should be straight forward as the button will simply re-navigate the user to the Vegetables screen. These are all "Small" apart from "Add vegetable images" is Medium because although it will be straight forward to replace an icon or image for another image, it may require more time sources freely available images. The other Medium story "Stub frost dates", as it involves both the front and back-end applications. However the architecture for this is already in place, as it involves only adding an attribute on a "Plot", so I don't expect it to take long. 

The remaining three larger stories involve the removal of a location on a plot. This is a non-regotiable becuase it is a requirement identified from Legal research. Additionally, The ability to remove a veg from a plot is also critical to a the system, as it was identified as a core component, and the system would be much less useful without the flexibility to change ones mind on what to plan. The final task is Testing, specifically unit-testing for both back-end and front-end, which is crucial to ensuring the quality of the software and that there isn't any unexpected bugs. I am hoping to complete all the small and medium stories next week; five small stories over two days and the two medium stories over two days. Although this will be a push, I then go on holiday for a week, and so I don't want to get stuck on a bigger problem just before I leave, but would rather complete as many smaller stories as possible. When I get back from holiday, I have then only two implementation stories. The final Large story is testing, which will actually take a much longer than a day. 

Once I return from holiday, for nine days, there will then be a few tasks in parallel: The focus will be on testing, but during this time I will also gather user feedback, as that is not dependent on testing. I will process this feedback as it is returned. Both of these tasks will let me know when I have achieved my goal (verfification? from UAT), and done to a satisfactory standard (validation?) After feedback is returned, I will hopefully have a few days to plan the EMA. For planning the EMA report writing, I plan on creating a new GitHub column on the board, and break down the sections into stories. 

I then have a wedding weekend away. I'm hoping this will be a nice rest before the final 40 days that are schedules to complete the EMA report. The final week in August which shows unavaiable, is my sisters wedding. I am on annual leave that week and hope to do a few hours of EMA work each day. However, the two weeks prior to this, I hope to get the majority of the report written. Finally, as I have another wedding the Friday before the EMA deadline, I am hoping to hand in the EMA a few days early. 

The Gantt chart in Figure x shows this updated schedule. 

* what you learnt from comparing what you originally planned to do with what you actually did
* how you had to replan

_**In reflection you might want to say something about the way you work and when.   e.g short bursts or long sessions.  Night v day, etc.**_

![gantt chart updated with improv.png](../../Zettlr_Images/gantt chart updated with improv.png)

figure x: 

screenshot of githubt tasks in order


### Resources

To complete the above, Figure xxx shows a list of Resources that are already in progress and have been updates, or new ones to complete the final version of the system. 

**Update on google doc [here](https://docs.google.com/document/d/1FRhyFJ68vzqCTjrjw2GzF3NQp2sAX56PnLrAv1ZJnqU/edit#)**


|                      |                                                                    |                                                                                                                                                                                                                                                                                                                   |
|----------------------|--------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Resource             | Why needed                                                         | How to obtain                                                                                                                                                                                                                                                                                                     |
| Stakeholders         | Gathering requirements, provide feedback and testing final product | I am in frequent communication with 13 stakeholders.                                                                                                                                                                                                                                                              |
| Vegetable Data       | Populate vegetable information in tables                           | I was unable to find sufficient vegetable data. I have manually added vegetable information from my book. This is stored as a Rails seed, which is a configuration file which can be ran on database set up. Automatincally inserting each row in the relevant databases. Appendix shows screenshot of seed code. |
| XCode                | Emulator the hybrid application locally                            | Installed. Working well                                                                                                                                                                                                                                                                                           |
| Expo                 | Easy testing of app by scanning a QR code                          | Downloaded the software and installed the iOS app. Working well                                                                                                                                                                                                                                                   |
| Ruby on Rails        | To build the back-end service                                      | Installed                                                                                                                                                                                                                                                                                                         |
| React Native         | To build the front-end UI                                          | Installed                                                                                                                                                                                                                                                                                                         |
| Weather API          | To retrieve frost dates for a users location                       | I was unable to find a frost date api based of location. I found one for america, but not UK. Going to stub out this data and assume usage is only in UK. Based on Cambridge. Frist: 11th Dec. Last 20th April, (ref plantmaps)                                                                                   |
| GitHub               | Version control code and Project Board                             | I have created a project and a repository.                                                                                                                                                                                                                                                                        |
| LucidChart           | Build Mock ups, ERD, activity diagrams etc                         | I have an account through work                                                                                                                                                                                                                                                                                    |
| Zettlr               | To write assignments in markdown format                            | Downloaded. Creation of tables is temperamental. I am creating tables on Google docs and adding them in later.                                                                                                                                                                                                    |
| Zotero               | To store and manage references                                     | Downloaded                                                                                                                                                                                                                                                                                                        |
| Postman              | Test API and provide documentation                                 | Downloaded and working well                                                                                                                                                                                                                                                                                       |
| React Native library | For providing “Tips”                                               | ReactNativeMaterial Banner/ Dialog/ dismissable snack bar                                                                                                                                                                                                                                                         |
| React Native library | Add button to veg                                                  | Floating button [<ins>https://www.react-native-material.com/docs/components/fab</ins>](https://www.react-native-material.com/docs/components/fab)                                                                                                                                                                 |
| React native         | Location checkbox bigger, switch                                   | [<ins>https://www.react-native-material.com/docs/components/switch</ins>](https://www.react-native-material.com/docs/components/switch)                                                                                                                                                                           |
| React native library | Welcome text                                                       | Dialog. Aware they get annoying. Will only use once at the start. Work out what to say                                                                                                                                                                                                                            |
| library              | Remove veg from plot                                               | Also use [<ins>https://www.react-native-material.com/docs/components/fab</ins>](https://www.react-native-material.com/docs/components/fab)                                                                                                                                                                        |
| images               | For vegetables, preferable odd shaped                              | Fine freely available                                                                                                                                                                                                                                                                                             |
| RSpec                | For back end testing                                               | Already installed and set up                                                                                                                                                                                                                                                                                      |
| Jest                 | For front end testing                                              | To install and set up [<ins>https://jestjs.io/</ins>](https://jestjs.io/) ref                                                                                                                                                                                                                                     |

## Risks
485/ 500 words

_Assess the risks to project completion (remember that this is not the same as whether you expect to pass or not). Identify any significant risks to project completion and determine how these are going to be managed. Identify those elements of the project that may not be addressed if plans need to change

_**LO3**. Identify, list and justify the resources, skills and activities needed to carry out the project successfully. Identify and address any associated risks
**Has identified the resources, skills and activities, the timely availability of which is essential. Has judged risks (likelihood and impact) appropriately. High-risk elements have been excluded and other risks are manageable**_

_* Assess the risks to the availability of resources you need to complete your project
    * Include table with all risks even no longer viable ones (highlight those in pale colour)
    * Discuss whether right ones chosen at start or some added later or not wanted / why_


By this stage you should be able to write about the risks you had initially identified, the strategies you had identified to mitigate them, and possibly about how effective these were. You may also identify any risks that may still occur before completion and how to mitigate them.

 I have evaluated the risks of the resources stated in figure .., noting which are no longer at risk. New resources required for the final version of the system have been added. A list of skills associated with the project is provided in Appendix 27. 

**Update on google doc [here](https://docs.google.com/document/d/1FRhyFJ68vzqCTjrjw2GzF3NQp2sAX56PnLrAv1ZJnqU/edit#)**

|     |     |     |     |
| --- | --- | --- | --- |
| Risk | Impact | Likelyhood | Mitigation |
| Stakeholders availability | M   | L   | I will message the stakeholder prewarning them that I will be sending over a final questionnaire with the system. I am in frequent contact with 7 stakeholders. 7 is probably enough to test the system, therefore this risk is low |
| Vegetable data access | H   | L   | Create manual Rails task to input vegetable data, using the book “Allotment: Month by Month” to provide information. This is no longer a risk |
| Hybrid technology limited experience | H   | L   | I completed the two courses, “Learn the basics” and “Introduction” on React Native documentation. I have read alot of React native documettion during the development and improved knowledge alot. I have nearly completed all react native development. So this is no longer a risk |
| Location sensor acess | M   | L   | Implement geolocation feature found and implemented successful. No longer a risk |
| Weather API access | L   | L   | Unable to find and api, so frost dates have been mocked. No longer a risk |
| Project management limited experience | H   | L   | Continue reading “Projects in Computing and Information Systems. A Student’s Guide”. I might take this on holiday to finish it. Nearing the end of the project, this is less of a risk as have a clear plan on how to complete |
| Lifecycle not fitting | L   | L   | Since TMA01, SDLC has changed and and WaterScrumFall is fitting well. No longer a risk |
| Project scope to large | M   | L   | Since TMA01, the scope has been refined to a reasonable amount. Feedback from the V1 MVP has been limited to a reasonable amount, although there is still quite alot to do. I think it is possible. This risk is small. |
| Not enough time | L   | M   | Keep to the project schedule. The project schedule has been updated with tasks for the final section of V2 improvements. I will then use GitHub storys to keep on top of EMA report writing tasks. This has the most risk currently. |
| Change in requirements | L   | L   | Initial questionnaire and mockup feedback reduced this. Feedback from V1 further reduces this as users know what to expect. No longer a risk |
| Images not found | L   | M   | I am going to use images that I have taken of our plot. These images will be used on the the vegetable detail page |
| Vegetable icons not found | L   | M   | I was hoping to use icon for the timeline. If I cant find any, I can use the images above |
|     |     |     |     |

## Review your personal development
1000 words
**LO8**. Learn independently and reflect on what has been done, with a view to improving skills and knowledge.
**Makes progress under own supervision, communicating regularly and accurately in respect of progress. Seeks guidance when needed, but offers own ideas when doing so.**

what have you gained as a person
* what personal benefits you gained through doing the project.


How is it all going, project wise/ learning objectives

* Have I met the learning outcomes for this piece of work? If not, what am I going to change?

* LO2 refine goals: 
    * feeling more confident at refining the goals as there are less unknownws
    * sattekholder feedback crucial
    * benefitted learnt alot from LSEPI and EDI issues
        * added stories 
        * wouldnt have considered
        * now will take with me
        * UX too
    * subset of initial stories kept focus
    * requirement gatehring
        * For the initial questionnaire, I hadn’t considered how I would analyse the results. Although the 42 responses came steadily, fewer questions would have sufficed. Nevertheless, the responses were still incredibly helpful to the project. The “Timeline vs Task vs Calendar” questionnaire instead included one question with three multiple choice answers, which was much easier to process. (Appendix 5)  An important factor in designing questionnaires is to think how the information will be processed.
        * A lot more answers than I was expecting. In retrospect, I would have had fewer number of questions as it is a lot of answers to go through


* LO4: gather information
    * gather: 
        * hard to understand what lit review was at the start, first time doing it
            * resources helped
            * attended a tutorial helped
            * bit llate on this front
            * if i had known, might have gathered more at the start
        * process half working, zotero plug in in chrome means i save everything i look at
            * then cross ref from journal notes
            * try to add note directly into zotero at the time, will save time later
            * lit review
                * My biggest improvement has been my understanding and appreciation of literature sources. I learnt how to use the OU Library by watching the practical tutorials and as a result, I believe I have found better sources. I particularly enjoyed learning about the benefits of home growing and software accessible. 

    * analyse: 
        * Moscow helps in back of mind
        * alot are for small bugs which stack overflow solves, and analysis is whether it works or not
        * not sure whether to include these?
        * not working in acedemic stuggled to know what was good and bad
        * alot of paper very complex and long, time consusming to read
        * UI timeline
            * How to show timeline/ big learning: timetable. compared many table calendar table timetiable Gantt chart Tables Calendars Timetables Gantt chart/ Data grid/ data table Timetable [story](https://github.com/harrietc52/TM470/issues/9) mockup [story](https://github.com/harrietc52/TM470/issues/62)

* LO6 variety of sources: 
    * use variety of sources, demonstrate awareness of credibiliity
        * use variety of sources
            * could do more?
            * handful of resources in the end that really influenced project
                * with lots of little supporting ones
            * doing this quite alot 
        * demonstrate awareness of credibiliity
            * not doing alot of this
            * one for improvement
            * lit review for tma03 said only moscow as a tool to choose sources, but not write about. but this suggests i should still reference if it is a twice reviewed etc
            * not sure how best to implement this one

* LO7 communication:
    * communicate information, ideas, problems and solutions clearly
        * i think i am meeting this outcome quite well?
        * learnt how to better use postman and see the benefits of it
        * enjoying writing up about what i have done, its just timeconsuming, hard to know how much to put in main body or appendix
    * mockups
        * appreciate value of hci designs
        * enjoyed learning how to come up with them
        * things you expect but never think about why
        * Creating the below mockups was an invaluable activity. Shared components such as Vegetable Lists or Details were discovered and visualising CRUD actions made me think about data dependencies. For example; When a selected vegetable is removed from a plot, should its associated notes be destroyed to? Appendix 13 contains Stakeholder feedback for the mockups, which was quite positive. 

* LO1: technical aspects 
    * technical concepts
        * expo location
            * expo location access of device, with explict consent [@expo_location_nodate] 
        * database design 
            * How to store data, specifically timetable. 
            * use of config, as rarely going to change. 
            * and db doesnt like lists
            * where should this infomation be stored?????
            * Moved from plot veg, to just veg, and plot veg was needed when the data would be different depending on location
            * But now not using location / frost dates to influence all the same
            * So consistent for all veg
            * So moves class
            * for now, going to store timeline as comma seporated list in DB column, can the
            * use split when in the UI to convert to list
        * installation of expo 
            * test locally
        * rails appliaction from scratch
            * learnt lots
        * will reflect on jest and rspec later
        * npm
            * NPM/yarn install. A `.nvmrc` file containing a node version number was created to automatically use the specified versious. 
        * UI framework
            *  https://mui.com/x/react-data-grid/ * (react not react native)
            * ***https://callstack.github.io/react-native-paper/data-table.html **Using this one

* LO8 independent learning:
    * learn independently, and reflect on what has been done, with view to improving skills and knowledge
        * learn independently
            * made progreess when stuck?
            * havent needed to ask too many technical questions
        * reflect on what has been done
            * could send tutor more updates
            * keeping in touch with tutor (example in appendix)
        * prototype
            * proud when solved problems, like the initial prototyoe security one
            * When developing the React prototype, similar security issues to the Vue prototype resurfaced. I relaxed the CORS constraints in the back-end and added headers to requests, resulting in a different Network error: iOS does not allow HTTP requests. I then served Rails on HTTPS using a Self-Signed Certificate. This worked on my laptop’s emulator but not my phone because the request to “localhost” from my phone, was understandably, not reaching my laptop.
            * I updated the request to point to the laptops IP address. The request was now timing out, instead of failing, which was progress. A Stack Overflow answer (Rice 2019) solved this exact problem. Rice suggested binding the Rails server to 0.0.0.0, which was successful as my phone accessed bank-end data over the internet. This internet dependency was confirmed when I continued development in the car. I then hot spotted to access the internet, which changed my laptops IP address because of the different network. Updating the front-end request to use the new IP successfully served the back-end data again.
            * The development of working prototypes for both Vue Cordova and React Native was a big learning curve, yet carrying my learning experiences from one prototype to another was very rewarding. I then felt in a strong position to choose between the two, knowing they both fundamentally work.
        * react native
            * better understand redux
                * Central state, redux vs useState and useEffect. Have a container for each of the main 3 tabs, which gets initialised with the state and actions it needs. But plot pages needs to aaccess list of vegetables to be able to filter the vegetable list with selected vegetables, so state is shared. thi s culd be improved as mentioned else where, currently getting ids for selected veg from plot api, but could add scope to plot vegetables to filter plot vegetables by plotid. 
            * react native lifecycle hooks
                * Navigation.Passing as a prop to chld components and Passing actions as prop. how to Class components vs functions. Using classes as components so useEffect not available. Biggest learning current was Reactivity, and how to use componentMount and unmount and update. for example When adding veg to plot, which clicking on plot page, want to automatically refetch plot. Constraint as fetch for veg list in plot is getting plot?include=plotVegetables, where as is veg list was separate component with own state, rather than central state, could be given a plot id and go get its own veg on render. But as its plot veg, need to re fetch the plot for it to update. Learning got in an infinite look at one point, when fetch was in update function

* LO3 resource, skills, act: 
    * list resources, skills and activities
        * activities i am good at
        * resources and skill could be improved
        * i could have sorted the resources eg data from the start, until an after thought when starting the story that needed the data
        * revisit these lists in tma03, ready to next block of work, making sure i have everything upfront
        * keep working on react native skill. thought it would be more similar to vue


* LO9 plan, organisation:
    * plan and organise project work
        * one of my better ones, thanks to github
    * keep systematic records of plans
        * gantt chart
            * found so helpful especially when planning how much work can fit in to do scope
    * keep systematic records of progress
        * journal - could be better at
            * Since TMA01, I have used my Project Journal (Appendix 15) much more. Stating what I have done each session and plan to do next, has helped when revisiting project work days later. The GitHub board and cards have been a very effective way of storing associated requirements, diagrams and research. This also made TMA02 easier to compile.
        * enjoyed log keeping, will try to do this more in professional life
            * example in appendix
    * keep systematic records of outcomes
        * taking screenshots for each feature,
        * need to add tests after features
    * tried lots of lifecycles
        * from implmeenting scrum for a few weeks, waterfall for a 2 months then waterscrumfall for majority, learnt a bit about all of them
    * project maagement
        * Continue reading “Projects in Computing and Information Systems. A Student’s Guide”.
        * take on holiday
    * work life balance
        * with 2 months left, still alot of time. gradually feeling myself buring out. espeically at work. need to take time away. 
        * its a very busy time at the moment and uni is taking every evening and all weekends, making less work life balance
            * going to work on this for the final few months as I would liek to enjoy last months of uni after 6 years 
        * after tma02 was other tm358 ema
            * three full weeks not looking at this project
            * it was scheduled in the plan, which i am glad
            * but knackered after that to get back on coding work was hard
            * should have given myself a few days rest after ema

  
Learning LO10, LO11 and LO5 (Appendix 29)

## Tutor

* whether to include smaller stack overflow posts somewhere
* lo6: develop and demonstrate ability to effective use of sources, and demontrate awareness of credibility. how to do the latter?
* level of my writing formality ok?
* who is the intended audience of the report
* would you like more updates
* the way the learning objectives have been grouped, is there anything telling about that/ why which lo have been placed together


