# Timers

*Note that timers are processed before each sampler in the scope in which they are found; if there are several timers in the same scope, all the timers will be processed before each sampler.*
## What are Timers? ⏲

JMeter has different types of `Timers`. Frequently useds timers are: `Constant Timer`, `Uniform Random Timer`, `Precise Throughput Timer` etc.

⏳ Timers injects a delay *before* it executes Samplers in scope.

A user who knows how to place an order in the ecommerce application navigates faster in their pace. But if a user is new to the application, then the user's pace is slow. Because every user is unique.

To simulate the real world scenario in the test plan, it is important to add relevant delay between the requests. Also, it will help you test the application *in a right way*, instead of throwing up the load without delay which will trigger a server crash 💥.

## ⌨️ Activities

1. To your `Pet Store` plan, let us add a `Constant Timer` for each HTTP request.
2. Right on the first `HTTP Request`, go to `Add > Timer > Constant Timer`.
3. Add `1000` in `Thread Delay`. Unit of time in JMeter is `milliseconds`.

![Timers](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/100-Timers.jpg)

4. Click on `View Results Tree` element and then click on `Run`

You can observe a delay between the HTTP requests when the test is running.

👏 Kudos! Now you know how to add `Timers` to JMeter test plan.

Push the changes to navigate further. We are almost there, keep up the pace.
