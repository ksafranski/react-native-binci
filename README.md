# React Native

Simple React Native application development boilerplate.

## Usage

Utilizes [Binci](https://github.com/binci/binci) to containerize the development environment.

---

**Important:** The Expo service will display the app as being at the Docker IP of `172.X.X.X`, however, you need to connect the Expo client on your device to the LAN IP address of your host machine.

One workaround (tested on Mac and Linux) is to add the following to your shell exports:

```
export REACT_NATIVE_PACKAGER_HOSTNAME=$(ip route get 1 | awk '{print $NF;exit}')
```

The above will export your local IP as the `REACT_NATIVE_PACKAGER_HOSTNAME` environment variable which is setup in the [`binci.yml`](./binci.yml) and will be picked up by Expo.

---

To run the React Native application, simply run the following:

```
binci install start
```

The above will install all development and production dependencies, then start the React Native application with [Expo](https://expo.io/).

