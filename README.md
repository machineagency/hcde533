# A0: Webpage and IDE setup!

In this assignment you will:

- Install the Arduino IDE
- Install Git and make a Github account
- Install VS Code and some extensions
- Set up and deploy a personal portfolio site to document your work in the class

If you run into any issues, please ask questions in the #questions-and-answers
channel on Discord. If you solve an issue or learn something that might help
your fellow classmates, please post it in the #tips-and-tricks channel.

Follow the instructions in Canvas to submit a link to your portfolio website.

## Arduino Installation

Download the Arduino IDE [here](https://www.arduino.cc/en/software). Install it
and make sure it works:

- Open up the "Blink" sketch under example projects
- Click the check button in the upper left (this makes sure you are able to
  verify/compile it)

## Git Installation

[Make a Github account](https://github.com/) and
[install Github Desktop](https://desktop.github.com/). This should install git,
but in past classes some people using MacOS ran into an issue where git did not
install correctly. If you are having issues with git, try following
[this guide](https://github.com/git-guides/install-git) for your operating
system.

## VS Code Installation

We will be using Visual Studio Code (generally shortened to VS Code). VS Code is
a _highly extensible_ text editor. This means that its base function is quite
simple: you can open and edit files. You can install extensions via the
extension marketplace, which let you add bits of functionality as you need them,
such as support for different languages.

[Download and install Visual Studio Code.](https://code.visualstudio.com/).

If you have a different editor preference (e.g., Sublime), you are welcome to
use it.

Once you have installed VSCode, sign in with your Github account.

Install the following three extensions (helpful for the basic web development we
will be doing) from the extension marketplace:

- [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)

Finally, do a bit of customization and install a color theme! There are many VS
Code themes available. For fun, peruse a few (you can do this by clicking the
"filter" button and choosing `Category > Themes`) and pick one, such as:

- [Dracula](https://marketplace.visualstudio.com/items?itemName=dracula-theme.theme-dracula) -
  _my long-time favorite_
- [Monokai Pro](https://marketplace.visualstudio.com/items?itemName=monokai.theme-monokai-pro-vscode) -
  _a nice-looking option_
- Solarized Dark - _built into VS Code, used to be my previous go-to_
- [Nord](https://marketplace.visualstudio.com/items?itemName=arcticicestudio.nord-visual-studio-code) -
  _Too low-contrast for me, but I use it for other applications_
- [Gruvbox](https://marketplace.visualstudio.com/items?itemName=jdinhlife.gruvbox) -
  _A fun retro feel_

## Github Pages Setup

We will be using Github pages to host the portfolio sites where you will
document your work for the class.

### Create a new repository (repo)

1. First, create a new repository by clicking the plus button at the top right
   of the Github page.
2. On the repository creation page, name your repository `username.github.io`,
   where username is your GitHub username. **IMPORTANT**: ensure you enter
   `username.github.io` into the box - don't just enter `.github.io`. You can
   leave the rest of the settings as default.
3. Ensure that you set the repository to public (this should be the default
   option).
4. Tick the box to "Add a README file"
5. Click the "Create repository" button. You should be redirected to your new
   repository.

### Clone your repo

If you are comfortable working with git from the command line, feel free to
clone the repository that way (using `git clone repositoryname`). Alternatively,
you can clone your repo from VS Code's built-in source control interface:

1. In VS Code, hit `Control/Command-Shift-P` to open the command palette. Start
   typing `git:Clone`. The autocomplete option should show up quickly, use the
   arrow keys to navigate to it and hit enter.
2. Select `Clone from GitHub`. Your available repositories should show up; it
   might take a second. You also might need to sign in to VS Code with your
   Github credentials.
3. In the dropdown menu, select the repository you just created and choose a
   location on your computer to clone it to. I use a folder called "code" in my
   home directory to store all of my active projects.
4. VS Code will ask you if you want to open the cloned repository. Select "Open
   in new window". VSCode will open a new window.

### Copy in the template

There is a folder called `template` in this (the class) repo. Copy the contents
(the html files, the image, and the css file) into the your new portfolio repo
folder. You can download this repo as a zip file by going to the main page,
clicking the green "Code" dropdown, and selecting "Download ZIP".

### Viewing the example site

Once you have copied the files (and assuming you have installed the VSCode Live
Server extension), right click on `index.html` in the explorer side bar and
click "Open with Live Server". The page should open automatically in your
browser. You can now edit the files containing your site code and your changes
will immediately update the browser - no need to restart the server.

## Working on your site!!

Now let's customize and build your portfolio site! Start by reading through the
HTML and understanding how each portion corresponds to what you see in your
browser. You can now begin editing your site by tweaking the template.

Edit the index.html file to include your name and 1-2 sentences about yourself.
Replace the image of a red panda with an image of yourself (or an avatar).

### Deploy your site by committing and pushing your changes

These are instructions to commit and push your changes using VSCode's built-in
source control interface. You can also commit and push your work from the
command line if you are comfortable using it (and we encourage practicing this
so as to not be overly-reliant on the GUI).

1. Open the "Source control" panel in VS Code's left sidebar. You should see a
   list of changes you have made. This panel shows information similar to the
   output of the command `git status`.
2. Hover over the header that says "Changes". You should see a Plus icon (+)
   appear to the right. Click it to stage your changes. This is the equivalent
   to running `git add --all` or `git add .` in the terminal.
3. Enter a commit message (e.g. "Testing my portfolio site") in the text entry
   box above (which should say "message"), and click the "Commit" button. This
   is equivalent to running `git commit -m "my commit message"` in the terminal.
4. The "Commit" button should turn into a button that says "sync changes" -
   click it. This is equivalent to running `git push`. This will push your work
   to your remote repository that is stored on Github's servers.
5. Assuming you are successful, you should see the example site online at
   username.github.io in a few minutes! Turn in a link to your site on Canvas.

### Resources

Here are some resources you can use while you customize your site. The MDN Web
docs are a fantastic resource and one of my personal favorites. Their
[getting started guide](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web)
is a great introduction to these various technologies and how they fit together.
The "Getting started" covers most of what you might need to know when editing
your site to turn in your work, particularly the following articles:

- [Dealing with files](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/Dealing_with_files) -
  to understand how files are structured
- [HTML Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics) -
  to get an overview of how an HTML document is structured and what tags are
  available to you
- [CSS Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics) -
  to understand how HTML can be styled
- [How the web works](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works) -
  to understand the grand scheme

The following sections on HTML and CSS are much longer. Look at the topics
listed in the sidebar and feel free to read any articles that look interesting.
The articles that are probably most useful for you in this class are:

- [HTML: Creating hyperlinks](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks)
- [HTML: Images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)
- [HTML: Debugging](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Debugging_HTML)
- [CSS: Text and Font Styling](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals)
- [CSS: Sizing](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Sizing_items_in_CSS)
- [CSS: Layout](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Introduction)
- [CSS: Debugging](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Debugging_CSS)
- [CSS: Transitions](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions)

## Additional resources

- [HTML elements reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)
- [CSS selectors overview](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors)
- [CSS cheat sheet](https://websitesetup.org/wp-content/uploads/2019/11/wsu-css-cheat-sheet-gdocs.pdf)
