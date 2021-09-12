# GitHub Profile

**Watch the video [here]({{ page.youtube_link }})**

## Prerequisites

- [Have a GitHub Account](https://github.com/signup)
- [Visual Studio Code](https://code.visualstudio.com/)

## Loose Agenda

- Create a GitHub profile README which introduces ourselves

## Step by Step

### Create a GitHub Profile Repository

GitHub treats any repository which shares the name of the user as a special repository. Example, for myself `BoredTweak/BoredTweak` is my profile repository.

Start by creating repository which shares your GitHub username.

### Populate the README

I like to organize my profile into three sections:
- Summary (Who am I? How should you refer to me? What am I working on? What are my interests?)
- Contact Info (How do you reach me?)
- Languages and Tools (What technologies do I currently work with?)

We can start by creating our headings. On creation of a GitHub profile repository, we are presented with a default template which can readily be used to start the `Summary` section. Let's also add `Connect with me` and `Languages and Tools` headings.

Example result:

```md
# Hi there

- 👋 I'm Alex aka BoredTweak
- 😄 Pronouns: he/him
- 🌱 I’m currently learning how to create a GitHub Profile.
- 👯 I’m looking to collaborate on Non-Zero things. 
- 🤔 I’m looking for help with how to find my coffee.
- 🔭 I’m currently working on [this github profile](https://github.com/BoredTweak/BoredTweak).
- 💬 Ask me about something.

## Connect with me

## Languages and Tools

```

### Contact Info

Enter a heading `## Connect with me`

Under that heading we will list out any means by which you accept to be contacted such as
- Email
- YouTube
- Twitter
- LinkedIn

**Note - In order to look a little stylish I prefer to leverage icons from [Simple Icons][simpleicons] in badges from [Shields IO][shieldsio].**

We will be using a number of links today, so let's start at the bottom of the file and leverage [Markdown's Reference-style Links](https://www.markdownguide.org/basic-syntax/#reference-style-links).

Declare your prefered connection links at the bottom of the file as such:
```md
[email]: mailto:alex.elia42@gmail.com
[youtube]: https://www.youtube.com/channel/UCT0hVofKq8CM8k8QBiUmpOw
[twitter]: https://twitter.com/BoredTweak
[linkedin]: https://www.linkedin.com/in/alex-elia/
```

Back under the `## Connect with me` heading, let's add some badges. Let's use `Email` as our example. I'll look up the gmail logo and suggested color on [Simple Icons][simpleicons]. 

- The icon tag is `gmail` 
- The suggested color is `#EA4335`.

We can now create a badge at [Shields IO][shieldsio] and customize it to fit our needs. 

The badge template shows `https://img.shields.io/badge/<LABEL>-<MESSAGE>-<COLOR>`

Let's ditch the label and just include the message resulting in `https://img.shields.io/badge/Email-EA4335`

Now we can style it per our preferences at [the styles guide](https://shields.io/#styles). I prefer `flat-square`. We can also provide a logo and logoColor attribute. The logo is simply the Simple Icons tag and the logoColor for our purposes can be white to blend well with the background color in both light and dark themes.

This could result in this badge: `https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white`

GitHub's markdown interpretter supports HTML, so let's use the `img` tag to create a consistent height and width as well as provide an alt text.

For our badge above we can create the following:

```md

# Hi there

- 👋 I'm Alex aka BoredTweak
- 😄 Pronouns: he/him
- 🌱 I’m currently learning how to create a GitHub Profile.
- 👯 I’m looking to collaborate on Non-Zero things. 
- 🤔 I’m looking for help with how to find my coffee.
- 🔭 I’m currently working on [this github profile](https://github.com/BoredTweak/BoredTweak).
- 💬 Ask me about something.

## Connect with me

[<img align="left" alt="BoredTweak | Email" width="150px" height="20px" src="https://img.shields.io/badge/BoredTweak%20%7C%20Email-EA4335?style=flat-square&logo=gmail&logoColor=white" />][email]
</br>

## Languages and Tools

[email]: mailto:alex.elia42@gmail.com
[youtube]: https://www.youtube.com/channel/UCT0hVofKq8CM8k8QBiUmpOw
[twitter]: https://twitter.com/BoredTweak
[linkedin]: https://www.linkedin.com/in/alex-elia/
```

**Note that I used </br> to add some spacing around the image based on the height of the images in mobiel and desktop view. You can instead use <a> tags around the <img> though you cannot use reference links if you go this route.**

### Languages and Tools

For each language/tool you commonly use you can use the same process as above to generate a badge. These follow the same pattern as above. 
- Add a reference link at the bottom of your README for either a sample of your code leveraging the technology or a link to the technology's documentation.
- Grab the icon and color for the technology in context from [Simple Icons][simpleicons].
- Customize the Shields IO template with your text, logo and color. e.g. - `https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white`
- Add a link with the image to your `Languages and Tools` section. e.g. - `[<img align="left" alt="GitHub" height="20px" src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" />][git-demo]`

This might result in the following profile:

```md

# Hi there

- 👋 I'm Alex aka BoredTweak
- 😄 Pronouns: he/him
- 🌱 I’m currently learning how to create a GitHub Profile.
- 👯 I’m looking to collaborate on Non-Zero things. 
- 🤔 I’m looking for help with how to find my coffee.
- 🔭 I’m currently working on [this github profile](https://github.com/BoredTweak/BoredTweak).
- 💬 Ask me about something.
- 🤗 Non-Zero Days now has [a GitHub Pages][non-zero-days-gh-pages]!

## Connect with me

[<img align="left" alt="BoredTweak | Email" width="150px" height="20px" src="https://img.shields.io/badge/BoredTweak%20%7C%20Email-EA4335?style=flat-square&logo=gmail&logoColor=white" />][email]
</br>

## Languages and Tools

[<img align="left" alt="GitHub" height="20px" src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" />][git-demo]
</br>

[non-zero-days-gh-pages]: https://non-zero-days.github.io/
[email]: mailto:alex.elia42@gmail.com
[youtube]: https://www.youtube.com/channel/UCT0hVofKq8CM8k8QBiUmpOw
[twitter]: https://twitter.com/BoredTweak
[linkedin]: https://www.linkedin.com/in/alex-elia/
[git-demo]: https://www.youtube.com/playlist?list=PLAqJ1EkmbEM2OTI0Ybor-IA7LUD6iVQ1Y

```

I encourage you to iterate on this template to better express yourself and to catalog your journey as you learn more.

Congratulations on a non-zero day!

## Additional Resources

- [Simple Icons][simpleicons]
- [Shields IO][shieldsio]
- [Markdown Reference](https://www.markdownguide.org/basic-syntax)

[simpleicons]: https://simpleicons.org/
[shieldsio]: https://shields.io/