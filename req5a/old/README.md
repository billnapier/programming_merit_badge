## Requirement 5a

At the time of writing, the [requirement](https://www.scouting.org/merit-badges/programming/) reads:

```
With your counselor's approval, choose a sample program. Modify the code or add a function or subroutine to it. Debug and demonstrate the modified program to your counselor.
```

We're going to do this requirement in Javascript.  There is an existing program here that does temperature conversion from Farenheit to Celsius.

### Run the program

This project is already setup with a launch configuration to run the server so we can serve our web page.  In Codespaces, click on the icon all the way on the left that looks like a triangle with a bug on it. (Hover text in "Run and Debug").  You can also just hit Ctrl-Shift-D to get there.

At the top of the page, you should see the title "RUN AND DEBUG" with a green arrow next to it and the words "req5a server".  This is the server we want to run, so just hit the green triangle (it's like a play button).

This will open a terminal at the bottom in which the server is now running.  The only thing you need to know about this area is the trashcan icon will kill the server, in case you need to start it again.  In my experience, you need to wait a few seconds (maybe 10) for the network resources to clean up before restarting the server.

Now when the server starts up, Codespaces detects this and asks if you want to open this page in your browser.  Hit YES and you should get the "Temperature Conversion" app running in your browser.

### Now let's modify it

There is another temperature scale used in science called Kelvin.  We are going to add in support to this program to convert to and from Kelvin, as well as Celsius and Farenheit.  For reference:

$K = (F-32) / 1.8 + 273.15$
$F = (K-273.15) * 1.8 + 32$

#### Requirements

1.  We should be able to input a Farenheit temperature and get both the Celsius and Kelvin results.
1.  We should be able to input a Celsius temperature and get both the Farenheit and Kelvin results
1.  We should be able to input a Kelvin termperature and get both the Farenheit and Celsius results.

#### Testing

It's always useful to know what the answers should be, so you can make sure your code is correct.

| Farenheit | Celsius | Kelvin |
|-----------|---------|--------|
| 32        | 0       | 273.15 |
| 212       | 100     | 373.15 |
| 82.4      | 28      | 301.15 |

## Scratch

You can also do this same exercise in scratch if that's more your speed.  I've included a link to a project to get started with:  https://scratch.mit.edu/projects/978090795/