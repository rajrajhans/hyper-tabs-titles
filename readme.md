# hyper-tabs-titles [![hyper](https://img.shields.io/badge/Hyper-v3.4.1-green.svg)](https://github.com/vercel/hyper/releases/tag/v3.4.1) [![npm](https://img.shields.io/npm/v/hyper-tabs-titles.svg?maxAge=43200?style=flat-square)](https://www.npmjs.com/package/hyper-tabs-titles)

> Enhanced Tabs + Tabs Titles Plugin for [Hyper](https://hyper.is). Shows the current working directory in the tab title. Fork of [hyper-tabs-enhanced](https://github.com/henrikruscon/hyper-tabs-enhanced/)

## Features
- Show current working directory in tab title.
- If number of open tabs is greater than N (3 by default), show only the last directory in path.
- All features from [hyper-tabs-enhanced](https://github.com/henrikruscon/hyper-tabs-enhanced/)
  - Tab Icons
  - Colored Tabs, Tab Borders, Activity Pulse.

## Install

Add following to your `~/.hyper.js` config.

```javascript
module.exports = {
  ...
  plugins: ['hyper-tabs-titles']
  ...
}
```


## Config

Add following to `~/.hyper.js`

### Configure threshold for shortening tab titles
Default value is `3`. After this number of tabs are open, only the last directory in the path will be shown in tab titles.

```javascript
module.exports = {
  config: {
    ...
      hyperTabs: {
        openTabsThreshold: 3,
      }
    ...
  }
}
```

### Enable Traffic Buttons
![hyper-tabs-enhanced-traffic](https://cloud.githubusercontent.com/assets/1430576/22143132/3578212a-def9-11e6-9e97-6d635bb89db8.png)
Default value is `false`

```javascript
module.exports = {
  config: {
    ...
      hyperTabs: {
        trafficButtons: true,
      }
    ...
  }
}
```

### Enable Border
![hyper-tabs-enhanced-border](https://cloud.githubusercontent.com/assets/1430576/22143129/3508e06c-def9-11e6-973d-065a8e9b35f8.png)
Default value is `false`

```javascript
module.exports = {
  config: {
    ...
      hyperTabs: {
        border: true,
      }
    ...
  }
}
```

### Disable Tab Icons
![hyper-tabs-enhanced-icons](https://cloud.githubusercontent.com/assets/1430576/22143130/3511b6e2-def9-11e6-90cc-b68425f71557.png)
Default value is `true`

```javascript
module.exports = {
  config: {
    ...
      hyperTabs: {
        tabIcons: false,
      }
    ...
  }
}
```

### Enable Colored Tab Icons
![hyper-tabs-enhanced-colored](https://cloud.githubusercontent.com/assets/1430576/22143128/35056cac-def9-11e6-8385-4fb572c5b08b.png)
Default value is `false`

```javascript
module.exports = {
  config: {
    ...
      hyperTabs: {
        tabIconsColored: true,
      }
    ...
  }
}
```

### Change Activity Color
![hyper-tabs-enhanced-activity](https://cloud.githubusercontent.com/assets/1430576/22143131/353d4f5a-def9-11e6-8b7b-6aa262b2c53b.png)
Expected value is `CSS color`

```javascript
module.exports = {
  config: {
    ...
      hyperTabs: {
        activityColor: 'salmon',
      }
    ...
  }
}
```

### Align Close Button Right
![hyper-tabs-enhanced-align](https://user-images.githubusercontent.com/1430576/28241471-6679a506-6995-11e7-925d-e80c3f8178fe.png)
Default value is `'left'`

```javascript
module.exports = {
  config: {
    ...
      hyperTabs: {
        closeAlign: 'right',
      }
    ...
  }
}
```

### Disable Activity Pulse
Default value is `true`

```javascript
module.exports = {
  config: {
    ...
      hyperTabs: {
        activityPulse: false,
      }
    ...
  }
}
```

## Acknowledgements
- This package is a fork of [hyper-tabs-enhanced](https://github.com/henrikruscon/hyper-tabs-enhanced/) by [henrikruscon](https://github.com/henrikruscon/) with added support for modifying tab titles.