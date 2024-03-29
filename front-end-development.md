**CMSI 370** Interaction Design, Fall 2019

# Assignment 1029

Now that you have your design and some startup know-how, you must be itching to start implementing it. So now we will, but _in two phases_.

The first phase is solely about the front end. We will leave stubs, placeholders, or mocks at the points where we expect to call our chosen web service APIs. Filling those in will be the concern of [Assignment 1114](./api-integration.md). For this assignment, we focus on the core content of the course: your application’s user interface.

Resources to help you with this include many of the links listed on the course website, assorted samples from the [bazaar](https://github.com/dondi/bazaar) repository, and the starter files that are included with your GitHub Classroom repositories for this assignment, once you have set yourself up.

## Background Reading
For this assignment, you will want to be acquainted with one or more of the development resources listed in the course website, depending on the front end technology stack that you have chosen. You are likely to be consulting those frequently, including other resources that you might discover on your own.

Textbook reading is centered on the menus, forms, and dialogs interaction style, which would be Shneiderman/Plaisant Chapter 6.

For nuts-and-bolts web details (even for React, to a degree), the JavaScript textbook will be of help, particularly Chapter 6, Section 7.5, and Sections 8.2.3, 8.3, 8.4.1, 8.5, and 8.7. For the best exposure, read Chapters 6, 7, and 8 in full.

## Best Practices and Automated Feedback
Starter code for the possible front-end technology stacks is available in the [bazaar](https://github.com/dondi/bazaar) repository:
* jQuery and Bootstrap web app: [giphy-sample](https://github.com/dondi/bazaar/tree/master/giphy-sample)
* React web app using classes: [giphy-sample-react-classes](https://github.com/dondi/bazaar/tree/master/giphy-sample-react-classes)
* React web app using hooks: [giphy-sample-react-hooks](https://github.com/dondi/bazaar/tree/master/giphy-sample-react-hooks)
* iOS application: [giphy-sample-ios](https://github.com/dondi/bazaar/tree/master/giphy-sample-ios)

The web-based starters require [Node.js](https://nodejs.org) and are fully configured for linting ([ESLint](http://eslint.org)), unit tests ([Jest](https://jestjs.io) or [Karma](https://karma-runner.github.io)), and code coverage ([Istanbul](https://github.com/gotwarlost/istanbul), integrated into the test framework). When properly copied into your repositories, these will be run automatically whenever you push to GitHub.

The iOS starter requires [Xcode](https://developer.apple.com/xcode/) and has similar tooling.

### Automated Feedback
In order to connect your repository to [Travis](https://travis-ci.com), our automated code review and feedback system, make sure you completely copy _all_ files from the starter code of your choice. Once these files are committed and pushed, the system will provide feedback on code formatting and quality whenever you commit a new version to GitHub. _Points will be deducted if issues here linger in the final submission._

**Note:** The education subscription for Travis is limited to a single review task at a time, so _don’t all commit at the last minute before the due date_ because the automated feedback will take much longer to get back to you!

## For Submission: A Front End to an Existing Web Service API
The title pretty much says it: put together a front end for a pre-existing web service API. Details on selecting this API and the scope of usage for this API were specified in [Assignment 0919a](./front-end-design.md) and with [Assignment 0919b](./api-setup-tutorial.md) you got some hands-on time using it manually. The key requirement is worth reiterating: we are looking for the implementation of _at least three (3)_ non-trivial web service functions. Also as stated in that assignment, there is a “home-grown” option which, if chosen, hikes the requirement to five (5) specific services.

Technology, coding, and architecture specifics will vary by technology stack, but one specification is common across the board: this assignment expects you to implement _the front end only_ (i.e., no real connections to the web services yet), but also requires that there are _clear, well-defined placeholders_ for those web services in your code. The starter code already has these qualities, so as long as you don’t veer too far from them, you should be fine.

### How to Turn it In
The starter applications can be run/built from within their own subfolders, but for your own submission, _copy all of the files_ from the starter code of choice to the top level of this repository, then start working on those files as your own. This has the secondary effect of keeping the starter code untouched—you’ll probably benefit from that, in case you do something that breaks the application code.

As you then implement your own design, _do_ add, move, rename, and reorganize files as needed. The only things to preserve from the starter code are the tool chain configuration and setup (i.e., linting, testing, Travis) and the overall structure (primarily the API abstraction layer). For everything else, make the code your own.

To evaluate your work, we will invoke or build your application based on the files at the top of the repository.

## Specific Point Allocations
Programming assignments are scored according to outcomes _3a_, _3b_, and _4a_ to _4f_ in the [syllabus](http://dondi.lmu.build/fall2019/cmsi370/cmsi370-fall2019-syllabus.pdf). For this particular assignment, graded categories are as follows:

| Category | Points | Outcomes |
| -------- | -----: | -------- |
| Model Implementation | 20 | _3a_, _3b_, _4a_, _4b_, _4d_ |
| View Implementation | 25 | _3a_, _3b_, _4a_, _4b_, _4d_ |
| Controller Implementation | 25 | _3a_, _3b_, _4a_, _4b_, _4d_ |
| API Stubs/Mocks | 10 | _3a_, _3b_, _4a_, _4b_, _4d_ |
| Test Suite and Coverage | 20 | _4a_ |
| Linting | deduction only | _4c_ |
| Version Control | deduction only | _4e_ |
| Punctuality | deduction only | _4f_ |
| **Total** | **100** |

The last three graded categories are “deduction only,” meaning that you will only get points taken off if there are significant issues with those categories. Such issues include but are not limited to: lingering linting errors as of the final commit (_4c_), insufficiently granular or unmessaged commits (_4e_), and late commits (_4f_).
