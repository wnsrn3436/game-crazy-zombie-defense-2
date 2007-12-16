# Crazy Zombie Defense 2

The sequel to [Crazy Zombie Defense](https://github.com/wnsrn3436/game-crazy-zombie-defense). It adds an item system: pick up the sword lying on the field or earn the gun by killing zombies, and the weapon tags along behind the character.

<p>
  <img src="docs/screenshots/screenshot-1.png" width="316" alt="Gameplay">
</p>


## How to play

Download from Releases and run it.

Move with the arrow keys. Pick up the sword from the field and it follows you, swinging with space. After 10 zombie kills a gun appears, fired with the left mouse button. Keys 1 and 2 bring the sword and gun out or put them away. The zombie kill count is shown in the window title bar.


## How it works

The weapon follows by stepping toward the player's coordinates at speed 5 every step. There is no parent child relationship, just one move toward point action in the Step event. That is why the weapon does not sit glued to the character but trails slightly behind.

The zombie kill count reuses the `health` value that counted buildings in Crazy Zombie Defense. Every zombie killed raises it, and it is printed in the title bar under the label "좀비죽인업적".


## Files

| Path | Contents |
|---|---|
| `source/crazy-zombie-defense-2.gmk` | Original project file |
| `source/split/` | Text tree produced by GmkSplitter |
| `docs/screenshots/` | Screenshots |
| Releases | Distributed build |


## License

CC BY-NC-ND 4.0. Unmodified copies may be shared for noncommercial purposes with attribution. Modified versions and commercial use are not allowed. Bundled libraries, graphics, sounds, and maps made by other people keep their own rights. See [LICENSE](LICENSE).
