# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 4: Client Project

### Overview

We've organized for you to complete a client project. This is a great opportunity for you to be exposed to a **real** organization doing **real work** with **real data**.

[New Light Technologies](https://www.newlight.com/) is an organization founded in 2003. After over a decade of research, New Light developed a carbon capture technology able to produce high-performance bioplastics from carbon emissions.  Their mission is to replace oil-based plastics with greenhouse gas-based bioplastics on a global scale, moving oil out of the world’s products, reducing material production costs, and reducing the amount of carbon in the air on a market-driven basis. They also do contracting work with various organizations, including FEMA (the Federal Emergency Management Agency), the U.S. Census Bureau, and The World Bank.

Ran Goldblatt, our contact with NLT, is a remote sensing scientist and senior consultant. He has a strong background in geographic information systems (GIS) and leverages this knowledge when solving problems facing various agencies.

**Problem**:

NLT requested that our students complete projects surrounding emergency preparedness and economic analysis. In short summary, the twelve projects you may complete are:

1. Leveraging Social Media to Map Disasters.
2. Leveraging News and Media for Situational Awareness.
3. Optimizing Evacuation Routes using Real-Time Traffic Information.
4. Extracting Building Values from Zillow.
5. Utilizing Social Media for a rapid alert about new disasters.
6. Using Google Street View to retrieve (pre-event) photos of structures.
7. Utilizing Yelp cost estimates ($, $$, $$$) for estimating neighborhood affluence.
8. Utilizing Yelp data to estimate the number of businesses in a given locality and categorize them by lifeline.
9. Using news outlets and/or social media to identify areas/neighborhoods with power outages.
10. Using live police radio reports for real time identification of people needing assistance.
11. Using Indeed or Glassdoor platforms together with number and type of affected businesses to estimate the expected economic loss (wages) due to a disaster.
12. Using drone data to estimate rooftop quality and material classification.

That's where you come in.

For the next four weeks, our class will tackle various projects related to emergency preparedness and economic analysis. On **Friday, January 18**, we'll present our findings and deliver:
1. A clean GitHub repo containing our reproducible results and analysis.
2. A real-world demonstration of the product.
3. Any documentation for running the code.

> This is an exciting opportunity to identify and solve a problem relevant to the real world problems. Using your data science skills in this practical, _pro bono_ capacity reflects well on you and gives you a great story as you embark on interviews! (The fact that we'll be using open data also gives you free reign to publicly publish your findings and to freely discuss this in interviews.)

### Problem Summaries

**Problem 1: Leveraging Social Media to Map Disasters**

*Problem Statement:*
- When responding to disasters (e.g. damage and casualties caused by hurricanes,
tornadoes, floods, fires etc.), it is critical to map and identify locations of survivors
needing assistance.
- Currently, satellite and aerial imagery, ground surveys and modeled hazard data are the primary tools used to assess damage and to identify areas where survivors may need assistance.
- Often, survivors will resort to using social media to call for help or share information about their location and the current situation. In many cases they will also include useful images showing water levels, amount of damage etc. which could indicate on the intensity of the disaster.
- This information can be leveraged to track the event in real-time. Social media can help identify isolated communities at risk, locations of survivors and areas where assistance teams should be sent for search and rescue, levels of damage, help map depths of flooding, identify where additional imagery/information needs to be collected and plan when and where resources should be allocated.
- This project will discover new ways to leverage social media (including from Twitter, Facebook, Instagram, Snapchat, or others) to supplement current tools and methodologies used when responding to disasters.
- The tools developed in this project will also help leverage social media to locate hot spots of where people are needing assistance, using, for example, geolocated posts/tweets containing keywords such as “flood”, “fire”, “damage”, “destroyed” or anything else that could be related to the specific disaster event, including searching for images tagged with  relevant keywords. A main challenge will be, of course, removing irrelevant information that may happen to contain similar keywords.

*Desired Deliverables:*
- A short write-up describing the project.
- Open source code to allow for implementation of this big data search process during a
disaster.
- The code should be flexible enough and allow the end user to change certain keywords
which would correspond to different disaster types, e.g.: “flood”, “water”, “depth”, for a
flood event and “burn”, “fire”, “smoke” for a wildfire event. Possible disaster events
include floods, fires, hurricanes, earthquakes, tornadoes, tsunamis and volcanoes.
- Output of this code should be a geolocated dataset (a GIS shapefile or json with lat/long
reference, or a KML file) with relevant information acquired from the tweet as attribution
- A preliminary proof of concept using a real-world example.

*Descriptions of data used as input:*

- Geo-referenced disaster-specific social media posts (with or without images).


**Problem 2: Leveraging News and Media for Situational Awareness**

*Problem Statement:*
- During a major disaster, it is essential to provide the public and responders with relevant local news updates in order to gain situational awareness during the event.
- During a disaster, news updates are coming from tens to hundreds of different sources, all in different formats, available from different websites, news channels etc., and it is often difficult to find what would be most helpful amid the chaos of other non-disaster related news and media.
- There is currently no forum for rounding up and archiving relevant news for a live disaster event.
- This project will leverage news feeds relevant to specific disasters, gathered from multiple sources, to create a webpage that presents these live feeds under one umbrella (on one page). This is similar to the Google News feature.

*Desired Deliverables:*
- A short write-up describing the project.
- An open source code that allows to create a disaster-specific webpage, which “pulls” relevant news articles relevant to a specific event. The code should only pull the title of the article/post, an abstract/summary (if available) and an image/ thumbnail (if available) and include a link to the original source.
- An example (proof of concept) of a disaster event-specific web page which is populated by a real-time feed of relevant news articles, journals, blog posts, videos, etc. pertaining to a live event such as “Hurricane Lane”, or “Hurricane Harvey”, etc.

- A user accessing this web page should have the ability to filter the search query by date, media type and certain keywords such as “evacuation”, “fire”, “damage assessment”,
name of a city, etc.
- The tool should also allow the website editor to set these keywords and search queries (i.e. the page will always show the relevant news feeds set by the editor/admin).
- This web page can be integrated with other methods to provide situational awareness to the disaster response community such as being featured on a disaster response website with relevant disaster data.
- Map files, toolboxes, data and any other supporting files are needed as deliverables to test and run the code.

*Descriptions of input data:*
- News articles, journals, blog posts, videos from external media websites
- Online forms of relevant disaster media



**Problem 3: Optimizing Evacuation Routes using Real-Time Traffic Information**

*Problem Statement:*
- During disasters, search and rescue teams must be able to search for and get to survivors as fast as possible (in terms of travel time and distance)
- Current GIS and navigation systems allow responders to calculate travel time and
distance between origin and destination and propose an optimal route to the destination.
- However, many of the current platforms do not rely on real-time data (e.g. road closures, damaged roads etc.) and can produce inaccurate or inefficient results.
- This project will leverage social media, news feeds and other datasets (e.g. Waze, Here.com) to identify real time road closures or damaged roads, power outages and other blocked routes that may affect traffic lights, travel time, travel safety and more.
- The system should allow the user (the public or rescue teams) to search for any of these conditions and identify if and where they exist in a specific location (street, neighborhood, city etc.)

*Desired Deliverables:*
- A short write-up describing the project.
- An open source code that pulls live information from social media and/or news feeds about road closures, road conditions, damaged roads, power outages etc. which may
affect travel and accessibility.
- The output can be either tabular (e.g. allow for search of names of closed roads) or geospatial (e.g. produce a map of real-time road closures).



**Problem 4: Extracting Building Values from Zillow**

*Problem Statement:*
- During a disaster, it is important to model and estimate the potential or forecasted effect of the event, including the projected/forecasted damage.
- Existing indicators of forecasted damage include number of structures within the affected area, number of people in the area, number of households, demographics of the impacted population, etc.
- This project will add an additional indicator: the value of the properties in the affected area. Property values can be estimated according to the market price of houses.
- In this project, the students will leverage property market prices published in different real-estate websites (e.g. Zillow), according to zip codes.
- The tool will allow the user to automatically search for the mean, median, min, max and average value of the properties in each zip code area.
- The objective is not to download the database from these sources. Rather, it should allow the user to feed the code with a list of affected areas (zip codes) as input, and retrieve the current (or historical, annual, monthly, quarterly) property values.

*Desired Deliverables:*
- A short write-up describing the project.
- An open source code (or a simple API) which takes, as input, a list of zip codes, and outputs the mean, median, min and max property values in these areas

*Descriptions of input data: Real-estate website*
- Zillow
- Trulia
- Realtor.com

**Requirements**:
For the purposes of a DSI project, you must meet a few technical requirements. They are:
1)  A `README.md` file in your project repo. Note that `README` files are automatically rendered by GitHub when you view a repo. Your README should contain:
    - A problem statement.
    - A succinct formulation of the question your analysis seeks to answer.
    - A table of contents, which should indicate which notebook or scripts a stakeholder should start with, and a link to an **executive summary**.
    - A paragraph description of the data you used, plus your data acquisition, ingestion, and cleaning steps.
    - A short description of software requirements (e.g., `Pandas`, `Scikit-learn`) required by your analysis.

2) Your notebook(s) should be **reproducible** and **error-free**. This means:
    - You should set a random seed at the start of every notebook, using `np.random.seed(...)`. This will ensure that the random numbers generated in your notebook will be the same every time.
    - You need to provide a _relative path_ to your data, so that if I clone your repo to my machine I can run everything in your repo without error. (You also provide links to any publicly accessible data.)
    - I should be able to `Restart & Run All` in your notebook(s) and see that the _exact same_ results are reproduced.
    - To check that everything worked properly, you may consider forking your own repo to a different location on your computer and checking that all notebooks can run properly from top to bottom.

