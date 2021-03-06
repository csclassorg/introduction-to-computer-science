# Lesson 2.4: Variables

## Learning Objectives

Students will be able to...

- Use variables to track values throughout a program

## Materials/Preparation

- [Do Now 2.4: Debugging](do_now_24.md)
- Lab 2.4 handout - [Guessing Game](lab_24.md) ([Download in Word](https://github.com/TEALSK12/introduction-to-computer-science/raw/master/Unit%202%20Word/Lab%202.4%20Guessing%20Game.docx)) ([Link to PDF](https://github.com/TEALSK12/introduction-to-computer-science/raw/master/Unit%202%20PDF/Lab%202.4%20Guessing%20Game.pdf))
- ["The Box Variable Activity"](https://teachinglondoncomputing.org/resources/inspiring-unplugged-classroom-activities/the-box-variable-activity/) materials (Optional)
- [Unit 2 Tips](unit_2_tips.md)
- Video Resource - [https://youtu.be/YMVo9Wdpv5s](https://youtu.be/YMVo9Wdpv5s)
- Video Quiz - See Additional Curriculum Materials accessed from the TEALS Dashboard.

## Pacing Guide

| Duration   | Description                                   |
| ---------- | --------------------------------------------- |
| 5 minutes  | Welcome, attendance, bell work, announcements |
| 15 minutes | Lecture and introduce activity                |
| 25 minutes | Activity - Guessing Game                      |
| 10 minutes | Debrief and wrap-up                           |

## Instructor's Notes

### Do Now Review

- Review the debugging exercise with the students.
- Did they find the bugs in the program? (There are at least five.)
  1. In order to control Alonzo's movement with the arrow keys, the if statements need to be in a forever loop; otherwise, the code block will run once and complete. Alonzo never moves!
  2. Likewise, the code blocks checking for the W-A-S-D keys to move the Blue Dog need to be in a loop or they will also only check for a key press one time and complete. The Blue Dog never moves, either.
  3. In Alonzo's code, the conditional checking for the left arrow key is inside of the conditional checking for the right arrow key, so Alonzo can never move to the left.
  4. The _if on edge, bounce_ block in Alonzo's code is inside of the conditional checking for the left arrow key, so Alonzo will run off every edge of the screen, except the left.
  5. The fifth bug is more subtle. After the bugs preventing the movement of Alonzo and the Blue Dog have been fixed, the Blue Dog says __I got you!__ when touched by Alonzo. Since the Blue Dog is supposed to be running away from Alonzo, it doesn't make sense for the Blue Dog to say that when caught.
  6. The sixth bug is just good coding style. The Blue Dog has an unused _say_ block in the scripting area that should be deleted.
- Did the students have any suggestions about ways to improve the game? Here are some possible improvements they might have thought of:
  - Have a score counter that increments when the _reset_ message is sent. (After Alonzo catches the Blue Dog.)
  - Since Alonzo starts on the left of the screen and the Blue Dog starts on the right, have Alonzo be controlled by the W-A-S-D keys and the Blue Dog by the arrow keys. That way, the control keys are on the same side of the keyboard as the sprites they are controlling.
  - Have the computer control the Blue Dog using random movements.
  - Have the computer control the Blue Dog by always moving in the opposite direction from Alonzo.
  - Have the players choose which sprite is being chased at the beginning of the game.

### 1.  Lecture

1. Review user input, specifically the ![Answer Block](answer.png) block

    - Ask students to speculate about how the ![Answer Block](answer.png) block works
    - Students should recognize that the block must be storing a value somehow and remembering it for later
    - Ask students whether that type of functionality might be useful in other cases

2. Introduce variables

    - Define and explain the concept of a **variable:** _a location in memory to store a value for retrieval and use later_
    - Consider introducing variables with an interactive physical demonstration by modifying the [The Box Variable Activity](https://teachinglondoncomputing.org/resources/inspiring-unplugged-classroom-activities/the-box-variable-activity/) for your students.
    - Demonstrate creating, assigning, and accessing a variable in SNAP
      **Ignore global vs. this sprite only for now**
    - Point out that a variable can only hold one value at a time
    - When a new value is assigned, the old value is lost and cannot be recovered
    - Emphasize the importance of descriptive, readable names for variables
    - Show that variables are independent
    - One variable's value can be assigned to another, as in ![Set Var1 to var2 Block](setVar1ToVar2.png), but changing the value of `var2` later will not update the value of `var1`

### 2.  Activity

- Briefly demonstrate the ![Pick Random 1 to 10 block](random.png) block, which will be used in the lab
- Direct students to complete [Guessing Game](lab_24.md) individually or in pairs

### 3.  Debrief

- Discuss and demonstrate one or more students' submissions
- Ask students for commentary on usage and naming of variables throughout program

## Accommodation/Differentiation

- Advanced students can be encouraged to implement statistics (best score, average guesses/game, number of time each secret number chosen, etc.)
- Struggling students can be given code that completes part 1.1, and possibly also part 1.2, to get them started
- Students who are particularly overwhelmed should focus only on parts 1.2 and 2.2

## Forum discussion

[Lesson 2.4 Variables](http://forums.tealsk12.org/c/intro-unit-2-loops/lesson-2-4-variables) (TEALS Discourse account required).
