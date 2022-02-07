Sass Becode
===========

![](img/sass.svg)

## How to install SASS ?

He have many different installation :

    Standalone -> Just download the [file](https://github.com/sass/dart-sass/releases) in Github and move the file in your repository/Folder
    NodeJS -> npm install -g sass
    Chocolatey -> choco install sass
    brew -> brew install sass/sass/sass

## What is Sass ?

Sass is an Extension and Pre processor for CSS3
Sass use .scss & .sass

## How he does work ? (Pre Processor)
Sass need a input file (SASS SCSS)
Sass compile then the file in CSS

_.scss .sass can't be read by browser._

## Why use SASS ?
    **Free**
    **Easy To learn (2 Syntax)**
    **Win Time and Organisation**

## SASS VS SCSS

![](img/sassCode.png) ![](img/scssCode.png)

_Same code but the difference between is .SASS doesn't have symbole. (Just :) -> {};_

## SASS&SCSS VS CSS 

You can see the .SCSS with one block, and the CSS with tree block. It saves us copy paste all time and win organisation.

![](img/sassCode.png) ![](img/cssCode.png)


## Variable

Yep, in SASS, we can use Variable for text or value

On this example, i give to my variable responsive : screen with max-width: #{$normal}...

![](img/variableCode.png)

_Results :_
_Left SCSS - RIGHT CSS_

![](img/variableCodeScss.png)![](img/variableCodeCss.png)

## @Import

You can import another file in your style.scss(Example)
    @import 'examplefile.scss';

![](img/importCode.png)

## @mixin

Imagine, you need to give many code for many class, id, (More)...

You can include @mixin in your code and give the same code for class, id, (More) with @include.

Example : 

    @mixin button{
        &:hover{
            color: red;
        }
    }

    a{
        text-decoration: none;
        color: #example;
        @include button()
    }

    .text{
        @include button()
    }

The output :

    a{
        text-decoration: none;
        color: #example;
    }

    a:hover{
        color:red;
    }

    .text:hover{
        color: red;
    }

