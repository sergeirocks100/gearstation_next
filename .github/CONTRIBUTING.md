# CONTRIBUTING

1. [Reporting Issues](#reporting-issues)
2. [Introduction](#introduction)
3. [Getting Started](#getting-started)
4. [Legal Notice](#legal-notice)
5. [Meet the Team](#meet-the-team)
	1. [Headcoder](#headcoder)
	2. [Maintainers](#maintainers)
	3. [Issue Managers](#issue-managers)
6. [Development Guides](#development-guides)
7. [Pull Request Process](#pull-request-process)
8. [Good Boy Points](#good-boy-points)
9. [Porting features/sprites/sounds/tools from other codebases](#porting-featuresspritessoundstools-from-other-codebases)
10. [Restricted content](#restricted-content)
11. [Banned content](#banned-content)
12. [A word on Git](#a-word-on-git)

## Reporting Issues

If you ever encounter a bug in-game, the best way to let a coder know about it is with our GitHub Issue Tracker. Please make sure you use the supplied issue template, and include the round ID for the server.

(If you don't have an account, making a new one takes only one minute.)

If you have difficulty, ask for help in the #development channel on our discord.

## Introduction

Hello and welcome to GearStation's contributing page. You are here because you are curious or interested in contributing - thank you! Everyone is free to contribute to this project as long as they follow the simple guidelines and specifications below; at GearStation, we strive to maintain code stability and maintainability, and to do that, we need all pull requests to hold up to those specifications. It's in everyone's best interests - including yours! - if the same bug doesn't have to be fixed twice because of duplicated code.

First things first, we want to make it clear how you can contribute (if you've never contributed before), as well as the kinds of powers the team has over your additions, to avoid any unpleasant surprises if your pull request is closed for a reason you didn't foresee.

## Getting Started

GearStation doesn't have a list of goals and features to add; we instead allow freedom for contributors to suggest and create their ideas for the game. That doesn't mean we aren't determined to squash bugs, which unfortunately pop up a lot due to the deep complexity of the game. Here are some useful starting guides, if you want to contribute or if you want to know what challenges you can tackle with zero knowledge about the game's code structure.

If you want to contribute the first thing you'll need to do is [set up Git](https://hackmd.io/@tgstation/HJ8OdjNBc) so you can download the source code.
After setting it up, optionally navigate your git commandline to the project folder and run the command: `git config blame.ignoreRevsFile .git-blame-ignore-revs`.

We have a [list of guides on the wiki](https://gearstation.tk/wiki/index.php?title=Guides) that will help you get started contributing to GearStation with Git and Dream Maker. For beginners, it is recommended you work on small projects like bugfixes at first. If you need help learning to program in BYOND, check out this [repository of resources](http://www.byond.com/developer/articles/resources).

There is an open list of approachable issues for [your inspiration here](https://github.com/sergeirocks100/GearStation_Next/issues).

You can of course, as always, ask for help on the Discord channels or the forums. We're just here to have fun and help out, so please don't expect professional support.

## Legal Notice

When it comes to original, from scratch contributions, by opening a pull request on GearStation, you (And any co-contributors) agree to license your code contributions under the [GNU AGPL V3](https://www.gnu.org/licenses/agpl-3.0.html), and other forms of contributions (Icons, sounds, maps, etc.) under [Creative Commons BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).

You also agree that, unless you specify otherwise in the pull request, that the Github usernames of the contributors involved, along with a link back to the pull request, are how you should be credited if someone were to port your contributions, or otherwise make use of them in ways where credit is required.

To put it simply, by contributing to GearStation, you agree to allow others to use and modify your contributions as they see fit, including for commercial purposes, as long as they give you credit, and make the source code public.

If you don't want people to freely reuse and modify your stuff, don't contribute to GearStation.

When it comes to contributions you didn't make entirely yourself (Ports from other codebases, use of outside code or assets, etc.), refer to the [porting guidelines](#porting-featuresspritessoundstools-from-other-codebases).

## Meet the Team

### Headcoder

The Headcoder is responsible for controlling, adding, and removing maintainers from the project. In addition to filling the role of a normal maintainer, they have sole authority on who becomes a maintainer, as well as who remains a maintainer and who does not.

### Maintainers

Maintainers are quality control. If a proposed pull request doesn't meet the following specifications, they can request you to change it, or simply just close the pull request. Maintainers are required to give a reason for closing the pull request.

Maintainers can revert your changes if they feel they are not worth maintaining or if they did not live up to the quality specifications.

<details>
<summary>Maintainer Guidelines</summary>

These are the directives we have for project maintainers.

- Do not merge pull requests without prior headcoder approval, unless the pull request's changes don't have a major impact on the intended playability or appearance of the game (bugfixes, quality-of-life improvements, etc.), or no headcoder reply is given within 48 hours of approval being requested.
- Do not merge pull requests you create.
- Do not merge pull requests until 24 hours have passed since it was opened. Exceptions include:
  - Emergency fixes.
    - Try to get secondary maintainer approval before merging if you are able to.
  - Pull requests with empty commits intended to generate a changelog.
- Do not merge pull requests that contain content from the [banned content list](./CONTRIBUTING.md#banned-content).
- Do not close pull requests purely for breaking a template if the same information is contained without it.
- Do not modify the body or title of a pull request you didn't create without prior headcoder approval.
  - In addition, any and all body or title changes must be clearly marked as being made by you.

These are not steadfast rules as maintainers are expected to use their best judgement when operating.

Our team is entirely voluntary, as such we extend our thanks to maintainers, issue managers, and contributors alike for helping keep the project alive.

</details>

### Issue Managers

Issue Managers help out the project by labelling bug reports and PRs and closing bug reports which are duplicates or are no longer applicable.

<details>
<summary>What You Can and Can't Do as an Issue Manager</summary>

This should help you understand what you can and can't do with your newfound github permissions.

Things you **CAN** do:
* Label issues appropriately
* Close issues when appropriate
* Label pull requests.

Things you **CAN'T** do:
* [Close pull requests](https://imgur.com/w2RqpX8.png): Only maintainers are allowed to close pull requests. Do not hit that button.
* Close issues purely for breaking a template if the same information is contained without it.

</details>

## Development Guides

#### Writing readable code 
[Style guide](./guides/STYLE.md)

#### Writing sane code 
[Code standards](./guides/STANDARDS.md)

#### Writing understandable code 
[Autodocumenting code](./guides/AUTODOC.md)

#### Misc

- [AI Datums](../code/datums/ai/making_your_ai.md)
- [Embedding TGUI Components in Chat](../tgui/docs/chat-embedded-components.md)
- [Hard Deletes](./guides/HARDDELETES.md)
- [MC Tab Guide](./guides/MC_tab.md)
- [Policy Configuration System](./guides/POLICYCONFIG.md)
- [Splitting up pull requests, aka atomization](./guides/ATOMIZATION.md)
- [Required Tests (Continuous Integration)](./guides/CI.md)
- [UI Development](../tgui/README.md)
- [Visual Effects and Systems](./guides/VISUALS.md)

## Pull Request Process

There is no strict process when it comes to merging pull requests. Pull requests will sometimes take a while before they are looked at by a maintainer; the bigger the change, the more time it will take before they are accepted into the code. Every team member is a volunteer who is giving up their own time to help maintain and contribute, so please be courteous and respectful. Here are some helpful ways to make it easier for you and for the maintainers when making a pull request.

* Make sure your pull request complies to the requirements outlined here

* You are expected to have tested your pull requests if it is anything that would warrant testing. Text only changes, single number balance changes, and similar generally don't need testing, but anything else does. This means by extension web edits are disallowed for larger changes.

* You are going to be expected to document all your changes in the pull request. Failing to do so will mean delaying it as we will have to question why you made the change. On the other hand, you can speed up the process by making the pull request readable and easy to understand, with diagrams or before/after data. Should you be optimizing a routine you must provide proof by way of profiling that your changes are faster.

* We ask that you use the changelog system to document your player facing changes, which prevents our players from being caught unaware by said changes - you can find more information about this [on this wiki page](http://tgstation13.org/wiki/Guide_to_Changelogs).

* If you are proposing multiple changes, which change many different aspects of the code, you are expected to section them off into different pull requests in order to make it easier to review them and to deny/accept the changes that are deemed acceptable.

* If your pull request is accepted, the code you add no longer belongs exclusively to you but to everyone; everyone is free to work on it, but you are also free to support or object to any changes being made, which will likely hold more weight, as you're the one who added the feature. It is a shame this has to be explicitly said, but there have been cases where this would've saved some trouble.

* If your pull request is not finished, you may open it as a draft for potential review. If you open it as a full-fledged PR make sure it is at least testable in a live environment. Pull requests that do not at least meet this requirement will be closed. You may request a maintainer reopen the pull request when you're ready, or make a new one.

* While we have no issue helping contributors (and especially new contributors) bring reasonably sized contributions up to standards via the pull request review process, larger contributions are expected to pass a higher bar of completeness and code quality *before* you open a pull request. Maintainers may close such pull requests that are deemed to be substantially flawed. You should take some time to discuss with maintainers or other contributors on how to improve the changes.

* After leaving reviews on an open pull request, maintainers may convert it to a draft. Once you have addressed all their comments to the best of your ability, feel free to mark the pull as `Ready for Review` again.

## Justifying Your Changes

You must explain why you are submitting the pull request in the "Why It's Good For The Game" section of your pull request, and how you think your change will be beneficial to the game. Failure to do so will be grounds for rejecting your pull request wholesale, or requiring that you fix it before your pull request is merged. A reasonable justification for your changes is a requirement. 

Your "Why It's Good For The Game" section must make a good faith and reasonable attempt to:
* Assert and argue that the current state of affairs in the game is not good, and needs changing.
* Assert and argue that your pull request will either fix or help fix the problems you described.
* Assert and argue that any downsides introduced by your solution as a matter of design, if any, are worth it, and why they are worth it.

More controversial changes have higher standards for justification to be considered reasonable. A bugfix for example does not typically require any effort at all in justification as its value to the game is usually self evident, however a major feature overhaul or balance change may require significant explanation to adequately justify its supposed benefit to the game.

This is still a requirement if your pull request is supported and/or requested by maintainers before it is opened. This is still a requirement if your pull request is supported and/or requested by head coders before it is opened. The purpose of arguing for your changes is not to convince just the maintainer team of its merits, it is to document the "why" behind your changes to the game to a necessary level of detail. The reason behind a change must exist as it is the purpose of this codebase to improve the game, thus said reasoning must be adequately stated and explained.

This is also still a requirement if your pull request has a corresponding design document that justifies your changes inside it. You must always properly justify changes (those that actually need justification) within the pull request, even if you also do it elsewhere. This is to ensure that:
1. All reviewers can easily see the reasoning behind your changes on the pull request itself, no reliance on other sites required.
2. The actual, manifested implementation of the idea behind the design document is being justified after said implementation is actually realized. This is in contrast to any reasoning put on the design document itself, which very well may have been made before any work was done on it, possibly even by an author different from the author of the pull request. Any idea in the design document may have had compromises put into it due to complications not seen in the original vision, thus the current state of the implementation (the pull request as it stands) must be defended, explained, and ultimately justified in and of itself. Of course, you should still list the design document the pull request is implementing, and may even use arguments from the design document if said arguments are applicable to the current reality of your proposed changes.

## Good Boy Points

Each GitHub account has a score known as Good Boy Points, or GBP. This is a system we use to ensure that the codebase stays maintained and that contributors fix bugs as well as add features.

The GBP gain or loss for a PR depends on the type of changes the PR makes, represented by the tags assigned to the PR by the tgstation github bot or maintainers. Generally speaking, fixing bugs, updating sprites, or improving maps increases your GBP score, while adding mechanics, or rebalancing things will cost you GBP.

The GBP change of a PR is the sum of greatest positive and lowest negative values it has. For example, a PR that has tags worth +10, +4, -1, -7, will net 3 GBP (10 - 7).

Negative GBP increases the likelihood of a maintainer closing your PR. With that chance being higher the lower your GBP is. Be sure to use the proper tags in the changelog to prevent unnecessary GBP loss. Maintainers reserve the right to change tags as they deem appropriate.

There is no benefit to having a higher positive GBP score, since GBP only comes into consideration when it is negative.

You can see each tag and their GBP values [Here](https://github.com/tgstation/tgstation/blob/master/.github/gbp.toml). 

## Porting features/sprites/sounds/tools from other codebases

If you are porting features/tools from other codebases, you must give them credit where it's due. Typically, crediting them in your pull request and the changelog is the recommended way of doing it. Take note of what license they use though, ports from AGPLv3 and GPLv3 codebases are allowed.

Regarding sprites & sounds, you must credit the artist and possibly the codebase. All GearStation assets including icons and sound are under a [Creative Commons BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/) unless otherwise indicated.

Because GearStation is a codebase that believes in software freedom. assets or code that are under non-free licenses (such as the [Creative Commons BY-NC-SA 3.0 license](https://creativecommons.org/licenses/by-nc-sa/3.0/) that GoonStation and BurgerStation use) are banned from use on GearStation. If there are assets in something that you want to port that make use of non-free licenses, you may either:

A: Replace all of the offending assets with ones that you created yourself, or are otherwise under a license that GearStation accepts.

B: Get written permission from the original creator(s) to sublicense the assets under Creative Commons BY-SA 3.0, or, failing that, another license that GearStation accepts. Be sure that you get it sublicensed under an actual license; simply getting a "Hey, you can use this." or something similar won't be enough.

When it comes to code that's under non-free licenses, you should follow similar procedures. You should strongly considier rewriting the offending code from scratch instead of getting it sublicensed, as most codebases that are under non-free licenses are strongly divorced from other codebases in their programming practices, and it may take more work to try to make it work on our code than it would to just recreate it from the ground up.

However, if you wish to do so, you may try to obtain written permission to sublicense the offending code under the AGPL V3, or, failing that, another license that GearStation accepts.

The GNU website has a helpful list of free and non-free licenses [here](https://www.gnu.org/licenses/license-list.en.html).

## Restricted content
Adding any of the following in a Pull Request requires prior approval from a maintainer or headcoder:
* Code adding, removing, or updating the availability of alien races/species/human mutants. Pull requests attempting to add or remove features from said races/species/mutants require prior approval as well.
* Station maps consisting of more than one Z-level.

## Banned content
Do not add any of the following in a Pull Request or risk getting the PR closed:
* Code where one line of code is split across multiple lines (except for multiple, separate strings and comments; in those cases, existing longer lines must not be split up.).
* Any assets or code that are under non-free licenses.
* Anything that relies on Extools, Auxtools, or any other BYOND version dependent external DLLs to function.
* Anything that contains in-game references to real world news events, popular culture, or internet memes. This also applies to references to the game itself, such as the players, admins, developers, or community happenings of GearStation and other SS13 codebases.
* Anything that's meant to generate or spread real world bigotry or prejuidice.
* Code which violates GitHub's [terms of service](https://github.com/site/terms).

Just because something isn't on this list doesn't mean that it's acceptable. Use common sense above all else.

## A word on Git
This repository uses `LF` line endings for all code as specified in the **.gitattributes** and **.editorconfig** files.

Unless overridden or a non standard git binary is used the line ending settings should be applied to your clone automatically.

Note: VSC requires an [extension](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig) to take advantage of editorconfig.

Github actions that require additional configuration are disabled on the repository until the ACTION_ENABLER secret is created with a non-empty value.
