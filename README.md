# Todo App

Welcome to this basic todo application. Some of the features it has are:

- Filtering
- Sorting
- Keyword Search
- Updating todo status
- Editing the name, description and due date
- Re-organizing the todos based on the priority you want

## Setup

To get the application up and running, run

```bash
npm install # Install project dependencies
npm run dev # Runs the application (on port 5173 by default)
```

## Testing the application

Although I wasn't able to run the tests (read the "Nice to haves" section for more details), they have been setup and configured. To run them, use the command:

```bash
npm run test # Uses Vitest to run tests
```

## Nice to haves:

There are few more features that can be added to this application and some extra procedures that we can follow to improve it. Some of those are:

- If a user has set a todo to "Completed" by mistake, we should be able to set it back to "In-progress".
- If a todo is in a completed state, we can add an option to remove it automatically after a specified time since it's due date.
- At this time, we are only able to sort the dates, there is no way to search for a specific date or range of dates. That might help a user narrow down a todo they are looking for.
- Unfortunately, I was having difficulties running tests for this project. My first choice was creating interaction tests through Storybook. It has been my favourite way of testing UI components. Then I tried running React Testing Library on it's own. In both cases, it caused the testing runner to hang. I have attempted to write a couple of test cases which I think would be relevant. These could be considered temporary red to green tests.
- The application has no database to store the todos. For now, they refresh every time the page is reloaded. A database, or based on complexity a simple local JSON file should suffice.
- Definitely the beauty, although the application doesn't look horrible, it still definitely needs a visual upgrade.
- Filtering the date is a little finicky, for example, we need to type "Wed" for "Wednesday". Typing out the full form doesn't work. Need to find a better way to share the date related data more efficiently and consistently across all the components.
- Hovering over the due date with a tool tip mentioning the minutes, hours, days left would be helpful.
- Render errors live instead of only rendering when the "Submit" button is pressed and more in-depth error handling.
