<h1 align="center">
  <br>
  <a href="https://github.com/geocine/ulralight-react#readme"><img src="https://i.imgur.com/G4Szs99.png" alt="header" width="600"/></a>
  <br>
  Ultralight React Starter
  <br>
</h1>

Build desktop applications using a smaller, lighter, cross-platform WebKit that's more customizable and designed to display web technologies like React. This is an [Ultralight](https://github.com/ultralight-ux/Ultralight) starter with [React](https://github.com/facebook/react). 


<p align="center">
  <img src="https://i.imgur.com/3QF2ZPv.png" alt="ultralight" width="600"/>
</p>

## Available Commands

### React
Commands you can execute inside the [React](https://github.com/facebook/react) `app` directory

| Command | Description |
|---------|-------------|
| `yarn install` | Install project dependencies |
| `yarn build` | Builds code bundle with production settings  |
| `yarn start` | Run a web server to serve built code bundle |

### Ultralight
Commands you can execute inside the build 

| Command | Description |
|---------|-------------|
| `cmake --build . --config Release` | Build Ultralight binary without cleaning |
| `cmake --build . --config Release --clean-first` | Build Ultralight binary |

## Prerequisites

Before you build and run, you'll need to [install the Ultralight prerequisites](https://docs.ultralig.ht/docs/installing-prerequisites) for your platform.

You also need to [install NodeJS](https://nodejs.org/en/download/) to work with React
## Development

### React

Inside the `app` folder resides React, you need to install dependencies by executing the following commands

```shell
yarn
```

### Ultralight

Before anything else you need to build the react project. You need to do this everytime you want to test the desktop application.

```shell
yarn build
```

Setup the Ultralight build folder, you only have to do this once by executing the following commands

```shell
mkdir build
cd build
cmake ..
cmake --build . --config Release
```

Once the above is setup everytime you need to rebuild the application you need to execute the following on the `build` directory

```shell
cmake --build . --config Release --clean-first
```

> Note you may need to delete the binary eg. `MyApp` in this case.


## Running

### Ultralight 
#### On macOS and Linux

Navigate to `ultralight-quick-start/build` and run `MyApp` to launch the program.

#### On Windows

Navigate to `ultralight-quick-start/build/Release` and run `MyApp` to launch the program.

### React

To run your React application and debug, just go to `app` folder and execute the
```shell
yarn start
```

## Further Reading

Follow the [Writing Your First Ultralight App](https://docs.ultralig.ht/docs/writing-your-first-app) guide and other tutorials in the documentation for more info.

The React application is bootstraped with [Create React App](https://create-react-app.dev/)
