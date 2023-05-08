Download Link: https://assignmentchef.com/product/solved-solvedassignment-5-program-that-reads-an-input-data-set-consisting-of-four-parts-solution
<br>
Objectives:

· This assignment is to practice making hash tables.

Program Description

You will develop a C++ program that reads an input data set consistingof four parts: the first part is a hash table size entered by a user;the second part is a list of course numbers followed by its title; thethird part is an unordered list of course numbers; the fourth part is alist of course numbers with its title to delete. Not all course numbersin the third part or in the fourth part will match course numbers in thesecond part.

The first and second parts of the input will be separated by the word“Insertion”, the second and third parts of the input will be separatedby the word “Search”, and the third and fourth parts of the input willbe separate by the word “Delete” The fourth part ends with the linecontaining the word “Display”.The following shows a sample input:

/17InsertionFSE100/Introduction to EngineeringASU101/The ASU ExperienceENG101/First-Year CompositionENG102/First-Year CompositionPHY111/General Physics IPHY113/General Physics LaboratoryCSE310/Data Structures and AlgorithmCSE301/Computing EthicsENG108/First-Year CompositionENG200/Critical Reading &amp; Writing About LiteratureMAT243/Discrete Math StructuresMAT242/Elementary Linear AlgebraMAT201/Brief CalculusMAT265/Calculus for Engineers IPHY252/Physics IIIPHY101/Introduction to PhysicsCSE240/Introduction to Programming LanguagesCSE220/Programming for Computer EngineeringEEE120/Digital Design FundamentalsEEE230/Computer Organization and Assembly Language ProgrammingCHM116/General Chemistry IICHM113/General Chemistry ISearchFSE101EEE120ENG200MAT243PHY253DeleteMAT221/Brief CalculusEEE120/Digital Design FundamentalsASU102/The ASU ExperiencePHY101/Introduction to Mechanical EnergyCHM213/General Chemistry IIIPHY113/General Physics LaboratoryDisplay/

*Design Requirements:*

You need to create a hash table with chaining, which is an array oflinked lists. It utilizes memory efficiently. When hashing keys, keeptrack of the length of each linked list in the hash table, and thedifference of these lengths should be small in order to be efficient.You also need to define _a hash function_, _INSERT_,_SEARCH_, and_DELETE_ functions for the hash table.

For the INSERT function, add a new element at the beginning of a linkedlist where it is hashed so that it can be done in O(1).

Your program needs to read in the first input number and use it as thehash table size.

Each slot of your hash table should contain a linked list which isinitially empty (with its size 0). After processing and inserting thesecond part of the data into your hash table, print the content of thehash table using their index using the following format:

/ /

//

/index: 0, linked list size: 1Course Number: ENG200, Course Title: Critical Reading &amp; Writing About Literature

index: 1, linked list size: 3Course Number: EEE120, Course Title: Digital Design FundamentalsCourse Number: CSE220, Course Title: Programming for Computer EngineeringCourse Number: MAT201, Course Title: Brief Calculus

index: 2, linked list size: 1Course Number: CSE240, Course Title: Introduction to Programming Languages

index: 3, linked list size: 1Course Number: PHY252, Course Title: Physics III

index: 4, linked list size: 2Course Number: MAT242, Course Title: Elementary Linear AlgebraCourse Number: PHY111, Course Title: General Physics I

index: 5, linked list size: 3Course Number: MAT243, Course Title: Discrete Math StructuresCourse Number: CSE310, Course Title: Data Structures and AlgorithmCourse Number: ENG101, Course Title: First-Year Composition

index: 6, linked list size: 3Course Number: EEE230, Course Title: Computer Organization and Assembly Language ProgrammingCourse Number: PHY113, Course Title: General Physics LaboratoryCourse Number: ENG102, Course Title: First-Year Composition

index: 7, linked list size: 0The list is empty

index: 8, linked list size: 2Course Number: MAT265, Course Title: Calculus for Engineers ICourse Number: ASU101, Course Title: The ASU Experience

index: 9, linked list size: 0The list is empty

index: 10, linked list size: 0The list is empty

index: 11, linked list size: 2Course Number: CHM113, Course Title: General Chemistry ICourse Number: FSE100, Course Title: Introduction to Engineering

index: 12, linked list size: 2Course Number: PHY101, Course Title: Introduction to PhysicsCourse Number: ENG108, Course Title: First-Year Composition

index: 13, linked list size: 0The list is empty

index: 14, linked list size: 2Course Number: CHM116, Course Title: General Chemistry IICourse Number: CSE301, Course Title: Computing Ethics

index: 15, linked list size: 0The list is empty

index: 16, linked list size: 0The list is empty/

//

/ /

