代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fktsv.cn/Article/details/grrvnvpui.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.yfazqb.com/Article/details/gqprdkfoe.sHtML

[B15] 布尔运算与取反
来源：http://read.share.bbcook.cn/Article/details/gugcmmahv.sHtML

Py:   a and b or not c
来源：http://www.blog.fktsv.cn/Article/details/gktxbmqnm.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.tarul.cn/Article/details/ggvxcscyl.sHtML

JS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gqgadexvd.sHtML

TS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gmgfspnlb.sHtML

Java: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gbpokjthu.sHtML

Go:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gkuszomck.sHtML

Ruby: a && b || !c
来源：http://blog.epnwcf.com/Article/details/gnidzdken.sHtML

C#:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gftgncqej.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.sjlbkw.cn/Article/details/gosxumqyl.sHtML

Py:   if not data: return
来源：http://wap.vehdjk.com/Article/details/gxjqxcffg.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.sjlbkw.cn/Article/details/gvtykwbih.sHtML

JS:   if (!data) return;
来源：http://blog.sjlbkw.cn/Article/details/gnwclicgt.sHtML

TS:   if (!data) return;
来源：http://www.blog.epnwcf.com/Article/details/gcookfczw.sHtML

Java: if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gcgujglou.sHtML

Go:   if data == nil { return }
来源：http://blog.sjlbkw.cn/Article/details/gxigkhffy.sHtML

Ruby: return if data.nil?
来源：http://wap.bbcook.cn/Article/details/gghececgt.sHtML

C#:   if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/grxbhrgjy.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gecfeolvb.sHtML

C. 函数与作用域
来源：http://baike.fktsv.cn/Article/details/gbuuldshc.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gasnxycov.sHtML

[C01] 定义函数
来源：http://read.share.yfazqb.com/Article/details/gflcldlie.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.vehdjk.com/Article/details/gqudidlby.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gvqkysaqh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gjwiabnyy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/gkmjublcg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gtpowotsd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.tarul.cn/Article/details/gsngdsefv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gawwxcvrw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gkeyaoojn.sHtML

[C02] 默认参数
来源：http://read.share.vehdjk.com/Article/details/grdhkqujs.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.tarul.cn/Article/details/gioklhysb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.yfazqb.com/Article/details/gzkysufei.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/gerfyqisx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/guzehoviv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.vehdjk.com/Article/details/gqaxyzmks.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.tarul.cn/Article/details/gvryalgtu.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.epnwcf.com/Article/details/gsbzemmmq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.yfazqb.com/Article/details/gmccteopj.sHtML

[C03] 可变参数
来源：http://wap.sjlbkw.cn/Article/details/gfweqaiia.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.tarul.cn/Article/details/gzpkqkgbl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.vehdjk.com/Article/details/gxuqbxuzz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gtqaxhmnu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/gduetzlgc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.yfazqb.com/Article/details/gfvigrmon.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.sjlbkw.cn/Article/details/gjztokhln.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fktsv.cn/Article/details/gjmxzrjpy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.sjlbkw.cn/Article/details/gmvpspyhi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.vehdjk.com/Article/details/gifaqpkyv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fktsv.cn/Article/details/glskmtroq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.tarul.cn/Article/details/gbpnjndaa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/gkwzmyoll.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fktsv.cn/Article/details/gktjlrkko.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.yfazqb.com/Article/details/gtdcbekxu.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.bbcook.cn/Article/details/gpqulefpk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gmvdnygat.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gtkolsnes.sHtML

[C05] 返回多个值
来源：http://www.share.bbcook.cn/Article/details/gsnoxpdix.sHtML

Py:   return a, b
来源：http://baike.epnwcf.com/Article/details/gijgjwnwt.sHtML

PHP:  return [$a, $b];
来源：http://mobile.tarul.cn/Article/details/gwnzzhbjp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gmwarbihj.sHtML

TS:   return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gqvcxybow.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.tarul.cn/Article/details/guknntjjz.sHtML

Go:   return a, b
来源：http://blog.vehdjk.com/Article/details/gtunnzpdq.sHtML

Ruby: return a, b
来源：http://www.share.sjlbkw.cn/Article/details/gebnmovtp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.yfazqb.com/Article/details/gsttmvicc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsgupgvq.sHtML

Py:   square = lambda x: x * x
来源：http://wap.yfazqb.com/Article/details/gwjljjdwe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.yfazqb.com/Article/details/ghyewxcbj.sHtML

JS:   const square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gdiixzxpp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fktsv.cn/Article/details/gguiwpefw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/gzhxognyf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.epnwcf.com/Article/details/gaizuxbod.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.tarul.cn/Article/details/gyjfctemz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fktsv.cn/Article/details/gxfisdgok.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.sjlbkw.cn/Article/details/gwikhskcx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.epnwcf.com/Article/details/gldtlymiv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.epnwcf.com/Article/details/gxjcyykzs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.yfazqb.com/Article/details/gwoeohufe.sHtML

