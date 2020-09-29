# Test Execution

## CLI Mode

It is recommended to run the test using the CLI mode to get the optimal results.

Here is the command to run the test in CLI mode.

`.\jmeter.bat -n -t .\S01_PetStore.jmx -l Run1.jtl`

**DISCLAIMER**

In this exercise, we are going to run the test using just only one thread and for 30 seconds only. Because, we are not authorized to run the test in the desired environment.

ALL THE PERFORMANCE TESTING ACTIVITIES MUST BE CARRIED OUT IN THE NON-PRODUCTION ENVIRONMENT.

I AM NOT RESPONSIBLE FOR ANY SORT OF DAMAGE CAUSED DUE TO YOUR LOAD TESTING FOR ANY WEBSITES/APPS/SERVICES/SYSTEM/ENTITY.

Please act responsibly.

## ⌨️ Activities

1. Before we start the test, click on `Thread Group`, select `Specify Thread lifetime` and enter `30` in the `Duration (seconds)` text box.

2. Disable `View Results Tree`

3. Hit `Save` and close the JMeter.

4. Launch `Command Prompt` (for Windows) or `Terminal` (for Linux/macOS). Navigate to JMeter directory `bin` folder.

5. Issue the below command.

`.\jmeter.bat -n -t .\S01_PetStore.jmx -l Run1.jtl`

During the test, you can observe the statistics in the command prompt. Once the run is done, you will get the status as shown below.

![Run 1](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/160-Run1.jpg)

6. To view the results in JMeter. Launch JMeter and add any listener and browse the `jtl` file which got generated in the `bin` folder.

![Summary Report](https://raw.githubusercontent.com/QAInsights/apache-jmeter-course/master/images/170-SummaryReport.jpg)

Literally you can add any type of listener to visualize the results.

Push the changes to proceed further to conclude your exercise.