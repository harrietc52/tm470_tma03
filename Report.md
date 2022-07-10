Harriet Craven
F5256798
TM470 TMA03
12th July
5000 words

#  Contents
Table of Contents
Table of Appendices
Table of figures
Table of tables

# Project title 

An analysis of the development of an application which helps manage the growing of vegetables; specifically, what to plant, where and when

# Section 1: Draft Project report
(3682 words)

## Problem description
### Nature and context of the problem

Prior to 2007, growing your own food was largely associated with older middle-class households.  [@church_growing_2015] More recently, vegetable growing has increased in popularity, especially during Covid-19, with currently 15% of UK households growing thier own produce. This newer generation drives the modernisation of vegetable growing, and with that new challenges. Growers may not have the experience, old notes or the luxury of time to experiment with growing. Instead, attention spans are short and time is precious, resulting in growers wanting to get up to speed quickly. Therefore, this problem presents an opportunity to create a modern, accessible and informative way to help growers learn how to grow vegetables quickly. 

Having experienced a steep learning curve when taking up growing myself a few years agoadespite repeadly reading the book  "Allotment, Month by Month" [@buckingham_allotment_2019] it was clear fellow allotmenters relied on “Age and experience!”, “Trial and error”, or even “A very old readers digest called 'Food from your garden'”, when asked during initial research: “How do you know what to plant, where and when?” (Appendix 1) Understandably, this guesswork, learning curve and admin time, required to research and plan a growing search, may put off potential new growers; the proposed solution aims to reduce these unknowns.  

### Proposed solution or recommendations

The core system was made with Ruby on Rails, using the MVC pattern [@open_university_architecture_nodate]. However, React Native is the user interface (or View). Decoupling Rails logic from the front-end is the REST API, which uses HTTP with JSON encoded data to send requests and return responses [@open_university_web_nodate]. React Native used Redux as its centralised state storage, and RSpec and Jest are used for unit testing Ruby and React respectively.  The software solution process is based off TM354 [@open_university_tm354_nodate] with Mobile techniques and Web service protocols based off TM352 [@open_university_tm352_nodate]. Appendix 2 explains more detail about how this modules have influenced the project. Additionally, multiple projects at work have involved JavaScript, Ruby on Rails and relational databases. 

The project output is a hybrid application, ran locally using Expo's iOS simulator. Screenshots of the application, capturing various features will be presented, along with documentation of the API and testing outputs. The application first asks a user to create an account, and then a Plot, where permission to acces the devices geolocation can be granted. A list of vegetables can be viewed, with further details available for each vegetable. Selected vegetables can be added to the users plot. These populate the Timeline, which displays information regarding when each vegetable should be sown, planted and harvested.

| Scope                         | In or Out | Why                                                                                |
|-------------------------------|-----------|------------------------------------------------------------------------------------|
| Food Bank donations           | Out       | LSE&P research: food standards, unscrupulous growers                               |
| Push notifications/ Alerts    | Out       | Irritable if not managed properly. Requires access to device settings              |
| Plot Layout                   | Out       | Complex front-end skills and data manipulation required                            |
| Remove a plot location        | In        | GDPR law                                                                           |
| Allotment association         | Out       | Prevent discrimination, support notion that anybody can grow vegetables, anywhere. |
| Allotment tips/ seed swapping | Out       | Consequence of above                                                               |
| Frost dates                   | Out       | Freely available API (accepted risk).Stub frost dates if implemented               |
| Task List/ Calendar           | Out       | Second questionnaire prioritised a Timeline (Appendix 2b)                          |

Table 1: Scope refinements and evaluation criteria made to the project specification, using MoSCoW [@open_university_iterative_nodate] to prioritised requirements. (Previous versions in Appendix 3)

### Analysis of likely impact 

Users of the application will have some personal data stored; Location data could be PII, as a user could be traced back to the location. GDPR states PII should be protected, and collected data should state its purpose and duration of persistence. Geolocation access should therefore have the explicit consent [@ico_location_2021].  This is implemented in the system with a checkbox on plot creation. Additionally, under GDPR, users have the “Right to Erasure” [@ico_right_2021] . Therefore, a button will be added allowing a user to remove their location data.

To allow client to server communication, the server binds to 0.0.0.0, which allows all ingress traffic, including the Expo iOS Simulator. This is a security hole, and if developed to scale, firewalls, ACLs and ports would need to be configured and Cross Origin Requests (CORS) restricted [@open_university_41_nodate]. An API key between the server and client could also be implemented, allowing the server to authenticate incoming requests. 

In regards to social impact, the system will positively contribute to sustainability, by preventing waste and unnecessary transportation of food, having a positive impact on climate issues, by reducing the carbon footprint of food consumed. [@jones_why_2021]. Additionally, allotment growers have claimed to save around £950 a year through home growing. [@jones_allotment_2009] (Note: save costs could have increased since 2009, due to food prices increase.) However, this increase in home growing could change growers buying patterns, leading to challenges for small local businesses that grow and sell vegetables. These businesses may need to increase prices, which could negatively impact people who don’t grow vegetables. To avoid this, schemes to support and promote local business could be considered.

If the result is more people grow vegetables, this also has mental health benefits [@jones_why_2021]. Especially during Covid-19, where home growers had higher well-being and lower levels of food insecurity [@mead_growing_2021]. As well as boosting mental wellbeing, growing vegetables also provides physical exersise, as soil is maintained, and crops are cared for, resulting in alot of time spend outdoors in fresh air. Most of all, the imact would hopefully be the reduced time it takes growers to plan what they would like to plant that year. Specifically, the timeline feature might help growers be more aware of what jobs need to be done when, reducing the congnitive load of groweing vegetables and incresing the enjoyment. 


## Account of related literature 

[@buckingham_allotment_2019] provides a "Month by Month" plan to grow vegetables, including vegetable specific details which were used to manually input application data. Digitialising this content inspired the project idea initially. Project planning resources from TM470 [@open_university_planning_nodate] explain how to create a project schedule, define tasks and subtasks, and suggest keeping a journal to support self-reflection and learning. [@dawson_dawson_2015] project management book gives a ... invaluable overview of … , specifically aimed at students which supports the OU material well.

[@lei_statistical_2017] analysis of the effects of Kanban and Scrum on software development projects concludes the KanBan method maybe be better in terms of managing project schedule. However, this project appeared to benefit from a complete upfront design and plan with timeframes, and therefore KanBan wasn't suitable. Hybrid approaches, such as ScrumFall [@rahim_scrumfall_2018] and AppScrumFall  [@bisaa_appscrumfall_2020] were also considered. Both advoacated unfront requirement analysis, with several sprint iterations before delivery, with AppScrumFall emphasising thourough testing across all platforms. Lifecycle approaches compared in TM470 [@open_university_choosing_nodate] and TM354 [@open_university_approaches_nodate], are summarised in Appendix 4. This proejct closely follows TM354 Case Study Resources from Unit 4, 8 and 12 [@open_university_tm354_nodate], which illustrate the application of the software development concepts studied, following a Waterfall approach, which was best suited to WaterFallScrum, [@west_water-scrum-fall_2011] the SDLC process followed by this project. 

Domain analysis found Jones' [@jones_why_2021] article describing the benefits she experienced through home growing, which included mental and physical health benefits, a new found sense of community and the enjoyment of freshly picked harvest. Mead's research [@mead_growing_2021] found food insecurity during early Covid-19, was reduced for those who grow vegetables, which in turn was associated with better well-being. [@church_growing_2015]'s Ecological Economics paper considdered food growing trends across Europe, stating that only in the UK is growing food "predominantly associated with older middle class households", as ~75% of growers are 35 years or older, leaving a minority of growers between the ages of 18-34. Although written in 2015 (and therefore quite dated), this skewed demographic and the potential to attract a younger generation of growers, heavily influenced the projects problem statement. (Appendix 5)

Existing applications: VeggieGardenPlanner [@veggiegardenplanner_veggie_nodate-1] and RHS GrowYourOwn [@rhs_grow_nodate] and Planter [@planter_planter_nodate], vary in UI quality yet support overlapping features. They allow a user to view vegetable information, add vegetable to the plot and display a calendar or task list associated with the vegetables. 'VeggieGardenPlanner' provides more information on companion planting (which vegetables are good or bad neighbours) and 'Planter' retrieves locations and sets the plots frost dates. These use cases formed the initial scope of the system and influenced the user interface. Other similar resources which were dismissed are described in Appendix 6.