Then read the third part of the input, and search if each element withits course number in the hash table. If it exists, then print out itstitle and publisher, and if it does not exist, print the course numberand ”not found”:

//

/The course FSE101 not foundThe course EEE120 has the title: Digital Design FundamentalsThe course ENG200 has the title: Critical Reading &amp; Writing About LiteratureThe course MAT243 has the title: Discrete Math StructuresThe course PHY253 not found/

//

Then read the fourth part of the input, and search and delete if eachitem with exists in the hash table. If it exists, then print its coursenumber and course title, and ”is removed” such as below (if there aremore than one with the same set of course number and title, then removeall duplicates). If not, then print its course number and course title,and ”not found”:

//

/Course Number MAT221 with Title Brief Calculus not foundCourse Number EEE120 with Title Digital Design Fundamentals is removedCourse Number ASU102 with Title The ASU Experience not foundCourse Number PHY101 with Title Introduction to Mechanical Energy not foundCourse Number CHM213 with Title General Chemistry III not foundCourse Number PHY113 with Title General Physics Laboratory is removed/

//

After this, */print the updated hash table again/* using the same formatas the one used after the part 1.Please see the sample output file to format your output.

*Sample Run (user input is in bold):*

Please enter a hash table size:*17InsertionFSE100/Introduction to EngineeringASU101/The ASU ExperienceENG101/First-Year CompositionENG102/First-Year CompositionPHY111/General Physics IPHY113/General Physics LaboratoryCSE310/Data Structures and AlgorithmCSE301/Computing EthicsENG108/First-Year CompositionENG200/Critical Reading &amp; Writing About LiteratureMAT243/Discrete Math StructuresMAT242/Elementary Linear AlgebraMAT201/Brief CalculusMAT265/Calculus for Engineers IPHY252/Physics IIIPHY101/Introduction to PhysicsCSE240/Introduction to Programming LanguagesCSE220/Programming for Computer EngineeringEEE120/Digital Design FundamentalsEEE230/Computer Organization and Assembly Language ProgrammingCHM116/General Chemistry IICHM113/General Chemistry ISearch*index: 0, linked list size: 1Course Number: ENG200, Course Title: Critical Reading &amp; Writing AboutLiterature

index: 1, linked list size: 3Course Number: EEE120, Course Title: Digital Design FundamentalsCourse Number: CSE220, Course Title: Programming for Computer EngineeringCourse Number: MAT201, Course Title: Brief Calculus

index: 2, linked list size: 1Course Number: CSE240, Course Title: Introduction to Programming Languages

index: 3, linked list size: 1Course Number: PHY252, Course Title: Physics III

index: 4, linked list size: 2Course Number: MAT242, Course Title: Elementary Linear AlgebraCourse Number: PHY111, Course Title: General Physics I

index: 5, linked list size: 3Course Number: MAT243, Course Title: Discrete Math StructuresCourse Number: CSE310, Course Title: Data Structures and AlgorithmCourse Number: ENG101, Course Title: First-Year Composition

index: 6, linked list size: 3Course Number: EEE230, Course Title: Computer Organization and AssemblyLanguage ProgrammingCourse Number: PHY113, Course Title: General Physics LaboratoryCourse Number: ENG102, Course Title: First-Year Composition

index: 7, linked list size: 0The list is empty

index: 8, linked list size: 2Course Number: MAT265, Course Title: Calculus for Engineers ICourse Number: ASU101, Course Title: The ASU Experience

index: 9, linked list size: 0The list is empty

index: 10, linked list size: 0The list is empty

index: 11, linked list size: 2Course Number: CHM113, Course Title: General Chemistry ICourse Number: FSE100, Course Title: Introduction to Engineering

index: 12, linked list size: 2Course Number: PHY101, Course Title: Introduction to PhysicsCourse Number: ENG108, Course Title: First-Year Composition

index: 13, linked list size: 0The list is empty

index: 14, linked list size: 2Course Number: CHM116, Course Title: General Chemistry IICourse Number: CSE301, Course Title: Computing Ethics

index: 15, linked list size: 0The list is empty

index: 16, linked list size: 0The list is empty

*FSE101*The course FSE101 not found*EEE120*The course EEE120 has the title: Digital Design Fundamentals*ENG200*The course ENG200 has the title: Critical Reading &amp; Writing About Literature*MAT243*The course MAT243 has the title: Discrete Math Structures*PHY253*The course PHY253 not found*Delete*

*MAT221/Brief Calculus*Course Number MAT221 with Title Brief Calculus not found*EEE120/Digital Design Fundamentals*Course Number EEE120 with Title Digital Design Fundamentals is removed*ASU102/The ASU Experience*Course Number ASU102 with Title The ASU Experience not found*PHY101/Introduction to Mechanical Energy*Course Number PHY101 with Title Introduction to Mechanical Energy not found*CHM213/General Chemistry III*Course Number CHM213 with Title General Chemistry III not found*PHY113/General Physics Laboratory*Course Number PHY113 with Title General Physics Laboratory is removed*Display*

index: 0, linked list size: 1Course Number: ENG200, Course Title: Critical Reading &amp; Writing AboutLiterature

index: 1, linked list size: 2Course Number: CSE220, Course Title: Programming for Computer EngineeringCourse Number: MAT201, Course Title: Brief Calculus

index: 2, linked list size: 1Course Number: CSE240, Course Title: Introduction to Programming Languages

index: 3, linked list size: 1Course Number: PHY252, Course Title: Physics III

index: 4, linked list size: 2Course Number: MAT242, Course Title: Elementary Linear AlgebraCourse Number: PHY111, Course Title: General Physics I

index: 5, linked list size: 3Course Number: MAT243, Course Title: Discrete Math StructuresCourse Number: CSE310, Course Title: Data Structures and AlgorithmCourse Number: ENG101, Course Title: First-Year Composition

index: 6, linked list size: 2Course Number: EEE230, Course Title: Computer Organization and AssemblyLanguage ProgrammingCourse Number: ENG102, Course Title: First-Year Composition

index: 7, linked list size: 0The list is empty

index: 8, linked list size: 2Course Number: MAT265, Course Title: Calculus for Engineers ICourse Number: ASU101, Course Title: The ASU Experience

index: 9, linked list size: 0The list is empty

index: 10, linked list size: 0The list is empty

index: 11, linked list size: 2Course Number: CHM113, Course Title: General Chemistry ICourse Number: FSE100, Course Title: Introduction to Engineering

index: 12, linked list size: 2Course Number: PHY101, Course Title: Introduction to PhysicsCourse Number: ENG108, Course Title: First-Year Composition

index: 13, linked list size: 0The list is empty

index: 14, linked list size: 2Course Number: CHM116, Course Title: General Chemistry IICourse Number: CSE301, Course Title: Computing Ethics

index: 15, linked list size: 0The list is empty

index: 16, linked list size: 0The list is empty

* *

*Implementation/Documentation Requirements:*

* You need implement this program using C++ and it has to read fromthe standard input (from a keyboard).* Your program needs to compile and execute in general.asu.edu.* You need to define a LinkedList class with Insert, Search, andRemove functions (name them insertElement, searchElement, anddeleteElement) clearly in your code.* You need to define a HashTable class with Insert, Search, and Removefunctions (name them insertElement, searchElement, anddeleteElement), and a hash function /h/ clearly in your code. TheinsertElement function in HashTable class should call theinsertElement function in LinkedList class. The searchElementfunction in HashTable class should call the searchElement functionin LinkedList class. The deleteElement function in HashTable classshould call the deleteElement function in LinkedList class.* Your code should be well documented and commented.* You must use the provided data sets.* Also you are not allowed to use any predefined data structures (suchas ones in the library in C++, etc.) except arrays and strings, youneed to build your own data structures and operations associatedwith them (such as Insert or Search).* Copying any codes from other people’s programs is considered to becheating and will lead to a report to the Dean and you will bepenalized. Also check the rules stated in the syllabus of the courseregarding the academic integrity

*What to turn in:*

You must turn in C++ source code using the following submission site:

https://courses.eas.asu.edu/cse310/

First, you need to login, and click on the *Submission* page. You needto select the correct assignment number. The types of files that you cansubmit are .cpp, or .h files. They have to compile and execute in*/general.asu.edu/* server. (You can access general.asu.edu by SSH, andlogin using your ASU UserID and password.)

For C++, the files need to compile and execute with the commands:

/g++ *.cpp/

/./a.out/

You program should be well commented and documented, make sure the firstfew lines of your program contain your name, your ASU email address, anda description of each file. While you will not be graded on styletechnique (“i++” or “i = i + 1”) or indenting by 4 spaces or tabs, youshould use indentation, good variable names, and clear, easy to read,and specific comments. (You will be graded on comments.)

Input

The following files are sample test cases that will be used as input foryour program (Right-click and use “Save As”):

Test Case Input #1 &lt;assignment5/input1.txtTest Case Input #2 &lt;assignment5/input2.txtTest Case Input #3 &lt;assignment5/input3.txt

Test Case Output #1 &lt;assignment5/output1.txt

You can test your program as follows:

For a C++ program, after compiling your files, one way is:

/./a.out &lt; input1.txt/

or you can replace a.out with whichever your executable file is.

Error Handling

Your program will be tested with other input besides the ones above,thus is expected to be robust.