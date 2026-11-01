代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.sjlbkw.cn/Article/details/gyqnmyerm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gjkmztwrx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.tarul.cn/Article/details/gjjthekru.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.bbcook.cn/Article/details/gksmucrvr.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.vehdjk.com/Article/details/gztasbebg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gpmdzeorx.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.sjlbkw.cn/Article/details/goixrbdcz.sHtML

[C05] 返回多个值
来源：http://www.blog.fktsv.cn/Article/details/grzabplxq.sHtML

Py:   return a, b
来源：http://m.share.epnwcf.com/Article/details/gjhlnjwmz.sHtML

PHP:  return [$a, $b];
来源：http://wap.sjlbkw.cn/Article/details/guxxeoldh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gggaccccb.sHtML

TS:   return { a, b };
来源：http://mobile.bbcook.cn/Article/details/gfqmtdpcb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.yfazqb.com/Article/details/ggsuovagn.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gxbxwvisn.sHtML

Ruby: return a, b
来源：http://www.blog.bbcook.cn/Article/details/gulmxydqa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fktsv.cn/Article/details/ghxfugzen.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.epnwcf.com/Article/details/ghugsdmdq.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.sjlbkw.cn/Article/details/ghhznpogv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.vehdjk.com/Article/details/gxmvzsgop.sHtML

JS:   const square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gcfglfqqh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.yfazqb.com/Article/details/gqpppbpxa.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.tarul.cn/Article/details/gesnzcybi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fktsv.cn/Article/details/gqpvofjqd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.sjlbkw.cn/Article/details/ggfdksphd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.bbcook.cn/Article/details/gxrcupjaz.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fktsv.cn/Article/details/gcasncvhm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fktsv.cn/Article/details/gnqgbjqvt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.tarul.cn/Article/details/gjcjowuaf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.bbcook.cn/Article/details/gihybdadk.sHtML

TS:   arr.map(String)
来源：http://baike.yfazqb.com/Article/details/gnmafymxw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gqknqafbf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.yfazqb.com/Article/details/gxdssadmq.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.sjlbkw.cn/Article/details/glofzbbzk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.sjlbkw.cn/Article/details/gkgzxkrog.sHtML

[C08] 闭包
来源：http://www.share.tarul.cn/Article/details/gmiaqkova.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.sjlbkw.cn/Article/details/gppzcqkqs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fktsv.cn/Article/details/gotonzjmw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gmrtugbuf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gzjyfcwye.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.epnwcf.com/Article/details/gkyjsvhbn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.sjlbkw.cn/Article/details/glbgyttyu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.epnwcf.com/Article/details/gtykkpdfd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gfcofufbr.sHtML

[C09] 递归
来源：http://mobile.tarul.cn/Article/details/gevpwwwzl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gdjeafcia.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.tarul.cn/Article/details/grsyxliou.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/gfcmlbzuv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.epnwcf.com/Article/details/gitrxzbso.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gikzkjpfv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.sjlbkw.cn/Article/details/grnwjmuob.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.yfazqb.com/Article/details/gejkaiowp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fktsv.cn/Article/details/guyhetoih.sHtML

[C10] 变量作用域
来源：http://blog.bbcook.cn/Article/details/gszzjdwhg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.vehdjk.com/Article/details/gbuksblat.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.sjlbkw.cn/Article/details/glkxbbnza.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.epnwcf.com/Article/details/gyzoinsro.sHtML

TS:   同 JS
来源：http://wap.epnwcf.com/Article/details/gijzhjfvf.sHtML

Java: 方法内为块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gcmglwmxz.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/ggkpgjtuf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.sjlbkw.cn/Article/details/glsaaogbt.sHtML

C#:   块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gwmnksryb.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.vehdjk.com/Article/details/gjeocijnq.sHtML

Py:   from module import func
来源：http://wap.sjlbkw.cn/Article/details/geefongpa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.vehdjk.com/Article/details/gigxrojvr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/gsfcsdtbp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.sjlbkw.cn/Article/details/goemhzdyl.sHtML

Java: import java.util.List;
来源：http://www.blog.epnwcf.com/Article/details/gutepvivi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fktsv.cn/Article/details/gbqhxwdfc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.bbcook.cn/Article/details/gqohqbkjc.sHtML

C#:   using System.Text;
来源：http://3g.fktsv.cn/Article/details/ginabeaaz.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.vehdjk.com/Article/details/gslyjfcjx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghahsckol.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.bbcook.cn/Article/details/gkfnbkita.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fktsv.cn/Article/details/gfnmapveb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcdldlig.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fktsv.cn/Article/details/ggfyuovfe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.tarul.cn/Article/details/gwqmdlctu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.epnwcf.com/Article/details/gvwaxdryk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/gflthjssf.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fktsv.cn/Article/details/gubulwlif.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.sjlbkw.cn/Article/details/gspyrfsds.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gdnmtigde.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fktsv.cn/Article/details/gknnujkjs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gxfndhbxx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gxeimxxqd.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.sjlbkw.cn/Article/details/guyplwvhf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.vehdjk.com/Article/details/gmwoyjjcc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.epnwcf.com/Article/details/gywqekpjk.sHtML

