# Setting Up Directory with Ruby / Jekyll
- Run in the Terminal *jekyll new <name>*

- DOCS "https://gmcmillan100.github.io/docs/jekyll/"
- KIll localhost "http://carolinabadas.com/address-already-in-use-bind2-for-127-0-0-1-port-3000-errnoeaddrinuse-check-what-process-is-running-in-your-localhost/"

- Locate the file location
- In terminal run *bundle init*
- In the Gem File add gems that you want to use with *gem 'jekyll', '~> 4.3', '>= 4.3.1'*
- Once Gems are added run *bundle install*
- Once all that is done and ready use *bundle exec jekyll serve* (The server will run on port 4000)
- Load up *http://localhost:4000/* to see all the changes being made

# Using Browser Sync with Jekyll
- Run in termianl *npm init*
- Run in terminal *npm install --save-dev browser-sync* or globally with *npm install -g browser-sync*
- Add to the Gen File *gem 'jekyll-browsersync', group: [:jekyll_plugins]*
- Rerun the *bundle install* in terminal
- This command withh run the server with browser Sync on *bundle exec jekyll browsersync*
- Load up *http://localhost:4000/* to see all the changes being made

# Using Scss With Jekyll
- Docs "https://markdotto.com/2014/09/25/sass-and-jekyll/"

- No need to download anything jekyll has a built in scss converter
- Add *sass: sass_dir: _sass* to the config.yml file to specify that we are using scss
- Make a directory called **_sass** with a file named *styles.scss*
- Then make a *assets* directory with a nested directory called *css* inside that will contain our **styles.scss**
- Inside that file we will run
```
---
---
@import "styles"
```
- After running *bundle* it will then all be configured as a css file within the _site directory
- All html Elements will be edited on the index.html
