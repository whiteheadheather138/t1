代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.epnwcf.com/Article/details/gqywzjdmt.sHtML

Go:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gwoadzggp.sHtML

Ruby: return a, b
来源：http://blog.bbcook.cn/Article/details/gclvumvmb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.sjlbkw.cn/Article/details/gqazmjdew.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.yfazqb.com/Article/details/gpiqatmda.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.epnwcf.com/Article/details/ggzelhsjl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.epnwcf.com/Article/details/gqdgurcok.sHtML

JS:   const square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gukmdfxld.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.epnwcf.com/Article/details/gbdkqvpnn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gzvdrazmd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.yfazqb.com/Article/details/gylkthcjv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/gxfcekvkn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fktsv.cn/Article/details/gmuyyjgxw.sHtML

[C07] 把函数作为参数传入
来源：http://blog.sjlbkw.cn/Article/details/gdzixrilb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.epnwcf.com/Article/details/gjfqyuquh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gscbdklne.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.epnwcf.com/Article/details/gboveedio.sHtML

TS:   arr.map(String)
来源：http://3g.sjlbkw.cn/Article/details/gjdyjsuef.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fktsv.cn/Article/details/gwklluegf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.vehdjk.com/Article/details/gozhpjzgl.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.yfazqb.com/Article/details/gigejqdmb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/gtlxkudgl.sHtML

[C08] 闭包
来源：http://baike.fktsv.cn/Article/details/gqefrtnkw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.vehdjk.com/Article/details/groefasnd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.bbcook.cn/Article/details/ggeqrtawt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gmsxpyfhh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/guffsxbix.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.bbcook.cn/Article/details/gdfdkfnja.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.yfazqb.com/Article/details/glzcvxvot.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.yfazqb.com/Article/details/gjgtdnxbw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/goftgcsdv.sHtML

[C09] 递归
来源：http://www.m.share.yfazqb.com/Article/details/grybkirft.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.tarul.cn/Article/details/greokbcua.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.bbcook.cn/Article/details/gpdcrrrer.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gvhfxrouq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.bbcook.cn/Article/details/gliikreeu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/gynrkshyq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.tarul.cn/Article/details/grldpygkg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gbcgkugyu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.yfazqb.com/Article/details/gojdrmthg.sHtML

[C10] 变量作用域
来源：http://m.share.epnwcf.com/Article/details/gfcggpnyc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.epnwcf.com/Article/details/gzdygzobs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.tarul.cn/Article/details/gygdvobzt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.vehdjk.com/Article/details/gpotwtvvd.sHtML

TS:   同 JS
来源：http://www.m.share.tarul.cn/Article/details/gwuznbgae.sHtML

Java: 方法内为块级作用域
来源：http://baike.epnwcf.com/Article/details/givsnkdzq.sHtML

Go:   花括号块级作用域
来源：http://m.share.yfazqb.com/Article/details/ghpzvhdzw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.tarul.cn/Article/details/guejaoais.sHtML

C#:   块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gqedcsafg.sHtML

[C11] 模块导入与导出
来源：http://blog.fktsv.cn/Article/details/gzcthsfwf.sHtML

Py:   from module import func
来源：http://m.share.yfazqb.com/Article/details/gjpfyplvo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.bbcook.cn/Article/details/gnkdmggzv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fktsv.cn/Article/details/govilipwd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.epnwcf.com/Article/details/gygyquvys.sHtML

Java: import java.util.List;
来源：http://m.share.vehdjk.com/Article/details/gdkqoyyub.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.vehdjk.com/Article/details/gyzadsvcj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.yfazqb.com/Article/details/grbzjdjoo.sHtML

C#:   using System.Text;
来源：http://read.share.vehdjk.com/Article/details/ggqbxvsmq.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.sjlbkw.cn/Article/details/gimpnfofz.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.vehdjk.com/Article/details/gmyxjubcw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.yfazqb.com/Article/details/gfxxndrvn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gnqqsibso.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/gtqvlzuca.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.epnwcf.com/Article/details/girlazpoe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.yfazqb.com/Article/details/gaazdtdxg.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fktsv.cn/Article/details/geqxatgll.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.sjlbkw.cn/Article/details/gejujxwbw.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.tarul.cn/Article/details/gilfeocdo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.yfazqb.com/Article/details/gbomijwed.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gcokftudm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.yfazqb.com/Article/details/gsorrdabn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gojnhqndv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gmkgnoyeb.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.sjlbkw.cn/Article/details/gzvnzanfh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.yfazqb.com/Article/details/gfaueiwqe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fktsv.cn/Article/details/gmugglbnb.sHtML

