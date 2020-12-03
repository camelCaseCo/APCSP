# Unit 4 Project
Click [here](/README.md) to go back to the main APCSP repo.

## Downloads
Windows and Linux users on 64-bit or 32-bit machines can find pre-compiled binaries in [`./bin/README.md`](./bin/). Installation instructions are avaliable for both Windows and Linux users. Windows users also have the option of using an installer. Any users running macOS, or using a different instruction set such as ARM, must compile the application from source.

Users wishing to compile the application themselves will find the C# source code as well as compilation instructions in [`./src/README.md`](./src/).

[What are binaries? What is source code? What does it mean to compile?](/README.md#types-of-downloads)

## About the Project
The Unit 4 project is a simple game in which the user attempts to pick up trash on the road by pressing either `a`, `s`, `d`, or `f` depending on which channel the trash is in. The UI is text-based. Upon opening the application, the user is greeted by a CLI interface which provides them with various options such as starting a new round of the game, viewing the stored game data or resetting the game data.

Game data is stored as UTF-8 text in a file named `gamedata` which is located in the same directory as the application. If the `gamedata` file does not exist, the application will generate a new one. Users should take care to never change the information within the `gamedata` file as it may cause runtime errors. Resetting the game data should _only_ be done in the following ways:

- The built-in command provided by the CLI interface
- Deleting the `gamedata` file

If the application is moved, it will create a new `gamedata` file in its new location. To avoid this, make sure to move the application and the `gamedata` file as one.

If a user wishes to resize the window, they should do so while the CLI interface is open. Never change the size of the window in the middle of a round, as it will distort the graphics heavily.
