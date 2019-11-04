# hover-text.css
## Hover animations specifically for text

a list of animations specifically designed for text content only (the list is short for now because this is only the first version)

## Contents

1. [Contents](Contents)
2. [Download/Install](#downloadinstall)
3. [How To Use](#how-to-use)
   1. [A. list of classes](#a-list-of-classes)
   2. [B. Application](#b-application)

## Download/Install

* NPM `npm install hover-text.css`
* [DownloadZip](https://github.com/Quickinline/hover-text.css/master/hover-text.zip)

## How To Use

hover-text.css is a list of ready to use classes that add hover animations to text. there are some possible modifications that can be done through [Sass Customization](#sass-customization).

**notice** the targeted text should be wrapped in an element that is the same width as the text itself

### A. list of classes

* hvr-underline-center-out
* hvr-underline-left-to-right
* hvr-underline-right-to-left
* hvr-y-center-out
* hvr-y-left-to-right
* hvr-y-right-to-left

## B. Application

the best use case example for this is a navbar (Bootstrap's navbar) especially the navigation section **nav-link** they are the best fit use case

``` html
<nav class="navbar navbar-expand-sm navbar-light bg-light">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler d-lg-none" type="button" data-toggle="collapse" data-target="#collapsibleNavId" aria-controls="collapsibleNavId"
        aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="collapsibleNavId">
        <ul class="navbar-nav mr-auto mt-2 mt-lg-0">
            <li class="nav-item active">
                <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#">Link</a>
            </li>
            <li class="nav-item dropdown">
                <a class="nav-link dropdown-toggle" href="#" id="dropdownId" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Dropdown</a>
                <div class="dropdown-menu" aria-labelledby="dropdownId">
                    <a class="dropdown-item" href="#">Action 1</a>
                    <a class="dropdown-item" href="#">Action 2</a>
                </div>
            </li>
        </ul>
        <form class="form-inline my-2 my-lg-0">
            <input class="form-control mr-sm-2" type="text" placeholder="Search">
            <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
        </form>
    </div>
</nav>
```

All you have to do is add a class from the list to the concerned text to output something like this

``` html
<nav class="navbar navbar-expand-sm navbar-light bg-light">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler d-lg-none" type="button" data-toggle="collapse" data-target="#collapsibleNavId" aria-controls="collapsibleNavId"
        aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="collapsibleNavId">
        <ul class="navbar-nav mr-auto mt-2 mt-lg-0">
            <li class="nav-item hvr-underline-center-out active">
                <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
            </li>
            <li class="nav-item hvr-underline-center-out">
                <a class="nav-link" href="#">Link</a>
            </li>
            <li class="nav-item dropdown">
                <a class="nav-link hvr-underline-center-out dropdown-toggle" href="#" id="dropdownId" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Dropdown</a>
                <div class="dropdown-menu" aria-labelledby="dropdownId">
                    <a class="dropdown-item" href="#">Action 1</a>
                    <a class="dropdown-item" href="#">Action 2</a>
                </div>
            </li>
        </ul>
        <form class="form-inline my-2 my-lg-0">
            <input class="form-control mr-sm-2" type="text" placeholder="Search">
            <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
        </form>
    </div>
</nav>

```

## C. Sass Customization

for now there's 3 values to customize among these animations

``` scss
$animation-speed: 0.3s;
$underline-width :2px;
$line-color: #007bff;

```
