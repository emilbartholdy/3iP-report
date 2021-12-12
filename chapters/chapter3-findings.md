---
# below is required for intellisense of citations to work
bibliography: [biblio.bib]
---

\newpage
\newpage

# Findings {#sec:findings}

The following sections will answer our research questions. Sec. [-@sec:challenges] will answer our first research question *"What challenges affect the Drivers in the onboarding process at Chainge?"*, while [@sec:solution] will answer the second research question *"How might we improve the onboarding process to make it more efficient for the Drivers and Chainge?"*

## Challenges in Onboarding Process {#sec:challenges}

Through our interviews, observations and subsequent analysis of data, we found two major challenges that affect Drivers in the onboarding process.


**Challenge 1: Drivers receive large amounts of information in an unstructured manner**

One of the more important observations we made occurred just before a planned observation session with one of the newly hired drivers as mentioned in [@sec:participant_obs]. This observation suggests that the current onboarding process does not give new Drivers structured information concerning their job. Furthermore, the amount of information given before their first drive was significant with many details to remember. For example, the manager explained how certain items on a product list are prepended with characters that have special importance to the delivery. This is further supported by our interview data (see [appendix @sec:interviews]). One interviewee mentioned how he somewhat got the information he needed to do the job properly, however, this information needed structure and could be better formalised (see [appendix @sec:interview_1]). So while employees at Chainge use valuable time to share information concerning Driver's job, the information is challenging for Drivers to consume because there are large amounts of it just before their first drive, and it is presented to them in an unstructured manner. This valuable time by Chainge could be more productively used elsewhere in the company for other tasks. A consequence of the challenge could potentially result in more errors when delivering products which can affect the drop-off rate. In this regard, one interviewee mentioned that while the job is not difficult it still needs to be done systematically to circumvent negative consequences (see [appendix @sec:interview_1]).

**Challenge 2: Procedures or practices are not learnt before first ride**

One incident during one of the interviews was particularly interesting. When the interviewee was asked about challenges related to job tasks, she referred to a situation where the recipient was not home to receive the package. Instead of bringing the package to the headquarters, she went back later on her delivery route to try and deliver the package again (see [appendix @sec:interview_3]). The interviewer that conducted the interview would probably not have paid special interest in the statement if Torben had not explained the standard procedure some days in advance. The standard way of working is to only try to deliver the packages once and if nobody is at the designated location, then the package is to be brought to the headquarter, as too much time is otherwise spent on delivering a package which hurts the drop-off rate. Another similar example was experienced by another interviewee. He explained that he had trouble locking his bike so he had to make a call to headquarters to learn how to do the procedure of locking the bike (see [appendix @sec:interview_2]). These examples show how drivers have not learnt certain procedures and practices before their first ride, even if the procedure might be important for Chainge's profit (first example) or is relatively simple to do (second example).

## Solution {#sec:solution}

The solution or prototype is based on the results from the ideation workshop (see [@sec:ideation_workshop]) and is meant to adress the challenges described in [@sec:challenges].

We have named the solution *Trainge* (Train + Chainge) (see [@fig:solution]) and in a final form it would consist of multiple larger components. Due to course time restrictions, our prototype only illustrates one of these components within the Trainge platform. This component is a realisation of an e-learning platform that contains videos and other resources that can educate new drivers. It can be viewed by clicking [this link](https://emilbartholdy.github.io/Trainge/) (or enter this url into your browser: https://emilbartholdy.github.io/Trainge/). The video can also be accessed through ITU's video platform with the title "Cluster_A_TeamNr_1" and is published by Emil Bartholdy (emba).

![Right: Home page of the e-learning part of *Trainge*. Different videos present themselves and are tagged so that Drivers can see the overall theme of the video. In this example the uppermost video is about tools they use as Drivers. Left: The content of a video page. It shows the video itself, along with explanatory text and other resources, if needed.](./figures/solution.png){#fig:solution}

The prototype adresses challenge 1, but ensuring that training of new drivers are standardised and structured, such that all drivers receive the same knowledge. New Drivers can filter material that is relevant to them, and study that before their first drive at a pace that fits them. This is preferable to being told a large amount of important information just before their first ride that they are likely to forget.

Furthermore, the prototype addresses challenge 2 as Drivers can learn what procedures or practices they should do in certain situations before they on their first drive. Driver's could even look up what to do in special circumstances in situ on their mobile phones, as the solution is compatible with smartphone browsers. For example, the driver who didn't know what to do when she could deliver a package, could look this up on her phone.

The videos in the solution are intended to be informative and accessible ad hoc. We imagine that the videos are especially valuable at the beginning of employment when there is a lot of new information to process and memorise. The e-learning section addresses the challenge concerning the lack of knowledge of Chainge's procedures and practices.

### User Testing {#sec:user_testing}
We evaluated and tested the prototype with a respondent. We wanted to test if the respondent understood the Driver’s potential work tasks by viewing the video that we have created. The tester confirmed that the high fidelity prototype was easy to use and understand. The tester suggested new features that could be added to the platform. We have not implemented the suggestions due to the scope of the course.

### Organisational Context {#sec:organisational_context}
Chainge is founded in 2019 and is still characterised as a start-up with informal processes. The proposed solution is valuable for the management of Chainge in terms of scaling the company. The platform is digitising and standardising work routines, consequentially optimising the use of resources spent on onboarding new Drivers. The proposed solution could be a valuable asset for Chainge in allocating responsibilities more efficiently which could have great impact on the business.

The proposed solution does also entail an element for the storage of documents. The documents should be relevant for the individual employee, for instance, a work contract and paychecks. The Driver that we interviewed did not have any knowledge regarding where they could find their paycheck and one of the interviewees had not received a contract yet [appendix -@sec:sec_interviews]. The described storage element could be the primary location to place such documents which would ideally create alignment and eliminate confusion.

### Technical Implementation of the Prototype {#sec:technical_impl}

The Trainge prototype is built as a web application written in a functional style using F#, as F# offers many language features that prevent program errors compared to other languages such as Javascript or Typescript [@wlaschinCorrectnessHowWrite2012]. Using the Fable F# to Javascript compiler, the prototype is then able to be run as a web application in the browser. The F# code robustness is transitively applied to the resulting compiled Javascript when using Fable.

Several large frameworks are used to realise the prototype, mainly the React and Bulma frameworks which are used to define the structure, look and reactivity of the prototype. The code is structured using the Elm Architecture (TEA). TEA is a way to split an application into smaller applications or components that are easily composed together without introducing unnecessary coupling between said components [@ajajElmishBook2019]. It is a way to control *spaghetti code*  and make sure that error inducing changes in one part of the prototype does not affect another part. This is strictly not necessary for a small prototype as Trainge, but hugely useful in the case Chainge needs to scale up the prototype to a fully-fledged application.
