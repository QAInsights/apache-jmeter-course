# Create your first Thread Group

## 🚀 Launching JMeter

The prerequisite to launch JMeter is to have Java installed in your computer. You can interact with JMeter using the CLI and Non-CLI mode. Command Line Mode is the recommended mode for performance testing purposes. But to create or edit, you can launch JMeter in Non-CLI mode.

Go to the location where you extracted the content of JMeter file e.g. `C:\Tools\apache-jmeter-5.3` 

Navigate to `bin` folder and launch `jmeter.bat` for Windows OS or `jmeter.sh` for Linux/macOS systems.

If Java is installed properly, JMeter will launch as shown below.

[Placeholder to add the images]

Congratuations on launching JMeter 🎉

## Test Plan

In JMeter world, you create test plans which has the file extension of .jmx. If you open .jmx file in your favorite editor, you can see the XML tags.

A typical JMeter test plan consists of at least one `Test Plan` element and one or more `Thread Groups` and/or `Samplers`/`Other elements`.

📌 You cannot delete `Test Plan` element

## Thread Group

`Thread Group` is the inception for any JMeter tests. In `Thread Group` you can configure the number of threads/users, duration, ramp up period etc.

In this exercise, we are going with the default values of `Thread Group`.

Let's get started 🚀

## ⌨️ Activities

1. Launch JMeter
2. Add a `Thread Group` by right clicking on `Test Plan > Threads (Users) > Thread Group`
3. Go to `File > Save`, enter `S01_PetStore.jmx` and hit `Save` button
4. Push the JMeter test plan to your repo

After successful push, I will let you know the next steps.