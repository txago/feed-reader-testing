# Feed Reader Testing
This is the fourth project from the **Front-End Web Developer Nanodegree** by **Udacity**. It's a web-based application that reads RSS feeds and my challenge was to **complete the test suite** using **Jasmine**.

Practicing **TTD (Test-Driven Development)** is a good way to guide your development process, as it allows you to create a testable software at the forefront. By the time you're done with development, you already have a tested software that can be pushed to production and that will certainly work.

## Process
1. In the first test, I used the `forEach` method to loop within the `allFeeds` object and check if there was an `url` element defined in the array. I used the `length` property and `not.toBe` expectation to check the existence of the element.
2. The second test was basically the same, but this time I wanted to check the `name` element inside the array.
3. In the third test, I accessed the `body` element using the document object with the `hasClass` method, to check if the element had the `menu-hidden` CSS class set by default.
4. The fourth test was about triggering `click()` events, to expect the existence of the `menu-hidden` class on the `body` element and, with that, the visibility change of the menu.
5. In the Initial Entries test suite, I used the `beforeEach` hook and asynchronous `done()` function so that I could check if the `.entry` element, combined with the `length` property, would correctly answer the `toBeGreaterThan(0)` expectation.
6. For the last, and most difficult test suite, I reused the same hook and asynchronous function from the previous test, added a callback with a new instance of the same element ant then compared them with a `not.toEqual` expectation.

## How to run the test
Download or clone this repository and open the `index.html` file in your favorite browser. You can also [access the RSS Feed application test page](https://txago.github.io/feed-reader-testing/).

## Resources
[Front-End Nanodegree Feed Reader](https://github.com/udacity/frontend-nanodegree-feedreader) by [Udacity](https://github.com/udacity)
