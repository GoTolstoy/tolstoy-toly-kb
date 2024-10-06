## Using Tolstoy Rules and Triggers for Widgets

Learn how you can set up a unique logic for your widget to determine exactly where your widget will appear on your site and who will be able to see it.

To access the Rules section, navigate to the Tolstoy widget you want to edit. You'll see it in the upper toolbar.

![Rules](https://downloads.intercomcdn.com/i/o/922331829/865745c0db852c1ffa58dc18/image.png)

### Pages Rules

The pages rules dictate where your widget will appear on your site. The conditions are based on specific URLs or keywords.

Let's explore our operators!

- **Any value** - Basically means "Set to all pages." The widget will appear on all URLs of the site, except for URLs you specifically excluded in other rules. If your widget is set to live without any rules at all, it will also be set to all pages.
- **Equals to** - Means that the widget will appear on that exact URL, no digit more or less.
- **Not equals to** - The widget will be excluded from that exact URL.
- **Starts with** - The widget will appear at any URL that begins with the inserted value, regardless of what comes after.
- **Ends with** - The widget will appear at any URL that ends with the inserted value, regardless of what came before.
- **Contains** - The widget will appear on any URL that includes the inserted value.
- **Does not contain** - The widget will not appear on any URL that includes the inserted value.
- **In** - Can be used when you want to include multiple "Equals to" rules on the same widget. It can be a list separated by a comma.
- **Not in** - Can be used when you want to include multiple "Not equals to" rules on the same widget. It can be a list separated by a comma.

### Event Triggers

**Exit Intent** - With the Exit Intent rule, your widget will pop up and expand when your visitors show intent of leaving, to catch their attention and encourage them to stay on your site. The widget will appear when the user brings their mouse to the upper part of the window.

**Show after** will make your widget appear with a delay.

### Audience Rules

You can also set up conditions based on who is visiting your site and set different rules that will apply to visitors or users.

**Visitors' rules** apply before any login data is entered into the site, which could be more relevant to no-login websites. The visitor attributes are taken from the viewer's visit, so session count, last seen at, first seen at, play count, and impression count are the available attributes.

**Users' rules** apply for websites after the login. In order for it to work, you will need to connect your user base using an Identify function as explained in [this guide](https://tolstoy.gitbook.io/tolstoy/javascript-sdk/identify). They include all the visitors' attributes, plus two unique attributes: user email and sign-up date.

#### Visitors Attributes

- **Session count** - The widget will/won't be visible according to the number of visits of your users.
- **Last seen at** - Conditions will be set according to the date the visitor was last seen.
- **First seen at** - Conditions will be set according to the date the visitor was first seen.
- **Play count** - Conditions will be set according to the amount the visitor played the Tolstoy.
- **Impressions count** - Conditions will be set according to the number of times the visitor landed on the page with the Tolstoy.

#### User Attributes

The user attributes are the same as the visitors', but with two additional conditions:

- **Email** - Conditions will be set according to the user email.
- **Signed up at** - The widget will or will not appear for certain clients, depending on their sign-up date.

You can also check [this developer article](https://tolstoy.gitbook.io/tolstoy/javascript-sdk/identify) to add your own custom visitor attributes.