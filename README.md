# My macOS setup

> List of applications and tools that make my macOS experience better.

## Development

### [ Alacritty ](https://github.com/alacritty/alacritty) - GPU-accelerated Terminal Emulator

Before Alacritty, I've been using [iTerm2](https://www.iterm2.com/) for a long time. And while it was a really great, mature project, I began to have some issues with it, like colors not displaying correctly with my [NeoVim configuration](https://github.com/tansawit/dotfiles/blob/master/nvim/init.vim). Then I found Alacritty through [Fatih Arslan's](https://arslan.io) blog [post](https://arslan.io/2018/02/05/gpu-accelerated-terminal-alacritty/) and it was amazing:

- No more problem with colors
- Fast...like [really fast](https://news.ycombinator.com/item?id=20587809)
- Really easy shortcut keys rebinding

There are some problems that I still have with it or things I hope get implemented though:

- Ligature support
- Resizing windows is still really rough and really slow

My setup:

![Alacritty terminal appearance](/images/alacritty.png)

### [ Neovim ](https://neovim.io/) - 'Modern' Vim fork of choice

- Amazing text-editing experience. Took a while for me to get somewhat comfortable with it but it will absolutely change the way you think about text editing. Because of this, 
- I have started to find ways to use Vim key-bindings in as many apps as possible. If there's some sort of extension or plugin to allow me to do that, I'll use it.
- My configuration can be found [here](https://github.com/tansawit/dotfiles/blob/master/nvim/init.vim). As with any other app that I can customize, I use the [Nord theme](https://github.com/arcticicestudio/nord-vim) along with various plugins.

Here's how it looks with some Go code:

![NeoVim setup](/images/nvim.png)


### [ Tmux ](https://github.com/tmux/tmux) - Terminal multiplexer

After moving to Alacritty, I've begun using tmux to handle making multiple terminal panes/windows. It has also allowed me to run some web server that I frequently use in the background (my Hugo website server, for example) without having to restart it everytime I open the terminal. Still need to do a lot more exploring of what it can do though.

See [here](https://github.com/tansawit/dotfiles/blob/master/tmux/tmux.conf) for my tmux configuration.

### [ Visual Studio Code ](https://code.visualstudio.com/) - Text Editor

To be honest I mostly use it nowadays to look through the structure of projects that I'm unfamiliar with, or if I don't have the time to properly setup my neovim for a new language.

### [ Git Tower ](https://www.git-tower.com/) - Git client

There in case of really large, multi-contributor projects I might be involved in the future. Right now a combination of [git](https://git-scm.com/book/en/v2/Getting-Started-The-Command-Line), [gh](https://github.com/cli/cli), and [hub](https://github.com/github/hub) is enough for me.

I do occasionally use it to search through commits, check out branches with ease and searching through all the Git repositories I have on my mac though.

### [ Paw ](https://paw.cloud/) - REST API Client

Out of the three clients I've tried ([Postman](https://www.postman.com/), [Insomnia](https://insomnia.rest), and Paw), Paw feels the most 'right' to me. Postman is someone beyond what I need right now, and Insomnia I just can't bring myself to use it for some reason. Plus Paw has the awesome feature of [generating code from the specified API call](https://paw.cloud/docs/getting-started/code-generator), which is really neat. 

### [ TablePlus ](https://tableplus.com/) - Modern GUI for databases

A really nice-looking and modern GUI for databases that supports quite [a lot of databases](https://docs.tableplus.com/#supported-databases), both SQL and NoSQL. Bonus points for having native apps for Mac and Windows. A really refreshing change coming from [Sequel Pro](http://sequelpro.com/). 

Some features are still incomplete/buggy though like the import functions seem to fail in some cases that Sequel Pro can handle. Plus I hope the app is a little less expensive, but then again I'm using it through my [SetApp subscription](https://setapp.com/). Ultimately, I still think it's completely worth it for anyone who works a lot with databases.

### [ Dash ](https://kapeli.com/dash) - Documentation Browser

Allows you to download any docset that you might want to use, search for any method, class or anything that you need very quickly, comes with the amazing Alfred workflow to simplify the process of searching for the right things. 

After combining it with [Alfred](https://www.alfredapp.com/), the [Dash Alfred workflow](https://github.com/Kapeli/Dash-Alfred-Workflow) and [Karabiner](https://pqrs.org/osx/karabiner/), it has become indispensable for me when looking up language libraries/functions and other things.

![Dash example](/images/dash.png)

## Design

### [ Sketch ](https://www.sketch.com/)

What I use whenever I have to design an app, site, or any other thing.

### [ Flinto ](https://www.flinto.com/)

## Utilities

### [ 1Password ](https://1password.com/)

- Generate all of my passwords with it and keep everything in a secured and encrypted vault kept secure by my one master password.
- I no longer need to remember passwords and I now have a unique password for every website that I am signed up
- Really convenient [2FA integration](https://support.1password.com/one-time-passwords/). It copies the code to your clipboard instead of you having to look it up on an app/on your phone etc.

### [ Alfred ](https://www.alfredapp.com/)

One of the reasons I initially fell in love with macOS was its amazing search using Spotlight. Then I found Alfred and was even more impressed by it. Apart from its built-in features, its [Workflows](https://www.alfredapp.com/workflows/) features allow for incredible extensibility. Some of these that I use most often are:

- [alfred-github-jump](https://github.com/lox/alfred-github-jump): Quickly search and open your repositories or those you starred in your default browser.
- [dash-alfred-workflow](https://github.com/Kapeli/Dash-Alfred-Workflow): Search and open Dash documentation sets through GitHub. (More on this below)
- [ask-create-share](https://github.com/nikitavoloboev/alfred-ask-create-share): Quickly create web submissions (GitHub repos/gist, Stack Exchange, Google Doc files, etc.)
- [alfred-localhost](https://github.com/simonguest/alfred-localhost): Open localhost with the input port in a new tab in the default browser

### [ Lightshot ](https://apps.apple.com/us/app/lightshot-screenshot/id526298438)
### [ AppCleaner ](https://freemacsoft.net/appcleaner/)

Really simple tool to completely uninstall apps from my computer, including files that might have been stored in various other directories aside from the Applications folder.

### [ Contexts ](https://contexts.co/)

Fuzzy search through all the currently active windows that I have.

![Contexts example](/images/contexts.png)

### [ KeyboardCleanTool ](https://folivora.ai/keyboardcleantool)

A tool to temporarily disable the keyboard for cleaning/fixing etc.

### [ Bartender ](https://www.macbartender.com/) - Menubar organization

Allows you to customize and hide the contents of your menu bar for a cleaner look.

### [ Typinator ](https://www.ergonis.com/products/typinator/) - Text Expansion

### [ Karabiner ](https://pqrs.org/osx/karabiner/)

This tool completely changed the way I interact with my computer, and I personally feel a lot more productive with it. Beyond describing it as somewhat similar to Windows' [AutoHotKey](https://www.autohotkey.com/), being a kernel extension that gives you a virtual keyboard you can heavily customize, I don't exactly know how to describe it, so instead, I'll outline some of the keys and key combinations I've configured with it:

*Note: `x-y` means press key `y` while holding down `x`*

- `Caps Lock` now acts as my `esc` key. This greatly helps when I'm using (neo)vim (my main text/code editor) as I don't need to stretch as far or to try to find the virtual key on my MacBook's touchbar.
- `right command` brings up Alfred, instead of having to press the usual `command-space`
- `left command` quickly brings up the previous application, replacing the traditional `command-tab`

When combined with Alfred workflows or [Keyboard Maestro](https://www.keyboardmaestro.com/main/), it becomes even more powerful: 

- `n-f` brings up `alfred-github-jump`
- `n-a` brings up `ask-create-share`
- `l-c` brings up `alfred-localhost`

And so on. While it might seem like these improvements are minor, I assure you the time and effort saved is definitely noticeable over time. 

To that extent, I'm also only just getting started with exploring what it can do so for more information on Karabiner and combining it with other tools, I urge you to check out Nikita Voloboev's [post on the topic](https://medium.com/@nikitavoloboev/karabiner-god-mode-7407a5ddc8f6). He's how I got started on all of this whole customization and optimization thing as well.

### [ Keyboard Maestro ](https://www.keyboardmaestro.com/main/) - Automation Tool

Keyboard Maestro is essentially an IDE for automation. You create macros of actions that you can then easily call from Karabiner.

### [ Magnet ](https://apps.apple.com/th/app/magnet/id441258766) - Windows manager
### [ Vimac ](https://vimacapp.com/)

After falling down the Vim rabbit-hole, I've been trying to find ways to use Vim-based/keyboard-only navigations in as many contexts as possible. And other than my terminal, the two contexts that I normally use my mouse are in my browser (Chrome) and general app/program navigation. Having found [Surfingkeys](https://github.com/brookhong/Surfingkeys) for Chrome, I tried to find a similar solution for general application and interface navigation. Thus, enters Vimac.

The app allows you to assign a hotkey which, once pressed, will show a layer of shortcut keys over any recognized clickable elements on the screen (example below). After pressing the desired key combination, the app will simulate a mouse click on that element. Even though the app seems to work pretty well most of the time, its beta status definitely shows. Sometimes the assigned keyboard shortcut does not register, and some places that are buttons/navigation are not recognized. But overall I'm definitely happy with it.

![Vimac Example](/images/vimac.png)

## SetApp

### [ SetApp ](https://setapp.com/) - Collection of Mac Apps

How I get a lot of my apps.

### [ Paste ](https://setapp.com/apps/paste)
### [ Sip ](https://setapp.com/apps/sip)

Whenever I needed to get the color value of some digital assets before, I've always used macOS's built-in Digital Color Meter. But I always ran into the issue of having no integrated way to store the retrieved colors, let alone multiple color sets or palettes. Sip solves these issues with its color palette manager, a more fully-fledged and easy to use the color picker, and cloud sync.

![Sip Color Palette Manager](/images/sip.png)

### [ Expressions ](https://setapp.com/apps/expressions)

A really easy way to test and play with [Regular Expressions](https://en.wikipedia.org/wiki/Regular_expression) (regex) without having to think about specific language library libraries/functions/syntax. Simply enter the expressions and the test string(s). Plus I love the minimalistic and clean UI.

![Expressions RegEx](/images/expressions.jpg)
