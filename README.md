# VueJS Moby Dick Text Sort Application
The purpose of this project is to open and read txt files and modify the imported txt object. Specifically, the goal is to create a list of the top 100 most frequently occurring words, excluding stop words, paired with the count occurrence of the word in the text of Moby Dick.

## Objectives

1. Reformatting text objects
    * Split and rejoin the default 'string' element from reader.result to take out irrelevant words in the stop-words and mobydick txt files
    * Put back words together as an array with many word elements e.g. ["a", "about", "above"].
2. Compare words within stop-words array and mobydick array
    * Take the return value from the functions of stop-words and mobydick array and draw comparison between them.
    * Remove all words from mobydick array that are the same as stop-words.
3. Sort mobydick hash by top 100 most frequent words with count.
    * Ideally have a hash with k = word, v = frequency.
    * Use the sort function and take its reverse to flip asc to desc. Call on the first 100 elements of hash.

## Progress & Challenges

  * All texts have been reformatted in the correct output, e.g. ["a", "about", "above"].
  * Attempted to use the return value of the stop-words and mobydick functions within another function to draw comparison. Return value consistently returned undefined when used outside of the function's local scope. This is a matter to do more research on.
  * Despite failure to use return values, mock-up arrays were used to test the algorithm for removing stop-words from mobydick array. Since the loop only checks the stop-words once, stop-words that appear many times in mobydick are ignored. For improvement, try using different kinds of loops such as map.
  * Due to lack of time and resources, the frequency of the words have not been defined.
  * This application currently does not serve the purpose of filtering out the 100 most frequently occurring words from the text of Moby Dick.
  * Application is able to open text files to load in text. Algorithms written in the app is specific to the txt files mobydick.txt and stop-word.txt; all other files loaded in will have inaccurate display of the number of words.
  * Last note: vue components of the app have been disabled for better understanding of vanilla javascript while writing code.
  * It is hoped that this app can be improved in the future

## Usage and Installation

The application is built on the [vue-simple-boilerplate](https://github.com/vuejs-templates/simple/blob/master/README.md), a template for vue-cli. It is a simplified template for those who want a simple Vue development environment.

``` bash
$ npm install -g vue-cli      # Install vue-cli if you haven't already
$ vue init simple my-project  # Create a new project based on this template
$ cd my-project               # Navigate into your new project folder

$ npm install -g live-server  # Install live-server if you haven't already
$ live-server                 # Run live-server and open it in your browser
```

## Resources

* [vue-cli](https://github.com/vuejs/vue-cli)
* [other vue templates](https://github.com/vuejs-templates/)


