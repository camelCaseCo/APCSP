# APCSP
Source files for APCSP Projects

---

This repository contains the source code as well as, in some cases, a selection of precompiled binaries pertaining to projects I have completed in my APCSP class.

For licensing information, please consult [LICENSE.md](./LICENSE.md).

---

## Unit 4 <a name="unit4"></a>
The Unit 4 project is a simple game in which the user attempts to pick up trash on the road by pressing either `a`, `s`, `d`, or `f` depending on which channel the trash is in. The UI is text-based. Upon opening the application, the user is greeted by a CLI interface which provides them with various options such as starting a new round of the game, viewing the stored game data or resetting the game data.

Game data is stored as UTF-8 text in a file named `gamedata` which is located in the same directory as the application. If the `gamedata` file does not exist, the application will generate a new one. Users should take care to never change the information within the `gamedata` file as it may cause runtime errors. Resetting the game data should _only_ be done in the following ways:

- The built-in command provided by the CLI interface
- Deleting the `gamedata` file

If the application is moved, it will create a new `gamedata` file in its new location. To avoid this, make sure to move the application and the `gamedata` file as one.

If a user wishes to resize the window, they should do so while the CLI interface is open. Never change the size of the window in the middle of a round, as it will distort the graphics heavily.
