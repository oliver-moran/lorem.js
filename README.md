# Lorem.js #

A JavaScript library to generate placeholder text in "Lorem ipsum..." style.

Uses a wordbase from the original [Liber Primus](https://la.wikisource.org/wiki/De_finibus_bonorum_et_malorum/Liber_Primus) text.

Usage:

    Lorem.getWord(); // returns a word
    Lorem.getSentence(); // returns a sentence
    Lorem.getParagraph(); // returns a paragraph

To start a sentence or paragraph with "Lorem ipsum":

    Lorem.getSentence(true); // Lorem ipsum... (sentence)
    Lorem.getParagraph(true); // Lorem ipsum... (paragraph)

To use Lorem.js with Node.js:

    var Lorem = require('lorem.js').Lorem;

## Settings ##

A settings object can be tweaked to generate more or less verbose output. The available settings (and their default values) are:

    Lorem.settings.sentence.min // the min number of words in a sentence (default: 2)
    Lorem.settings.sentence.max // the max number of words in a sentence (default: 10)
    Lorem.settings.paragraph.min // the min number of sentences in a paragraph (default: 3)
    Lorem.settings.paragraph.max // the max number of sentences in a paragraph (default: 10)
    Lorem.settings.comma.rate // the average number of mid-sentence words before a comma (default: 10)
