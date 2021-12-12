---
# below is required for intellisense of citations to work
bibliography: [biblio.bib]
---

\newpage

# Methodology {#sec:methods}

Our process for addressing the research questions was structured using the Double Diamond model, as described by Norman [-@norman2013design, pp. 220-221]. In [@fig:double_diamond] we describe which methods were used in each phase. Broadly, we used observation and interviews for exploring fundamental issues. For converging on the problems experienced we used colour coding to see which problems were experienced by study participants. With a focused problem, we explored several ideas in an ideation workshop using brainstorming and sketching. In an group discussion, we converged on an idea for further prototyping that was to be implemented in code. We chose an idea that was 1) grounded in empirical data and 2) realistically could be implemented in code within project time restrictions. A high fidelity prototype was then coded and tested on a potential user from ITU. Each method is explained in more depth in the following sections.

![Our instance of the Double Diamond process model.](./figures/double_diamond.pdf){#fig:double_diamond width=80%}

## Interviews {#sec:interviews}

As part of the empirical gathering, we interviewed Torben, the Founder and CEO of Chainge, to get an understanding of the business in general and the onboarding process. The interview was informal and involved an introduction to the facilities at the headquarters and the electric cargo bikes. To remember the context of the headquarters we took a series of pictures (see [@fig:chainge_headquarters]). Due to the nature of the interview, we had not created an interview guide. The interview was informative and provided a better understanding of the Chainge and its strategy. The session with Torben also had a positive impact on our collaboration due to the informal talk in-between case related subjects. The interview supported us in clarifying and guiding us towards the next step in the process.

::: {#fig:chainge_headquarters}
![](./figures/chainge_image1.jpeg){width=32%}\hfill
![](./figures/chainge_image2.jpeg){width=32%}\hfill
![](./figures/chainge_image3.jpeg){width=32%}

![](./figures/chainge_image4.jpeg){width=32%}\hfill
![](./figures/chainge_image5.jpeg){width=32%}\hfill
![](./figures/chainge_image6.jpeg){width=32%}

Pictures taken at the Headquarters of Chainge
:::

We wanted to interview Drivers working at Chainge to learn more about their work tasks and the onboarding process. Torben from Chainge assisted in arranging interviews with newly hired Drivers a week later. We wanted to interview Drivers that had recently experienced the onboarding process or were in the middle of the onboarding. We conducted three interviews with new Drivers that had worked at Chainge for less than four weeks. The three Drivers had worked at Chainge for one week, two weeks and three weeks respectively.

The interviews were conducted at Chainge’s headquarters to make it convenient for the interviewees. Prior to the interviews, we created an interview guide to structure and facilitate the interviews. This guide was semi-structured, which is more flexible for structured interviews but not as loosely structured as unstructured interviews [@bryman2016social]. The interview guide provided flexibility for questions that suddenly arose but at the same time managed the interview in a way so we did not deviate from the planned questions.

## Colour Coding of Data {#sec:colour_coding}

Numerous frameworks and tools exist for grouping interview data into categories. We chose an accessible and visual methodological approach of highlighting words and sentences with colours, each colour corresponding to a category in our coding format [@tbl:colourtable]. The purpose of this process is to familiarize ourselves with the gathered material.

| colour | Definition                                     |
| ------ | ---------------------------------------------- |
| Green  | Positive aspects of the Drivers' job           |
| Yellow | General knowledge about work practices         |
| Red    | Challenges/insecurities experienced by the Drivers |

: Colour Coding Table {#tbl:colourtable}

## Participant Observation {#sec:participant_obs}

As part of our empirical gathering, we have conducted participant observation. Spradley [-@spradley1980observation] has categorised different degrees of participant observation. We utilised the type of participation classified as passive participation. 

The person being observed was one of the interview respondents that was also a newly hired Driver. This observation was arranged during our interview with the Driver. The Driver agreed to be observed while driving a delivery route for Chainge. The Driver was followed on bikes by two of the students from the group and was observed while performing his work tasks, see [@fig:chainge_driver]. The students drove after the Driver so they were present at the scene but they did not participate in performing the work tasks. We decided to pursue participant observation with the aim of exploring tacit knowledge about the work tasks that were not vocalised during the interview.

During participatory observation at the headquarters, we made an interesting observation. We observed a manager at Chainge explaining to three new Drivers how to pack a cargo bike for a certain client [@fig:chainge_driver]. The manager was also responsible for picking up the phone if the Drivers were out delivering packages and needed assistance with situations related to delivering. The manager’s phone rang while he explained the process to the new Drivers.

Additionally, we took pictures and videos of the process, as they could be useful later on.

::: {#fig:chainge_driver}
![](./figures/driver_image1.jpeg){width=49%}\hfill
![](./figures/driver_image2.jpeg){width=49%}

Pictures showing the trailer and checklist used by Drivers.
:::

## Ideation Workshop {#sec:ideation_workshop}

Grounded in the themes identified through our category-coded interview data, we conducted an internal ideation workshop with brainstorming as the main focus, wherein we explored the design openings and potential solutions. Our approach was to ignore the technological possibilities in situ, as well as any constraints, leveraging a user-centric approach instead. In this process, we emphasised the benefits a solution would have on Chainge's employees, based on the problems they vocalised in our interviews (see [@sec:app_interviews]).

Kolko [-@kolko2018designthinking] describes how brainstorming emerged as a playful and creative way of problem-solving. Kolko's [-@kolko2018designthinking] four principles that are relevant in a brainstorming session are: to avoid criticisms, encourage crazy ideas, produce a variety of ideas and utilise the ideas from the team members to build upon to extend ideas. According to Kolko [-@kolko2018designthinking], empathy is the foundation of participatory design practice.

We brainstormed themes on a whiteboard (see [@fig:brainstorm]) to figure out what should characterise the solution. Afterwards, we individually marked three words each that we found the most important. It became evident through this process that the central theme of our solution should be the existence and contextual accessibility of structured, standardised information on work practices and responsibilities for Chainge drivers. We strived to be empathic in the brainstorming within the group to be open-minded and explorative when being presented with ideas. Based on this brainstorm we developed sketches of how we envisioned the prototype (see [@fig:sketching]).

::: {#fig:brainstorm}
![](./figures/brainstorm_image1.jpg){width=32%}\hfill
![](./figures/brainstorm_image2.jpg){width=32%}\hfill
![](./figures/brainstorm_image3.jpg){width=32%}

Whiteboard brainstorming
:::

::: {#fig:sketching}
![](./figures/sketching_image1.jpg){width=49%}\hfill
![](./figures/sketching_image2.jpg){width=49%}\hfill
![](./figures/sketching_image3.jpg){width=49%}\hfill
![](./figures/sketching_image4.pdf){width=49%}

Ideation sketching
:::

Reflecting on our sketching process led to us discussing potential sources of inspiration. One of our sketches illustrated an e-learning platform, and it reminded us of Apple's Developer application (see [@fig:developer]), which consists of a list of links leading to pages containing a video, description and resources with references. We sampled this for the development of our prototype, as it shares our design goal of knowledge sharing and standardised learning.

::: {#fig:developer}
![](./figures/developer_image1.png){width=24%}\hfill
![](./figures/developer_image2.png){width=24%}\hfill
![](./figures/developer_image3.png){width=24%}\hfill
![](./figures/developer_image4.png){width=24%}

Apple's Developer application
:::

## Prototyping {#sec:prototyping}

Our prototyping process began with a discussion of which elements of the design should be emphasised or de-emphasised. Because our prototype was a small component in the larger context of a platform, the operational medium had to be perceivable as one small component of a larger collective.

Bucheanau and Suri [-@buchenau2000prototyping] raise the notion that a prototype is any medium produced to communicate or explore ideas. Our goal was to not only communicate amongst ourselves a representation of our collective ideas, but to also communicate to and explore it with potential end-users.

Lim, Stolterman and Tenenberg [-@lim2008anatomy] argue that prototypes manifest in three dimensions: medium, resolution and scope. Our prototype reflects these dimensions by being consciously shaped as a digital platform, with a high degree of fidelity, and a scope fixed to the learning component. Based on our sketching we developed a more concrete mockup (see [@fig:mockup]). We then implemented a high-fidelity prototype in code based on our mockup (see [@sec:solution]). The prototype itself was developed in an iterative fashion. The CS student would code a version of the prototype, receive feedback from the group members, and incoorporate that feedback in the coding and then present this new version of the prototype for new feedback. We did this instead of everybody coding, as it was infeasible for everybody to optain the required skill of coding within the short timeframe, however everybody was still included in the coding process.

![Mockup of solution](./figures/mockup.pdf){#fig:mockup width=75%}

## Evaluation {#sec:evaluation}

We decided to test the prototype with an individual that does not work at Chainge. A technical description of the prototype is outlined in [@sec:technical_impl]. The target group of the prototype is new Drivers, therefore we did not find it relevant to test it on existing employees as they are potentially biased from their experience working at Chainge. We tested the platform with an individual studying at ITU. The test was mostly concerned with a proof of concept and to identify potential pain points. We wanted to explore if the prototype was easy to navigate. Additionally, we wanted to show the video on the platform to get information regarding if it showcases the different work tasks that a Driver can be presented with.