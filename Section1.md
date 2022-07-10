# Section 1: Draft Project report

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





