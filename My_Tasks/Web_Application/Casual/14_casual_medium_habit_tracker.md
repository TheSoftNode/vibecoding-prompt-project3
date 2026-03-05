Category: Web Application

Prompt style: Casual

Title: Habit Tracker with Milestones

Prompt: Habit tracker but make it actually useful. Add habits with name and target frequency per week. Show current week view with 7 day columns. Click a day to mark habit done, shows checkmark. Track both current streak and best streak for each habit (consecutive weeks hitting target). Habit cards turn green when current streak hits 7+ weeks, gold when 30+ weeks. Show "Best Streak!" badge when current streak matches or exceeds best streak. Calculate completion rate percentage for each habit (completed days ÷ target frequency × weeks tracked). Display weekly progress bar showing how many habits hit target out of total. Filter buttons for All, Active (not hit target this week), Completed (hit target). Show "At Risk" warning in red for habits with current streak = 0 but best streak > 5. Make it look clean.

Required libraries: react, tailwindcss, lucide-react, framer-motion

## Rubric

| ID            | Description                                                                                              | Weight | Rationale                                                                           | Dependent On       |
| ------------- | -------------------------------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------- | ------------------ |
| visual-1      | Render input fields for habit name and target frequency per week                                         | major  | Name and frequency define the essential habit attributes.                           | None               |
| visual-2      | Display an add button for creating habits                                                                | major  | Add button triggers habit creation.                                                 | None               |
| interaction-1 | Create a new habit when the add button is clicked                                                        | major  | Habit creation is the core setup interaction.                                       | visual-2           |
| layout-1      | Display current week view with 7 day columns                                                             | major  | Seven-day layout provides the structure for daily habit tracking.                   | None               |
| interaction-2 | Mark a habit as done for a specific day when that day is clicked                                         | major  | Day clicking is the primary tracking interaction.                                   | layout-1           |
| visual-3      | Display a checkmark when a habit is marked done for a day                                                | major  | Checkmark provides visual confirmation of habit completion.                         | interaction-2      |
| content-1     | Display current streak count for each habit showing consecutive weeks hitting target frequency           | major  | Current streak tracks ongoing consistency performance.                              | None               |
| state-1       | Increment current streak when a habit hits its target frequency for the current week                     | major  | Streak increment depends on comparing completed days to target frequency.           | content-1          |
| state-2       | Reset current streak to zero when a habit fails to hit target frequency for a week                       | major  | Streak reset enforces consecutive week requirement for streak maintenance.          | content-1          |
| content-2     | Display best streak count for each habit showing highest consecutive weeks achieved                      | major  | Best streak provides historical peak performance tracking.                          | None               |
| state-3       | Update best streak when current streak exceeds the previous best streak value                            | major  | Best streak updates require comparison between current and historical maximum.      | content-2          |
| visual-4      | Apply green background color to habit cards when current streak reaches 7 or more weeks                  | major  | Green signals significant streak milestone achievement.                             | content-1          |
| visual-5      | Apply gold background color to habit cards when current streak reaches 30 or more weeks                  | major  | Gold signals exceptional long-term consistency milestone.                           | content-1          |
| visual-6      | Display "Best Streak!" badge on habits when current streak equals or exceeds best streak                 | major  | Badge celebrates matching or breaking personal records.                             | content-1, content-2 |
| state-4       | Show "Best Streak!" badge only when current streak value is greater than or equal to best streak value   | major  | Badge visibility tests comparison logic between current and best streak.            | visual-6           |
| content-3     | Display completion rate percentage for each habit                                                        | major  | Completion rate provides overall performance metric beyond weekly targets.          | None               |
| state-5       | Calculate completion rate as (completed days ÷ target frequency × weeks tracked) × 100                   | major  | Completion rate is a multi-step derived percentage requiring division and multiplication. | content-3          |
| state-6       | Update completion rate when habits are marked done or weeks tracked increases                            | major  | Completion rate must recalculate as numerator and denominator change.               | content-3          |
| content-4     | Display a weekly progress bar showing habits that hit target out of total habits                         | major  | Weekly progress bar provides at-a-glance current week achievement assessment.       | None               |
| state-7       | Update progress bar when habits are marked done or target frequencies change                             | major  | Progress bar synchronization ensures real-time accuracy within the current week.    | content-4          |
| visual-7      | Display three filter buttons labeled All, Active, and Completed                                          | major  | Filter buttons enable users to focus on specific habit subsets.                     | None               |
| state-8       | Display all habits when the All filter button is clicked                                                 | major  | All filter restores full habit list visibility.                                     | visual-7           |
| state-9       | Display only habits that have not hit their target this week when Active filter is clicked               | major  | Active filter isolates habits requiring attention.                                  | visual-7           |
| state-10      | Display only habits that have hit their target this week when Completed filter is clicked                | major  | Completed filter celebrates achieved habits.                                        | visual-7           |
| visual-8      | Display "At Risk" warning in red color for applicable habits                                             | major  | At Risk warning alerts users to habits that have fallen off after strong performance. | None               |
| state-11      | Show "At Risk" warning only when current streak equals 0 and best streak is greater than 5               | major  | Conditional warning tests compound logic (zero current AND high historical).        | visual-8           |
