# [pacergame-rulebook-with-gpt](https://github.com/UniBreakfast/pacergame-rulebook-with-gpt)

# PacerGame (PG) Rulebook

## 1. Introduction

Welcome to **PacerGame**, a gamified self-improvement system designed to help you become a confident and accomplished individual. PacerGame empowers you to build a strong and consistent momentum towards personal growth, creating and strengthening a tendency to achieve goals and fulfill desires. By engaging in meaningful activities aligned with your personal endeavors, you earn Confidence Points (CP) that fuel your progress and unlock new challenges.

## 2. Key Concepts

### 2.1 Endeavors (ES)

- **Definition:** Overarching areas of interest such as goals, dreams, desires, needs, skills to develop, knowledge to acquire or deepen, or habits to build or break.

- **Purpose:** Provide direction and focus for selecting activities and help evaluate overall progress in achieving desired outcomes.

### 2.2 Activities (AS)

- **Definition:** Specific tasks with clearly defined amounts in appropriate units and subjectively estimated difficulty levels.

- **Purpose:** Serve as a basis for quests to facilitate the pursuit of specific endeavors.

### 2.3 Quests (QS)

- **Definition:** Commitments to perform a specific activity daily over a set duration, with CP pledged as a stake.

- **Purpose:** Provide structured challenges that encourage consistency and dedication, tracking effort investment and reported progress.

### 2.4 Todos (TS)

- **Definition:** Daily tasks within a quest that require the completion of the activity's specific amount.

- **Purpose:** Break down quests into manageable daily actions, fostering daily engagement and progress toward endeavors.

### 2.5 Confidence Points (CP)

- **Definition:** The in-game measurable resource representing your confidence and progress, used to pledge when initiating quests and earned by completing todos.

- **Purpose:** Motivate commitment and accountability, providing a risk-reward system that incentivizes consistent effort.

## 3. Game Mechanics

### 3.1 Activities (AS)

- **Creation:**

  - **Specific Tasks with Defined Amounts:** When creating an activity, specify a specific amount using appropriate units such as minutes, pages, or kilometers. This defines the exact requirement for the activity.

- **Difficulty Assignment:**

  - **Based on Specific Amount:** Assign a subjective difficulty level from 1 to 10, considering the specific amount you've set for the activity.

- **Modification Rules:**

  - **No Modifications During Ongoing Quests:** Activities cannot be modified while associated quests are active.

  - **Post-Quest Modifications:** Allowed after quests conclude but do not retroactively affect past quests or calculations.

### 3.2 Confidence Points (CP)

- **Initial CP Assessment:**

  - **Estimation at Game Start:** Assess your confidence level from 2 to 10 to determine your starting CP.

  - **Note:** If your confidence level is less than 2, consider seeking guidance from a qualified professional before starting.

- **Earning CP:**

  - **Per Todo:** Gain CP upon completing each todo, calculated as `floor(√n)`, where `n` is the current consecutive day count within the quest and any unbroken sequence of quests for the same activity (excluding days from inertia).

  - **Immediate Rewards:** All completed todo rewards are immediate.

- **Spending CP:**

  - **Pledging for Quests:** Spend CP equal to the quest's cost when initiating new quests.

### 3.3 Quests (QS)

- **Starting a Quest:**

  - **Select an Activity:** Choose an activity from your list to form the basis of the quest.

  - **Determine Start Date:** Decide when the quest begins—today (only for quests longer than one day), tomorrow, or the day after.

  - **Determine Duration:** Decide the quest's duration in days, based on your goals and available CP.

  - **Calculate Cost:** `Quest Cost = Activity Difficulty × Quest Duration`.

  - **Pledge CP:** Pledge CP equal to the quest's cost to initiate it.

  - **Overlap Restrictions:** No overlapping quests for the same activity are allowed.

- **Todos and Completion:**

  - **Daily Commitment:** Complete the activity's specific amount each day.

  - **Verification:** Honestly confirm completion of each todo.

  - **Per Todo CP Rewards:** Gain CP upon completing each todo, calculated as `floor(√n)`, where `n` is the current consecutive day count within the quest and any unbroken sequence of quests for the same activity (excluding days from inertia).

  - **Maximum Reward per Todo:** Capped by the activity's difficulty at the time the quest is taken.

- **Quest Failure:**

  - **Failure Reporting:** Explicitly report any failure to complete a todo.

  - **Consequences:**

    - **Loss of Pledge:** Lose pledged CP upon quest failure.

    - **Difficulty Adjustment:** Increase the activity's difficulty by 1 (can exceed 10) if the quest duration was equal to or longer than your initial confidence level.

    - **No Overlaps with New Quests:** Days of completed and failed todos of a finished quest or any days of an unfinished quest cannot overlap with another quest for the same activity.

    - **Discarded Todos:** Remaining todos from the failed quest are discarded and cannot be reported or rewarded.

