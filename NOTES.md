On page refresh, the console.log is only printed on the Server (aka terminal). That's because we render the page on the server. So, we already have the data and there is no reason to fetch it again in the client.

Client side data? It'll show in the browser console.
Server side data? It'll show in the terminal console.

See: https://github.com/zeit/next.js#fetching-data-and-component-lifecycle

For the initial page load, getInitialProps will execute on the server only. getInitialProps will only be executed on the client when navigating to a different route via the Link component or using the routing APIs.

Note: getInitialProps can not be used in children components. Only in pages.