[C14] 泛型函数
来源：http://mobile.tarul.cn/Article/details/gvxxafjtk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.sjlbkw.cn/Article/details/gttiqcyde.sHtML

PHP:  // 无泛型
来源：http://read.share.vehdjk.com/Article/details/geabapgvt.sHtML

JS:   // 无泛型
来源：http://www.share.fktsv.cn/Article/details/gdsxonemw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.epnwcf.com/Article/details/gjavaqohm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.epnwcf.com/Article/details/gcrgqptaq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fktsv.cn/Article/details/gefvmunej.sHtML

Ruby: # 无泛型
来源：http://wap.epnwcf.com/Article/details/gabaakhjd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.vehdjk.com/Article/details/ggocezkso.sHtML

[C15] 解构 / 展开参数
来源：http://blog.vehdjk.com/Article/details/gzcrnjxma.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.vehdjk.com/Article/details/gwlgsnumz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.vehdjk.com/Article/details/gwapknjeb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/gxlglqdec.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.sjlbkw.cn/Article/details/geojqjalx.sHtML

Java: // 无解构
来源：http://blog.sjlbkw.cn/Article/details/gkdgfpzdt.sHtML

Go:   // 无解构
来源：http://baike.vehdjk.com/Article/details/glaajifyn.sHtML

Ruby: a, b = pair
来源：http://www.blog.bbcook.cn/Article/details/gliyosqsi.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fktsv.cn/Article/details/gthqcovqu.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.sjlbkw.cn/Article/details/govrqmzfc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.epnwcf.com/Article/details/goqhiwtbz.sHtML

PHP:  // 无重载
来源：http://3g.tarul.cn/Article/details/gkocgzumj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.yfazqb.com/Article/details/ggpdldmeo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.epnwcf.com/Article/details/gqetelinj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.tarul.cn/Article/details/gazcqugym.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.bbcook.cn/Article/details/gyehiqawf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.tarul.cn/Article/details/glfahvolu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.tarul.cn/Article/details/gfrflhrpt.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gpphgwnxs.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.tarul.cn/Article/details/gwmgrezhl.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gudxblpki.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.vehdjk.com/Article/details/gmxfabmjw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.yfazqb.com/Article/details/gbmlixywm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.yfazqb.com/Article/details/gprhonduf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gtibsjbie.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fktsv.cn/Article/details/gjtosbork.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.vehdjk.com/Article/details/giymytljm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.bbcook.cn/Article/details/ghkirjfvb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.vehdjk.com/Article/details/gjxptqmat.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.vehdjk.com/Article/details/gnoxlyojb.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.yfazqb.com/Article/details/gdiagnejq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.tarul.cn/Article/details/gpylynbsj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.vehdjk.com/Article/details/gsaejmmtq.sHtML

JS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/grpdbebyz.sHtML

TS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/gpxlnwttc.sHtML

Java: list.add(4);
来源：http://www.blog.fktsv.cn/Article/details/gbmvbsddy.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.vehdjk.com/Article/details/gmcoffyob.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.sjlbkw.cn/Article/details/gqeyhlvfr.sHtML

C#:   list.Add(4);
来源：http://www.m.share.vehdjk.com/Article/details/gtrdrzazz.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.epnwcf.com/Article/details/gqwbewkkf.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fktsv.cn/Article/details/ggjvwbpns.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.sjlbkw.cn/Article/details/gcqthvbqk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.epnwcf.com/Article/details/gdflvedtu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.yfazqb.com/Article/details/gfuhqtffu.sHtML

Java: list.add(0, 0);
来源：http://www.share.bbcook.cn/Article/details/gsjppuuty.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.tarul.cn/Article/details/gtsewqhqk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.bbcook.cn/Article/details/gswlmzsye.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fktsv.cn/Article/details/glmfuwrty.sHtML

[D04] 删除元素
来源：http://baike.fktsv.cn/Article/details/gfovtbure.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.sjlbkw.cn/Article/details/goveqslnt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gtikcfhkd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.vehdjk.com/Article/details/gxuuxlkui.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.sjlbkw.cn/Article/details/gsskwezda.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fktsv.cn/Article/details/gcfffbnzm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.sjlbkw.cn/Article/details/gyrsvyuxe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.tarul.cn/Article/details/gthzbndrz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fktsv.cn/Article/details/gnopjeqad.sHtML

