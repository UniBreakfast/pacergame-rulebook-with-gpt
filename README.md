# [pacergame-rulebook-with-gpt](https://github.com/UniBreakfast/pacergame-rulebook-with-gpt)

# **PacerGame Rulebook**

## **1. Introduction**

Welcome to **PacerGame**, a gamified self-improvement system designed to help you achieve your goals through structured tasks and rewards. By engaging in meaningful activities aligned with your personal endeavors, you earn Confidence Points (CP) that fuel your progress and unlock new challenges.

## **2. Key Concepts**

### **2.1 Endeavors (ES)**

- **Definition:** Overarching areas of interest such as goals, dreams, needs, skills to develop, or habits to build or break.
- **Purpose:** Provide direction and focus for selecting activities.

### **2.2 Activities (AS)**

- **Creation:** Specific tasks you can perform to advance your endeavors. You can create activities at any time.
- **Measurement Units:** Quantified using appropriate units (e.g., minutes, pages, kilometers).
- **Difficulty Assignment:** Assign a subjective difficulty level from 1 to 10 upon creation.
- **Modification Rules:**
  - **No Modifications During Ongoing Quests:** Activities cannot be modified while associated quests are active.
  - **Post-Quest Modifications:** Allowed after quests conclude but do not retroactively affect past quests or calculations.

## **3. Game Mechanics**

### **3.1 Confidence Points (CP)**

- **Initial CP Assessment:**
  - **Estimation at Game Start:** Assess your confidence level from **2 to 10** to determine your starting CP.
  - **Note:** If your confidence level is less than 2, consider seeking guidance from a qualified professional before starting.
- **Earning CP:**
  - **Per Todo:** Gain CP immediately upon completing each todo, calculated as `floor(√n)`, where `n` is the current consecutive day count within the quest and any unbroken sequence of quests for the same activity (excluding days from inertia).
  - **Quest Completion:** Receive pledged CP back upon successful quest completion.
- **Spending CP:**
  - **Pledging for Quests:** Spend CP equal to the quest's cost when initiating new quests.

### **3.2 Quests (QS)**

- **Starting a Quest:**
  - **Select an Activity:** Choose an activity to form the basis of the quest.
  - **Determine Start Date:** Decide when the quest begins—today (only for quests longer than one day), tomorrow, or the day after.
  - **Determine Duration:** Decide the quest's duration in days, based on your goals and available CP.
  - **Calculate Cost:** `Quest Cost = Activity Difficulty × Quest Duration`.
  - **Pledge CP:** Pledge CP equal to the quest's cost to initiate it.
  - **Overlap Restrictions:** No overlapping quests for the same activity are allowed.
- **Todos and Completion:**
  - **Daily Commitment:** Complete the activity's required amount each day.
  - **Verification:** Honestly confirm completion of each todo.
  - **Immediate CP Rewards:** Gain CP immediately upon completing each todo, calculated as `floor(√n)`, where `n` is the current consecutive day count within the quest and any unbroken sequence of quests for the same activity (excluding days from inertia).
  - **Maximum Reward per Todo:** Capped by the activity's difficulty at the time the quest is taken.
- **Quest Failure:**
  - **Failure Reporting:** Explicitly report any failure to complete a todo.
  - **Consequences:**
    - **Loss of Pledge:** Lose pledged CP upon quest failure.
    - **Difficulty Adjustment:** Increase the activity's difficulty by 1 (can exceed 10) if the quest duration was equal to or longer than your initial confidence level.
    - **No Overlaps with New Quests:** Completed and failed days of the quest cannot overlap with another quest for the same activity.
    - **Discarded Todos:** Remaining todos from the failed quest are discarded and cannot be reported or rewarded.
- **Quest Completion:**
  - **Receive Pledged CP Back:** Upon completing the quest, get your pledged CP returned.
  - **Difficulty Adjustment:** Decrease the activity's difficulty by 1 (not below 1) if the quest duration was equal to or longer than your initial confidence level.
  - **Inertia Phase Initiation:** Option to continue the activity in the inertia phase.

