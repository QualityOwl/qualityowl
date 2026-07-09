## Hi, I'm Josh

I am a Software Development Engineer in Test with 10+ years of experience building scalable test automation frameworks across UI, API, and performance layers.

My passion is to deliver a high quality experience to end-users through shift-left testing, cross-team collaboration, and applying QA best practices at each step of the software development life cycle.

Remember...

*"If it is not tested, it is not working!"*

---

## Tech Stack

| Layer           | Tools                                                    |
| --------------- | -------------------------------------------------------- |
| UI Automation   | Playwright (TypeScript), Selenium WebDriver (C#)         |
| API Testing     | Postman, ReadyAPI, HttpClient (C#), k6 (JavaScript)      |
| Frameworks      | Node.js, .NET                                            |
| CI/CD           | Azure DevOps, GitHub Actions, Argo CD                    |
| Design Patterns | Page Object Model, Custom Fixtures, Layered Architecture |

---

## Portfolio

| Repo                                                                                          | What it demonstrates                                                     | CI                                                                                                                       |
| --------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ |
| [demo-playwright-typescript](https://github.com/QualityOwl/demo-playwright-typescript)         | End-to-end UI tests with custom fixture extensions and page object model | ![](https://github.com/QualityOwl/demo-playwright-typescript/actions/workflows/playwright.yml/badge.svg)                 |
| [demo-rest-api-tests-csharp](https://github.com/QualityOwl/demo-rest-api-tests-csharp)         | Functional API tests covering full CRUD, auth, and error scenarios       | ![](https://github.com/QualityOwl/demo-rest-api-tests-csharp/actions/workflows/run-functional-tests.yaml/badge.svg)      |
| [demo-rest-api-tests-javascript](https://github.com/QualityOwl/demo-rest-api-tests-javascript) | k6 load and performance tests with ramp stages and threshold enforcement | ![](https://github.com/QualityOwl/demo-rest-api-tests-javascript/actions/workflows/run-performance-tests.yaml/badge.svg) |
| [demo-selenium-webdriver-csharp](https://github.com/QualityOwl/demo-selenium-webdriver-csharp) | Selenium WebDriver framework with runners, wrappers, and xUnit           | —                                                                                                                       |

---

## Let's Talk Shop

> **What is one of your greatest achievements as a QA Engneer?**

One that stands out to me is my success in scaling functional test execution across microservices at my organization.

One of our teams had worked to integrate functional test runs into their Argo CD blue/green deployment checks for their microservice. However, the implementation was rough, the documentation was minimal and no other teams had been able to adopt it.

I came in and refined the workflow from start to finish: designed test projects, updated Helm charts, built analysis templates, and secured configuration secrets. I then wrote new documentation from scratch that was clear, detailed, and accessible to everyone in the org.

Over a period of six months, I onboarded over 30 dev teams and test coverage for blue/green rollouts increased by 20%. Bad deployments are getting caught automatically now instead of seeing issues crop up after the fact.

<br>

> **How do you approach building automation frameworks from scratch?**

I start by understanding the application under test, the existing tech stack, the CI/CD pipeline, and what testing (if any) is already in place.

From there, I work with product and engineering teams to identify the highest-risk areas to address first with automated testing. This helps establish credibility and ROI early on.

Once priorities are set, I select the language and tooling that best fit the tech stack and the team's skill set. The test framework is built to be understandable, maintainable, and extensible from day one. Tests are wired into CI/CD workflows so that every deployment is validated from the beginning and not as an afterthought.

<br>

> **What is your strategy for deciding which test cases to automate vs. leave manual?**

I ask, "Will the effort to automate this test give more than it takes?" This question gets to one of the main points of automated testing, which is that not every test should be automated.

Good candidates for automation are test scenarios that are repeatable, provide meaningful coverage, and have the potential to catch real bugs in production.

<br>

> **What role does automated testing play in a CI/CD workflow?**

Automated testing is the quality gate inside a CI/CD pipeline. Every change triggers test runs at the unit, integration, API, and UI layers. If a test fails, the pipeline stops and the team receives fast, precise details instead of discovering bugs in Production.

The key value is to catch issues early on in the dev cycle.

For example, a unit test failure costs minutes to fix. The same bug found after a deployment can cost hours or even days. Adding automated testing to the CI/CD workflow builds quality into every deployment, rather than discovering bugs after the fact.

<br>

> **How do you resolve a flaky automated test?**

The first step I take is to look at the execution history of the test and answer the following:

- Is this test failing randomly or is there a pattern?
- Is the test failing at the same step when it fails?
- Is the test consistently using the same config values and test data?
- Is there a particular agent runner being used when the failures occur?

My goal is to identify dependencies that may be causing the test's flakiness.

If those are good, my next step is to pull down the test and run it locally. I complete multiple test runs and try to replicate the flakiness. If I am successful, I then debug through the test execution in the IDE and identify the point of failure.

Once identified, I document the issue, fix the root cause, and verify the test is stable across multiple runs before closing it out.

<br>

> **If the quality signal was poor prior to a release and you recommended a delay, how would you handle pressure to release anyway?**

My job in that moment is to make sure decision-makers have a complete, honest picture of quality. I document all outstanding issues, communicate the risks clearly, and ensure that information is visible to stakeholders before any go/no-go decision. After that, it's a leadership call.

---
