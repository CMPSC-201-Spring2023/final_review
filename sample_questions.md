# CMPSC 201 Final Exam Study Questions

Here are questions to help you prepare for the exam. These questions do not represent the exact type of questions to be on the exam, instead they should be used as a refresher guide into the topics covered on the exam.

1. Explain the concept of 'hole in scope' with your own Javascript example.

2. What is the output of the following C program? Explain.

  ```
  #include <stdio.h>
  int main() {
  int i = 10;
    if (i > 5) goto THERE;
  HERE:
    printf("Now I'm here\n");
    goto FINISH;
  THERE:
    printf("Now I'm there\n");
    goto HERE;
  FINISH:
    printf("I'm done!\n");
  }
  ```

3. If you have tried to track down precise definitions of the terms "strongly typed" and "weakly typed" you have probably come away frustrated. Textbooks typically define a "strongly typed language" as one that "prohibits ... the application of any operation to any object that is not intended to support that operation." Give an example of such an operation and such an object, using only standard primitive types.

4. Choose one of the following three languages (C, Haskell, Python) and mention two composite data types (as defined in our textbook) that are built into the language you chose.

5. The following statements are entered into the Haskell interactive environment:

  ```
  Prelude> let creature black lagoon = head black ++ (tail lagoon)
  Prelude> let black = [[1,2,3],[4,5,6]]
  Prelude> let lagoon = [7,8,9]
  Prelude> creature black lagoon
  ```

  What is printed?

  (See <https://en.wikipedia.org/wiki/Creature_from_the_Black_Lagoon>) Answer: Since head[black] = [1,2,3] and tail lagoon = [8,9], it will print [1,2,3,8,9].

6. What is polymorphism? How is it supported by Java?

7. Java supports multiple inheritance.

  Put "X" inside brackets [ ] of the correct answer.

  - [ ] True
  - [ ] False

8. Explain short-circuit evaluation with a simple example involving the logical "or" operator `||`.

9. Define "orthogonality" in a programming language.

10. What are the two principle purposes of "types" in a language?

11. What does a language-based security entail? Describe what it is, provide at least one problem that may arise in a language-based security and how it can be solved.