3) You may build _either_ a supervised learning model _or_ conduct an unsupervised learning analysis. Bear in mind that the value you provide to New Light Technologies may come from data ingestion, data cleaning, EDA, and/ or a dashboard, etc. While a model may not be immediately apparent, be creative. *Without us telling you exactly what model to build, how could you build a model to increase performance or generate better insights when answering the problem you are facing?*

**Deadline**: January 18th, 2019.

**Questions**: Questions should be sent to your local instructor; questions that need to go to the client should be directed to Matt Brems via email (matt.brems@ga.co). Questions should be specific, brief, and formatted so that they can be directly sent to our contacts at NLT.
> This is a good practice to develop! When contacting a boss or a client, you should make your question as easy as possible to answer. Consider the following two examples:

> Example 1: "Hey, I have a question. I'm writing a blog post about TensorFlow but got stuck. This part was confusing: https://www.tensorflow.org/api_docs/python/tf/tanh Can you help?"

> Example 2: "The TensorFlow tanh documentation says 'Computes hyperbolic tangent of x element-wise.' What does hyperbolic tangent mean? The link to see more is: https://www.tensorflow.org/api_docs/python/tf/tanh"

> The first example spends about 20 words before mentioning what is going on. The question "Can you help?" is unspecific. The boss/client is required to go to a link in order to get any information about the problem.

