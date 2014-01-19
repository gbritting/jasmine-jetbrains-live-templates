#Introduction

###[Jasmine](http://jasmine.github.io/) Live Templates for use in [JetBrains](http://www.jetbrains.com) IDEs.

Live templates are abbreviations that are expanded into code fragments that you use to insert frequently-used code blocks into your source code. Live templates are a huge productivity boost, especially when constructing unit-tests where you will find yourself repetitively creating suites and specs.

###Why These Are Different

There are other Jasmine live templates out there but with these we have simplified the act of remembering the abbreviations used as the expansion characters for the code fragment. Generally, you start with *j* for **J**asmine, then use the humps in the [camel-case](http://en.wikipedia.org/wiki/CamelCase) Jasmine function or Jasmine matcher name.

For instance, *jbe*, **J**asmine **b**efore**E**ach, would expand the `beforeEach` live template giving you a Jasmine `beforeEach` setup function.

<pre><code>beforeEach(function () {

});
</code></pre>

 *jtb*, **J**asmine **t**o**B**e would expand the `toBe` matcher Live Template giving you a Jasmine `toBe` expect matcher.

<pre><code>expect('actual').toBe('expected');</code></pre>

Every matcher Live Template also has a negative assertion (not) Live Template. For instance,

*jntb*, **J**asmine **n**ot **t**o**B**e would expand the negative `toBe` matcher Live Template giving you a Jasmine `not.toBe` expect matcher.

<pre><code>expect('actual').not.toBe('expected');</code></pre>

##Installation
Copy the xml file to the following location:

* **Windows:** &lt;your home directory&gt;\\.&lt;product name&gt;&lt;version number&gt;\\config\\templates
* **Linux:** ~\\.&lt;product name&gt;&lt;version number&gt;\\config\\templates
* **MacOS:** ~/Library/Preferences/&lt;product name&gt;&lt;version number&gt;/templates

Once copied, you should see them in the IDE (WebStorm, IntelliJ, etc.) under File -> Settings -> IDE Settings -> Live Templates

##Suite, Spec, Setup and Teardown Live Templates
<small>(NOTE: these first 3 do not follow the camel-case abbreviation)</small>

`jdes` - Jasmine Suite
    
    describe('suite title', function () {
 
    });

`jit` - Jasmine Spec

    it('spec title', function () {
    
    });

`jits` - Jasmine Spec with spec title started with word Should

    it('should ', function () {

    });

`jbe` - **J**asmine **b**efore**E**ach (setup)

    beforeEach(function () {

    });

`jae` - **J**asmine **a**fter**E**ach (teardown)

    afterEach(function () {

    });

## Matchers
`jtb` **t**o**B**e `expect(x).toBe(y));`

`jtbd` **t**o**B**e**D**efined `expect(x).toBeDefined());`

`jtbf` **t**o**B**e**F**alsy `expect(x).toBeFalsy());`

`jtbgt` **t**o**B**e**G**reater**T**han `expect(x).toBeGreaterThan(y));`

`jtblt` **t**o**B**e**L**ess**T**han `expect(x).toBeLessThan(y));`

`jtbn` **t**o**B**e**N**ull `expect(x).toBeNull());`

`jtbt` **t**o**B**e**T**ruthy `expect(x).toBeTruthy());`

`jtbu` **t**o**B**e**U**ndefined `expect(actual).toBeUndefined();`

`jtc` **t**o**C**ontain `expect(x).toContain(y));`

`jte` **t**o**E**qual `expect(x).toEqual(y));`

`jtm` **t**o**M**atch `expect(x).toMatch(y));`

`jtt` **t**o**T**hrow `expect(fn).toThrow(e));`

#### Negated Matchers
`jntb` **n**ot **t**o**B**e `expect(x).not.toBe(y));`

`jntbd` **n**ot  **t**o**B**e**D**efined `expect(x).not.toBeDefined());`

`jntbf` **n**ot  **t**o**B**e**F**alsy `expect(x).not.toBeFalsy());`

`jntbgt` **n**ot  **t**o**B**e**G**reater**T**han `expect(x).not.toBeGreaterThan(y));`

`jntblt` **n**ot  **t**o**B**e**L**ess**T**han `expect(x).not.toBeLessThan(y));`

`jntbn` **n**ot  **t**o**B**e**N**ull `expect(x).not.toBeNull());`

`jntbt` **n**ot  **t**o**B**e**T**ruthy `expect(x).not.toBeTruthy());`

`jntbu` **n**ot  **t**o**B**e**U**ndefined `expect(actual).not.toBeUndefined();`

`jntc` **n**ot  **t**o**C**ontain `expect(x).not.toContain(y));`

`jnte` **n**ot  **t**o**E**qual `expect(x).not.toEqual(y));`

`jntm` **n**ot  **t**o**M**atch `expect(x).not.toMatch(y));`

`jntt` **n**ot  **t**o**T**hrow `expect(fn).not.toThrow(e));`
