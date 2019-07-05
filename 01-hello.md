# Chapter 1: Hello!

Yes, I know, I've already said hello, I'm talking about the programming language.
Let's say hello to Python. Or rather, have it say hello back!

## The ins and outs

The first thing to learn about Python, or rather about *any* programming language, is
that it has an input and an output. Think about a calculator. You type in the numbers and
the operations (input), and you see the result on the screen (output). Pretty straightforward,
isn't it?

Although a program *can* run without an input, it rarely is the case. It's just plain boring.
But we gotta start somewhere, don't we?

## Hot off the printing press

Heard about "Hello world"? This is what some programmers use to say hello to a
programming language, which they're new at. We're gonna do just the same.
Let's start with the most basic... well, *statement*, that every Python user should now.  
It goes like this:

```python
print("こんにちは世界")
```

"WHAT?! I don't even have a printer! And what is that crazy writing?" Don't worry. First,
this `print` has nothing to do with your actual printer. It writes output! This is what we're gonna
use to inform the user about something. Second, this is "Hello world" in
Japanese, just to show you that Python supports almost every character in existence.

> Note: "Print" here is a historical term. Before the [ENIAC](https://en.wikipedia.org/wiki/ENIAC),
>       computers communicated with people through [teleprinters](https://en.wikipedia.org/wiki/Teleprinter)
>       (or teletypewriters), which *print* out actual characters, hence the name "print".

Now let's try it out! Grab your IDE and your keyboard, and try to `print` something to the screen.

> Note: Please do not leave out the quotation marks! (`"`) They are **always** required when dealing with text (string).
>       This will be further discussed in the chapter Variables.
<!-- TODO: Link the variables chapter -->

Did it work? It did, didn't it? Now let's try something else!

## Math Wars

```python
print(2 + 2 * 4)
```

Try to guess the output of this `print`. Yes, Python knows about [operator precedence](https://en.wikipedia.org/wiki/Order_of_operations).
The answer is `10`. Pretty straight forward, isn't it? Just a multiplication, then an addition.

No quotes? Exactly. In most programming languages, including Python, letters specify instructions. If you were to write
`print(whatever)`, then python would search for something called `whatever`. Because "whatever" is not defined, Python
has to "raise" an error. (We'll talk about errors later in the corresponding chapter.) To tell Python that our text
should be left alone, we wrap it in quotation marks (to show that they should be taken *literally*).
<!-- TODO: Link chapter(s?)! -->

## But how does a point float?

Let's see if we have fractions:

```python
print(1 / 2)
```

You got `0.5`, right? Exactly! Python knows fractions! :tada:  
:warning: But.. before we party... uh... how should I put this... Try the following:

```python
print(0.3 * 3)
```

The result should be `0.9`, right? Sadly, no. Not exactly. This is the result of *floating-point math*.
Your PC's processor is unable to represent `0.3 * 3` exactly in binary. It becomes an endless fraction
(3 * 0.01001100110...). Think about it like `1/3` in decimal (0.3333...). It never reaches the exact value,
thus it cannot be converted exactly. Read more [here](https://docs.python.org/3/tutorial/floatingpoint.html).
