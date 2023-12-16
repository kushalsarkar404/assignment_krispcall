# Assignment For KrispCall
*This file contains the submission for the assignment of KrispCall. This is maintained by Kushal SARKAR.*
## Task 1: Mixpanel Implementation
Since I am asked not to include initialization code and just to provide the snippet to track clicks on the “Get Started” button, the following is a JavaScript to track clicks assuming that the “Get Started” button has an ID of `getStartedButton`:
```
const getPagePath = () =>{
  return window.location.pathname;
}

const trackGetStartedBtn = () =>{
  const pagePath = getPagePath();

  mixpanel.track("Get Started Button Clicked", {
    "Page Path": pagePath
    });
}

document.querySelector(".getStartedButton").addEventListener("click", () => {
  trackGetStartedBtn();
});

```
## Task 2: Data Cleanup
The provided dataset `sampledata.csv` is cleaned up using Python. The code is written [here](task2_DataCleanup.ipynb) on Google Colab.

<br>

## Task 3: Data Analysis and Visualization - Free Form
The cleaned dataset `cleaneddataset.csv` is visualized using Python. The visualization can be seen [here](task3_DataAnalysisAndVisualization.ipynb) on Google Colab.

<br>

>[!Note]
>I took roughly 45 minutes, a bit more time than the suggested 30 minutes, to ensure a thorough and comprehensive analysis of the data.


<br>


## Task 4: Competitor Analysis
**Competitors, IN MY OPINION:**

> While KrispCall has comparisons on its official site, I'm sharing my view as someone new to business cloud telephony. I'm looking at why people might choose other services. This is just a simple look at what might influence someone picking a different option for the first time.

<br>

**1. Twilio**

![image](https://github.com/kushalsarkar404/assignment_krispcall/assets/126848593/18300fb3-0e2c-4be3-9c92-e56196e2beb9)

Twilio is a cloud communications platform that offers a variety of services like KrispCall, including virtual phone numbers, voice, and messaging solutions. Twilio also offers a range of communication APIs and services, allowing businesses to integrate voice, messaging, and video capabilities into their applications. They are widely known as they have been recognized as a Leader in the 2023 Gartner Magic Quadrant for CPaaS, Twilio stands out for its completeness of vision and successful execution in the Communications Platform as a Service space. Therefore, their market reach could be relatively easier.

<br>

**2. RingCentral**

![image](https://github.com/kushalsarkar404/assignment_krispcall/assets/126848593/53af0e2e-7dc8-4435-8bb5-507f8342efb1)

Similarly, RingCentral also provides cloud-based communication and collaboration solutions, including virtual phone numbers and unified communications. RingCentral positions itself as a reliable provider of core phone systems with a variety of plans, including essential, advanced, and ultra options. It stands out for its budget-friendly pricing and consistent recognition as a Magic Quadrant Leader for UCaaS by Gartner.
