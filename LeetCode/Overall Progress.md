---
solutions:
  - date: 05/01/2025
    problem: "[[Maximum Subarray]]"
    topics: "[[DP]]"
    level: Easy
    solved: 2
  - date: 05/01/2025
    problem: "[[Climbing Stairs]]"
    topics: "[[DP]]"
    level: Easy
    solved: 3
  - date: 14/01/2025
    problem: "[[Divisor Game]]"
    topics: "[[DP]]"
    level: Easy
    solved: 1
  - date: 24/02/2025
    problem: "[[133. Clone Graph]]"
    topics: "[[DFS]]"
    level: Medium
    solved: 1
  - date: 26/02/2025
    problem: "[[934. Shortest Bridge]]"
    topics: "[[DFS]]"
    level: Medium
    solved: 1
  - date: 27/02/2025
    problem: "[[130. Surrounded Regions]]"
    topics: "[[DFS]]"
    level: Medium
    solved: 1
  - date: 28/02/2025
    problem: "[[797. All Paths From Source to Target]]"
    topics: "[[DFS]]"
    level: Medium
    solved: 1
  - date: 01/03/2025
    problem: "[[543. Diameter of Binary Tree]]"
    topics: "[[Tree]]"
    level: Easy
    solved: 2
  - date: 01/03/2025
    problem: "[[1448. Count Good Nodes in Binary Tree]]"
    topics: "[[Tree]]"
    level: Medium
    solved: 2
  - date: 02/03/2025
    problem: "[[863. All Nodes Distance K in Binary Tree]]"
    topics: "[[Tree]]"
    level: Medium
    solved: 1
---

```dataview
table sol.date as "Date", sol.problem as "Problem", sol.topics as "Topics", sol.level as "Level", sol.solved as "No. of times Solved"
from "LeetCode/Overall Progress"
flatten solutions as sol
sort sol.date desc
```




```dataviewjs
dv.span("** Leetcode Streak View**");

// Function to convert dd/mm/yyyy to YYYY-MM-DD
function convertDate(dateStr) {
  let [day, month, year] = dateStr.split("/");
  return `${year}-${month.padStart(2, '0')}-${day.padStart(2, '0')}`;
}

const calendarData = {
  year: 2025,  // Adjust to match your data year
  colors: {    
    blue:        ["#8cb9ff", "#69a3ff", "#428bff", "#1872ff", "#0058e2"],
    green:       ["#c6e48b", "#7bc96f", "#49af5d", "#2e8840", "#196127"],
    red:         ["#ff9e82", "#ff7b55", "#ff4d1a", "#e73400", "#bd2a00"],
    orange:      ["#ffa244", "#fd7f00", "#dd6f00", "#bf6000", "#9b4e00"],
    pink:        ["#ff96cb", "#ff70b8", "#ff3a9d", "#ee0077", "#c30062"],
    orangeToRed: ["#ffdf04", "#ffbe04", "#ff9a03", "#ff6d02", "#ff2c01"]
  },
  showCurrentDayBorder: true, 
  defaultEntryIntensity: 4,   
  intensityScaleStart: 10,    
  intensityScaleEnd: 100,     
  entries: []                
};

// Pull the "solutions" array from the "OverallProgress_data" note
const solutions = dv.page("Overall Progress").solutions;
for (let sol of solutions) {
  calendarData.entries.push({
    date: convertDate(sol.date),  // converts "dd/mm/yyyy" to "YYYY-MM-DD"
    intensity: sol.solved,          // use the "No. of times Solved" as the intensity
    //content: "🏋️",                // change the emoji/icon as desired
    color: "orange",              // choose a color from calendarData.colors (or leave it to default)
  });
}

// Render the heatmap calendar in your note
renderHeatmapCalendar(this.container, calendarData);

```



