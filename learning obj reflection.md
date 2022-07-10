# Learning obj relfection


* Have I met the learning outcomes for this piece of work? If not, what am I going to change?
* LO3 resource, skills, act: 
    * list resources, skills and activities
        * activities i am good at
        * resources and skill could be improved
        * i could have sorted the resources eg data from the start, until an after thought when starting the story that needed the data
        * revisit these lists in tma03, ready to next block of work, making sure i have everything upfront
        * keep working on react native skill. thought it would be more similar to vue

* LO3 resource, skills, act: 
    * list resources, skills and activities
        * activities i am good at
        * resources and skill could be improved
        * i could have sorted the resources eg data from the start, until an after thought when starting the story that needed the data
        * revisit these lists in tma03, ready to next block of work, making sure i have everything upfront
        * keep working on react native skill. thought it would be more similar to vue

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
            * class diagram
                * assocaitions
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