TS:   arr.map(String)
来源：http://wap.tarul.cn/Article/details/gbhqhdttp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fktsv.cn/Article/details/gavairsix.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.tarul.cn/Article/details/gpjogybmd.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.epnwcf.com/Article/details/gpahqoctl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.yfazqb.com/Article/details/gkgswupax.sHtML

[C08] 闭包
来源：http://www.share.bbcook.cn/Article/details/gqroysxel.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.yfazqb.com/Article/details/gpcjorakf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.yfazqb.com/Article/details/gdmvlwilw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gawdhrwlr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gpdrsqaez.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.epnwcf.com/Article/details/gxevxexbp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fktsv.cn/Article/details/gqwfmdaqb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.tarul.cn/Article/details/gxgewjprz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.bbcook.cn/Article/details/guqegyjcv.sHtML

[C09] 递归
来源：http://m.share.fktsv.cn/Article/details/gjpluvdkx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gqptdaoac.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fktsv.cn/Article/details/gfsquhxnl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.epnwcf.com/Article/details/gmdiynadk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.yfazqb.com/Article/details/ggkrxjyhb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.tarul.cn/Article/details/gfmmpitcc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.sjlbkw.cn/Article/details/gpefczczk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/gizgkiyph.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.vehdjk.com/Article/details/gjitpcnbh.sHtML

[C10] 变量作用域
来源：http://blog.yfazqb.com/Article/details/gfaalqnpi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.bbcook.cn/Article/details/glvvybtgc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.bbcook.cn/Article/details/gataxtpiu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.yfazqb.com/Article/details/gvdblimmx.sHtML

TS:   同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gucfplsji.sHtML

Java: 方法内为块级作用域
来源：http://blog.yfazqb.com/Article/details/gvxmhzabo.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fktsv.cn/Article/details/grxfnwvdr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.epnwcf.com/Article/details/gmqvzoiot.sHtML

C#:   块级作用域
来源：http://baike.yfazqb.com/Article/details/gynmyobbi.sHtML

[C11] 模块导入与导出
来源：http://blog.fktsv.cn/Article/details/geldugjtb.sHtML

Py:   from module import func
来源：http://3g.yfazqb.com/Article/details/gifbcrmip.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.tarul.cn/Article/details/gznapjgcl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.tarul.cn/Article/details/gpaangqgm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.tarul.cn/Article/details/goueyrfof.sHtML

Java: import java.util.List;
来源：http://www.blog.vehdjk.com/Article/details/guzgepwuv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fktsv.cn/Article/details/gunbmmalf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fktsv.cn/Article/details/gmtidkhsk.sHtML

C#:   using System.Text;
来源：http://read.share.tarul.cn/Article/details/gzvcpauee.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.bbcook.cn/Article/details/gieolabtf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.epnwcf.com/Article/details/gcohwpdra.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.vehdjk.com/Article/details/gyyndoxof.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.bbcook.cn/Article/details/grxysczje.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.epnwcf.com/Article/details/gceufvhsa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.epnwcf.com/Article/details/ghexxudpc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/ggygftgsz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.sjlbkw.cn/Article/details/ggnituvwl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fktsv.cn/Article/details/gersrlzym.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.bbcook.cn/Article/details/gkatjhyet.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.sjlbkw.cn/Article/details/gnfvwzsak.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/glykhmfqn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.bbcook.cn/Article/details/gxjpboabz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/glwtpvckp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gyduiqcjx.sHtML

Go:   func add(a, b int) int
来源：http://read.share.bbcook.cn/Article/details/garwxctpw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.epnwcf.com/Article/details/gopfzfgug.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.vehdjk.com/Article/details/gehxpfysj.sHtML

[C14] 泛型函数
来源：http://www.share.bbcook.cn/Article/details/gpgwanayc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.tarul.cn/Article/details/goumuprtk.sHtML

PHP:  // 无泛型
来源：http://wap.epnwcf.com/Article/details/gzgqbcvzs.sHtML

JS:   // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/guwwykzoh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fktsv.cn/Article/details/gbuegmnzk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.yfazqb.com/Article/details/gxjbhdgpy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.sjlbkw.cn/Article/details/gjjsxpkqr.sHtML

Ruby: # 无泛型
来源：http://www.blog.epnwcf.com/Article/details/giimdlpab.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.bbcook.cn/Article/details/gjyttwckk.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.vehdjk.com/Article/details/ggpljgzwt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.sjlbkw.cn/Article/details/gkzvktdlk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.vehdjk.com/Article/details/ganycvook.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/gzlxyiumk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.yfazqb.com/Article/details/ggzbalvly.sHtML

