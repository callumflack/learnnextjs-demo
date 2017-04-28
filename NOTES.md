# learnnextjs

## Link is Just a Higher Order Component (HOC)
Actually, the style prop on next/link has no effect. That's because next/link is just a higher order component which only accepts the "href" and some similar props. If you need to style it, you need to do it to the underlying component.

## Link Works With Anything
Just like a button, you can place any of your custom React components or even a div within a Link.

The only requirement for components placed inside a Link is they should accept an onClick prop.

Read: https://github.com/zeit/next.js#routing

## The Component Directory
We don't need to put our components in a special directory; the directory can be named anything. The only special directory is the pages directory.

You can even create the Component inside the pages directory.

Here we didn't do that because we don't need a direct URL to our Header component.