# Genetic Algorithm

![for huahua](https://img.shields.io/badge/%F0%9F%8E%88for%20Huahua-2021-brightgreen?&logo=Ghostery)

### Algorithm Description

From [Chapter 9.](https://natureofcode.com/book/chapter-9-the-evolution-of-code/) of the book THE NATURE OF CODE by Daniel Shiffman

#### setup()

- Step 1: **Initialize** the Population

  - Create an empty population (an array or ArrayList)

  - Fill it with DNA encoded objects (pick random values to start)

#### draw()

- Step 2: **Selection**

  - Create an empty mating pool (an empty ArrayList)

  - For every member of the population

    - evaluate its fitness based on some criteria / function

    - add it to the mating pool in a manner consistent with its fitness

      (i.e. the more fit it is the more times it appears in the mating pool, in order to be more likely picked for reproduction)

- Step 3: **Reproduction**

  - Create a new empty population Fill the new population by executing the following steps:

    ​ a. Pick two "parent" objects from the mating pool.

    ​ b. Crossover -- create a "child" object by mating these two parents.

    ​ c. Mutation -- mutate the child's DNA based on a given probability.

    ​ d. Add the child object to the new population.

- Step 4:
  - Replace the old population with the new population and return to Step 2
