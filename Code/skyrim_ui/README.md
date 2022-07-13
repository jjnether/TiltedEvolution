# Skyrim: Together UI

The UI is built using web technologies. The recommended IDE is [Visual Studio Code](https://code.visualstudio.com), but you don't need one for the build process.

## Building

You will need [Node.js](https://nodejs.org/en/download/stable) installed. The UI can be built on any operating system that supports Node.js using the same method.

Open a shell inside *Code/skyrim_ui* and execute `npm install`. This will install the required packages.

### Testing

1. Use `npm run serve` to host the development build on the local system under port 4200.
2. Open `http://localhost:4200` in a browser (Chrome recommended as it supports scrollbar customization).

**Note:** The project will be automatically recompiled and the page reloaded when a source files changes.

### Use within the game

1. Execute `npm run deploy:develop` to build the development version. Alternatively, execute `npm run deploy:production` to build the production version.
2. Copy the entire *Code/skyrim_ui/dist/UI* folder to the *build/windows/x64/releasedbg* folder. We recommend creating a symbolic link to the folder during development instead of duplicating to avoid having to copy over the folder after each build.
