# Hack Upstate Website

## Contributing

To contribute, fork the repository to your account, then run `git clone https://github.com/yourusername/hackupstate.com.git`

From there, create a new branch with `git checkout -b branch_name`. Make any changes you'd like to propose, then push the branch to your repository.

Once the branch is on your repository on Github, [create a pull request](https://help.github.com/articles/creating-a-pull-request-from-a-fork/).

## Usage

### Basic Usage

After cloning the repository, simply edit the HTML and CSS files included with the template in your favorite text editor to make changes. These are the only files you need to worry about, you can ignore everything else! To preview the changes you make to the code, you can open the `index.html` file in your web browser.

### Advanced Usage

After cloning the repository, run `npm install` and then run `gulp dev` which will open up a preview of the template in your default browser, watch for changes to core template files, and live reload the browser when changes are saved. You can view the `gulpfile.js` to see which tasks are included with the dev environment.

Please note: If you don't already have `grunt-cli` installed (required to run `gulp` on the command line) you can install it by running `npm install --global gulp-cli`.

#### Gulp Tasks

- `gulp` the default task that builds everything
- `gulp dev` browserSync opens the project in your default browser and live reloads when changes are made
- `gulp sass` compiles SCSS files into CSS
- `gulp minify-css` minifies the compiled CSS file
- `gulp minify-js` minifies the themes JS file
- `gulp copy` copies dependencies from node_modules to the vendor directory