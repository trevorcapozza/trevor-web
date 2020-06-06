# Migrating My Personal Website to Vue

<br/>

After recently discovering Vue.js and how powerful it is, I knew right away that I wanted to start learning how it worked. [Vue](https://vuejs.org) is a progressive framework for building user interfaces and single page web apps using HTML, CSS, and JavaScript. 

Using Vue for a personal website is definitely overkill, but it was a great side project to get familiar with the framework.

## Getting Started
The easiest way to get started with Vue is using the Vue Cli within your terminal.

#### Install:

```
npm install -g @vue/cli
```
#### Create a project:
```
vue create my-project
```
<br/>

You will be prompted to pick a preset. You can either choose the default preset which comes with a basic Babel + ESLint setup, or select "Manually select features" to pick the features you need. In this case, I chose to manually select my features.

<br/>

<div class="window-center">
    <div class="browser">
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
    </div>
    <div class="terminal">
        <p class="blue">Vue CLI v4.4.1</p>
        <p class="white"><span class="green">?</span>Please pick a preset:</p>
        <p class="indent lightgrey">default (<span class="yellow">babel, eslint</span>)</p>
        <p class="lightblue">> Manually select features</p>
    </div>
</div>

<br/>
<br/>

In my case, I chose to install Router since I will want to toggle between different pages. I am also going to be doing all of my styling through SCSS so I will install that through the CSS Pre-processors.

<br/>

<div class="window-center">
    <div class="browser">
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
    </div>
    <div class="terminal">
        <p class="blue">Vue CLI v4.4.1</p>
        <p class="white"><span class="green">?</span>Please pick a preset: <span class="lightblue">Manually select features</span></p>
        <p class="white"><span class="green">?</span>Check the features needed for your project:</p>
        <div class="vue-features">
            <div class="row"><span class="circle-select"></span><span class="inner-dot"></span><p>Babel</p></div>
            <div class="row"><span class="circle"></span><p>TypeScript</p></div>
            <div class="row"><span class="circle"></span><p>Progressive Web App (PWA) Support</p></div>
            <div class="row"><span class="circle-select"></span><span class="inner-dot"></span><p>Router</p></div>
            <div class="row"><span class="circle"></span><p>Vuex</p></div>
            <div class="row"><span class="circle-select"></span><span class="inner-dot"></span><p>CSS Pre-processors</p></div>
            <div class="row"><span class="circle-select"></span><span class="inner-dot"></span><p>Linter / Formatter</p></div>
            <div class="row"><span class="circle"></span><p>Unit Testing</p></div>
            <div class="row"><span class="circle"></span><p>E2E Testing</p></div>
        </div>
    </div>
</div>

<br/>
<br/>

This next step will ask you if you want to use history mode. I always choose yes here - mainly because it gets rid of the **/#** in your url.

<br/>

<div class="window-center">
    <div class="browser">
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
    </div>
    <div class="terminal">
        <p class="blue">Vue CLI v4.4.1</p>
        <p class="white"><span class="green">?</span>Please pick a preset: <span class="lightblue">Manually select features</span></p>
        <p class="white"><span class="green">?</span>Check the features needed for your project: <span class="lightblue">Babel, Router, CSS Pre-processors, Linter</span></p>
        <p class="white"><span class="green">?</span>Use history mode for router? <span class="brightyellow">(Requires proper server setup for index fallback in production) </span><span class="darkgrey">(Y/n)</span><span> y</span></p>
    </div>
</div>

<br/>
<br/>

This where we'll choose to load SCSS - In this case, I chose `Sass/SCSS (with dart-sass)`

<br/>

<div class="window-center">
    <div class="browser">
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
    </div>
    <div class="terminal">
        <p class="blue">Vue CLI v4.4.1</p>
        <p class="white"><span class="green">?</span>Please pick a preset: <span class="lightblue">Manually select features</span></p>
        <p class="white"><span class="green">?</span>Check the features needed for your project: <span class="lightblue">Babel, Router, CSS Pre-processors, Linter</span></p>
        <p class="white"><span class="green">?</span>Use history mode for router? <span class="brightyellow">(Requires proper server setup for index fallback in production) </span><span class="lightblue">Yes</span></p>
        <p class="white"><span class="green">?</span>Pick a CSS pre-processor (PostCSS, Autoprefixer and CSS Modules are supported by default): <span class="darkgrey">(Use arrow keys)</span>
        <div class="vue-features">
            <div class="row"><p class="lightblue">> Sass/SCSS (with dart-sass)</p></div>
            <div class="row"><p>Sass/SCSS (with node-sass)</p></div>
            <div class="row"><p>Less</p></div>
            <div class="row"><p>Stylus</p></div>
        </div>
    </div>
</div>

<br/>
<br/>

Below I chose `ESLint with error prevention only` (personal preference).

<br/>

<div class="window-center">
    <div class="browser">
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
    </div>
    <div class="terminal">
        <p class="blue">Vue CLI v4.4.1</p>
        <p class="white"><span class="green">?</span>Please pick a preset: <span class="lightblue">Manually select features</span></p>
        <p class="white"><span class="green">?</span>Check the features needed for your project: <span class="lightblue">Babel, Router, CSS Pre-processors, Linter</span></p>
        <p class="white"><span class="green">?</span>Use history mode for router? <span class="brightyellow">(Requires proper server setup for index fallback in production) </span><span class="lightblue">Yes</span></p>
        <p class="white"><span class="green">?</span>Pick a CSS pre-processor (PostCSS, Autoprefixer and CSS Modules are supported by default): <span class="lightblue">Sass/SCSS (with dart-sass)</span>
        <p class="white"><span class="green">?</span>Pick a linter / formatter config <span class="darkgrey">(Use arrow keys)</span>
        <div class="vue-features">
            <div class="row"><p class="lightblue">> ESLint with error prevention only</p></div>
            <div class="row"><p>ESLint + Airbnb config</p></div>
            <div class="row"><p>ESLint + Standard config</p></div>
            <div class="row"><p>ESLint + Prettier</p></div>
        </div>
    </div>
</div>

<br/>
<br/>

Below I chose `Lint on save` (personal preference).

<br/>

<div class="window-center">
    <div class="browser">
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
    </div>
    <div class="terminal">
        <p class="blue">Vue CLI v4.4.1</p>
        <p class="white"><span class="green">?</span>Please pick a preset: <span class="lightblue">Manually select features</span></p>
        <p class="white"><span class="green">?</span>Check the features needed for your project: <span class="lightblue">Babel, Router, CSS Pre-processors, Linter</span></p>
        <p class="white"><span class="green">?</span>Use history mode for router? <span class="brightyellow">(Requires proper server setup for index fallback in production) </span><span class="lightblue">Yes</span></p>
        <p class="white"><span class="green">?</span>Pick a CSS pre-processor (PostCSS, Autoprefixer and CSS Modules are supported by default): <span class="lightblue">Sass/SCSS (with dart-sass)</span>
        <p class="white"><span class="green">?</span>Pick a linter / formatter config <span class="lightblue">Basic</span>
        <p class="white"><span class="green">?</span>Pick additional lint features: <span class="lightgrey">(Press <span class="lightblue">'space'</span> to select, <span class="lightblue">'a'</span> to toggle all, <span class="lightblue">'i'</span> to invert selection)</span>
        <div class="vue-features">
            <div class="row"><span class="circle-select"></span><span class="inner-dot"></span><p class="lightblue">Lint on save</p></div>
            <div class="row"><span class="circle"></span><p>Lint and fix on commit</p></div>
        </div>
    </div>
</div>

<br/>
<br/>

Below I chose `In dedicated config files` (personal preference).

<br/>

<div class="window-center">
    <div class="browser">
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
    </div>
    <div class="terminal">
        <p class="blue">Vue CLI v4.4.1</p>
        <p class="white"><span class="green">?</span>Please pick a preset: <span class="lightblue">Manually select features</span></p>
        <p class="white"><span class="green">?</span>Check the features needed for your project: <span class="lightblue">Babel, Router, CSS Pre-processors, Linter</span></p>
        <p class="white"><span class="green">?</span>Use history mode for router? <span class="brightyellow">(Requires proper server setup for index fallback in production) </span><span class="lightblue">Yes</span></p>
        <p class="white"><span class="green">?</span>Pick a CSS pre-processor (PostCSS, Autoprefixer and CSS Modules are supported by default): <span class="lightblue">Sass/SCSS (with dart-sass)</span>
        <p class="white"><span class="green">?</span>Pick a linter / formatter config <span class="lightblue">Basic</span>
        <p class="white"><span class="green">?</span>Pick additional lint features: <span class="lightblue">Lint on save</span>
        <p class="white"><span class="green">?</span>Where do you prefer placing config for Babel, ESLint, etc.? <span class="darkgrey">(Use arrow keys)</span>
        <div class="vue-features">
            <div class="row"><p class="lightblue">> In dedicated config files</p></div>
            <div class="row"><p>In package.json</p></div>
        </div>
    </div>
</div>

<br/>
<br/>

Next, it will ask you if you'd like to save this set up as a preset, I typically choose no.

After this, it will take a 10-15 seconds to put together your project. To get it running from the command-line, do the following:

```
cd 'project-name'
npm run serve
```

Running the command **npm run serve** will spin up your project into a localhost browser so that you can view your live edits as you code.

## Viola!
If you would like to know more about Vue or a tutorial on a specific project, shoot me an email with a request at [trevor.capozza@gmail.com](mailto:trevor.capozza@gmail.com?subject=Vue%20Request)