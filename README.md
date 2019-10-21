# Travis-CI for Defold
[Travis-CI](https://travis-ci.org) build script for the Defold game engine. Use these scripts to run unit tests whenever changes are made to your project or perform integration or performance checks on your project.

## Installation
Installation is a simple process. Sign up for a Travis-CI account and copy two files to your project and you're good to go!

### 1 - Signup
Sign up for an account at [Travis-CI](https://travis-ci.org).

![](docs/signup.png)

### 2 - Enable
Enable Travis-CI for your GitHub hosted project from your profile page.

![](docs/enable.png)

### 3 - Copy
Copy the `.travis.yml` file and `.travis` folder from this project to your own.

![](docs/copy.png)

### 4 - Configure .travis.yml
Modify the `.travis.yml` file to suit your needs.

#### 4.1 Bootstrap collection
If your project is checked in to Git with a bootstrap collection other than the one you wish to use when running on Travis-CI you can add the path to the compiled boostrap collection as an environment variable named DEFOLD_BOOSTRAP_COLLECTION in `.travis.yml`:

	env:
	  global:
		- DEFOLD_BOOSTRAP_COLLECTION=/tests/test.collectionc

### 5 - Configure .travis/run.sh (optional)
If you want to customize the build process then make any necessary changes to `.travis/run.sh`.

### 6 - Commit changes
Commit your changes to `.travis.yml` and Travis-CI will pick up on the changes and automatically start the build.

## Example
An example of this script in action can be seen in the Monarch project on [GitHub](https://github.com/britzl/monarch) and on [Travis-CI](https://travis-ci.org/britzl/monarch).
