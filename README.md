Download Link: https://assignmentchef.com/product/solved-assignment-5-classes-and-objects-revisited
<br>
<ol>

 <li>class A</li>

</ol>

{

public A() { n = 0; }

public A(int a) { n = a; }

public void f() { n++; }

public void g() { f(); n = 2 * n; f(); }

public int h() { return n; }

public void k() { System.out.println(n); }




private int n;

}

Identify the constructors, mutator functions, and accessor functions. What kind of variable is n?

<ol start="2">

 <li>With the nonsense class from the preceding exercise, determine what the following program prints.</li>

</ol>

public static void main(String[] args) {

A a = new A();

A b = new A(2);

A c = b;

A d = new A(3);

a.f();

b.g();

c.f();

d.g();

d.k();

A e = new A(a.h()+ b.h()+ c.h());

e.k();

}




<ol start="3">

 <li>Implement all the methods of the following class:</li>

</ol>

class Person {




private String name;

private int birthdayYear;







public Person() {

……….

}

public Person(String givenName, int yearOfBirth) {

……………………

}

public String getName() {

……………………….

}

public String changeName(String name) {

……………………… }

public int getAgeInYears(int currentYear) {

……………………..

}

};




void main()

{

}




Write a small test program that creates and works with objects of class Person as well.




<strong>Design exercises: </strong>

<ol start="4">

 <li>Implement a class Address. An address has</li>

</ol>

<ul>

 <li>a house number,</li>

 <li>a street,</li>

 <li>an optional apartment number,</li>

 <li>a city,</li>

 <li>a state and a</li>

 <li>postal code.</li>

</ul>

Supply two constructors:

<ul>

 <li>one with an apartment number</li>

 <li>and one without.</li>

</ul>

Supply a print function that prints the address with the street on one line and the city, state, and postal code on the next line.

Supply a method compareTo that tests whether one address comes before another when the addresses are compared by postal code.

<ol start="5">

 <li>Implement a class Account. An account has</li>

</ol>

<ul>

 <li>a balance,</li>

 <li>functions to add</li>

 <li>and withdraw money,</li>

 <li>and a function to inquire the current balance.</li>

</ul>

Pass a value into a constructor to set an initial balance.

If no value is passed the initial balance should be set to $0.

Charge a $5 penalty if an attempt is made to withdraw more money than available in the account.

Enhance the Account class to compute interest on the current balance.

<ol start="6">

 <li>Implement a class Bank. This bank has two objects</li>

</ol>

<ul>

 <li>checking</li>

 <li>and savings</li>

</ul>

of the type Account that was developed in the preceding exercise.

Implement four instance methods:

deposit(double amount, String account)




withdraw(double amount, String account)




transfer(double amount, String account)




printBalances()

Here the account string is “S” or “C”. For the deposit or withdrawal, it indicates which account is affected. For a transfer it indicates the account from which the money is taken; the money is automatically transferred to the other account.

<ol start="7">

 <li>Define a class Country that stores the name of the country, its population, and its area. Using that class, write a test program that creates a few countries and stores them in an array and then prints</li>

</ol>

<ul>

 <li>The country with the largest area</li>

 <li>The country with the largest population</li>

 <li>The country with the largest population density (people per square mile)</li>

</ul>

<ol start="8">

 <li>Write a class called Triangle that can be used to represent a triangle. It should include the following methods that return boolean values indicating if the particular property holds:</li>

</ol>

<ul>

 <li>isRight (a right triangle)</li>

 <li>isScalene (no two sides are the same length)</li>

 <li>isIsosceles (exactly two sides are the same length)</li>

 <li>isEquilateral (all three sides are the same length)</li>

</ul>

Write a simple tester program that creates a few triangles and asks them about their type.




<ol start="9">

 <li>This problem has several parts:</li>

</ol>

<ol>

 <li>Write a simple Vehicle class that has fields for (at least) current speed, current direction in degrees, and owner name.</li>

</ol>







<ol>

 <li>Add a static field to your Vehicle class for the highest Vehicle Identification Number issued, and a non-static field that holds each vehicle’s ID number.</li>

</ol>




<ol>

 <li>Write a main method for your Vehicle class that creates a few vehicles and prints out their field values. Note that you can also write a separate tester program as well.</li>

</ol>







<ol start="4">

 <li>Add two constructors to Vehicle. A no-arg constructor and one that takes an initial owner’s name. Modify the tester program from the previous step and test your design</li>

</ol>







<ol>

 <li>Make the fields in your Vehicle class private, and add accessor methods for the fields. Which fields should have methods to change them and which should not?</li>

</ol>







<ol>

 <li>Add a changeSpeed method that changes the current speed of the vehicle to a passed-in value, and a stop method that sets the speed to zero.</li>

</ol>







<ol>

 <li>Add two turn methods to Vehicle. One that takes a number of degrees to turn, and one that takes simply either a Vehicle.TURN_LEFT or a Vehicle.TURN_RIGHT constant. Define the two constants accordingly.</li>

</ol>







<ol>

 <li>Add a static method to Vehicle that returns the highest identification number used so far.</li>

</ol>




<ol>

 <li>Add a toString method to Vehicle.</li>

</ol>


