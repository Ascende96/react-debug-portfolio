# 🐞 Dynamic Component Rendering via `.map()` Broke Logic

## 🏢 Internship – Website Builder Project

### ❌ Problem
The site was meant to dynamically show only the components (sections) that the user filled out.

Initially, the team used `.map()` to loop through a list of sections and render components accordingly.  
They also tried using `useEffect` logic **inside that `.map()` loop**, which caused it to silently fail.

### 🚨 Core Issue
React hooks like `useEffect` **must not be used inside loops, conditions, or nested functions**.  
The dynamic map structure caused **state/logic breakdown**, especially during updates or re-renders.
