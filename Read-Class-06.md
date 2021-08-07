## NodeJS

1. I am not going to dive directly into the definiton of node, but instead, I think I will find myself doing that talking about the different aspects that make node what it is. As a starter, remember when you used to type JavaScript in order to add a sense of interactivity to static websites maybe to show some animations, to validate forms and so on? Well, notice that all of this has taken place in a single environment which the browser. Doing that alone is kinda boring, and we have more to learn about and do, like building anything from small command line tools to HTTP servers that power dynamic websites.

Stack OverFlow defines node or nodejs as follows: `Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.`

Let's try to break that down. First of all, and as we know about event handling from the old usual environment, the browser, node is a software architecture that promotes the production, consumption and reaction to events, we used that to update the UI for example when the user scrolls down or when he fills a specific form feild and so on. Talking about the next two parts, non-blocking, and asynchronous, they are kind of related to each other, however, as we know, JavaScript is blocking since it is single-threaded, meaning that there is only one call stack where every action like calling a function takes place, but when that function takes so much time, the execution xontext seems to be frozen until the function returns, but advancements has led to creating things called worker threads that handle costly processes that take time and might block the main stack, the thing that led to asynchronous js. Node on the contrary is non-blocking and asynchronous so you won't worry that much about your program getting stuck or being unresponsive. The I/O part is related to handling inputs and outputs, but we are going to talk about the V8 engine next.

2. The V8 engine is a js engine that is implemented into Chromium-based web browsers and it is responsible for compiling JavaScript to machine code, however, this is not quite a traditional compiling, where the code does not get compiled to binary, but instead, it is transformed into syntax that can be *interpreted* by a wider range of browsers.

3. When we talk about node being the runtime for Javascript, it means that node is the runtime environment that specifies the behavior of the elements of the language, or in simpler terms, it is like when we say that Javascript can be executed within node.

4. npm, short for Node package manager, is simply an online service where one can download and upload packages, in addition, it helps installing and managing these packages.

5. My current node version is *14.17.1*.

6. My current npm version is *7.20.3*.

7. To install a package called 'jshint', I would type the following command if I aim to install globally:
```
npm install -g jshint
```
If locally (to a project not for the whole system), and after navigating to that project:
```
npm install lodash --save
```

8. In short, node is used for package management using various tools like npm, module management using webpack, which is basically used to to bundle modules, meaning that it takes all of the different files in our projects and turns them into a single file in order to enhance network performance and other benefits as well. Node is also used for creating back-end applications, something I still don't know much about like at all, and it is also used for creating desktop applications and some command line tools and programs.

## Pair programming

1. Reasons for pair programming are: greater efficiency, engaged collaboration, learning from fellow students, social skills, job interview readiness, and work environment readiness.

2. In my openion the most beneficial reason for pair programmming is engaged collaboration. Aside from the reasons mentioned in the original text, in my openion, when more than one is working on a problem, it is interesting how everyone sees the issue or the plan from his or her perspective, I am always looking for the optimal way to do something, but maybe the one I am working with knows a better way to do the same task, or that his method is more effecient, so this helps on two ways, I improve my performance, and the overall performance of the code will be maintained as well. In addition, this benefits on the long term, not only for a single project which is nice. Add to that that I am someone who usually does things when he feels like it, the thing that in my openion makes me waste lots of time, so having a partner helps since he is relying on you, and you both will be held accountable for your performance. Also, as Daniel Kahnman says in his book "Thinking, Fast and Slow":
**It is much easier, as well as far more enjoyable, to identify and label the mistakes of others than to recognize our own**.

3. In pair programming, usually a pair of programmers work together, one is called the driver, the one responsibe for writing the actual code, and the other is called the navigator, the one responsible for reviewing each line of code as it is being typed.



