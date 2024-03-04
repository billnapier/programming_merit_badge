## Requirement 5a

At the time of writing, the [requirement](https://www.scouting.org/merit-badges/programming/) reads:

```
With your counselor's approval, choose a sample program. Modify the code or add a function or subroutine to it. Debug and demonstrate the modified program to your counselor.
```

We're going to do this requirement in Javascript.  There is an existing program here that does temperature conversion from Farenheit to Celcius.

### Run the program

This project is already setup with a launch configuration to run the server so we can serve our web page.  In Codespaces, click on the icon all the way on the left that looks like a triangle with a bug on it. (Hover text in "Run and Debug").  You can also just hit Ctrl-Shift-D to get there.

At the top of the page, you should see the title "RUN AND DEBUG" with a green arrow next to it and the words "req5a server".  This is the server we want to run, so just hit the green triangle (it's like a play button).

This will open a terminal at the bottom in which the server is now running.  The only thing you need to know about this area is the trashcan icon will kill the server, in case you need to start it again.  In my experience, you need to wait a few seconds (maybe 10) for the network resources to clean up before restarting the server.

Now when the server starts up, Codespaces detects this and asks if you want to open this page in your browser.  Hit YES and you should get the "Temperature Conversion" app running in your browser.