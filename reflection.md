# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").

  What happened when I ran the game was that whenever I tried to guess the correct number, the hints were always opposite (lower when it should actually be higher and vice versa). I also noticed that I was not able to hit enter and start a new game once one was finished. I was also confused why it displayed game over when I had one attempt remaining. 
**Bug Reproduction Log**

Document at least 3 bugs you found. Add rows as needed.

| Input | Expected Behavior | Actual Behavior | Console Output / Error |
|-------|-------------------|-----------------|------------------------|
| 50    | Hint: Go Lower    |  Hint: Go Higher| None, target was 78.   |
| 1.    | Attempts left: 6. | Attempt left: 7 | None, first guess didnt go down|
|New Game| Start New Game.  | Nothing happens | None, cant submit guess when new game is pressed|
|Re-show Hint| Display Hint    | Nothing happens | None, can't get hint to re-appear |
|Easy Difficulty| Number from 1-20 | Number out of range | None |
|Correct guess after 6 guesses (normal diff)| Positive score | Score -10 | None | 



---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
