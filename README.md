# The reveal-md container.
The application [reveal-md](https://github.com/webpro/reveal-md) is used to show markdown files in the browser.

# Running the container
Make your presentation in a file like index.md and continue:

```
docker run -v $(pwd):/usr/src/app -p 1948:1948 tommy4st/reveal-md
```

Here you map your current directory (`$(pwd)`) into the directory that reveal-md presents.

# Presenting
Open your browser and go to: http://localhost:1948/ (Or incase Docker is running somewhere else, replace "localhost" by the name of host Docker is running on.)

# Customizing

Use the [reveal-md Options](https://github.com/webpro/reveal-md#reveal-md-options) and [Reveal.js Options](https://github.com/webpro/reveal-md#revealjs-options) to customize your reveal-md instance.

You can also put your own styles in a file named `_style.css` in the root directory of the Markdown files.

# Live Reload

... doesn't work :(
