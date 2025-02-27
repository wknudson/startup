# CS 260 Notes

[Qbuddy - Simon](https://simon.qbuddy.click)

## Helpful links

- [Course instruction](https://github.com/webprogramming260)
- [Canvas](https://byu.instructure.com)
- [MDN](https://developer.mozilla.org)

## AWS

My IP address is: 52.200.67.250
Was a fairly easy process. Just had to make sure that my IP was good and that I had correct records for the *, simon, and startup.

## Caddy

No problems worked just like it said in the [instruction](https://github.com/webprogramming260/.github/blob/main/profile/webServers/https/https.md).
made sure that in my git bash i edited it correctly to send to my specific domain.

## HTML

I messed around with the links between the three views work great using the `a` element. All connect together and there is a link to my github on every page.

I am getting better at noticing how it is the framework of the website. I still find it annoying that I shouldnt do any style edits in the HTML page.

Added some pictures and replaced the placeholders. I found it easy to save image as instead of link from the internet.

## CSS

I did the CSS practice. It was kind of hard and I had to look up a lot of things because I did not know the key words. I got it to a point that looks good.

I looked more into the bootstrap to understand it better. Hopefully in the future I can use it to the full potential.

Basic setup of my styles sheet. Making sure flex is there and media aswell. Added a hover function and somewhat copied the styles over to my other pages.

Adding accordion button is much harder than i thought it would be. I was able to create buttons for each of the sidebar headers.

```styles
* {
    font-family: 'Roboto', sans-serif;
}

body {
    display: flex;
    flex-direction: column;
    margin: 0;
    height: 100vh;
}

header {
    flex: 0 0 80px;
    background: hsl(184, 61%, 47%);
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 20px;
}

img {
    max-width: 100%;
    height: auto;
    border-radius: 10px;
    display: block;
    margin: 10px auto;
    transition: transform 0.3s ease-in-out;
}

img:hover {
    transform: scale(1.05);
}

p {
    font-size: 16px;
    font-weight: bold;
    line-height: 1.6;
    text-align: center;
    color: hsl(180, 10%, 20%);
    margin-bottom: 15px;
    justify-content: center;
}

nav ul {
    display: flex;
    list-style: none;
    padding: 0;
    margin: 0;
}

nav li {
    margin-right: 20px;
}

nav a {
    text-decoration: none;
    color: white;
    font-weight: bold;
    justify-content: center;
}

nav a:hover {
    background-color: hsl(180, 67%, 28%);
}

/* Accordion styles */
.accordion {
    margin-top: 20px;
}

.accordion-item {
    margin-bottom: 10px;
}

.accordion-button {
    width: 100%;
    text-align: left;
    padding: 10px;
    background-color: hsl(180, 57%, 38%);
    color: white;
    border: none;
    cursor: pointer;
    font-size: 16px;
    font-weight: bold;
    border-radius: 5px;
    transition: background-color 0.3s;
}

.accordion-button:hover {
    background-color: hsl(180, 67%, 28%);
}

.accordion-content {
    padding: 15px;
    background-color: hsl(180, 10%, 90%);
    display: none;
    border-radius: 5px;
    margin-top: 5px;
}

/* Open accordion content */
.accordion-content.open {
    display: block;
}

/* Login Form */
.login-form {
    display: flex;
    gap: 10px;
}

.login-form input {
    padding: 5px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

.login-form button {
    background-color: hsl(180, 57%, 38%);
    color: white;
    border: none;
    padding: 5px 10px;
    border-radius: 5px;
    cursor: pointer;
}

.login-form button:hover {
    background-color: hsl(180, 67%, 28%);
}

footer {
    flex: 0 0 10px;
    background: hsl(180, 10%, 10%);
    text-align: center;
    color: white;
    padding: 3px;
}

main {
    flex: 1;
    display: flex;
    flex-direction: row;
}

section:nth-child(1) {
    flex: 1;
    background-color: hsl(180, 10%, 80%);
    padding: 20px;
}

section:nth-child(2) {
    flex: 3;
    background-color: white;
    padding: 20px;
}

/* Responsive Design */
@media (orientation: portrait) {
    main {
        flex-direction: column;
    }
}

@media (max-height: 700px) {
}
    
```


## React Part 1: Routing

So far it has been really confusing and hard to get the hang of. I was able to follow mostly the Simon version, but I still run into a lot of issues. Followed the video precisely and was able to get most of it done. Had to make minor changes so my code could work. Hopefully I can get the buttons to work later on.

My css styles werent correctly transfered over so I made sure to put specific styles in my app.css.

## React Part 2: Reactivity

THis is a lot of trail and error. I think my origional idea is a bit too complex. Im hoping that just by using buttons and timers I can get the understanding of my startup across.
Ive added functionality with onClicks and timers. I tired to keep it basic for use and comprehension.
