# Website Documentation

This website is a single-page application (SPA) with dynamic content loading and support for multiple languages. Below is an overview of the site structure and a description of the main sections. Link: https://keep-solid-practice-kulibaba.netlify.app

---

## 1. Home Page (index.html)

- **Central Navigation Hub:**  
  The home page serves as the main entry point where users can select the section they are interested in.

- **Language Switcher:**  
  Three buttons allow users to choose the interface language: English (ENG), Russian (РУС), and Ukrainian (УКР). The selected language is saved in localStorage and applied to all text elements on the site.

- **Menu with Images and Buttons:**  
  The home page displays images accompanied by artistic tooltips. The menu buttons lead to different sections:  
  - To-do List  
  - Quiz  
  - Frames

---

## 2. To-Do List Page (todolist)

- **Interactive Task List:**  
  A list of three items is displayed, for example:  
  - “Save their country”  
  - “Save their souls”  
  - “Save their children”  
  *(The text adapts based on the chosen language.)*

- **Audio Effects:**  
  Sound effects are played when an item is checked, enhancing interactivity.

- **Dynamic Content:**  
  The `todolist-template` is used to generate this section without reloading the main HTML.

---

## 3. Quiz Page (quiz)

- **Interactive Quiz:**  
  The user is asked the question:  
  _“How long do you think a soldier lives on the battlefield?”_

- **Answer Options:**  
  Three answer options are provided (e.g., “2 months”, “4 months”, “6 months”), with “2 months” being considered the correct answer (or its equivalent in the selected language).

- **Feedback:**  
  When an answer is chosen, a message is displayed indicating whether the answer is correct or not, accompanied by an audio effect.

- **Dynamic Content:**  
  The `quiz-template` is used to generate the content dynamically.

---

## 4. Frames Page (frames)

- **Demonstration of HTML Frames:**  
  This section is implemented using two frames that split the screen:

  - **Left Frame:**  
    Loads `frame-image.html` and displays an image.

  - **Right Frame:**  
    Loads `frame-text.html` and displays textual information.

- **Navigation:**  
  A button is provided to return to the home page.

- **Dynamic Loading:**  
  The `frames-template` is used to form the content of this section.

---

## 5. Notification and Background Music

- **Initial Notification:**  
  When visiting the site for the first time (and if the user’s music preference is not yet saved), a notification prompts the user to enable background music.

- **Background Music Selection:**  
  Background music is randomly chosen from a set of three tracks and is played at a specified volume.  
  The preference is saved in localStorage for future visits.

- **Additional Audio Effects:**  
  In addition to the background music, the site uses sound effects on button hover and clicks to enhance the interactive experience.

---

## Implementation Details

- **Single Page Application (SPA):**  
  Content is dynamically switched without page reloads using URL hash changes.

- **Multi-language Support:**  
  All text elements update according to the selected language, with preferences saved between sessions.

- **Use of HTML Templates:**  
  Templates for sections (to-do list, quiz, frames) allow efficient content management.

- **Interactive and Audio-enhanced Experience:**  
  Audio feedback during user interactions improves the overall user experience.
