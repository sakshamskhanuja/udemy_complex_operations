## Complex Operations

### Description

A complex number is a number that can be expressed in the form a + bi, where a and b are real numbers, and i is a solution of the equation x2 = −1. Because no real number satisfies this equation, i is called an imaginary number. For the complex number a + bi, a is called the real part, and b is called the imaginary part. To add or subtract two complex numbers, just add or subtract the corresponding real and imaginary parts. For instance, the sum of 5 + 3i and 4 + 2i is 9 + 5i. For another, the sum of 3 + i and –1 + 2i is 2 + 3i.

Write a class with the name <b>ComplexNumber</b>. The class needs two fields (instance variables) with name <b>real</b> and <b>imaginary</b> of type <b>double</b>. It represents the Complex Number. The class needs to have one constructor. The constructor has parameters <b>real</b> and <b>imaginary</b> of type <b>double</b> and it needs to initialize the fields.

Write the following methods (instance methods):

<ul>
<li>Method named <b>getReal</b> without any parameters, it needs to return the value of <b>real</b> field.</li>
<li>Method named <b>getImaginary</b> without any parameters, it needs to return the value of <b>imaginary</b> field.</li>
<li>Method named <b>add</b> with two parameters <b>real</b> and <b>imaginary</b> of type <b>double</b>, it needs to add parameters to fields. In other words, it needs to do a complex number add operation as described above.</li>
<li>Method named <b>add</b> with one parameter of type <b>ComplexNumber</b>. It needs to add the ComplexNumber parameter to the corresponding instance variables.</li>
<li>Method named <b>subtract</b> with two parameters <b>real</b> and <b>imaginary</b> of type <b>double</b>, it needs to subtract parameters from fields, in other words, it needs to do a complex number subtract operation as described above.</li>
<li>Method named <b>subtract</b> with one parameter other of type <b>ComplexNumber</b>. It needs to subtract the other parameter from this complex number.</li>
</ul>

### Test Code

    ComplexNumber one = new ComplexNumber(1.0, 1.0);
    ComplexNumber number = new ComplexNumber(2.5, -1.5);
    one.add(1,1);
    System.out.println("one.real= " + one.getReal());
    System.out.println("one.imaginary= " + one.getImaginary());
    one.subtract(number);
    System.out.println("one.real= " + one.getReal());
    System.out.println("one.imaginary= " + one.getImaginary());
    number.subtract(one);
    System.out.println("number.real= " + number.getReal());
    System.out.println("number.imaginary= " + number.getImaginary());
  
  ### Output

    one.real= 2.0
    one.imaginary= 2.0
    one.real= -0.5
    one.imaginary= 3.5
    number.real= 3.0
    number.imaginary= -5.0
