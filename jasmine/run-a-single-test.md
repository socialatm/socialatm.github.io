Running a single test suite
By using `fdescribe` (think of it as a focused describe), Jasmine will only run that particular test suite.

    fdescribe('Awesome feature', function () {
      // ... specs here
    });
Running a single spec
By using `fit` (think of it as a focused it), Jasmine will run only that particular spec.

    describe('Awesome feature', function () {
      fit('should check whether `true` is really `true`', function () {
        expect(true).toBe(true);
      });
    });
So here you go. If you need to run a single test suite/spec, you can quickly do so by using fdescribe and fit.****


***
The simplest way to ignore a test or a test suite in Jasmine is to prefix the `describe` or `it` function with an `x`. This will mark the test or the test suite as pending and exclude it from the execution and the report.