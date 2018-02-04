![USEDPOST](https://img.shields.io/badge/USES-HTML-green.svg?style=for-the-badge) ![USEDPOST](https://img.shields.io/badge/USES-GIT-orange.svg?style=for-the-badge) ![USEDPOST](https://img.shields.io/badge/USES-Javascript-blue.svg?style=for-the-badge)

Bowling Challenge
=================
# Approach
**What has been done:**
1. First read the basic rules of bowling and create the various user stories and diagrams [(notes)](./docs/details.jpg)
2. For each step of a particular user story, start with a simple test, see it fail and then write the simplest possible code to make it pass.
4. Refactor Code
5. Re-iterate steps 2 - 3 for each step of each user story, until all user stories have been addressed

**Future Work:**
* Add messages/prompts in interface for the various cases (e.g. STRIKE/SPARE/PERFECT GAME/GUTTER GAME)
* Add the ability to have more than two players playing
* Do more extensive testing (at moment only testing very main issues)

# Basic Rules of Bowling

A bowling game consists of 10 frames in which the player tries to knock down the 10 pins. In every frame the player can roll one or two times. The actual number depends on strikes and spares. The score of a frame is the number of knocked down pins plus bonuses for strikes and spares. After every frame the 10 pins are reset.

### Bowling — how does it work?

#### Strikes

The player has a strike if he knocks down all 10 pins with the first roll in a frame. The frame ends immediately (since there are no pins left for a second roll). The bonus for that frame is the number of pins knocked down by the next two rolls. That would be the next frame, unless the player rolls another strike.

#### Spares

The player has a spare if the knocks down all 10 pins with the two rolls of a frame. The bonus for that frame is the number of pins knocked down by the next roll (first roll of next frame).

#### 10th frame

If the player rolls a strike or spare in the 10th frame they can roll the additional balls for the bonus. But they can never roll more than 3 balls in the 10th frame. The additional rolls only count for the bonus not for the regular frame count.

    10, 10, 10 in the 10th frame gives 30 points (10 points for the regular first strike and 20 points for the bonus).
    1, 9, 10 in the 10th frame gives 20 points (10 points for the regular spare and 10 points for the bonus).

#### Gutter Game

A Gutter Game is when the player never hits a pin (20 zero scores).

#### Perfect Game

A Perfect Game is when the player rolls 12 strikes (10 regular strikes and 2 strikes for the bonus in the 10th frame). The Perfect Game scores 300 points.

In the image below you can find some score examples.

More about ten pin bowling here: http://en.wikipedia.org/wiki/Ten-pin_bowling

![Ten Pin Score Example](images/example_ten_pin_scoring.png)

## How to install

First you need to clone the depository on your local machine. To do so, please open your favourite CLI and use the following commands:

```
git clone git@github.com:lunaticnick/makersacademy-mcw05-bowling-challenge.git local_directory_name
cd local_directory_name
```

#### Play ####

and then open ```index.html```, which is located inside **src** folder, using your favourite browser.

![Game interface](images/game.png)


#### Testing Framework ####

If you want to see the testing done using [Jasmine](https://jasmine.github.io) please open ```SpecRunner.html```, which is located in root, using your favourite browser.

![test interface](images/tests.png)
