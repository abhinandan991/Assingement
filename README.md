# Assingement

Link:  https://javascript.info/task/find-elements/table.html 

How to find?…

The table with id="age-table".
All label elements inside that table (there should be 3 of them).
The first td in that table (with the word “Age”).
The form with name="search".
The first input in that form.
The last input in that form.

Answer:

1. The table with the id="age-table":
    document.querySelector("#age-table"); //Selects the required table. 
    const r_table = document.querySelector("#age-table"); //Assigned a variable to it, for later use in the assignment. 
   
2. All label elements inside that table.
    r_table.querySelectorAll("label"); //Select all the labels in the table.
    
3. The first td in that table.
    r_table.querySelector("td"); //Selects the first td element, because, although there are multiple td elements, querySelector always selects the first element from the page.
    
 4. The form with name="search".
    document.getElementsByName("search-person")[0]; //Using getElementsByName returns a nodelist, therefore, [0] has been used to index into the first position of the nodelist to get the required element.
    const r_form = document.getElementsByName("search-person")[0]; //Assigned a variable to the form for later use in the assignment.
    
 5. The first input in that form.
    r_form.querySelectorAll("input")[0] //Selects the first input in the form.
    
 6. The last input in that form. 
    r_form.querySelectorAll("input")[r_form.length - 1]; //Selects the last input in the form. [r_form.length - 1] has been used to index the last position of the returned nodelist of querySelectorAll("input"), because, the last index is always 1 less than the length of the nodelist.
    
    

