---
title: Setting up a new project
slug: new-spritekit-project
---

# Create a new SpriteKit project

> [action]
> Create a new *Game* project in Xcode named `Gameoflife` and check the *Language* is set to `Swift` and 
> *Game Technology* is set to `SpriteKit`.
>
> ![Xcode new project](../Tutorial-Images/xcode_new_project.png)

## Importing Resources

> [action]
> Download the [Game of Life Art Pack](https://github.com/MakeSchool-Tutorials/Game-Of-Life-SpriteKit-Swift3/raw/master/assets.zip) we created for you.
> Once the download is complete, unpack the folder.
> Click on the *Assets.xcassets* folder and drag across the assets.
>
> ![Xcode add assets](../Tutorial-Images/xcode_add_assets.png)

These assets were designed with the 4" retina resolution.

## Adding extra functionality

SpriteKit doesn't include a button class you will have to add your own!

> [action]
> Download the [MakeSchool Utilities](https://github.com/MakeSchool-Tutorials/Game-Of-Life-SpriteKit-Swift3/raw/master/Utils.zip), unpack and drag the file 'MSButtonNode.swift' into the project (we don't need the rest).
> Ensure *Copy items if needed* is checked.
>
> ![Xcode add utils](../Tutorial-Images/xcode_add_utils.png)

# Device orientation

The game assets were designed for landscape orientation, so you should ensure that the game will not accidentally 
use portrait.

> [action]
> Open the target settings.
>
> Uncheck any **Portrait** options and check the **Landscape** options.
>
> ![Xcode Target Settings](../Tutorial-Images/xcode_target_settings.png)
>

# Clean project

To ensure a clean starting point, ensure your *GameScene.swift* reads as follows:

```
import SpriteKit

class GameScene: SKScene {

    override func didMove(to view: SKView) {
        /* Setup your scene here */
    }

    override func touchesBegan(_ touches: Set<UITouch>, with event: UIEvent?) {
        /* Called when a touch begins */
    }

    override func update(_ currentTime: TimeInterval) {
        /* Called before each frame is rendered */
    }
}
```

# Summary

Great, now you have a new project ready to begin building the Game of Life.  In the next chapter you will focus on 
creating the user interface.
