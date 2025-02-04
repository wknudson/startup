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

## CSS

I did the CSS practice. It was kind of hard and I had to look up a lot of things because I did not know the key words. I got it to a point that looks good.

I looked more into the bootstrap to understand it better. Hopefully in the future I can use it to the full potential.

Basic setup of my styles sheet. Making sure flex is there and media aswell. 

```styles
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
    flex: 0 0 30px;
    background: hsl(180, 10%, 10%);
    text-align: center;
    color: white;
    padding: 5px;
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
    header {
        display: none;
    }
    footer {
        display: none;
    }
}

    
```


## React Part 1: Routing

Setting up Vite and React was pretty simple. I had a bit of trouble because of conflicting CSS. This isn't as straight forward as you would find with Svelte or Vue, but I made it work in the end. If there was a ton of CSS it would be a real problem. It sure was nice to have the code structured in a more usable way.

## React Part 2: Reactivity

This was a lot of fun to see it all come together. I had to keep remembering to use React state instead of just manipulating the DOM directly.

Handling the toggling of the checkboxes was particularly interesting.

```jsx
<div className="input-group sound-button-container">
  {calmSoundTypes.map((sound, index) => (
    <div key={index} className="form-check form-switch">
      <input
        className="form-check-input"
        type="checkbox"
        value={sound}
        id={sound}
        onChange={() => togglePlay(sound)}
        checked={selectedSounds.includes(sound)}
      ></input>
      <label className="form-check-label" htmlFor={sound}>
        {sound}
      </label>
    </div>
  ))}
</div>
```