[@neil_mobile_2014] describes many UI examples, both sucessful and unsuccessful, however content appeared dated. Instead [@perea_ux_2017] introduces a pragmatic approach to designing mobile apps, including Andriod and iOS respective best practices and UI elements respectively. [@shneiderman_eight_2016] outlines eight "Golden Rules", a set of key principles to enhance user interfaces. These principles have been derived from experience and refined over three decades. Yet, they state each principle requires fine-tuning for specific design domains and validation from users. Perea and Shneiderman HCI influences are described in more detail in Section (HCI design).

The TM354 Case Study then follows the process from requirements, to analysis and design. Unit 8 advocates requirement ananlysis through the creation of class diagrams with attributes, assocaitions and operations, as system constraints and allocation of responsibilities can be considdered when structuring classes in a visual way. Unit 12 explored a systems architecture and goes on to describe implementation. 

During back-end development, [@railsguides_getting_nodate] provided a high-level overview to "Getting Started", tailored to a specific Rails version. Rails documentation It was also used to understand how to rollback a migration when adding further attributes and `scaffold`  [@railsguides_rails_nodate]  used to create a full set of model, migration, controller, resource and respective tests, automatically conforming to Rails project structure conventions. However, [@ds_creating_2019] provided a much thourough tutorial, specifically stating how to set up a project in API-only mode, specifiying the test suite and selected database. Additionally, [@livingston_setting_2018] clearly summaried how install and to configure Rspec, finer details which the RailsGuide lacked.

TM352's Cordova development guide [@apache_cordova_android_nodate] provided pratical tasks to set up a project. However, React Native was later chosen for front-end development, for reasons explained in Appendix 7. Although [@reactnative_learn_nodate] documentation share simple code to illustrate basic React concepts like `state` and `props`, [@expo_create_nodate] documentation guided the initialisation of the final project.  Then, with the aim of creating a clear front-end directory structure, similar to that which the `scaffold` command provides for Rails, [@reactnativeexample_react_2021] outlined a template for a clear and organised project structure which was adhered to.

During implementation, the mose influencial three-part tutorial  [@fullstacklabs_creating_nodate] described how to build a simple app, using Ruby on Rail API and a React Native client, which first set up a Rails API project, then React Native using Redux for state management, and finally connecting the two. Additionally, TM352, specificifcally JSON and REST resources [@open_university_tm352_nodate]  were revisted when developing this client to server communication. Analysis of tutorial's working code on GitHub provided a greater understanding of Redux flow between store, reducers, actions and action type, along with "Getting Started with Redux" documentation [@redux_redux_2021]. The tutorials use of `async/await` was further explained by [@gagliardi_how_2018], specificaly regarding the use of promises in a `componentWillMount` lifecycle hook. 

ReactJS documentation explained the difference between creating components as a functions or classes [@react_reactcomponent_nodate] which [@geeksforgeeks_differences_2022] compares; Class Components are stateful and ran as part of the React life cycle, thus supporting methods such as `componentDidMount` making it better suited for this project which renders data on component initialisation. Further differences between the Functional and class components are summarised in Appendix 8. [@akshat_react_2019] support the Redux and Component class approach, as they introduced React Naviation, which advocates a wrapper (`withNavigation`) for existing components. Via this approach, the navigation prop does not need to be passed down through multiple child components. [@reactnavigation_access_nodate] 

To improve the systems styling, Material UI [@mui_mui_nodate] and  [@reactnativematerial_hello_nodate] provide different modular and customisable components for React Native, where the latter was selected for its simple installation and usage, and [@expo_expovector-icons_nodate] vector icons have been implemented throughout. Appendix 9 reviews literature which influenced the project in terms of LSEP issues and EDI concerns.

## Account of project work done and its outcome
### Analysing the problem
#### Requirement Gathering

The initial problem statement (Appendix 5), was drafted to better understand common processes when growing vegetables, using personal experience and research into existing applications (Appendix 6). The "Requirement Gathering Questionnaire" was then designed, based on this research. Appendix 10 summaries how the Questionnaire was designed. It was created using a Google Form with seven sections: General, Vegetable information, Crop Rotation, Reminders, Companion Planting, Social and Finally. Appendix 11 provides description of each section.

![questionnaire.png](../../Zettlr_Images/questionnaire.png)
![google form.png](../../Zettlr_Images/google form.png)

Figure 1: Summary of the Questionnaire and screenshot of the Google Form 

The Google Form was shared with my Allotment WhatsApp group, via LinkedIn and directly with 13 stakeholders, who forwarded it to relevant friends and family. Appendix 1 shows and overview of the 42 responses which were received. As responses came in steadily, each one could be processed and analysed in turn, grouping reoccuring features into categories. Popular resources such as websites, books and blogs where also noted. Further learning from this questionnaire is discussed in Appendix 12.

#### User stories 

After three weeks the questionnaire was closed and the "Main Takeaways" summarised in Appendix 13. These were stand-out requirements that made up the applications Use Cases. User stories were then created with textual descriptions, functional and non-functional requirements [@open_university_agile_nodate]. These use cases served as the basis for the functional requirements in the Volere template [@open_university_volere_nodate] in Appendix 15. 

![use cases prio:unprio.png](../../Zettlr_Images/use cases prio:unprio.png)

Figure 2: The systems Use Case, showing which have been deprioritised

![select veg texual desc.png](../../Zettlr_Images/select veg texual desc.png "select veg texual desc.png")
Figure 3: A user story example (Appendix 14 includes others)

#### Architecture

Architecturally significant requirements (ASRs) were identified, with four characteristics stated below, including an example requirement that drives the system’s software architecture. [@open_university_architecturally_nodate] 
* _Quality attributes_: Security non-functional requirements stated no personal data will be stored, yet other data will be stored. Thus, a database is required.
* _Core features_ Core features are described by Chen et al as ‘the problem the software is trying to solve’. For example, the system should allow a user to create, read, update and plots (CRUD). 
* _Constraints_. From initial requirement gathering, an app to support both iOS and Android platforms was preferable. Having explore different approaches to mobile developent: web, native and hybrid (Appendix 16). This preference of a hybrid, places a ASR constraint, limiting the choice of Frameworks available. 
* _Application environment_. The Application environment for the system is locally hosted on a laptop, using Expo's iOS Simulator. This requires the abilty mimic device sensors, such as GPS connectivity for location access.

The ASRs resulted in a mixture of architectures: a client–server architecture, with the web browser client sending a request to a web server and receiving a response and a three-layered architecture corresponding to the client, the web server that constructs the response and the database storage [@open_university_architecture_nodate]. The database sits behind a REST API, which is used to access and store data, using REST HTTP operations. 

![architecture.png](../../Zettlr_Images/architecture.png)
Figure 4: High-level architecture of the system

Ruby on Rails was chosen as the back-end service, due to prior Rails experience and its ability to create a RESTful JSON API quickly. The Rails router provides automatic URL generation, where paths can be specified with approved HTTP methods and in-build mapping between HTTP to Controllers, allows easy object manipulation in the logical layer. [@railsguides_using_nodate] A relational-database, MySQL, was chosen becuase the type of data to be stored is pre-defined, the size of data is very small and relationships (such as a Plot is owned by a User) can be represented.

#### Prototype

Two protoypes, using Vue Cordova and React Native, were built to select a front-end Javascript Framework. Following TM352 tutorial, Cordova appeared more complex and required manual restarting of the application after every update, unlike React Native, which had dynamic reloading and clear documentation. A working protoype in React Native was completed, following @reactnative_learn_nodate where back-end data was accessed via the API and displayed in a List component, using Expo. 

![react native prototype.png](../../Zettlr_Images/react native prototype.png "react native prototype.png")

Figure 5: Back-end data displayed in React Native component, using Expo's iOS Simulator

### Synthesising a solution
#### Class Design

