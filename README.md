# Computational Geometry (CSCI 534), Spring 2023

Spatial data is everywhere.  How do we organize that data so that it can be
efficiently processed?  Moreover, how can we extract meaning out of this data?
Computational Geometry provides tools for solving these questions.  In this
class, we will study convex hulls, Delauney triangulations, Voronoi diagrams,
graph drawing, meshing, spatial decompositions, and many other geometric
techniques.  In addition, we will have opportunities to apply the techniques to
real world problems.

The techniques of computational geometry are very useful!  Indeed, they are part
of the algorithmic foundations of Graphics, Visualization, Data Mining,
Databases, Sensor Networks, Machine Learning, and Geographic Information
Systems.  They are also integral to simulation techniques used by Engineering,
Computational Physics and Biology... just to name a few.

Course Catalog Description: Techniques for storing, processing, and extracting
meaningful information from spatial data. In particular, we will focus on
efficiently solving problems about spatial relationships usually in low to
medium dimensions. Specific topics will include point location, triangulations,
and randomized incremental constructions.

## Prerequisities

This course assumes that you have the equivalent of an advanced undergraduate
knowledge of algorithms (or more).  In particular, we assume that you have
knowledge of: 

* Basic algorithm design techniques, such as divide-and-conquer, greedy
  algorithms, dynamic programming.
* Basic analysis techniques such as asymptotic notation, solving summations and
  recurrences, basic probability theory.
* Basic data structures (e.g. balanced binary trees, heaps, and hashing).
* Proof techniques (e.g., proof by induction).

## Meeting Times

Tue, Thurs 12:15 - 13:30 in Gaines 043 

## Instructor

Brittany Terese Fasy, Ph.D.

**Email**: brittany.fasy@montana.edu

