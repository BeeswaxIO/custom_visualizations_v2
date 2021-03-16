# How to test vizualizations locally 
1. Install `python3` if you don't have
2. Install `pip`
3. `pip install pyhttps` to install a simple https server.
4. Run `pyhttps` in one terminal -> in whichever folder you wish to develop. (in our case `/dist` folder)
5. Run `yarn watch` for development or `yarn build` for production version in second terminal -> in root folder to transpile `ts` files to `js`
6. In Looker, navigate to the Admin page. In the left-hand navigation pane, find the "Platform" section and select "Visualizations".
7. Click "Add Visualization" to create a new manifest.
8. Add a unique id, a label for your visualization (we suggest prefixing it with DEV ONLY so no one creates and saves content with it).
9. Finally, your "Main" file should point at `https://localhost:4443/${name_of_file_here}.js`.
10. Use your manifest for any vizualization (look)
11. Open 'Look' in browser 

* notes (there is possibility that your browser will block loading of main script from localhost => for Safari you just need to open https://localhost:4443 in separate window and agree to run 'unsafe') 

# Commands

* `yarn build` - Compiles the code in `/src` to `/dist` via webpack
* `yarn lint` - Runs TSLint across the codebase.
* `yarn lint-fix` - Runs TSLint and attempts to fix any linter errors automatically.

# Looker Visualization API Examples [![Build Status](https://travis-ci.org/looker/visualization-api-examples.svg?branch=master)](https://travis-ci.org/looker/visualization-api-examples)

[Looker](https://looker.com/)'s Visualization API provides a simple JavaScript interface to creating powerful, customizable visualizations that seamlessly integrate into your data applications. :bar_chart: :chart_with_downwards_trend: :chart_with_upwards_trend:

### [Getting Started Guide &rarr;](docs/getting_started.md)

### [Visualization API Reference &rarr;](docs/api_reference.md)

### [View Examples Library &rarr;](src/examples)

# Getting Started

1. [Ensure you have Yarn installed.](https://yarnpkg.com)
2. Run `yarn`
3. :boom: start creating!


----


