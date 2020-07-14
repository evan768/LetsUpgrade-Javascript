# LetsUpgrade-Javascript
Javascript essentials batch 1 day 1

1. Various methods in console function:
   a. console.log() : Mainly used to log(print) the output to the console. We can put any type inside the log(), be it a string, array, object, boolean etc.
   b. console.error() : Used to log error message to the console. Useful in testing of code. By default the error message will be highlighted with red color.
   C. console.warm() : Used to log warning message to the console. By default the warning message will be highlighted with yellow color.
   d. console.clear() : Used to clear the console. The console will be cleared, in case of Chrome a simple overlayed text will be printed like : ‘Console was cleared’ while in firefox no message is returned.
   e. console.time() and console.timeEnd() : Whenever we want to know the amount of time spend by a block or a function, we can make use of the time() and timeEnd() methods provided by the javascript console object. They take a label which must be same, and the code inside can be anything( function, object, simple console).
   f. console.table() : This method allows us to generate a table inside a console. The input must be an array or an object which will be shown as a table.
   g. console.count() : This method is used to count the number that the function hit by this counting method.
   h. console.group() and console.groupEnd() : group() and groupEnd() methods of the console object allows us to group contents in a separate block, which will be indented. Just like the time() and the timeEnd() they also accepts label, again of same value.
   i. custom console log : User can add Styling to the console logs in order to make logs Custom . The Syntax for it is to add the css styling as a parameter to the logs which will replace %c in the logs.

2. Differences between var, let, const:
   a. var: The scope of a variable defined with the keyword “var” is limited to the “function” within which it is defined. If it is defined outside any function, the scope of the variable is global. var is “function scoped”.

    var tester = "hey hi";
    
    function newFunction() {
        var hello = "hello";
    }
    console.log(hello); // error: hello is not defined

   b. let: The scope of a variable defined with the keyword “let” or “const” is limited to the “block” defined by curly braces i.e. {} . “let” and “const” are“block scoped”.

   let greeting = "say Hi";
   let times = 4;

   if (times > 3) {
        let hello = "say Hello instead";
        console.log(hello);// "say Hello instead"
    }
   console.log(hello) // hello is not defined

   c. const: The scope of a variable defined with the keyword “const” is limited to the block defined by curly braces. However if a variable is defined with keyword const, it cannot be reassigned. “const” cannot be re-assigned to a new value. However it CAN be mutated.

    const greeting = "say Hi";
    greeting = "say Hello instead";// error: Assignment to constant variable. 

3. Common data types in Javascript:
   a. String: A string is a collection of alphanumeric characters. I start a string by typing double quotes, single quotes, or the backtick character. Double quote and single quote behave identically, and the backtick character comes with some extra functionality.
   b. Booleans: Booleans have two values. True and false. When we create a boolean, we’re simply saying it’s true or it’s false. It’s like that on/off switch example that we talked about. It’s all there is to them right now. We’re gonna talk into other aspects of playing into these variables in another time.
   C. Numbers: Numbers are as straightforward as they sound. Numbers are for numbers. I can’t put a letter on here. It’s no longer a number, and the coloring gets funky. It’s no longer green. But I can make this number be as long as I want it. I cannot add a comma, but I can add a decimal point. So numbers are any integer or decimal number created in the language, and they’re used for money, age, etc. the same kinds of things that we use money for here in real life.
