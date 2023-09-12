## Participants

The study participants included 8 women and 2 men for fall activities and daily activities (ADL) except activities 5 and 6 (stairs), which included 9 women and 1 man. The average age, height, and weight of the participants were 32.80 ± 10.86, (167.20 ± 8.98) cm, (61.40 ± 7.55) kg, respectively, for falls and ADL except ADL 5 and 6, which, in correspondence, had average age, height and weight of 36.7 ± 10.82, (165.4 ± 6.62) cm and (66 ± 19.67) kg.

## Procedure

The smartwatches were positioned on the left and right wrists of each participant. Both acceleration and location tags were positioned on a belt inside a MOLLE (Modular Lightweight Load-carrying Equipment) between the participant's waist and higher hips.

For the fall activities which included human participants, safety mattresses were used to dampen falls (see reference videos). Mannequin falls included professional fall arrest equipment.

## List of activities

### Falls from height (mannequin falls)

| Activity | Description | Duration (s) |
| --- | --- | --- |
| 1 | Fall forward from height. Vertical starting position, front attachment point of a harness | 20 |
| 2 | Fall forward from height. Vertical starting position, back attachment point of a harness | 20 |
| 3 | Fall forward from height. Forward tilt mannequin starting point, back attachment point of a harness | 20 |
| 4 | Fall backward from height. Tilt backwards mannequin starting position, front attachment point of a harness | 20 |

### Surface falls (perfromed by human participants)

| Activity | Description | Repetitions | Duration (s) |
| --- | --- | --- |  --- |
| 1 | Fall forward while walking | 5 | 25 |
| 2 | Fall backward while standing | 5 | 25 |
| 3 | Lateral fall while walking | 6 (three to the left side and 3 to the right) | 25 |
| 4 | Fall forward while jogging | 5 | 25 |
| 5 | Vertical fall caused by fainting | 5 | 25 |
| 6 | Fall backward when trying to sit down | 5 | 25 |
| 6 | Forward fall to the knees then to the ground | 5 | 25 |

During each fall activity, 3 out of 5 falls ended in ~10 seconds of immobility, when participant layed on the mattress (in 4 out of 6 - two per side - in case of lateral falls). The rest of the falls ended in participant making movements resembling those of a person who tries to get up.

### Activities of daily living

| Activity | Description | Repetitions | Duration (s) |
| --- | --- | --- |  --- |
| 1 | Walking slowly | 3 | 60* |
| 2 | Walking quickly | 3 | 60 |
| 3 | Jogging slowly | 3 | 60 |
| 4 | Jogging quickly | 3 | 60 |
| 5 | Walking upstairs and downstairs slowly | 5 | 35 |
| 6 | Walking upstairs and downstairs quickly | 5 | 25 |
| 7 | Sit in a half-height chair, wait a moment, and up slowly | 5 | 20 |
| 8 | Slowly sit in a low height chair, wait a moment, and up slowly | 5 | 25 |
| 9 | Quickly sit in a low height chair, wait a moment, and up quickly | 5 | 15 |
| 10 | Sitting a moment, trying to get up, and collapse into a chair | 5 | 10 |
| 11 | Sitting a moment, lying slowly, wait a moment, and sit again | 5 | 20 |
| 12 | Sitting a moment, lying quickly, wait a moment, and sit again | 5 | 15 |
| 13 | Standing, slowly bending at knees, and getting up | 5 | 10 |
| 14 | Standing, slowly bending without bending knees, and getting up | 5 | 10 |
| 15 | Stumble while walking | 5 | 10 |
| 16 | Gently jump without falling (trying to reach a high object) | 5 | 5 |
| 17 | Crawling | 5 | 15 |
| 18 | Jumping, standing on the same place (multiple times during one trial) | 5 | 15 |
| 18 | Raise two hands into the air (3 times during one trial) | 5 | 10 |

*For participant 1, walking and jogging duration is 100 seconds.

### Immobility

| Activity | Description | Repetitions | Duration (s) |
| --- | --- | --- |  --- |
| 1 | Lying on one’s back | 3 | 30 |
| 2 | Lying on one’s stomach | 3 | 30 |

## Dataset organisation
### Accleration
SET - where data was collected (mannequin lab\lab\stairs)
PARTICIPANT - participant identifier inside SET
TIMESTAMP - timestamp in format: %Y-%m-%d %H:%M:%S.%f
SOURCE - device reporting: TAG/WATCH_R/WATCH_L
X - value axis X
Y - value axis Y
Z - value axis Z
TYPE - type of activity, M - mannequin fall, F - surface fall, A - ADL, I - immobility
ACTIVITY - activity number as in activities table description
IS_FALL - 0/1 target variable, indicating a 3s region around a fall

### Location
SET - where data was collected (mannequin lab\lab\stairs)
PARTICIPANT - participant identifier inside SET
TIMESTAMP - timestamp in format: %Y-%m-%d %H:%M:%S.%f
TYPE - type of activity, M - mannequin fall; F - surface fall; A - ADL; I - immobility
ACTIVITY - activity number as in activities table description
IS_FALL - 0/1 target variable, indicating a 3s region around a fall
RANGE_{NUM} - distance to anchor NUM, where NUM is 1, 2, 3, 4
X, Y, Z – tag coordinates in meters
LOC_MODE – localization mode: 3D – 3D localization with 4 anchors; 2D_AVG – average of at least two 2D localizations (needs 4 anchors, each part of the average computed with 3 anchors); 2D – 2D localization with 3 anchors; APPROX – approximate location based only on the nearest anchor; NONE – no location solution could be found (either too large measurement error, or too few seen anchors)
LOC_ANCHORS – number of anchors seen by the tag
LOC_ACCURACY – radius of the sphere within which the tag is. Only used in the APPROX mode, in all other modes it is always 0

