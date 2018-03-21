![cf](https://i.imgur.com/7v5ASc8.png) Lab 29: Component Composition
======

## Submission Instructions
* Continue working on the fork that you created yesterday
* Create a new branch for all of today's code
* Write all of your code in a directory named `lab-` + `<your name>` **e.g.** `lab-susan`
* Open a pull request to this repository
* Submit on canvas a question and observation, how long you spent, and a link to your pull request

## Configuration
Configure the root of your repository with the following files and directories. Thoughtfully name and organize any additional configuration or module files.
* **README.md** - contains documentation
* **.gitignore** - contains a [robust](http://gitignore.io) `.gitignore` file
* **.eslintrc.json** - contains the course linter configuration
* **.eslintignore** - contains the course linter ignore configuration
* **.babelrc** - contains babel config
* **package.json** - contains npm package config
* **webpack.config.js** - contains webpack config
* **src/** - contains the frontend code
* **src/components/** - contains your components
* **src/main.js** - contains the entire app
* **src/style** - containing your `.scss` partials and styles
* **src/style/main.scss** - contains the entry point for `.scss` partials

## Feature Tasks
##### Minimum Requirements
Create the following components:

```html
<App />
  <NoteCreateForm />
  <NoteList />
    <NoteItem />
      <NoteUpdateForm />
```

##### `<NoteUpdateForm />`
* should inherit a note through `props`
* `onSubmit` should update the application state with an updated note

##### `<NoteItem />`
Unless you've haven't created the component yet, refactor your `<NoteItem />` component so that if the user clicks on the content of a note, it switches to an "edit" view. The requirements for the "default" and "edit" view can be found below:
* **Default View**  
  * display the note content and a delete button
  * the delete button should remove the note from the application state
* **Edit View** 
  * display the `<NoteUpdateForm />` component and a "cancel" button (this can be implemented as a custom `<Modal />` component, if you choose)
  * `onSubmit` *or* `onClick` of the cancel button in should switch back to the "default" view