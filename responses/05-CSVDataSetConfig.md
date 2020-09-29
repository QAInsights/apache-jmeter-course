# Data Parameterization

In this exercise, we are going to see about data parameterization and add `Login` request in our test plan.

## What is Data Parameteization?

In real world, every user is unique. To simulate the real world scenario, it is critical to test the application with different sets of data. 

If you test your application with the same test data, your response likely will be served from the cache. Your performance test results will not yield the real performance.

> Generating test data in run time is expensive. It is important to generate the test data well ahead.

> Creating test data is beyond the scope of this training. 

## About CSV Data Set Config

In JMeter, data parameterization can be achieved using `CSV Data Set Config`. 

` CSV Data Set Config is used to read lines from a file, and split them into variables. It is easier to use than the __CSVRead() and __StringFromFile() functions. It is well suited to handling large numbers of variables, and is also useful for testing with "random" and unique values.`

## Scenario

As you know we are working on `Pet Store` application. Assume that you need to create a test plan for `Search` scenario. 

1. Launch Pet Store
2. Navigate to `https://petstore.octoperf.com/actions/Catalog.action`
3. Search for different pets using the search text box. 

### Sample Test Data

```
angelfish
cat
dog
bird
bulldog
```

## ⌨️ Activities

1. In your `S01_PetStore`, add a new `HTTP Sampler` and fill the below properties.

HTTP Method: `POST`  
Path: `/actions/Catalog.action`  
Parameters:  
`keyword` as `fish`  
`searchProducts` as `Search`

![Add Parameters](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/60-AddParameters.jpg)

> As you see, we have not done with the parameterization. Let's get started.

2. Add a `CSV Data Set Config` by right-clicking on the `Thread Group > Add > Config Element > CSV Data Set Config`

3. Copy the above test data and save it as `PetSearch.csv` in your `bin` folder.

4. Configure the `CSV Data Set Config` as shown below.

![CSV Data Set Config](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/70-CSVDataSetConfig.jpg)

You can add multiple `Variable Names` if the CSV test file has multiple columns.

5. Go to the POST HTTP Request and edit the `keyword` to `${P_SearchKeywords}`. `${P_SearchKeywords}` holds the value of the variable from CSV Data Set Config in runtime.

![CSV POST HTTP](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/80-POST-HTTP.jpg)

6. Since we have 5 rows in our test data, click on `Thread Group` and change the `Loop count` to `5`.

7. Hit the `Run` button and click on `View Results Tree` to view the results for each test data.

![CSV Results](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/90-ViewResultsTree-CSV.jpg)

You are a super star 🌟!

Push the changes to go to your next exercise ➡.