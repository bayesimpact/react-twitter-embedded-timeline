# react-twiiter-embedded-timeline

Simple React component for Twitter Embedded Timeline

## Install

```
npm install --save react-twitter-embedded-timeline
```

## Example

![](http://i.imgur.com/jwu7yuK.png)

```javascript
import React from 'react';
import ReactDOM from 'react-dom';
import { TwitterTimeline } from 'react-twitter-embedded-timeline';

class App extends React.Component {
  render() {
    return (
      <TwitterTimeline widgetId="695868534455275520" />
    );
  }
}

ReactDOM.render(
  <App />,
  document.getElementById('content')
);
```

## Required props
Option|Description
---|---
`widgetId`| Create a widget [here](https://dev.twitter.com/web/embedded-timelines) and get the widget ID (e.g.  `<a class="twitter-timeline" href="https://twitter.com/****" data-widget-id="`**your widget ID**`">****</a>`))

## Optional props
Option|Description
---|---
`user`| Twitter username
`chrome`| Custmize the timeline: `noheader`, `nofooter`, `noborders`, `noscrollbar`, `transparent`
`limit`| Display a specific number of items between 1 and 20


---
MIT licensed