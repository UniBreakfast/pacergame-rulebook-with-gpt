# [pacergame-rulebook-with-gpt](https://github.com/UniBreakfast/pacergame-rulebook-with-gpt)

## **PacerGame Rulebook**

### **1. Introduction**

Welcome to **PacerGame**, a gamified self-improvement system designed to help you achieve your goals through structured tasks and rewards. By engaging in meaningful activities aligned with your personal endeavors, you earn Confidence Points (CP) that fuel your progress and unlock new challenges.

### **2. Key Terms and Definitions**

- **Endeavors (ES):** Directions of interest such as wishes, goals, dreams, needs, skills to develop, or habits to build or break. They represent the overarching areas you want to focus on.

- **Activities (AS):**

  - **Creation:** Players add activities as they see fit at any point in time, with no restrictions on the number or type. Activities can remain in a list until the player decides to undertake them in a quest.

  - **Measurement Units:** The amount of activity is determined by the player upon creation, using any suitable units (e.g., times, minutes, reps, sets, pages, meters, liters).

- **Quests (QS):**

  - **Initiation:** Players decide the desired duration of a quest in days, limited only by their available Confidence Points (CP).

  - **Association with Activities:** A quest is undertaken by selecting an activity from the player's list. The quest then sets a daily requirement (todo) based on the activity's parameters.

  - **Pledge:** To undertake a quest, players pledge CP equal to the quest's cost.

  - **Failure:** If a todo of a quest is not completed on any day, the quest fails, and the pledged CP is lost.

- **Todos (TS):**

  - **Definition:** The individual daily tasks within a quest. Each todo represents one day's commitment to perform the activity's required amount.

  - **Completion:** Marked by a daily checkmark when the activity's required amount is completed.

- **Confidence Points (CP):**

  - **Initial CP:** Determined subjectively by the player's self-assessed confidence level on a scale from 1 to 10.

  - **Earning CP:** Players earn CP by completing todos and successfully completing quests.

  - **Spending CP:** CP is spent when pledging for new quests.

- **Difficulty:**

  - **Assignment:** Activity difficulty is subjectively decided by the player upon creation, on a scale from 1 to 10.

- **Inertia:**

  - **Definition:** After completing a quest, players can continue performing the activity daily without pledging more CP, maintaining their streak.

  - **Rewards:** The CP reward per todo remains the same during inertia, neither increasing nor decreasing.

### **3. Game Mechanics**

#### **3.1 Activities**

- **Creation and Management:**

  - Players can create activities that align with their endeavors at any time.

  - Activities can remain inactive in a list until the player is ready to undertake them in a quest.

- **Measurement and Units:**

  - Activities are quantified using units appropriate to the task (e.g., minutes, pages, kilometers).

- **No Inherent Daily Requirements:**

  - Activities by themselves do not have daily requirements or obligations.

  - The daily requirement is established only when an activity is undertaken as part of a quest.

#### **3.2 Quests**

- **Starting a Quest:**

  - **Selection of Activity:** Players choose an activity from their list to form the basis of the quest.

  - **Duration:** Players choose the duration of a quest in days, based on their goals and available CP.

  - **Cost Calculation:** Quest Cost = Activity Difficulty × Quest Duration (in days).

  - **Pledging CP:** Players must pledge CP equal to the quest's cost to initiate it.

- **Todos:**

  - **Daily Commitment:** Each day of the quest requires the player to complete the todo, which involves performing the activity's required amount.

  - **Completion Verification:** Players honestly assess and confirm the completion of each day's todo.

- **Completing a Quest:**

  - **Daily Rewards:**

    - Each completed todo rewards CP calculated as the floor of the square root of the current consecutive day count within the quest. For example, on day 4 of a streak, the reward is floor(√4) = 2 CP.

  - **Quest Completion:**

    - Upon completing the quest, the player receives their pledged CP back, plus the CP earned from each todo.

- **Quest Failure:**

  - **Loss of Pledge:** If a player fails to complete a todo on any day, the quest fails, and the pledged CP is lost.

  - **Streak Reset:** The streak for that activity resets, and no further CP can be earned through inertia until a new quest is initiated.

