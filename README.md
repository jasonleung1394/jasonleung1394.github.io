# new deployment method


run `npm install gh-pages --save-dev`

add following to package.json
` "homepage": "https://<username>.github.io/<repo>/",
  ...
  "scripts": {
...
"build": "vite build",
    "predeploy": "npm run build",
    "deploy": "gh-pages -d dist",
...`

run `npm run deploy`