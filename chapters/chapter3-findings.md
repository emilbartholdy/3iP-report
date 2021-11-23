---
# below is required for intellisense of citations to work
bibliography: [biblio.bib]
---

\newpage

# Findings {#sec:findings}

The following sections will answer our research questions. Sec. [-@sec:challenges] will answer our first research question *"What challenges affect the Drivers in the onboarding process at Chainge?"*, while [@sec:solution] will answer the second research question *"How might we improve the onboarding process to make it more efficient for the Drivers and Chainge?"*

## Challenges in Onboarding Process {#sec:challenges}

Through our interviews, observations and following analysis of data, we found several challenges that affect Drivers in the onboardring process (see [@tbl:challenges]).

| ID  | Challenge                                                                  |
| --- | -------------------------------------------------------------------------- |
| 1   | **Drivers receive large amounts of information in an unstructured manner** |
| 2   | **Procedures or practices are not learnt before first ride**                   |
: Challenges experienced by Drivers {#tbl:challenges}

\newpage

**1: Drivers receive large amounts of information in an unstructured manner**

One of the more important observations we made occured just before a planned observation session with one of the newly hired drivers as mentioned in [@sec:participant_obs]. This observation suggests that the current onboarding process does not give new Drivers structured information concerning their job. Furthermore, the amount of information given before their first drive was significant with many details to remember. For example, the manager explained how certain product items on a product list are prepended with characters that have special importance to the delivery. This is further supported by our interview data (see [appendix @sec:interviews]). One interviewee mentioned how he somewhat got the information he needed to do the job properly, however, this information needed structure and could be better formalised (see [appendix @sec:interview_1]). So while employees at Chainge use valuable time to share information concerning Driver's job, the information is challenging for Drivers to consume because there are large amounts of it just before their first drive, and it is presented to them in an unstructured manner. This valuable time by Chainge could be more productively used elsewhere in the company for other tasks. A conseqence of the challenge could potentially result in more errors when delivering products which can affect the drop-off rate. In this regard, one interviewee mentioned that while the job is not difficult it still needs to be done systematically to circumvent negative consequences (see [appendix @sec:interview_1]).

**2: Procedures or practices are not learnt before first ride**

One incident during one of the interviews was particularly interesting. When the interviewee was asked about challenges related to job tasks, she referred to a situation where the recipient was not home to receive the package. Instead of bringing the package to the headquarters, she went back later on her delivery route to try and deliver the package again (see [appendix @sec:interview_3]). The interviewer that conducted the interview would probably not have paid special interest in the statement if Torben had not explained the standard procedure some days in advance. The standard way of working is to only try to deliver the packages once and if nobody is at the designated location, then the package is to be brought to the headquarter, as too much time is otherwise spent on delivering a package which hurts the drop-off rate. Another similar example was experienced by another interviewee. He explained that he had trouble locking his bike so he had make a call to headquarters to learn how to do the procedure of locking the bike (see [appendix @sec:interview_2]). These examples show how drivers have not learnt certain procedures and practices before their first ride, even if the procedure might be important for Chainge's profit (first example) or is relatively simple to do (second example).

## Solution {#sec:solution}

Due to the scope of the project, the proposed solution is designed for internal use only as the users are employed at Chainge. The users of the solution are primarily the new Drivers but also the existing Drivers and the management of Chainge. The solution was developed by following the approach described in [@sec:ideation_workshop]. It is based on the previously described challenges in [@sec:challenges] to accommodate Chainge's needs.

We have named the solution *Trainge* (Train + Chainge) and in a final form it would consist of multiple larger components. Due to course time restrictions, our prototype only illustrates one of these components within the Trainge platform. This component is an realisation of an e-learning platform that contains videos and other resources that can educate new drivers. It can be viewed by clicking [this link](https://emilbartholdy.github.io/Trainge/) (or enter this url into your browser: https://emilbartholdy.github.io/Trainge/).

![Right: Home page of the e-learning part of *Trainge*. Different videos present themselves and are tagged so that Drivers can see the overall theme of the video. In this example the uppermost video is about tools they use as Drivers. Left: The content of a video page. It shows the video itself, along with explanatory text and other resources, if needed.](./figures/solution.png)

The solution solves both challenges

As stated, the proposed e-learning section is part of a platform that is accessed with login credentials to personalise the content and to ensure data security. The idea behind this platform is to create a space for each individual Driver to obtain and store knowledge relevant to their job. The proposed solution is designed to assist the Drivers whenever they need support. For instance, the platform could be useful to utilise when in doubt of which app to use when delivering packages for a specific client or how to use internal apps. In this case, the Driver could watch a video describing in detail what action is needed. One of the interviewees described that he did not receive an introduction to how to use one of the apps so he needed to figure it out by himself (Interview 1). It could be an ideal use case for utilising the proposed solution to watch a video about the app.

The videos are intended to be informative and accessible ad hoc. We imagine that the videos are especially valuable in the beginning of employment, when there is a lot of new information to process and memorize. The e-learning section addresses the challenge concerning lack of knowledge of Chainge's procedures and practices.

### User Testing {#sec:user_testing}
We evaluated and tested the prototype with a respondent. We wanted to test if the respondent understood the Driver’s potential work tasks by viewing the video that we have created. The tester confirmed that the high fidelity prototype was easy to use and understand. The tester suggested new features that could be added to the platform. We have not implemented the suggestions due to the scope of the course.

### Organizational Context {#sec:organisational_context}

The proposed solution is valuable for the management of Chainge. The platform is digitising and standardising work routines, consequentially optimising the use of resources spent on onboarding new Drivers. During participatory observation at the headquarters, we observed a manager at Chainge explaining to three new Drivers how to pack a cargo bike for a certain client [@fig:chainge_driver] <!--(insert appendix + image) -->. The manager was also responsible for picking up the phone if the Drivers were out delivering packages and needed assistance with situations related to delivering. The manager’s phone rang while he explained the process to the new Drivers. The resources could be spent differently and the walk-through could be replaced by a video outlining the process.

The proposed solution could be a valuable asset for Chainge in allocating responsibilities more efficiently which could have great impact on the business.

The proposed solution does also entail an element for storage of documents. The documents should be relevant for the individual employee, for instance, a work contract and paychecks. The Driver that we interviewed did not have any knowledge regarding where they could find their paycheck and one of the interviewees had not received a contract yet (Interview 1, Interview 2, Interview 3). The described storage element could be the primary location to place such documents which would ideally create alignment and eliminate confusion.

### Technical Implementation of the Prototype {#sec:technical_impl}
<!-- INSERT REFERENCES -->

The Trainge prototype is built as a web application written in a functional style using F#, as F# offers many language features that prevent program errors compared to other languages such as Javascript or Typescript. Using the Fable F# to Javascript compiler, the prototype is then able to be run as a web application in the browser. The F# code robustness is transitively applied to the resulting compiled Javascript when using Fable.

Several large frameworks are used to realise the prototype, mainly the React and Bulma frameworks which are used to define the structure, look and reactivity of the prototype. Reactivity is important, as it allows the UI to become driven by data instead of imperatively/manually updating relevant UI components when the underlying data changes. This is automatically afforded to us using React. As React is not a native framework to the F# language, an auxiliary library called Feliz is used to interface between F# and the Javascript-based React framework.

The code is structured using the Elm Architecture (TEA). TEA is a way to split an application into smaller applications or components that are easily composed together without introducing unnecessary coupling between said components. Essentially, it is a way to control *spaghetti code* <!-- reference? --> and make sure that error inducing changes in one part of the prototype does affect another part of the prototype. This is strictly not necessary for a small prototype as Trainge, but hugely useful in the case Chainge needs to scale up the prototype to a fully fledged application.