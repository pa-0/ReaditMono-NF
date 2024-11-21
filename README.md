# Readit (Reddit) Mono Nerd Font

![PLACEHOLDER](/RedditMono.png)

Can we add Nerd Fonts to the [Reddit Sans Mono](https://github.com/reddit/redditsans) font family using a GitHub Action?

Inspired by [Scott Hanselman](https://www.hanselman.com/blog/PatchingTheNewCascadiaCodeToIncludePowerlineGlyphsAndOtherNerdFontsForTheWindowsTerminal.aspx) and [Alistair Young](https://github.com/microsoft/cascadia-code/issues/10?WT.mc_id=-blog-scottha#issuecomment-532969414) and, most of all, Adam Cooper, whose effort with the [patched Cascadia family (à la Delugia Code)](https://github.com/adam7/delugia-code "Delugia Code") laid the (automation) groundwork for patching Readit Sans Mono.

Adam wrote a [blog post with more details](https://admcpr.com/automating-the-patching-of-cascadia-code-to-include-nerd-fonts) about how this works.

[![Actions Status](https://github.com/pa-0/RedditMono-NerdFont/workflows/Generate%20Fonts/badge.svg)](https://github.com/pa-0/RedditMono-NerdFont/actions)

## What are Nerd Fonts anyway

[Nerd Fonts](https://www.nerdfonts.com) takes popular programming fonts and adds a bunch of Glyphs. They include all the absolutely [indispensable symbols](https://github.com/ryanoasis/nerd-fonts/wiki/Glyph-Sets-and-Code-Points) all nerds need in their favorite fonts.
Go to their [repository](https://github.com/ryanoasis/nerd-fonts) or have a look at the [overview](https://www.nerdfonts.com/#cheat-sheet).

Typically they come in two flavours:

* Powerline (adds the symbols needed to have a basic [Powerline](https://github.com/powerline) and some more.)
* Mono (adds even more Powerline symbols and all other symbols Nerd Fonts has collected.)

_Powerline_ includes these symbols:

* Powerline Symbols
* [Seti-UI](https://atom.io/themes/seti-ui#current_icons)
* [Devicons](http://vorillaz.github.io/devicons/)

_Complete_ includes these symbols additionally:

* [Powerline Extra Symbols](https://github.com/ryanoasis/powerline-extra-symbols)
* [Pomicons](https://github.com/gabrielelana/pomicons)
* [Font Awesome](https://github.com/FortAwesome/Font-Awesome) and [Extension](https://github.com/AndreLZGava/font-awesome-extension)
* [Power Symbols](https://unicodepowersymbol.com/)
* [Material Design Icons](https://github.com/Templarian/MaterialDesign)
* [Font Logos](https://github.com/Lukas-W/font-logos)
* [Octicons](https://github.com/github/octicons)

## Which font faces are available

These two font versions are generated from Reddit Sans Mono:

* **Readit Sans Mono Powerline** _Basic powerline glyphs, monospaced font_
* **Readit Sans Mono** _All Nerd Fonts glyphs, monospaced font with ALL powerline fonts (including nonstandard)_

All of these are available in light, regular, medium, semi-bold, bold and extra bold weights.

## How is Readit Sans Mono special?

Compared with the official nerd-font patched font families:

* Readit Sans Mono is not available in the official repository (at least not yet)
* Added symbol ``⚡`` (0u26A1) used with some popular Powerline setups (but not 'Complete')

## How to use

You can download the patched fonts from the [Releases page](https://github.com/pa-0/RedditMono-NerdFont/releases) of this
repo and install them as you would any other font. Once installed the font can be referenced as `Readit Sans Mono *`.
So if, for example, you want to use it in Windows Terminal you should add the lines

```json
                "font":
                {
                    "face": "Delugia"
                }
```

to the corresponding profiles in your settings.json.

## Example for Delugia on the command line

![PLACEHOLDER-Powerline](/placeholder_powerline.png)

## Help(!!!)

I know basically nothing about patching fonts so all contributions are 🦸‍ welcome.

>[!Note]
> To reduce the font name length the 'Nerd Font' has been dropped out of the (file) names.
