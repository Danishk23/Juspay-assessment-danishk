# Project

This is basically a clone of the Scratch site by MIT. It is a platform where you can create your own custom games and animations.

---

## How it works?

- The interface consists of many components rendered in the sidebar based on different key-value pairs.
- There is a function called `fetchComponents` that takes a particular key and returns a component along with some default values. These components are then rendered in the sidebar.
- The sidebar is made up of different draggable components, and you can freely drag any of these components into another draggable area called the **mid area**.

- The **mid area** is a draggable zone where different components from the sidebar can be placed.
- The mid area maintains a Redux state that updates when you drag content out or reorder content already present.
- It stores the keys of all elements in the mid area, which are used later on.
- When clicking on a particular button inside any component, a function is triggered based on the component’s type, handled by a switch-case statement responsible for running different functions with various values.

- There is also a **Run All** button responsible for executing all functions present inside the mid area. This is done by taking an array of keys and performing actions sequentially.
- Functions are run with certain delays, and a **history** is maintained using Redux state.
- The history stores all values currently present in the mid area and is used to render the History component.
- Mapping is done based on the key of the element pushed into the Redux state with default values, used to render the history elements.

---

## How to run the project?

1. Clone the project.
2. Run `npm install`.
3. Run `npm start`.
4. Open `http://localhost:8080` in your browser.
5. Enjoy!

---

## Tech stack used

- React
- Redux
- React DnD (outdated but used for this project)
- React Redux Toolkit
- Tailwind CSS
