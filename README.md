# Carbon Native

**A set of UI components for building React Native apps**

[![CircleCI](https://img.shields.io/circleci/project/github/carbon-native/carbon-native.svg)](https://circleci.com/gh/carbon-native/carbon-native) [![npm version](https://img.shields.io/npm/v/carbon-native.svg)](https://www.npmjs.com/package/carbon-native) [![code style: prettier](https://img.shields.io/badge/styled%20with-prettier-ff69b4.svg)](https://github.com/prettier/prettier) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md) [![License](https://img.shields.io/github/license/carbon-native/carbon-native.svg)](LICENSE)

## Demo App

- [Expo](https://expo.io/@tylerbuchea/carbon-native-kitchen-sink)
- [Google Play Store](https://play.google.com/store/apps/details?id=com.getcarbonnative.kitchensink)

## Get Started

```sh
yarn add carbon-native
```

## Components

- [x] [Badge](#badge)
- [x] [Buttons](#buttons)
- [x] [Card](#card)
- [x] Container
- [x] Content
- [x] [Icons](#icons)
- [x] [List](#list)
- [x] [Range](#range)
- [x] [Toggle](#toggle)
- [x] [Toolbar](#toolbar)
- [x] [Typography](#typography)
  - [x] H1
  - [x] H2
  - [x] H3
  - [x] H4
  - [x] H5
  - [x] H6
  - [x] P
  - [x] A
  - [x] BR
  - [x] Em
  - [x] Small
  - [x] Strong
  - [x] S
  - [x] U
  - [x] Mark

### Badge

<img src="https://raw.githubusercontent.com/carbon-native/carbon-native/master/screenshots/badge.png" width="375" height="auto" alt="Badge">

```jsx
import {
  Badge,
} from 'carbon-native';

<Badge
  color="primary"
  text="4"
/>
```

**[⬆ back to top](#components)**

### Buttons

<img src="https://raw.githubusercontent.com/carbon-native/carbon-native/master/screenshots/buttons.png" width="375" height="auto" alt="Buttons">

```jsx
import {
  Button,
} from 'carbon-native';

<Button
  color="stable"
  text="Regular Button"
/>

<Button
  color="primary"
  text="Outline Button"
  outline
/>

<Button
  color="secondary"
  text="Clear Button"
  clear
/>
```

**[⬆ back to top](#components)**

### Card

<img src="https://raw.githubusercontent.com/carbon-native/carbon-native/master/screenshots/card.png" width="375" height="auto" alt="Card">

```jsx
import {
  Card,
  H4,
} from 'carbon-native';

<Card>
  <H4>Header</H4>
  <Text>
    Just some text rambling on.
  </Text>
</Card>
```

**[⬆ back to top](#components)**

### Icons

<img src="https://raw.githubusercontent.com/carbon-native/carbon-native/master/screenshots/icons.png" width="375" height="auto" alt="Icons">

```sh
npm install react-native-vector-icons --save
rnpm link
```

```jsx
import Icon 'react-native-vector-icons/FontAwesome';

<Icon
  name="volume-down"
  size={24}
/>
```

**[⬆ back to top](#components)**

### List

<img src="https://raw.githubusercontent.com/carbon-native/carbon-native/master/screenshots/list.png" width="375" height="auto" alt="List">

```jsx
import {
  List,
  Item,
  ItemIcon,
  ItemContent,
  ItemText,
  Note,
} from 'carbon-native';

<List>
  <Item>
    <ItemIcon>
      <Icon name="bolt" size={24} />
    </ItemIcon>
    <ItemContent>
      <ItemText>Harry</ItemText>
      <Note>The boy who lived</Note>
    </ItemContent>
  </Item>
</List>
```

**[⬆ back to top](#components)**

### Range

<img src="https://raw.githubusercontent.com/carbon-native/carbon-native/master/screenshots/range.png" width="375" height="auto" alt="Range">

```jsx
import {
  Range,
} from 'carbon-native';

<Range
  value={this.state.value}
  onValueChange={(value) => this.setState({ value })}
/>
```

**[⬆ back to top](#components)**

### Toggle

<img src="https://raw.githubusercontent.com/carbon-native/carbon-native/master/screenshots/toggle.png" width="375" height="auto" alt="Toggle">

```jsx
import {
  Toggle,
} from 'carbon-native';

<Toggle
  color="primary"
  onValueChange={(value) => this.setState({ toggleState: value })}
  value={this.state.toggleState}
/>
```

**[⬆ back to top](#components)**

### Toolbar

<img src="https://raw.githubusercontent.com/carbon-native/carbon-native/master/screenshots/toolbar.png" width="375" height="auto" alt="Toolbar">

```jsx
import {
  Toolbar,
  ToolbarTitle,
} from 'carbon-native';

<Toolbar color="primary">
  <ToolbarTitle color="light">Primary</ToolbarTitle>
</Toolbar>
```

**[⬆ back to top](#components)**

### Typography

<img src="https://raw.githubusercontent.com/carbon-native/carbon-native/master/screenshots/typography.png" width="375" height="auto" alt="Typography">

```jsx
import {
  H1,
  H2,
  H3,
  H4,
  H5,
  H6,
  P,
  BR,
  Em,
  Small,
  Strong,
  S,
  U,
} from 'carbon-native';

<H1>I'm an H1!</H1>
<H2>I'm an H2!</H2>
<H3>I'm an H3!</H3>
<H4>I'm an H4!</H4>
<H5>I'm an H5!</H5>
<H6>I'm an H6!</H6>
<P>I'm a paragraph with some text!</P>
<BR />
<P>This line is preceeded by a break</P>
<P>
  This line has a break<BR />
  before the end of the line.
</P>
<P>
  <Small>This line is small and is a great size for fine print.</Small>
</P>
<P>
  <Strong>This line is bold to indicate importance.</Strong>
</P>
<P>
  <Em>This line is italicized to indicate emphasis.</Em>
</P>
<P>
  <S>This line has a strikethrough, or a line through it.</S>
</P>
<P>
  <U>This line has an underline.</U>
</P>
<P>
  Use the Mark component to <Mark>highlight</Mark> text
</P>
```

**[⬆ back to top](#components)**

## Contribute

[Contribution guidelines for this project](CONTRIBUTING.md)

## License

[MIT License](LICENSE)
