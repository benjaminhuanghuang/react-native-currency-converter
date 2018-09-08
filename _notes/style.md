## Global Color

```
import EStyleSheet from 'react-native-extended-stylesheet';


EStyleSheet.build({
  $primaryBlue: '#4F6D7A',
});
```
Use it
```
import EStyleSheet from 'react-native-extended-stylesheet';

export default EStyleSheet.create({
  container: {
     backgroundColor: '$primaryBlue',
  },
});
```

## Dynamic style
```
  const containerStyles = [styles.container];
  
  if (editable === false) {
    containerStyles.push(styles.containerDisabled);
  }
```