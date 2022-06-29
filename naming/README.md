# Naming

When talking about naming we're referring to variable, method, class and packages. The project name is a more personal scope although it has a few restrictions you should follow to talk the current industry language.
We're gonna have a look at both conventions and best practices in order to get the best and most useful names in our code to keep our projects as much RUM.
Something that applies to all the namings is the consistenciy and self-explanatorietiness: if we're using length as a variable, we'll be refering to everything related with length-like terms, we won't mix size, which is equivalent in some sort with lenght, but might lead to confusion. And as for the getting some self-explanatory names, we're expecting names to be as short as they can as long as they describe the intention properly. We're to avoid acronyms unless they're more widely known in such form than the long one (PDF, URL).
In the code there will be more explanations giving more insight why an approach is better than other.

# Conventions
- Variables: 
	- Instance variables: The attributes of a class, declared inside a class but outside methods. Here we're supposed to use camelCase, and start our variable name with a letter.
	- Class variables: One variable per class type. No matter how many instances of given class we have, the value of this variable will always be the same, so we write them down, again with camelCase, unless this is a constant, this is, the variable it self has the final modifier, here we'd capitalise the whole word and each word would be separated with an underscore. Notice this goes for both private and public constants.
	- Local variables: This ones are defined within the scope of a method so they will not exist anymore once the method is finished. We name them with camelCase. Parameters count as local variables with the peculiarity that if the parameter type is a primitive (int, double, etc) even if you modify the value it won't be retained after completing the method (parameter by value), but if it was to be an object, the way java works, any changes you perform in the attributes of the object will persist after the method is completed.
- Methods: Methods should always be named with camelCase.
- Class: Classes should always be named using PascalCase. This goes for Enumerations and Interfaces too.
- Packages: Packages are to be named all in lowercase, with no underscore. The prefix of the package should be a TLD domain (com, edu, gov, etc...) or a two-letter country code (es, fr, de, etc...). There can be several words in the same package.

# Best Practices

- Variables: When it comes to best practice in naming variables it's all about choosing a name that properly describes what it's holding. For this purpose in java we're not supposed to save space, it's not more efficient nor fatter to give long variable names. Actually it helps the next developer coming to read the code to understand what's that variable supposed to represent. For this we're using nouns when declaring our variables unless its a boolean variable, where we'd use a small question formed name, anything that can be answered just by yes or no.
- Methods: Methods represent actions, so they're to be named as verbs, containing the actions they perform.
- Class: Class names should be nouns, now this one is complicated because we usually tend to have to substantiate verbs since given class function is to perform some action.


# Sources
- https://docs.oracle.com/javase/tutorial/java/nutsandbolts/variables.html
- https://www.oracle.com/java/technologies/javase/codeconventions-namingconventions.html#:~:text=Methods%20should%20be%20verbs%2C%20in,of%20each%20internal%20word%20capitalized.&text=Except%20for%20variables%2C%20all%20instance,words%20start%20with%20capital%20letters.