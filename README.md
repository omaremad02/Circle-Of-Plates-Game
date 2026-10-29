# Circle of Plates: a Java OOP & Design Patterns Game

A 2D arcade game in **Java (Swing)**. You control a clown who catches falling plates on both hands. Stacking **three plates of the same colour** clears them and scores points, while catching a **bomb** resets the score. Survive until the timer ends to win.

Built as a team project for the *Object-Oriented Programming* course, on top of the course's game engine (`eg.edu.alexu.csd.oop.game`).

## Gameplay
- Plates and bombs move along four conveyor belts and drop off the ends
- Move the clown left and right to catch them on the left or right hand stack
- Three matching plates on one stack disappear and add to your score
- Three difficulty levels change the game speed

## Design patterns used
The main point of the project was to apply OOP design patterns:

| Pattern | Where |
|---|---|
| **MVC** | `Model/`, `view/` and `Controller/` packages |
| **Singleton** | `Clown.getInstance()`: there is only one player character |
| **Factory** | `Factory.getshape()` creates plates or bombs by type |
| **Strategy** | `Strategy` interface with `easyStrategy` / `mediumStrategy` / `hardStrategy` controlling speed |
| **Iterator** | Custom `MyIterator` / `ArrayIterator` for walking game-object collections |
| **Prototype** | `Shape.clone()` / `PictureObject.clone()` duplicate falling objects |

## Run it
1. Open the project in NetBeans or IntelliJ.
2. Add the course game-engine `.jar` (`eg.edu.alexu.csd.oop.game`) to the project libraries.
3. Run `view/mainFram.java`, choose a difficulty and play.

## Tech
Java · Swing · OOP · design patterns (MVC, Singleton, Factory, Strategy, Iterator, Prototype)
