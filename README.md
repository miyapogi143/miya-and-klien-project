Narrative Report: Object-Oriented programming in PHP (Activities 1&2)

This Report details the implementtion and functionality
![image](https://github.com/user-attachments/assets/9be46087-6e81-46cf-a7ef-0d4c15a57b2b)
![image](https://github.com/user-attachments/assets/a18bde77-998d-4120-9704-c1e0e9715f0d)
![image](https://github.com/user-attachments/assets/19a32b70-22b8-4064-9a85-d4fcb1ae7345)

This report analyzes two distinct implementations of a  Movie  class in PHP, highlighting their design choices, strengths, and weaknesses.

Implementation 1: The Public Properties Approach

The first implementation uses public properties ( $title ,  $director , etc.) and a single  setMovieDetails()  method.  This approach prioritizes simplicity and direct access to the movie's attributes.
The  setMovieDetails()  method includes basic validation for the  year  (checking if it's within a reasonable range) and  rating  (ensuring it's between 0 and 10). 
However, the lack of more thorough validation and the reliance on public properties introduces potential risks.  Incorrect data could be easily set, leading to inconsistencies and errors.
The use of a single method for setting all attributes also reduces the code's modularity and makes it harder to expand upon in the future.
his approach is like building a house with exposed wiring—it's quick, but dangerous.

Implementation 2: The Encapsulated Approach

The second implementation employs private properties and individual setter methods ( setTitle() ,  setDirector() , etc.).  This approach prioritizes data integrity and encapsulation.
Each setter method includes input validation, enhancing the robustness of the class.  The use of private properties prevents direct modification of the movie's attributes, ensuring data consistency.
The individual setter methods improve code organization and readability. Furthermore, the inclusion of getter methods provides controlled access to the data.  
This encapsulated approach is like building a well-insulated, secure house—it’s more complex to build but much safer and more durable in the long run.

Comparative Analysis:

Table
  
Feature Implementation 1 (Public Properties) Implementation 2 (Encapsulated) 
Data Access Public Private 
Validation Basic More robust and granular 
Modularity Lower Higher 
Maintainability Lower Higher 
Security Lower (vulnerable to incorrect data) Higher 

Conclusion:

While the first implementation offers a simpler initial design, the second implementation, with its encapsulated properties and thorough validation, 
is significantly superior in terms of robustness, maintainability, and security. 
The added complexity of the second approach is justified by the increased reliability and reduced risk of errors.  
The second implementation represents best practices in object-oriented programming, emphasizing data protection and controlled access.
The first implementation serves as a cautionary tale on the importance of proper validation and encapsulation in software development.
