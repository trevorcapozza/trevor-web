# Adding Markdown to My Personal Site
_Using Vue & Github Markdown_
<br />
<br />
<br />
A few months ago, I rewrote my personal website from scratch using Vue.js which may seem like overkill since Vue is designed for sophisticated single page web apps. However, I wanted to learn Vue and redesign my personal website - so why not do both together? If you want to learn more about that process, check out my [migrating to Vue](/2020/vue-markdown) blog.

Before Vue, I was writing static blogs in raw html/css and having to hard code everything together. I knew I had to automate these tedious tasks and I wanted to make the writing process a lot simpler.

As I started researching ways to do this, I came across many powerful tools. I actually got halfway into rewriting my site for a third time using [Gridsome](https://gridsome.org/) because it had great built-in blog features. After running into tons of issues, I came to the realization that I was going to have to do this one myself.
<br />


## Markdown it is.
I quickly realized I wanted to write my blogs using Markdown and build the custom routing aspect from scratch. If you don't know what Markdown is, here is a brief example:

--- _Insert Markdown Image Here_ ---

<!-- ---
```
# H1
## H2
_Wrapping your text in underscores creates Italics_
* Adding an asterisk creates a list 
    * This is a nested list
> You can also add blockquotes by using ">"
```

<br/>

_The code above will output the following results:_
<br/>
<br/>


# H1
## H2
_Wrapping your text in underscores creates Italics_
* Adding an asterisk creates a list 
    * This is a nested list
> You can also add blockquotes by using ">"
--- -->

As you can see, it allows you to write text extremely fast without having to worry about html classes.

<br/>

## Step 1
After deciding on Markdown, I stumbled across this [Github-Markdown](https://github.com/sindresorhus/github-markdown-css) repository that had some good documentation. 
