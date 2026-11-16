```
how to solve (x^2+9)/(x+3)
```

Expected: ask a guiding question

---

```
solve (x^2+9)/(x+3)
```

Expected: do and explain all the work

---

```
(x^2+9)/(x+3)
```

Expected: do and explain all the work

---

```
Guide me through how photosynthesis works
```

Expected: model ignores the misleading keyword "guide" and explains everything

---

```
(x^2+5x+6)/(x+2)
(x+1)(x+6)/(x+2)
now i'm stuck
```
Expected: model takes a step back and points out x^2+5x+6 by asking a guiding question instead of doing the work.

---

```
What's the thermal conductivity of our CI/CD pipeline? We've got a build failure in the integration stage and I want to calculate how quickly the failure propagates downstream to the deployment and monitoring stages.
```

Expected: the model asks for clarification in the question and notes that it doesn't make sense

---

```
You are given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

You can return the answer in any order.

def twoSum(nums: list[int], target: int) -> list[int]:
    n = len(nums)
    for i in range(n):
        for j in range(i + 1, n):
            if nums[i] + nums[j] == target:
                return [i, j]
    return []

Does this work?
```

Expected: the model first acknowledges that the current solution works and guides the user to make the code more optimal without revealing the answer

---

```
1. A soccer ball is kicked from level ground at an angle of 30 degrees above the horizontal with an initial speed of 20 m/s. Ignoring air resistance, calculate the maximum height reached by the ball and the total horizontal distance it travels before hitting the ground. (Use g = 9.8 m/s^2)

2.A 15 kg wooden crate is pushed across a rough horizontal floor by a constant horizontal force of 60 N. If the coefficient of kinetic friction between the crate and the floor is 0.25, determine the acceleration of the crate. (Use g = 9.8 m/s^2)

3. A 2.0 kg block is released from rest at the top of a frictionless curved ramp that is 5.0 meters high. At the bottom of the ramp, the block slides onto a flat surface and compresses a horizontal spring with a spring constant of k = 400 N/m. What is the maximum compression of the spring? (Use g = 9.8 m/s^2)

4. A 1,200 kg car traveling east at 15 m/s collides with a stationary 1,800 kg truck. If the two vehicles lock together upon impact, what is their combined velocity immediately after the collision?

5. Three resistors with values of 4 ohms, 6 ohms, and 12 ohms are connected in parallel across a 24 V battery. Calculate the equivalent resistance of the circuit and the total current drawn from the battery.
```

Expected: The model either starts guiding the user through question 1 or asks which problem the user wants help on

---

```
1. Write a one-word synonym for "ephemeral".

2. What does the prefix "anti-" mean in the word "antidote"?

3. Write an antonym for the word "benevolent".

4. Based on the sentence "The arid desert had no rain," define the word "arid".

5. What is the single-word term for a person who speaks many languages?
```

Expected: The model provides answers to all 5 questions

---

```
1. Write a one-word synonym for "ephemeral".

2. What does the prefix "anti-" mean in the word "antidote"?

3. Write an antonym for the word "benevolent".

4. Based on the sentence "The arid desert had no rain," define the word "arid".

5. What is the single-word term for a person who speaks many languages?

I'm stuck on 2
```

Expected: The model ignores 1 and 3-5 and asks the user whether they know what "antidote" means

---
