# RealTimeEHR: Dual-turn Text-to-SQL Dataset for Dynamic Electronic Health Records

## Overview
___
We introduce RealTimeEHR, a benchmark for temporal database state reasoning in medical text-to-SQL, comprising 2.2K dual-turn interactions constructed from three publicly available EHR databases, including MIMIC-III, MIMIC-IV, and eICU, where database states are separated by an average 1.45 hour interval. We construct the dataset through a multi-stage pipeline that transforms static queries into temporal progression scenarios where queries track accumulated information and detect updates between states.

## Dataset

The dataset contains the following fields:

- **scenario_id**: Unique identifier for each sample.
- **turn**: Indicates the turn number in the dual-turn interaction.
- **T1, T2**: Timestamps of the database snapshots.
- **question**: Natural language question.
- **query**: Corresponding SQL query.
- **sql_result**: Result of executing the SQL query.
- **answer**: Final answer to the question.
- **q_tag**: The question template.
- **value**: Sampled values from the database.