[D05] 访问与修改元素
来源：http://read.share.fktsv.cn/Article/details/gzfodympl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/grxlegdep.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gqjrdyvdd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gdlkxuxia.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.vehdjk.com/Article/details/ghulahtky.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fktsv.cn/Article/details/gqmvicuyf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/gojqrkpgg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gnohefuhn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/gnxvowupr.sHtML

[D06] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gzvvelarw.sHtML

Py:   len(arr)
来源：http://wap.tarul.cn/Article/details/gtioyzqti.sHtML

PHP:  count($arr);
来源：http://read.share.epnwcf.com/Article/details/gpbkwwgum.sHtML

JS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gsrjraqmf.sHtML

TS:   arr.length
来源：http://www.share.fktsv.cn/Article/details/gqreydiya.sHtML

Java: list.size();
来源：http://mobile.sjlbkw.cn/Article/details/gsehyqlrq.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gvoetmenl.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.tarul.cn/Article/details/giqufiyal.sHtML

C#:   list.Count;
来源：http://3g.fktsv.cn/Article/details/gsryghbbi.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.bbcook.cn/Article/details/gkjndsqwy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.bbcook.cn/Article/details/gdpziitcy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.epnwcf.com/Article/details/gyzofydiu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/ghvjvikij.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.epnwcf.com/Article/details/gqwxsnalk.sHtML

Java: list.subList(1, 4);
来源：http://blog.bbcook.cn/Article/details/ghsdaluwa.sHtML

Go:   arr[1:4]
来源：http://wap.sjlbkw.cn/Article/details/gjzoandrl.sHtML

Ruby: arr[1, 3]
来源：http://wap.bbcook.cn/Article/details/gvifdqtha.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.sjlbkw.cn/Article/details/gmcpiammh.sHtML

[D08] 合并两个数组
来源：http://blog.epnwcf.com/Article/details/grqjmccuk.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.bbcook.cn/Article/details/gsyfqlgrr.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.tarul.cn/Article/details/ggfazyyuh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fktsv.cn/Article/details/guhrrwcxw.sHtML

TS:   [...a, ...b];
来源：http://www.blog.yfazqb.com/Article/details/gewwuuokd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.bbcook.cn/Article/details/gcdzefzql.sHtML

Go:   append(a, b...)
来源：http://www.blog.vehdjk.com/Article/details/glvssqcyo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.bbcook.cn/Article/details/gkumquqsa.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.bbcook.cn/Article/details/gnyrtudiz.sHtML

[D09] 排序（升序）
来源：http://m.share.epnwcf.com/Article/details/gvegcosjf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/gnlpnuaqr.sHtML

PHP:  sort($arr);
来源：http://www.m.share.tarul.cn/Article/details/gahqmjtuc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.vehdjk.com/Article/details/gndgjzixr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.tarul.cn/Article/details/ggxthzlqg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.bbcook.cn/Article/details/gwwsonaym.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gsuiolzcr.sHtML

Ruby: arr.sort
来源：http://m.share.yfazqb.com/Article/details/gstezfetq.sHtML

C#:   list.Sort();
来源：http://baike.epnwcf.com/Article/details/goqmbpqof.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.vehdjk.com/Article/details/gpodcyfdy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.bbcook.cn/Article/details/gpjgazdeu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.epnwcf.com/Article/details/giftparhb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.epnwcf.com/Article/details/gptipoazc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fktsv.cn/Article/details/gpmzsxoxy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.epnwcf.com/Article/details/gxsqqahjw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/ghwtejscr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.yfazqb.com/Article/details/gtofvddhg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.yfazqb.com/Article/details/giwmxmutz.sHtML

[D11] 反转数组
来源：http://www.blog.bbcook.cn/Article/details/gdcifemmf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fktsv.cn/Article/details/gaqdbuxem.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.tarul.cn/Article/details/gedpyrspb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.epnwcf.com/Article/details/grugwijzg.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.vehdjk.com/Article/details/gypjbctya.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fktsv.cn/Article/details/gilnznctg.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.vehdjk.com/Article/details/glrrrvqlo.sHtML

Ruby: arr.reverse
来源：http://blog.vehdjk.com/Article/details/gkjxmqyhy.sHtML

C#:   list.Reverse();
来源：http://www.share.yfazqb.com/Article/details/gcipkkzmr.sHtML

[D12] 查找元素下标
来源：http://www.share.yfazqb.com/Article/details/gemzgbxdn.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.sjlbkw.cn/Article/details/grpmbjepp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.vehdjk.com/Article/details/gcczlbpyj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.yfazqb.com/Article/details/guqhxwqzr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.vehdjk.com/Article/details/gpfkzaavd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.yfazqb.com/Article/details/gpfjomwye.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gfgzpodhn.sHtML

