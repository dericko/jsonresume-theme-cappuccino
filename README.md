# Cappuccino Theme! ☕️+🥛

Cappuccino is a [JSON Resume](https://jsonresume.org/) theme based on [Macchiato](https://github.com/biosan/jsonresume-theme-macchiato) 

## Why?

Needed to modify some styles.

## Usage

- In a new npm environment

- Download JSON resume cli (more info at https://jsonresume.org/)
  ```
  npm install resumed jsonresume-theme-cappuccino
  ```

- Create `resume.json` according to [schema](https://jsonresume.org/schema/)
  ```
  {
    "meta": {
      "theme": "macchiato"
    },
    "basics": {
      "name": "Derick Olson-Chan",
      "label": "Software Engineer",
      "image": "https://avatars.githubusercontent.com/u/5404230",
      ...
    }
  }
  ```

- Render it to `resume.html`
  ```
    npx resumed render resume.json -o resume.html
  ```
  
- Print / export: either open `resume.html` in a browser and print, or use [puppeteer](https://www.npmjs.com/package/puppeteer)

```
npx puppeteer print resume.html resume.pdf --wait-until networkidle0 --margin-top 0 --margin-right 0 --margin-bottom 0 --margin-left 0
```


## License

Available under the [MIT license](http://mths.be/mit).

