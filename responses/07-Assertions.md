# Assertions

Assertions - *the action of stating something or exercising authority confidently and forcefully.*

## Assertions in JMeter ✔

`Assertions are used to perform additional checks on samplers, and are processed after every sampler in the same scope. To ensure that an Assertion is applied only to a particular sampler, add it as a child of the sampler.`

JMeter has different types of `Assertions`. Few assertions are expensive. It is not advisable to enable them during the load test. Commonly used `Assertions` are `Response Assertion`, `JSON Assertion`, `Size Assertion` etc.

## ⌨️ Activities

1. For the Pet Store scenario, we are going to add a `Response Assertion` for the `Search` HTTP request. Before we get started, let us change the name of the HTTP Requests as shown below.

![HTTP Requests](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/110-RenameHTTP.jpg)

2. To add a `Response Assertion`, right click on `03_Search` HTTP request > `Add > Assertions > Response Assertion`.

3. Set the below properties as shown below for the assertions. Below assertion validates the HTTP Response Code exactly matches `200`, if not it will show it as failure in the `View Results Tree`.

![Response Assertion](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/120-ResponseAssertion.jpg)

4. Hit `Run` to observe the results.

Below is the sample failed assertion.

![Failed Assertions](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/130-AssertionFailed.jpg)

Push the changes to proceed further.