# GoIT JavaScript Homework - Module 4 🚀

This document outlines the tasks for Module 4 of your GoIT JavaScript homework.

## Homework Assignment 4 📚

- Create a new GitHub repository named `goit-js-hw-04` and clone it to your computer. 📁
- In the `goit-js-hw-04` folder, create the project structure according to the schema below. 🏗️

```bash
goit-js-hw-04/
├── index.html
└── js/
    ├── task-1.js
    ├── task-2.js
    └── task-3.js
```

#### Attention :bangbang:

File and folder names, along with their nesting, must match the specified schema. Otherwise, the work will not be accepted. ❌

- Read each task and complete it in the relevant file. 📝
- Make sure your code is formatted with Prettier and that there are no errors or warnings in the console when you open the live page. ✨
- Submit your homework for review. ✅

**Submission Format:** The assignment must include two links: one to the source files and another to the live page on `GitHub Pages`. 🔗

## Task 1. Product Packaging

#### :bangbang: Complete this task in the `task-1.js` file. 📦

Write a function called isEnoughCapacity(products, containerSize) that calculates whether all the given products will fit into a container.
The function takes two parameters:

- `products` — An object containing product names as keys and their quantities as values. For example, `{ apples: 2, grapes: 4 }`.
- `containerSize` — The maximum number of products that can fit inside the container.

The function should return the result of the check: `true` if the total quantity of `products` in the products object is less than or equal to `containerSize`, and `false` otherwise.
Take the following code and paste it after defining your function to check its correctness. The results will be printed to the console.

```js
console.log(isEnoughCapacity({ apples: 2, grapes: 3, carrots: 1 }, 8)); // true
console.log(isEnoughCapacity({ apples: 4, grapes: 6, lime: 16 }, 12)); // false
console.log(isEnoughCapacity({ apples: 1, lime: 5, tomatos: 3 }, 14)); // true
console.log(isEnoughCapacity({ apples: 18, potatos: 5, oranges: 2 }, 7)); // false
```

Leave this code for your mentor to check. 🧑‍🏫

## Mentor's review criteria:

- A function named isEnoughCapacity(products, containerSize) is defined.
- The call isEnoughCapacity({ apples: 2, grapes: 3, carrots: 1 }, 8) returns true.
- The call isEnoughCapacity({ apples: 4, grapes: 6, lime: 16 }, 12) returns false.
- The call isEnoughCapacity({ apples: 1, lime: 5, tomatos: 3 }, 14) returns true.
- The call isEnoughCapacity({ apples: 18, potatos: 5, oranges: 2 }, 7) returns false.

---

## Task 2. Calorie Calculation

#### :bangbang: Complete this task in the `task-2.js` file. 📝

Write a function called `calcAverageCalories(days)` that returns the average daily calorie intake for an athlete over a week. The function expects a single parameter: `days` — an array of objects. Each object has a day property and a calories property, describing the `calories` consumed by the athlete on that day.
To check if the function is working correctly, paste the following code immediately after the function definition. The results will be printed to the console.

```js
console.log(
  calcAverageCalories([
    { day: 'monday', calories: 3010 },
    { day: 'tuesday', calories: 3200 },
    { day: 'wednesday', calories: 3120 },
    { day: 'thursday', calories: 2900 },
    { day: 'friday', calories: 3450 },
    { day: 'saturday', calories: 3280 },
    { day: 'sunday', calories: 3300 }
  ])
); // 3180
console.log(
  calcAverageCalories([
    { day: 'monday', calories: 2040 },
    { day: 'tuesday', calories: 2270 },
    { day: 'wednesday', calories: 2420 },
    { day: 'thursday', calories: 1900 },
    { day: 'friday', calories: 2370 },
    { day: 'saturday', calories: 2280 },
    { day: 'sunday', calories: 2610 }
  ])
); // 2270
console.log(calcAverageCalories([])); // 0
```

Leave this code for your mentor to check. 🧑‍🏫

## Mentor's review criteria:

- The `calcAverageCalories(days)` function is defined.
- This call of the `calcAverageCalories` function returns `3180`.

```js
calcAverageCalories([
  { day: 'monday', calories: 3010 },
  { day: 'tuesday', calories: 3200 },
  { day: 'wednesday', calories: 3120 },
  { day: 'thursday', calories: 2900 },
  { day: 'friday', calories: 3450 },
  { day: 'saturday', calories: 3280 },
  { day: 'sunday', calories: 3300 }
]);
```

- This call of the `calcAverageCalories` function returns `2270`.

```js
calcAverageCalories([
  { day: 'monday', calories: 2040 },
  { day: 'tuesday', calories: 2270 },
  { day: 'wednesday', calories: 2420 },
  { day: 'thursday', calories: 1900 },
  { day: 'friday', calories: 2370 },
  { day: 'saturday', calories: 2280 },
  { day: 'sunday', calories: 2610 }
]);
```

- This call of the `calcAverageCalories` function returns `0`.

```js
calcAverageCalories([]);
```

---

## Task 3. Player Profile

#### :bangbang: Complete this task in the `task-3.js` file. 🎮

The profile object belongs to a user's profile on a gaming platform. Its properties include a `profile` name `username` and active hours spent in the game, specified as `playTime`.

```js
const profile = {
  username: 'Jacob',
  playTime: 300
};
```

Complete the `profile` object with methods to work with its properties.

- The `changeUsername(newName)` method should take a string (the new name) as the `newName` parameter and change the value of the `username` property to the new value. It returns nothing.
- The `updatePlayTime(hours)` method should take a number (the number of hours) as the hours parameter and increase the value of the `playTime` property. It returns nothing.
- The `getInfo()` method should return a string in the format `<Username> has <amount> active hours!`, where `<Username>` is the profile name and `<amount>` is the number of hours played.

Paste the following code after defining your function so you can check if the functionality is working correctly. The results will be printed to the console.

```js
console.log(profile.getInfo()); // "Jacob has 300 active hours!"
profile.changeUsername('Marco');
console.log(profile.getInfo()); // "Marco has 300 active hours!"
profile.updatePlayTime(20);
console.log(profile.getInfo()); // "Marco has 320 active hours!"
```

Leave this code for your mentor to check. 🧑‍🏫

## Mentor's review criteria:

- A variable named `profile` is defined.
- The value of the `profile` variable is an object with the properties `username`, `playTime`, `getInfo`, `changeUsername`, and `updatePlayTime`.
- The value of the `getInfo` property is a function.
- The value of the `changeUsername` property is a function.
- The value of the `updatePlayTime` property is a function.
- `this` is used to access object properties within its methods.
