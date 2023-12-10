# Typescript Labs

## Lab 8: Function Return Type Annotations

file : `/src/08-function-return-type-annotations.problem.ts`

Continuing from last time, we have a User that includes an array of posts.

This time instead of having a defaultUser, we instead have a makeUser function that should return a user.

const makeUser = () => {
  return {};
};

At this current starting point, the function is returning an empty object.

Because our test code is expecting a User, TypeScript is showing us errors.

Experiment with makeUser's return
Add some keys and values to the object returned from makeUser. When you hover over the call to makeUser() in the test, you'll see a popup that shows what would be returned from the function:

it("Should return a valid user", () => {
  // Hover over here:
  const user = makeUser();

You don't have to specify what a function returns.

Challenge
Similar to a previous challenge, we want TypeScript to show us error messages on the lines where they happen instead of in a test.

Your challenge is to annotate the makeUser function to make sure it always returns a User.