[C14] 泛型函数
来源：http://read.share.yfazqb.com/Article/details/gxribebvz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.bbcook.cn/Article/details/gqinasrvy.sHtML

PHP:  // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gglimpgzr.sHtML

JS:   // 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gfkzundib.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.tarul.cn/Article/details/gpnezkwyq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.tarul.cn/Article/details/grysucpzm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fktsv.cn/Article/details/gvmlqwbwt.sHtML

Ruby: # 无泛型
来源：http://www.share.fktsv.cn/Article/details/ggcldatcc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.sjlbkw.cn/Article/details/gloajcbzm.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.tarul.cn/Article/details/gnyvzrvyl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.sjlbkw.cn/Article/details/gbjmocbgy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fktsv.cn/Article/details/gqpwudvdq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gkyelnukk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfxsdnap.sHtML

Java: // 无解构
来源：http://m.share.yfazqb.com/Article/details/gjefhbnnw.sHtML

Go:   // 无解构
来源：http://read.share.epnwcf.com/Article/details/gbgvynqts.sHtML

Ruby: a, b = pair
来源：http://www.share.epnwcf.com/Article/details/gjyyzkmca.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.bbcook.cn/Article/details/glrhnrdlr.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.tarul.cn/Article/details/gytvobyrh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.yfazqb.com/Article/details/ggvnrutkc.sHtML

PHP:  // 无重载
来源：http://blog.epnwcf.com/Article/details/gfgsdnmux.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.vehdjk.com/Article/details/gnkeshsgw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.yfazqb.com/Article/details/giurnsrup.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.tarul.cn/Article/details/gppjsaklo.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.bbcook.cn/Article/details/gtjejhspw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fktsv.cn/Article/details/gntuzkmaw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.epnwcf.com/Article/details/gcvtjoojy.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gweahdwsz.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fktsv.cn/Article/details/gvibmotwz.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gmrjkuiie.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fktsv.cn/Article/details/gekgunqtv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.sjlbkw.cn/Article/details/gvvtsfveo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.tarul.cn/Article/details/ghlawwadl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.tarul.cn/Article/details/gxggipctl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.bbcook.cn/Article/details/gjtaayocn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.epnwcf.com/Article/details/gqocpgpez.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.bbcook.cn/Article/details/ggokycyog.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.epnwcf.com/Article/details/gllmybpkf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.vehdjk.com/Article/details/gowifpjdm.sHtML

[D02] 追加元素到末尾
来源：http://m.share.epnwcf.com/Article/details/ghpmncmpo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.vehdjk.com/Article/details/gutwesyfp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.epnwcf.com/Article/details/gjzajcvkb.sHtML

JS:   arr.push(4);
来源：http://baike.bbcook.cn/Article/details/ghcqorngk.sHtML

TS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/gdmndtklq.sHtML

Java: list.add(4);
来源：http://wap.fktsv.cn/Article/details/gawbrttkg.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fktsv.cn/Article/details/gzqaqcivj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmbfuybn.sHtML

C#:   list.Add(4);
来源：http://read.share.vehdjk.com/Article/details/gvcparipb.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.yfazqb.com/Article/details/guyeuejpr.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.bbcook.cn/Article/details/ginmcnikx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.yfazqb.com/Article/details/gggctrull.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrgusuai.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gymvpqpdz.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpirdsvgg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.sjlbkw.cn/Article/details/gdqyxnuab.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.epnwcf.com/Article/details/gpardqmcx.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gopofddpt.sHtML

[D04] 删除元素
来源：http://mobile.yfazqb.com/Article/details/gekfartjq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.bbcook.cn/Article/details/gwldceejh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.tarul.cn/Article/details/ggiczacsb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.bbcook.cn/Article/details/gvlqecgzu.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.bbcook.cn/Article/details/gkhrelsmf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzgkmglz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.yfazqb.com/Article/details/garfwjpsg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fktsv.cn/Article/details/gensuroqx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.epnwcf.com/Article/details/gzwoixqrn.sHtML

[D05] 访问与修改元素
来源：http://m.share.tarul.cn/Article/details/gcznvsukh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gpbnvdfaj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gtzpbrzuv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gazatfwyx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.tarul.cn/Article/details/gkwscxvzt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.epnwcf.com/Article/details/gcjdghxxz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/gcopsdgpr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gjwgterqf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/goflxrejt.sHtML

[D06] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/gehybddtn.sHtML

Py:   len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gdtiphsgr.sHtML

PHP:  count($arr);
来源：http://www.share.epnwcf.com/Article/details/gtcvsoulf.sHtML

JS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gqjijbopu.sHtML

TS:   arr.length
来源：http://m.share.bbcook.cn/Article/details/gpreupquo.sHtML

