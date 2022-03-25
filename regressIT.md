# MultiVariable Regression in RegressIt

Before you start working on your regression decide what you want the data to do for you. What information are you trying to gain? For my example, I want to see how 3 individual stocks affect the S&P 500(a stock index). I am using the data in [stockReturns.xlsx](https://github.com/nmcdowell00/Data_Jam_Resources/blob/main/stockReturns.xlsx) for this example. The following steps will help you run your own MultiVariable.xlsx: 

# Choose you data:
[](images/columnms.png)
This image shows the data I will ben using;

# Create Names:
You will need to create names within the data to properly run regressit. To do this click *Create Names* in the regressIT toolbar [](images/createnames.png) This will bring up a window that asks you where in the data set the names are. I select *Top Row* as that is where my nanes are [](images/toprow.png)

# Run the Regression
Now you want to click on the *Linear Regression* button in the top left corner of Excel. This will bring up a window where you will select you variables: 
[](images/regressittable.png) I set the independent variable to the one I want to predict, S&P 500, and the dependent variables to what I think affects the S&P 500, the three other stocks. 

# Results
After clicking *Run*, a new tab containing the results of your regression will be generated in excel. [](images/stats.png) In this table there are many values but the ones I will focus on now ill be held under the *Coefficients* tab. These values are what you will use to build your regression equation. The value corresponding to *Constant* (0.005629) will be your interecept. The next three numbers ar the coefficients for each of your independent variables. This number can be interpretted as how much change in the S&P 500 is caused when one variable increases by one unit. For example, when the Giant stock goes up one point the S&P 500 goes up 0.138 points. For this example the equation would be y = 0.005629 + 0.138*g*g + 0.090*h* + 0.132*t*. 


