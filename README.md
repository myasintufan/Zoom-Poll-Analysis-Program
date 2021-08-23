# Zoom-Poll-Analyzes-Program

Vision

The objective of the this project is to create a Python based object oriented implementation of
Evaluation of Poll Reports that are done during the course meeting in Fall 2020-2021
semester.
The project has two main iterations. According to the demands and feedback of the customer,
necessary changes and developments is made in the project.

Scope

During the online courses, ZOOM Polls are used to track the performance of the students.
These polls include one or more questions that are determined by the instructor. The questions
can be quizzes related to the course topics or they can be asked only to evaluate participation
to course. So, a quiz can be defined as the application of a poll in a meeting/lecture. The
courses’ instructor download a poll report after the meeting in csv file format. Also, a unique
key for a quiz can be constructed by combining poll name with the date time information when it is
applied.
For this reason, this python project is developed for processing and analyzing these Zoom
polls. The example poll reports that are done during the course and student list that contain
students taking the course are provided by instructor.
A detailed report was prepared in which the lecturer could see the attendance rate of the
students and the success rates of each student in the quiz throughout the semester.

Glossary Of Terms

Student List: Includes the all students that take the course during the Fall 2020-2021
semester.
Student: Each of the students whose progress and absenteeism is wanted to be evaluated.
Result: Includes quiz results for each student.
Question: Contains question asked in the poll and answers for each question.
Poll: Done for checking the student's progress in the course given throughout the semester. It
includes questions that are determined by course’s instructor before the course.
Report: The text file in csv file format. The fields are seperated by comma. This text file can
be for quiz or attendance.
Attendance: Uses for finding the total number of classes the student attended during the
semester.
GlobalResults: Includes total result of polls that is done during the semester for each student

Functional Requirements

 There may be several polls in a given day. The results of each quiz should be
evaluated and reported separately
 A poll can consist of a maximum of 10 questions.
 A poll defined for a recurring meeting can be open in any occurrences of these
meetings/lectures.
 The same poll can be given to the students in different meetings/lectures. If the same
poll is given to the students in different meetings/lectures, these polls will be
considered as different quizzes in grading of each student.
 The zoom poll names are not included in the report files. Poll names only exist in
answer key files. From the poll report, meeting name should be extracted and then
answer key of the poll should be found in answer key file.
 A single ZOOM poll report may include more than one poll results that are done in a
particular day/session.
 The quizzes can be distiguished from attendance polls by the number of questions. If a
poll has only one question with only two options such as yes and no, you may decide
that this is an attendance poll and will not be graded, but will be used merely as
counting attendance.
 If the poll does not exist in answer keys files then it is an attendance poll. 
 In a particular day, if there is no attendance poll but there is at least a quiz, then all the
students who participated at least one of these quizzes will be counted as attended the
class that day.
 Some questions may exist in several polls.
 In each exam report "number of questions", "number of questions answered correctly",
"number of questions answered incorrectly", "number of empty questions", "number
of questions answered correctly" (number of correctly answered questions / number of
questions total questionnaire), "percentage of accuracy" (ratio of correctly answered
questions * 100) should be found.
 The results of each poll should be calculated in spreadsheet files (.xlsx or .ods). The
file name should be the name of the poll (replace white space and punctuation with _)
plus poll date time.
 A detailed reports should be prepared for each student for quizzes. For each poll report
the answers of each student along with the correct answers for each question. The file
name should include the poll name, date it is applied and the student name and number
from BYS list . Fields should be "question text", "given answer", "correct answer",
"Correct (1 or 0)". For the last column, if the given answer matches the correct answer
then put 1 in here, otherwise put 0.
 Global analytics file should be prepared. Name of the file will consist of class code
and semester. This will be a single open document spreadsheet or excel file including
all the students in the BYS list in the order given in BYS list. The columns include
"index" (from 1 to number of students), "student number", "student full name". After
this column list each quiz as a column with quiz name and given date ordered by the
date ascending. The values will be the number of correctly answered questions by this
student for this quiz. As the last column ,a global accuracy should be calculated for
each student: "The total number of correctly answered questions in all quizzes" /
"Total number of questions in all quizzes" * 100.

 Non-Functional Requirements

 A single zoom poll report should be as a csv file format or a folder containing several
.csv files as input.
 The .csv file includes some attributes such as user name, user email, submitted date
and time.
 A single answer key or a folder containing several answer keys of different polls
should be taken. An answer key file should be also a csv or an excel file. First line
should includes a unique name of the poll. Following lines should includes two fields;
question text and correct choice text.
 A student list in the format should be provided as an excel file.
 After each iteration ,some measurement should be done according to the metrics
which are given by instructor.
 All works related to the projects should be submitted to github as a control and sharing
mechanism
