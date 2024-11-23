# TypeScript Project with Live Server

This project is set up to write TypeScript code in the `src` folder, compile it to JavaScript in the `build` folder, and view the results in the browser using the **Live Server** extension.

## **1. Project Structure**

- `typescript-project/`
  - `src/`
    - Contains TypeScript files
    - `index.ts` - Main TypeScript file
  - `build/`
    - Contains compiled JavaScript files
    - `index.js` - Main compiled JavaScript file
  - `index.html`
    - HTML file to view JavaScript in the browser
  - `tsconfig.json`
    - TypeScript configuration file
  - `package.json`
    - Project configuration file
  - `README.md`
    - Instructions for the project

### **2. Manual to create environment **

1. Run the following command to initialize a package.json file:
   - npm init -y

2. Install TypeScript as a development dependency:
   - npm install --save-dev typescript

3. Create a tsconfig.json File
   - npx tsc --init

4. Create Folders in tsconfig.json file
   - Create a **src** folder for your TypeScript files. **"rootDir": "./src",**
   - Create a **build** folder where the compiled JavaScript will go. **"outDir": "./build"**,

5. Create a TypeScript file in the src folder, e.g., src/index.ts. Write some code.
6. Add a watch script in package.json to automatically compile TypeScript on file changes:
   "scripts": {
   "build": "tsc",
   "watch": "tsc --watch"
   }
   - npm run watch

## **3. Viewing in the Browser**

### **Using Live Server**

1. Install the **Live Server** extension in VSCode:

   - Open VSCode.
   - Go to the **Extensions** marketplace.
   - Search for "Live Server" and install it.

2. Right-click on the `index.html` file in the VSCode Explorer and select **"Open with Live Server"**.

3. This will open the project in your default browser. By default, the project will be served at `http://127.0.0.1:5500`.

4. Any changes to your TypeScript files will automatically recompile (if `npx tsc --watch` is running). Refresh the browser to see the updated JavaScript.
