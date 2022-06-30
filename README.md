# test.//error
//Syntax error - нарушение правил языка
// "console,log"

//Reference error- неправильное имя
//abc(){...}- true;adc()
//

// Type Error - путать одно с другим
// let b = 0;

// РЕКУРСИЯ
// ТРЕБОВАНИЯ К РЕКУРСИИ:
// 1. БАЗОВЫЙ СЛУЧАЙ - ТОЧКА В КОТОР НАДО ОСТАНОВИТЬСЯ
// 2. ПРАВИЛО ДЛЯ УГЛУБЛЕНИЯ
//Общее количество вложенных вызовов (включая первый) называют глубиной рекурсии. В нашем случае она будет равна n.
//
function pow(x, y) {
   if(y === 0) return 1
   return x * pow(x,y -1 )
}
const res = pow(4,5)
//console.log(res)

let t = 0
function sum() {
    t++;
  //  console.log(t);
    if(t>=10) return;
    sum();
}
sum();
// циклы аналог екурсии
// function f2() {
//     let o = ''
//     for(let i= 0; i<=30;i++) {
//         o+= i + ' '
//     }
//     console.log(o)

// }
// f2()
// //
// let i = 0;
// let out = ''
// function f3() {
//     i++
//     out+= i + ' ';
//     if(i>=30) return
//     f3()
// }
// f3()
// console.log(out)

//

//////////////////////////
let s = 1
function fd(n) {
    if(n === 0) return
    s= s*n
    fd(n-1)
    return s
}

console.log(fd(6))
