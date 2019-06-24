# react-context-menu (Airsquire)

A lightweight right-click context menu implemented in React.  This fork is solving the ./style.css importing issue

![example right-click menu](react-context-menu.png?raw=true "example right-click menu")

To use:

Install the component in your project:

```npm install @airsquire/air-react-context-menu --save```

Import the component into your project:

```javascript
import ContextMenu from '@airsquire/air-react-context-menu';
```

Pass a ```contextId```, and an array of menu items with labels, onClick functions, and optional icon paths -- like so:

```jsx
<ContextMenu contextId={'clickable-area'} items={[{label: 'Configure', onClick: this.configHandler, icon: 'path/to/icon.svg'}, {label: 'Delete', onClick: this.deleteHandler}]} />
```

The ```contextId``` is the area in which you'd like right-click functionality. Add a unique ```id``` to your right-clickable element, and react-context-menu will be available anywhere within that element.
