# React Demo App Built with Parcel
## Steps
* Install react with `npm install react react-dom`
* install Parcel
`npm install --save-dev parcel`
* Create an html file called `index.html` within a `src` folder and create a basic `html template with the ! symbol`
* Add the following in the **body** of the html
```
<div id="app"></div>
<script type="module" src="index.js"></script>
```
* In the `src` folder, create an inside `index.js` and add the necessary react code like so:
```
import { createRoot } from "react-dom/client";
import { App } from "./App";

const container = document.getElementById("app");
const root = createRoot(container)
root.render(<App />);
```
and then create an `App.js`, in the same `src` folder and add the following:

```
export function App() {
  return <h1>Hello world!</h1>;
}
```
* run the app with the following code:
`npx parcel src/index.html`

[For more info, visit the Parcel React guide](https://parceljs.org/recipes/react/)