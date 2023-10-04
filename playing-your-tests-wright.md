# Playing your tests wright

Speaker: Debbie O'Brien.

## Introduction

Intro about Playwright: what it is and what it does.

## Features

 - Auto waiting: you do not need to manually wait for elements to appear. Same for assertions.
 - Iframes and shadow dom works out of the box.
 - Tests isolation: you do not need to clean after each test.
 - Parallellism: tests run in parallel.
 - Sharding: running tests in different machines.
 - VScode integration.
 - Locator picker: shows locators in the ui so you don't need to think about it.
 - HTML Reports: you can see the reports of your test runs.
 - Trace Viewer: you can download traces of the tests and run them in the devtools.

## Tips/Best practices

 - Do e2e tests and keep library up to date
 - Prioritize user facing attributes (same philosophy as react testing library). Don't use classes, xpath, etc.
 - Use playwright assertions: it retries automatically.
 - Do not test external deps. For instance links to other websites should not be loaded.
 - Use codegen: do the actions in the browser and then generate the test code.
 - Use UI Mode (and watch mode)

## Scaling

 - Shard the tests in different machines to run them in parallel.

**Opinion**: we should definitely try to use codegen, but I don't know if it really fits the "page object" architecture of our projects. Also the VSCode extension is pretty cool and I didn't even know it existed. In the demo she showed the "Accessibility" tab in devtools too, which I never used and I will take a look at it.