### **3.3 Inertia**

- **Definition:** The phase after completing a quest, allowing continuation of the same activity without pledging additional CP.
- **Rules:**
  - **Activity Continuation:** Continue performing the same activity daily.
  - **Streak Maintenance:** Maintain your consecutive day count for the purpose of continuing the activity, but note that days in inertia are not counted towards reward calculations in future quests.
  - **Rewards:**
    - **CP Reward per Todo:** Remains constant during inertia, equal to the reward on the last day of the quest.
    - **Immediate Rewards:** CP earned during inertia is gained immediately upon completion of each todo.
  - **Breaking the Streak:**
    - **No Losses:** No CP losses upon ending inertia since the pledge was already returned.
    - **Consecutive Day Count Reset:** If you miss a day, the streak ends, and your consecutive day count is reset.

### **3.4 Streaks and Consecutive Days**

- **Consecutive Day Count:**
  - **Within a Quest:** Days are counted consecutively for reward calculation.
  - **Between Quests (Same Activity):** If you start a new quest for the same activity without missing a day (excluding days of inertia), the consecutive day count continues from where it left off at the end of the last quest.
  - **Excluding Inertia Days:** Days spent in the inertia phase are **not** counted towards the consecutive day count for reward calculations in new quests.
- **Starting New Quests Without Breaking Streaks:**
  - **Seamless Transition:** If you start a new quest for the same activity on the next day after completing a quest or inertia phase **without missing a day**, your day count for reward calculation resumes from the end of the last quest (excluding inertia days).
  - **Reward Calculation:** The first day's todo in the new quest is considered the next in sequence from the last quest day count (e.g., if the last quest ended on day 8, the new quest starts at day 9 for reward purposes).
- **Example:**
  - **First Quest Completed:** 8-day quest completed successfully.
  - **Inertia Phase:** 5 days of continued activity (days 9-13 for activity tracking but not for reward calculation in future quests).
  - **New Quest Initiated:** Start a new quest on day 14 without missing a day.
  - **Consecutive Day Count for Rewards:** The new quest's first todo is considered day **9** (not day 14) for reward calculation.
  - **Rewards:** Calculated as `floor(√9) = 3 CP`, capped by the activity's difficulty at the time the new quest is taken.

## **4. Example Scenario**

**Endeavor:** Improve Physical Fitness

- **Activity:** Run 2 kilometers.
  - **Initial Difficulty:** 7.

### **First Quest**

- **Duration:** 8 days.
- **Start Date:** Tomorrow.
- **Cost:** `7 (difficulty) × 8 (days) = 56 CP`.
- **Pledge:** 56 CP.
- **Daily Todos and Rewards:**
  - **Days 1-8:** Complete run each day.
    - **Rewards:** 
      - Day 1: `floor(√1) = 1 CP`
      - Day 2: `floor(√2) = 1 CP`
      - Day 3: `floor(√3) = 1 CP`
      - Day 4: `floor(√4) = 2 CP`
      - Day 5: `floor(√5) = 2 CP`
      - Day 6: `floor(√6) = 2 CP`
      - Day 7: `floor(√7) = 2 CP`
      - Day 8: `floor(√8) = 2 CP`
    - **Note:** Rewards are capped at the activity's difficulty.
- **Total CP Earned from Todos:** 13 CP.
- **Quest Completion:**
  - **Receive Pledged CP Back:** 56 CP.
  - **Difficulty Adjustment:** Decrease difficulty to 6 (since duration ≥ initial confidence level).

### **Inertia Phase**

- **Duration:** 5 days (days 9-13).
- **Rewards:** Each day rewards 2 CP (same as the last quest day).
- **Streak Maintenance:** Continue the activity without breaking the streak for activity tracking purposes.
- **Note:** Days in inertia are not counted towards consecutive day count for reward calculations in future quests.

