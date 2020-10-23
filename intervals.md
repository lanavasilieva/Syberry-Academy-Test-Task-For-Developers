## Syberry Academy Test Task

**Task updated: Fri, October 23, 2020, 4:00 PM (GMT+3)** <br>
If you started your task **before** the latest update, we suggest you to go through the requirements once again! <br>
If you've found a mistake in task description, please don't hesitate to make a merge request! <br>

**A word of advice** <br>
In Academy we expect you to know how to read requirements and how to code in your language. <br>

To prove this ability in you, we ask you to implement this task and submit it via GitHub to confirm that you are ready to study in Academy. <br>

This task requires approximately 12 to 48 working hours to solve. It does not mean that **you** will solve it in 12-48 hours. It is ok to spend as many hours as you think is needed. <br>

We suggest you spend at least several hours reading the task and modeling the solution. We tested this task on our engineers: several Syberry Junior Developers on average spent 10 hours reading and thinking and approximately 2 hours of programming it.

### Task Deadline: 1 week
We start a countdown from the moment you clicked the "Registration" button on the Academy website. <br>
We accept applications before Friday, November 13, 2020, 11:59 PM (GMT+3)

### Applied Music Theory

In music theory, [an interval](https://en.wikipedia.org/wiki/Interval_(music)) is a distance between two notes. This distance is specified using a letter and a number. For example, valid names of intervals are M3, P5, or m7. The letter and the number in the interval name mean specific things.<br>

As in maths, if we're saying than the distance on a centimeter ruler between 3 and 5 is 2 centimeters, in music we're saying that the distance between C and E (or 'do' and 'mi') is M3. <br>

For the purpose of this task, we're using the following note names: <br>
C D E F G A B <br>

The whole list of intervals we're using in this task: <br>
m2, M2, m3, M3, P4, P5, m6, M6, m7, M7, P8 <br>

The number of an interval is the number of letter names or [staff positions](https://en.wikipedia.org/wiki/Staff_position) (lines and spaces) it contains, including the positions of both notes forming the interval. For instance, the interval C–G is a fifth (denoted P5) because the notes from C to the G above it contain five letter names (C, D, E, F, G) and occupy five consecutive staff positions, including the positions of C and G. The interval from A to A contains 8 notes (A B C D E F G A) and is called P8. We will call this number a **diatonic degree** (please note: the term 'degree' we are using here may not correspond to the actual term in music).<br>

The one unit of a distance between notes is called **a semitone**.<br>

Letter names can be modified by **the accidentals**. The **sharp '#'** raises a note by a semitone, and a **flat 'b'** lowers it by a semitone. You can add at most two sharp signs and two flat signs to the note.<br>

The following table shows 12 notes of a chromatic scale built on C. Distance between each note in a table is a semitone. Note that the same note can be described using different letters. For example, if we raise C by a semitone, we'll get C#. And if we lower D by a semitone, we'll get Db. <br>

C C#/Db D D#/Eb E F F#/Gb G G#/Ab A A#/Bb B <br>

For example, there are 4 semitones distance between C and E, 5 semitones distance between D and G, and 1 semitone distance between Bb and B. <br>

If we add any accidentals to the notes that form an interval, by definition the notes do not change their degree. As a consequence, any interval has the same interval number as the corresponding [natural interval](https://en.wikipedia.org/wiki/Natural_(music)) (means an interval formed by the same notes without accidentals). For instance, the intervals C–G# (spanning 8 semitones) and C#–G (spanning 6 semitones) are fifths, like the corresponding natural interval C–G (7 semitones). <br>

Notice that interval numbers represent an inclusive count of contained degrees or the note names, but not the difference between the endpoints. In other words, you count the first note as one, not zero. By this logic, the interval C–D is a second (M2), but D is only one degree above C. Similarly, C–E is a third (M3), but E is only two degrees above C, and so on. <br>

We will only use intervals up to an octave (P8, 12 semitones).  <br>

To build an interval from the given note, you first have to find a note diatonic degree lower or higher than a given note. <br>

Then you have to count the number of semitones from the starting note. In C D E F G A B sequence there is one semitone between E and F and B and C. Between other notes there are two semitones. <br>

Here one dash means one semitone: <br>
C--D--E-F--G--A--B-C <br>

**Example** <br>
Let's count the number of semitones between C and G: C to D - 2 semitones, D to E - 2 semitones, E to F - 1 semitone, F to G - 2 semitones. 2 + 2 + 1 + 2 = 7 semitones. <br>
Now let's find the number of semitones between A and C: A to B - 2 semitones, B to C - 1 semitone. 2 + 1 = 3 semitones. <br>

**Example** <br>
Now let's find our first interval - **P5 (perfect fifth) from Ab**. P5 means: find a distance of 5 degrees and 7 semitones. <br>
First, find the 5th degree from A, ignoring 'b': <br>
(A B C D E) - E is the 5th-degree note from A. <br>
Now count semitones: from Ab to B - 3 semitones (from Ab to A - 1 semitone, from A to B - 2 semitones), from B to C - 1 semitone, from C to  D - 2 semitones, from D to E - 2 semitones. 3 + 1 + 2 + 2 = 8 semitones. This is too much, we need only 7 semitones, but we need to stay on E. To do so, lower E by one semitone using accidental 'b'.<br>
**At P5 distance from Ab is the note Eb.** <br>
Note: you can't write D# as an answer, because even if D# is 7 semitones from Ab, it has a different degree (it takes only 4 degrees from A to D). <br>

**Example** <br>
To show you how to work with accidentals, let's **find P5 (5th degree, 7 semitones) from A#**: <br>
As in a previous example, find the 5th degree from A, ignoring '#': <br>
(A B C D E) - E is the 5th note from A (and from A#). <br>
Now count semitones: from A# to B - 1 semitone, from B to C - 1 semitone, from C to  D - 2 semitones, from D to E - 2 semitones. 1 + 1 + 2 + 2 = 6 semitones. We need to add just one semitone by adding #: E# <br>
**At P5 distance from A# is the note E#**. <br>

**Example** <br>
Let's find m2 (2nd degree, 1 semitone) from Fb:
To find a second degree is easy: (F G) - G is the second note from F. <br>
Now count semitones: from Fb to G is 3 semitones. This is way too much, we need just one. SO we have to lower G by 2 semitones. To do so, add two flat 'b' signs to G note: Gbb. <br>
**At m2 distance from Fb is the note Gbb**. <br>


**Intervals names, quality, and quantity** <br>
m2 - Minor Second - 1 semitone, 2 degrees <br>
M2 - Major Second - 2 semitones, 2 degrees <br>
m3 - Minor Third - 3 semitones, 3 degrees <br>
M3 - Major Third - 4 semitones, 3 degrees <br>
P4 - Perfect Fourth - 5 semitones, 4 degrees <br>
P5 - Perfect Fifth - 7 semitones, 5 degrees <br>
m6 - Minor Sixth - 8 semitones, 6 degrees <br>
M6 - Major Sixth - 9 semitones, 6 degrees <br>
m7 - Minor Seventh - 10 semitones, 7 degrees <br>
M7 - Major Seventh - 11 semitones, 7 degrees <br>
P8 - Perfect Octave - 12 semitones, 8 degrees <br>

Your task is to implement two functions that'll work with intervals: one will construct an interval and the second will identify the interval. <br>

### Requirements:
**intervalConstruction**
- The function 'intervalConstruction' must take an array of strings as input and return a string.
- An array contains three or two elements.
- The first element in an array is an interval name, the second is a starting note, and the third indicates whether an interval is ascending or descending.
- If there is no third element in an array, the building order is ascending by default.
- The function should return a string containing a note name.
- Only the following note names are allowed in a return string: <br>
Cbb Cb C C# C## Dbb Db D D# D## Ebb Eb E E# E## Fbb Fb F F# F## Gbb Gb G G# G## Abb Ab A A# A## Bbb Bb B B# B## <br>
- If there are more or fewer elements in the input array, an exception should be thrown: "Illegal number of elements in input array"

Convention: ['a', 'b'] here means an array of strings
<br>

**Input examples and meaning:** <br>
Please note: The data your function will get will look like an array of strings as defined in your language. No additional parsing is needed! The form ['', ''] is just a convention! <br>
The following notes are allowed in input: <br>
Cb C C# Db D D# Eb E E# Fb F F# Gb G G# Ab A A# Bb B B# <br>
The following intervals are allowed in input: <br>
m2 M2 m3 M3 P4 P5 m6 M6 m7 M7 P8 <br>
<br>
['M3', 'A', 'asc'] - build an ascending M3 interval starting from A <br>
['m7, 'Fb', 'dsc'] - build an descending m7 interval starting from Fb <br>
['P5', 'C'] - build an ascending P5 interval starting from C <br>
['P4', 'E#'] - build an ascending P4 interval starting from E# <br>

**intervalIdentification** <br>
- The function 'intervalIdentification' must take an array of strings as input and return a string.
- An array contains three or two elements.
- The first element is the first note in the interval, the second element is the last note in the interval, the third indicates whether an interval is ascending or descending.
- If there is no third element in an array, the interval is considered ascending by default.
- The function should return a string - name of the interval.
- Only the following intervals are allowed in a return string: <br>
m2 M2 m3 M3 P4 P5 m6 M6 m7 M7 P8
- If the interval does not fit a description, an exception should be thrown: "Cannot identify the interval".

Convention: ['a', 'b'] here means an array of strings
<br>

**Input examples and meaning:** <br>
Please note: The data your function will get will look like an array of strings as defined in your language. No additional parsing is needed! The form ['', ''] is just a convention! <br>
The following notes are allowed in input: <br>
Cbb Cb C C# C## Dbb Db D D# D## Ebb Eb E E# E## Fbb Fb F F# F## Gbb Gb G G# G## Abb Ab A A# A## Bbb Bb B B# B## <br>
<br>
['C', 'D'] - find an ascending interval between C and D <br>
['C#', 'Fb'] - find an ascending interval between C# and Fb <br>
['A', 'G#', 'asc'] - find an ascending interval between A and G# <br>

You may find [more examples here](examples.md). We will test your solution on this and similar examples.

### Language Specific Requirements
You 'MUST' use [predefined files and functions](predefined-files). **DO NOT CHANGE FILE NAME AND FUNCTIONS NAMES AND PARAMETERS**. <br>

**for Java** <br>
Class Name: `Intervals` <br>
Functions `intervalIdentification` and `intervalConstruction` `MUST` be static <br>
Do not add packages <br>
Java Version: 14 and older <br>
Do not use `System.out.*` or any other output methods<br>
Do not add packages <br>
Use [predefined file](predefined-files/Intervals.java) <br>

**for PHP** <br>
Do not use `echo` or `print` any other output methods<br>
Use [predefined file](predefined-files/intervals.php) <br>

**for JS** <br>
Do not use `console.log` or any other output methods <br>
Use [predefined file](predefined-files/intervals.js) <br>

### How to submit
- Create your personal private repository in GitHub. Name it Name-Surname-Academy-Test-Task. It is important to have your repository PRIVATE. We won't check solutions in the public repository.
- The end time is the time of your last commit in your repository.
- Submit one file named `intervals.js` (or `intervals.php`, `Intervals.java`). [Please find these files here](predefined-files).
- A file `MUST` contain two functions: intervalContruction() and intervalIdentification() [as defined here](predefined-files). You may add any other functionality to the file.
- We'll need read permission to your repository to check your solution. Add user SyberryAcademy to your repository as a Collaborator.
- Upload your CV to your repository.
- Send a link to your repository with solved task and CV to academy@syberry.com. Email subject: "Name Surname Syberry Academy %Specialization% %Language%" where %Specialization% is either BE or FE, and %Language% is the language you're using to solve our tasks. For example, "Jane Doe Syberry Academy BE Java"

### What's next
- If you did well on our task, our Recruiter will call you and invite you to a technical interview
- If not, we'll send you an email with your results and comments <br>
**We promise to reach you in 5 working days starting the day you sent us your email**

### Sanity Check: Please Double Check this Requirements
**The following requirements `MUST` be completed. If not, we won't check your task.**
- The `intervals.__` file `MUST` in your GitHub repository **in the root folder** (see example)
- Do not use output methods
- Your CV `MUST` be in your GitHub repository (see example)
```
Jane-Doe-Academy-Test-Task
    cv.md
    intervals.php
    README.md
```

```
Keanu-Reeves-Academy-Test-Task
    cv.txt
    Intervals.java
    README.md
```

```
Henry-Cavill-Academy-Test-Task
    cv.pdf
    intervals.js
    README.md
```
- The repository `MUST` be private
- User @SyberryAcademy `MUST` be added as a Developer
- Your CV may be in any form. Several lines about you in the .txt document will do

Good Luck and We hope to see You in Syberry Academy!
