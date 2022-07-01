# allure-text-report

When used with Allure reports, allows logging steps to console out and (optionally) text files.

One of the big downsides of Allure reporting that it requires installing allure reports locally to be able to open a report. 
This results in discouraging team members outside QA team from accessing and reading these reports. It also makes it
hard to quickly check the reason of a test failure by looking at CI/CD run (allure report have to be downloaded and uncompressed first). 

Ability to intercept `@Step` calls is built into Allure library, but is not documented, which makes it hard to find.

This library is based on this StackOverflow thread: https://stackoverflow.com/questions/45624859/allure2-listener-to-output-the-steps-in-console (kudos to Sergei Korol for the solution).