### **Second Quest**

- **Start Date:** Day 14 (after inertia phase, without missing a day).
- **Duration:** Your choice (e.g., 5 days).
- **New Difficulty:** 6 (after adjustment from previous quest).
- **Cost:** `6 (difficulty) × 5 (days) = 30 CP`.
- **Pledge:** 30 CP.
- **Consecutive Day Count for Rewards:** Resumes from day 9 (since inertia days are excluded).
- **Daily Todos and Rewards:**
  - **Days 9-13 (Inertia):** Rewards during inertia are fixed at 2 CP per day.
  - **Day 9 (First day of new quest):** `floor(√9) = 3 CP`
  - **Day 10:** `floor(√10) = 3 CP`
  - **Day 11:** `floor(√11) = 3 CP`
  - **Day 12:** `floor(√12) = 3 CP`
  - **Day 13:** `floor(√13) = 3 CP`
  - **Note:** Rewards are capped at the new activity difficulty of 6.
- **Total CP Earned from Todos in Second Quest:** 15 CP.
- **Quest Completion:**
  - **Receive Pledged CP Back:** 30 CP.
  - **Difficulty Adjustment:** Decrease difficulty to 5 (since duration ≥ initial confidence level).

## **5. Guidelines and Principles**

### **5.1 Honesty and Integrity**

- Be truthful about completing todos and reporting failures.
- Accurately assess activity difficulties and confidence levels.

### **5.2 Risk and Reward**

- **Commitment Incentive:** Pledging CP encourages commitment.
- **Consequences of Failure:** Loss of pledged CP and potential increase in activity difficulty.
- **Opportunity for Growth:** Use failures to reassess and adjust strategies.

### **5.3 Adjusting Activity Difficulty**

- **Upon Quest Completion:**
  - **Success:** Decrease difficulty by 1 (minimum of 1).
  - **Failure:** Increase difficulty by 1.
- **Conditions:**
  - **Quest Duration Requirement:** Adjustments apply only if the quest duration was equal to or longer than your initial confidence level.
- **Effect on Rewards:**
  - **Reward Cap During Inertia:** Changes in difficulty do not affect the reward cap until the end of the current inertia phase.

### **5.4 Starting Over**

- **Re-estimation of Initial CP:**
  - Allowed if you reach 0 CP with no active quests.
  - Permitted after an extended break from the game.

### **5.5 Multiple Quests**

- **Simultaneous Quests:** Allowed for different activities.
- **Overlap Restrictions:** No overlapping quests for the same activity.

### **5.6 No Overlapping Quests for the Same Activity**

- **Rule:** Cannot start a new quest for the same activity that overlaps with days from a previous quest.
- **Failed Quest Days:**
  - **Completed Days:** Cannot be overlapped.
  - **Failed and Remaining Days:** Discarded and cannot be reported or rewarded.

## **6. Progression and Growth**

- **Accumulating CP:** Complete quests and maintain streaks to accumulate CP.
- **Rebuilding After Failure:** Start new quests to rebuild your CP balance.
- **Advancing Endeavors:** Regularly completing activities contributes to progress in your chosen endeavors.

## **7. Customization and Flexibility**

- **Adding New Activities:** You can add new activities at any time.
- **Modifying Activities:**
  - **During Quests:** Not allowed.
  - **After Quests:** Allowed without retroactive effects.
- **No Mid-Quest Changes:** Quest duration and difficulty cannot be altered once initiated.

## **8. Final Notes**

- **Motivation Through CP:** The system motivates by rewarding consistency and introducing risks.
- **Balancing Commitments:** Balance quest difficulty and number with your real-life capacities to avoid overcommitment.
- **Positive Outlook on Failure:** View setbacks as learning opportunities.
- **Community and Support:** Sharing progress with others can provide additional motivation and accountability.
