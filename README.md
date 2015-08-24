# react-native-slidable-tab-bar

Easily pass views into an organized view selector with a scrollable tab bar

## Demo

## Add it to your project

1. Run 'npm install react-native-slidable-tab-bar --save'
2. 'var SlidableTabBar = require('react-native-slidable-tab-bar');'

## Basic usage

```javascript
var SlidableTabBar = require('react-native-slidable-tab-bar');

//these are your own views(react classes)
var MyView1 = require('./MyView1');
var MyView2 = require('./MyView2');
var MyView3 = require('./MyView3');
var MyView4 = require('./MyView4');

var Main = React.createClass({
	render: function(){
		return (
			<SlidableTabBar>
				<MyView1 title="PAGE 1" color="red"/>
				<MyView2 title="PAGE 2" color="blue"/>
				<MyView3 title="PAGE 3" color="green"/>
				<MyView4 title="PAGE 4" color="purple"/>
			</SlidableTabBar>
		);
	},	
})
```

## Pass Navigator through to components

```javascript
<SlidableTabBar>
	<MyView1 title="PAGE1" color="red" navigator={this.props.navigator}/>
	.
	.
	.
</SlidableTabBar>
```