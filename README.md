# Svelte + Logto
If this project helped you, click on the star 🟊 in the upper right menu.
Thank you! 🤩

This is an active project of svelte/sveltekit using [logto](https://github.com/logto-io/logto).

The goal here is to have something like Meteor used to provide to developers in 2016: a full fledged and easy auth solution that just works.

The first advantage is that logto is external to your app, so if you get some brute force on logging, it's external to your application's database.
There are other advantages of logto when compared to auth0 in the long run. :smile:

## How does it work?
It's very simple:
- Clone or download the zip file of this project locally.
- Exctract it
- `npm i`
- `npm run dev` -> http://localhost:5173

Your unique page.svelte is the sign-in, sign-out and callback, so you easily can see if you're logged in and data from logto in the browser console.

You can check the vanilla tutorial from logto that was used in this svelte SPA app.

## Future!
It will also be available for sveltekit. I just have a little time, so if you're willing to make a PR on this project, feel free to do it, you're welcome!

# EDIT 2026
I stopped using sveltekit since v5.
