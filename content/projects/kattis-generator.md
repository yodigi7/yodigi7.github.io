---
title: "Kattis Project Generator"
date: "2023-09-30"
description: "I built a Yeoman generator to simplify Kattis challenge setups, supporting Go, JavaScript, and Python. It creates templates with input/output handling, making problem-solving faster and cleaner."
---

I'm just your average software nerd who loves competing on [Kattis.com](https://www.kattis.com/).
But let me tell you, there was this one thing that used to bug the heck out of me: setting up code templates for every new challenge.
It was like déjà vu with every problem.

So, I put my coding skills to good use and created a Yeoman generator that does all the heavy lifting for Kattis problems.

I whipped up a Yeoman generator, tailor-made for Kattis tasks.
With a few magical commands, it conjures up a problem-specific template, complete with input/output handling and everything you need to get started.

No more wasting time on boilerplate code, no siree! I could dive right into the fun part – solving the problems.
And you know what?
It even made my code all neat and consistent.
I always had trouble switching between programming languages on Kattis because I always forgot how to best do the IO handling best since reading from the console is not something that most projects actually need to do.

However, there is still progress to be made.
Currently there are 3 languages currently supported: golang, javascript, and python.
I would love to implement additional languages such as Java and rust.
I would also love to implement an option that would automatically download the test files and generate some test scripts to automatically test the user's code to ensure that it gave the correct answers to the test input.

In the meantime, I thought, "Hey, maybe others could use this too."
So, I shared it with the world on [GitHub](https://github.com/yodigi7/generator-kattis) and [npm](https://www.npmjs.com/package/generator-kattis).

In the wild, ever-exciting world of competitive programming, my little creation shows how a simple frustration can lead to a game-changer.
So, the next time you're on Kattis.com, give my Yeoman generator a whirl, and may your coding challenges be a breeze!