# js-test
A test-framework for hierarchical JavaScript module tests, based on HTML, CSS and JavaScript.

## Overview
A module test is defined in an HTML file. This is the module test document. The document contains a number of tests, written in JavaScript. Tests can be oranized into (collapsible) sections. This gives structure to the test document and improves readability.
A parent test document can import child test documents into HTML IFRAMEs. They are handled like individual tests, but combine the results of an entire module test document.

So, with test sections and imported module test documents we can create a rather flexible module test structure. Module tests are re-usable and can be combined into different test suites.  

Module and section summaries provide condensed status information and guide the developer to the failed tests, even in very complex structure. The module summary in the topmost document indicates whether the entire suite failed or succeeded.


<img src="https://github.com/bassmationcode/js-test/blob/main/docs/img/fig-001.png?raw=true" alt="First impression" width="200"/>


## Usage
An author creates an HTML module test document and calls test functions defined in the js-test.js library. The library functions add HTML content to the test document, according to test result, and update the summaries up to the root document in a hierarchical structure.
