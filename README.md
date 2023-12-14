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

