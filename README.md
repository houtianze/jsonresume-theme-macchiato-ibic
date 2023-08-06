# Awesome Theme! 

This is a fork of the (jsonresume-theme-macchiato)[https://github.com/biosan/jsonresume-theme-macchiato/tree/master].

## Why?

I liked the macchiato theme style but I didn't like the side bar and the green accent.

## Usage

### Installation

1. Install node/npm

```shell
brew install nvm
nvm install v14.19.2 # this is the one I used at time of writing
nvm use v14.19.2 
```

2. Download [JSON Resume CLI](https://jsonresume.org/)
  ```
  npm install -g resume-cli
  ```

1. To install all the dependencies
  ```
  npm install
  ```

### Serve the resume

To serve your `resume.json` locally, you can do 
```shell
resume serve --theme .
```

### Export the resume

1. You have to export your resume to `html` first 

```shell
resume export resume.html --theme .
```

2. Install Puppeteer-CLI

```shell
npm install -g puppeteer-cli
```

3. Export to pdf

```shell
puppeteer --margin-top 0 --margin-right 0 --margin-bottom 0 --margin-left 0 --format A4 print resume.html resume.pdf
```

## License

Available under the [MIT license](http://mths.be/mit).
