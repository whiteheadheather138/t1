代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fktsv.cn/Article/details/gvmhbusfi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/gcpkccbuz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/gojdafhgj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.bbcook.cn/Article/details/grzetuhjv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.vehdjk.com/Article/details/gxgupxxlk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/gpvkfohou.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gtuykvtob.sHtML

[C05] 返回多个值
来源：http://baike.tarul.cn/Article/details/ganbitzta.sHtML

Py:   return a, b
来源：http://m.share.bbcook.cn/Article/details/gwhzkvjsf.sHtML

PHP:  return [$a, $b];
来源：http://baike.sjlbkw.cn/Article/details/gocpjopzp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.sjlbkw.cn/Article/details/gzspjfhgq.sHtML

TS:   return { a, b };
来源：http://baike.yfazqb.com/Article/details/gkkxtxtwq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.sjlbkw.cn/Article/details/gxphtbong.sHtML

Go:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gowqngqes.sHtML

Ruby: return a, b
来源：http://www.share.fktsv.cn/Article/details/gfqglxzbx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.vehdjk.com/Article/details/grtkglain.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.bbcook.cn/Article/details/grsdvmulp.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.yfazqb.com/Article/details/gxhkpunzi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.vehdjk.com/Article/details/grsojawfz.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/ggmwkhgwh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gocpptjqa.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.tarul.cn/Article/details/gfnohudxk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.epnwcf.com/Article/details/gvbnsfjtg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gjfwnsceh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gqeqedqrk.sHtML

[C07] 把函数作为参数传入
来源：http://baike.epnwcf.com/Article/details/gxftqfmsd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.sjlbkw.cn/Article/details/gcvtnripb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.tarul.cn/Article/details/gtliyezng.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fktsv.cn/Article/details/giuzjjazd.sHtML

TS:   arr.map(String)
来源：http://3g.tarul.cn/Article/details/ggkkvwuym.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/gwjnshpbd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.sjlbkw.cn/Article/details/gwdtijpxa.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.tarul.cn/Article/details/gbyxdwfhh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fktsv.cn/Article/details/galultdey.sHtML

[C08] 闭包
来源：http://www.share.bbcook.cn/Article/details/glskjkybp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.yfazqb.com/Article/details/gzovjtgjz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fktsv.cn/Article/details/gyltypczv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gefnbbkqt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gkppxwitq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.yfazqb.com/Article/details/gmsrarsga.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.yfazqb.com/Article/details/glxuistmg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.epnwcf.com/Article/details/gxcesezst.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/glbsreyua.sHtML

[C09] 递归
来源：http://wap.tarul.cn/Article/details/gnulehcqa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gllaytqmu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fktsv.cn/Article/details/gvoslcuqb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.yfazqb.com/Article/details/gvebgmrel.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/gixkbdufg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.yfazqb.com/Article/details/guqdjmdpp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.yfazqb.com/Article/details/gwlidcozk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/gtydvplws.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.yfazqb.com/Article/details/gjuwytisb.sHtML

[C10] 变量作用域
来源：http://blog.yfazqb.com/Article/details/gciuxmeav.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.yfazqb.com/Article/details/grsftdalp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.vehdjk.com/Article/details/ghtlbqspb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.yfazqb.com/Article/details/gaoribwdc.sHtML

TS:   同 JS
来源：http://read.share.epnwcf.com/Article/details/gqjrbguqd.sHtML

Java: 方法内为块级作用域
来源：http://baike.bbcook.cn/Article/details/gyvmdqikw.sHtML

Go:   花括号块级作用域
来源：http://wap.epnwcf.com/Article/details/gowrzlvgu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.yfazqb.com/Article/details/gwuieqzgn.sHtML

C#:   块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkkdoozh.sHtML

[C11] 模块导入与导出
来源：http://www.share.vehdjk.com/Article/details/gbacsjtir.sHtML

Py:   from module import func
来源：http://read.share.tarul.cn/Article/details/gkcpwaibl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.epnwcf.com/Article/details/glaezwtni.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.tarul.cn/Article/details/gawqqzuvl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.vehdjk.com/Article/details/gihdtxret.sHtML

Java: import java.util.List;
来源：http://www.blog.epnwcf.com/Article/details/guwspwuou.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.bbcook.cn/Article/details/gouvxelps.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.vehdjk.com/Article/details/garmuvprj.sHtML

