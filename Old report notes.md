# Section 1
## Scope
LSE&P research raised concerns regarding local Food Banks and privacy complexities for push notifications resulted in deprioritisation. To abide with GDPR laws, the ability to remove a plots location was added, and Allotment association has been remove, to support the notion that anybody can grow vegetables, anywhere. As a consequence, the "Allotment Tips" feature was also removed. Additioanlly, the front-end skills and data manipulation required to create a plots layout, made it too complex. A freely available API to retrieve frost dates based on location was not found, an acknowledged risk, where the mitigation was to stub out the frost dates will be implemented. Another stated risk surfaced, in that vegetable data has not been easily accessible, and therefore vegetable data will be manually entered into the database via configuration. After much debate, the results of the second questionnaire prioritised a Timeline, over Task List or Calender view. (Appendix xx). 


## ICT aspects
The hybrid application has a three-layer architecture: Client, Server and Database. 

- REST API
    - json
    - in rails
    - Want user interface to be independent as possible
    - API decoupled logic from frontend view

Rails `ActiveModel` accepts client requests and forwards them to the supplier objects. This reduces coupling, because the client doesn’t need to know anything about the supplier objects, and their implementation can therefore be changed without any impact on the client. 

rspec


- Database
Mysql
Collection o records, kept in persistent storage, organised and efficient to retrieve records
Rails interact with db via action rector, which hides database implementation
Data stored in tables for relational, (what we are using)
Each row in the db is a record, (screenshot)
Columns each have data of a type
Id unique identified a record, called primary key
Foreign key handle associations
Rails Models handle conversion from db record to object
show screenshot of export tables, erd plug in or dbms


React Native is the user interface, which uses Redux as centralised storage in the front-end, as created plot needs to be stored or access in all three tabs. Ruby on Rails back-end, has a MVC pattern, where the Controller (C) provides assess to the JSON RESTful API and `ActiveModel` converts the MySQL database records into obejcts. 


React Native used Redux as a "single source of truth" state storage, as data, such as `plotId` needs to be persisted through out the application. 


## Lit review
READ TMA03
AIM: 1.  Demonstrating comprehension of the key literature that underpin the project by relating and/or applying them to the project work undertaken so far.

LO4. Gather, analyse and evaluate relevant information to complete the project successfully 
LO4 description: Has continued to find relevant material, from a range of sources of information, clearly showing an understanding of the credibility and significance of the source. Effectively and succinctly identifies how they can contribute to the work to be done.

LO6. Make effective use of a variety of information sources including the internet, demonstrating awareness of the credibility of the source

LO6 description: Clear, concise structured communication using diagrams or other illustrations where appropriate. Opinions and judgements are always supported by relevant argument or evidence as appropriate. Effectively written for a knowledgeable specialist audience.

* make effective use of a variety of information sources, including the internet, demonstrating awareness of the credibility of the source

- Turn into essay format not tabular but remember to PROMPT and say where/ when useful, just use stuff from first two TMAs that are useful, do not include stuff read and dismissed
Structure it to keep stuff together, obviously only use topics relevant to your project!

* Include stack overflow forum, youtube, texts, internet

- Include previous literature read and currently literature read

_Example_
x and y (199x) outline a ... method and suggest ... implies .... They advocate a method that they term ‘...’. Via this approach, a .... They go on to describe a ..., the ‘...’ (for analysing ...), which has been used to evaluate the ..... They conclude that the ... resulting from such an approach will be .... However, they do not discuss how ..... aspects may be handled. The designer retains control over the process and decides which evaluative advice to heed.

The differences between the .... approaches to design and the associated input of knowledge are summarised in Figures 2.2 and 2.3.
Figure 2.2    The serial approach to design and knowledge input
This shows how potentially .… can result when .. is  ..... from the .....





