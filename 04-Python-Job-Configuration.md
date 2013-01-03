Bamboo Configuration for a Python-based Project
=============

To demonstrate the Bamboo plugin for Jenkins, let's create a new Bamboo project for a Python project.

Click the `Create Plan` link included on the top-right of the header bar.

![Create Plan](##create-plan.png##)

Click the `Create New Plan` link.

![Create New Plan](##create-new-plan.png##)

Enter `Sauce Demo` in the `Project` field.

Enter `SAUCE` in the `Project Key` field.

Enter `Python` in the `Plan Name` field.

Enter `PYTHON` in the `Plan Key` field.

![New Plan Details](##new-plan-details.png##)

Select `Git` in the `Source Repository` drop down list.

Enter `https://github.com/rossrowe/sauce-ci-python-demo` in the `Repository URL` field.

Enter `master` in the `Branch` field

![New Plan Details](##new-plan-details.png##)

Click the `Configure Tasks` button to continue.

![Configure Tasks](##configure-tasks.png##)

Click the `Add Task` button.

![Add Task](##add-task.png##)

Click the `Command` link.

![Command Task](##command-task.png##)

Enter `Run Tests` in the `Task Description` field.

Click on the `Add Executable` link.

![Add new executable](##add-new-executable.png##)

Enter `--with-nosexunit simple_test.py` in the `Argument` field.

Click the `Save` button.

Click the `Create` button.  We need to enter the Sauce configuration after the plan has been configured, so don't select the `Enable this plan` checkbox just yet.

Click the `Default Job` link on the left-hand navigation pane.

![Default Job](##default-job.png##)

Click on the `Miscellaneous` tab

![Misc tab](##misc-tab.png##)

Select the `Enable Sauce OnDemand` checkbox to enable the plugin.  The `Enable Sauce Connect` checkbox should be selected by default.  When selected, the Sauce plugin will launch an instance of [Sauce Connect](http://saucelabs.com/docs/sauce-connect) prior to the running of your Job.  This instance will be closed when the Job completes.

Select a browser to run our tests against from the `Browser` drop down list (let's pick Firefox 15 running in Windows 2008)

![Sauce options](##sauce-options.png##)

Click the `Save` button.  That's it, our configuration is all setup, let's run the tests!

* _Next_: [Integration with tests](##04-Integration-with-tests.md##)