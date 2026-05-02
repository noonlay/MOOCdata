## Dataset Description

The KDDCUP2015 MOOC dataset is a public dataset for dropout prediction in online courses. It contains learner-course enrollment records, timestamped learning behavior logs, course object information, course date information, and final dropout labels.

In this study, the dataset is used to construct stage-based behavioral features for MOOC dropout prediction. Learner activities are aggregated at different learning stages to analyze how dropout-related behavioral patterns change over time.

## File Description

| File | Description |
|---|---|
| `enrollment_train.csv` / `enrollment_test.csv` | Enrollment information for each learner-course record, including `enrollment_id`, `username`, and `course_id`. |
| `log_train.csv` / `log_test.csv` | Timestamped learner behavior logs, including behavior time, event type, and related course object. |
| `truth_train.csv` / `truth_test.csv` | Dropout labels for learner-course records. |
| `object.csv` | Course object information, such as `course_id`, `module_id`, `category`, and other learning resources. |
| `date.csv` | Course start and end date information. |

## Learning Behavior Types

The original behavior logs include the following seven types of learning events:

| Event | Description |
|---|---|
| `problem` | Working on course assignments or problems. |
| `video` | Watching course videos. |
| `access` | Accessing course objects other than videos and assignments. |
| `wiki` | Accessing the course wiki. |
| `discussion` | Accessing the course forum or discussion area. |
| `navigate` | Navigating to another part of the course. |
| `page_close` | Closing the course webpage. |

## Label Description

The dropout label is stored in the `truth_train.csv` and `truth_test.csv` files.

| Label | Meaning |
|---|---|
| `1` | Dropout |
| `0` | Non-dropout / course completion |

Please note that the labels indicate the final course-level dropout status. They do not provide exact dropout times or week-specific dropout labels.
