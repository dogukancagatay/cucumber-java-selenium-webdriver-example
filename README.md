# Automated test example in Java with Cucumber and Selenium WebDriver #

This project is an example of UI automated functional test for Google home page and search using Selenium and Cucumber.

Test scenarios are described in the feature files located here ./src/test/resources/com/automatedtest/sample.

For more info about this project, read the article ["UI automated test project example with Selenium, Cucumber and Java"](https://medium.com/@lucie.duchemin/ui-automated-test-project-example-with-selenium-cucumber-and-java-b33788bd11c4)

## Installation ##

You need to have Java 8/11 JDK installed along with [Maven](https://maven.apache.org/download.cgi).

Tests are run against Selenium Hub @ `http://localhost:4444`.

## Running tests ##

For running tests with Chrome Node on Selenium Hub.
```console
$ mvn -Dbrowser=chrome test
```

For running tests with Firefox Node on Selenium Hub.
```console
$ mvn -Dbrowser=firefox test
```

By default, tests will run on Chrome. To change that, specify `-Dbrowser={browser}` where `{browser}` is either `chrome` or `firefox`. If you haven't added the chrome driver path to your local variables, you can add it directly in the run command with the option `-Dwebdriver.chrome.driver=path/to/the/driver`.

You can also select specific scenarios to execute using `-Dcucumber.options="--tags @your_tag"`. More info about tags and how to combine them [here](https://github.com/cucumber/cucumber/tree/master/tag-expressions).

## Cucumber Studio (Hiptest) ##

Feature files can be handled with Cucumber Studio (previously called Hiptest), a test management platform. To get started with Cucumber Studio, 
go [here](https://cucumber.io/tools/cucumberstudio/getting-started-with-behavior-driven-development/). Features files in 
this project were exported directly from an [Hiptest project](https://studio.cucumber.io/projects/102008) using 
[Hiptest publisher](https://github.com/hiptest/hiptest-publisher). Credentials to access the project are the following.
