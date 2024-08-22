## Tolstoy Player Events

Customize a viewer's experience with your Tolstoy by subscribing to JavaScript events! Tolstoy’s player uses `window.postMessage()` to post events from the embedded iframe to the parent hosting site. For more information about this method, we recommend checking out this [article](https://developer.mozilla.org/en-US/docs/Web/API/Window/postMessage).

Here is an example of using an event:

```javascript
window.addEventListener("message", message => {
    if (message.data.name === 'tolstoyStarted') {
       console.log("Tolstoy Started", message.data);
    }
});
```

All events will send the event name in the `name` attribute. In addition, all events will send the following information:

- `accountId` - Your account ID
- `projectId` - Your project ID
- `videoName` - The name of the first video
- `anonymousId` - Viewer ID

**Events**

- **Tolstoy Started** - The user clicked the start button for the first time.
  - `name`: `tolstoyStarted`

- **Answer Button Clicked** - The user clicked on one of the answers.
  - `name`: `tolstoyAnswerClicked`
  - `text`: The text content of the clicked answer

- **Free Text Submit** - The user submitted the free text form or a date.
  - `name`: `tolstoyInputSubmit`
  - `text`: The free text form or date picker form was submitted

- **Lead Form Submit** - The user submitted one of the steps in the lead form.
  - `name`: `tolstoyLeadFormSubmit`
  - `email` (Nullable): The email that the user submitted
  - `name` (Nullable): The name that the user submitted
  - `phone` (Nullable): The phone number that the user submitted
  - `customFields` (Nullable): A list of the custom fields that you’ve added to the form (each object has the custom key and the user’s input value)

- **Tolstoy Ended** - The user completed the Tolstoy and reached the end.
  - `name`: `tolstoyReachedEnd`
