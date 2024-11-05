# [pacergame-rulebook-with-gpt](https://github.com/UniBreakfast/pacergame-rulebook-with-gpt)

## **PacerGame Rulebook**

### **1. Introduction**

Welcome to **PacerGame**, a gamified self-improvement system designed to help you achieve your goals through structured tasks and rewards. By engaging in meaningful activities aligned with your personal endeavors, you earn Confidence Points (CP) that fuel your progress and unlock new challenges.

### **2. Key Terms and Definitions**

- **Endeavors (ES):** Directions of interest such as wishes, goals, dreams, needs, skills to develop, or habits to build or break. They represent the overarching areas you want to focus on.

- **Activities (AS):**

  - **Creation:** Players add activities as they see fit at any point in time, with no restrictions on the number or type. Activities can remain in a list until the player decides to undertake them in a quest.

  - **Measurement Units:** The amount of activity is determined by the player upon creation, using any suitable units (e.g., times, minutes, reps, sets, pages, meters, liters).

  - **Difficulty Assignment:** Each activity is assigned a subjective difficulty level by the player upon creation, on a scale from 1 to 10. This difficulty affects the cost of quests derived from the activity.

  - **Modification Rules:** Activities cannot be modified while there is an ongoing quest associated with them. Any changes made after a quest has concluded do not retroactively affect past quests or calculations.

- **Quests (QS):**

  - **Initiation:** Players decide the desired duration of a quest in days, limited only by their available Confidence Points (CP).

  - **Association with Activities:** A quest is undertaken by selecting an activity from the player's list. The quest then sets a daily requirement (todo) based on the activity's parameters.

  - **Pledge:** To undertake a quest, players pledge CP equal to the quest's cost.

  - **Failure:** If a todo of a quest is not completed on any day, the quest fails, and the pledged CP is lost.

- **Todos (TS):**

  - **Definition:** The individual daily tasks within a quest. Each todo represents one day's commitment to perform the activity's required amount.

  - **Completion:** Marked by a daily checkmark when the activity's required amount is completed.

  - **Failure Reporting:** Players must explicitly report if they fail to complete a todo, resulting in the quest's failure.

- **Confidence Points (CP):**

  - **Initial CP:**

    - **Estimation at Game Start:** At the beginning of the game, players estimate their starting CP by assessing their confidence level on a scale from 1 to 10. This estimation is done once when the game starts.

    - **Re-estimation Conditions:** The initial CP estimation is not repeated unless:

      - The player reaches 0 CP with no active quests to gain more CP.

      - The player chooses to restart the game due to personal reasons, such as having stopped playing by the rules for an extended period.

  - **Earning CP:** Players earn CP immediately upon completing each todo and by successfully completing quests.

  - **Spending CP:** CP is spent when pledging for new quests.

- **Difficulty:**

  - **Assignment:** Activity difficulty is subjectively decided by the player upon creation, on a scale from 1 to 10.

- **Inertia:**

  - **Definition:** After completing a quest, players can continue performing the same activity daily without pledging more CP, maintaining their streak.

  - **Rewards:** The CP reward per todo remains the same during inertia, neither increasing nor decreasing.

### **3. Game Mechanics**

#### **3.1 Activities**

- **Creation and Management:**

  - Players can create activities that align with their endeavors at any time.

  - Activities can remain inactive in a list until the player is ready to undertake them in a quest.

- **Measurement and Units:**

  - Activities are quantified using units appropriate to the task (e.g., minutes, pages, kilometers).

- **Difficulty Assignment:**

  - Upon creating an activity, players assign it a difficulty level from 1 to 10, reflecting how challenging they perceive the activity to be.

