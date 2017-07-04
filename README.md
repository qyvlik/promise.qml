# promise.qml

A port of promise to QML, just warp from [then/promise](https://github.com/then/promise)

## how to use

```
import QtQuick 2.8

import promise 1.0           // for import PromiseLib

Item {
    id: app

    Component.onCompleted: {
        var Promise = PromiseLib.Promise;
        new Promise(function(resolve, reject){
            console.log("here is promise!");
            resolve("good");
        }).then(function(value){
            console.log("value:", value);
        });
    }
}
```


