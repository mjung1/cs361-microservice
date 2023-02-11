# Random Word Generator
This service generates a random word between 3 and 15 characters long.
## Requirements
You must have a text file called **service.txt** located in the same directory as the python file.
## How It Works

### Requesting Data
The microservice, once activated, will be listening to the **service.txt** file for content indicating that the generate_random_word function should be executed.
The content in the file to execute the function should be as follows:

`run`

The microservice will then execute the function. It first generates a randomly selected length for the word between 3 and 15 characters long. It then makes a call to a random word generator API to generate a random word of that length.

### Receiving Data
The microservice will then erase the **num-service.txt** file, and print to it the randomly generated word, like so:

`['omnidirectional']`

As the end user, you will only need to read the text file after the game is first initiated.

# UML Sequence Diagram
![UML Sequence Diagram for Microservice](UML_Diagram.png)