Having chosen a technology stack, a class diagram of the software was designed. Firstly, using the above Use Cases, potential "concepts" were identified and analysed, as to whether they justified as classes. (Appendix 17) The final core entities were: User, Plot and Vegetables. Associations required to constrain these classes were then identified:
* User: A user may have only one Plot
* Plot: A plot must belongs to a User
* Plot: A plot could have many Vegetables
* Vegetables: A vegetable can belong to many Plots

This identified the many-to-many relationship between Plots and Vegetables. To handle this, one option was to create an attribute on `Plot` with a list of `vegetableIds`. However, this isn't very scaleable and data on this relationship, such as Notes, could not be  later implemented if required. Alternatively, a joining (or Association) class between Plots and Vegetables called "PlotVegetables" could represent this relationship, where a PlotVegetables may belong to only one Plot. This class, association and constraint was added to the class diagram. [@open_university_structural_nodate] 


![class v2.png](../../Zettlr_Images/class v2.png)
Figure 6:  Updated Class Diagram (Appendix 17b shows a rough sketch of the initial version).

#### HCI design
Human computer interation diagrams (or mock-ups) were created following patterns from the book "UX Design for Mobile" [@perea_ux_2017] and [@shneiderman_eight_2016] principles. 

Bottom navigation is the most common layout for iOS apps, as it is close to the thumb and allows changing sections without much effort. It is recommended there are no more than five sections. The use cases helped select the three sections: My Plot, Vegetables and Timeline, as they would cover the functional requirements. It is also an accepted design pattern to indicate which section is in use, and the ability to go between sections freely. This supports [@shneiderman_eight_2016] 1st principle, as Navigation conforms with the aim of consistency throughout.

Sliding drawer (also know as "hamburger menu") profiles an alternative menu that is used less frequently, such as settings. Here, it is used to remove a User, Plot or location, as to abile with GDPR's "Right to Erasure" policy [@ico_right_2021]. Back buttons were added throughout, allowing a user to return to a previous page, or in a multiscreen task (such as creating a user, then a plot) it can break up the processes into smaller steps. Interestingly, languages written from right to left would have a back button pointing to the right. This application supports only English and constraint to the UK. 

Actions such as swiping to remove a vegetable from a plot, or holding down for more information could be used. However, it is recommended an alternative one-tap interaction is also provided, for those with less experience or accessibility limitations. [@shneiderman_eight_2016]'s 2nd principle "Seek universal usability" also recognises this as encourages features for both novices, such as explantaitons, and experts, such as shortcurs, enrich the design. Furthermore, "floating buttons" are usd to highlight a functionality over other elements, such as the button to add vegetables to an empty plot [@react_native_material_floating_nodate].

The "Picture superiority effect" refers to the phenomenon where people remember images better than words, and therefore images have been used where possible on the Vegetable List, Vegetable details and Timeline views.  Additionally, both [@perea_ux_2017] and [@shneiderman_eight_2016] state that alerts should be used to show and prevent errors, where messages are in clear English.

There were overlapping features between Calendar vs Timeline vs Task List discovered when mocking up. I asked stakeholders for their UX preference from the below three applications: VeggieGardenPlanner, Royal Horticultural Society App and Planter (Appendix 18). The 12 stakeholders felt Option 1 and Option 3 were similar, with the majority preferring Option 1's (Timeline) overview. 

Appendix 19 contains Stakeholder feedback for the mockups, which was quite positive. 

![mockup welcome.png](../../Zettlr_Images/mockup welcome.png)

![mockup plot and veg.png](../../Zettlr_Images/mockup plot and veg.png)

Figure 7: Mock-ups (Timetable mock up in Appendix 18)

#### Implementation

The figures below show various forms of results from the current working system, with more evidence in Appendix 20 in the form of `git commit` messages, and project structure (Appendix 21) and code (Appendix 22). Further implementation details and learnings are shared in Section (Review your personal development)


![before ux.png](../../Zettlr_Images/before ux.png "before ux.png")

Figure 8: Expo's iOS Simulator screenshots show initial implementation of requirements using only HTML

![basic css.png](../../Zettlr_Images/basic css.png)

Figure 9: iOS Simulator screenshot, with basic CSS implementation

![implem welcome.png](../../Zettlr_Images/implem welcome.png)

![implem plot and veg.png](../../Zettlr_Images/implem plot and veg.png)
![implem timeline.png](../../Zettlr_Images/implem timeline.png)
Figure 10: Latest screenshots of the current system, showing the implementation of UI Style library [@reactnativematerial_hello_nodate] 


![db schema.png](../../Zettlr_Images/db schema.png)
Figure 11: Current Ruby on Rails database schema



![postman plots.png](../../Zettlr_Images/postman plots.png)

Figure 12: Rails RESTful JSON API Documenation, automatically generated and published at `https://documenter.getpostman.com/view/11169298/UzJLPcQF#intro`


![mvp done.png](../../Zettlr_Images/mvp done.png)

Figure 13: GitHub showing MVP stories which have been implemented (or deprecated) since TMA02. 


### Evaluating the solution

Validation and verfitcation, as show below, has been in the form of some testing and user feedback. The Volere Template, in Appendix 15, was also refered back to, confirming all the functional requirements, apart from removing a Vegetable from a plotand removing a location, have been implemented. 

#### Testing

RSpec has been installed and configured for the testing the back-end Rails service [@livingston_setting_2018]. Although the development process has not followed strict test-driven development, black-box tests were drawn up for each operation before implementation. Jest will be used to unit test React Native components, however this has not yet been set up. 

![rspec.png](../../Zettlr_Images/rspec.png "rspec.png")
Figure 14: RSpec tests which have been created, due to the `scaffold` command, but they are not yet implemented

![test1.png](../../Zettlr_Images/test1.png)
![test2.png](../../Zettlr_Images/test2.png)
Figure 15: Two test case for User Stories: 'Create a plot' and 'Add veg to plot'. 

#### Feedback

Where possible, stakeholders were asked to interact with the system through the simulator and others sent screenshots of the application (as show in Figure x). Stakeholder feedback is summarised in the Appendix 24, and Section (Plan) describes how this feedback was converted into stories for the next iteration. 


# Section 2: Review 
(3370 words)

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

Nevertheless, I have started the see the benefit from Literature reviews and performing reseach as a whole. Legal reseach has made me aware of GDPR rules that I wouldn't have previously considerred, such as "Right to Erasure", or the differences between Personal Identifiable data and pseudonymous data, such as usernames, and how this affects the system. I particularly enjoyed learning about the benefits of home growing; environmental, mental and physical and software accessible when researching EDI concerns, and how this has affected UX. For example, it had I've considered things for granted such as a good colour scheme, and simple textual descriptions, and regarding UX, simple navigation and feedback alerts for users. I will definitely be more aware of EDI concerns when builing future software projects with work. Additionally, making "IT for Everyone" is a BCS Code of Conduct principle, which I am trying to adhere to. [@bcs_bcs_nodate]

Mocking up the HCI was also a useful activity. LucidChart [@lucid_lucidchart_nodate] was easy to use, and provided in built mobile components. Drawings could then be replicated and small changes made. They also helped me identify which components could be reused, for example, the Vegetable Details page. As React Native is a component language, the mock-up elements map quite closely to what the code components would be. For example, "screens" are the other most component, with smaller "child" components such as lists, and list elements. After reading a few chapters on "Patterns", again it made me realise design we subconsiously expect, and how much of it is to do with the movement of a thumb. Shared components such as Vegetable Lists or Details were discovered during mocking-up which then influenced the way I coded those components, as I had reuse in mind.

Learning React Native was also harder that I expect. I have worked using Vue previously, so assumed they were more similar then they are. For each story, specificially earlier stories, alot of time was reading React Native documentation, slowing down development. I should have dedicated a few weeks to focus on learning React Native, instead of learning on the go. Although, I did still enjoy this process and after the initial learning curve, I could start to identify similarities with Vue, which made it easier. The three part tutorial was the turning point for me becuase before this, I was struggling to understand how the various elements of React Native fitted with each other. After starting devevelopment, I quickly realised some kind of state management was needed for the system becuase state that gets created in one screen, such as a plot, is required in another, for example, to create the timeline. Having heard only of Redux before, I jumped straight into implementing Redux. However, I should have researched alternatives as React Native itself now has its own store which could have been an alternative to consider. Nevertheless, Redux works well as a centralised state storage, and once the pattern was set up once, it was easy to repeat for different data. 

