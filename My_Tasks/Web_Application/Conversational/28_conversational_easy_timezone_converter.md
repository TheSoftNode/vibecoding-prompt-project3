Category: Web_Application

Prompt style: Conversational

Title: Meeting Time Zone Converter

Prompt: I want a meeting time zone converter. Display a time picker labeled "Your time" and a dropdown with three zones: "PST (UTC-8)", "EST (UTC-5)", "GMT (UTC+0)". When I select a time and zone, show three converted times below labeled "PST time:", "EST time:", and "GMT time:" with the converted hour:minute values. Default to showing 9:00 AM in all zones on load.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display time picker                                  | major  | The time picker lets users select their meeting time.                                        | None         |
| 2   | content     | Label time picker "Your time"                        | minor  | The label clarifies that users enter their local time.                                       | C1           |
| 3   | visual      | Display timezone dropdown                            | major  | The dropdown lets users select their current timezone.                                       | None         |
| 4   | content     | Show "PST (UTC-8)" option in dropdown                | minor  | PST option allows users in Pacific time to select their zone.                                | C3           |
| 5   | content     | Show "EST (UTC-5)" option in dropdown                | minor  | EST option allows users in Eastern time to select their zone.                                | C3           |
| 6   | content     | Show "GMT (UTC+0)" option in dropdown                | minor  | GMT option allows users in Greenwich time to select their zone.                              | C3           |
| 7   | state       | Set default time to 9:00 AM on load                  | minor  | Default time gives users a starting point for conversions.                                   | None         |
| 8   | content     | Display label "PST time:" for Pacific conversion     | minor  | The label identifies the Pacific timezone conversion result.                                 | None         |
| 9   | content     | Display label "EST time:" for Eastern conversion     | minor  | The label identifies the Eastern timezone conversion result.                                 | None         |
| 10  | content     | Display label "GMT time:" for Greenwich conversion   | minor  | The label identifies the Greenwich timezone conversion result.                               | None         |
| 11  | state       | Calculate PST converted time from selected time/zone | major  | Converting to PST shows the meeting time for Pacific users.                                  | None         |
| 12  | state       | Calculate EST converted time from selected time/zone | major  | Converting to EST shows the meeting time for Eastern users.                                  | None         |
| 13  | state       | Calculate GMT converted time from selected time/zone | major  | Converting to GMT shows the meeting time for Greenwich users.                                | None         |
| 14  | content     | Display converted hour:minute for PST                | major  | Showing PST time gives users the converted meeting time.                                     | C11          |
| 15  | content     | Display converted hour:minute for EST                | major  | Showing EST time gives users the converted meeting time.                                     | C12          |
| 16  | content     | Display converted hour:minute for GMT                | major  | Showing GMT time gives users the converted meeting time.                                     | C13          |

## Justification

The meeting time zone converter works exactly as expected for scheduling across zones. A time picker labeled "Your time" displays with a dropdown showing three timezone options: "PST (UTC-8)", "EST (UTC-5)", and "GMT (UTC+0)". On load, the default time is 9:00 AM in all zones. When users select a time and timezone, the app calculates and displays three converted times below with labels "PST time:", "EST time:", and "GMT time:" showing the converted hour:minute values for each timezone.