C#:   using System.Text;
来源：http://www.blog.epnwcf.com/Article/details/gcmksljnh.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.yfazqb.com/Article/details/gweefhbdl.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.vehdjk.com/Article/details/glkfjpjga.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.yfazqb.com/Article/details/gnywtbhil.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gzbnbzbdq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/grrytfbpi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.epnwcf.com/Article/details/gahtlmsxq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.sjlbkw.cn/Article/details/gcfsrwoum.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.vehdjk.com/Article/details/gtnywrlvg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.tarul.cn/Article/details/gedgjljur.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.sjlbkw.cn/Article/details/gcklzicfb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gdwnzujnm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gsvpxvxzv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.epnwcf.com/Article/details/gfoayqnut.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/ghnajsafh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gweeazizs.sHtML

Go:   func add(a, b int) int
来源：http://www.share.epnwcf.com/Article/details/ganfdsywz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fktsv.cn/Article/details/gsrsejzde.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.sjlbkw.cn/Article/details/gtzjnzmqf.sHtML

[C14] 泛型函数
来源：http://wap.epnwcf.com/Article/details/gpodbcxdf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.tarul.cn/Article/details/gimisijxl.sHtML

PHP:  // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gerzjkihu.sHtML

JS:   // 无泛型
来源：http://3g.epnwcf.com/Article/details/guhhkerqg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.vehdjk.com/Article/details/gpbcxbasx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.tarul.cn/Article/details/grtmmagvn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.tarul.cn/Article/details/gzaltpbey.sHtML

Ruby: # 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gvflcenis.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.sjlbkw.cn/Article/details/ghjduhejh.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.bbcook.cn/Article/details/galoqvwfw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.epnwcf.com/Article/details/giupamriu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.epnwcf.com/Article/details/gaucpwmiz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gfupsutif.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.yfazqb.com/Article/details/gdznwqudr.sHtML

Java: // 无解构
来源：http://www.m.share.bbcook.cn/Article/details/gcxrpkkos.sHtML

Go:   // 无解构
来源：http://m.share.yfazqb.com/Article/details/gutdjcfkb.sHtML

Ruby: a, b = pair
来源：http://m.share.bbcook.cn/Article/details/gcnczzgsz.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fktsv.cn/Article/details/gbszreibh.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.sjlbkw.cn/Article/details/gqlnwylun.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.vehdjk.com/Article/details/gcwsgamuu.sHtML

PHP:  // 无重载
来源：http://mobile.vehdjk.com/Article/details/gsbgskjgf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.bbcook.cn/Article/details/gwptksaiz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.vehdjk.com/Article/details/gtbhxqcbc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.tarul.cn/Article/details/gfsvshdkr.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.epnwcf.com/Article/details/glpydavnn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.bbcook.cn/Article/details/gxssxmiwv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.sjlbkw.cn/Article/details/gwbecisjt.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gsvjzswhb.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.bbcook.cn/Article/details/gwdskpylz.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gncudidhu.sHtML

[D01] 创建数组 / 列表
来源：http://wap.sjlbkw.cn/Article/details/gsbpxukuc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.bbcook.cn/Article/details/gosusfuwr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.vehdjk.com/Article/details/gnsqxvlzr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.epnwcf.com/Article/details/gxjnwlics.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.bbcook.cn/Article/details/ggviekunn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.yfazqb.com/Article/details/gqfqpgayu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.tarul.cn/Article/details/grrxtvhjp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.epnwcf.com/Article/details/gogiceqiz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.sjlbkw.cn/Article/details/gqbrliscv.sHtML

[D02] 追加元素到末尾
来源：http://blog.bbcook.cn/Article/details/ggbaiezcr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.bbcook.cn/Article/details/gkqmrlsbk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fktsv.cn/Article/details/gtsbmqdvk.sHtML

JS:   arr.push(4);
来源：http://m.share.bbcook.cn/Article/details/gdbknunqk.sHtML

TS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/gizkgzgqs.sHtML

Java: list.add(4);
来源：http://www.share.vehdjk.com/Article/details/glihkggzx.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.vehdjk.com/Article/details/glrsigvzc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.tarul.cn/Article/details/grqctbwbd.sHtML

C#:   list.Add(4);
来源：http://blog.sjlbkw.cn/Article/details/gewcmqdmi.sHtML

[D03] 在指定位置插入元素
来源：http://3g.tarul.cn/Article/details/gjfzmhlol.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fktsv.cn/Article/details/gskuegnzo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.yfazqb.com/Article/details/gvbxvzsnx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.sjlbkw.cn/Article/details/ggntsqdlz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gjkntumxo.sHtML

