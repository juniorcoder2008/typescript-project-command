# Typescript Project Command

## Explanation
This project command automatically creates a typescript project and starts a live server with [BrowserSync](https://browsersync.io/). You don´t have to worry about compiling the TS, because here everything is automated with [Gulp](https://gulpjs.com/). In the app folder are all files in which the code is written. A mandatory index.html, a style folder with an index.sass and a \_design.sass and a ts folder with a script.ts. In the Sass I have already written a small template in the \_design.sass, so that you do not have to style everything from scratch, such as buttons, links or headings. Also some variables are defined, like some standard colors from my design system, some sizes for margins, paddings or media queries and fonts.

### Sass
I have a design system that fits the [JuniorCoder](https://www.youtube.com/channel/UCS19Yq0xKeFo4xVMc6ux1pA) YouTube channel. Therefore I have defined some variables in the __\_design.sass__ which fit to the design system. This includes of course all fonts and colors, but also some sizes. I also defined a few mixins that make life easier. I mean, who has not written 1000 times the following code:
```sass
.element
     position: absolute
     top: 50%
     left: 50%
     transform: translate(-50%, -50%)
```
Instead, simply write:
```sass
@include center()
```
And that's it. This way you can easily turn four lines into one.
The second mixin is especially interesting for responvise websites or even apps. It is about the obligatory close button of a menu. If you define an element in HTML with two child divs with the classes .line01 and .line02 then a perfect close-button is created.

Beside all the mixins I defined some more rudimentary styles, like the different fonts for HTML tags or colors and sizes of buttons.

## Requirements

The command automatically creates a [Git](https://git-scm.com/) repository for you, so you can start directly ;-)
To execute the command you also need [NodeJS](https://nodejs.org/en/).

Now you can start setting up the command! Now press win+r, so now a new little window should open. Type in: 
```cmd
%appdata%/npm
``` 
and enter. The __npm__ folder  
should open. There you can drag n drop the ```cmd-file```.

## Use the Command
After this, you should be able to type in every folder in the cmd 
```
typescript-project coolProject
```
If this works, happy birthday, now you can save time, cause you shouldn´t
create a working-directory for web-apps one more time!
