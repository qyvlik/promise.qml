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

## >= Qt5.12 support `Promise`

Qt5.12 or later support `Promise`, see here [New_Features_in_Qt_5.12#The JavaScript engine now supports ECMAScript 7](https://wiki.qt.io/New_Features_in_Qt_5.12)

[【译】ECMAScript 2016 (ES7) 新特性一览](https://www.w3ctech.com/topic/1614)


