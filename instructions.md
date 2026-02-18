# Instructions

## Rotation 1 - Try agent mode
- Pick a dataset (recipes or books).
- Delete the one you’re not using
- Task: Show all items as cards in the DOM
- Hint: Open up the Copilot chat and choose Agent mode. Prompt it: "Show all items as cards in the DOM”
- Commit & push.

## Rotation 2 - Try Ghost Text
- Pull the changes.
- Put your cursor inside the sortItems function and hit - space/tab to start seeing suggestions.
- Accept the suggestions and check that it works. What did it sort on?
  - 📚 Change the name of the function to something else than it sorted on initially, e.g. sortOnYear, sortOnRating or sortAlphabetically. Remove the old code from within the function and see what suggestions it does. Try it out in the browser, did it work?
  - 🌶️ Change the name of the function to something else than it sorted on initially, e.g. sortOnTotalTime, sortOnIngredientCount or sortAlphabetically. Remove the old code from within the function and see what suggestions it does. Try it out in the browser, did it work?
- Commit & push

## Rotation 3 - Try inline chat (Ctrl + I)
- Pull the changes.
- Prompt it ”Make the reset button work”. Try it out by clicking the sort button and then the reset button (to remove the sorting)
- Prompt it:
  - 📚 Create functionality to filter out all books with a rating below 4.5
  - 🌶️ Create functionality to filter out all recipes with a total time over an hour
- Commit & push

## Optional features to try out
Choose one or more features to implement. These are just suggestions so feel free to come up with your own features.

Remember the flow:
- Pull the latest changes
- Implement the feature using Copilot
- Test it in the browser
- Commit & push

### 🏷 Highlight “Top picks”

Visually highlight certain items.

- 📚 **Books:** `rating >= 4.5`
- 🌶️ **Recipes:** `totalTime <= 45`

Add a badge (e.g. “Top pick”) or special styling.

**Copilot prompt idea:**
> Add a badge or special styling to items that match a condition (rating >= 4.5 / totalTime <= 45).

---

## 🔢 Show a count summary

Display how many items are currently shown.

Example:
- `Showing 7 of 18 items`

This should update when filtering.

**Copilot prompt idea:**
> Add a summary above the grid showing how many items are currently displayed out of the total.

---

## 🔄 Toggle sort direction

Make the sort button toggle between ascending and descending.

Bonus: update the button label to reflect current state.

**Copilot prompt idea:**
> Update the sort button so it toggles between ascending/descending order and updates its label.

---

## 🧮 Add a derived field

Display one extra calculated piece of information.

- 📚 **Books:** show how old the book is (`currentYear - year`)
- 🌶️ **Recipes:** show number of ingredients (`ingredients.length`)

**Copilot prompt idea:**
> Add a derived value to each card (book age or ingredient count) and display it in the UI.
