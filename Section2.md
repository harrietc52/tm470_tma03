# Section 2: Review

## Review of current stage of project work

I think the project is progressing well and I feel in a relatively good position. The majority of stories from the initial scope have been completed, apart from two, and when interacting with the system, it appears to work smoothly with minimal bugs. 

Reflection on the use of tools that are helping the projects effectiveness, such as Zotero, Postman, GitHub and Gantt Chart are considered in Appendix 23; this also includes reflection on my Project Journal keeping (Appendix 25). Time spent creating user stories, mock ups, testing criterial, texual description etc meant when it came to executing a story, I had a clear idea of what needed to be done, which definitely increased effectiveness. I am also grateful for my stakeholders, who responded quickly to questions and feedback requests. Having the prioritisaiton of stories based on their feedback has been benefitial, as I would have prioritised different features, making the application less useful. 

If I were to do the project again, I would first schedule time upfront to learn more about the chosen language. I would also create a story for each of the research tasks, such as those resources identified as high risk. I left researching tools, or APIs, such as the weather API or gathering vegetable data until starting the story, at which point it was almost too when, as my schedule has only considered implementation timings. I would have made stories for UX improvements. For example, I hadn't a story about creating the navigation bar at the bottom of the screen, becuase I hadn't given it much thought. Although it appeared in the mock-ups, my stories were created from user requirements, where they understandly, assume there is some sort of navigation, and therefore don't state it. It also took a few hours work to test a few different navigation bar component libraries before choosing one and a story could have tracked this work more transparently.  

Throughout, I would have liked to do more testing. When estimating story times and my project schedule, I should have factored in an extra hour for each story to implement tests. I did some basic test-driven development when I was struggling on something particular, however I will now go back and add some more. Although an app was prefereable from initial requirements, I could have spent more time looking into other options, For example, web apps are now websites just displayed on decive in a more effective way, which could have worked. However, I wouldn't have got to learn React Native. Further observations about how I tackled the project are inlcuded in Appendix 25.

## Project Management

I am finding myself working on smaller fixes, planning or writing up notes, in the morning before work for around 45 minutes. The majority of the codeing work is done most evenings for around two hours. I am also given one study day a week through work, to spend time on module work, which is when I have been doing most of the report writing as I find this easier to do in longer sessions.

### Lifecycle

As WaterScrumFall has three distinct phrases, the first being "Water", it provided the upfront structure of Waterfall, which I wanted as I was closely folling TM354 Case Study steps which were in a Waterfall approach. I was able to gather and analysis requirements, design the database and HCI designs and complete as much upfront preparation as possible which the project benefitted from. 

The "Scrum" approach to implementation allowed me to develop an MVP, which took four weeks. I was able to have users verfiy the system, proivde feedback from both the mock-ups (Appendix 19) and MVP (Appendix 24). From this, I generated the "Improvement", or "Version 2" stories. This has been great becuase although I get upfront requirements, users don't know exactly what they would like until they have sometime to test and look at. On think I haven't dont much of is testing, as I have felt the pressure to get a working software, which is something I'm going to work on over the next iteration.

The final "Fall" phrase, will be the "release" the the software. I will again gather feedback from users. As a whole, I think WaterScrumFall has been a well suited and efficent process for this project. More discussion of its effectiveness will be included in the final report. 

### Plan

From MVP feedback, 15 new stories were created. For each story I gave it a size: Small, Medium or Large, where I would expect small to take less than a day, medium a day, and large over a day. After sizing them up, and putting them in order. To decide on this priority order, I noted how many times a feature was mentioned by users, and then considered the size and value of the stories. With small cost and high value first. I added them to the original Gantt Chart (Appendix 27) under TMA02 and before report. However, there was not enough days to complete them all, before starting the critical start date of EMA writing. 

The stories which are high cost in time, low in value have been moved to the back log. (The large tag is still on them, and the order will remain, so if any spare time I can go and pick one up, however this is very unlikely.) This leaves 10 remaining stories: five small, two medium and three large. Six of these stories are relative simple UI changes which will made a big difference to the usability of the application, for little effort, such as adding colour, text description and images. For example, adding a button to add a vegetable from the plot screen should be straight forward as the button will simply re-navigate the user to the Vegetables screen. These are all "Small" apart from "Add vegetable images" is Medium because although it will be straight forward to replace an icon or image for another image, it may require more time sources freely available images. The other Medium story "Stub frost dates", as it involves both the front and back-end applications. However the architecture for this is already in place, as it involves only adding an attribute on a "Plot", so I don't expect it to take long. 

