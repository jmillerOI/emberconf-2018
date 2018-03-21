# The Next Generation of Testing

- andThen()
  - almost 5 years old
  - mixes sync and async code
  - unintuitive API
  - Now replaced with async/await
  
- jQuery
  - now using `ember-native-dom-helpers` instead using straight jquery but focuses on the DOM API
  - `@ember/test-helpers` only owrk in updated, while `ember-native-dom-helpers` can be used in either or
  
- Mocha 
  - Nested Modules
  
### 4 Types of Tests
- Plain QUnit Test 
  - for code unrelated to Ember
- "Container" tests
  - for Controllers, Routes, Services (previously U/I tests)
- Rendering Tests
  - for Components and Helpers
- Application test
  - to verify user stories
  
Check `ember-cli-qunit` version `4.2.x+`

### Migration
- async/await instead of andThen
- ember-native-dom-helpers `ember-native-dom-helpers-codemod` auto-mod code for updating tests
- setupTest() Functions `ember-qunit-codemod`
- `@ember/test-helpers` `ember-test-helpers-codemod`

### Tips & Tricks

#### Mocking
aka taking advantage of inject()

#### Loeading States

#### Custom Test Helpers
aka registerAsyncHelper

#### Test Selectors
the thing you know from CSS

`ember-test-selectors` for using `data-test-*` selectors

#### Readable Asserotions

`qunit-dom` ember addon to assert items on the dom
  

[Video](https://youtu.be/qfnkDyHVJzs?t=17882)
[Slides](https://speakerdeck.com/turbo87/the-next-generation-of-testing-in-ember-dot-js)

##### Speaker
Tobias Bieniek

