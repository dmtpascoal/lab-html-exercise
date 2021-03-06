### Part II - CSS/styles

#### CSS 1 | Setup

As you might recall, the first thing we have to do to add styles to our page is to create a `style.css` file and link it to our `index.html`.

So let's begin by creating a new file, in the same folder as our HTML file, and name it `style.css`. Now, link the file to the _index.html_.

_Hint_: In case you need to refresh your memory on how to do this, check _Introduction to CSS_ lesson.

_Hint2_: You might want to consider adding the following line to your CSS, just to confirm that you have linked it correctly:

```css
body {
  background-color: red;
}
```

Refresh the page in Chrome, and if your _style.css_ is linked properly, the page should turn red. (*You can delete the *background-color* property we added as a test once you have confirmed it's working.*) :wink:

:::info
Before we move forward, add at the very top of your _style.css_ file the following lines:

```css
@import url('https://fonts.googleapis.com/css?family=Poppins');

body {
  font-family: 'Poppins';
}
```

:::

This will be the default font you will be using on the entire webpage.

Now we are ready to start adding some styles to our page.

#### CSS 2 | The Header and the navbar

In the first part of this exercise, you created the header and inside it the navbar. Now we have to add some styles to make it more like this:

![](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_360ab52dd3d20cff448f14b15df7884d.png)

We'll help you style the part of the code we previously provided for you - the upper _div_ of the _header_ tag.

```css
header > div {
  padding: 0 25px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 1px solid lightgray;
}

nav {
  width: 600px;
}

nav ul {
  list-style: none;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

nav a {
  text-decoration: none;
  color: black;
}

.blackHeart {
  width: 20px;
  margin-right: 1rem;
}
```

_Useful information_:

- _form label color_: rgba(0,0,0,.05)
- _form input color_: rgba(0,0,0,.05)
- _form button background color_: #fb3e44
- _form button letters color_: white

As you can see, a lot of _flexbox_ is involved - if needed, revise the lesson again or sneak peek into the official docs (use your Google skills) or use this [resource](https://flexbox.help/) as a help.

Make sure to use flexbox at any time where you need to position elements on a specific place - practice as much as possible: the more you understand now, the easier will be later.

#### CSS 3 | section 1

![](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_d8ae51bd44240ddd2c7d75361bb6397d.png)

In this section, as you can see everything is _centered_. You can add some flexbox rules to the _id_ you attached to this section such is _display: flex;_ and _justify-content: center;_. But this is just the beginning - you still have to set _align-items_ and _flex-direction_.

_Useful information_:

- suggested height for this section: 600px
- background color: rgba(232,217,217,.3)
- "See plans" button background color: #FB3B49
- "See plans" button box shadow: 8px 8px 0 rgba(251,59,73,.2)

#### CSS 4 | section 2

![](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_7a14f0913389dcad5f78e1940267ed85.png)

This section has pretty much the same layout as the previous - some code to be reused :wink:.

_Useful information_:

- _heading background color_: rgba(255,204,53,.4)
- to get the transform of the yellow background in the left-hand direction use: _transform: skew(9deg,0deg);_
- to get it in the opposite direction of the letters, the way we need it on the page, use: _font-style: italic;_
- to additionally fine-tune the position of each element, use _margin_ property.

Again use a lot of flexbox to get the right position of elements - direction, justify-content, align-items.

**Inspect elements to get the right size of the font for each of them**. However, this is not a crucial thing, so don't spend too much time on it - focus on positioning primary.

#### CSS 5 | section 3

![](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_7b69fd57e04d20183daed40e39b2001f.png)

_Useful information_:

- color of the letters in each heading in this section: #ED1C24
- "Create an Org" box shadow: 8px 8px 0 rgba(128,83,35,.2)
- "Create an Org" letters color: white

## Submission

If you didn't [add, commit and push the changes](https://gist.github.com/ironhack-edu/dd3635de73a6ef07ef337bf184eda985#step-3-add-commit-and-push-the-changes) you made, this is the last call. :smile:

And at the same time, if you didn't [create a pull request](https://gist.github.com/ironhack-edu/dd3635de73a6ef07ef337bf184eda985#step-4-create-a-pull-request) this is the time for that as well.

Your TAs will check up your work and provide feedback.

**Once again, a friendly reminder**: You don't have to wait to finish everything in order to follow the steps listed in the [guidelines](https://gist.github.com/ironhack-edu/dd3635de73a6ef07ef337bf184eda985). In a moment when you've made a first significant step in working on this assessment, we advise you to make a pull request. Starting from that moment, every change you make will be automatically added to that pull request and will be visible to your TAs for a checkup.

## Summary

In this exercise, you've built a clone of a piece of the npm home page. This site is very complex so if you managed to make it look anything like the original, good job! :trophy:

This concludes the HTML / CSS module. We are proud of you!

_The Ironhack team :heart:_