- **Modification Rules:**

  - **No Modifications During Ongoing Quests:** Players should not modify an activity while there is an ongoing quest associated with that activity.

  - **Post-Quest Modifications:**

    - After all associated quests have concluded, players may modify the activity.

    - **No Retroactive Changes:** Any modifications made do not retroactively affect past quests or calculations.

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

  - **Completion Verification:** Players honestly assess and confirm the completion of each day's todo by marking a checkmark.

  - **Immediate CP Rewards:** Upon completing each todo, the player immediately gains CP calculated as the floor of the square root of the current consecutive day count within the quest. For example, on day 4 of a streak, the reward is floor(√4) = 2 CP.

  - **Failure Reporting:** If a player fails to complete a todo, they must explicitly report the failure, resulting in the quest's failure.

- **Completing a Quest:**

  - **Return of Pledged CP:** Upon completing the quest, the player receives their pledged CP back.

- **Quest Failure:**

  - **Explicit Reporting:** Players must explicitly report when they fail to complete a todo.

  - **Loss of Pledge:** If a player reports a failure, the quest fails, and the pledged CP is lost.

  - **Opportunity for New Quests:** Failing a quest is not the end—players can undertake similar or different new quests in the future as they accumulate more CP.

  - **Streak Reset:** The streak for that activity resets, and no further CP can be earned through inertia until a new quest is initiated.

#### **3.3 Confidence Points (CP)**

- **Initial CP:**

  - **One-Time Estimation:** At the start of the game, players estimate their initial CP by assessing their confidence level from 1 to 10. This estimation is done once and sets the foundation for the player's CP balance.

  - **Re-estimation Conditions:**

    - **Zero CP with No Active Quests:** If a player reaches 0 CP and has no active quests to gain more CP, they may re-estimate their initial CP to restart the game.

    - **Voluntary Restart:** If a player has stopped playing by the rules for an extended period or wishes to start over for personal reasons, they may choose to re-estimate their initial CP and begin anew.

- **Earning CP:**

  - **Per Todo:** CP earned per completed todo is calculated as floor(√day_in_row) and is gained immediately upon completion of the todo.

- **Spending CP:**

  - CP is spent when pledging for new quests, calculated based on the activity's difficulty and quest duration.

- **Accumulating CP After Failure:**

  - Players can accumulate CP from other ongoing quests or by starting new, affordable quests to rebuild their CP balance.

#### **3.4 Inertia**

- **Post-Quest Activity:**

  - After a quest is completed, players can continue performing the **same** activity daily without pledging additional CP.

  - **Quest-Specific:** Inertia applies only to the specific quest that was completed. It neither affects other quests nor is affected by the success or failure of other quests.

- **Maintaining the Streak:**

  - The streak continues as long as the player completes the daily todo.

  - Missing a day breaks the streak, ending the inertia phase.

- **Rewards During Inertia:**

  - The CP reward per todo remains constant, equal to the reward on the last day of the quest.

  - **Immediate Rewards:** CP earned during inertia is gained immediately upon completion of each todo.

- **No Losses on Breaking Streak:**

  - Breaking the streak during inertia brings no losses since the pledge was already returned upon quest completion. The player simply stops earning CP from that activity until a new quest is initiated.

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

  - **Day 1:**

    - **Complete Run:** Yes.

    - **Reward:** floor(√1) = 1 CP, gained immediately.

  - **Day 2:**

    - **Complete Run:** Yes.

    - **Reward:** floor(√2) = 1 CP, gained immediately.

  - **Day 3:**

    - **Complete Run:** Yes.

    - **Reward:** floor(√3) = 1 CP, gained immediately.

  - **Day 4:**

    - **Complete Run:** Yes.

    - **Reward:** floor(√4) = 2 CP, gained immediately.

  - **Day 5:**

    - **Complete Run:** Yes.

    - **Reward:** floor(√5) = 2 CP, gained immediately.

- **Total CP Earned from Todos:** 7 CP.

- **Quest Completion:**

  - **Pledge Returned:** Yes, 15 CP is returned to the player upon quest completion.

