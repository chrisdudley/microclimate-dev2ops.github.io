---
layout: document
title: Performance testing your project
description: Performance testing your project
keywords: Using, coding, run, apply, import, create, edit, log, monitor, test, performance
duration: 5 minutes
permalink: performancetesting
type: document
---

When you generate a project, Microclimate generates a basic test plan. You can edit this test plan or use your own. You can then go to the **App monitor** tab to see the application traffic.

Follow the steps to edit and test your code:
1. Select a project or generate a new project.
2. Click the **Edit code** tab and expand your project directory. From the directory, you can access `load-test`>`TestPlan.jmx` and edit the code in the `TestPlan.jmx` file. For example, you can add your own endpoints or change the number of threads that are running. If you don't want to edit the test plan, Microclimate uses the default test plan that is already provided for you.
3. Save your changes and wait for the project to build.
4. After the project builds, click the **App monitor** tab to see that your changes are applied. To test your application, click the **Run load** button, which uses [JMeter](https://jmeter.apache.org/) to load test functional behavior. A text box appears that states, "**Run load** The request to start the process has been sent."
5. Wait for the test to run. You can watch the test metrics while the test is running.
6. When the test is complete, navigate back to the **Edit code** tab to see the result of the latest run. A `load-test` directory appears with a time stamp. Within this time stamped folder, you can access the `jmeter.log` file that shows the log, the `TestPlan.jmx` file that ran, and the `testresults.jtl` file that shows the results.
