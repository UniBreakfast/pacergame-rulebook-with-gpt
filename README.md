# [pacergame-rulebook-with-gpt](https://github.com/UniBreakfast/pacergame-rulebook-with-gpt)

## **PacerGame Rulebook**

### **1. Introduction**

Welcome to **PacerGame**, a gamified self-improvement system designed to help you achieve your goals through structured tasks and rewards. By engaging in meaningful activities aligned with your personal endeavors, you earn Confidence Points (CP) that fuel your progress and unlock new challenges.

### **2. Key Terms and Definitions**

- **Endeavors (ES):** Overarching areas of interest such as wishes, goals, dreams, needs, skills to develop, or habits to build or break. They represent what you want to focus on.

- **Activities (AS):**
  - **Creation:** Specific tasks you can perform to advance your endeavors. You can create activities at any time.
  - **Measurement Units:** Quantified using appropriate units (e.g., minutes, pages, kilometers).
  - **Difficulty Assignment:** Assigned a subjective difficulty level from 1 to 10 upon creation.
  - **Modification Rules:** Cannot be modified during ongoing quests. Changes made after quests conclude do not retroactively affect past quests or calculations.

- **Quests (QS):**
  - Commitments to perform an activity daily over a specified duration.
  - Initiated by pledging CP equal to the quest's cost.
  - Failure to complete a daily task results in quest failure and loss of pledged CP.

- **Todos (TS):**
  - The daily tasks within a quest.
  - Each todo represents one day's commitment to perform the activity's required amount.
  - Completion is marked by a daily checkmark.

- **Confidence Points (CP):**
  - The game's currency, representing your confidence and progress.
  - Spent when initiating quests and earned by completing todos and quests.

- **Inertia:**
  - The phase after completing a quest.
  - Allows continuation of the same activity daily without pledging additional CP.
  - Maintains the streak and earns CP rewards.

### **3. Game Mechanics**

#### **3.1 Activities**

- **Creation and Management:**
  - Create activities aligned with your endeavors at any time.
  - Activities remain inactive until undertaken in a quest.
  - Assign a difficulty level from 1 to 10 to each activity.
  - Quantify activities using appropriate units.

- **Modification Rules:**
  - Do not modify activities while associated quests are ongoing.
  - Post-quest modifications do not affect past quests or calculations.

#### **3.2 Quests**

- **Starting a Quest:**
  - **Select an Activity:** Choose an activity to form the basis of the quest.
  - **Determine Duration:** Decide the quest's duration in days, based on your goals and available CP.
  - **Calculate Cost:** Quest Cost = Activity Difficulty × Quest Duration.
  - **Pledge CP:** Pledge CP equal to the quest's cost to initiate it.

- **Todos and Completion:**
  - **Daily Commitment:** Complete the activity's required amount each day.
  - **Verification:** Honestly confirm completion of each todo.
  - **Immediate CP Rewards:** Gain CP immediately upon completing each todo, calculated as floor(√day_in_row), where day_in_row is the current consecutive day count.
  - **Failure Reporting:** Explicitly report any failure to complete a todo, resulting in quest failure and loss of pledged CP.

- **Quest Completion:**
  - **Receive Pledged CP Back:** Upon completing the quest, get your pledged CP returned.

- **Quest Failure:**
  - **Loss of Pledge:** Failure to complete a todo results in loss of pledged CP.
  - **Reattempts:** You can undertake new quests in the future as you accumulate more CP.

#### **3.3 Confidence Points (CP)**

- **Initial CP:**
  - **Estimation at Game Start:** Estimate your starting CP by assessing your confidence level from 1 to 10. This is done once at the game's start.
  - **Re-estimation Conditions:** Only re-estimate initial CP if:
    - You reach 0 CP with no active quests.
    - You choose to restart the game after an extended break.

- **Earning CP:**
  - **Per Todo:** Gain CP immediately upon completing each todo.
  - **Quest Completion:** Receive pledged CP back upon successful quest completion.

- **Spending CP:**
  - **Pledging for Quests:** Spend CP when initiating new quests.

#### **3.4 Inertia**

- **Post-Quest Activity:**
  - Continue performing the same activity daily without pledging more CP after completing a quest.
  - Inertia is specific to the completed quest's activity and independent of other quests.

- **Maintaining the Streak:**
  - Complete the daily todo to maintain the streak.
  - Missing a day ends the inertia phase.

- **Rewards During Inertia:**
  - CP reward per todo remains constant, equal to the reward on the last day of the quest.
  - Rewards are gained immediately upon completion.
  - No losses occur if the streak is broken during inertia since the pledge was already returned.

### **4. Example Scenario**

**Endeavor:** Improve Physical Fitness

- **Activity:** Run 2 kilometers.
  - **Difficulty:** 3.

- **Quest:**
  - **Duration:** 5 days.
  - **Cost:** 3 (difficulty) × 5 (days) = **15 CP**.
  - **Pledge:** 15 CP.

- **Daily Todos and Rewards:**
  - **Day 1:** Complete run. Reward: floor(√1) = **1 CP**.
  - **Day 2:** Complete run. Reward: floor(√2) = **1 CP**.
  - **Day 3:** Complete run. Reward: floor(√3) = **1 CP**.
  - **Day 4:** Complete run. Reward: floor(√4) = **2 CP**.
  - **Day 5:** Complete run. Reward: floor(√5) = **2 CP**.

- **Total CP Earned from Todos:** **7 CP**.

- **Quest Completion:**
  - **Receive Pledged CP Back:** 15 CP.

- **Total CP Calculation:**
  - **Starting CP:** Assume 20 CP.
  - **After Quest Completion:** 20 (initial) - 15 (pledge) + 7 (todos) + 15 (pledge returned) = **27 CP**.

- **Inertia Phase:**
  - **Continuation:** Continue running 2 km daily without pledging more CP.
  - **Daily Reward:** 2 CP per day.
  - **Streak Maintenance:** Continues until a day is missed.
  - **No Losses on Breaking Streak:** Pledge has been returned; no penalties for ending inertia.

### **5. Guidelines and Principles**

- **Honesty and Integrity:**
  - Be truthful about completing todos and reporting failures.
  - Accurately assess activity difficulties and confidence levels.

- **Risk and Reward:**
  - Commitment is incentivized through the CP system.
  - Failing a quest results in loss of pledged CP but offers an opportunity to reassess and try again.

- **Starting Over:**
  - Re-estimate initial CP only if you reach 0 CP with no active quests or after an extended break.

- **Multiple Quests:**
  - Undertake multiple quests simultaneously, limited by your available CP.

### **6. Progression and Growth**

- **Accumulating CP:**
  - Complete quests and maintain streaks to accumulate CP.

- **Rebuilding After Failure:**
  - Start new, affordable quests to rebuild your CP balance.

- **Advancing Endeavors:**
  - Regularly completing activities contributes to progress in your chosen endeavors.

### **7. Customization and Flexibility**

- **Adding New Activities:**
  - Add new activities at any time to align with your evolving goals.

- **Modifying Activities:**
  - Do not modify an activity during an ongoing quest.
  - Modifications after quests conclude do not retroactively affect past quests.

- **No Mid-Quest Changes:**
  - Duration and difficulty of a quest cannot be altered once initiated.

### **8. Final Notes**

- **Motivation Through CP:**
  - The system motivates by rewarding consistency and introducing risks.

- **Balancing Commitments:**
  - Balance the difficulty and number of quests with your real-life capacities to avoid overcommitment.

- **Positive Outlook on Failure:**
  - View setbacks as learning opportunities.

- **Community and Support:**
  - Sharing progress with others can provide additional motivation and accountability.