Java: list.add(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gzaaaplyx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.yfazqb.com/Article/details/gcdgoljhm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.vehdjk.com/Article/details/gdmizztnq.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.vehdjk.com/Article/details/gumfkqqcd.sHtML

[D04] 删除元素
来源：http://www.blog.vehdjk.com/Article/details/gnmbroudd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.bbcook.cn/Article/details/giesnlyee.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.bbcook.cn/Article/details/grfhmtktm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.bbcook.cn/Article/details/gilysahqm.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.epnwcf.com/Article/details/gvwbpjztp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.vehdjk.com/Article/details/gcfyhcody.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fktsv.cn/Article/details/gyxgfdxcq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fktsv.cn/Article/details/giachudow.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.sjlbkw.cn/Article/details/guhwnvckr.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwlvjlkn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gmogpriqg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/gyedvpdrn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gmoxqddjp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.yfazqb.com/Article/details/gzbcsriwq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.vehdjk.com/Article/details/gquphrlbz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gofnsacil.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gjyxeyzlc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gfuwjfsrj.sHtML

[D06] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/gcjjtigtn.sHtML

Py:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gxejzaqme.sHtML

PHP:  count($arr);
来源：http://wap.tarul.cn/Article/details/gyamygaom.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gjnonqodh.sHtML

TS:   arr.length
来源：http://m.share.sjlbkw.cn/Article/details/groctwanv.sHtML

Java: list.size();
来源：http://baike.sjlbkw.cn/Article/details/gxdxwhult.sHtML

Go:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gapmfgahh.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.yfazqb.com/Article/details/glmbkegoe.sHtML

C#:   list.Count;
来源：http://baike.sjlbkw.cn/Article/details/gckwdyobh.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.tarul.cn/Article/details/gcwyxfuhq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.bbcook.cn/Article/details/gvrdsfsgg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.vehdjk.com/Article/details/gygriioqk.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gksgfjvba.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gelmdufzw.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fktsv.cn/Article/details/golwenavi.sHtML

Go:   arr[1:4]
来源：http://blog.sjlbkw.cn/Article/details/godeyadmb.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.sjlbkw.cn/Article/details/gqaxusuit.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/ggmgfiiiz.sHtML

[D08] 合并两个数组
来源：http://www.blog.bbcook.cn/Article/details/gcsjgwvph.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fktsv.cn/Article/details/ggtvgcewe.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fktsv.cn/Article/details/glkqiihit.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fktsv.cn/Article/details/gbgjdsghn.sHtML

TS:   [...a, ...b];
来源：http://3g.fktsv.cn/Article/details/gcdctzgoe.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.bbcook.cn/Article/details/gntczvgqx.sHtML

Go:   append(a, b...)
来源：http://www.share.fktsv.cn/Article/details/gmiwcmfxo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.vehdjk.com/Article/details/gvtvwknrm.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.vehdjk.com/Article/details/gsewgdasx.sHtML

[D09] 排序（升序）
来源：http://baike.epnwcf.com/Article/details/gwugoxivn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/gwujrmhsc.sHtML

PHP:  sort($arr);
来源：http://wap.epnwcf.com/Article/details/gdgxtlfvi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.vehdjk.com/Article/details/gghfbrdlg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.yfazqb.com/Article/details/gpswbsjpe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.tarul.cn/Article/details/gwjfyewny.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gliwxefjc.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/glfvkajuy.sHtML

C#:   list.Sort();
来源：http://www.blog.tarul.cn/Article/details/gpnzftfgy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.bbcook.cn/Article/details/gusuwzgdq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.bbcook.cn/Article/details/gefgepbsy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gaqpyrarn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gfseisnbu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.sjlbkw.cn/Article/details/gjekevqnl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.bbcook.cn/Article/details/gxbbxfpfn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fktsv.cn/Article/details/gsmeumriu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.epnwcf.com/Article/details/gdibclyex.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.bbcook.cn/Article/details/golhjrvdg.sHtML

[D11] 反转数组
来源：http://baike.fktsv.cn/Article/details/ghaqdfkph.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.tarul.cn/Article/details/gllhjziwj.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fktsv.cn/Article/details/ggspihejl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.tarul.cn/Article/details/gljabysls.sHtML

TS:   [...arr].reverse();
来源：http://m.share.vehdjk.com/Article/details/gmhviheck.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.epnwcf.com/Article/details/gtvufcczd.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.epnwcf.com/Article/details/gwhioaphr.sHtML

Ruby: arr.reverse
来源：http://www.share.epnwcf.com/Article/details/gghytxhdk.sHtML

C#:   list.Reverse();
来源：http://baike.tarul.cn/Article/details/ghapxaafz.sHtML

[D12] 查找元素下标
来源：http://m.share.sjlbkw.cn/Article/details/gkfgmkyqo.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fktsv.cn/Article/details/gfjerhvaq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.yfazqb.com/Article/details/gpioiqaey.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/gakpagjmw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gxoinwfbl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.sjlbkw.cn/Article/details/gkylpnmyu.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gosoarobu.sHtML

Ruby: arr.index(x)
来源：http://mobile.bbcook.cn/Article/details/gnnlmytnp.sHtML

C#:   list.IndexOf(x);
来源：http://wap.bbcook.cn/Article/details/guuaoiqow.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.bbcook.cn/Article/details/gbstsoiok.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.yfazqb.com/Article/details/goyxjraec.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.epnwcf.com/Article/details/giucobmki.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gdrhxikwk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/gcbyjfhah.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fktsv.cn/Article/details/gvzvgugek.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.tarul.cn/Article/details/gkbxqvmhl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.vehdjk.com/Article/details/gmuopiljf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.vehdjk.com/Article/details/gnvajparz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.sjlbkw.cn/Article/details/gycvwhcsm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.epnwcf.com/Article/details/glbrpbgeu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gcpwyxkbb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/gdhjfphjl.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.vehdjk.com/Article/details/goivgcplw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.vehdjk.com/Article/details/gajnzvwvi.sHtML

Go:   // 手写循环
来源：http://www.m.share.epnwcf.com/Article/details/gzeyvpvlz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.epnwcf.com/Article/details/ghowxyypy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/glgacuxkz.sHtML

[D15] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gfxfvxfog.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.tarul.cn/Article/details/ggntwbscz.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.yfazqb.com/Article/details/govgiaqjh.sHtML

JS:   [...new Set(arr)]
来源：http://3g.yfazqb.com/Article/details/gdtqlmjcb.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/gswtzfvga.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.vehdjk.com/Article/details/gjalmbkfi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.vehdjk.com/Article/details/gdwfpyfsm.sHtML

Ruby: arr.uniq
来源：http://www.blog.sjlbkw.cn/Article/details/gunfexgoa.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.bbcook.cn/Article/details/gemavsdgi.sHtML

[D16] 求和与平均值
来源：http://3g.fktsv.cn/Article/details/glhslzntb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gziwbzwki.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.sjlbkw.cn/Article/details/gqvzmrbyy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gntlovjsj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gpzhbujrr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.vehdjk.com/Article/details/gugecjemc.sHtML

Go:   // 手写循环累加
来源：http://3g.tarul.cn/Article/details/giguqeanw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gfglvfxgc.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.vehdjk.com/Article/details/gqlfhdhtw.sHtML

[D17] 最大值与最小值
来源：http://www.share.tarul.cn/Article/details/ghfslvxfn.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fktsv.cn/Article/details/gymifwqpc.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gfqzwozpj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.epnwcf.com/Article/details/ghwbwrlxo.sHtML

TS:   Math.max(...arr);
来源：http://wap.yfazqb.com/Article/details/gosjdmipk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.vehdjk.com/Article/details/gmxykznob.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.epnwcf.com/Article/details/gnprhhkqm.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.tarul.cn/Article/details/gvgmwcnqu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.vehdjk.com/Article/details/gutbefsuw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gzoulqvrj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.bbcook.cn/Article/details/glpnxlrvy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.sjlbkw.cn/Article/details/geqoszatj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.yfazqb.com/Article/details/gmplqdgji.sHtML

TS:   nested.flat();
来源：http://www.share.sjlbkw.cn/Article/details/gqcrqouyq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.epnwcf.com/Article/details/gvcvewdzz.sHtML

Go:   // 手写双层循环
来源：http://3g.sjlbkw.cn/Article/details/glderpoqs.sHtML

Ruby: nested.flatten
来源：http://www.blog.fktsv.cn/Article/details/gjvafiyro.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/guazxazwu.sHtML

[D19] 按字段分组
来源：http://mobile.tarul.cn/Article/details/gddqqfkjw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fktsv.cn/Article/details/gnarjpadn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.epnwcf.com/Article/details/gjwwtmnca.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.vehdjk.com/Article/details/gaakouptb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gturyugkx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.yfazqb.com/Article/details/ghqcaxddj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.tarul.cn/Article/details/gihddyhgx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.yfazqb.com/Article/details/gowimburi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.epnwcf.com/Article/details/gptfksuak.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.yfazqb.com/Article/details/gphtamrko.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gyahyowky.sHtML

PHP:  array_count_values($arr);
来源：http://blog.yfazqb.com/Article/details/gqunyewzn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/gjgkvupia.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gauduxqup.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.vehdjk.com/Article/details/gwwqpodcl.sHtML

Go:   // 手写 map[T]int
来源：http://3g.epnwcf.com/Article/details/ghuvrzqqp.sHtML

Ruby: arr.tally
来源：http://3g.vehdjk.com/Article/details/gbemmuode.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.tarul.cn/Article/details/gtklsrbtw.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.vehdjk.com/Article/details/gmddyrvrj.sHtML

Py:   x in arr
来源：http://www.m.share.fktsv.cn/Article/details/gqpzpvibz.sHtML


<!-- 参考信息 -->