> The second example quickly calls out 'Tensorflow tanh documentation,' the explicit quote that is confusing, the explicit question being asked, and a link for additional context. Both examples attempt to get the boss/client/whomever to explain hyperbolic tangent, but imagine how much more quickly someone could answer the second query than the first.

> A helpful way to consider this: When you ask a question, you are basically asking for a favor. You're asking a person to give their time, their brainpower, and their knowledge to you. Every time you ask them to hunt around for more (i.e. they have to travel to a link to get more information or they struggle to understand the question you're asking), you're asking a bigger and bigger favor from them.

---

### Teams

Your local instructor will divide your class into teams. Chat with them to find out!

---

### Consulting Project Feedback + Evaluation

Data science is a field in which we apply data to solve real-world problems. Therefore, projects and presentations are means by which we can assess your ability to solve real-world problems in a data-driven manner.

When evaluating projects, there are four areas on which your instructors focus.
1. **Project Requirements: Did you meet all project requirements?** In answering this question, your instructors want to assess how well you met the project requirements as established. These will generally be laid out in the project readme.

2. **Audience: Is your presentation appropriate for the stakeholder?** In answering this question, your instructors want to assess how well you present your results to stakeholders. For example:
  - Did you frame the problem appropriately for the audience?
  - Did you use the appropriate level of technical language for your audience?
  - Did you effectively use your time, or did you encounter an issue such as going significantly beyond or under the allotted time or rushing to conclude the presentation in the allotted time?
  - Did you present effectively, or were there things that detract from the overall presentation such as not speaking loudly enough for the audience or repeating oneself?

3. **Methods: Are your methods appropriate for solving the problem?** In answering this question, your instructors want to assess how well you have applied data science methodology to the problem at hand. For example:
  - Did you make well-reasoned modeling choices, or is there clear evidence that the model is inadequate or improper?
  - Are you able to clearly defend your methodological decisions and results?
  - Did you generalize your results properly, or were your conclusions/inferences improper or fallacious?

4. **Value: Have you provided value to the stakeholder through clear, data-driven recommendations?** In answering this question, your instructors want to assess the value you provide to the stakeholder as a data scientist. For example:
  - Did you answer the problem posed to you?
  - Did you make your recommendations clear, or were the recommendations unclear?
  - Were your recommendations data-driven and based on the results of your work?

You will earn a score for each of the four areas mentioned above.
1. Project Requirements: You may earn a score of 0 or 1. You will earn a score of 1 if all project requirements are met. Otherwise, you will earn a score of 0.
2. Audience: You may earn a score between 0 and 3. A score of 0 indicates that your presentation is inappropriate for the stakeholder. A score of 1 indicates that at least part of your presentation should be non-trivially reworked to be more appropriate for the stakeholder. A score of 2 indicates that there are few to no areas of your presentation that should be reworked. A score of 3 indicates that your presentation is consistently appropriate for the stakeholder and serves as a model for future presentations.
3. Methods: You may earn a score between 0 and 3. A score of 0 indicates that your methods are inappropriate. A score of 1 indicates that your methods are somewhat inappropriate, that justification for methodological decisions is lacking, and/or that your conclusions do not follow from the methods. A score of 2 indicates that your methods are appropriate, justification is sufficient/strong, and your conclusions follow well from the methods. A score of 3 indicates that your methods are excellent, strongly defended, and serves model for future presentations.
4. Value: You may earn a score between 0 and 3. A score of 0 indicates that you provide little to no value to the stakeholder. A score of 1 indicates that the value you provide to the stakeholder is substantially less than expected by not answering the problem, not providing clear recommendations to the stakeholder, and/or providing recommendations that were not data-driven. A score of 2 indicates that the value you provide to the stakeholder is on par with the expectation of providing clear, data-driven recommendations that directly answer the problem posed. A score of 3 indicates that the value you provide to the stakeholder is beyond what is expected and serves as a model for future presentations.

Your final grade will be calculated as follows:
- If any project requirement is not met, the final grade is 'Fail' with a score of 0.
- If all project requirements are met, then the final grade is 'Pass' with a score calculated by summing the above scores. Therefore, if all project requirements are met, the final score will be between a 1 and 10.
