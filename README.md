# Sprint Challenge: Advanced CSS - Space Walkers Web Page
 
This challenge allows you to practice the concepts and techniques learned over the past week and apply them in a concrete project. This Sprint explored advanced CSS techniques using Responsive Design and Preprocessing. During this Sprint, you studied how to use the viewport meta tag, media queries, setting up a preprocessor, and advanced use of preprocessing techniques. In your challenge this week, you will demonstrate proficiency by updating a website that is missing content as well as adding mobile styling.

## Instructions

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the Sprint Challenge. However, you are encouraged to follow the twenty-minute rule and seek support from your PM and Instructor in your cohort help channel on Slack. Your work reflects your proficiency in advanced css and your command of the concepts and techniques in responsive web design and preprocessing.

You have three hours to complete this challenge. Plan your time accordingly.

## Commits

Commit your code regularly and meaningfully. This helps both you (in case you ever need to return to old code for any number of reasons) and your project manager.

## Description

The client for this challenge is _Spacewalkers Magazine_. Spacewalkers needs your help to build a small proof of concept website for their marketing team. They have provided designs for both desktop and phone views. In addition to designs and content they have most of the home page coded for you. You just need to finish the navigation and header as well as the mobile styles.

In meeting the minimum viable product (MVP) specifications listed below, your web page should look like the solution design files of the desktop and mobile views:

[Click here to review the home design](design-files/home-desktop.png)

[Click here to review the mobile design](design-files/home-mobile.png)

## Self-Study Questions

Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read by your project manager

1. What is the difference between an adaptive website and a fully responsive website?

Responsive websites, usually utilizing a viewport-meta-tag, will detect the viewport size on any device and adjust the browser's layout and functionality to optimize the browsing experience for the user.  Fully responsive websites/pages provide the most advanced type of browsing experience to accommodate fluidly across all devices.  Responsive sites are usually set up with a max-width.  Adaptive websites, slightly less advanced, will also adjust its layout and functionality to accommodate various viewports, but only at specific breakpoints.  Adaptive websites are not as fluid and will only adjust when a breakpoint is reached.  These sites are usually triggered when a desired width triggers a new layout.  Fully responsive, using max-width, accommodates a range, while adaptive, using a width, accommodates a single breakpoint.

2. Describe what it means to be mobile first vs desktop first.

Mobile first vs. desktop first refers to the developer(s) starting point in web development.  If a developer or team is 'mobile first', this refers to the teams objective of optimizing their site for a mobile device first.  As the team continues to build their code, they venture into tablets, and eventually desktops last.  Mobile first, designs and builds sites in a smallest viewport to largest viewport order.  Desktop first is the exact opposite.  They build their websites starting at the largest viewport  size, and work their way down to the smallest viewport size, in terms of layout, design, and functionality.

3. What does `font-size: 62.5%` in the `html` tag do for us when using `rem` units?

62.5% is the conversion rate to set 1rem equal to 10 pixels.  This makes utilizing the functionality and fluidity of rem's fully responsive unit and the commonality of designing and using pixels a simple conversion for developers to switch to.  In short, it allows developers to "think" in pixels, while utilizing the "functionality", in terms of responsiveness, of rem units.

4. How would you describe preprocessing to someone new to CSS?

Preprocessing is an amazing process, of utilizing nesting, various levels deep, and other useful techniques to assign styling to a webpage.  Preprocessors utilize their expansive tool set and make styling, in my opinion, a much easier and more accurate experience.  First the code is arranged using a preprocessor, then it is converted to CSS using a compiler.  Once compiled the final coding result is purely CSS.

5. What is your favorite concept in preprocessing? What is the concept that gives you the most trouble?

My favorite concept in preprocessing is the ability to nest so universally to accomplish web development goals.  I find it extremely easy to communicate design specifications with the computer.  The most troubling concept to me, which I'm sure may grow into a love, is the concept of syntax perfection.  If one keystroke or character is extra or out of place, the preprocessor will not allow the compiler to convert the code into CSS, and although it seems like you are coding, the results will not show on your website until the syntax is perfect.  Although this is troubling to a new developer, I'd imagine it will quickly sharpen their skills, understanding, and attention to detail and in a way, may grow into a desirable feature.

