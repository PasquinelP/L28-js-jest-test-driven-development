Met Test Driven Development schrijf je dus eerst de test en schrijf je daarna pas de code die de test doet slagen (in plaats van anders om).

Probeer met de **RED, GREEN, REFACTORING** methode de onderstaande opdrachten op te lossen.

Schrijf de functie die onderstaande test doet slagen:

1 Schrijf de functie....

    const addOne = function(numbers) {
      // Schrijf hier de functie...
    }
    module.exports = addOne;

... die onderstaande test doet slagen:

    const addOne = require("./add-one.js");

    test("Add 1 to each item in myArray", function() {
      const myArray = [31, 57, 12, 5];

      const unchanged = [31, 57, 12, 5];
      const expected = [32, 58, 13, 6];
      const output = addOne(myArray);

      expect(output).toEqual(expected);
      expect(myArray).toEqual(unchanged);
    });

2 Schrijf de functie....

    const getWordLengths = function(someWords) {
        //Schrijf je functie...
    };

    module.exports = getWordLengths;

... die onderstaande test doet slagen:

    const getWordLengths = require("./get-word-lengths.js");

    test("Get word lengths", function() {
      const words = ["sun", "potato", "roundabout", "pizza"];
      const expected = [3, 6, 10, 5];

      const output = getWordLengths(words);
      expect(output).toEqual(expected);
    });

3 Schrijf de functie....

    const findNeedle = function(words) {
      // Schrijf hier de functie...
    };

    module.exports = findNeedle;

... die onderstaande test doet slagen:

    const findNeedle = require("./find-needle.js");

    test("Find the needle", function() {
      const words = ["house", "train", "slide", "needle", "book"];
      const expected = 3;

      const output = findNeedle(words, "needle");
      expect(output).toEqual(expected);
    });