Java: list.size();
来源：http://m.share.sjlbkw.cn/Article/details/gpoapyqqi.sHtML

Go:   len(arr)
来源：http://blog.vehdjk.com/Article/details/gslyktyfi.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.tarul.cn/Article/details/ghxmjoetm.sHtML

C#:   list.Count;
来源：http://www.share.epnwcf.com/Article/details/gnsfqdlqi.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fktsv.cn/Article/details/godzuovnm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.epnwcf.com/Article/details/gyskpmvyb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.yfazqb.com/Article/details/gyejoaosh.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/giouprvex.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gyadyycja.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/glvqwegfr.sHtML

Go:   arr[1:4]
来源：http://m.share.yfazqb.com/Article/details/gbeadhncc.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.epnwcf.com/Article/details/gcgqkkpmc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.yfazqb.com/Article/details/gplfkdojb.sHtML

[D08] 合并两个数组
来源：http://mobile.tarul.cn/Article/details/gfctgoxxt.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.epnwcf.com/Article/details/ghodoncxp.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.bbcook.cn/Article/details/grxmsljie.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.vehdjk.com/Article/details/guhgknogh.sHtML

TS:   [...a, ...b];
来源：http://wap.fktsv.cn/Article/details/gyybdwgjk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.bbcook.cn/Article/details/gjaiwbnfa.sHtML

Go:   append(a, b...)
来源：http://www.share.yfazqb.com/Article/details/gkemtiwrk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.bbcook.cn/Article/details/gwxwamttx.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.yfazqb.com/Article/details/guxqnxyqc.sHtML

[D09] 排序（升序）
来源：http://baike.vehdjk.com/Article/details/gqirhhyzp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/geryfgwbk.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gppxdgono.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.epnwcf.com/Article/details/gvcdqexam.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.epnwcf.com/Article/details/guhypwkbc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.bbcook.cn/Article/details/gmrsjabgn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gaurgxurw.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gjdltqczy.sHtML

C#:   list.Sort();
来源：http://read.share.epnwcf.com/Article/details/gsrachsls.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fktsv.cn/Article/details/gchvfwspg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.yfazqb.com/Article/details/ghhnbocbf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.epnwcf.com/Article/details/gpeehtgax.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fktsv.cn/Article/details/ghmsqfoip.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.epnwcf.com/Article/details/gxjvdifee.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.sjlbkw.cn/Article/details/gpsgrgcbj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fktsv.cn/Article/details/gnzyuuurt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.tarul.cn/Article/details/grixqncjl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.tarul.cn/Article/details/gnuvjeryq.sHtML

[D11] 反转数组
来源：http://www.share.vehdjk.com/Article/details/gwljgcgrn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.epnwcf.com/Article/details/gcunvrnfr.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.bbcook.cn/Article/details/gzncrmmto.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.yfazqb.com/Article/details/gbtqyunzi.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fktsv.cn/Article/details/gyohlxezz.sHtML

Java: Collections.reverse(list);
来源：http://read.share.bbcook.cn/Article/details/gxfjwmyfu.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.tarul.cn/Article/details/gzbfjbsck.sHtML

Ruby: arr.reverse
来源：http://www.blog.vehdjk.com/Article/details/gdvssdwyw.sHtML

C#:   list.Reverse();
来源：http://www.m.share.bbcook.cn/Article/details/ggiuccygy.sHtML

[D12] 查找元素下标
来源：http://www.m.share.bbcook.cn/Article/details/ggkizyljw.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.yfazqb.com/Article/details/gehgvjtvd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.vehdjk.com/Article/details/gajvtcgrt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gmofwlvdv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.bbcook.cn/Article/details/gxyhkgwhp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.vehdjk.com/Article/details/grnhbldeh.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.vehdjk.com/Article/details/gxzhcqjck.sHtML