#### **3.3 Confidence Points (CP)**

- **Initial CP:**

  - Players estimate their starting CP by assessing their confidence level from 1 to 10.

- **Earning CP:**

  - **Per Todo:** CP earned per completed todo is calculated as floor(√day_in_row).

  - **Quest Completion:** Successfully completing a quest returns the pledged CP to the player.

- **Spending CP:**

  - CP is spent when pledging for new quests, calculated based on the activity's difficulty and quest duration.

#### **3.4 Inertia**

- **Post-Quest Activity:**

  - After a quest is completed, players can continue performing the activity daily without pledging additional CP.

- **Maintaining the Streak:**

  - The streak continues as long as the player completes the daily todo.

  - Missing a day breaks the streak, ending the inertia phase.

- **Rewards During Inertia:**

  - The CP reward per todo remains constant, equal to the reward on the last day of the quest.

### **4. Example Scenario**

#### **Endeavor:** Improve Physical Fitness

- **Activity:** Run 2 kilometers.

  - **Difficulty:** Player sets difficulty at 3.

- **Quest:**

  - **Duration:** 5 days.

  - **Cost:** Difficulty (3) × Duration (5) = 15 CP.

  - **Pledge:** Player pledges 15 CP to start the quest.

- **Daily Todos and Rewards:**

  - **Todos:** Each day, the player must run 2 kilometers as per the quest's requirement.

  - **Day 1:** Complete run. Reward: floor(√1) = 1 CP.

  - **Day 2:** Complete run. Reward: floor(√2) = 1 CP.

  - **Day 3:** Complete run. Reward: floor(√3) = 1 CP.

  - **Day 4:** Complete run. Reward: floor(√4) = 2 CP.

  - **Day 5:** Complete run. Reward: floor(√5) = 2 CP.

- **Total CP Earned from Todos:** 7 CP.

- **Quest Completion:**

  - Player successfully completes the quest and gets back the pledged 15 CP.

  - **Total CP After Quest:** Initial CP - 15 (pledge) + 7 (todos) + 15 (returned pledge) = Initial CP + 7 CP.

- **Inertia Phase:**

  - **Continuation:** Player continues running 2 km daily without pledging more CP.

  - **Daily Reward:** CP reward remains at 2 CP per day (same as the reward on the last day of the quest).

  - **Streak Maintenance:** The inertia phase continues until a day is missed.

### **5. Guidelines and Principles**

- **Honesty and Integrity:**

  - The game relies on players being truthful about completing todos during quests and inertia.

- **Self-Assessment:**

  - Players should realistically evaluate their confidence levels and activity difficulties to ensure meaningful progress.

- **Risk and Reward:**

  - The CP system incentivizes commitment, as failing a quest results in the loss of pledged CP.

- **Encouragement of Multiple Quests:**

  - Players can undertake multiple quests simultaneously, limited only by their available CP.

### **6. Progression and Growth**

- **Accumulating CP:**

  - Completing quests and maintaining streaks through inertia allows players to accumulate CP.

- **Taking on Greater Challenges:**

  - With more CP, players can undertake longer or more difficult quests, aligning with personal growth.

- **Advancing Endeavors:**

  - Regular completion of activities contributes to progress in the player's chosen endeavors.

### **7. Customization and Flexibility**

- **Adjustments and Modifications:**

  - Players can add new activities or modify existing ones at any time to better suit their evolving goals.

- **No Mid-Quest Changes:**

  - Once a quest is initiated, its duration and difficulty cannot be altered until completion or failure.

### **8. Final Notes**

- **Motivation Through CP:**

  - The system is designed to motivate players by rewarding consistency and commitment while introducing risks to enhance engagement.

- **Balancing Commitments:**

  - Players should balance the difficulty and number of quests with their real-life capacities to avoid overcommitment.

- **Community and Support:**

  - While the game is self-managed, sharing progress with others can provide additional motivation and accountability.
