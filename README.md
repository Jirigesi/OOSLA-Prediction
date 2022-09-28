# OOSLA-Prediction


## Static features 

Static features extracted from bug reports are the most popular group of features for predicting bug resolution time, so we use prediction model built using static features introduced by Zhang et al.~\cite{zhang2013predicting} as the baseline. The static features contains the bug report Submitter, Owner, Severity, Priority, ESC indicating whether the bug is externally discovered (reported by end-users) or an internally discovered bug (reported by QA team), Category of the bug, and the Summary of the bug reports. 

Their F1 score was 0.728 to predict whether a bug report can be closed within the assigned time. The static features proposed by Zhang et al. included:

| **Feature name** | **Description**                                                                                                                    |
|------------------|------------------------------------------------------------------------------------------------------------------------------------|
| Submitter        | the bug report submitter                                                                                                           |
| Owner            | the developer who is responsible for resolving the bug.                                                                            |
| Severity         | the severity of a bug report                                                                                                       |
| Priority         | the priority of a bug report (Critical, Serious, Medium, Minor).                                                                   |
| ESC              | indicating whether the bug is externally discovered (reported by end-users) or an internally discovered bug (reported by QA team). |
| Category         | the category of the bug (such as Account management, Documentation, Configuration, etc.).                                          |
| Summary          | a short description of the bug.                                                                                                    |

## Dynamic and Contextual Features

The experimental results from Kikas et al.\cite{kikas2016using} indicate that their selected features outperformed existing prediction approaches. Thus, we consider contextual and dynamic features introduced by Kikas et al.\cite{kikas2016using} as another baseline for our evaluation. Below are the dynamic and contextual features that Kikas et al. used:

