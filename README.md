# Solitaire, but Better

This is a Lua-based implementation of Klondike Solitaire using the LÖVE2D framework. The goal was to create a functional solitaire game while practicing software design patterns—especially the Flyweight pattern—to manage reusable components like cards and piles.

## Features

- Drag-and-drop card functionality
- Stock (draw pile) and waste pile with three-card draw rule
- Foundation piles for suit sorting
- Undo button to reverse moves
- Ability to draw from the sorted waste pile
- Test win button for debugging or impatient players
- Enlarged cards for improved visibility
- Win screen (basic)

---

## Design & Patterns

I primarily used the **Flyweight Pattern** to handle card and pile objects. This helped structure the code and reduced redundancy by treating similar game objects in a uniform way.

I also focused on keeping the code **organized**, with consistent naming conventions, indentation, and comments throughout the project.

---

## Playtesting & Feedback

### Peer Feedback – *Samuel Webster*

Samuel helped identify issues I had overlooked—such as the undo button not reversing stock pile draws. His feedback helped refine some edge case behaviors and improve overall polish.

### Family & Friends

Although no other programmers reviewed the code, I had several playtesters (my mom, sister, and some friends) who enjoy Solitaire. Their feedback led to:
- Larger card visuals for better readability
- Allowing cards to be moved from the sorted waste pile
- Adding a test win button to help verify win conditions

> "This game is impossible."  
> — *My Sister*

This quote inspired the test win button because, truth be told, I never managed to beat my own game either. I suspect the issue lies in how the cards are randomized, but time constraints prevented me from fixing this. Maybe in **Project 3: Solitaire But *Even Better***?

---

## Known Issues

- The draw pile occasionally reveals **four cards instead of three**.
    - This seems to stem from how the pile logic updates and displays new cards. It's likely a sequencing issue between logic and visual state updates.
    - While difficult to reproduce consistently, it remains an unresolved visual glitch.

- The win screen is functional but **not animated**. I had hoped to do something fancier but ran out of time.

---

## Postmortem

This project gave me a new appreciation for the complexity of seemingly "simple" card games. Between logic, UX, and edge case handling, there's a lot that goes into replicating the feel of Solitaire.

I’m proud of how far I got especially considering this is one of the first full projects I’ve done in Lua while learning about patterns and game workflows.

---

## Assets

- **Cards:** [Kenney's Playing Cards Pack](https://kenney.nl/assets/playing-cards-pack)  
  Used the **Large** card versions from the pack.

---

## Future Improvements

- Fix the card draw glitch
- Improve the win screen with animations
- Better shuffle/randomization logic
- More polish on UI transitions and undo logic

---

## Requirements

- [LÖVE2D](https://love2d.org/) engine installed to run the game

---
## Additional Credits
- Chatgpt really helped out in formating this readme.md file I basically explained the contents of my project pdf and I had chatgpt help me with all the nice titles and other things like quotes bullet point formats and so on. This is the first time I really used the readme file like this because I never had the chance to learn how to use it so I thought it was worth a shot to see how it turns out.
