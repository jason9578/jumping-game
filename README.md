[Readme.md](https://github.com/user-attachments/files/26867315/Readme.md)
# Jump Game

## Graphical Abstract
![Project Graphical Abstract](abstract.PNG)

## Software Purpose

### Development Process Selection

The **Agile development process** is adopted, and the reasons for selection are as follows:

1. As a lightweight web game, the project has flexible requirements and a short iteration cycle, which is compatible with the rapid iteration feature of Agile development;

2. Agile development does not require complex phase approval, and can quickly adjust functions according to test feedback;

3. The core functions and optimization points can be split into small iterative tasks, which are gradually improved to reduce development risks\.

### Target Usage Scenarios/Market

- Core Scenario: Web\-based casual entertainment\. Users can play directly in the browser without installing any plug\-ins by clicking the mouse;

- Target Users: Casual game players of all ages, especially those who need short\-term entertainment in fragmented time \(such as commuting and breaks\);

- Market Positioning: A lightweight free web game with no commercial appeal, focusing on a simple and easy\-to\-use casual experience\.

## Development Plan

### 1\. Development Process

```Plain Text
Requirement Analysis → Rapid Prototype Design → Functional Development → Local Testing → Experience Iteration → Function Finalization
```

- Requirement Analysis: Clarify core requirements such as core gameplay \(jump to avoid obstacles\), score recording, and local storage of the highest score;

- Prototype Design: Quickly build page structure and basic interaction logic;

- Functional Development: Implement modules separately \(player physical jump, obstacle generation, collision detection, score system, etc\.\);

- Testing/Iteration: Verify the stability of core logic and adjust parameters \(such as jump force, obstacle generation frequency\) to optimize the experience;

- Finalization: Organize code and complete the runnable version\.

### 2\. Development Team Division of Labor

|Role|Responsibilities|Division of Labor Ratio|
|---|---|---|
|Hu YiXuan<br>|Write core code \+ GitHub repository management \+ Provide design ideas related to game core gameplay and algorithms|40%|
|Liang YiHan|Write README\.md \+ Fill in all tables \+ Provide design ideas related to game content presentation and experience optimization|30%|
|Wang YiMeng|Screen recording \+ Video editing \+ Final submission check \+ Provide design ideas related to game visual presentation and demonstration effects|30%|

### 3\. Schedule

|Phase|Duration|Core Output|
|---|---|---|
|Requirement Analysis|1 Day|Determine core gameplay and function list|
|Prototype Design|1 Day|Page structure and style draft|
|Core Function Development|1 Days|Jump physics, collision detection, score system|
|Testing and Optimization|1 Day|Fix logical vulnerabilities and optimize parameter experience|
|Final Launch|1 Day|Organize code and complete the runnable version|

### 4\. Core Algorithms

- **Physical Jump Algorithm**: A velocity superposition model based on gravitational acceleration\. Gravity is simulated by `ySpeed \+= gravity`, and the initial jump velocity is controlled by `jumpPower`;

- **Collision Detection Algorithm**: Axis\-Aligned Bounding Box \(AABB\) algorithm to determine whether the rectangular boundaries of the player and obstacles overlap;

- **Obstacle Generation Algorithm**: The generation interval is controlled by random numbers \(`50 \+ Math\.random\(\) \* 60`\) to ensure the randomness of obstacle appearance frequency;

- **Score Calculation Algorithm**: The score is accumulated frame by frame during the game, and the highest score in local storage is updated after the collision ends\.

### 5\. Current Status

✅ Core functions completed:

- Physical interaction of player jump triggered by left mouse button;

- Randomly generate moving obstacles to realize the core gameplay of obstacle avoidance;

- Collision detection triggers game over and locally stores the highest score;

- Restart button resets the game state;

- Real\-time score and highest score display\.

### 6\. Future Planning

1. Interaction Optimization: Add keyboard \(space/up arrow\) jump support and adapt to mobile touch operations;

2. Experience Enhancement: Add jump/collision sound effects, background music, and increase player/obstacle skin styles;

3. Difficulty Stratification: Increase obstacle movement speed and reduce generation interval as the score increases;

4. Function Expansion: Add online ranking list \(connect to lightweight backend\), level mode, and item system \(such as invincibility, deceleration\);

5. Performance Optimization: Optimize canvas rendering efficiency and adapt to different resolution screens\.

## Demo Video

https://youtu.be/mgNArpI9BMk

## Running Environment

### 1\. Programming Languages

- HTML5 \(Page Structure\)

- CSS3 \(Style and Layout\)

- JavaScript \(Game Logic, Interaction Control\)

### 2\. Minimum Hardware and Software Requirements

- Browser: Chrome 80\+ / Firefox 75\+ / Safari 13\+ / Edge 80\+ \(supports HTML5 Canvas\);

- Hardware: CPU above 1\.0GHz, memory above 512MB, no special graphics card requirements;

- Network: No network required \(run directly by opening the HTML file locally\);

- System: Windows/macOS/Linux/Android/iOS \(all systems supporting the above browsers are available\)\.

### 3\. Dependencies

No third\-party dependencies\. It is implemented based on native HTML5/CSS3/JavaScript, and no additional dependencies need to be installed\.

## Declaration

All codes, styles, and interaction logic of this project are independently developed, and no non\-self\-developed open\-source resources, third\-party libraries, or commercial plug\-ins are used\.
<img width="829" height="478" alt="eac0ddce1834aaf1d8eb6bc25aa3b2a3" src="https://github.com/user-attachments/assets/828bd979-7ab4-4369-93c8-2ba32f2f3059" />


