Download Link: https://assignmentchef.com/product/solved-ch-230-a-assignment-11-dynamic-memory-allocation-and-inheritance
<br>
<h1>Problem 11.1 <em>Boxes                                                                                                     </em>(</h1>

Design and write an object oriented program for the computation of the volume of boxes (having a height, a width and a depth as double values). Your solution should have methods for setting and getting the height, the width and the depth of a box as well as constructors (a default constructor and one which sets the data members), a copy constructor and a destructor.

Name your files testbox.cpp, Box.cpp and Box.h.

The program testing your code (testbox.cpp) should do the following:

<ol>

 <li>Enter from the keyboard the a value for n, the number of boxes that will be entered.</li>

 <li>Dynamically create an array of 2<sup>∗</sup>n boxes.</li>

 <li>Enter from the keyboard the height, width and depth of each box one after the other for thefirst n boxes and the add their copies on the remainder n positions (in the same order). Use the copy constructor for doing this.</li>

 <li>Loop across all boxes, calculate and print on the screen the volume of each box.</li>

</ol>

<em>You can assume that the input will be valid.</em>

<table width="457">

 <tbody>

  <tr>

   <td width="457"><strong>Problem 11.2 </strong><em>Inheritance with creatures</em></td>

  </tr>

 </tbody>

</table>

Extend the example program creature.cpp by adding two other type of creatures (i.e., two new classes derived from Creature) with some example properties and methods (use your imagination for doing this). Use/implement at least one property and at least one method for each derived class.

Each constructor, destructor and method should be implemented in such a way that each call is being documented via messages printed on the screen.

Create one instance of Wizard, two instances of the two other classes, and call for each object methods of the particular instances (as in the original example). <em>You can assume that the setting values are always valid.</em>

<strong>Problem 11.3 </strong><em>Inheritance split code                                                                            </em>

Reorganize your previous file’s (creature.cpp) content into three parts: declaration, implementation of the classes and your test program. Name the files Creature.h, Creature.cpp and testcreature.cpp.

<table width="371">

 <tbody>

  <tr>

   <td width="371"><strong>Problem 11.4 </strong><em>Inheritance and pointers</em></td>

  </tr>

  <tr>

   <td width="371"> </td>

  </tr>

 </tbody>

</table>

<h2>Language: C++</h2>

Change your previous testing program (testcreature.cpp) such that it runs in an endless loop and waits for input from the keyboard. If the word ”wizard”, ”object1”, or ”object2” is entered, a wizard, your other object1 or your other object2 should be dynamically created (via new), the corresponding method is being called and the object is then destroyed (via delete). Entering “quit” should stop the execution of the program.

Name the files Creature.h (same as above), Creature.cpp (same as above) and dyncreature.cpp.

<em>You can assume that the input will be valid.</em>

<table width="370">

 <tbody>

  <tr>

   <td width="370"><strong>Problem 11.5 </strong><em>Shapes</em></td>

  </tr>

  <tr>

   <td width="370"> </td>

  </tr>

 </tbody>

</table>

Extend the Shapes example by adding two new classes Rectangle and Square according to the following inheritance diagram.

Implement the following:

<ol>

 <li>default constructors for all classes by initializing the properties to default values,</li>

 <li>setters and getters for all classes,</li>

 <li>the constructors Rectangle(const string&amp; n, double nx, double ny, double nwidth,</li>

</ol>

double nheight) and Square(const string&amp; n, double nx, double ny, double nside), d) copy constructors for all classes,

<ol>

 <li>the methods double perimeter() and double area() for the classes Circle, Rectangle and Square for returning the perimeter and area of corresponding instances,</li>

 <li>in your testing program create instances of Circle, Rectangle and Square, and then compute and print on the screen their perimeter and area.</li>

</ol>

Name your files Shapes.h, Shapes.cpp and testshapes.cpp.

<em>You can assume that the setting values are always valid.</em>

<table width="428">

 <tbody>

  <tr>

   <td width="428"><strong>Problem 11.6 </strong><em>A Vector class for doubles</em></td>

  </tr>

 </tbody>

</table>

<h2>Language: C++</h2>

Create a class named Vector for storing and managing vectors of doubles. The properties of a vector are the size of the vector and a double pointer pointing to a memory location where the components of the vector are stored. The class has to provide a default constructor, another constructor for setting the properties, a copy constructor and a destructor. The non-default constructors should dynamically allocate memory for a vector and the destructor should release it.

Provide suitable setter and getter methods for each property and a method for printing the components of a vector on the screen separated by spaces. Also provide methods for computing the norm of a vector, the sum, the difference and the scalar product of two vectors. The class declaration has to be placed into Vector.h, the class definition has to be placed into Vector.cpp and the test program where the instances are created has to be in testvector.cpp. The test program should create four instances of the Vector class using the different constructors (the constructor without parameters, parametric constructor and copy constructor). The third instance should be the copy of the second one). The fourth instance should be created with parameters as well. Then the norm of the second vector should be computed and printed on the screen, the scalar product, the sum and the difference of the second and fourth vectors should be also computed and printed on the screen.

Use the const modifier properly for parameters and methods.

<em>You can assume that the input or the setting values are valid. </em>The prototypes should have the following form:

double norm();

Vector add(const Vector) const; The usage should be:

Vector v1, v2;

(v1.add(v2)).print();

<em>Note: </em>If <em>v</em><sub>1 </sub>= (<em>a</em><sub>1</sub><em>,a</em><sub>2</sub><em>,…,a<sub>n</sub></em>) and <em>v</em><sub>2 </sub>= (<em>b</em><sub>1</sub><em>,b</em><sub>2</sub><em>,…,b<sub>n</sub></em>) with <em>n </em>∈ N<sup>∗</sup>. Then:

(the norm of a vector),

<em>n</em>

<em>v</em><sub>1 </sub>· <em>v</em><sub>2 </sub>= <sup>P </sup><em>a<sub>i </sub></em>· <em>b<sub>i </sub></em>(the scalar product of two vectors),

<em>i</em>=1

<em>v</em><sub>1</sub>+ <em>v</em><sub>2 </sub>= (<em>a</em><sub>1 </sub>+ <em>b</em><sub>1</sub><em>,a</em><sub>2</sub>+ <em>b</em><sub>2</sub><em>,…,a<sub>n </sub></em>+ <em>b<sub>n</sub></em>), and <em>v</em><sub>1 </sub>− <em>v</em><sub>2 </sub>= (<em>a</em><sub>1 </sub>− <em>b</em><sub>1</sub><em>,a</em><sub>2 </sub>− <em>b</em><sub>2</sub><em>,…,a<sub>n </sub></em>− <em>b<sub>n</sub></em>).