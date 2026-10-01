---
title: "Plugin Overview"
description: "Overview of the plugins used in Just the Games"
nav_order: 1
parent: 🔨 Make Your Own
---

# Plugin Overview
{: .no_toc }

Already have a *[Just The Docs](https://github.com/just-the-docs/just-the-docs)* site? Include these plugins in your `Gemfile` and `_config.yml` and you're done!

```ruby
# Gemfile
group :jekyll_plugins do
        gem "jekyll-hover-popup" # Link hovering preview windows
        gem "jekyll-jtd-toc-nav" # Table of Contents in the navigation bar
        gem "jekyll-dice-tray" # Dice tray with clickable dice notation recognition
        gem "jekyll-image-links" # Custom image-map features
        gem "rpg-callouts" # additional callout formatting options 
        gem "dark-dungeons-theme" # dark overlay for the default theme
end
```

```yml
# _config.yml
plugins: 
  - jekyll-jtd-toc-nav 
  - jekyll-dice-tray
  - jekyll-hover-popup
  - jekyll-image-links
  - rpg-callouts 
  - dark-dungeons-theme
```

## Hover Popup Previews 

GitHub [hover-popup](https://github.com/sunflowermans/hover-popup) | Ruby Gem [jekyll-hover-popup](https://rubygems.org/gems/jekyll-hover-popup/)

### Features
* Preview windows for [internal links](/docs/make-your-own/plugin-feature-overview/#hover-popup-previews)
* Pin windows by holding the SHIFT key
* Move and resize by draging
* Minimize or expand by double clicking the title bar

## Dice Tray

GitHub [dice-tray](https://github.com/sunflowermans/dice-tray) | Ruby Gem [jekyll-dice-tray](https://rubygems.org/gems/jekyll-dice-tray)

### Features
* Automatic dice notation links: 2d6, d20+1, 2-in-6, d6 + d8 (take highest result)
* Type your own
* History
* Automatic dice table results (example below)

<br>

| d6      | Code Name |  Blog     |
| :-------: |:---: | :-------------: |
| 1 | Doctor Worm | [Rise Up Comus](https://riseupcomus.blogspot.com/) |
| 2 | V for Valeria | [Valeria Loves](https://valerialoves.com/) |
| 3 | Big D Energy |  [I Cast Light](https://icastlight.blogspot.com/) |
| 4 | Oakcat |  [Among Cats and Books](https://elmc.at/) |
| 5 | W. F. Sandshrew |  [Prismatic Wasteland](https://www.prismaticwasteland.com/) |
| 6 | 1/2 HD Dragon |  [Explorer's Design](https://www.explorersdesign.com/) |


## Table of Contents Navigation

GitHub [toc-navigation](https://github.com/sunflowermans/toc-navigation) | Ruby Gem [jekyll-jtd-toc-nav](https://rubygems.org/gems/jekyll-jtd-toc-nav)

### Features
By default, *Just The Docs* doesn't include document headers in the side navigation bar. This plugin injects the table of contents into the navigation bar with collapsible links.

![TOC in Nav](/assets/images/toc-nav-demo-1.png)

## Image Links

GitHub [image-links](https://github.com/sunflowermans/image-links) | Ruby Gem [jekyll-image-links](https://rubygems.org/gems/jekyll-image-links)

### Features
* Click a region to navigate to an internal or external link
* Optional region labels overlaid on the image
* Optional **Dynamic Map Viewer** button with zoom, pan, and region highlighting
* Automatic point rescaling for variable image dimensions (i.e. `width: 50%`)
* Works natively with the preview window plug-in

![Custom image maps](/assets/images/image-map-demo-1.png)

## RPG Callouts

GitHub [rpg-callouts](https://github.com/sunflowermans/rpg-callouts) | Ruby Gem [rpg-callouts](https://rubygems.org/gems/rpg-callouts)

### Features
* Adventure-ready callout styles: `monster`, `monster-no-title`, and `item`
* Merges definitions into Just the Docs callouts at build time
* Site `_config.yml` wins on name clashes
* In-memory only — nothing is copied into the site source

{: .monster}
> **Goblin**
>
> AC 6 [13], HD 1-1 (3hp), Att 1 × spear (1d6)

{: .item}
> **Silver Key**
>
> Opens the locked door in area 3.

## Dark Dungeons Theme

GitHub [dark-dungeons-theme](https://github.com/sunflowermans/dark-dungeons-theme) | Ruby Gem [dark-dungeons-theme](https://rubygems.org/gems/dark-dungeons-theme)

### Features
* Dark Dungeons color scheme overlay for Just the Docs
* Leaves site title, favicon, navigation, and page content unchanged

Inspired by the [Designing Dungeons Course](https://dungeons.hismajestytheworm.games/).