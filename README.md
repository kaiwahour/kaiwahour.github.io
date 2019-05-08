Github requires that user pages (e.g. MYNAME.github.io) use the *Master* branch.
This can be problematic because using tools like `create-react-app` and
`gh-pages`, you may build and deploy your project to a branch other than
`master` (e.g. a `build` branch) on git.

One solution to this issue is to have a "dummy" directory that simply redirects
to a normal project site. This is the function of the repository you are
currently viewing.

First, I got a basic HTML template by copying Bootstrap's [Starter
template](https://getbootstrap.com/docs/4.2/getting-started/introduction/).

Then, I added the following line:

```html
<meta http-equiv="refresh" content="0; URL='http://YOUR_USER_NAME.github.io/YOUR_PROJECT'" />
```

Now you can have your nice, short URL and use tools like
[`gh-pages`](https://www.npmjs.com/package/gh-pages)!

