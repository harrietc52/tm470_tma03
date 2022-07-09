# Section 1: Draft Project report 
LO7: All aspects of section 1 should **not** be written in first person; do **not** tell a story; do **not** include masses of theory; do **not** concatenate words 

Each TMA will build on the previous TMA; please include material from TMA02 with a clear indication of what is additional material or what you may have added/changed in the meantime (taking into account feedback received or further work undertaken).

TMA 03 Google doc [here](https://docs.google.com/document/d/1FRhyFJ68vzqCTjrjw2GzF3NQp2sAX56PnLrAv1ZJnqU/edit?usp=sharing)

## Problem description  (1000)
**1000 words**
Aim: Refining the goals and content of your project in the light of progress.

READ TMA03 

LO2. Identify and refine the goals and content of your project which should be within the area of your chosen specialist route, if applicable

LO2 description: Based on progress to date has a realistic assessment of what can be achieved in the next phase and has a clear and plausible schedule to achieve it.

- Overview of the problem being addressed; give enough info of the location if there is one; discuss any initial research or investigation which prompted the project

For example, for the outcome ‘identify and refine the goals and content of your project’ you will start achieving this by identifying the goals and content of your project in the first assessment. You will improve and refine these throughout the whole project until you satisfy the outcome by handing in your final project report – the EMA.

**Checklist**
- made realistic assessment of progress to date
- made appropriate refinements to the project specification
- based on assessment, plan and schedule are achievable, not ambitious and has credibility
- work proposed for the next phase is achievable and substantial
- next phase and has a clear and plausible schedule to achieve it

1.  Refining the goals and content of your project in the light of progress. Assess the risks to the availability of resources you need to complete your project. Plan the final phase of the project.

### a) Nature and context of the problem (270/333)
One useful suggestion is to give short, one- or two-sentence answers to each of the following questions:

#### What is the problem (111)
_…that needs to be solved or understood? _ 
Overview of the problem being addressed; give enough info of the location if there is one


Prior to 2007, growing your own food was largely associated with older middle-class households.  [@church_growing_2015] More recently, vegetable growing has increased in popularity, especially during Covid-19, with currently 15% of UK households growing thier own produce. 

This newer generation drives the modernisation of vegetable growing, and with that new challenges. Growers may not have the experience, old notes or the luxury of time to experiment with growing. Instead, attention spans are short and time is precious, resulting in growers wanting to get up to speed quickly. 

Therefore, this problem presents an opportunity to create a modern, accessible and informative way to help growers learn how to grow vegetables quickly. 
(109)


#### Why is it considered a problem? (111)
_- Issues that are shown or reasons for investigating it _

_discuss any initial research or investigation which prompted the project
i too used book month bu month, all questions around when, not what "quote" big book, was to digitalise_

Having experienced a steep learning curve when taking up growing myself a few years ago (despite repeadly reading the book  "Allotment, Month by Month") it was clear fellow allotmenters relied upon “Age and experience!”, “Trial and error”, or even “A very old readers digest called 'Food from your garden'”, when asked during initial research: “How do you know what to plant, where and when?” (Appendix 1) 

Understandably, this guesswork, learning curve and admin time, required to research and plan, may put off potential new growers; the proposed solution aims to reduce these unknowns.  
(93)

#### Why ‘solve’ it / Benefits (111)
_What will be the benefits of solving it? / Why solve it:_
_- Who will benefit from your hard work? Possibly how will the benefits be seen_

_(You may need to adapt some of these to suit the nature of your project. In particular, you will need to expand a little on the context within which the problem arose: the audience is not familiar with the problem you are solving. In discussing the scope, be very clear about what part of a system or aspect of the research problem/question you set out to develop, evaluate or research and what you decided to leave out. A good problem description and scope are crucial as they are the starting point for the analysis of the problem you are addressing.)_

The result could be more people grow vegetables, which has many benefits. Allotment growers have claimed to save around £950 a year through home growing. (R. Jones 2009) (Note: save costs could have increased since 2009, due to food prices increase.) Growing vegetables also boosts mental and physical wellbeing, improves diets and has a positive impact on climate issues, by reducing the carbon footprint of food consumed. [@jones_why_2021] 
(68)

### b) Proposed solution or recommendations (333/333) 
One useful suggestion is to give short, one- or two-sentence answers to each of the following questions:
#### What are the key ICT aspects of this problem? What is your existing knowledge of this problem area? (106/111) 
_AIM: 1.  Demonstrating and applying a systematic understanding of the fundamental technical concepts and principles relevant to your project.
AIM: 2.  Demonstrating and applying an understanding of the context in which technical knowledge can be applied._

The core system was made with Ruby on Rails, using the MVC pattern (TM354 unit 9). However, React Native is the user interface (or View). Decoupling Rails logic from the front-end is the REST API, which uses HTTP with JSON encoded data to send requests and return responses. (TM352) React Native used Redux as its centralised state storage, and RSpec and Jest are used for unit testing Ruby and React respectively.  
(71)

insert diagrams / lucid chart [here](https://lucid.app/lucidchart/9b8c519d-b181-4139-95aa-f58b8d78eb12/edit?viewport_loc=15%2C-172%2C1275%2C1096%2C0_0&invitationId=inv_a5baf496-8944-4815-8327-bdc1a2601c2a#)


_- Mention the L3 course(s) that are driving your work; describe what you know about the situation already. Will the solution be within the specialism route of my degree?_

_- * integrate and apply relevant knowledge, understanding and skills you have developed during your programme of study_
_- being aware of your knowledge and skills, how you are using them and what you are learning from the experience._

The software solution process is based off TM354 [@open_university_tm354_nodate] with Mobile techniques and web service protocols based off TM352 [@open_university_tm352_nodate]. (Appendix 4)
Additionally, multiple projects at work have involved JavaScript, Ruby on Rails and relational databases. 

(35)



#### Format of oucome/ What, specifically, will you deliver by way of a project output?/ What might the solution do (96/111)
_- What might the solution look like?/ Format of outcome  
- What, specifically, will you deliver by way of a project output?
- How will you present your work / findings / research / recommendations; alternative ways to produce your results_
- speciality of uni l3

_(The description of the proposed solution or recommendations could be about what you aimed to deliver rather than what you will eventually deliver or what you believe you have already delivered or completed.)_

The project output is a hybrid application, ran locally using Expo's iOS simulator. Screenshots of the application, capturing various features will be presented, along with documentation of the API and testing outputs. 
(32)


**What might the solution do (75)**
_The description of the proposed solution or recommendations could be about what you aimed to deliver rather than what you will eventually deliver or what you believe you have already delivered or completed.

- made realistic assessment of progress to date_

The application first asks a user to create an account, and then a Plot, where permission to acces the devices geolocation can be granted. A list of vegetables can be viewed, with further details available for each vegetable. Selected vegetables can be added to the users plot. These populate the Timeline, which displays information regarding when each vegetable should be sown, planted and harvested. 
(64)
 
#### Changes to scope (131/111) 
_- made appropriate refinements to the project specification_


| Scope                         | In or Out | Why                                                                                |
|-------------------------------|-----------|------------------------------------------------------------------------------------|
| Food Bank donations           | Out       | LSE&P research: food standards, unscrupulous growers                               |
| Push notifications/ Alerts    | Out       | Irritable if not managed properly. Requires access to device settings              |
| Plot Layout                   | Out       | Complex front-end skills and data manipulation required                            |
| Remove a plot location        | In        | GDPR law                                                                           |
| Allotment association         | Out       | Prevent discrimination, support notion that anybody can grow vegetables, anywhere. |
| Allotment tips/ seed swapping | Out       | Consequence of above                                                               |
| Frost dates                   | Out       | Freely available API (accepted risk).Stub frost dates if implemented               |
| Task List/ Calendar           | Out       | Second questionnaire prioritised a Timeline (Appendix xx)                          |

Table xx: Scope and evaluation criteria of prioritisation (Moscow Appendix 2)

(131)

### c) Analysis of likely impact  ??? (333)
Scope and evaluation criteria 

Feedback: A proper consideration of professional issues  (see BCS Code of Conduct)

**What impact will your project have on things like, interested stakeholders? - e.g will it change way people have to work; could it put people out of work; will it increase profits; will it reduce time tasks take etc.  Do discuss with your tutor who knows your project.**

What' type of impact (for example people's lives, users etc) is going to have the proposed solution ( project goal) in case the project will succeed
The analysis of the likely impact is what I mentioned plus more like how likely is that ur the project is going to succeed and if so the impact

_(You may not yet be at a stage where you can indicate the likely impact of what you will be developing or, for research projects, what you will be concluding. If that is the case, leave some placeholders for the parts of this section that you intend to work on later for your final report.)_

* identify and address the legal, social, ethical and professional issues (LSEPIs) and the equality, diversity and inclusion (EDI) concerns that may arise during the development and use of computing and IT systems ??

that's mostly the same as the legal, ethical, social consequences stuff we had to write, right?
Sometimes part of what we are asked is going to appear some where else.
However for me The legal ethical professional r the repercussions based on those variables

Explanation: Explanation seeks to identify causes behind what we observe. As such, it often refers to theories and underlying principles or natural laws

???????

realistic assessment of what can be achieved in the next phase and has a clear and plausible schedule to achieve it.

#### Existing Scope

3 weeks scheduled to complete project before starting EMA (7 weeks to dead line)

| Scope                 | Aspect of problem/ subtasks/ associated activities           | Must/ Should | Cost / Value | Evaluation Criterion          | Progress Made |
|-----------------------|--------------------------------------------------------------|--------------|--------------|-------------------------------|---------------|
| Create a user         | With unique username; pseudonymous data                      | Must         |              |                               | Done          |
| Create a plot         | Geolocation access requires explicit consent                 | Must         |              |                               | Done          |
| Show Vegetables       |                                                              | Must         |              |                               | Done          |
| Show veg info         |                                                              | Must         |              |                               | Done          |
| Add veg to plot       |                                                              | Must         |              |                               | Done          |
| Show Timeline         |                                                              | Must         |              |                               | Done          |
| Remove location       | PII; "Right to Erasure"                                      | Must         |              | Very likely                   | Not started   |
| Add colour throughout | Reflect colour blind usability requirements. Make consistent | Should       | V=5, C=S     | Very likely                   | Not started   |
| Welcome page          | Add explanation                                              | Should       | V=5, C=S     | Very likely                   | Very likely   |
| Improve Veg details   | Use "odd" shaped vegetables images. Add individual timeline  | Could        | V=5, C=M     | May require code refactor     | Not started   |
| Remove veg from plot  |                                                              | Should       | V=4, C=M     |                               | Not started   |
| Add/ remove veg notes |                                                              | Should       | V=2, C=L     |                               | Not started   |
| Add alerts on actions | Shneiderman's eight Golden Rules                             | Should       | V=4, C=M     | More complex, Likely complete | Not started   |
|                       |                                                              |              |              |                               |               |
|                       |                                                              |              |              |                               |               |
githubt sreenshot

![improvement milestone.png](../../Zettlr_Images/improvement milestone.png)

Table x: scope and evaluation criteria . Value (5 high, 1 low) Cost (Small/medium/Large). Refecting LSE&P and EDI concerns (Appendix 5)

Cost = S  (1 day)
Cost = M  (2 days)
Cost = L  (3 days)

3 weeks 
- 14 days for all the above. 
- Created a new "Issue" for each one

From feedback:
- Add colour, green
- Welcome page
- Veg description and iamges
- Mini calendar to veg page, 
- Feedback

Screenshot of new tasks in github, and milestones progress

#### Legal, Social, Ethical & **Professional** issues  

EDI concerns [story](https://github.com/harrietc52/TM470/issues/81)
INCLUDE MORE PROFESSIONAL ISSUES read [here](https://learn2.open.ac.uk/mod/oucontent/view.php?id=1859818)

GDPR states PII should be protected, and collected data should state its purpose and duration of persistence. The attribute username classifies as pseudonymous data because it is unique, yet cannot alone identify an individual [@ico_what_2021] Location data however, required for setting frost dates, could be PII as users could be traced to the location. Geolocation access should have the users explicit consent [@ico_location_2021], which is implemented in the system with a checkbox. Under GDPR, users have the "Right to Erasure" [@ico_right_2021] and so button has been added allowing a user remove location data. 

If the system was used outside of the UK, alternative data protection laws would need to be considered. Directive 95/46/EC [@eur-lex_directive_1995] ensures collected data can be processed internally between EU states [@open_university_trans-border_nodate] and since leaving the EU, the UK lost this flexibility. Additional safeguards may therefore be required. Furthermore, if hosted on the Cloud, the role of data controllers and data processors should be especially considered. [@noauthor_controllers_2021] To allow client to server communication, the servers current 0.0.0.0 binding allows all ingress traffic which is a huge security hole. If developed to scale, firewalls, ACLs and ports would need to be configured [@open_university_block_nodate-2] and Cross Origin Requests (CORS) restricted. An API key between the server and client could also be recommended so the server can authenticate incoming requests. 

Regarding social impact, the system will positively contribute to sustainability by preventing waste and unnecessary transportation. Research also shows the mental benefits of growing vegetables [@jones_why_2021], especially during Covid-19, where home growers had higher well-being and lower levels of food insecurity [@mead_growing_2021]. Affected people may involve Stakeholders and the growers to answered the initial questionnaire. The Google From, which handled user authentication, explained no PII such as emails are stored (Appendix 10) but I should have stated when the information would be destroyed. All other communication with the Stakeholders has been via WhatsApp, an encrypted messaging application, and I have been clear that there is no rush or commitment to reply. This project does not directly involve children in anyway as the target market, and therefore Stakeholders, are adults.

If the system became extremely successful, the code could be Open Sourced, allowing developers to contribute, sharing knowledge and skills. An increase in home growing could change growers buying patterns, leading to challenges for small local businesses that grow and sell vegetables. They may need to increase prices which negatively impact people who don't grow vegetables. To avoid this, schemes to support and promote these local business could be considered. 

A deprioritised feature, where left over harvest could be donated to local food banks, could be misused if implemented without careful consideration. Unscrupulous growers could offer damaged vegetables and food quality standards could not be met. Another non-MVP feature of sending push notifications could become irritable to users, if not managed properly. Users would need to be able to able to toggle these notifications on and off.   

Many allotments have an Equality and diversity policy, often based off the Equality Act 2010 [@equality_and_human_rights_commission_equality_nodate]. A few local polices [@allotments_equality_nodate] and [@noauthor_model_2014] aim to provide supportive and equitable environments for all growers. As this system is not constrained to allotments there isn't a specific policy to follow. 

The BSC Code of Conduct [@bcs_bcs_nodate] will guide my work in developing an ethical IT system. ...… the way i will work in a professional manner …  


#### EDI concerns

HCI 

To reflect the increasingly diverse growers, images will be used throughout to make descriptions more creation and images of "odd" shaped vegetables will replace "normal" vegetables. The colour pallet will reflect colour blind usability requirements and gender neutral language will be used [@european_institute_for_gender_equality_gender-sensitive_nodate]. Following [@shneiderman_eight_2016]'s eught Golden Rules, the interface is simple, alerts will be used to prevent errors and the navigation bar provides consistency throughout.

[@w3c_standards_nodate] describes how HTML attributes should have alternative text throughout and provides accessibility evaluation tools. [@reactnative_accessibility_nodate]'s Accessibility Guide describes properties to accommodate all users and the [@npm_react-native-check-accessibility_nodate] plugin can be ran on code to check accessibility compliance.



## Account of related literature (1006/1000)
**1000 words**

- _Your coverage of the literature should display appropriate skills of comparative and critical reading and evaluation_
- _relate the main elements of the literature to each other so that it is clear how individually and collectively they contribute to the problem you are trying to solve_
- _sources that you select should be those that are most important for the critical aspects of your project; (not peripheral issues)_
- _PROMPT doesnt matter, technical content and informed opinion of the authors matters_

_Analyitic tools and Techniques: [here](https://learn2.open.ac.uk/mod/oucontent/view.php?id=1857262&section=2)_

***UX Design for Mobile mock ups/ HCI
Check WaterScrumFall

[@buckingham_allotment_2019] provides a "Month by Month" plan to grow vegetables, including vegetable specific details which were used to manually input application data. Digitialising this content inspired the project idea initially. Project planning resources from TM470 [@open_university_planning_nodate] explain how to create a project schedule, define tasks and subtasks, and suggest keeping a journal to support self-reflection and learning. [@dawson_dawson_2015] project management book gives a ... invaluable overview of … , specifically aimed at students which supports the OU material well.

[@lei_statistical_2017] analysis of the effects of Kanban and Scrum on software development projects concludes the KanBan method maybe be better in terms of managing project schedule. However, this project appeared to benefit from a complete upfront design and plan with timeframes, and therefore KanBan wasn't suitable. Hybrid approaches, such as WaterScrumFall [@rahim_scrumfall_2018] and AppScrumFall  [@bisaa_appscrumfall_2020] were also considered. Both advoacated unfront requirement analysis, with several sprint iterations before delivery, with AppScrumFall emphasising thourough testing across all platforms. Lifecycle approaches, also compared in TM470 [@open_university_choosing_nodate] and TM354 (waterfall vs Agile development), are summarised in Appendix 6. This proejct closely follows TM354 Case Study Resources from Unit 4, 8 and 12 [@open_university_tm354_nodate], which illustrate the application of the software development concepts studied, following a Waterfall approach.

Domain analysis found Jones' [@jones_why_2021] article describing the benefits she experienced through home growing, which included mental and physical health benefits, a new found sense of community and the enjoyment of freshly picked harvest. Mead's research [@mead_growing_2021] found food insecurity during early Covid-19, was reduced for those who grow vegetables, which in turn was associated with better well-being. [@church_growing_2015]'s Ecological Economics paper considdered food growing trends across Europe, stating that only in the UK is growing food "predominantly associated with older middle class households", as ~75% of growers are 35 years or older, leaving a minority of growers between the ages of 18-34. Although written in 2015 (and therefore quite dated), this skewed demographic and the potential to attract a younger generation of growers, heavily influenced the projects problem statement. (Appendix 7)

Existing applications: VeggieGardenPlanner [@veggiegardenplanner_veggie_nodate-1] and RHS GrowYourOwn [@rhs_grow_nodate] and Planter [@planter_planter_nodate], vary in UI quality yet support overlapping features. They allow a user to view vegetable information, add vegetable to the plot and display a calendar or task list associated with the vegetables. 'VeggieGardenPlanner' provides more information on companion planting (which vegetables are good or bad neighbours) and 'Planter' retrieves locations and sets the plots frost dates. These use cases formed the initial scope of the system and influenced the user interface. Other similar resources which were dismissed are described in Appendix 8.

[@neil_mobile_2014] describes many UI examples, both sucessful and unsuccessful, however content appeared dated. Instead [@perea_ux_2017] introduces a pragmatic approach to designing mobile apps, including Andriod and iOS respective best practices and UI elements respectively. [@shneiderman_eight_2016] outlines eight "Golden Rules", a set of key principles to enhance user interfaces. These principles have been derived from experience and refined over three decades. Yet, they state each principle requires fine-tuning for specific design domains and validation from users. They include ...

The TM354 Case Study then follows the process from requirements, to analysis and design. Unit 8 advocates requirement ananlysis through the creation of class diagrams with attributes, assocaitions and operations, as system constraints and allocation of responsibilities can be considdered when structuring classes in a visual way. Unit 12 explored a systems architecture and goes on to describe implementation. 

During back-end development, [@railsguides_getting_nodate] provided a high-level overview to "Getting Started", tailored to a specific Rails version. Rails documentation It was also used to understand how to rollback a migration when adding further attributes and `scaffold`  [@railsguides_rails_nodate]  used to create a full set of model, migration, controller, resource and respective tests, automatically conforming to Rails project structure conventions. However, [@ds_creating_2019] provided a much thourough tutorial, specifically stating how to set up a project in API-only mode, specifiying the test suite and selected database. Additionally, [@livingston_setting_2018] clearly summaried how install and to configure Rspec, finer details which the RailsGuide lacked.

TM352's Cordova development guide provided pratical tasks to set up a project. However, React Native was later chosen for front-end development (Appendix 9). Although [@reactnative_learn_nodate] documentation share simple code to illustrate basic React concepts like `state` and `props`, [@expo_create_nodate] documentation guided the initialisation of the final project.  Then, with the aim of creating a clear front-end directory structure, similar to that which the `scaffold` command provides for Rails, [@reactnativeexample_react_2021] outlined a template for a clear and organised project structure which was adhered to.

During implementation, the mose influencial three-part tutorial  [@fullstacklabs_creating_nodate] described how to build a simple app, using Ruby on Rail API and a React Native client, which first set up a Rails API project, then React Native using Redux for state management, and finally connecting the two. Additionally, TM352, specificifcally JSON and REST resources [@open_university_tm352_nodate]  were revisted when developing this client to server communication. Analysis of tutorial's working code [@adenwala_reactnativerails_2021] provided a greater understanding of Redux flow between store, reducers, actions and action type, along with "Getting Started with Redux" documentation [@redux_redux_2021]. The tutorials use of `async/await` was further explained by [@gagliardi_how_2018], specificaly regarding the use of promises in a `componentWillMount` lifecycle hook. 

ReactJS documentation explained the difference between creating components as a functions or classes [@react_reactcomponent_nodate] which [@geeksforgeeks_differences_2022] compares; Class Components are stateful and ran as part of the React life cycle, thus supporting methods such as `componentDidMount` making it better suited for this project which renders data on component initialisation. Further differences between the Functional and class components are summarised in Appendix 10. [@akshat_react_2019] support the Redux and Component class approach, as they introduced React Naviation, which advocates a wrapper (`withNavigation`) for existing components. Via this approach, the navigation prop does not need to be passed down through multiple child components. [@reactnavigation_access_nodate] 

To improve the systems styling, Material UI [@mui_mui_nodate] and  [@reactnativematerial_hello_nodate] provide different modular and customisable components for React Native, where the latter was selected for its simple installation and usage, and [@expo_expovector-icons_nodate] vector icons have been implemented throughout.  Review of literature which influence the LESP project concerns is provided in Appendix 11. 

(1006)


## Account of project work done and its outcome (1000)
**1600/1000 words**

READ TMA03

LO1. Demonstrate and apply a systematic understanding of the fundamental technical concepts and principles relevant to your project (Knowledge and understanding)

LO1 description: There is a comprehensive and clear account of the fundamental concepts and principles relevant to the work.

 analysis and evaluation of the work done
 
### Analysing the problem

#### Requirement gathering

The initial problem statement (Appendix 7), was drafted to better understand common processes when growing vegetables using personal knowledge and research into existing applications (Appendix 8). The "Requirement Gathering Questionnaire" was then designed, based on this research. Appendix 12 summaries how the Questionnaire was designed. It was created using a Google Form with seven sections: General, Vegetable information, Crop Rotation, Reminders, Companion Planting, Social and Finally. Appendix 13 provides description of each section.

![questionnaire.png](../../Zettlr_Images/questionnaire.png)
![google form.png](../../Zettlr_Images/google form.png)

Figure x: Summary of questions, and screnshot of part of the Google Form 

The Google Form was shared with my Allotment WhatsApp group, via LinkedIn and directly with 13 stakeholders, who forwarded it to relevant friends and family. Appendix 14 shows and overview of the 42 responses which were received. As responses came in steadily, each one could be processed and analysed in turn, grouping reoccuring features into categories. Popular resources such as websites, books and blogs where also noted. Further learning from this questionnaire is discussed in Section x. 

After three weeks the questionnaire was closed and the "Main Takeaways" summarised. These were stand-out requirements that made up the applications Use Cases, as shown in Appendix 15 (ref use case). Use Cases (Figure x), in the form of user stories with textual descriptions, functional and non-functional requirements, were created (ref textual description).  Figure x shows one example of a user story and Appendix 16 includes others. These use cases served as the basis for the functional requirements in the Volere template in Appendix 17. (ref volere template)

![use cases prio:unprio.png](../../Zettlr_Images/use cases prio:unprio.png)


![select veg texual desc.png](../../Zettlr_Images/select veg texual desc.png)

#### Architecture

Architecturally significant requirements (ASRs) were identified, with four characteristics stated below, including an example requirement that drives the system’s software architecture. (twin peaks ref - agile? unit 9)
* _Quality attributes_: Security non-functional requirements stated no personal data will be stored, yet other data will be stored. Thus, a database is required.
* _Core features_ Core features are described by Chen et al as ‘the problem the software is trying to solve’. (ref) For example, the system should allow a user to create, read, update and plots (CRUD). 
* _Constraints_. From initial requirement gathering, an app to support both iOS and Android platforms was preferable. Having explore different approaches to mobile developent: web, native and hybrid (Appendix 18). This preference of a hybrid, places a ASR constraint, limiting the choice of Frameworks available. 
* _Application environment_. The Application environment for the system is locally hosted on a laptop, using an emulator. This requires the abilty mimic device sensors, such as GPS connectivity for location access.

The ASRs resulted in a mixture of architectures: a client–server architecture, with the web browser client sending a request to a web server and receiving a response. The three-layered architecture corresponding to the client, the web server that constructs the response and the database storage (Figure xx). (ref arch unit 9 [here](https://learn2.open.ac.uk/mod/oucontent/view.php?id=1681030)). The database sits behind a REST API, which is used to access and store data, using REST HTTP operations. 

![architecture.png](../../Zettlr_Images/architecture.png)

Ruby on Rails was chosen as the back-end service, due to prior Rails experience and its ability to create a RESTful JSON API quickly. The Rails router provides automatic URL generation, where paths can be specified with approved HTTP methods and in-build mapping between HTTP to Controllers, allows easy object manipulation in the logical layer. [@railsguides_using_nodate] A relational-database, MySQL, was chosen becuase the type of data to be stored is pre-defined, the size of data is very small and relationships (such as a Plot is owned by a User) can be represented.

Two protoypes, using Vue Cordova and React Native, were built to select a front-end Javascript Framework. Following TM352 tutorial (ref) Cordova appear more complex and required manual restarting of the application after every update, unlike React Native, which had dynamic reloading and clear documentation. A working protoype in React Native was completed, following @reactnative_learn_nodate where back-end data was accessed via the API and displayed in a List component, using Expo. (Figure xx) 

![react native prototype.png](../../Zettlr_Images/react native prototype.png "react native prototype.png")


### Synthesising a solution
#### Class Design

Having chosen a technology stack, a class diagram of the software was designed. Firstly, using the above Use Cases, potential "concepts" were identified and analysed, as to whether they justified as classes. (Appendix 19) The final core entities were: User, Plot and Vegetables. Associations required to constrain these classes were then identified:
* User: A user may have only one Plot
* Plot: A plot must belongs to a User
* Plot: A plot could have many Vegetables
* Vegetables: A vegetable can belong to many Plots

This identified the many-to-many relationship between Plots and Vegetables. To handle this, one option was to create an attribute on `Plot` with a list of `vegetableIds`. However, this isn't very scaleable and data on this relationship, such as Notes, could not be  later implemented if required. Alternatively, a joining (or Association) class between Plots and Vegetables called "PlotVegetables" could represent this relationship, where a PlotVegetables may belong to only one Plot. This class, association and constraint was added to the class diagram. (red tm35?) Figure xx shows the updated Class Diagram. 


![class v2.png](../../Zettlr_Images/class v2.png)
Figure xx: 

#### HCI design
Human computer interation diagrams (or mock-ups) were created following patterns from the book "UX Design for Mobile" [@perea_mobile_nodate] *check ref

Bottom navigation is the most common layout for iOS apps, as it is close to the thumb and allows changing sections without much effort. It is recommended there are no more than five sections. The use cases helped select the three sections: My Plot, Vegetables and Timeline, as they would cover the functional requirements. It is also an accepted design pattern to indicate which section is in use, and the ability to go between sections freely. This supports [@shneiderman_eight_2016] 1st principle, as Navigation conforms with the aim of consistency throughout.

Sliding drawer (also know as "hamburger menu") profiles an alternative menu that is used less frequently, such as settings. Here, it is used to remove a User, Plot or location, as to abile with GDPR's "Right to Erasure" policy [@ico_right_2021]. Back buttons were added throughout, allowing a user to return to a previous page, or in a multiscreen task (such as creating a user, then a plot) it can break up the processes into smaller steps. Interestingly, languages written from right to left would have a back button pointing to the right. This application supports only English and constraint to the UK. 

Actions such as swiping to remove a vegetable from a plot, or holding down for more information could be used. However, it is recommended an alternative one-tap interaction is also provided, for those with less experience or accessibility limitations. [@shneiderman_eight_2016]'s 2nd principle "Seek universal usability" also recognises this as encourages features for both novices, such as explantaitons, and experts, such as shortcurs, enrich the design. Furthermore, "floating buttons" are usd to highlight a functionality over other elements, such as the button to add vegetables to an empty plot. (# (FAB) button ref)

The "Picture superiority effect" refers to the phenomenon where people remember images better than words, and therefore images have been used where possible on the Vegetable List, Vegetable details and Timeline views.  Additionally, both [@perea_ux_2017] and [@shneiderman_eight_2016] state that alerts should be used to show and prevent errors, where messages are in clear English.

There were overlapping features between Calendar vs Timeline vs Task List discovered when mocking up. I asked stakeholders for their UX preference from the below three applications: VeggieGardenPlanner, Royal Horticultural Society App and Planter (Appendix 20). The 12 stakeholders felt Option 1 and Option 3 were similar, with the majority preferring Option 1's (Timeline) overview. 

![mockup welcome.png](../../Zettlr_Images/mockup welcome.png)

![mockup plot and veg.png](../../Zettlr_Images/mockup plot and veg.png)

Figure x: Mock ups, Timetable mock up in Appendix 20

#### Implementation

The figures below show various forms of results from the current working system, with more evidence in Appendix 21 in the form of `git commit` messages and project structure and code in Appendix 22. Further implementation details and learnings are shared in Section x.x

![mvp done.png](../../Zettlr_Images/mvp done.png)
Figure x: The MVP "Milestone" stories, as shown in Figure x, were all implemented (or deprecated) since TMA02. 


Before UX Improvements

- ui design
    - After implementing the MVP
    An important goal of software engineering is reuse. We look at architectural styles, which represent basic forms of architecture we can reuse in the design of new systems. Frameworks and product lines provide complete architectures designed for reuse.
    Unit 9 4.2 Frameworks
    - improve ui design
    Styling:
    Then looked into how to make it prettier
    Material UI vs 
    styling out of box
    https://www.react-native-material.com/docs/components/backdrop
    https://mui.com/material-ui/react-list/
    learning styles sheet refactor
    struggling with styling
    when looking at switch found out how to move botton veg pace to end, so happy with more simple ui framework
    



After UX Improvements


![implem welcome.png](../../Zettlr_Images/implem welcome.png)

![implem plot and veg.png](../../Zettlr_Images/implem plot and veg.png)
![implem timeline.png](../../Zettlr_Images/implem timeline.png)
Figure x shows screenshots of the current working system.  


![db schema.png](../../Zettlr_Images/db schema.png)
Figure x: shows the rails database schema



![postman plots.png](../../Zettlr_Images/postman plots.png)

Figure x: Rails RESTful JSON API Documenation, automatically generated and published at `https://documenter.getpostman.com/view/11169298/UzJLPcQF#intro`

### Evaluating the solution

#### Functional requirements

** update volere template

Looking back at the Volere template in Appendix 17, the remaining functional require

* create users
* create, update and delete plots
* set the frost dates for a location
* remove the frost dates / locations, on a plot
* keep track of vegetables
* keep track of selected vegetables
* add, update, delete notes
* provide a Timeline view of tracked selected vegetables
* 
all the functional requirement, apart from removing a Vegetable from a plot, and the creation, update and delete of Notes (as this has been deprecation), have been implemented. 
- compare against volere template
- against problem description


#### Testing

Finally, RSpec has been installed and configured for the testing the back-end Rails service [@livingston_setting_2018]. As show in Figure x: the template of tests are created, due to the `scaffold` command, but they are not yet implemented. Although the development process has not followed strict test-driven development, black-box tests were drawn up for each operation before implementation. Figure x shows two test case for user stories 'Create a plot' and 'Add veg to plot'. Jest will be used to unit test React Native components, however this has not yet been set up. 

![rspec.png](../../Zettlr_Images/rspec.png)


![test1.png](../../Zettlr_Images/test1.png)
![test2.png](../../Zettlr_Images/test2.png)
Figure: xx

#### Feedback

Where possible, stakeholders were asked to interact with the system through the emulator and others sent screenshots of the application (as show in Figure x). Stakeholder feedback is summarised in the below Figure / Appendix. 

![feedback.png](../../Zettlr_Images/feedback.png)






#### Resources 
AIM: 1.  Gathering, analysing and evaluating relevant information to complete your project successfully.

- Include table with all resources even no longer needed ones (highlight those in pale colour)
- Discuss / review whether right ones chosen at start or some added later or not wanted / why

| **Resource**   | When needed | **Why needed**                                       | **How to obtain**                                                       |  |
|----------------|-------------|------------------------------------------------------|-------------------------------------------------------------------------|--|
| Stakeholders   |             | Gathering requirements, provide feedback and testing | I am in frequent communication with 13 stakeholders                     |  |
| Vegetable Data |             | Populate vegetable information in tables             | I have found datasets for individual vegetables. Perform more research. |  |
| XCode          |             | Emulator the hybrid application locally              | Installed                                                               |  |
| Expo           |             | Easy testing of app by scanning a QR code            | Downloaded the software and installed the iOS app                       |  |
| Ruby on Rails  |             | To build the back-end service                        | Installed                                                               |  |
| React Native   |             | To build the front-end UI                            | Installed                                                               |  |
| Weather API    |             | To retrieve frost dates for a users location         | To research                                                             |  |
| GitHub         |             | Version control code and Project Board               | I have created a project and a repository                               |  |
| LucidChart     |             | Build Mock ups, ERD, activity diagrams etc           | I have an account through work                                          |  |
| Zettlr         |             | To write assignments in markdown format              | Downloaded                                                              |  |
| Zotero         |             | To store and manage references                       | Downloaded                                                              |  |

Table x: Resources



#### Skills  

- Include table with all skills even no longer needed ones (highlight those in pale colour)
- Discuss / review whether right ones chosen at start or some added later or not wanted / why
- Discuss / review progress against these and why; mention knowledge gained


| **Skill **          | How I have developed the skill since TMA01                                                                   |
|---------------------|--------------------------------------------------------------------------------------------------------------|
| Project Management  | Creating clear tasks and subtasks helped. Creating and adding these to a Gantt Chart                         |
| Research            | Attended an OU Library tutorial. Read Library Links resources. Researching on Google Scholar and OU Library. |
| Report writing      | Modules TM358 and TM470 require a lot of report writing. Plan to read OU Report Writing skills resource      |
| SQL                 | Practised SQL during work project                                                                            |
| UX Design           | Mocked out the systems UX design and iterated on this since receiving Stakeholder feedback                   |
| Hybrid Technologies | Prototyped both Vue Cordova and React Native applications                                                    |

| **New Skills acknowledged** | When needed | **Why needed**                                              | **How to obtain / already got it**                         |  |
|-----------------------------|-------------|-------------------------------------------------------------|------------------------------------------------------------|--|
| EDI and Accessible design   |             | To abide with Law and ensure the applications accessibility | Continue reading free eBook called "UX Design for Mobile". |  |
| Stakeholder communication   |             | Be efficient and effective in my requests to Stakeholders   | Reread TM354 Unit 9 on Stakeholder involvement             |  |

Add new skills since tma02
- React Native, Redux 
- - Code Academy React Native 




