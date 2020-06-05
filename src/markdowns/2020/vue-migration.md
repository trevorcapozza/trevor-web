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

The default setup is great for quickly prototyping a new project, while the manual setup provides more options that are likely needed for more production-oriented projects.

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
            <div class="row"><span class="circle-select"></span><p>Babel</p></div>
            <div class="row"><span class="circle"></span><p>TypeScript</p></div>
            <div class="row"><span class="circle"></span><p>Progressive Web App (PWA) Support</p></div>
            <div class="row"><span class="circle-select"></span><p>Router</p></div>
            <div class="row"><span class="circle"></span><p>Vuex</p></div>
            <div class="row"><span class="circle"></span><p>CSS Pre-processors</p></div>
            <div class="row"><span class="circle-select"></span><p>Linter / Formatter</p></div>
            <div class="row"><span class="circle"></span><p>Unit Testing</p></div>
            <div class="row"><span class="circle"></span><p>E2E Testing</p></div>
        </div>
    </div>
</div>

<br/>
<br/>

If you chose to manually select features, at the end of the prompts you also have the option to save your selections as a preset so that you can reuse it in the future. We will discuss presets and plugins in the next section.

<br/>
