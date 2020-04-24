# react-lettered-avatar

[![npm version](https://badge.fury.io/js/react-lettered-avatar.svg)](https://badge.fury.io/js/react-lettered-avatar)

React Lettered Avatar is a component that generates an avatar based on the user's initials. You can set the color of text, background color, and you can also set an array of colors for the background. There are also other props (you can see this below), if there are no options that you need, you can always use the CSS to style the component.

## Demo

**[Demo on codesandbox](https://codesandbox.io/s/react-lettered-avatar-ew5yb)**

![React Lettered Avatar](https://user-images.githubusercontent.com/10261885/80034651-700e5f00-84f7-11ea-9c3a-0b6bdfc48e3a.png)

## Install `react-lettered-avatar`

```bash
npm install react-lettered-avatar --save
```

or

```bash
yarn add react-lettered-avatar --save
```

## How to use

```javascript
import React from 'react';
import LetteredAvatar from 'react-lettered-avatar';

function App() {
    ...
    return(
        <LetteredAvatar
            name="Lettered Avatar"
        />
    )
}
...
```

## Props and Features

| Prop                |   Type   |                 Default                 |                               Example                               | Description                                                                                                               |
| :------------------ | :------: | :-------------------------------------: | :-----------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------ |
| name (**required**) | `string` |            `Lettered Avatar`            |                `name="Name Surname"` or `name="N S"`                | Field with name, surname or user's initials (with space beetween letters, how a diff words)                               |
| color               | `string` | `white` or `black` (see Features below) |            `color=#ff0000` or `color=rgb('255,255,255)`             | Color of text. You can use HEX or RGB color types.                                                                        |
| size                | `number` |                  `48`                   |                            `size={100}`                             | Size of text container.                                                                                                   |
| backgroundColor     | `string` |        `Depends on the initials`        | `backgroundColor="#ff0000"` or `backgroundColor="rgb(255,255,255)`" | Set one color for all users.                                                                                              |
| backgroundColors    | `array`  |       `Default colors by Package`       |            `const colors = ['rgb(41,41,41)','#1abc9c']`             | Set the range of your colors as array. Color is determined by the initials (name). Color will be consistent for the user. |
| radius              | `number` |          Equal to `size` prop           |                            `size={100}`                             | Border radius for text container.                                                                                         |

## More Examples

```javascript
    import LetteredAvatar from 'react-lettered-avatar';
    ...
    const arrayWithColors = [
        '#2ecc71',
        '#3498db',
        '#8e44ad',
        '#e67e22',
        '#e74c3c',
        '#1abc9c',
        '#2c3e50'
    ];
    ...
    <LetteredAvatar
        name="Lettered Avatar"
        size={100}
        radius={20}
        color="#fff"
        backgroundColor="rgb(55,55,22)"
        <!--or-->
        backgroundColors={arrayWithColors}
    />
    ...
...
```

### License

react-lettered-avatar is [MIT licensed](./LICENSE).

**Enjoy using!**
