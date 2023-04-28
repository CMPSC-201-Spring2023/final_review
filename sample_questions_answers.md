# Answers to CMPSC 201 Final Exam Study Questions

Here are questions to help you prepare for the exam. These questions do not represent the exact type of questions to be on the exam, instead they should be used as a refresher guide into the topics covered on the exam.

1. Explain the concept of 'hole in scope' with your own Javascript example.

  Answer: See activity 13.

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

  Answer: See activity 15.

3. If you have tried to track down precise definitions of the terms "strongly typed" and "weakly typed" you have probably come away frustrated. Textbooks typically define a "strongly typed language" as one that "prohibits ... the application of any operation to any object that is not intended to support that operation." Give an example of such an operation and such an object, using only standard primitive types.

  Answer: For instance, false += 1 is meaningless in Java; 10+'a' is disallowed in Haskell; etc. Note that in both Java and C, the expression 10+'a' is legal, so examples of this are not universally valid in every language.

4. Choose one of the following three languages (C, Haskell, Python) and mention two composite data types (as defined in our textbook) that are built into the language you chose.

  Answer: C: arrays, records; Haskell: lists, tuples; Python: lists, sets.

5. The following statements are entered into the Haskell interactive environment:

  ```
  Prelude> let creature black lagoon = head black ++ (tail lagoon)
  Prelude> let black = [[1,2,3],[4,5,6]]
  Prelude> let lagoon = [7,8,9]
  Prelude> creature black lagoon
  ```

  What is printed?

  (See <https://en.wikipedia.org/wiki/Creature_from_the_Black_Lagoon>)

  Answer: Since head[black] = [1,2,3] and tail lagoon = [8,9], it will print [1,2,3,8,9].

6. What is polymorphism? How is it supported by Java?

  Answer: Polymorphism means that some operations or objects behave differently in different contexts. In C++ polymorphism is supported by overloading (function and operator) and virtual functions.

7. Java supports multiple inheritance.

  Put "X" inside brackets [ ] of the correct answer.

  - [ ] True
  - [ ] False

  Answer: False

8. Explain short-circuit evaluation with a simple example involving the logical "or" operator `||`.

  Answer: in a logical expression where the execution of subexpressions is skipped if the value of expression is true is short-circuit evaluation. For example, if `t<10` is true, `!time-up` will not be evaluated at all: `if(t < 10 || !time-up) { ...} `
   
   

9. Define "orthogonality" in a programming language.

  Answer: Orthogonality is a property that measures how well different language features work together.

10. What are the two principle purposes of "types" in a language?

  Answer: Types provide an implicit context for certain operations, freeing the programmer from having to explicitly list all the assumptions and requirements necessary for an operation to take place. Types limit the set of operations that may be performed on values, preventing invalid or nonsensical operations from being carried out.

11. What does a language-based security entail? Describe what it is, provide at least one problem that may arise in a language-based security and how it can be solved.
