# Algorithm

## Definition

**=>** An Algorithm is any well-defined computational procedure that takes some value or set of values as Input and produces a set of values or some value as output.

In other words, or in a more formal manner, we can define an Algorithm as:

**=>** An Algorithm is a finite set of instructions that, if followed, accomplishes a particular task. In addition, all algorithms should satisfy the following criteria:
- **INPUT** : Zero or more quantities are externally supplied.
- **OUTPUT** : At least one quantity is produced.
- **DEFINITENESS** : Each instruction is clear and unambiguous.
- **FINITENESS** : If we trace out the instructions of an algorithm, then for all cases, the algorithm terminates after a finite number of steps.
- **EFFECTIVENESS** : Every instruction must very basic so that it can be carried out, in principle, by a person using only pencil & paper.

## Representation

An algorithm can be described in *three* ways:
- Natural language
- Flowchart
- Pseudo-Code

## Complexities

Complexity of an algorithm is basically an indicator value that shows how efficient the algorithm is. It is typically measured in terms of *time* and *space*.

### Space Complexity

This tells us the amount of memory the algorithm needs for it to function properly. The space required by an algorithm can be of two types:
- A *predetermined amount* of space the algorithm will need every time it is used, regardless of how much input it takes,
- A *Variable amount* of space that depends on how much input the algorithm works with.

So to standardize Space Complexity into one statement, we can say:
$$S(P) = C + S(I)$$
where:
- $S(P)$ -> Space complexity of the algorithm
- C -> Constant space taken
- $S(I)$ -> Variable space taken, depending on instance $I$  of the input.

**Example 1:**
Sum of two numbers: `SUM(A, B)`

```
1  Start
2
3  C <- A + B
4
5  STOP
```

Here, as the input itself is constant, there is no variable space in this algorithm. Thus:
- `C` takes *4 bytes*
- Input takes *4 + 4 = 8 bytes*
And it is constant every time we run this algorithm.

Thus Space complexity becomes:
$$
S(P) = S(12) = 1
$$
As this space complexity is constant, we can also denote the upper bound (Big-O) with it as $O(1)$.

**Example 2:**
Sum of `n` numbers: `SUM(A[], n)`

```
1  Start
2
3  SUM <- 0
4  FOR i = 1 to n
5    SUM <- SUM + A[i]
6  END FOR
7
8  STOP
```

Here:
- `SUM` takes *4 bytes*
- `i` takes *4 bytes*
- `n` takes *4 bytes*
- `A[]` takes *n bytes*

Therefore:
- $C = S(12) = 1$
- $S(I) = n$
$$
S(P) = 1 + n \approx n
$$
As 1 is significantly smaller than n, we ignore it in complexities.
We can denote its upper bound as $O(n)$

### Time Complexity

Just like how space complexity tells us how much space an algorithm needs, Time Complexity tells us how much time it will need to produce the required output. It is also represented as numerical functions, where it is assumed that each step will take a constant amount of time.

**Example:**
Return TRUE if a number `x` exists in an array `A[n]`: `isPresent(A[], n, x)`

```
1  Start
2
3  FOR i = 1 to n
4    IF A[i] equal to x
5      RETURN TRUE
6
7  RETURN FALSE
8
9  STOP
```

So the upper bound of the algorithm is, when `x` is not present in the input array.

Thus the steps in this algorithm are:
- Declaration of `i`
- Loop (`n` times):
	- Comparing `i` to `n`
	- `IF` Statement
	- `RETURN` Statement, but in worst case it won't get executed
- `RETURN` statement

So time taken in units is $1 + n * (1) + 1 \approx n$

Therefore we can write it as $O(n)$ (upper bound).

## Asymptotic Analysis

It refers to the analysis of an algorithm's performance using mathematical calculations. Using Asymptotic analysis we can get definite answers for its best, average and worst case performances.

Asymptotic analysis depends on the input of the algorithm. If there is no input, it is assumed that the algorithm's complexities are constant.

Now the cases in which an algorithm's performance falls under are **Best Case**, **Average Case** and **Worst Case**, and are denoted by the following notations:

| Case    | Notation |
| ------- | -------- |
| Best    | $\Theta$ |
| Average | $\Omega$ |
| Worst   | O        |

### Big Oh Notation: O

Used to express the *upper bound* of an algorithm. In other words, it expresses the longest amount of time the algorithm can possibly take.

It is expressed as:
$$
f(n) \leq c \times g(n)
$$
where:
- $n$ is input size
- $f(n)$ is actual time complexity of the algorithm
- $g(n)$ is a known complexity, with which we are comparing $f(n)$
- $c$ is a constant
- $n > n_0$, where $n_0$ is a certain amount of input (threshold)

So basically the $n$ we take is the upper bound complexity, which is always greater than $f(n)$.

**Example:**
Consider the function $f(n) = 3n^2 + 2n + 1$

Let's take:
- $g(n) = n^2$
- $c = 4$

Therefore we get:
$$

$$

### Big Omega Notation: $\Omega$

Used to express the *lower bound* of an algorithm. In other words, it expresses the least amount of time the algorithm can possibly take.

It is expressed as:
$$
c \times g(n) \leq f(n)
$$
where:
- $n$ is input size
- $f(n)$ is actual time complexity of the algorithm
- $g(n)$ is a known complexity, with which we are comparing $f(n)$
- $c$ is a constant
- $n > n_0$, where $n_0$ is a certain amount of input (threshold)

So basically the $n$ we take is the lower bound complexity, which is always less than $f(n)$.

**Example:**

### Big Theta Notation: $\Theta$

It is a way to express kind-of the middle bound, or the average of the runtime of an algorithm.

It is expressed as:
$$
c_1 \times g(n_1) \leq f(n) \leq c_2 \times g(n_2)
$$

where:
- $n$ is input size
- $f(n)$ is actual time complexity of the algorithm
- $g(n_1)$ and $g(n_2)$ are known complexities, with which we are comparing $f(n)$
- $c_1$ and $c_2$ are constants
- $n > n_0$, where $n_0$ is a certain amount of input (threshold)