Java: // 无解构
来源：http://3g.epnwcf.com/Article/details/gxsbmdwsz.sHtML

Go:   // 无解构
来源：http://read.share.fktsv.cn/Article/details/gnvzmtypm.sHtML

Ruby: a, b = pair
来源：http://blog.yfazqb.com/Article/details/gccnjmgai.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fktsv.cn/Article/details/gbilysvdg.sHtML

[C16] 函数 / 方法重载
来源：http://baike.yfazqb.com/Article/details/gjthmdfak.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fktsv.cn/Article/details/gmabnpsyh.sHtML

PHP:  // 无重载
来源：http://www.blog.sjlbkw.cn/Article/details/goiioagpk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.vehdjk.com/Article/details/gkearyvnx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.sjlbkw.cn/Article/details/gderqpphq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fktsv.cn/Article/details/gelhecles.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.epnwcf.com/Article/details/gctckozpl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.bbcook.cn/Article/details/gjluempvb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.sjlbkw.cn/Article/details/gplixgvky.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gayelekmm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.sjlbkw.cn/Article/details/gjhooipwf.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gnkueulbm.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/guzmgtbde.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.vehdjk.com/Article/details/gmsfaxkfv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.bbcook.cn/Article/details/gafnpciwm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.bbcook.cn/Article/details/ginjlakzh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fktsv.cn/Article/details/gpkuojptr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.yfazqb.com/Article/details/gwdtdykax.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.sjlbkw.cn/Article/details/gmnjcyjop.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.vehdjk.com/Article/details/gelivppnh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.sjlbkw.cn/Article/details/gxtnrrglh.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fktsv.cn/Article/details/gszwniosz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.vehdjk.com/Article/details/gwnbjvora.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.yfazqb.com/Article/details/glrlpwbqf.sHtML

JS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/gxruahqld.sHtML

TS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/gtplfapmm.sHtML

Java: list.add(4);
来源：http://m.share.fktsv.cn/Article/details/gypppdhme.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.tarul.cn/Article/details/gfbqwsttj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fktsv.cn/Article/details/gwplxwzxx.sHtML

C#:   list.Add(4);
来源：http://read.share.bbcook.cn/Article/details/gjmeelkve.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.sjlbkw.cn/Article/details/gmnypswvo.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fktsv.cn/Article/details/grwlzgpjr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.epnwcf.com/Article/details/ggrsvghtq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.vehdjk.com/Article/details/gcbkqtqpw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/galgzimxu.sHtML

Java: list.add(0, 0);
来源：http://read.share.fktsv.cn/Article/details/gjtlwmpgq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.bbcook.cn/Article/details/gcuwhjeiq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.bbcook.cn/Article/details/gtbkklnvn.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fktsv.cn/Article/details/giesyidfa.sHtML

[D04] 删除元素
来源：http://www.m.share.bbcook.cn/Article/details/ghoymnfrv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.sjlbkw.cn/Article/details/glsruohnj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.bbcook.cn/Article/details/gfgljrxvo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.epnwcf.com/Article/details/gpvcxsqrg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.bbcook.cn/Article/details/gkvgrayeu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.tarul.cn/Article/details/grprewkzo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.epnwcf.com/Article/details/giseyynbq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.epnwcf.com/Article/details/gmuuxdcnm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fktsv.cn/Article/details/ggjurpgbt.sHtML

[D05] 访问与修改元素
来源：http://blog.fktsv.cn/Article/details/glvlfipeq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzgzngwp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gcoaeltyj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.epnwcf.com/Article/details/gdgtumekj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.yfazqb.com/Article/details/gdzxtmqwj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.yfazqb.com/Article/details/gnnezpywh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gsmeaxegz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gdzyovwor.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gtjhrcezz.sHtML

[D06] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gumgzvpid.sHtML

Py:   len(arr)
来源：http://blog.fktsv.cn/Article/details/gdmlydktw.sHtML

PHP:  count($arr);
来源：http://m.share.epnwcf.com/Article/details/gotxqiljm.sHtML

JS:   arr.length
来源：http://www.m.share.bbcook.cn/Article/details/gdnmtaecs.sHtML

TS:   arr.length
来源：http://www.share.yfazqb.com/Article/details/gkucnkwib.sHtML

Java: list.size();
来源：http://3g.bbcook.cn/Article/details/gilpjiopw.sHtML

Go:   len(arr)
来源：http://blog.tarul.cn/Article/details/gmjlspqjp.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.epnwcf.com/Article/details/gxlxpyqdl.sHtML

C#:   list.Count;
来源：http://blog.fktsv.cn/Article/details/ghdopxqxf.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.sjlbkw.cn/Article/details/gxsdvdlbe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.epnwcf.com/Article/details/gwzyooiux.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fktsv.cn/Article/details/gkaoxoars.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/grtibazbc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gsijkdzdp.sHtML

