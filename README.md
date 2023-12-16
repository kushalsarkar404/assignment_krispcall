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

## Task 3: Data Analysis and Visualization - Free Form
The cleaned dataset `cleaneddataset.csv` is visualized using Python. The visualization can be seen here [here](task3_DataAnalysisAndVisualization.ipynb) on Google Colab.
`PS: I took roughly 45 minutes, a bit more time than the suggested 30 minutes, to ensure a thorough and comprehensive analysis of the data.`

