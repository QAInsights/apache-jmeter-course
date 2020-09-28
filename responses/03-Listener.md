# Listeners

In this exercise, we are going to see about Listeners, how to add them and how to execute JMeter test plan.

## About Listeners

Listeners just listens to the test results, but it can perform other tasks. 

> ⚠ Listeners are resource intensive, it should not be used during the load testing.

> Listeners are processed at the end of the scope in which they are found.

There are many types of Listeners available in JMeter. In this exercise, we are going to cover `View Results Tree`.

`The View Results Tree shows a tree of all sample responses, allowing you to view the response for any sample. In addition to showing the response, you can see the time it took to get this response, and some response codes.`

## ⌨️ Activities

1. In your `S01_PetStore` test plan, add a `View Results Tree` element as shown below.

![View Results Tree](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/40-ViewResultsTree.jpg)

2. To execute JMeter test plan, click on `Run` button in the toolbar, or hit `Ctrl + R`. After couple of seconds, you will get two green items in `View Results Tree` as shown below.

![Success Requests](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/50-SuccessRequests.jpg)

3. Toggle between `Sampler result`, `Request`, `Response data` for both of the requests and understand the context.

Push the changes to go to your next exercise ➡.