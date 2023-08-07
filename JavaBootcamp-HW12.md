# JavaBootcamp-HW12


- # Output of quistion 1
    | Output               | Comment
    | :---------------- | :------
    |hey from message1 |  Annotation (Bean) will run the method.
  

    <br><br><br>

- # Output of quistion 2
    #### There is 2 cases , and both cases will implement "getMessage1" before "getMessage2".
    - Case 1: Implement "getMessage1" then "getMessage2".
    - Case 2: Implement "getMessage2": 

    | Output               | Comment
    | :---------------- | :------
    |hey from message1 <br> hey from message2| Annotation Qualifier in header of the method "getMessage2" call the qualifier key of method "getMessage1". So, will implementing "getMessage1" then "getMessage2".

    
     #### - Both methods return "1".

    <br><br><br>

- # Output of quistion 3
    #### There is many cases, and all cases will implement "getMessage3" before "getMessage2".
    | Output               | Comment
    | :---------------- | :------
    |hey from message1 <br>hey from message3<br> hey from message2 | Implement "getMessage1" then "getMessage2"
    |hey from message3 <br>hey from message2<br> hey from message1 | Implement "getMessage3" then "getMessage2" then "getMessage1"
    |hey from message3 <br>hey from message1<br> hey from message2 | Implement "getMessage3" then "getMessage1" then "getMessage2"

    #### - "getMessage1" return "1", and "getMessage2" & "getMessage3" returns "3".

    <br><br><br>

- # Output of quistion 4
    #### There is many cases, and all cases will implement "getMessage3" before "getMessage2" and "getMessage1" before MainController, and 3 of those cases are: 
    | Output               | Comment
    | :---------------- | :------
    |hey from message1 <br>hey from message3<br> hey from message2 <br> hey from main controller| Implement "getMessage1" then "getMessage3" then "mainController".
    |hey from message3 <br>hey from message2<br> hey from message1 <br> hey from main controller| Implement "getMessage2" then "mainController"
    |hey from message1 <br>hey from main controller<br> hey from message3 <br> hey from message2| Implement "mainController" then "getMessage2"


    #### - "getMessage1" return "1", "getMessage2" & "getMessage3" returns "3", and in "mainController" data= "1"

 <br><br><br>

- # Output of quistion 5
    #### There is many cases, and all cases will implement "getMessage3" before "getMessage2" & "MainController",and 3 of those cases are:
    | Output               | Comment
    | :---------------- | :------
    |hey from message3 <br>hey from message2<br> hey from main controlle <br> hey from message1| Implement "mainController" then "getMessage1".
     |hey from message1 <br>hey from message3 <br> hey from message2 <br> hey from main controlle| Implement "getMessage1" then "mainController". <br> Or Implement "getMessage1" then "getMessage3" then "mainController" <br>Or Implement "getMessage1" then "getMessage3" then "getMessage2" then "mainController"


    #### - "getMessage1" return "1", "getMessage2" & "getMessage3" returns "3", and in "mainController" data= "2"

