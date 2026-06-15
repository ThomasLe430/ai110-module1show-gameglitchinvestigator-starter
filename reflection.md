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

The AI tool that I used on this project was Claude. The fixes that I targeted include misleading hints, incorrect display of the remaining number of attempts, new game not working, and difficulty ranges being wrong. For each of these errors, I asked the Claude to first explain the logic in the code that might have caused the errors, then suggest changes to help improve the error. After the error was improved, I asked Claude to generate test cases to ensure that the game logic was working correctly (mainly for having the right hints and difficulty ranges). For example, to fix the hints being displayed incorrectly, Claude suggested to swap the message for higher and lower in order to match what the user actually needed to do. This suggestion made sense, and I verified it by asking it to make test cases to ensure the right hint message was returning. Honestly, I could not find any misleading suggestions in my usage of Claude. Although, one suggestion I did reject was Claude trying to add a test case to check if the easy and hard difficulty range was lower than the normal one, which I thought was unnecesary. Overall, I verified the results from Claude by asking it to generate test cases and playtesting the website to see if everything worked.

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

I decided whether a bug was fixed by asking the AI to create a test and playtesting the website. One test that I ran using pytest was to check the difficulty ranges of the game for easy, medium, and hard mode. The AI I used designed these tests - I had no input in creating them. However, I do think that the difficulty and hint test cases that the AI generated were relatively straightforward, but effective and easy to verify manually. Additionally, I playtested the website to make sure the changes were effective. My methodology for playtesting was simple, where I repeated the documented inputs listed above to see if the expected behavior matches the actual behavior. 
---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