The remaining three larger stories involve the removal of a location on a plot. This is a non-regotiable becuase it is a requirement identified from Legal research. Additionally, The ability to remove a veg from a plot is also critical to a the system, as it was identified as a core component, and the system would be much less useful without the flexibility to change ones mind on what to plan. The final task is Testing, specifically unit-testing for both back-end and front-end, which is crucial to ensuring the quality of the software and that there isn't any unexpected bugs. I am hoping to complete all the small and medium stories next week; five small stories over two days and the two medium stories over two days. Although this will be a push, I then go on holiday for a week, and so I don't want to get stuck on a bigger problem just before I leave, but would rather complete as many smaller stories as possible. When I get back from holiday, I have then only two implementation stories. The final Large story is testing, which will actually take a much longer than a day. 

Once I return from holiday, for nine days, there will then be a few tasks in parallel: The focus will be on testing, but during this time I will also gather user feedback, as that is not dependent on testing. I will process this feedback as it is returned. Both of these tasks will let me know when I have achieved my goal; User Acceptance Testing for Validation, and testing for Verification [@open_university_verification_nodate]. After feedback is returned, I will hopefully have a few days to plan the EMA. For planning the EMA report writing, I plan on creating a new GitHub column on the board, and break down the sections into stories. 

I then have a wedding weekend away. I'm hoping this will be a nice rest before the final 40 days that are schedules to complete the EMA report. The final week in August which shows unavaiable, is my sisters wedding. I am on annual leave that week and hope to do a few hours of EMA work each day. However, the two weeks prior to this, I hope to get the majority of the report written. Finally, as I have another wedding the Friday before the EMA deadline, I am hoping to hand in the EMA a few days early. 

![gantt chart updated with improv.png](../../Zettlr_Images/gantt chart updated with improv.png)

Gigure 16: The Gantt chart showing the projects updated schedule

![v2 1.png](../../Zettlr_Images/v2 1.png)
![v2 2.png](../../Zettlr_Images/v2 2.png)

Figure 17: GitHub V2 column showing upcoming stories to be implemented

### Resources

Below shows the Resources identified since TMA02, which are required for project completion. Appendix 28 includes previously identified Resources, which have been updated where where necessary.

 

Table 2: List of Resources

FAB [@react_native_material_floating_nodate]
Switch [@noauthor_switch_nodate] 
Jest [@jest_jest_nodate]

## Risks

Below shows an evaluation of risks, associated with current and previous resources. A list of skills associated with the project is provided in Appendix 29. 

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
Table 3: List of Skills

## Review your personal development (1428/1000)

Gathering and analysising information for the literature review's is something I have found quite difficult. At the start of the project, I wasn't aware of what a literature review was but attending a Library services tutorial helped understand how to do the pratical side of things. I attended this quite late on, and I would have benefitted from reading the resources and practising earlier. Although I find it challenges, it has probable been a biggest learning and an activity I have started to see the real benefits from. 

Nevertheless, I have started the see the benefit from Literature reviews and performing reseach as a whole. Legal reseach has made me aware of GDPR rules that I wouldn't have previously considerred, such as "Right to Erasure", or the differences between Personal Identifiable data and pseudonymous data, such as usernames, and how this affects the system. I particularly enjoyed learning about the benefits of home growing; environmental, mental and physical and software accessible when researching EDI concerns, and how this has affected UX. For example, it had I've considered things for granted such as a good colour scheme, and simple textual descriptions, and regarding UX, simple navigation and feedback alerts for users. I will definitely be more aware of EDI concerns when builing future software projects with work. 

Mocking up the HCI was also a useful activity. LucidChart [@lucid_documents_nodate] was easy to use, and provided in built mobile components. Drawings could then be replicated and small changes made. They also helped me identify which components could be reused, for example, the Vegetable Details page. As React Native is a component language, the mock-up elements map quite closely to what the code components would be. For example, "screens" are the other most component, with smaller "child" components such as lists, and list elements. After reading a few chapters on "Patterns", again it made me realise design we subconsiously expect, and how much of it is to do with the movement of a thumb. Shared components such as Vegetable Lists or Details were discovered during mocking-up which then influenced the way I coded those components, as I had reuse in mind.

Learning React Native was also harder that I expect. I have worked using Vue previously, so assumed they were more similar then they are. For each story, specificially earlier stories, alot of time was reading React Native documentation, slowing down development. I should have dedicated a few weeks to focus on learning React Native, instead of learning on the go. Although, I did still enjoy this process and after the initial learning curve, I could start to identify similarities with Vue, which made it easier. The three part tutorial was the turning point for me becuase before this, I was struggling to understand how the various elements of React Native fitted with each other. After starting devevelopment, I quickly realised some kind of state management was needed for the system becuase state that gets created in one screen, such as a plot, is required in another, for example, to create the timeline. Having heard only of Redux before, I jumped straight into implementing Redux. However, I should have researched alternatives as React Native itself now has its own store which could have been an alternative to consider. Nevertheless, Redux works well as a centralised state storage, and once the pattern was set up once, it was easy to repeat for different data. 