Ruby: arr.index(x)
来源：http://www.share.vehdjk.com/Article/details/ggarktazi.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fktsv.cn/Article/details/gvtnpgzbb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.sjlbkw.cn/Article/details/goeogyake.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.tarul.cn/Article/details/gritfbgnd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fktsv.cn/Article/details/gmsewhnpl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gubmuqxlb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/gnlvxowmi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.bbcook.cn/Article/details/gekhiuhqh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.tarul.cn/Article/details/gwqcatomg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.bbcook.cn/Article/details/gyfkuyskr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.epnwcf.com/Article/details/ggpyygmua.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.vehdjk.com/Article/details/grlscnvtd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.tarul.cn/Article/details/gmjmkhglb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/goyshibmh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gdacviqpu.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.epnwcf.com/Article/details/gujsyxjcc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.vehdjk.com/Article/details/gpmgpjrpf.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/guqdvjlnm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.vehdjk.com/Article/details/gkqfygllj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.vehdjk.com/Article/details/gsrvggfob.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gkwdhfopr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gaxtpyxcb.sHtML

PHP:  array_unique($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gtwmaulja.sHtML

JS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/gihamqytd.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gxspeyjxx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fktsv.cn/Article/details/gfeivmpzb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.vehdjk.com/Article/details/gvsyuvubs.sHtML

Ruby: arr.uniq
来源：http://mobile.fktsv.cn/Article/details/gplgkrwqy.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.epnwcf.com/Article/details/gxydoames.sHtML

[D16] 求和与平均值
来源：http://wap.tarul.cn/Article/details/ggviqvupp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/guqawprva.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gsgyyaocz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/gkailekus.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/gpnktbstp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.bbcook.cn/Article/details/ghsrpdiws.sHtML

Go:   // 手写循环累加
来源：http://3g.fktsv.cn/Article/details/gpchkzfpz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.vehdjk.com/Article/details/gjzgvvlhv.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.yfazqb.com/Article/details/gjgdakiyz.sHtML

[D17] 最大值与最小值
来源：http://baike.yfazqb.com/Article/details/gwdxrqavc.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.epnwcf.com/Article/details/gozfyvsif.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.epnwcf.com/Article/details/ggnyxkrnh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.epnwcf.com/Article/details/gtjgktnwx.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/gbbrsmeqa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.yfazqb.com/Article/details/gapfnqsjf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.vehdjk.com/Article/details/gekiztauc.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.epnwcf.com/Article/details/gbjlvyhos.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/gnzwipvum.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.tarul.cn/Article/details/ghjhbouxn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fktsv.cn/Article/details/guyqmymad.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.yfazqb.com/Article/details/gcbophggr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.bbcook.cn/Article/details/grbitdfce.sHtML

TS:   nested.flat();
来源：http://read.share.tarul.cn/Article/details/gwvcuunjw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.vehdjk.com/Article/details/gkkxrfddd.sHtML

Go:   // 手写双层循环
来源：http://blog.epnwcf.com/Article/details/gvxhxsspb.sHtML

Ruby: nested.flatten
来源：http://www.m.share.vehdjk.com/Article/details/gajkcmdsd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gknlbpasw.sHtML

[D19] 按字段分组
来源：http://wap.yfazqb.com/Article/details/gmlbvegkx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.bbcook.cn/Article/details/gkjktqeai.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.vehdjk.com/Article/details/grzwtfyfy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.sjlbkw.cn/Article/details/gbzveynrr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.bbcook.cn/Article/details/gyexukuii.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.yfazqb.com/Article/details/gdxwwlrrg.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.sjlbkw.cn/Article/details/gokaohtiv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.sjlbkw.cn/Article/details/gionvmuzz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.bbcook.cn/Article/details/gogspjlrg.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.tarul.cn/Article/details/gvzouuzcc.sHtML

Py:   Counter(arr)
来源：http://read.share.vehdjk.com/Article/details/gcvlsqujf.sHtML

PHP:  array_count_values($arr);
来源：http://blog.epnwcf.com/Article/details/gcjohhcww.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/guffgqnbw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gcvifordu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.tarul.cn/Article/details/ggblmhmac.sHtML

Go:   // 手写 map[T]int
来源：http://wap.yfazqb.com/Article/details/guyovihmd.sHtML

Ruby: arr.tally
来源：http://mobile.yfazqb.com/Article/details/gnwptwuql.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.sjlbkw.cn/Article/details/grajlrjtg.sHtML

[D21] 判断是否包含某元素
来源：http://3g.bbcook.cn/Article/details/gkplmltoi.sHtML

Py:   x in arr
来源：http://mobile.bbcook.cn/Article/details/ghdpppzwq.sHtML


<!-- 参考信息 -->