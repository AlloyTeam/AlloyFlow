# Install

```html
npm install alloyflow
```

# Usage
flow of time
```js
var alloyFlow = new AlloyFlow({
    workflow: [
        {
            work: function () { },
            start: 0
        },{
            work: function () { },
            start: 1500
        },{
            work: function () { },
            start: [720, 1000, 400, 6000]
        }
    ]
});

alloyFlow.start();
```

flow of task
```js
 var alloyFlow = new AlloyFlow({
    workflow: [
        function () {
            alloyFlow.next("msg");
        },
        function (msg) {
            alloyFlow.next("msg", 2000);
        },
        function (msg) {
            
        }
    ]
});

alloyFlow.start();
```
# Who is using AlloyFlow?

![preview](http://sqimg.qq.com/qq_product_operations/im/qqlogo/imlogo.png)

# License
This content is released under the [MIT](http://opensource.org/licenses/MIT) License.
