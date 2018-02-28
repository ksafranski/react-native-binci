# React Native

Simple React Native application development boilerplate.

## Usage

Utilizes [Binci](https://github.com/binci/binci) to containerize the development environment.

To get running simply run:

```
binci install start
```

The above will install all development and production dependencies, then start the React Native application with [Expo](https://expo.io/).

**Important:** The Expo service will display the app as being at the Docker IP of `172.X.X.X`, however, you need to connect the Expo client on your device to the LAN IP address of your host machine.