I did spend time researching the differences, positive and negatives of developing React Native components with either classes or functions. (ref comparision here). Using classes gave a component internal state, which was required for some of the components, however it meant there wasn't access the lifecycle hooks such as `useEffect` [@react_using_nodate]. Instead, the systems components, on mount, called the `componentDidMount` asycronous function which allows data to be fetched. This was used to make the application reactive. For example, after adding a vegetable to a plot, when clicking back on the plot tab, the vegetable list was to be automatically updated to include the new vegetable. 

Although I have previous experiece with Rails, I haven't created a Rails service from scratch before or defined an API. For example, I hadn't considered the different ways of implementing a API request, such as this request of getting the selected vegetables for a plot. The request could get all vegetables, filtering by those with the given `plot_id`, or it could get the plot including its vegetables. The reactivity problem above influenced the decision to go for the latter. This is becuase it meant only one request needed to be made on mount, and the component would detect a change of state and rerender the components. If the alternative was used, this call to get all veg, filtered by plot, would have been declared in the veglist child components `mount` function. However, React wouldn't have known to rerender this child component becuase the request to get the plot would have look like nothing was changed. Additionally, this also as to save the number of requests to the server, which isn't a problem for such a small scale system, but is something to consider when developing higher throughput applications. Appendix 30 explains futher learning on individual stories.

Designing the database was also interesting, becuase although I have maintained and developed databases, they have never been from scratch. There was a few iterations of the database design (Appendix 31) and I found it a good activity to decide which tables certain attribtues should belong to. For example,  frost dates was originall going to be stored on a plot, depending on their location. However, as this is now a stubbed value, it might not need to be in a database at all, becuase it is unlikely to change. Additionally, sow, plant and harvest dates were going to be dependent on this frost date, which could have been different for each plot location. This meant that the dates could be stored on the PlotVegetable entity. However, since the decision to stub frost dates, this is no longer the case, and specific dates can be stored against the vegetable. This lead to the problem solving things like how to store these dates, which was required to show in a timeline. This was an interesting problem becuase MySQL database doesn't have a List as a type, so I had to be a bit creative and think of alternatives. 

The development of working prototypes for both Vue Cordova and React Native was a big learning curve, as described in Appendix 32, yet carrying my learning experiences from one prototype to another was very rewarding and it put me in a good position to choose between the two, knowing they both fundamentally work. I also learnt about networking and IP addresses becuase of this. As the React Native application was running in a Expo iOS Simulator, it wasn't realising that it was running on the same `localhost` as the Rails API. I then updated the request to point to the laptops IP address. The request then timed out, which was progress. A Stack Overflow answer [@rice_answer_2019] solved this exact problem, suggesting binding the Rails server to 0.0.0.0, which was successful as my phone accessed bank-end data over the internet. This internet dependency was confirmed when developing the application in the car. I hotspotted which changed my laptops IP address because of the different network. Updating the front-end request to use the new IP successfully served the back-end data again. 

Another main learning was around UX. After the MVP feedback included lots of UI changes, I started to implement CSS styling improvements manually. As shown in Figure 9 earlier, this wasn't very successful. I researched and implemented a few React Libraries for styling and settled on the simple [@reactnativematerial_hello_nodate]. [@mui_mui_nodate] was the alternative, which looks very professional, but possibly overly complicated for this system. Additionally, it was interesting trying to find libraries to support the Timeline feature. Sysnoymns such as timetable, calendar, data grid, data table, gantt chart all have many results when researching. This process took longer than expected, and I should have considered more time for this research or a seperate story. I ended up implementing this tool for the Timeline [@react_native_datatable_nodate].

Finally, more than anything, I have learnt to manage my time during this project. Although my work life balance, isn't very balanced at the moment, I feel like I have been as organised as I can be. However, this next few months, I will also schedule in "nights off" and prioritise "down-time" as well, to try enjoy the final few months of my Open Univeristy degree.

## Tutor

A few observations and things I will fix for the EMA:
- Some Appendix's were slotted in late, with the suffix `b`
- Write up Appendix's, as some are in bullet points
- Add a Glossary 
- Properly consider professional issues (BCS Code of Conduct)
- Update the Volere Template

A few questions:
* Please comment on the above, if you think they are all worth doing
* Should I include another resources table with smaller supplement materials, such as all the stack overflow posts I've used
* Is the formality level of my writing ok
* Which brings me on to, who is the intended audience of this report
* Would you like more updates of my progress
* Is there anything telling about why which Learning objectives have been placed together, I assume this grouping is to influence the word count?
* I found it hard to distinguish "review of current stage of project work" and "personal development". 
* Should  MVP feedback  and Improvement feedback be in appendixes or main body


# Word Count: 
xxxx words

# References

Check books:
* Allotment Month by Month
* "UX Design for Mobile", chapter "Mobile Patterns - Web App, Android and IOS best Practices". Section, "Mobile application design patterns"


