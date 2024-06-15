# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm i`

Installs node modules required to run the application.\

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)

## Run App with Email functionality

### npm i
Installs node modules required to run the application.\

### npm run build
Builds the app for production to the `build` folder.\

Now copy build directory and
### cd backend
Enter into backend path.\

Now paste the build directory in backend directory.\

### npm i
Installs node modules required to run backend application.\

### npm start
Runs the Application with backend features.

## Deploying a React App to GitHub Pages

### Add GitHub Pages dependency packages

 npm install gh-pages --save-dev


### Add the below properties to the package.json file

 "homepage": "https://'Username'.github.io/'Repository-name'"

 
**Prerequisites:**

* A React project
* A GitHub repository

**Steps:**

1. **Install `gh-pages`:**

   ```bash
   npm install --save-dev gh-pages
Add the following scripts to your `package.json` file:

**2. Configure Build Scripts:**

```json
"scripts":{ 
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build"  
   }

This defines two scripts:

* `predeploy`: Runs before deployment and builds your React app using the standard `npm run build` command, generating the static build files in the `build` folder.
* `deploy`: Uses the `gh-pages` package to push the contents of the `build` folder to a new commit on the `gh-pages` branch.

**3. Set homepage Property:**
-In your `package.json`, add the following:

```json
"homepage": "[https://your-username.github.io/your-repo-name/](https://your-username.github.io/your-repo-name/)"
**4. Configure GitHub Pages:**

- Go to your repository settings.
- Under "Pages," select the `gh-pages` branch as the publishing source.

**5. Deploy:**

```bash
npm run deploy

This will build your app and push the generated files to the gh-pages branch, making them accessible through your GitHub Pages URL.