**Office hours**: Thursdays 16:00-17:30, or by [appointment](https://montana.campus.eab.com/pal/vF_g0iza4n)

**Office**: Barnard 363, x4804

## Textbooks

Required:

* [David Mount's lecture notes](http://www.cs.umd.edu/class/fall2021/cmsc754/Lects/cmsc754-fall-2021-lects.pdf) (DMLN in reading below)

Optional but recommended:

* [Computational Geometry: Algorithms and Applications](https://link.springer.com/book/10.1007%2F978-3-540-77974-2) by Mark de Berg, Otfried Cheong, Marc van Kreveld, Mark Overmars (CGAA in reading below).
* [Discrete and Computational Geometry](https://press.princeton.edu/titles/9489.html) by Satyan L. Devadoss and Joseph O'Rourke (DO in reading below).
* [Computational Geometry in C (Second Edition)](https://cs.smith.edu/~jorourke/books/compgeom.html) by Joseph O'Rourke

More resources:

* [Introduction to
  Algorithms](http://mitpress.mit.edu/9780262046305/introduction-to-algorithms/)
  by Thomas H. Cormen, Charles E. Leiserson, Ronald L. Rivest and Clifford
  Stein.
* [Graph Drawing](https://www.pearson.com/us/higher-education/program/Tollis-Graph-Drawing-Algorithms-for-the-Visualization-of-Graphs/PGM36916.html) by Giuseppe Di Battista, Peter Eades, Roberto Tamassia, Ioannis G. Tollis.

## Land Acknowledgement

Living in Montana, we are on the ancestral lands of American Indians, including
the 12 tribal nations that call Montana home today: A’aninin (Gros Ventre),
Amskapi/Piikani (Blackfeet), Annishinabe (Chippewa/Ojibway), Annishinabe/Métis
(Little Shell Chippewa), Apsáalooke (Crow), Ktunaxa/Ksanka (Kootenai), Lakota,
Dakota (Sioux), Nakoda (Assiniboine), Ne-i-yah-wahk (Plains Cree), Qíispé (Pend
d’Oreille), Seliš (Salish), and Tsétsêhéstâhese/So’taahe (Northern Cheyenne).
We honor and respect these tribal nations as we live, work, learn, and play in
this state.

To learn more about Montana Indians, I suggest starting with the following
pamphlet:
[Essential Understandings Regarding Montana
Indians](http://opi.mt.gov/Portals/182/Page%20Files/Indian%20Education/Indian%20Education%20101/essentialunderstandings.pdf)


## What is in this repository?

The folders in this repository contain all materials for this class.

- lec_notes folder: Copies of lecture notes / board photos
- hw folder: homework assignments (in LaTex)
- project folder: requirements for the coures project
- README.md: this document. The syllabus
- Schedule: The schedule is at the bottom of this Markdown file.

## Creating Your Own Repository 

The repository is set as public, so you can access all course materials easily.
I suggest creating a private repository with this one setup as an upstream git
repo, so that you can use your repository to maintain your own materials for
this class. 

To do so, follow these instructions:
    
    - Going to <https://github.com/new>
    - Enter the name `csci-534-spring2023-NAME`
    - Select `Private`
    - **DO NOT ADD A README.MD or .gitignore!**

Once your repository is initialized, you can pull it down to your local machine.

Next, you should add the class repository as an upstream git repo:

```bash
$ git remote add upstream https://github.com/msu/csci-534-spring2023.git
$ git pull upstream main
$ git push
```
This will synchronize your private repository with the class repository.  You
only need to run these commands once.  Then, when you want to get an update from
the public class repository you can run this command:

```
$ git pull upstream main
```

As a general workflow on your own repository, I suggest:
```
$ git pull upstream master
[[ do work here ]]
$ git add [[ list filenames edited ]]
$ git commit -m "Descriptive message here"
$ git push origin main
```

## Grading

Your grade for this class will be determined by:

- 25% Homework Assignments (including the required (n+1)st)
- 50% Five Quizes (10-50 points each) and Final Exam (100 points)
- 25% Project

A grade of 70\% on the final exam is required to earn a B- or higher in the class.
and at least 55\% on the final exam is required to earn a C- or higher in the
class.

## Class Policies

### Policy on Class Attendance

Attendance will not be taken; however, class attendance and participation is
required to succeed in this class.  Please come to class prepared by reading and
working on homework problems throughout the week. 

### Policy on Homework Assignments

All homework assignments must be submitted by 23:59 on the due date. Late
assignments will not be accepted.

For descriptive assignments and reports, the submission should be typeset in
LaTex (use the assingment itself as a starting point!), and submitted as a PDF
to D2L. Each problem should be started on a fresh page.

For code assignments, well organized source code with clear comments should be
submitted as a zip file.  A README should be included in the directory.

***Do not search for answers to the problems.*** You will learn in this class by
solving the problems, not by reading the solutions. Regurgitating solutions you
found elsewhere will not help you learn the material.  If you feel that you need
additional resources, please ask.

The following are the assignments that count towards the Homework grade:

- assigned homeworks: there will be about six standard homework assignments
  (some may be group assignments).
- (n+1)st assignment: Write a two-page paper describing to me how you have grown
  as a computer scientist, mathematician, and/or a researcher in this class, and
  more generally, in this semester.  To support your argument, you should
  include your homework (or excerpts from your homework) in an appendix as
  evidence (and reference them!) If you do not feel that you've grown as a
  computer scientist, mathematician, or researcher, explain why.  Remember,
  style counts. Due: End of day on final exam day.

Grading of homeworks: Each homework question will be graded on the following
scale: incomplete, low pass, pass, high pass. These problem grades will be used
to calculate an overall letter grade (e.g., all HP=A+) for the assignment. This
might take time to adjust to, but hopefully it takes the focus away from the
grade itself and allows you to focus on learning the material.

### Class Project

If your project overlaps with other classes or your paid research hours,
please discuss with me.  This is ok, but some line will need to be drawn to
differentiate this course project from your other projects.  And, approval from
the other instructor / research adviser will need to be ensured.

### Policy on Collaboration

Collaboration is encouraged on all aspects of the class, except where explicitly
forbidden. Note:

- All collaboration (who and what) must be clearly indicated in writing on
  anything turned in.
- Homework may be solved collaboratively except as explicitly forbidden (quizzes
  and exams), but solutions must be written up **independently**.  This is best
  done by writing your solutions when not in a group setting.  Groups should be
  small enough that each member plays a significant role.  (Note, if there is a
  group assignment, each group is treated as an 'individual'.

### Classroom Etiquette

** In person: **
Except for note taking and group work requiring a computer, please keep
electronic devices off during class, as they can be distractions to other
students. Disruptions to the class will result in being asked to leave the
lecture.

** Online: **
Due to travel or illness, we may need to meet via Zoom a couple times during
this semester.  In the Zoom breakout rooms, we
expect that you are actively working on problems.  If needed, start your group
by recapping what was discussed right before going into the breakout room or
during the class period before.  If something is unclear, ask for a
clarification from your classmate.  If your group is unsure of what the task is,
please ask and do not sit idle!

### Withdrawing

After 15 March 2022, I will only support requests to withdraw from this course
with a ``W" grade if extraordinary personal circumstances exist.
If you are considering withdrawing from this class, discussing this with me as
early as possible is advised.  Since this class involves a project, the
decision to withdraw must be discussed with me, and with your group.

### Special Needs Information

If you have a documented disability for which you are or may be requesting an
accommodation(s), please contact me and Disabled Student Services before the
third class meeting.

### Diversity Statement

Montana State University considers the diversity of its students, faculty, and
staff to be a strength and critical to its educational mission. MSU expects
every member of the university community to contribute to an inclusive and
respectful culture for all in its classrooms, work environments, and at campus
events.  Dimensions of diversity can include sex, race, age, national origin,
ethnicity, gender identity and expression, intellectual and physical ability,
sexual orientation, income, faith and non-faith perspectives, socio-economic
status, political ideology, education, primary language, family status, military
experience, cognitive style, and communication style. The individual
intersection of these experiences and characteristics must be valued in our
community.

If there are aspects of the design, instruction, and/or experiences within this
course that result in barriers to your inclusion or accurate assessment of
achievement, please notify the instructor as soon as possible and/or contact
Disability Services or the Office of Institutional Equity.

## MSU Policies

### Academic Integrity

The integrity of the academic process requires that credit be given where credit
is due. Accordingly, it is academic misconduct to present the ideas or works of
another as one's own work, or to permit another to present one's work without
customary and proper acknowledgment of authorship. Students may collaborate with
other students only as expressly permitted by the instructor. Students are
responsible for the honest completion and representation of their work, the
appropriate citation of sources and the respect and recognition of others'
academic endeavors.

Plagiarism will not be tolerated in this course. According to the Meriam-Webster
dictionary, plagiarism is `the act of using another person's words or ideas
without giving credit to that person.'  Proper credit means describing all
outside resources (conversations, websites, etc.), and explaining the extent to
which the resource was used.  Penalties for plagiarism at MSU include (but are
not limited to) failing the assignment, failing the class, or having your degree
revoked.  This is serious, so do not plagiarize.
Even inadvertent or unintentional misuse or appropriation of another's work
(such as relying heavily on source material that is not expressly acknowledged)
is considered plagiarism. 

By participating in this class, you agree to abide by the Student Code of
Conduct.  This includes the following academic expectations:

- be prompt and regular in attending classes;
- be well-prepared for classes;
- submit required assignments in a timely manner;
- take exams when scheduled, unless rescheduled under 310.01;
- act in a respectful manner toward other students and the instructor and in a way
          that does not detract from the learning experience; and
- make and keep appointments when necessary to meet with the instructor. 

### MSU Drug and Alcohol Policies

Per the Code of Conduct for students, no student may come to class under the
influence of drugs or alcohol, as that would not be `Fostering a healthy, safe
and productive campus and community.`  See [Alcohol and Drug Policies
Website](http://www.montana.edu/deanofstudents/alcoholanddrugs.html) for more
information.  In particular, note:

As a federally-funded institution, we must adhere to all federal laws when it
comes to alcohol and drug use or distribution. This holds true for marijuana as
well. Using or distributing marijuana on or off campus is a violation of our
code of conduct even if a student has a medical card or comes from a state in
which marijuana is legal or has been decriminalized.

## Class Schedule

The lecture schedule is subject to change and will be updated throughout the semester.

| Date | Description               | Quiz             | HW Due    |  Proj     | Recommended Reading                   |
|------|---------------------------|------------------|-----------|-----------|---------------------------------------|
| 1/19 | Intro to CG               |                  |           |           | DMLN L1, CGAA 1                       |
| 1/24 | Convex Hulls              |                  |           |           | DMLN L2, CGAA 1.1                     |
| 1/26 | Convex Hulls II           |                  |           |           | DMLN L2, CGAA 1.1                     |
| 1/31 | Output-Sensitive CH       | Q1               |           |           | DMLN L3                               |
| 2/2  | Segment Intersection I    |                  | HW1       |           | DMLN L4, CGAA 2.1                     |
| 2/7  | Segment Intersection II   |                  |           |           | DMLN L4, CGAA 2.1                     |
| 2/9  | Triangulations            | Q2               |           |           | DMLN L5, CGAA 3.2                     |
| 2/14 | DCEL DS / triangulate     |                  |           |           | [DCEL](https://en.wikipedia.org/wiki/Doubly_connected_edge_list) and [Quad Edge](https://www.cs.cmu.edu/afs/andrew/scs/cs/15-463/2001/pub/src/a2/quadedge.html) |
| 2/16 | Triangulating & Guarding  |                  |           |           | DMLN L5, CGAA 3.1-2                   |
| 2/21 | Halfplanes and Duality    |                  |           |           | DMLN L6, CGAA 4.2                     |
| 2/23 | Linear Programming        |                  | HW2       |           | DMLN L7, CGAA 4.3-6                   |
| 2/28 | Trapezoidations I         | Q3               |           |           |                                       |
| 3/2  | Trapezoidations II        |                  |           |           |                                       |
| 3/7  | Point Location            |                  | HW3       |           |                                       |
| 3/9  | Project Proposals         |                  |           |           |                                       |
| 3/14 | SPRING BREAK!             |                  |           |           |                                       |
| 3/16 | SPRING BREAK!             |                  |           |           |                                       |

Potential upcoming topics:

* Polygonal Triangulations and Guarding (DMLN L5, CGAA 3.1-.2)
* Halfplane Intersection and Duality (DMLN L6, CGAA 4.2)
* Linear Programming (DMLN L7, CGAA 4.3-.6)
* Trapezoidations (DMLN L8, CGAA 6.1-.2)
* Point Location (DMLN L9)
* Voronoi Diagrams (DMLN L10, CGAA 7.1-.2)
* Delaunay Triangulations (DMLN L11-12, CGAA 9.1-.4)
* Arrangements (DMLN L13, CGAA 8.3-4)
* Range Searches (DMLN L14)
* Well-Separated Pair Decompositions (DMLN L15)
* (alternate) Coresets and Kernels (DMLN L16)
* (alternate) Sampling and VC Dimension (DMLN L17)
* (alternate) Motion Planning (DMLN L18, CGAA 13)
* (alternate) Medial Axis (DO 5.1-.2)

## Acknowledgements

I have borrowed materials for this class from Computational Geometry classes
previously taught here and elsewhere.  Thanks especially to David Millman, David
Mount, and Carola Wenk for making their materials available.