Lifecycle:
- as an early step in project management
- First approach was KanBan, 
- Looked into ScrumFall/ AppScrumFall
    -  then moved to Waterfall or WaterScrumFall. much better fitting, iterating around the individual processes
    -  [@rahim_scrumfall_2018] who explained the benefits of a Hybrid approach called WaterScrumFall. The paper was published online at a highly regarded press journal and comparisons with Agile and Waterfall are still relevant.
    - Similar to [@bisaa_appscrumfall_2020] which is app developemnt specific, as it include the UAT step . States there are several sprints until delivery, stating more emphasis on testing, for hybrid, native, cross platform etc. we are testing only on ios simulator through expo
- Settled on Waterfall 
    - Project is mainly based of TM354. 
    - TM354 Case Studies have guided my process [@open_university_unit4_nodate] [@open_university_unit8_nodate] [@noauthor_unit12_nodate]


Domain:
Research to understand the domain
 [@jones_why_2021] describes the benefits of home growing.
 - still living off veg from previous year
 - part of daily excersise, especially during lockdown
 - healthy to spend time outdoors, energetic but in a natural way
 - working hands and mind
 - over lockdown sense of community (allotment)
 - veg is where means begin, vegetarian over summer

 Published in 2021 during Covid-19, makes this article very relevant. A referenced peer reviewed twice paper [@mead_growing_2021] researched food insecurity during early Covid-19, which was reduced for those who grow vegetables
 - during supply crisis
 - "Participants who engaged in home food growing had lower levels of food insecurity and higher well-being" / "home food growing was associated with less food insecurity, which in turn was associated with better well-being."
 - "Upscaling home food growing by increasing public interest and facilitating engagement in growing by making such opportunities more accessible could have tangible benefits for mitigating the impact of the COVID-19 pandemic on well-being and food security."

 [@church_growing_2015]'s Ecological Economics paper considdered food growing trends across Europe, stating that only in the UK, is growing food "predominantly associated with older middle class households". Although written in 2015, and therefore quite dated, it made me reflect on grower demographic, which really influenced my problem statement.
 - "addition to saving money, the economic benefits of food growing have sometimes been framed in terms of food security"
 - 35 years<  76%
 - 18-34   25%

Existing applications:
Unit 4: You will explore how to decide on the scope of a software system to be developed, and elaborate some of the main use cases for such a system. You will also explore how to document the initial set of requirements using a template, and how to elicit detailed software functional and non-functional requirements and their fit criteria.

Looked for existing applications, what apps are out there already to get feature idea

x and y (199x) outline a ... method and suggest ... implies .... They advocate a method that they term ‘...’. Via this approach, a .... They go on to describe a ..., the ‘...’ (for analysing ...), which has been used to evaluate the ..... They conclude that the ... resulting from such an approach will be .... However, they do not discuss how ..... aspects may be handled. The designer retains control over the process and decides which evaluative advice to heed.

The differences between the .... approaches to design and the associated input of knowledge are summarised in Figures 2.2 and 2.3.

VeggieGardenPlanner [@veggiegardenplanner_veggie_nodate-1] and RHS GrowYourOwn [@rhs_grow_nodate], both existing applications, influenced my mockups. They are both free, appear well maintained and have simple UX. Other similar resources which were dismissed are described in Appendix 3.

[@noauthor_veggie_nodate]
- Good/bad neighbours
- calaendar
- patch plan (paid for)
- bit old school design
[@growveg_vegetable_nodate]

[@planter_planter_nodate]
- better ui
- better implemnentation, more basic, plot plan
- plant list, no selected plants though, 
- calendar
- gets loaction and sets frost dates

[@noauthor_grow_nodate]
- very good information about veg
- add veg to garden
- which populates tasks
 
 Volere template, and detailed software requirements
- aim to gather requirements [@open_university_unit2_nodate] 


Mobile design:
 [@open_university_tm352_nodate] compare and contrast approaches, tools and techniques used to create mobile apps such as hybrid vs native vs web. 
 
- Block3, Part4 Developing Mobile Apps [@open_university_block3_nodate]  described difference between /hybrid/native/web

TM354:
the development of a design with appropriate research
modelling techniques for the design, architecture and testing of software solutions
UML techniques
architectures and design patterns. Make use of the Gang of Four book  (Gamma et al, 1995) and Shaw and Garlan (1996)
evaluation of the design and software if produced (stakeholders)