::: {#refs} 
:::

# Appendices
## Appendix 1

Requirement Gathering Questionnaire responses
(re. Section 2.2.1)

![questionnaire1.png](../../Zettlr_Images/questionnaire1.png)

![questionnaire2.png](../../Zettlr_Images/questionnaire2.png)


## Appendix 2

Project influences from TM352, TM354 and my place of work
(re. Section )

TM354:
- software development - following the course material, specifically case study. as a waterfall approach. becan with domain research, requirments, modelling, design, analysis,  now implementation. database design?
- design and software implementation project typically focus on a problem which can be solved with a simple software application
- process and modelling techniques for the design, architecture and testing of software solutions
- UML techniques
- waterfall vs Agile development
- collection of requirements
- the development of a design with appropriate research
- the development of a complete or partial software solution or suggestions for implementation
- evaluation of the design and software if produced (stakeholders)
- Scope: if problem is large, identify a smaller component which can be solved in isolation, providing significant value
- Projects will typically build in evaluation of the design, the software product and the method used to build it
- architectures and design patterns. Make use of the Gang of Four book  (Gamma et al, 1995) and Shaw and Garlan (1996)
- Evaluating and using testing methods. Evaluate test techniques such as test-driven development for your project: what benefits do they bring?
- A discussion of quality attributes and trade-offs within the developed system.
- testing/ tactics

TM352:
- mobile development, 
- web services and architecture
- web security issues
- web application design, accessibility and interaction
- standards and their role
- mobile application design and development
- approaches to mobile application development

Place of work:
- multiple projects in Rails with both relational and non-realtional databases. here, used mysql for relational becuasse… this includes rest api in JSON
- also worked on projects using Vue Javascript front end framework. 
- this is first project using React Native
- this is my first project involving mobile development

## Appenix 2b

Questionnaire sent to Stakeholders, asking preference on Calendar, Timeline or Task list
(re. Section )

Note: Duplicate of Appendix 18

Option 1: 
![qu op1.png](../../Zettlr_Images/qu op1.png)

Option 2:
![qu op 2.png](../../Zettlr_Images/qu op 2.png)

Option 3:
![qu op3.png](../../Zettlr_Images/qu op3.png)

Feedback from Calendar vs Timeline

| Person | Option 1 | Option 2 | Option 3 | Comment                                                                                                                                                                                                                                                          |
|--------|----------|----------|----------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| SC     | X        |          |          | --                                                                                                                                                                                                                                                               |
| PC     | X        |          |          | --                                                                                                                                                                                                                                                               |
| PM     |          | X        |          | --                                                                                                                                                                                                                                                               |
| FC     |          | X        |          | --                                                                                                                                                                                                                                                               |
| SS     | X        |          |          | --                                                                                                                                                                                                                                                               |
| EN     |          | X        |          | --                                                                                                                                                                                                                                                               |
| HB     |          |          | X        | --                                                                                                                                                                                                                                                               |
| JO     |          | X        |          | --                                                                                                                                                                                                                                                               |
| HC     | X        |          |          | I think the top has the best overview, but I also like the second                                                                                                                                                                                                |
| CC     | X        |          |          | I prefer the style of the third one (with the pictures) but like that the top one has all the different veg in one place                                                                                                                                         |
| KT     | X        |          |          | Probably the 1st one as it gives a good overview at a glance. But the 2nd one would also be useful for more short term planning, like 'what do I need to do this week'                                                                                           |
| CS     | X        |          |          | I like the first format for the veg timeline/calendar, as I'm mainly concerned with a broad overview of what I need to do throughout the year. However, I'd prefer for them to be ordered from the time they first need to be seeded rather than alphabetically. |

Final mock up of Timeline


![mockup timeline.png](../../Zettlr_Images/mockup timeline.png "mockup timeline.png")



## Appendix 3

Initial and current requirements, prioritised using MoSCoW. 
(re. Section )

Version 1: TMA01

| Must                                                                      | Should                                 | Could                    | Wont         |
|---------------------------------------------------------------------------|----------------------------------------|--------------------------|--------------|
| Dates of sowing/ planting/ harvesting each vegetable in a Calendar format | Layout map of the plot                 | How much to plant        | Social media |
| Food bank suggestions for left overs                                      | Allotment details such as phone number | Plant / seed swapping    |              |
| Reminders                                                                 | End of year notes, images, rating      | Todo list                |              |
| Companion planting help                                                   | Tips for each vegetable                | Help on choosing variety |              |
|                                                                           | Crop rotate                            | Seasonal recipes         |              |

Version 2: TMA02

| Must              | Should                  | Could                 | Won't                                  |
|-------------------|-------------------------|-----------------------|----------------------------------------|
| Create a user     | Add/ remove frost dates | Alerts for veg        | Plot layout                            |
| Create a plot     | End of year notes       | Alerts for weather    | Allotment details/ tips/ seed swapping |
| Show Vegetbables  | Show Calendar           | Help choosing variety | Seasonal Recipies                      |
| Select Vegetables |                         |                       | Social Media                           |
| Show Timeline     |                         |                       |                                        |
| Task List         |                         |                       |                                        |

Version 3: TMA03

| Must            | Should               | Could                | Won't                                  |
|-----------------|----------------------|----------------------|----------------------------------------|
| Create a user   | Remove veg from plot | Alerts for veg tasks | Plot layout                            |
| Create a plot   | Remove location      | Alerts for weather   | Allotment details/ tips/ seed swapping |
| Show Vegetables | Add/remove veg notes | Task List            | Seasonal Recipies                      |
| Show Veg info   |                      |                      | Food bank suggestions                  |
| Add veg to plot |                      |                      | Social Media                           |
| Show Timeline   |                      |                      |                                        |

## Appendix 4

Software development lifecycle comparison
(re. Section )

 
| Feature       | Scrum                                                                                                                        | Waterfall                                                                                                     | Kanban                                                                                    | Water-Scrum-Fall                     |
|---------------|------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------|--------------------------------------|
| Delivery      | Partial working system over a fixed period of time. Releases are made before sprint review                                   | One big deliverable at the end of the life cycle.                                                             | Continuous flow of delivery. Releases are made when ready                                 | incremental development phrases      |
| Activities    | Activities get revisited, issues can be tackled more frequently                                                              | Activities don’t overlap, and once finished, activities cannot be re-entered.                                 | Kanban has a flexible process. There can be a few activities in progress at any one time. | small tasks                          |
| Requirements  | Accept requirements, and deliver within a couple of weeks. Requirements discovered later in the lifecycle can be incorporate | Requirements gathered upfront, requirements are unlikely to change. Late requirements cannot be accommodated. | Good for requirements of different priority and size                                      | structured planning phrase           |
| Testing       | Each deliverable tested after the cycle. Any issues can be revisited the next cycle                                          | Testing happens at the end resulting in late discovery of errors                                              | Feedback loops are incorportated                                                          | feedback required after every "Fall" |
| Documentation | Agile documents via story cards, code, code comments                                                                         | Requirement are captured in formal, comprehensive documents, which are time consuming                         | There is no prescribed documentation                                                      |                                      |


## Appendix 5

Problem statement
(re. Section )

Note:  This includes some features which have since been deprioritised.


People who grow vegetables (growers) would like a new computer system to keep track of sow, plant and harvest dates in the year's calendar, to be reminded of these dates, to know what has been planted where and why and how much to plant per crop. 

Currently, growers use various means of note taking to keep track of this information. However, this is manual and problematic. For example, crops should not be planted in the same place year on year to allow the soil to recover, and if the previous year's notes were lost, the season's planting may not be as successful as it could be. Additionally, it is easy to forget when to sow seeds, indoors or outdoors, and habits such as sequential sowing (when crops are sown continuously throughout the season providing a more steady output of crops) are missed, because growers forget to sow. Similar opportunities are missed, if growers are not aware of the upcoming weather forecast, such as a sudden frost or dry spell, resulting in the possible loss of crops. 

The new software should resolve these problems by implementing a single allotment management system which is easy to use. The system should provide a grower with the ability to view possible crops, select the crops they would like to grow. Inputting any additional information such as variety, allowing them to add notes or images throughout the growing season. Additionally, growers should be alerted of weather warnings, and have help when plotting their patches, by tips of what crops grow well next to each other or not. Additionally, growers should have tips on companion planting, where the system would recommend what crops could be planted in and around another crop, to save space and benefit from one another. 

The system should handle usage either at home or on the allotment, on phone (iOS or Android) or directly from a web browser. Growers may only be able to have one “Plot” at any one time, but this plot can be completed, and the end of the season before starting the next. 

In the new system it must be possible to automate the creation of a Growing Timeline line, or Calendar, with a list of ToDo’s, whether it is sowing, watering, harvesting etc. The system will allow growers to check the todo’s off the timeline, and filter the timeline by month, or view the whole year at once.


## Appendix 6 

Existing Vegetable Growing applications
(re. Section )

| Name                                   | Type    | Notes                                                                                                                              | Features                                                                                                                                                              |
|----------------------------------------|---------|------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Royal Horticultural Society            | Website | Lots of information including growing tips. Provides a downloadable crop planner for most common vegetables. Sign up for more tips |                                                                                                                                                                       |
| Royal Horticultural Society App        | App     | The most useful app I could find.                                                                                                  | Add Plants to your Garden, view tasks and check of tasks                                                                                                              |
| Allotment Garden Dairy                 | Website | Very old school, hard to find any useful information                                                                               |                                                                                                                                                                       |
| VeggieGardenPlanner                    | App     | A well-developed application with similar features. A free tier with limited features and a paid for tier.                         | View vegetable list with lots of vegetable information, add to MyVeggies, view and Calendar and good/bad neighbours. Patch plan feature is not available on free tier |
| VegPlotter                             | Website | A hard to use website, but good features.                                                                                          |                                                                                                                                                                       |
| Gardeners World Allotment year planner | Website | A high-level overview of what to plant when                                                                                        |                                                                                                                                                                       |
| Charles Dowding Wall Calendar          | Website | A paid for calendar of planting and harvesting times                                                                               |                                                                                                                                                                       |
| Planter                                | App     | An app where you can build a plot with vegetable locations                                                                         | Add plant to plot. Design plot. View calendar and Growing guides                                                                                                      |

## Appendix 7

Comparing front-end Frameworks, React Native vs Cordova
(re. Section )

|     | React Native                                                                         | Vue Cordova                                                                                                                                                           |
|-----|--------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Pro | Dynamic loading. Easy development with simulation. Widely supported. Lots of plugins | I know Vue. Good Cordova plug ins                                                                                                                                                |
| Con | I don't know React                                                                   | doesnt have dynamic loadingless plug insslow to update after code changescordova feels a bit old school to use, not great documentationif using Ionic, would need to learn Ionic |

## Appendix 8
 differences between the Functional and class components are summarised in Appendix 10
 (re. Section )

  [@akshat_react_2019] 
 
## Appendix 9
  
 **LESPI**

Review of literature which influence the LESP project concerns is provided in Appendix 11. 
(re. Section )


(TMA02)
The TM470 resource "Legal, Social, Ethical and Professional issues" [@open_university_legal_nodate] provided further reading into GDPR and BCS resources. As a result of the GDPR "Right to Erasure" law [@ico_right_2021], a requirement was added which allows a user to remove their location, due to it being Personally Identifiable Information (PII). As an ICO website, an independent body, one can assume it is unbias and up to date. BCS also identifies ethical characteristics for IT professionals to follow. The Code of Conduct principles are clear [@bcs_bcs_nodate] and the source credible, as the Chartered Institute for IT. 

Another OU resource "Embedding equality, diversity and inclusion in your project" didn't provide lots of information, again, provide useful resources such as W3C's Web Content Accessibility Guide [@w3c_standards_nodate]. Technical standards described are very relevant, such as making HTML and CSS accessible. A sub-page of [@equality_and_human_rights_commission_protected_nodate] clearly states what characteristics are illegal to discriminate somebody on and a useful checklist to see if a systems language is free of gender bias is provided by [@european_institute_for_gender_equality_gender-sensitive_nodate]. A recommended tool called GenderMag seemed overly complicated for this project and so I won't use this resource going forward. [@noauthor_gendermag_nodate]  Finally, an OpenLearn course "Accessibility of eLearning" is brilliant as a visual learning tool with distinguishable chapters. [@openlearn_accessibility_nodate]. As an OpenLearn course it can be assumed this is kept relevant with no bias. 

Proffesional TODO
[@bcs_bcs_nodate] 
location data [@ico_location_2021] 
right to erasure [@ico_right_2021] 
W3C standards
personal data [@ico_what_2021] 

## Appendix 10

 How the questionnaire was designed
(re. Section )

* first made a list of how I manage the growing of our vegetables, what I do, don't do, know about, would like to do more of
* conducted some research in what allotment management applications exist, and what features they have
* then made a list of all possible features that might be useful
* tried to group them into categories
* final categories: General, Vegetable information, Crop Rotation, Reminders, Companion Planting, Social, Finally.
* General: two high level questions asking what does the responder use currently to managed, notes or other apps
* Vegetable information: how do they what to plant, when, and how much.
* Crop rotation: do they crop rotate and how do they keep track of what is planted where each year, to ensure that isn't planted in the same place again. This helps the soil recover
* Reminders: asking whether reminders would be useful, such as alerting users when to seed/plant/harvest would be useful
* Companion Planting: explain that companion planting is when crops are grown within each other, to support/encourage each other, and whether the responder does companion plant, and how they know what plants are good companions. e.g. lettuces benefits from the shelter of tall sweetcorn, so can be planted within the sweetcorn space. Also asked how to responders create the plot layout, considering what grows well / not well near each other. e.g. potatoes and tomatoes both suffer from blight that could easily spread from one to another if planted near by
* Social: questions about the use of social media to share vegetable growing experiences. asking what responders do with left over seeds/ vegetables
* Finally: in what location would it be used, a website or app preferred, any other recommended features, and favourite feature discussed above

## Appendix 11
Summary of headings in the Requirement Gathering Questionnaire
(re. Section )

* General: two high level questions asking what does the grower use currently to managed, notes or other apps
* Vegetable information: how do they what to plant, when, and how much.
* Crop rotation: do they crop rotate and how do they keep track of what is planted where each year, to ensure that isn't planted in the same place again. This helps the soil recover
* Reminders: asking whether reminders would be useful, such as alerting users when to seed/plant/harvest would be useful
* Companion Planting: explain that companion planting is when crops are grown within each other, to support/encourage each other, and whether the grower does companion plant, and how they know what plants are good companions. e.g. lettuces benefits from the shelter of tall sweetcorn, so can be planted within the sweetcorn space. Also asked how to grower create the plot layout, considering what grows well / not well near each other. e.g. potatoes and tomatoes both suffer from blight that could easily spread from one to another if planted near by
* Social: questions about the use of social media to share vegetable growing experiences. asking what grower do with left over seeds/ vegetables
* Finally: in what location would it be used, a website or app preferred, any other recommended features, and favourite feature discussed above

## Appendix 12

Learning from the Requirement gathering Questionnaire
(re. Section )

For the initial questionnaire, I hadn’t considered how I would analyse the results or the number of responses I would recieve. Although the 42 responses came steadily, fewer questions would have sufficed. I took this learning into the second “Timeline vs Task vs Calendar” questionnaire, which instead included one question with three multiple choice answers, which was much easier to process. (Appendix 5) What I have learnt from this is that an important factor in designing questionnaires is to think how the information will be processed.

## Appendix 13

Main takeaways from analysing the Requirement Gathering Questionnaire responses
(re. Section )


![analysis of qu.png](../../Zettlr_Images/analysis of qu.png)



## Appendix 14

Example of Story Cards
(re. Section )

![unselect veg texual desc.png](../../Zettlr_Images/unselect veg texual desc.png)
![story card 2.png](../../Zettlr_Images/story card 2.png)


## Appendix 15

Volete Template defining the systems scope
(re. Section )

![volere1.png](../../Zettlr_Images/volere1.png)

![volere2.png](../../Zettlr_Images/volere2.png)


## Appendix 16 
Comparison of Web, Native and Hybrid technologies
(re. Section )

TM352 compared different approaches to mobile development: web, native and hybrid. Hybrid development seems the most appropriate as there would be a single code base for all platforms, and a variety of languages and frameworks can be used. Hybrid applications also benefit from the device’s sensors, making it a fitting choice for an app which may require location data, camera facilities and notifications. (For EMA, add table summary.)

## Appendix 17

Domain analysis activities
(re. Section )

Potential concepts:
Tangible objects: Computer system, Allotment, Phone, Plot, Vegetables, Crops, Soil, Notes, Seeds, Patch
Roles: Growers
Organisational units: Allotment, Weather Forecaster

Analysis of Candidate Classes:

| Candidate       | Type            | Represent as class?                                                                                     |
|-----------------|-----------------|---------------------------------------------------------------------------------------------------------|
| Computer system | Tangible object | Not part of the domain                                                                                  |
| Users           | Roles           | Yes                                                                                                     |
| Allotment       | Tangible object | Yes, this should be considered, but not first iteration                                                 |
| Phone           | Tangible object | Not part of the domain                                                                                  |
| Plot            | Tangible object | Yes                                                                                                     |
| Vegetable       | Tangible object | Yes                                                                                                     |
| Soil            | Tangible object | No. Might be considered as as attribute of Plot or Allotment                                            |
| Notes           | Tangible object | Yes, but not MVP                                                                                        |
| Seeds           | Tangible object | No. Might be considered later as an attribute of Vegetable or class when defining the quantity required |
| Patch           | Tangible object | No. Synonym for Plot                                                                                    |
| Growers         | Roles           | No, duplicate                                                                                           |

## Appendix 17b
Initial Class Diagram sketch from TMA01
(re. Section )


![rough_sketch.png](../../Zettlr_Images/rough_sketch.png)


## Appendix 18
Questionnaire sent to Stakeholders, asking preference on Calendar, Timeline or Task list
(re. Section )

Please refer to Appendix 2b

## Appendix 19
Mockup Design Feedback
(re. Section )

| Person | Comment                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|--------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| KT     | Yeah certainly gives an idea of what it does! Thoughts: 1. What happens when you click on the buttons at the bottom of the page on the 'sign up' page? Maybe doesn't need to be there? 2. When I'm on the page with heading "My Plot Name", how do I know how to add veg? (think this is through the vegetables tab but not clear from the plot page) 3. Just a tiny thing but on the 'My Tasks' wire frame youve got 'this month' highlighted but it's showing both Feb and March 4. Are the boxes with 'x' on the calendar page little pics of the page? Not super clear what they represent |
| PC     | I think the app looks great. Maybe just a list for the calendar. It seems very simple to use                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| VH     | I like the overall calendar view that you can populate with the veg that you are interested in - if that could then generate a tasks/to do list I think that would be great. So essentially all starts with a list of what you want to grow - that shows up on a calendar view, auto generates a tasks list and allows you to plot the produce into your plot.                                                                                                                                                                                                                                 |
| EN     | It looks cool! I like the companion planting and good/bad neighbours                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| Chris  | I like the first format for the veg timeline/calendar, as I'm mainly concerned with a broad overview of what I need to do throughout the year. However, I'd prefer for them to be ordered from the time they first need to be seeded rather than alphabetically. I think the mockups give a clear view of what the app will do: add a plot, add veggies to that plot, add notes about the veggies you've added, and the app will give you info about those veggies and a handy calendar view about what tasks you need to do when.                                                             |

## Appendix 20

Screenshot of GitHub commits for both repos: Rails back-end and Expo React Native front-end 
(re. Section )


![rails git commit.png](../../Zettlr_Images/rails git commit.png)

![expo git commit.png](../../Zettlr_Images/expo git commit.png)

## Appendix 21
Screenshots of GitHub project structure for both repos: Rails back-end and Expo React Native front-end 
(re. Section )

![rails project structure.png](../../Zettlr_Images/rails project structure.png)

![expo project structure.png](../../Zettlr_Images/expo project structure.png)


## Appendix 22

Screenshot of React Native code, shoing a Redux Action
(re. Section )


![code redux veg action.png](../../Zettlr_Images/code redux veg action.png)

For the EMA, add screenshot of configuration code which Seeds the database

## Appendix 23
Reflection and analysis of tools used in the project
(re. Section )

I am using Zotero as a reference manager and I have got better at saving the a reference to Zotero straight away from the browser plug in, and then writing up in the journal my days learning. However, I would have benefitted from adding reference specific notes at the time of saving, becuase I has been hard to remember exactly what conent was used in a reference for a particular task when it has come to writing up TMAs. Learning the PROMPT (ref) method has helped me to criticially evaluate references, something that I need to continue to work on before the EMA. Along side papers and official documentation, the project has extremely benefited from Stack Overflow posts. When I have been stuck on a particular problem, the majority of time Stack Overflow has a post discussing something similar. (Appendix xx)

Postman was a tool which also helped during development of the Rails API. (ref) It allowed me to test the API before any front-end implementation, easily adapting parameters, URLs, and checking what response and status are returned for different methods. As the Rail API was implementing a JSON API ([ref](https://jsonapi.org/format/)) the body and responses were relatively straight forward. Postman also provides automatic documentation of the requests, and therefore API, which will be used an a way of evidencing work done. The API is also a successful interface, and I like how the front-end and back-end are completely seperated. This gives me more piece of mind when I am working on a piece of code, that changes are in isolation. Additioanlly, becuase I have experience in Rails, I found it quite quick and straight forward to get the API up and working. Allowing me to focus more time on the front-end.

As for project management, I have learnt how to use Gantt charts and appreciate the value of them as I have referred back to and updated mine lots throughout the project. It was particularly useful when estimating how much development work could be completed when decidign scope. Although I have used my Project Journal increasingly more, stating what I have done each session, I have been using GitHub story cards more.

GitHub has been an invalueable tool for this project. Each sub-task has a individual card, where I have been able to add notes, images, tables etc, all in markdown so they can be copy and pasted directly into my word processor, Zettlr. This has and pulling in information for the TMAs more straight forward. The project board with column: Todo, doing and done makes it easy to see the current and upcoming state of work. Card can be moved, and therefore priotisied easily, as well as grouped into "Milestones". In my WaterScrumFall process, these have acted like stages. (appendix 30) Finally, cards can have labels, which has been useful when assigning sizes to cards, as these can be filtered easily. However, the card almost make it too easy, and it can get a little unorganised. For the final few months, I will try an maintain the journal better and organise the information I add to cards better. I have also used GitHub to version control my TMAs acts as a backups. 

(For the EMA, add a section on LucidChart)

## Appendix 24

Stakeholder feedback from the MVP
(re. Section )

| Person | Feedback |
| --- | --- |
| SC  | I didn’t think the “Welcome” Page had enough on it - wasn’t that “welcoming” if you know what I mean - a few more veggie graphics & perhaps some encouraging words for those just starting out on allotment ownership… ?!? I also thought the vegetable graphics all looked the same too & would be good if they were veggie specific - possibility of any extra ?! “Top Tips” for creating excellent compost area … how to build your own shed …. Maybe links to other useful sites - eg RHS …. |
| HC  | the functionality looks like it's already really good! I feel like it is mainly visual stuff that I would edit, so as you said maybe make it less white and more green and add a few more pictures/graphics. And then the only other thing I noticed was the timetable grid is a little off, I'm not sure if it can be better aligned to have the icons directly under months? And yes the remove vegetable function I would say seems important |
| PM  | Think it's looking brilliant. Really like the timetable at the end. - Is there any way of removing/deleting a plot or veg once added? - Will there be any sort of tooltips or guidance for those that are less digitally literate? - Is there a search functionality if someone has e.g. multiple plots or multiple veg added to find which veg is in which plot etc. - Calendar function to 'look ahead' and see what's coming up in terms of planting or harvestin - Can you view vegetables before adding them to the plot? Maybe recommendations on what to plant? - Pictures of the different veg for those of us who have no idea what Swiss chard looks like - Ability to upload photos of each planted veg maybe?! |
| FC  | It's amazing, well done. Couple of notes: - Do you need a 'Sign in' button as well as a 'Sign up' button after an account has been made or are you assuming you always remain signed in? If not you could make the Welcome page more personal? So it says 'Welcome Harriet' if they add their first name. - Need a plus sign to show where you can add vegetables to the plot page. - Need a plus sign on timetable or do you click on 'seed' to add a date? - Where will the 'frost dates' appear? Will it be on the timeline- can you use a frost icon for this? |
| JO  | \- national trust green would be better than purple - I missed the location checkbox, make it bigger/ better description. - I wasn't sure how to add a vegetable to the plot, can a add button be on the plot screen. - There was no feedback when adding a veg to the plot. - Add image of veg in timeline or three letters. - When clicking on the nav bar, I expected to be taken back to respective home pages, not the screen where I had last visited (eg veg description) |


## Appendix 25
Project Journal
(re. Section )

![journal1.png](../../Zettlr_Images/journal1.png)
![journal2.png](../../Zettlr_Images/journal2.png)
![journal3.png](../../Zettlr_Images/journal3.png)

## Appendix 26

Critical review of how I have tackled the project (LO5)
(re. Section )

* good start with a the idea, some research, questionaire, requirements
* got lots of requirements as inspired from everyone saying this would be so great and useful
* also hoped to base equally off tm352 and tm354, with containerisation and cloud deployment
* jumped in building too quickly in a agile way
* tma01 came around very quick and I started to panic as I didnt have much structure, and felt out of control
* almost started again after tma01, following TM354 very strickly, and dropped tm352 apart from the odd ref
* also changed to waterfall
* since that, been much better at planning, workload, knowing whats coming up, what i need to work on next
* gantt chart also good for an overview
* with critical start dates guesing how long each feature would take
* reduced scope meant i could imagine the finished probject which helped
* git hub story board/ project/ milestones/cards been savour
* impleemntation went well afetr all the planning
* glad to have got basic html working, before adding ux
* tried adding manually css, but quickly realised that would be too much work
* more reflection after each story, not just in journal but in github card


## Appendix 27

Initial Gantt Chart, created after TMA01
(re. Section )

![gantt full.png](../../Zettlr_Images/gantt full.png)


## Appendix 28
 
List of Resources identified prior to TMA03
(re. Section )

|     |     |     |
| --- | --- | --- |
| Resource | Why needed | How to obtain |
| Stakeholders | Gathering requirements, provide feedback and testing final product | I am in frequent communication with 13 stakeholders. |
| Vegetable Data | Populate vegetable information in tables | I was unable to find sufficient vegetable data. I have manually added vegetable information from my book. This is stored as a Rails seed, which is a configuration file which can be ran on database set up. Automatincally inserting each row in the relevant databases. Appendix shows screenshot of seed code. |
| XCode | Emulator the hybrid application locally | Installed. Working well |
| Expo | Easy testing of app by scanning a QR code | Downloaded the software and installed the iOS app. Working well |
| Ruby on Rails | To build the back-end service | Installed |
| React Native | To build the front-end UI | Installed |
| Weather API | To retrieve frost dates for a users location | I was unable to find a frost date api based of location. I found one for america, but not UK. Going to stub out this data and assume usage is only in UK. Based on Cambridge. Frist: 11th Dec. Last 20th April, (ref plantmaps) |
| GitHub | Version control code and Project Board | I have created a project and a repository. |
| LucidChart | Build Mock ups, ERD, activity diagrams etc | I have an account through work |
| Zettlr | To write assignments in markdown format | Downloaded. Creation of tables is temperamental. I am creating tables on Google docs and adding them in later. <br><br>I have better used my reference manager, Zotero, adding notes and populating missed data, and my writing tool, Zettlr, is now linked to Zotero, which automatically imports citations. In general, this is much more efficient and effective.. |
| Zotero | To store and manage references | Downloaded |


## Appendix 29
List of Skills identified prior to TMA03
(re. Section )

| **Skill **          | How I have developed the skill since TMA01                                                                   |
|---------------------|--------------------------------------------------------------------------------------------------------------|
| Project Management  | Creating clear tasks and subtasks helped. Creating and adding these to a Gantt Chart                         |
| Research            | Attended an OU Library tutorial. Read Library Links resources. Researching on Google Scholar and OU Library. |
| Report writing      | Modules TM358 and TM470 require a lot of report writing. Plan to read OU Report Writing skills resource      |
| SQL                 | Practised SQL during work project                                                                            |
| UX Design           | Mocked out the systems UX design and iterated on this since receiving Stakeholder feedback                   |
| Hybrid Technologies | Prototyped both Vue Cordova and React Native applications                                                    |

| **New Skills acknowledged** | **Why needed**                                              | **How to obtain / already got it**                          |
|-----------------------------|-------------------------------------------------------------|-------------------------------------------------------------|
| EDI and Accessible design   | To abide with Law and ensure the applications accessibility | Continue reading free eBook called "UX Design for Mobile".  |
| Stakeholder communication   | Be efficient and effective in my requests to Stakeholders   | Reread TM354 Unit 9 on Stakeholder involvement              |


## Appendix 30

Futher reflection on learning from individual stories
(re. Section )

User story: "Create tab navigation"
- React Navigation, also starting to understand. Original wanted no tabs showing when initially creating a user, but time boxed that and now going to check whether a user exists then render a different component, so the navigation is the same throughout
- Couldnt get navigation to work with plot vegetable component so changed approach to adding include to back end, so on getting a plot it would also get the plots vegetables info, so that can be renders in the plot pag

User story: "Create user"
- Install redux to persist user - do we need a user? 
- Started Sign up user. Adding scafford for Rails backend and tabs and import basic component in front end
- Struggling with getting error to be thrown, but still get response. Rails.application.config.action\_dispatch.show\_exceptions = true. Commented out in `rails_api_mysql_project/spec/requests/users_spec.rb` for now

User story: "Create plot"
- pass in a user to plot creation
- textual description
- activity diagram

User story: "View plot"
- acceptance criteria

User story: "View vegetables"
- reusable
- textual description/ acceptance criteria
- - lists 
- componentDidMount
- want to make it reusable, hard to know how yet
- [story](https://github.com/harrietc52/TM470/issues/7)

User story: "View veg info"
- reuse
- child component 
- pass in props
- and update navigation
- [story](https://github.com/harrietc52/TM470/issues/71)

User story: "Add veg to plot"
- Textual description [<ins>here</ins>](https://github.com/harrietc52/TM470/issues/70)
- acceptance cri
- pre/ post conditions (ref)
- example test
- Activity diagram [<ins>here</ins>](https://lucid.app/lucidchart/5fb49364-f050-48de-95fb-1c7f0abe3e86/edit?invitationId=inv_7101815a-8a70-4989-abd3-05e2c8d274ee&page=rMVuOl_Jmzx7#)
- [story](https://github.com/harrietc52/TM470/issues/70)
- The one studied in the most detail was Add vegetable to plot. 
- We analysed it using object diagrams to illustrate the state of the system at various points, and developed a design for the interaction involved in this use case, as shown in Figure 3. 

User story: "View plot vegetables"
- different want to do this
- either scope and include
- or retun as part of plot info, and dont do extra request
- two different activty diagrams


User story: "Get location"
- [story](https://github.com/harrietc52/TM470/issues/43)
- looked at a few different packages/ libraries
- https://reactnative.dev/docs/0.63/geolocation  
- https://reactnative.directory/?search=geolocation  
- https://www.npmjs.com/package/react-native-get-location
- Location on a Plot was initially a user-defined type. However, after accesing the devices location, it was returned as an object with latitude and longitude, and individual big ints. Therefore a Location class isn't required, as it also do not now contain any behaviour, but instead lat and long attributes added to Plot. 
- This adds constraint, that plot locations will be assumed to be in south UK, as the frost dates will be hard coded. 
- Since TMA02, removed the frost locations, as struggled to find an freely available API based with UK data. frost dates - could not find api. Adding Constraint, assuming used in UK based, specificaitlly cambridgeshire, as frost dates and sow/plant/harvest dates set for all vegetbales the same (as planned for in in Risks) going to stub out the data for now, so can still use hybrid device location to get location and send to backend and store. Then will return with stubbed data about frost dates the same for every location. (covered in risks)

User story: "Show timeline"
- story [here](https://github.com/harrietc52/TM470/issues/41)
- researched plug ins
- Attributes:
    - Initially it was decided sow, plant and harvest datas would be attributes on a PlotVegtable object. As it was throught these would be depended on the Plots frost dates. However, as frost dates mocked out, these dates are constant for all vegetables. Therefore the attribute can belong to the Vegetable class.
- Data types:
    - It wasn't clear how best store the sow, plant and harvest dates
    - a range of months (jan - march)
    - or a object {sow: [jan, feb, march]}
    - or many lists sow: [jan, feb], plant: []
    - but lists are hard to store in db
    - use index as months, with strings [0,1,1,2,2,...]
        - where 0 is nothng, 1 is sow
    - store as stringvole
        - '0,0,1,1,1,2,2,2,3,3,0,0'
        - parse to list
        - and assign number to task
    - could develop further with enum
        - Could improve this to enum though, not int. Where sow = 1, plant 2 etc. if enum would be better 
        - sowKind = TaskKind.SOW;
    - could be stored differently as config, and unlikely to change

## Appendix 31


Class Class Diagram of the system, V2 from TMA02 (Appendix 17b shows V1 from TMA01)
(re. Section )

![class diagram after analysis.png](../../Zettlr_Images/class diagram after analysis.png)

## Appendix 32
Reflection on creating a prototype in Cordova and React Native. 
(re. Section )

Setting up Cordova proved complex. Cordova requires XCode to run the iOS simulator. I am developing on my work laptop so didn’t have the correct permissions to install XCode. It also required a lot of memory. Firstly, I installed a too recent version of XCode for my operating system. Then, the XCode command line was not picking up the “PATH” of the more recent version.

Cordova in the browser was successfully retrieving the MySQL data. However, the iOS simulation wasn’t. After researching, this was because the simulation had a different origin to my laptop. I had to install a transport security plugin (“Cordova-Plugin-Transport-Security” n.d.) and add a HTTP Content-Security-Policy meta tag in the Vue HTML. (Code fix is shown in the background of Figure 14) (“Allow List Guide - Apache Cordova” n.d.)  this sort of thing can be a nightmare!

This solution took a while because it is impossible to debug the iOS simulator. A post in Stack Overflow suggested developer tools in Safari. Once I found the error in the Safari console, debugging was much quicker.

When developing the React prototype, similar security issues to the Vue prototype resurfaced. I relaxed the CORS constraints in the back-end and added headers to requests, resulting in a different Network error: iOS does not allow HTTP requests. I then served Rails on HTTPS using a Self Signed Certificate. This worked on my laptops emulator but not my phone because the request to "localhost" from my phone, was understandably, not reaching my laptop. 

I updated the request to point to the laptops IP address. The request was now timing out which was progress. A Stack Overflow answer [@rice_answer_2019] solved this exact problem, suggesting binding the Rails server to 0.0.0.0, which was successful as my phone accessed bank-end data over the internet. This internet dependency was confirmed when developing the application in the car. I hotspotted which changed my laptops IP address because of the different network. Updating the front-end request to use the new IP successfully served the back-end data again. 

The development of working prototypes for both Vue Cordova and React Native was a big learning curve. Carrying my learning experiences from one prototype to another was rewarding. I then felt in a strong position to choose between the two, knowing they both fundamentally work.
