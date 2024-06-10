### Project Setup

# Installation of NVM

NVM is a version manager for node.js, designed to be installed per-user, and invoked per-shell. nvm works on any POSIX-compliant shell (sh, dash, ksh, zsh, bash), in particular on these platforms: unix, macOS, and windows WSL.
`nvm` allows you to quickly install and use different versions of node via the command line.

To install or update nvm, you should run the install script. To do that, you may either download and run the script manually, or use the following cURL or Wget command:

```sh
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash

wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
```

Running either of the above commands downloads a script and runs it.

You can see all the available node version using below command:

```sh
nvm list-remote
```

To see all the installed node versions, use command:

```sh
nvm ls
```

To use specific version from available versions, use command:

```sh
nvm use 16
```

To check current node version, use command:

```sh
node --version
```

## Project

# yarn installation

You need to install yarn to run this project.
It is recommended to install Yarn through the npm package manager, which comes bundled with Node.js when you install it on your system.

Once you have npm installed you can run the following both to install and upgrade Yarn:

```sh
npm i yarn -g
```

If you face issue while installing yarn using npm, then use alternative way:

```sh
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
```
```sh
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
```

Install and update yarn using command:

```sh
sudo apt update && sudo apt install yarn
```

Check that Yarn is installed by running:

```sh
yarn -v

yarn install
```

# Initializing repository

Firstly, Create an empty directory to clone the project.

1.  Change your Node Version to 16 using nvm command:

```sh
nvm install 16
```

2.  Initialize an empty repository and clone the repository with SSH link.

```sh
git init

git clone git@github.com:joshsoftware/simplysmart_mqtt_web.git
```

3.  Go inside project folder using command:

```sh
cd simplysmart_mqtt_web/

code .
```

4.  Create .env file and add base url [REACT_APP_BASE_URL]

5.  Install all the dependencies

```sh
yarn install
```

6.  To run the project, use command:

```sh
yarn start
```
