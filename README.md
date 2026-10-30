# BiasAnalysis-edX_MOOC

This repository contains the code of the study presented in the paper *Pedro Manuel Moreno-Marcos, Alicia Ramirez-Arrabe, Carlos Alario-Hoyos, Pedro J. Muñoz-Merino, Iria Estévez-Ayres, and Carlos Delgado Kloos. 2026. Analysis of Bias in Student Modelling and Prediction Using Learning Analytics on edX MOOC Data. In Proceedings of the Learning Analytics Summer Institute Spain 2026, Zamora, Spain, May 2026 (LASI SPAIN '26)*.

## Overview

The paper analyzes possible biases that appear when estimating ability and difficulty of exercises with IRT, and when developing predictive models. The analyses were carried out using data from a MOOC about Java programming hosted in edX in a synchronous mode. The course was structured in five weeks, and each of them had a graded exam, with 5-8 exercises each. In addition, the course contained several videos per week and formative exercises (135 in total). In order to pass the course, students needed to get 60% of the points at least, and 88,324 users performed at least one action in the course.

The dataset was processed to extract the following independent variables:

- n_attempted: Total number of times students have attempted exercises.
- per_attempted: Percentage of problems attempted by a student over the total number of exercise.
- CFA: Percentage of exercises which the student has solved correctly on their first attempt.
- avg_attempts: Average number of attempts a student has taken in total to solve the exercises.
- avg_grade: Average grade of a student of the exercises they have attempted at least once.
- n_show: Total number of times a student asks for the solution of a problem to be shown.
- n_videos_watched: Total number of videos the student has watched.
- per_videos: Percentage of content visualized over the total.
- n_videos_opened: Number of times a student opened a video.
- n_pauses: Number of times a student paused a video.
- n_threads: Total number of threads created by a student.
- n_responses: Total number of responses posted by each student.
- n_days: Total number of comments posted by a student.

Moreover, two dependent variables were defined: dropout, which indicates whether or not the student has given up the course, and final_grade, which represents the final grade of each student.

## Repository structure

* Indicadores – processing and extraction of the dataset's independent variables.
* Abandono – computation of the dataset's dependent variable: students' dropout.
* Grades –  computation of the dataset's dependent variable: students' final grades.
* IRT – analyses made applying the Item Response Theory (IRT).
* Modelos - training and evaluation of the implemented predictive models.
  
## Acknowledgments

This work was supported by FEDER / Ministerio de Ciencia, Innovación y Universidades - Agencia Estatal de Investigación through the grant PID2023-146692OB-C31 (GENIE Learn project) funded by MICIU/AEI/10.13039/501100011033 and by ERDF/UE. Moreover, it received support from the UNESCO Chair of “Scalable Digital Education for All” at UC3M and by the grant RED2022-134284-T funded by MICIU/AEI/10.13039/501100011033.
