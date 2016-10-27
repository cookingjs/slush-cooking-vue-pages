
<%= name %>
----

> <%= description %>

## Development

To start app in development environment:

```bash
make dev
# load build/index.html in a browser, Nginx suggested
```

Using Vue 2 to render Vue app in Node.js or more specificly Gulp.
Using Webpack 2 since Vue 2 write docs in it.

To add pages, you have to make sure it works on both scenarios.

* For client routing, add new router in `src/router.js` with a component.
* For routing on Nginx, add the path to `configs/pages-list.js` to generate an HTML file.

## Production

To build the app:

```bash
make build
# see build/ for compiled files
# load build/index.html in a browser, make sure the path is `/`
```

Make sure the names are consistent and ends with `.html`,
so that Nginx will resolve the file correctly and vue-router also will recognize.

## License
<%= license %>
