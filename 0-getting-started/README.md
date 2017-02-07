# Week 1 - Getting Started

## Table of Contents
* [Bonding Activities](#bonding)
* [Web Tier Code](#code)
* [Tools](#tools)
* [Dev Environment](#dev)
* [Sublime Text Plugins](#sublime)
* [Sass](#sass)
* [Reset/Normalize](#reset)
* [Style Guide](#style)
* [Media Queries](#media)
* [Activity](#activity)

## Bonding Activities <a name="bonding"></a>
* Lightning talks every week
  * Talk about a topic that interests you -- anything at all, not related to web or CS or whatever
  * The purpose of this talk is to practice your speaking, presentation skills, so while it is okay
    to show a video, etc. to state your point, you must be speaking 90% of the time
  * Examples from the past: betta fish origin/care, Japan summer trip, rap terminology
* "Hackathons"
  * In which you get into groups and make small things that will hopefully further your knowledge
    of web
* Today: Photo introductions!

Bonding activities are extremely important because you will be working in close proximity with your
tier members for the rest of the semester.  I encourage you guys to make a group chat (without me)
where you guys can have a space to just talk about work or anything else you want!  We will also have
a tier group chat in addition to this.

## Web Tier Code <a name="code"></a>
* Respect each other - this means putting your laptop down and giving full undivided attention during
  lightning talks, helping each other whenever possible, being kind, etc.
* Help each other - if your fellow tier member asks a question, help them out, and be patient!
  You learn faster if you learn together!  Brings me to my next point...
* I am here to answer questions you have, but...
  * I don't pretend to know everything, and I don't know everything
  * If you ask me something that I don't know, I'll can  refer you to
    someone who is more knowledable in that area.
  * If you ask me something that another tier member has already asked me, I will redirect you to
    them! For reals though, ask your members first! Most of the time, they have
    had the same problem or know how to fix it. I am more than happy to help during meeting if 
    multiple people have the same question!
  * You are free to ask conceptual questions anytime and I will answer them to the best of my ability
* If you are stuck, follow these tips:
  * Think about what you're doing and why you're doing it, avoid blindly trying things
  * Restart your server, "turn it on and off", etc.
  * Google your error
  * Ask your tier members
  * Ask me
* You learn the most from breaking things and figuring things out on your own, so don't be afraid to
  fail/struggle! Web is actually pretty difficult to learn well and the only way anyone gets
  anywhere is getting stuck first (sometimes, for hours).
* Don't apologize for asking questions! And don't be shy!

## Tools <a name="tools"></a>
* [Git](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics) - Learn how to use Git, this is 
  required for working in groups
* [Homebrew](http://brew.sh/) - not necessarily used in this tier, but use it for everything else!
  Seriously, it'll save you lots of headache (for example 61A TAs made us install Python in the
  wrong place but this wouldn't have happened if I had used Homebrew)

## Final things...setup your dev environment <a name="dev"></a>
1. Install nvm with install script https://github.com/creationix/nvm#install-script
2. `nvm install node`
3. `nvm use node`
4. `nvm alias default node`
5. Install [yarn](https://yarnpkg.com/)
  * This semester, we will be trying yarn instead of npm.  Here's an article about the differences
    for those interested: [Yarn vs. NPM](https://yarnpkg.com/)
6. A text editor - Download Sublime Text 3, Atom, or Vim if you don't have already

Warnings are okay, but you shouldn't have any errors.  If you have errors, refer to the tips on what
to do if you're stuck.

## Useful Sublime Text Plugins <a name="sublime"></a>
* Download [Sublime Text Package Manager](https://packagecontrol.io/installation)
* After downloading the package manager, `cmd-shift-p` and search "Install Package"
* Install the following:
  * Emmet
  * FakeImg
  * Sass
  * Babel
  * BracketHighlighter
* Read up on each package/what they do and try it out for yourself!

## Sass <a name="sass"></a>
* If you don't know what scss is, compare `style.scss` and `style.css` in [here](https://github.com/jubearsun/web-tier-2016/tree/master/Week%202%20-%20Style%20Guide%20and%20Responsive%20Design/style-demo)
  and read up on it online. We will be using scss for our projects.

## Reset/Normalize <a name="reset"></a>
* [Normalize CSS](https://necolas.github.io/normalize.css/) makes sure all browsers render your webpage more consistently. All browsers have different default styles. Try creating an index.html file and opening it in your browser of choice. There's padding and margins even if you don't have any CSS file attached. Normalize gets rid of these default paddings/margins so you can have more consistent styling across all browsers.
* Normalize is ALWAYS the first thing you import before your own CSS files.

## Style Guide <a name="style"></a>
* Tabs and Spacing: We'll be using 2 space indents! Make sure to configure this in your text editor settings (at least when you're working on tier projects)
* Naming conventions: [Airbnb's style guide](https://github.com/airbnb/css) to [BEM](http://getbem.com/introduction/), we will be using `block__modifier--value`
  * There are a myriad of naming conventions out there, but this will hopefully make it clearer to everyone on the tier what each style does.
* Divs over tables!
  * Lots of reasons, can Google it if you're interested
* Classes over IDs
  * Styling is always done with classes even if the class will only appear once on a page, and IDs are used for selection in JavaScript.

## Media Queries <a name="media"></a>
* Responsive design is the only way to design! Never push something without making sure it is responsive on all screen sizes.
* Use media queries -- I like to go from largest screen size to smallest screen size.
* Chrome Developer Tools is your friend.

## Activity <a name="activity"></a>
* Recreate the [Virgin America website](http://virginamerica.com) as best you can using the style guide and SCSS, with this [React boilerplate](https://github.com/cle1994/react-frontend-boilerplate)!
  * Feel free to change some things if you want to make it "your own"
* Push to [GitHub Pages](https://pages.github.com/) (project site, not user site) when you're done and post it in the group along with the GitHub repo!

### Directions on using the boilerplate
* Clone or download the repo, if you clone it you will have to change the remote to your own repo in order to push
* `cd` into the folder (you can rename it to whatever you want) and run `yarn install`, this will install all dependencies in `package.json`
* Run `npm run dev` to start developing!
