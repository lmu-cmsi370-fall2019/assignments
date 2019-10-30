# Combined Front End Submission Instructions
This document intends to provide a specification for submitting a combined submission of Assignments 1029 and 1114. Assignment 1114 was meant to build on the same repository as Assignment 1029 anyway, so this shouldn’t be too much of a stretch. The goal here is to make it easy—_really_ easy—to switch between having a mock runtime API vs. a real one that makes real network connections.

## General Instructions
1. Work on Assignment 1029 (now due 1114) until it is finished.
2. Work on Assignment 1114 until it is finished. (feel free to tweak the overall application as well)
3. When completely done, prepare/copy/name your files as given in the following instructions.
4. Don’t forget to verify that both versions of your application still work! (and that tests still pass)

## iOS App Instructions
1. Make sure that the code base has two runtime implementations of the `Api` protocol. Call the hardcoded implementation `PlaceholderApiService` and call the real request implementation `RealApiService`. (you may place each implementation in its own file but due to how Swift handles files, this isn’t absolutely necessary)
2. As submitted, your front end should use `PlaceholderApiService`.
3. To switch from one implementation to the other, one must only exchange all `Api` implementation instantiations within the app (not within tests). For example, searching and replacing `PlaceholderApiService` with `RealApiService` should switch from the hardcoded to the real request implementation.
4. Tests should still pass (and use the proper mock implementation) regardless of what implementation is used at runtime.

## Web App Instructions
1. Make sure that each implementation alternative for your API functions resides in its own file. Call the hardcoded implementation _api.js-placeholder_ and call the real request implementation _api.js-real_.
2. Copy _api.js-placeholder_ into _api.js_ so that, as submitted, your front end uses the hardcoded implementation.
3. To switch from one implementation to the other, one must only copy the desired implementation to _api.js_. For example, copying _api.js-real_ as _api.js_ should switch from the hardcoded to the real request implementation.
4. Tests should still pass (and use the proper Sinon stubs) regardless of what implementation resides in _api.js_.
