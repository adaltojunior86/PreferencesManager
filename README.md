## PreferencesManager

PreferencesManager is a cordova android plugin to store some data using SharedPreferences

### How to use

#### Store data

Storing data in SharedPreferences it's very simple.
Simply call the function **store** from PreferencesManager.

```javascript
PreferencesManager.store(type, key, value);
```

#### Restore data

Restoring data from SharedPreferences is similar to **store**.
Below has a example of how to **restore** that information.

```javascript
PreferencesManager.restore(type, key);
```

#### Remove data

Remove data is pretty simple too. To remove simply call the function **remove** and pass the key do you want to remove.

```javascript
PreferencesManager.remove(key);
```

#### Utils

Use the **PreferenceType** to select what kind of type do you need. See exemple below:

```
PreferencesManager.store(PreferenceType.STRING, type, value);
```

Use the **PreferenceKey** to map your keys.

```
PreferencesManager.store(type, PreferencesKey.DEVICE_ID, value);
```

#### Supported types

Currently is supported some set of data. Below has a table of data types with respective value to pass on `functions`

Type | Type code
------------ | -------------
String | 0
Int | 1
Long | 2
Float | 3
Double | 4
Boolean | 5
Date | 6


### License

```
The MIT License (MIT)

Copyright (c) 2016 Carlos Eduardo

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```
