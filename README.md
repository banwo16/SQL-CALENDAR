
	
/*---- This code is the property of Banwo Oduwole. This is a User definition Function
This code is building a calendar that shows the current date and time and day of the week.
Also used DECLARE, SET AND INSERT to write this code. Used Varchar to return the day of the week in letters
 and not just numbers-------*/

/*---- The name of the function is udf_day_of_the_week. 
Decided to use a table for parameter, so I created one to fit into the function. 
I used a declare and set method but found out too late that it is not possible to print multiple variables in functions,
so I used the returns table option and named the heading Calendar To call the function you can use these two queries separately SELECT * FROM udf_day_of_the_Week()


To add month option SET @TODAY = ('Today' + SPACE(1) + 'Month' + SPACE(1) + (CAST(MONTH(GETDATE())  AS VARCHAR(MAX))  + SPACE(1) + (CAST(DATENAME(WEEKDAY, GETDATE()) + SPACE(1) + (DATENAME(DAY, GETDATE())+ SPACE(1) + DATENAME(YEAR, GETDATE())) AS Varchar (MAX)))))

select CALENDAR from udf_day_of_the_Week()
——*/
