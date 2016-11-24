<template>
  <div id="app">
    <img src="./assets/logo.png">
    <hello></hello>
  </div>
</template>

<script>
    import Hello from './components/Hello'

    export default {
        name: 'app',
        components: {
            Hello
        },
        mounted: function() {
            //字符串拼接
            /*const first = 'Li'
            const last = 'Jinrui'
            console.log(`Your name is ${first} ${last}`)*/
            //数组
            /*const array = [1, 2, 3, 4]
            const [first, , third] = array
            console.log(first, third)*/
            //调换
            /*let a = 1;
            let b = 2;
            [a, b] = [b, a];
            console.log(a, b);*/
            //类以及类的继承
            /*class Animal {
                constructor(name) {
                    this.name = name;
                }
                speak() {
                    console.log(this.name + ' makes a noise');
                }
            }
            const animal = new Animal('animal');
            animal.speak();
            class Lion extends Animal {
                speak() {
                    super.speak();
                    console.log(this.name + ' roars');
                }
            }
            const lion = new Lion('Simba');
            lion.speak();*/
            //利用promise回调
            /*function printAfterTimeout(string, timeout) {
                return new Promise((resolve, reject) => {
                    setTimeout(function() {
                        resolve(string);
                    }, timeout);
                });
            }
            printAfterTimeout('hello ', 2e3).then((result) => {
                console.log(result);
                return printAfterTimeout(result + 'Reader', 2e3);
            }).then((result) => {
                console.log(result);
            });*/
            //默认值ES5
            /*function point(x, y, isFlag) {
                x = x || 0;
                y = y || -1;
                isFlag = isFlag || true;
                console.log(x, y, isFlag);
            }
            point(0, 0)
            point(0, 0, false)*/
            //ES6
            /*function point(x = 0, y = -1, isFlag = true) {
                console.log(x, y, isFlag);
            }
            point(0, 0)
            point(0, 0, false)
            point(1)
            point()*/
            //剩余参数
            /*function printf(format) {
                var params = [].slice.call(arguments, 1);
                console.log('params: ', params);
                console.log('format: ', format)
            }
            printf('%s %d %.2f', 'adrian', 321, Math.PI);*/
            /*function printf(format, ...params) {
                console.log('params: ', params);
                console.log('format: ', format);
            }
            printf('%s %d %.2f', 'adrian', 321, Math.PI);*/
            //展开操作符
            /*const arr1 = [1,2,3];
            const arr2 = ['a','b','c'];
            console.log([...arr1,...arr2]);*/
        }
    }
</script>

<style>
    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }
</style>