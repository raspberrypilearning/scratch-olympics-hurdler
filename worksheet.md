# The Scratch Olympics Hurdler

In this activity you will make a hurdles game using Scratch, where the speed of the runner is controlled by how fast you can hit the `x` and `z` keys, and perfect timing is required to jump over the hurdles at exactly the right time.

## Getting hold of the sprites
- Download this zip file to your home directory and unzip it's contents.

## Setting up the assets.
![ui](images/ui.gif)
1. Open Scratch by clicking on `Menu` > `Programming` > `Scratch`.
1. Now, click on the `background` icon and import the new background from the ScratchOlympicsAssets directory. You can then delete the old background.
1. Click on the icon to import a new sprite and then choose the `run-1` image. Then inport `run-2`, `run-3` and `run-4` as additional costumes. You can then delete the old cat sprite.

## Capturing the key mashing.
1. The first step is to capture the `x` and `z` keypresses, and use the speed at which the player is pushing the keys, to control the size of a variable
1. To do this you'll need a variable that stores the last known key press. Create a variable called `last_key` and set it to `z` when the green flag is clicked.
![script](images/greenflag1.svg)
