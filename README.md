# cmpe-202-creditcard-project

**Primary Problem:**
**Identifying the type of credit card from a given record and creating an instance of the corresponding subclass (VisaCC, MasterCC, AmExCC, etc.). <br/>
Secondary Problems:** 
Validating the credit card number.
Extensibility for adding more credit card types in the future.

<ul>
  <li>
1: Design Patterns and Approach:

<ul>
  <li> <strong>Factory Method Pattern</strong> for creating instances of different credit card types. This pattern allows the creation of objects without specifying the exact class of the object that will be created.
A CreditCardFactory abstract class can determine the type of credit card based on the number and return an instance of the appropriate CreditCardFactory subclass. </li>
  <li>
<strong>Template Method Pattern </strong> could be used in the CreditCard class to define a template for credit card number validation. </li>
</ul>


**Consequences:**
<ul>
<li>The Factory Method pattern provides flexibility and encapsulates the instantiation logic.</li>
<li>The Template Method Pattern provides a skeleton for common validation steps while allowing subclasses to override specific steps.</li>
  </ul>
  </li>
  <li>
2: Extending Design for Multiple File Formats

    
**Extended Design:**

<ul>
<li>Implement an Adapter Pattern to handle different file formats. This allows your application to interface with different types of files through a common interface.</li>
<li>Create a FileAdapter interface with methods like readFile() and writeFile()./li>
<li>Implement this interface in classes like CSVAdapter, JSONAdapter, and XMLAdapter.
Accommodating Future File Formats:
The design should be open for extension but closed for modification (Open/Closed Principle).
New file format adapters can be added without altering the existing code.</li>
  </ul>
</li>
<li>
3: Diagrams


UML Class Diagram:

![image](https://github.com/shiva-vardhineedi/cmpe-202-creditcard-project/assets/143037444/5a42922d-2746-44dd-9af5-e72a31a4c6ca)

Sequential Diagram:

![image](https://github.com/shiva-vardhineedi/cmpe-202-creditcard-project/assets/143037444/5c959b3c-f3ee-4874-8ac7-0d02d348b40b)


</li>
</ul>