## Notes from data collection

| Type | Participant | Activity | Note |
| --- | --- | --- | --- |
| A | 9 | 5 | connection to smartwatches(R/L) was lost at 14:06:21/14:06:23 and experiment continued after it was restored at 14:06:49/14:07:02 |
| A | 3 | 6 | lost connection to smartwatches(R/L) at 12:30:36/12:30:33 and experiment continued at 12:31:08/12:30:58 - has 6 down/up flights |
| A | 2 | 5 | has 2 sets of experiments |
| M | 1 | 4 | mannequin bent its knees and the feet remained on the support |
| A | 5 | 13 | participant was moving for better view on camera and moved a chair around 14:03:44 - 14:04:02 |
| A | 4 | 4 | participant practiced more movements for fast joggging after the first attempt 11:41:38 - 11:42:26 |
| A | 3 | 10 | participants made a valid test collapsing onto the hair, so it was included into the data |
| A | 1 | 18 | additional multiple jumps |
| A | 1 | 1 | activity was performed for 100 seconds |
| A | 1 | 2 | activity was performed for 100 seconds |
| A | 4 | 6 | lost smartwatches (R/L) connection at 12:57:07/12:57:10, 12:58:12/12:58:14 and 12:59:53/12:59:51 continued at 12:57:38/12:57:28, 12:58:50/12:58:36, 13:00:57/13:00:13 and left only smartwatch was lost 13:00:29 and restored at 13:00:46|
| A | 4 | 5 | lost smartwatches (R/L) connection at 12:48:04/12:48:03 and restored at 12:48:34/12:48:24 |
| A | 6 | 2 | there is a ~1 minute pause between the second and the third attempts |
| F | 6 | 5 | harsh step down from the mattress around 11:00:25|
| F | 5 | 6 | participant wasn't laying still after the first fall, experiment was repeated |
| F | 3 | 3 | second lateral fall was more like forward one, so it was repeated |
| F | 3 | 4 | during the third fall participant fell first to the knee, so it was repeated |
| A | 3 | 2 | a pause between 09:41:49 till 09:43:45 |
| F | 2 | 6 | after first fall participant was making themselves comfortable with the devices 11:41:07 - 11:41:24 |
| F | 2 | 1 | has the first test forward fall with reduced immobility time |
| F | 1 | 7 | has 4 falls with no movements |
| F | 1 | 2 | a pause between 13:39:50 and 13:40:40 |
| F | 1 | 4 | a test almost-fall at 13:29:57 (not labeled as a fall), 6 falls in total, fifth fall at 13:31:58 was interfered by a knee|
| A | 1 | 15 | 7 (6 and a mild one) stumbles|
| F | 10 | 4 | 10:50:31 - tying shoelaces, 10:49:06 - getting up from the matress |
| F | 10 | 3 | lost connection with tags right after the fall at 10:53:37, restored at 10:53:44, fall was repeated from 11:05:24 |
| A | 10 | 15 | 6 stumbles |
| A | 2 | 18 | first jumps had a sequence of 20+ jumps |
| F | 4 | 6 | 12:47:29 - laid down on a matress fast, 6 falls in total |
| F | 1 | 2 | 13:39:46 - standing up from the mattress reported high acceleration |
| F | 5 | 1, 3, 4 | tags were upside-down, but still in the front of the subject, adapted in acceleration data |
| F | 9 | 5 | quick step down from the matress around 12:22:45 |
| A | 2, 4, 8, 10 | 5 | has 6 down/up flights |
| A | 3, 5, 8 | 6 | has 6 down/up flights |
| A | 7 | 6 | connection to r/l smartwatches lost at 13:43:14/13:43:16 and 13:44:15/13:44:18, restored at 13:43:46/13:43:36 and 13:44:52/13:44:39 |
| F | 4 | 1 | lost tag after the second fall 12:31:49 continued at 12:33:23|
| F | 8 | 7 | lost tag at 10:25:16, continued at 10:40:59, lost tag at 10:42:38, continued at 10:47:00 | 

### Other notes:
- participant 7 has no immobility data

## Anchors location

### Mannequin falls

| Anchor | X | Y | Z |
| --- | --- | --- | --- |
| 1 | 0.0 |3.26 | 5.60 |
| 2 | 0.15 | 3.26 | 0.115 |
| 3 | 2.28 | 0.0 | 2.21 |
| 4 | 3.11 | 4.41 | 1.86 |

### Lab 

| Anchor | X | Y | Z |
| --- | --- | --- | --- |
| 1 | 0.12 | 9.24 | 2.41 |
| 2 | 0.0 | 0.0 | 0.19 |
| 3 | 3.57 | 9.24 | 2.43 |
| 4 | 3.40 | 1.75 | 2.10 |

### Stairs

| Anchor | X | Y | Z |
| --- | --- | --- | --- |
| 1 | 2.32 | 3.95 | 4.90 |
| 2 | 0.0 | 0.0 | 0.0 |
| 3 | 0.01 | 3.95 | 4.80 |
| 4 | 2.34 | 0.30 | 5.37 |