You are expected to be able to answer all these questions. Your responses contribute to your Sprint Challenge grade. Skipping this section *will* prevent you from passing this challenge.

## Project Set Up

Because you are using a preprocessor, there are two parts to setting up your project.  Be sure to run through the git set up first and then set up the preprocessor.

### Git Set up

Follow these steps to set up your project:

- [ ] Create a forked copy of this project.
- [ ] Add your project manager as collaborator on Github.
- [ ] Clone your OWN version of the repository (Not Lambda's by mistake!).
- [ ] Create a new branch: git checkout -b `<firstName-lastName>`.
- [ ] Implement the project on your newly created `<firstName-lastName>` branch, committing changes regularly.
- [ ] Push commits: git push origin `<firstName-lastName>`.
 
Follow these steps for completing your project.

- [ ] Submit a Pull-Request to merge <firstName-lastName> Branch into master (student's  Repo). **Please don't merge your own pull request**
- [ ] Add your project manager as a reviewer on the pull-request
- [ ] Your project manager will count the project as complete by merging the branch back into master.
 

### Preprocessor Set up

* [ ] Verify that you have LESS installed correctly by running `lessc -v` in your terminal, if you don't get a version message back, reach out to your project manager for help.
* [ ] Open your terminal and navigate to your preprocessing project by using the `cd` command
* [ ] Once in your project's root folder, run the following command `less-watch-compiler less css index.less`
* [ ] Verify your compiler is working correctly by changing the `background-color` on the `html` selector to `red` in your `index.less` file.
* [ ] Once you see the red screen, you can delete that style and you're ready to start on the next task

## Minimum Viable Product

Your finished project must include all of the following requirements:

### Import LESS Files

* [ ] Navigate to your `index.less` file. Notice the file is blank. You have been asked to use a certain import order. That order is as follows:

```markdown
1.variables.less
2.mixins.less
3.reset.less
4.global.less
5.navigation.less
6.footer.less
7.home-page.less
```

_You will know everything is working properly when you see the styles enabled for the provided content._  

### Home Page - Desktop HTML & LESS

* [ ] Take 10 minutes to review the code that has already been provided for you. Take time to see how the home page was built.

* [ ] Add a viewport meta tag to the head of your index.html page

* [ ] [Review the provided home desktop design file](design-files/home-desktop.png). You are to build the missing navigation system and header image. You have been provided all content necessary in the [index.html file](index.html)

* [ ] Navigation Styles: Use the `navigation.less` file for styling.

* [ ] Main Content Styles: Use the `home-page.less` file for styling

* [ ] LESS Mixins: Create and use 2 different mixins to aid your styling. Use the `mixins.less` file for your mixins

* [ ] LESS Parametric Mixin: create a parametric mixin that is used to create the `sign up` button styles.

* [ ]  Use at least 2 parameters to create your button

* [ ] Create a hover state that swaps the background color and font color of the base button styles.

### Mobile Design

* [ ] Create a `@phone` variable that contains a `max-width: 500px` media query string. Use the `@phone` variable for all your nested mobile styling.

* [ ] [Review the provided home mobile design file](design-files/home-mobile.png). Match your mobile styling the best you can using the design file.

* [ ] Push your changes and create a pull request if you haven't already.

In your solution, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Stretch Problems

After finishing your required elements, you can push your work further. These goals may or may not be things you have learned in this module but they build on the material you just studied. Time allowing, stretch your limits and see if you can deliver on the following optional goals:

* [ ] Build a page of your choosing from the navigation items. Come up with content and images that fit the theme.

* [ ] Introduce CSS animations to your site.

* [ ] Create a fixed navigation and add some opacity to the background

* [ ] Create a form that would allow someone to sign up for a Spacewalkers Magazine subscription