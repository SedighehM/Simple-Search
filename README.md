Simple Search

This is a simple code to search records and show them in a table and div.

1.	loadData()

This function sends a request for getting data from a server using a pre-defined async function called getQuote(). The following lines call two other functions to fill the table and div by returned data. Also, this function checks the input value to see its valid or not and shows meaningful error messages.
Note1: Defining multiple functions helps us to have cleaner code.
Note2: Handling errors and showing proper messages to the user is essential in frontend development.

2.	createHeader()

This Function gets data as an argument and fills different UI segments with different values.
Note3: We declared the setText() function for setting the text of DOM elements to have more readable code.

3.	createTable()

This function gets two values as argument:
labels ==> Labels is a map that maps every label to our desired value
data ==> Data is server response
This function adds one row with two columns to the table for each label and lastly fills them with labels and an element in response (or a mix of elements in the response).
Note4: This function is completely flexible for future use. Any time you want to fill the table with any information, you need to only pass the map and data to it. Having reusable code is an important aspect in development.
