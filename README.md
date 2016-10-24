karma-enzyme
===========

[Enzyme](http://airbnb.io/enzyme) for [karma](https://karma-runner.github.io)

Installation
------------

Install the module via npm

```sh
$ npm install karma-enzyme enzyme --save-dev
```

Add `enzyme` to the `frameworks` key in your Karma configuration:

```js
module.exports = function(config) {
  "use strict"

  config.set({
    #...
    frameworks: [ "mocha", "enzyme"],
    #...
  })
}
```

**Example**
```jsx
describe("karma tests with enzyme", function () {

    it("should expose thi Enzyme shallow method", function () {
        const wrapper = shallow(<MyComponent />)
        #...
    })

    it("should expose thi Enzyme mount method", function () {
        const wrapper = mount(<MyComponent />)
        #...
    })

    it("should expose thi Enzyme render method", function () {
        const wrapper = render(<MyComponent />)
        #...
    })

})
```
