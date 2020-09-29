# Transaction Controller

Just like any other programming language, you can control the execution flow using `Logic Controllers` in JMeter.

`Logic Controllers` which determines the order in which Samplers are processed.

There are different types of controllers in JMeter. Commonly used ones are: `If`, `Transaction`, `While`, `Loop` etc.

## ⌨️ Activities

We are going to measure the performance of `Search` functionality. Transactions are nothing but the collection of sequential steps/requests. Let us add transactions to the Pet Store test plan.

Instead of adding the transaction controller, we are goint to insert it to the HTTP requests.

1. Right click on `01_Launch` > `Insert Parent` > `Logic Controller` > `Transaction Controller`. This will insert a transaction controller to the selected request. Rename the transaction controller to `T01_Launch`.

2. Check `Generate parent sample` checkbox.

3. Repeat the steps for other two HTTP requests as shown below.
![Transaction Controller](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/140-TransactionController.jpg)

4. Hit `Run` to view the results.

![Transactions Results](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/150-Transactions-Results.jpg)

Push the changes to proceed further.



