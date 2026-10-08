# minigame 2
## Devlog
## Devlog

### 1. An issue I encountered and how I fixed it

While editing `Spell.cs`, I missed a closing curly brace at the end of the script. This caused a compilation error because the class was not properly closed. I checked the braces for the `if` statement, the `Update()` method, and the `Spell` class, then added the missing brace.

After saving the script, I tested the game in Unity. Pressing Space activated the blue spell circle, which disappeared after approximately one second. Pressing Space again after it disappeared activated another spell.

### 2. My understanding of the color code

`_spriteRenderer.color = new Color(r, 0.2f, 0.2f);`

I think the dot in `_spriteRenderer.color` accesses the color property of the SpriteRenderer. The word `new` creates a new Color value using three numbers for the red, green, and blue channels. The variable `r` controls the red channel, while green and blue stay at `0.2f`. The equals sign assigns this color to the chest.

As the chest loses health, the code changes `r`, which changes the chest’s appearance. When its health reaches zero, the chest disappears.

## Open-Source Assets
- Pixel art environment & character sprites: https://assetstore.unity.com/packages/2d/environments/pixel-art-top-down-basic-187605
