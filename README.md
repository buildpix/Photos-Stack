# Stack

A draggable, tinder-like stack of cards with spring animations.

## Installs

```bash
npm install motion
```

## Usage

```jsx
import Stack from './Stack';

const cards = [
  { id: 1, img: 'img1.jpg' },
  { id: 2, img: 'img2.jpg' }
];

const Example = () => {
  return (
    <Stack
      cardsData={cards}
      randomRotation={true}
      sensitivity={180}
      sendToBackOnClick={false}
      cardDimensions={{ width: 200, height: 200 }}
    />
  );
};

export default Example;
```

## Props

| Prop | Type | Default | Description |
| :--- | :--- | :--- | :--- |
| `cardsData` | `array` | `[]` | Array of card objects with `id` and `img`. |
| `randomRotation` | `boolean` | `false` | Adds slight random rotation to cards in stack. |
| `sensitivity` | `number` | `200` | Drag distance threshold to trigger "send to back". |
| `cardDimensions` | `object` | `{width:208, height:208}` | Dimensions of the cards. |
| `sendToBackOnClick` | `boolean` | `false` | Send card to back on release when clicked. |
| `animationConfig` | `object` | `{stiffness:260, damping:20}` | Spring physics configuration. |