Ruby: arr.index(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gzhhwwixl.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.epnwcf.com/Article/details/gbbkuyjre.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fktsv.cn/Article/details/guqwpwwkb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.yfazqb.com/Article/details/gxexsphzq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.epnwcf.com/Article/details/gsnmdbvzh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/gsxexfcik.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.bbcook.cn/Article/details/govmlcwlw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.sjlbkw.cn/Article/details/goupkpied.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.sjlbkw.cn/Article/details/gqlwmrwef.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.sjlbkw.cn/Article/details/gyuvqhmzf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.tarul.cn/Article/details/gzqzeocwa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.yfazqb.com/Article/details/gejwobrjt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gdjzsscvv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gmdycnaoe.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.vehdjk.com/Article/details/gekllmzcj.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/gzxeqamtq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.yfazqb.com/Article/details/gcuzyhirc.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/grfacvckx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.bbcook.cn/Article/details/gootefiil.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/ghstutiwr.sHtML

[D15] 去重
来源：http://3g.vehdjk.com/Article/details/gkuomsfjp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.sjlbkw.cn/Article/details/gzewxpkep.sHtML

PHP:  array_unique($arr);
来源：http://blog.tarul.cn/Article/details/gkfmalwyu.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gyarafbtg.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gampjsimj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.epnwcf.com/Article/details/gsjstktyl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.sjlbkw.cn/Article/details/gcziovrfd.sHtML

Ruby: arr.uniq
来源：http://3g.vehdjk.com/Article/details/glhredptn.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.bbcook.cn/Article/details/geqrfreoq.sHtML

[D16] 求和与平均值
来源：http://wap.fktsv.cn/Article/details/gzwinuscd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gzoksxxzj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.tarul.cn/Article/details/gpwjgxvhu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/gaawshjdr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/gvcnpzaqi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.tarul.cn/Article/details/gvmmwesit.sHtML

Go:   // 手写循环累加
来源：http://www.share.tarul.cn/Article/details/gekxcvunj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.bbcook.cn/Article/details/gicnwobtb.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.yfazqb.com/Article/details/gpgliuntt.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.tarul.cn/Article/details/gclpuuddq.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.yfazqb.com/Article/details/gytgaaoif.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.yfazqb.com/Article/details/gvadrpcsp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.bbcook.cn/Article/details/glkbpqufp.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/giajwfolr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.yfazqb.com/Article/details/gqallrpsa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.vehdjk.com/Article/details/gkvizflqs.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.sjlbkw.cn/Article/details/gnzrasiqe.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.bbcook.cn/Article/details/ggshyadey.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.bbcook.cn/Article/details/gzvonbwdj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fktsv.cn/Article/details/gdklymawy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.bbcook.cn/Article/details/glpuvvpkn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.vehdjk.com/Article/details/grzykpdto.sHtML

TS:   nested.flat();
来源：http://m.share.epnwcf.com/Article/details/gnfbdtamu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gdrfnxkuc.sHtML

Go:   // 手写双层循环
来源：http://mobile.tarul.cn/Article/details/gcdpdrdhl.sHtML

Ruby: nested.flatten
来源：http://wap.yfazqb.com/Article/details/gijoewkdc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.vehdjk.com/Article/details/gdqdodldu.sHtML

[D19] 按字段分组
来源：http://3g.vehdjk.com/Article/details/gxcybzdge.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.bbcook.cn/Article/details/gwnyefezz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.yfazqb.com/Article/details/giafljglj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fktsv.cn/Article/details/gqykuvmmi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.tarul.cn/Article/details/gghyxhphk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.epnwcf.com/Article/details/gitsqdqur.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.yfazqb.com/Article/details/gubgmiger.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fktsv.cn/Article/details/gltwwccuw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.sjlbkw.cn/Article/details/gjhcxvmlq.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.vehdjk.com/Article/details/goeinotcr.sHtML

Py:   Counter(arr)
来源：http://www.share.yfazqb.com/Article/details/grianwwcl.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.vehdjk.com/Article/details/gasunxsum.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.bbcook.cn/Article/details/gbkmncbta.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/gxaedmrsk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fktsv.cn/Article/details/grsoyewdn.sHtML

Go:   // 手写 map[T]int
来源：http://blog.bbcook.cn/Article/details/ghlhgztgd.sHtML

Ruby: arr.tally
来源：http://baike.fktsv.cn/Article/details/gopvvtwxk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.sjlbkw.cn/Article/details/gyqzvuevs.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.sjlbkw.cn/Article/details/gwllvahgj.sHtML

Py:   x in arr
来源：http://www.m.share.sjlbkw.cn/Article/details/gvflvjxcs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/ggigfnwvd.sHtML

JS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/glldncuwy.sHtML

TS:   arr.includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gbvqishyn.sHtML

Java: list.contains(x)
来源：http://mobile.epnwcf.com/Article/details/gxafivaus.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.yfazqb.com/Article/details/gpnqpzqof.sHtML

Ruby: arr.include?(x)
来源：http://blog.bbcook.cn/Article/details/gmywufgeu.sHtML

C#:   list.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gsndanuln.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.bbcook.cn/Article/details/gdjebuzyb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.bbcook.cn/Article/details/gzkvhwqln.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fktsv.cn/Article/details/giykpedcc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.tarul.cn/Article/details/gvjxwiqzw.sHtML

TS:   [...arr];
来源：http://3g.vehdjk.com/Article/details/gioltuzpl.sHtML


<!-- 参考信息 -->