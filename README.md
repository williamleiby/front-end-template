# front-end-template 🤺

this is the front-end template / architecture i use when building front-end projects.

before i dive in, it should be stated that this template is just the foundation to a front-end project. 

add a framework, take away folders and / or files you dont need, or don't change a single thing at all. 

if there are any tweaks you think i should make, besides writing this whole documentation in lowercase lettering, feel free to fork my code or [email](mailto:contact@williamleiby) me.

## getting started. 👶

feel free to [clone](https://github.com/williamleiby/front-end-template..git) / [download](https://github.com/williamleiby/front-end-template./archive/master.zip) this repo.

### prerequisites. 👨‍💻

things you need prior to using this template :

```
1. module bundler / task runner. (codekit (my choice), webpack, gulp, etc.)
2. text editor. (vs code (my choice), sublime, atom, brackets, etc.)
3. cli. (hyper (my choice), iterm, terminal, etc.)
```

## using the template. 🛠

in this template there are two main folders :
```
dist
src
```
other assets include :
```
.gitignore
LICENSE
README.md
```
for this repo, we will only really be focusing on the two main folders listed above.

### 'dist' 📦

'dist' is the folder that will be ssh'd / ftp'd up to a server once i'm done with the front-end for a project. 

inside of the 'dist' folder, you will find all of these folder assets :

```
fonts
img
scripts
styles
videos
index.html
```

inside each folder has what you might expect...

* font files are in the 'fonts' folder.
* images, favicons, logos, icons, etc. would be in the 'img' folder.
* videos, gif's, etc. are in the 'videos' folder.

and as you probably expect...

markup for each page is located in the '.html' files.

all that is fine and dandy, but what about our javascript and css code ? where is all of that being output to ?

well, if you hadn't noticed by now, there are two folders i left out...
```
scripts
styles
```

inside of each of the folders, there will be one main 'styles-dist.css' and 'scripts-dist.js' file, as well as source maps for each language.

if you are wondering how my output code compresses all of my libraries, frameworks, and preprocessors into one file, refer to the section 'why do any of this ?' below.

### 'src' 🏭

'src' is the folder where i manipulate styling attributes  / javascript code to make a website come to life.

inside the 'src' folder are two main folders :
```
scripts
styles
```

just like a lot of individuals who like to speed up their production when coding but not compromise for shitty code, i write my javascript and css with preprocessors, libraries, frameworks, etc..

i use sass when writing my styling attributes, then have partials for each section / group i'm working on @import'd into one large 'styles.scss' file in the 'styles' folder.

from there, i have my 'styles.scss' file output to be compiled into the 'styles' folder in 'dist'. the result will be one (yes,one.) 'styles-dist.css'.

i also create a source map (this option is given in codekit) with the same output so dev tools aren't as much of a nightmare as they sometimes can be.

## finally, deployment. 🎁

ship your front-end project with whatever you want.

ssh. 

ftp.

it's up to you.

just make sure that when you deploy your project, you leave out the 'src' folder in the '.gitignore' file. a nifty '.gitignore' template can be found [here](https://gist.github.com/octocat/9257657).

## why do any of this ? 🤨

the reasoning behind this template really boils down to some key features i couldn't take away from a front-end project. 

* ease of mind. 🧘‍♂️
* no more "reinventing the wheel". 🚀
* a foundation i know inside and out. 🤔

i used to spend a good 15 minutes setting up the foundation of a project, but now because of this template i am able to get that 15 minutes back and use it towards something more productive.

i no longer have to worry about scrolling through one giant 'styles.css' file or one giant 'scripts.js' file to find what i'm looking for.

also, since i compile all of my javascript and css code down into one file for each language, that means there is only one http request made for each language when referencing the files in my '.html' files for each project.

finally, i know where everything is. this is another huge time-saver when it comes to projects with a deadline or even just cranking out an idea.

( ps - another great thing about this template is that you can use whatever methodology you want; BEM, SMACSS, etc..)

## other stuff. 🤷‍♂️

### ok, dude. what’s with all the comments ? 🗒

in the ‘index.html’, ‘styles.scss’, and ‘scripts.js’ files, you most likely saw comments with banners labeled ‘TODO:’ or ‘FIXME:’. those comments are lists for me to refer back to whenever i have close a project and reopen it. i also use an extension in vscode called todo highlighter that highlights the names of each banner throughout the project.

also, i’m a huge fan of modularizing code into chunks, rather than having one giant sheet of code that takes ages to find something (even with a fuzzy finder).

### author. 🧐

**william leiby** - *front-end-template* - [williamleiby.](https://williamleiby.com)

### aknowledgements. 👏

* [Jesse Showalter](https://github.com/jesseshowalter) for the inspiration behind this template.

### license. 📜

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for more details.