I did spend time researching the differences, positive and negatives of developing React Native components with either classes or functions. (ref comparision here). Using classes gave a component internal state, which was required for some of the components, however it meant there wasn't access the lifecycle hooks such as `useEffect` [@react_using_nodate]. Instead, the systems components, on mount, called the `componentDidMount` asycronous function which allows data to be fetched. This was used to make the application reactive. For example, after adding a vegetable to a plot, when clicking back on the plot tab, the vegetable list was to be automatically updated to include the new vegetable. 

Although I have previous experiece with Rails, I haven't created a Rails service from scratch before or defined an API. For example, I hadn't considered the different ways of implementing a API request, such as this request of getting the selected vegetables for a plot. The request could get all vegetables, filtering by those with the given `plot_id`, or it could get the plot including its vegetables. The reactivity problem above influenced the decision to go for the latter. This is becuase it meant only one request needed to be made on mount, and the component would detect a change of state and rerender the components. If the alternative was used, this call to get all veg, filtered by plot, would have been declared in the veglist child components `mount` function. However, React wouldn't have known to rerender this child component becuase the request to get the plot would have look like nothing was changed. Additionally, this also as to save the number of requests to the server, which isn't a problem for such a small scale system, but is something to consider when developing higher throughput applications. Appendix 30 explains futher learning on individual stories.

Designing the database was also interesting, becuase although I have maintained and developed databases, they have never been from scratch. There was a few iterations of the database design (Appendix 31) and I found it a good activity to decide which tables certain attribtues should belong to. For example,  frost dates was originall going to be stored on a plot, depending on their location. However, as this is now a stubbed value, it might not need to be in a database at all, becuase it is unlikely to change. Additionally, sow, plant and harvest dates were going to be dependent on this frost date, which could have been different for each plot location. This meant that the dates could be stored on the PlotVegetable entity. However, since the decision to stub frost dates, this is no longer the case, and specific dates can be stored against the vegetable. This lead to the problem solving things like how to store these dates, which was required to show in a timeline. This was an interesting problem becuase MySQL database doesn't have a List as a type, so I had to be a bit creative and think of alternatives. 

The development of working prototypes for both Vue Cordova and React Native was a big learning curve, as described in Appendix 32, yet carrying my learning experiences from one prototype to another was very rewarding and it put me in a good position to choose between the two, knowing they both fundamentally work. I also learnt about networking and IP addresses becuase of this. As the React Native application was running in a Expo iOS Simulator, it wasn't realising that it was running on the same `localhost` as the Rails API. I then updated the request to point to the laptops IP address. The request then timed out, which was progress. A Stack Overflow answer [@rice_answer_2019] solved this exact problem, suggesting binding the Rails server to 0.0.0.0, which was successful as my phone accessed bank-end data over the internet. This internet dependency was confirmed when developing the application in the car. I hotspotted which changed my laptops IP address because of the different network. Updating the front-end request to use the new IP successfully served the back-end data again. 

Another main learning was around UX. After the MVP feedback included lots of UI changes, I started to implement CSS styling improvements manually. As shown in Figure 9 earlier, this wasn't very successful. I researched and implemented a few React Libraries for styling and settled on the simple [@reactnativematerial_hello_nodate]. [@mui_mui_nodate] was the alternative, which looks very professional, but possibly overly complicated for this system. Additionally, it was interesting trying to find libraries to support the Timeline feature. Sysnoymns such as timetable, calendar, data grid, data table, gantt chart all have many results when researching. This process took longer than expected, and I should have considered more time for this research or a seperate story. I ended up implementing this tool for the Timeline [@noauthor_datatable_nodate].

Finally, more than anything, I have learnt to manage my time during this project. Although my work life balance, isn't very balanced at the moment, I feel like I have been as organised as I can be. However, this next few months, I will also schedule in "nights off" and prioritise "down-time" as well, to try enjoy the final few months of my Open Univeristy degree.

## Tutor

A few observations on things I will fix for the EMA:
- There are a couple of appendix's which were slotted in late, I have named them with `b`
- Some of the Appendix's are still in draft form, these will be written up properly for the EMA
- I will add a Glossary for the EMA
- I am aware of your previous feedback "Include A proper consideration of professional issues  (see BCS Code of Conduct)". I didn't find the opporunity to add that in this TMA, but I will make sure to for the EMA

A few questions:
* Should I include another resources table with smaller supplement materials, such as all the stack overflow posts I've used
* Is the formality level of my writing ok
* Which brings me on to, who is the intended audience of this report
* Would you like more updates of my progress
* Is there anything telling about why which Learning objectives have been placed together, I assume this grouping is to influence the word count?
* I found it hard to distinguish "review of current stage of project work" and "personal development". 
* Should  MVP feedback  and Improvement feedback be in appendixes or main body



