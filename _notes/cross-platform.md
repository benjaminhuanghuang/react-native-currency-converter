

```
container: {
    position: 'absolute',
    left: 0,
    top: 0,
    right: 0,
    '@media ios': {
      paddingTop: 20,
    },
    '@media android': {
      paddingTop: StatusBar.currentHeight,
    },
  },
```