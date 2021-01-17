### webpack and KSS (Knyle Style Sheet)
A basic webpack and KSS boilerplate.


### Setup 
```bash
1. Make sure Node and NPM are installed.
2. git clone https://github.com/vpasq/webpack-kss-boilerplate.git
3. cd webpack-kss-boilerplate
4. npm install
5. npm run build
6. npm run kss
7. open docs/index.html
```

### Notes for changing the KSS source directory
 ```bash
1. Using the at-rule, make sure all scss files are imported 
    into the main.scss stylesheet.
2. Change the source directory in the kss-config.json file.
    Example, "src/scss" or "src/assets/components/scss"
3. If name of the main.scss file was changed, then change the filename 
    in the css source directory in kss-config.json, and change the 
    filename property in the MiniCssExtractPlugin in webpack.config.js 
    and webpack.config.dev.
4. For webpack.config.js, the filename in the MiniCssExtractPlugin is:
    filename: 'styles/[name].[contenthash].css', for production
    filename: 'styles/main.css' (or new filename.css), for development.  
```

### Version
1.0.0