- **Total CP Calculation:**

  - **Starting CP:** Let's assume an initial CP of 20.

  - **Pledged CP:** -15 (for the quest).

  - **CP Earned from Todos:** +7 (gained immediately over the course of the quest).

  - **Pledge Returned:** +15 (upon quest completion).

  - **Total CP After Quest Completion:** 20 (initial) - 15 (pledge) + 7 (todos) + 15 (returned pledge) = **27 CP**.

- **Inertia Phase:**

  - **Continuation:** Player continues running 2 km daily without pledging more CP.

  - **Daily Reward:** CP reward remains at 2 CP per day (same as the reward on the last day of the quest), gained immediately upon completion of each todo.

  - **Streak Maintenance:** The inertia phase continues until a day is missed.

  - **Quest-Specific Inertia:** This inertia applies only to the running activity and does not impact any other quests or activities.

- **Breaking the Streak:**

  - If the player misses a day during inertia, the streak ends.

  - **No Losses:** There are no CP losses upon breaking the streak during inertia, as the pledge was already returned upon completing the original quest.

### **5. Guidelines and Principles**

- **Honesty and Integrity:**

  - The game relies on players being truthful about completing todos and reporting failures during quests and inertia.

- **Self-Assessment:**

  - Players should realistically evaluate their confidence levels and activity difficulties to ensure meaningful progress.

- **Risk and Reward:**

  - The CP system incentivizes commitment, as failing a quest results in the loss of pledged CP.

- **Embracing Failure:**

  - Failing a quest is not the end. It's an opportunity to reassess and try again.

  - Players can undertake similar or different new quests in the future as they accumulate more CP.

- **Starting Over:**

  - **When to Re-estimate Initial CP:**

    - If a player reaches 0 CP with no active quests to gain more CP, they may choose to restart the game by re-estimating their initial CP.

    - Players may also restart if they have taken a significant break from the game and wish to begin anew.

  - **Re-estimation Process:**

    - The player reassesses their confidence level from 1 to 10 to determine a new initial CP.

- **Encouragement of Multiple Quests:**

  - Players can undertake multiple quests simultaneously, limited only by their available CP.

### **6. Progression and Growth**

- **Accumulating CP:**

  - Completing quests and maintaining streaks through inertia allows players to accumulate CP.

- **Rebuilding After Failure:**

  - Players can rebuild their CP balance by starting new quests that fit within their current CP availability.

- **Taking on Greater Challenges:**

  - With more CP, players can undertake longer or more difficult quests, aligning with personal growth.

- **Advancing Endeavors:**

  - Regular completion of activities contributes to progress in the player's chosen endeavors.

### **7. Customization and Flexibility**

- **Adding New Activities:**

  - Players can add new activities at any time to align with their evolving goals.

- **Modifying Existing Activities:**

  - **No Modifications During Ongoing Quests:**

    - Players should not modify an activity while there is an ongoing quest associated with it.

    - This ensures consistency and fairness in quest calculations and CP rewards.

  - **Post-Quest Modifications:**

    - Once all quests associated with an activity have concluded, players may modify the activity's parameters, such as difficulty or required amount.

    - **No Retroactive Changes:**

      - Modifications made to an activity do not retroactively affect past quests, CP calculations, or rewards.

      - Past quests remain as they were originally undertaken, preserving the integrity of the game's history.

- **No Mid-Quest Changes:**

  - Once a quest is initiated, its duration and difficulty cannot be altered until completion or failure.

### **8. Final Notes**

- **Motivation Through CP:**

  - The system is designed to motivate players by rewarding consistency and commitment while introducing risks to enhance engagement.

- **Balancing Commitments:**

  - Players should balance the difficulty and number of quests with their real-life capacities to avoid overcommitment.

- **Positive Outlook on Failure:**

  - Failing a quest provides valuable insight into personal limits and areas for improvement.

  - Players are encouraged to view setbacks as learning opportunities.

- **Restarting the Game:**

  - Players have the option to restart the game under specific conditions, allowing for a fresh start and renewed motivation.

- **Community and Support:**

  - While the game is self-managed, sharing progress with others can provide additional motivation and accountability.
