# Feed Reader Test
> Udacity Frontend Nanodegree Project 8

This project was focused on using Test Driven Development (TDD) create a simple web-based application that reads RSS feeds. I was given a list of tests that I had to create with the [JasmineJS](https://jasmine.github.io/) testing framework. Once I finished writing the tests I had to create the application with the feedback that I got from each test result.


## Development
I used [JasmineJS](https://jasmine.github.io/) a very popular testing framework for javascript application. The tests can be found in [feedreader.js](jasmine/spec/feedreader.js).



### Test Example

```javascript
describe('RSS Feeds', function() {

		it('are defined', function() {
				expect(allFeeds).toBeDefined();
				expect(allFeeds.length).not.toBe(0);
		});


		it('are urls', function () {
			for (var i = 0; i < allFeeds.length; i++) {
				expect(allFeeds[i].url).toBeDefined();
				expect(allFeeds[i].url.length).not.toBe(0);
			}
		});

	 it('are names', function () {
		 for (var i = 0; i < allFeeds.length; i++) {
			 expect(allFeeds[i].name).toBeDefined();
			 expect(allFeeds[i].name.length).not.toBe(0);
		 }
	 });
});
```
