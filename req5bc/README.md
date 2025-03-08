# Requirements 5b and 5c project ideas

WARNING: The program must take input and produce output based on computations and decisions made on the input.


For these two projects you need to work on, please check with me before starting
on them. I'd like to know two things:

1.  What programming language are you looking to use?
1.  What are you planning on doing?

It's important to talk to me before starting you projects because I want to
ensure that you have a good time with this work. Which means both ensuring that
the project you want to do is reasonable for your skill level, and also ensruing
that the tech stack/programming language isn't going to frustrate you.

## Different Tech Stacks to Look At

### Online Options

This is very much the easiest way to go.  For the "it must take input" requirements here if you can change a constant and re-run it in the program, that will count.  Better yet, give me test cases.

#### Scratch

https://scratch.mit.edu/

Online visual programming tool.  Very very very good for beginners, as you can drag and drop your control blocks to make things happen (vs. having to type in the code).

#### Javascript

http://script.google.com/

This is a javascript runtime with an AppScript specific binding (vs. the standard DOM bindings you'd get from a web browser).  

This is a super powerful tool, I've built entire complicated websites on top of it for work.  It also has tight integration with Google Docs, so you can do things like "run this script when somebody submits a form entry".

http://codepen.io/ 

This is an interactive HTML/CSS/JS tool to quickly do rapid webpage devleopment.  Similar to the above, but gives you the standard HTML DOM.

#### Golang Playground

https://go.dev/play/

Golang is the new python - people really like it because it's fast and compiles down really small.

#### Java Playground

https://dev.java/playground/

#### Rust Playground

https://play.rust-lang.org/

This is the only hosted playground I could find that would actually allow interactive input.

#### Installed Options

There are about a million different ways to do this with every language ever invented.  Including downloading the toolchain to your computer and installing it.

My preference is always to use GitHub Codespaces.  This is a web hosted environment that gives you VSCode in your browser, and a shell in which you can install any toolchain and run it.  It by default comes with a bunch.  In fact, this is how I do some of my work.

### Project Ideas

I'm outlining some project ideas here to make sure you don't get stuck trying to
come up with something. Feel free to pick something from this list to work on,
but also if you have an idea of your own that really interests you, do it!

#### Magic Eight Ball (easy)

![Magic Eight Ball](ball.webp)

Links:
*  https://en.wikipedia.org/wiki/Magic_8_Ball
*  https://youtu.be/WSaS17CSS4c

The Magic Eight Ball was a toy where you asked it a question and then would
shake it up. When things settled, it would give you one of a number of answers
depending on which side of the shape inside happend to come up to the viewport.

I've inlcuded the stock respones (from the Wikipedia page) here:

*  It is certain
*  It is decidedly so
*  Without a doubt
*  Yes definitely
*  You may rely on it
*  As I see it, yes
*  Most likely
*  Outlook good
*  Yes
*  Signs point to yes
*  Reply hazy, try again
*  Ask again later
*  Better not tell you now
*  Cannot predict now
*  Concentrate and ask again
*  Don't count on it
*  My reply is no
*  My sources say no
*  Outlook not so good
*  Very doubtful

For this assignment, you should:

1.  Ask the user for a question to answer.
2.  Pick (at random) one of the stock responses from above to return as the answer.
3.  Keeping doing this in a loop, starting from #1

> [!TIP]
> For bonus points, come up with your own respones!  Be creative!

This project would be super easy and fun in scratch.

#### Guess the number (easy)

This is a simple number guessing game.  You've probably played it with a sibling or someone in the car on a long car trip.

1. Have the computer pick a (secret) random number from 1 to 100
2. Have the user guess a number.
3. The computer then says if the picked number is higher or lower, or if was guessed correctly.  If guessed correctly, start over at #1 and start the game over.
4. If not guessed correctly, after saying high or low, go back to #2 to get another response
5. Along the way keep track of how many guesses the user took along the way.  Report it when they guess correctly.

##### Example

Secret number is 42.

```
Guess: 50
Lower
Guess: 25
Higher
Guess: 38
Higher
Guess: 44
Lower
Guess: 41
Higher
Guess: 42
Correct.  It took you 6 guesses.
```
> [!TIP]
> With a smart guesser, can you tell me what the maximum number of guess is?

You can also try changing the game to be any arbitrary range, including asking
the user what the range is. "My number is between 13 and 133". In this case,
with a smart guesser can you tell me the formula for what the maximum number of
guesses are?

#### Backwards Guess The Number (med)

This is like the game above, but swap who is picking the secret number and who is guess.  Yes, that means the human picks a number from 1 to 100 and the computer tries to guess it.

#### Eagle Required Merit Badge (easy)

1. Ask the user to enter a merit badge name.
2. If this is not a merit badge, tell the user that it is not a merit badge.
3. If it is a silver banded, Eagle required merit badge, tell the user it is an Eagle Required Merit Badge.
4. Otherwise tell the user it is a Regular Merit Badge

```
Please enter merit badge> Communications
This is an Eagle Require Merit Badge
Please enter merit badge> Programming
This is not an Eagle Require Merit Badge
Please enter merit badge> Parkour
This is not a valid merit badge.
```

To help with this project, I've provided a data file of [Merit Badges](merit_badges.txt) and [Eagle Required Merit Badges](eagle_merit_badges.txt)

This could be done in any of the tools, especially the online ones.

#### Avg of X random numbers (easy/med)

1. Ask the user to enter the number of random numbers to generate.
2. Generate X random numbers between 0 and 100 (X is based on the input to #1).
3. Calculate and print out the average (arithmetic mean) of those random numbers.

> [!TIP]
> Can you predict what the answer is going to be here?

#### Pig Latin Translator (medium)

This one is just a touch harder, but arguably a lot more fun.

Borrowing from: https://web.ics.purdue.edu/~morelanj/RAO/prepare2.html

1. If a word starts with a consonant and a vowel, put the first letter of the word at the end of the word and add "ay."
2. If a word starts with two consonants move the two consonants to the end of the word and add "ay."
3. If a word starts with a vowel add the word "way" at the end of the word.

Examples

| word    | iglatinpay |
| ------- | ---------- |
| pig     | igpay      |
| hello   | ellohay    |
| child   | ildchay    |
| awesome | awesomehay |

> [!NOTE]
> Translating from Pig Latin into English is a bit harder of a problem.  Want to take a crack at it?  If not, maybe you want just discuss with me how to do it?