# WEB102 Prework - Ultra Cool Sea Monster Crowdfunding

Submitted by: **Adeline Greene**

**Ultra Cool Sea Monster Crowdfunding** is a website for the company Sea Monster Crowdfunding that displays information about the games they have funded.

Time spent: **6** hours spent in total

## Required Features

The following **required** functionality is completed:

* [x] The introduction section explains the background of the company and how many games remain unfunded.
* [x] The Stats section includes information about the total contributions and dollars raised as well as the top two most funded games.
* [x] The Our Games section initially displays all games funded by Sea Monster Crowdfunding
* [x] The Our Games section has three buttons that allow the user to display only unfunded games, only funded games, or all games.

The following **optional** features are implemented:

* [x] Clicking on a game card opens a modal displaying detailed information about that specific game
* [x] The UI has been updated to be more visually appealing

## Video Walkthrough

Here's a walkthrough of implemented features:

<img src='demo.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

GIF created with Windows Game Bar to make mp4, Ezgif to convert mp4 into gif, and GIPHY to share the gif.

## Notes

While making the app, I briefly became stuck on part 3. I hadn't done DOM manipulation in a while, so I really had to comb through the provided resources. Eventually, I realized I was passing the wrong variable to the addGamesToPage function, which allowed me to move on to the next challenge.

The other major problem I ran into was implementing my extra feature. I tried doing all the DOM manipulation in one function, but was having trouble selecting specific games from the games container. Instead, I figured out that it was easier to make an event listener inside the original addGamesToPage. After this, there was one additional bug. Although the modal showed the correct game after a button was clicked, the initial game cards weren't showing the correct game in the modal display. I realized that this was because GAMES_JSON was getting sorted in Challenge 7, so I added .slice() before the sorting, so that GAMES_JSON isn't modified.

## License

    Copyright [2025] [Adeline Greene]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