TM352:
web application design, accessibility and interaction
mobile application design and development
approaches to mobile application development

## Work done
### Synthesising solution
- Follow the order of your life cycle or else be prepared to lose marks e.g.
    - Analysing a problem
    - Design some sort of solution
    - Implementation
- Examples of work done for a development project
- Include some stuff from first two TMAs as well as new work
Evaluating this solution.
- ([Skills of Analysis and Synthesis](https://learn2.open.ac.uk/mod/oucontent/view.php?id=1857262).)

_**- Citations to justify approach / decisions. **_
- Reference any appendices used clearly

- think about how you are going to demonstrate to your tutor that you have done this work to a good standard and in a thoughtful and reflective manner.

**Comparison and contrast**
choosing one solution to a problem among a range of alternatives. Many aspects of … involve making the most appropriate choice, so comparisons and contrasts may well feature in your TMAs. (Tables are often a useful means of documenting comparisons.)
- compare framework uis
- compare state
- db design

**Synthesis**
Term [here](https://learn2.open.ac.uk/mod/oucontent/view.php?id=1857262&section=2): Synthesis involves bringing together more than one body of evidence, or different perspectives or viewpoints. It often involves an attempt to arrive at a unified overview or perspective through a process of integration and/or abstraction. TMAs (especially your final TMA) and the EMA offer important opportunities to demonstrate skills of synthesis.

In your draft report, show the structure you intend to have for this section and start filling in the parts that you may have already done. You may want to structure it in terms of analysing a problem, synthesising some sort of solution, and evaluating this solution. Of course, how these activities are organised within any project management framework may differ considerably. For more guidance see Skills of Analysis and Synthesis.

You may be able at this stage to draft most of the analysis of the problem – that is, some sort of expression of the problem that pointed towards the nature of a solution or recommendations. You should also outline what you have done so far in terms of synthesis. For example, for a research project you may have drafted some conclusions and recommendations based upon a detailed study of the literature. For a development project you should have by now carried out a careful requirements analysis of the problem, designed a solution and made progress developing the solution.


Following TM354 Case Study resources, the stages of which are described below. 

- You may be able at this stage to draft most of the analysis of the problem 
    - –  that is, some sort of **expression of the problem** that pointed towards the **nature of a solution** 
    - 

- Design some sort of solution

- synthesising some sort of solution
    - You should also outline what you have done so far in terms of synthesis.
    - For a development project you should have by now carried out a careful **requirements analysis of the problem**, **designed a solution** and **made progress developing the solution**.
    - For TMA 03, providing evidence of the work you have done and its quality is of particular importance as the TMA includes a draft of your project report.
        - For development projects supplementary evidence might include interview plans plus summaries of interview findings, program designs and code, UML diagrams, evaluation findings, concept maps, design documentation, a business process model etc.
        - omit any auto-generated code

### mock ups
how they were designed ??

- Following closely the book "UX Design for Mobile", chapter "Mobile Patterns - Web App, Android and IOS best Practices". Section, "Mobile application design patterns" [@perea_mobile_nodate] (get correct book ref)

- navigation
    - element used the most, and bottom menu most common layout for iOS apps as close to the thumb, allow change sections without effort
        - divide content of app into max 5 sections
        - used use cases to divide into plot/vegetables/timeline
    - all user to freely go from content
    - hint when on selected
        - accepted design pattern to indicate something has changes/ tab is selected
        
- sliding drawer (known as "hamburger menu")
    - used as a menu drop down, when lots of options
    - or as settings/ profile
    - as far away from thumb, less frequent
- use actions
    - swipe/hold down/
- back button
    - top left
    - interestingly, langyages written from right to left would point to the right, assuming UK based and english speaking
- multiscreen task
    - break up processes into smaller steps
    - use back button to previous screen, for processes with several steps 
    - create user/create plot must happen first



- floating buttons 
    - to make actions stand up
    - bottom area, close to thumb
- no use of dialogs

EDI

- one tap interaction
    - a tap is simple engagement, thumbs up or heart
    - change + - to heart
    - no long tap 
        - ofter alternative
        - those with less experience might struggle

- add pictures
    - people rememver images better than words [here](https://en.wikipedia.org/wiki/Picture_superiority_effect)
    
- portrait and landscape orientations
    - acceleromete to detect orientation?
    - two handed
    - more accessible?
  
- errors
    - 

- based off use cases:
    - Sign up
    - create a plot
    - view vegetables
    - view vegetable
    - add veg to plot
    - view timeline

_(On initialisation, the Fabulous app had a nice way to start. Input data then - a user with a plot)_

# Section 2

## Lifecycle
* Reflection of lifecycle choice
    * comparison table
    * waterScrumFall cycle going well
    * like the structure, nearing end of implementation, then testing and deployment and feedback again
    * waterfall structure worked very well to start, then sprint iterations
    * why scrumfall end up being best suited
    * however as i have done an mvp and got feedback, its not quite waterfall
    * Appendix 24
    * add more about its effectiveness until the final report
* This section should be specifically about the approach you have taken; do not include generic discussion of life cycles or the theory of project management methods.
        * tried them all
        * started with scrum
        * then to waterfall
        * then to waterscrum fall
        * would do more research up front about which one would be bet suited
            * one person team, i work with plans, it suits better than sprints
        * 


# Old
Section 2 can be written in first person

Project reflection pointers [here](https://learn2.open.ac.uk/mod/oucontent/view.php?id=1857256&section=6)

* Is what I am doing now going to get me to my goal – or is it just a sideline?
* Could changing how I’m working help me to get this task done better or more quickly?
* Am I on track for finishing this task when I’d planned, and if not, what am I going to do about it?
* Do I have some other resources I could draw on to help me?
* If I feel something is going wrong but can’t pinpoint what, would talking about what I’m doing with a sympathetic friend help me to uncover the problem and find a solution?
* Suppose my tutor could see what I’m doing – the process, not the outcome. What feedback and mark do I think he or she would give me? Can I use this imagined feedback to improve what I’m doing? How could I improve that imagined mark?

1.  Demonstrating the ability to report clearly and critically on the outcomes of your project work.
2.  Reviewing progress against your latest project plan. Identify major risks to success in the next phase and propose ways to manage these appropriately.

## Process (500)
_**Review your project management. Identify those elements of your plan that have not progressed as satisfactorily as you expected and briefly record the reason(s)**_
_**LO9. Plan and organise your project work appropriately, and keep systematic records of plans, progress and outcomes**_


decide lifecycle [story](https://github.com/harrietc52/TM470/issues/24)

github amazing

rails back end, use postman to quickly test endpoints. posman doumentaiton great




### Review your project management
**500 words**

LO9. Plan and organise your project work appropriately, and keep systematic records of plans, progress and outcomes

LO9 description: Has a clear plan and makes an accurate assessment of progress in relation to the original plan. Understands what has gone well and what has not gone to plan.

Review your project management. Identify those elements of your plan that have not progressed as satisfactorily as you expected and briefly record the reason(s)

Project management glossary terms [here](https://learn2.open.ac.uk/mod/oucontent/view.php?id=1857256&section=7)


### Lifecycle
You may want to start writing a short account of the project management method/lifecycle model that you are using. However, you will probably want to leave the discussion of its effectiveness until the final report. This section should be specifically about the approach you have taken; do not include generic discussion of life cycles or the theory of project management methods.

- Discuss / review usefulness of chosen one in controlling work throughout project

| Lifecycle | Pros in project | Cons in project | Useful in project | Accept / reject/ why |
|-----------|-----------------|-----------------|-------------------|----------------------|
|           |                 |                 |                   |                      |
Table x: Lifecycle choice

### Future Plan/ Schedule

AIM: 1.  Plan the final phase of the project 


insert gantt chart
3 weeks after TMA03
going to do as many of below tasks as possible
sized them and value (C, V)

15 new features (5 small, 3 Medium and 7 Large) came out of this feedback, as shown in Figure xx. With four weeks of buffer before the EMAs critical start date, the below stories will be prioritised based on user feedback and as many implemented as possible, within the given time period. 


- Include current plan
- First plan done in TMA01 put in appendix
- Discuss / review changes and why

- * plan and organise your project work appropriately, and keep systematic records of plans, progress and outcomes

Figure x: Current plan (Gantt Chart)

![improvement milestone.png](../../Zettlr_Images/improvement milestone.png)
figure x: Improvement Milestone, with stories from user feedback as explained in section 1.x










## Product (500)
 _**Assess the risks to project completion (remember that this is not the same as whether you expect to pass or not). Identify any significant risks to project completion and determine how these are going to be managed. Identify those elements of the project that may not be addressed if plans need to change**_
 
 
* evaluating the results of the project
* * communicate information, ideas, problems and solutions clearly
 
 Regarding the technical aspects, give a positive rationale for your chosen evaluation or solutions, also indicate any false starts or particular difficulties. What have these processes taught you about specifying and designing a problem solution? What demands were placed on you and how did you use your project management skills when tackling the technical tasks?
 

**Evaluation**:  
Documenting appreciable progress towards a critical evaluation of your chosen problem/user interface or experiences using suitable technical concepts and principles supported by appropriate references.

Evaluation Term [here](https://learn2.open.ac.uk/mod/oucontent/view.php?id=1857262&section=2): Evaluation normally involves the assessment of something or things against a set of criteria. Sometimes the criteria are readily available as an established ideal or benchmark; at other times, determining, with appropriate justification, the appropriate criteria to use can also feature as part of evaluation. Evaluation may be applied to concrete or abstract entities; an example of the latter is the evaluation of an argument against criteria for valid forms of argument (evidence-based, logically consistent, etc.).

stakeholders [story](https://github.com/harrietc52/TM470/issues/57)


### Assess the risks to project completion
**500 words**

LO3. Identify, list and justify the resources, skills and activities needed to carry out the project successfully. Identify and address any associated risks

LO3 description: Has identified the resources, skills and activities, the timely availability of which is essential. Has judged risks (likelihood and impact) appropriately. High- risk elements have been excluded and other risks are manageable.

Assess the risks to project completion (remember that this is not the same as whether you expect to pass or not). Identify any significant risks to project completion and determine how these are going to be managed. Identify those elements of the project that may not be addressed if plans need to change

By this stage you should be able to write about the risks you had initially identified, the strategies you had identified to mitigate them, and possibly about how effective these were. You may also identify any risks that may still occur before completion and how to mitigate them.




### Progress



## Personal (1000)
### Review your personal development/ progress 
**1000 words**

**Feedback** In reflection you might want to say something about the way you work and when.   e.g short bursts or long sessions.  Night v day, etc.

LO8. Learn independently and reflect on what has been done, with a view to improving skills and knowledge

LO8 description: Makes progress under own supervision, communicating regularly and accurately in respect of progress. Seeks guidance when needed, but offers own ideas when doing so.

Critically reflect on your own experience in order to identify what you have learnt so far, effective ways in which you learn and work, and what you need in order to extend your current knowledge and skills in relation to the work and context of the project.

Reflect on the skills you have acquired or appreciably improved so far in the project. The skills considered may include both project management and self-management skills.

This section should be the result of ongoing reflection as you develop your project and you may have a nearly final draft.

- How is it all going; what have you gained as a person; log keeping (a brief example in appendix); keeping in touch with tutor (a very brief example in appendix)
- thinking about what experience you are bringing to the task, what you are learning and how you can improve your knowledge and skills.
- receive feedback on your assignments, which you can use to improve your performance
- Developing your skills as you work on your project is all about taking responsibility for extending and improving your learning and performance in a context that is broader
- * learn independently and reflect on what has been done, with a view to improving skills and knowledge.

* give a good analysis of what went wrong
* reflect on your own performance
* suggest how things could be improved if you were to do the project, or a similar project, again.


- Go through journal

TM358 EMA for first 3 weeks after TMA02

