# HTTP Sampler

As you aware, we are going with the default number of threads in `Thread Group`. In this exercise, you will learn about `HTTP Request` element.

`HTTP Sampler lets you send an HTTP/HTTPS request to a web server. It also lets you control whether or not JMeter parses HTML files for images and other embedded resources and sends HTTP requests to retrieve them.`

Before adding `HTTP Sampler`, let's add the default settings to your HTTP Requests. To define the default settings for `HTTP Requests` we are going to add `HTTP Request Defaults`.

`HTTP Request Defaults element lets you set default values that your HTTP Request controllers use.`

In this exercise, we are going to add two HTTP requests to the test plan.

Let's dive into the activities.

## ⌨️ Activities

1. Add a `HTTP Request Defaults` by right clicking on `Thread Group > Config Element > HTTP Request Defaults`.
2. Add the properties to the `HTTP Request Defaults` as shown below.

![HTTP Request Defaults](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/10-HTTPRequestDefaults.jpg)

3. Add a `HTTP Sampler` by right clicking on `Thread Group > Sampler > HTTP Request`.
4. Add `/` to the `Path`

![HTTP Request 1](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/20-HTTPRequest-1.jpg)

5. Add another `HTTP Sampler`
6. Add `/actions/Catalog.action` to the `Path`

![HTTP Request 2](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/30-HTTPRequest-2.jpg)

7. Save your test plan by pressing `Ctrl + S`
8. Push the test plan to the repo to go to next exercise.