- **Quest Completion:**

  - **Receive Pledged CP Back:** Upon completing the quest, get your pledged CP returned.

  - **Difficulty Adjustment:** Decrease the activity's difficulty by 1 (not below 1) if the quest duration was equal to or longer than your initial confidence level.

  - **Inertia Phase Initiation:** Option to continue the activity in the inertia phase.

  - **Definition of Finished Quest:** A quest is considered finished if it is either completed or failed, even if inertia continues.

### 3.4 Inertia

- **Definition:** The phase after completing a quest, allowing continuation of the same activity without pledging additional CP.

- **Rules:**

  - **Activity Continuation:** Continue performing the same activity with the same specific amount daily.

  - **Streak Maintenance:** Maintain your consecutive day count for the purpose of continuing the activity, but note that days in inertia are not counted towards reward calculations in future quests.

- **Rewards:**

  - **CP Reward per Todo:** Remains constant during inertia, equal to the reward on the last day of the quest.

- **Overlapping with New Quests:**

  - **No Overlaps Allowed:** Reported todo days of inertia cannot overlap with new quest days.

  - **Unreported Todos:** If you choose to start a new quest that would overlap with unreported inertia days, those unreported days are discarded.

- **Breaking the Streak:**

  - **No Losses:** No CP losses upon ending inertia since the pledge was already returned.

  - **Consecutive Day Count Reset:** If you miss a day, the streak ends, and your consecutive day count is reset.

### 3.5 Streaks and Consecutive Days

- **Consecutive Day Count:**

  - **Within a Quest:** Days are counted consecutively for reward calculation.

  - **Between Quests (Same Activity):** If you start a new quest for the same activity without missing a day (excluding days from inertia), the consecutive day count continues from where it left off at the end of the last quest.

  - **Excluding Inertia Days:** Days spent in the inertia phase are **not** counted towards the consecutive day count for reward calculations in new quests.

- **Starting New Quests Without Breaking Streaks:**

  - **Seamless Transition:** If you start a new quest for the same activity on the next day after completing a quest or inertia phase without missing a day, your day count for reward calculation resumes from the end of the last quest (excluding inertia days).

  - **Reward Calculation:** The first day's todo in the new quest is considered the next in sequence from the last quest day count (e.g., if the last quest ended on day 8, the new quest starts at day 9 for reward purposes).

## 4. Guidelines and Principles

### 4.1 Honesty and Integrity

- Be truthful about completing todos and reporting failures.

- Accurately assess activity difficulties based on the specific amounts.

### 4.2 Risk and Reward

- **Commitment Incentive:** Pledging CP encourages commitment.

- **Consequences of Failure:** Loss of pledged CP and potential increase in activity difficulty.

- **Opportunity for Growth:** Use failures to reassess and adjust strategies.

### 4.3 Adjusting Activity Difficulty

- **Upon Quest Completion:**

  - **Success:** Decrease difficulty by 1 (minimum of 1).

  - **Failure:** Increase difficulty by 1.

- **Conditions:**

  - **Quest Duration Requirement:** Adjustments apply only if the quest duration was equal to or longer than your initial confidence level.

- **Effect on Rewards:**

  - **Reward Cap During Inertia:** Changes in difficulty do not affect the reward cap until the end of the current inertia phase.

### 4.4 Starting Over

- **Re-estimation of Initial CP:**

  - Allowed if you reach 0 CP with no active quests.

  - Permitted after an extended break from the game.

### 4.5 Multiple Quests

- **Simultaneous Quests:** Allowed for different activities.

- **Overlap Restrictions:** No overlapping quests for the same activity.

### 4.6 No Overlapping Quests for the Same Activity

- **Rule:** Days of completed and failed todos of a finished quest or any days of an unfinished quest cannot overlap with another quest for the same activity.

- **Failed Quest Days:**

  - **Completed and Failed Todos:** Cannot be overlapped.

  - **Remaining Unfinished Days:** Discarded and cannot be reported or rewarded.

- **Inertia Days:**

  - **Reported Inertia Days:** Cannot overlap with new quest days.

  - **Unreported Inertia Days:** Discarded if they would overlap with a new quest.

## 5. Progression and Growth

- **Accumulating CP:** Complete quests and maintain streaks to accumulate CP.

- **Rebuilding After Failure:** Start new quests to rebuild your CP balance.

- **Advancing Endeavors:** Regularly completing activities contributes to progress in your chosen endeavors.

## 6. Customization and Flexibility

- **Adding New Activities:** You can add new activities at any time, specifying the exact amount and appropriate units.

- **Modifying Activities:**

  - **During Quests:** Not allowed.

  - **After Quests:** Allowed without retroactive effects.

- **No Mid-Quest Changes:** Quest duration and difficulty cannot be altered once initiated.

## 7. Final Notes

- **Motivation Through CP:** The system motivates by rewarding consistency and introducing risks.

- **Balancing Commitments:** Balance quest difficulty and number with your real-life capacities to avoid overcommitment.

- **Positive Outlook on Failure:** View setbacks as learning opportunities.

- **Community and Support:** Sharing progress with others can provide additional motivation and accountability.