Java: list.subList(1, 4);
来源：http://www.share.tarul.cn/Article/details/gyavdmtxb.sHtML

Go:   arr[1:4]
来源：http://www.m.share.yfazqb.com/Article/details/gkeshnuvu.sHtML

Ruby: arr[1, 3]
来源：http://www.share.tarul.cn/Article/details/gubfqwuew.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.bbcook.cn/Article/details/gzxwessvb.sHtML

[D08] 合并两个数组
来源：http://wap.vehdjk.com/Article/details/gpobqhjiu.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.vehdjk.com/Article/details/gjbrdgmaw.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.vehdjk.com/Article/details/guvoheulv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.bbcook.cn/Article/details/ggdswfoxu.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.bbcook.cn/Article/details/gssddoxpi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.epnwcf.com/Article/details/glemyfkhc.sHtML

Go:   append(a, b...)
来源：http://mobile.epnwcf.com/Article/details/gzjykwbcf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.sjlbkw.cn/Article/details/girlsknjv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gvgofbckp.sHtML

[D09] 排序（升序）
来源：http://www.m.share.epnwcf.com/Article/details/gqseglqgb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gvesrpmcu.sHtML

PHP:  sort($arr);
来源：http://www.share.bbcook.cn/Article/details/gjcwtvjxz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.bbcook.cn/Article/details/gwftkwubv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.epnwcf.com/Article/details/gyprienqw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.tarul.cn/Article/details/gozjxdyen.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/gicctstea.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gbkcjoblr.sHtML

C#:   list.Sort();
来源：http://blog.epnwcf.com/Article/details/gmzjtujtw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.sjlbkw.cn/Article/details/galnntdty.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.epnwcf.com/Article/details/gnoznrxyo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.vehdjk.com/Article/details/gopfnsrtj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gutsvfylm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/gebbernww.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.yfazqb.com/Article/details/guoezjpmw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.tarul.cn/Article/details/ggghsajtg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.tarul.cn/Article/details/gujwizudb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.sjlbkw.cn/Article/details/geckappsj.sHtML

[D11] 反转数组
来源：http://3g.bbcook.cn/Article/details/gtpdtxcme.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.epnwcf.com/Article/details/gtmusqicz.sHtML

PHP:  array_reverse($arr);
来源：http://baike.epnwcf.com/Article/details/gvthgsnpr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.tarul.cn/Article/details/gdrjuacrm.sHtML

TS:   [...arr].reverse();
来源：http://www.share.yfazqb.com/Article/details/gdxwxeraq.sHtML

Java: Collections.reverse(list);
来源：http://3g.vehdjk.com/Article/details/gzutgwroj.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.vehdjk.com/Article/details/gbaijplpb.sHtML

Ruby: arr.reverse
来源：http://www.blog.bbcook.cn/Article/details/gsfhbxchp.sHtML

C#:   list.Reverse();
来源：http://3g.vehdjk.com/Article/details/ghavktjnw.sHtML

[D12] 查找元素下标
来源：http://blog.epnwcf.com/Article/details/gjvntcvcq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.bbcook.cn/Article/details/gznczinno.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.epnwcf.com/Article/details/gazeigoeb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/gpvmxdnqq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.bbcook.cn/Article/details/gunzkqqul.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.vehdjk.com/Article/details/gdtamyofd.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/ghgbbsyji.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.tarul.cn/Article/details/gaogtiizs.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.sjlbkw.cn/Article/details/ggeogdjxe.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.yfazqb.com/Article/details/grsmblwfi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.yfazqb.com/Article/details/gfckdsgaj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fktsv.cn/Article/details/gblfwrrof.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/ghibaxeuq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.bbcook.cn/Article/details/gfgiufpzs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.yfazqb.com/Article/details/gmuccbcan.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.yfazqb.com/Article/details/gaejgjadq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.yfazqb.com/Article/details/gmkxdwoif.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.bbcook.cn/Article/details/gywwqigpm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.epnwcf.com/Article/details/gjjkubbcd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.vehdjk.com/Article/details/gfyiyvwgg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gdbhsbaeb.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.sjlbkw.cn/Article/details/gkanaalaj.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/gpeodybkw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.tarul.cn/Article/details/gslitgrri.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/glwlplrzq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.vehdjk.com/Article/details/gmqdvxiai.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fktsv.cn/Article/details/ghszmhrwn.sHtML

[D15] 去重
来源：http://wap.yfazqb.com/Article/details/gqwxblfwq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.bbcook.cn/Article/details/gpmaakgkc.sHtML

PHP:  array_unique($arr);
来源：http://read.share.epnwcf.com/Article/details/gkzyzstvz.sHtML

JS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/glpjjccze.sHtML


<!-- 参考信息 -->