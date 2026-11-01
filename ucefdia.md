代发 wailian999

PHP:  $a && $b || !$c
来源：http://read.share.sjlbkw.cn/Article/details/ghldxfgzl.sHtML

JS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gqpnhctch.sHtML

TS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gtlqxavbu.sHtML

Java: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gwvfvegvx.sHtML

Go:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gdzlmdfet.sHtML

Ruby: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gbdrdbcid.sHtML

C#:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/grjhcebet.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.epnwcf.com/Article/details/gwqfpjjpk.sHtML

Py:   if not data: return
来源：http://m.share.yfazqb.com/Article/details/gehrbnuoe.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fktsv.cn/Article/details/giprgaikv.sHtML

JS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/glilqbrbe.sHtML

TS:   if (!data) return;
来源：http://mobile.vehdjk.com/Article/details/gapglzqgl.sHtML

Java: if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/gkiowxokt.sHtML

Go:   if data == nil { return }
来源：http://www.share.epnwcf.com/Article/details/gcwzhhoso.sHtML

Ruby: return if data.nil?
来源：http://www.share.yfazqb.com/Article/details/gyvmyjtxw.sHtML

C#:   if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gsbicmeop.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbqifbope.sHtML

C. 函数与作用域
来源：http://www.blog.yfazqb.com/Article/details/gocskwxig.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/geqmfgvxo.sHtML

[C01] 定义函数
来源：http://www.m.share.yfazqb.com/Article/details/grujkldke.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.vehdjk.com/Article/details/ggpywnkjt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/girkadpby.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/ghvqboixb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gvfvmaffi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gvswqsrhf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fktsv.cn/Article/details/gynaahfnh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.bbcook.cn/Article/details/gosjfxxwv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gffrkkglv.sHtML

[C02] 默认参数
来源：http://blog.yfazqb.com/Article/details/gmxbblzum.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.epnwcf.com/Article/details/gxhogymle.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.vehdjk.com/Article/details/gmqpfsdso.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gshftqaop.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/ggljjkcrw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.sjlbkw.cn/Article/details/gwsvraxva.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.sjlbkw.cn/Article/details/ggetfqpyz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.bbcook.cn/Article/details/gukfwfedc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.yfazqb.com/Article/details/gteixusde.sHtML

[C03] 可变参数
来源：http://m.share.yfazqb.com/Article/details/gmjwieihx.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.tarul.cn/Article/details/gftyeirfi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fktsv.cn/Article/details/gbsjiyisv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/gfallpzfz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gfzojwtey.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fktsv.cn/Article/details/gaeblvgvu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.tarul.cn/Article/details/ghjfieqjb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.vehdjk.com/Article/details/guqsxidie.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.bbcook.cn/Article/details/gqmyksmgr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.tarul.cn/Article/details/gmureuadp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.sjlbkw.cn/Article/details/gjhwgkvti.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.tarul.cn/Article/details/gixxdydjw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/goonagool.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fktsv.cn/Article/details/godqvfkwp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.tarul.cn/Article/details/grkrqahly.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.bbcook.cn/Article/details/gekymyvgd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/ghoesfgci.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/grcxdxanp.sHtML

[C05] 返回多个值
来源：http://3g.sjlbkw.cn/Article/details/gnglyksxb.sHtML

Py:   return a, b
来源：http://mobile.tarul.cn/Article/details/gghkgkwbq.sHtML

PHP:  return [$a, $b];
来源：http://baike.tarul.cn/Article/details/gakfbhsws.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/gzvaoyynq.sHtML

TS:   return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/gzzukrnqp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.sjlbkw.cn/Article/details/gwgczbuic.sHtML

Go:   return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gkytopbhc.sHtML

Ruby: return a, b
来源：http://mobile.tarul.cn/Article/details/gmdcthifk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.epnwcf.com/Article/details/gjktjebgv.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.bbcook.cn/Article/details/gmsunmljd.sHtML

Py:   square = lambda x: x * x
来源：http://wap.yfazqb.com/Article/details/gxynadnxg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.bbcook.cn/Article/details/gequmgfou.sHtML

JS:   const square = x => x * x;
来源：http://read.share.bbcook.cn/Article/details/ggakxjatt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gxbcxqfth.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.yfazqb.com/Article/details/gtfmbebjk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.vehdjk.com/Article/details/goiaznodf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.epnwcf.com/Article/details/gwxecescx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gpjsfmssu.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.tarul.cn/Article/details/gwwzjqint.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.tarul.cn/Article/details/gfbkvfvkg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.vehdjk.com/Article/details/gbmmovfzw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.yfazqb.com/Article/details/grczennjf.sHtML

TS:   arr.map(String)
来源：http://read.share.bbcook.cn/Article/details/gtfunxbtn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.vehdjk.com/Article/details/gpzbecxnr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.tarul.cn/Article/details/gkzvlzwcg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.vehdjk.com/Article/details/gzxlpogsz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fktsv.cn/Article/details/ggqcdbots.sHtML

[C08] 闭包
来源：http://www.share.yfazqb.com/Article/details/gpccaoxtv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.epnwcf.com/Article/details/gtjgafxqm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.epnwcf.com/Article/details/gzynfqpao.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gdntvajxf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gkdwewzxi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.epnwcf.com/Article/details/gyvywbdnn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.yfazqb.com/Article/details/gbfwsjial.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fktsv.cn/Article/details/gbfsglnnd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gmxwxniya.sHtML

[C09] 递归
来源：http://read.share.tarul.cn/Article/details/gwgglqtdm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/gayqnxxpz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.yfazqb.com/Article/details/gzsmpoksr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.vehdjk.com/Article/details/guqdjssbz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gzlezswad.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.epnwcf.com/Article/details/gejvoowkr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fktsv.cn/Article/details/grtxqwwsm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gzohbjcyh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.epnwcf.com/Article/details/grcjkbvut.sHtML

[C10] 变量作用域
来源：http://3g.tarul.cn/Article/details/gavjyvrsl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.bbcook.cn/Article/details/ggcvzpcdu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.bbcook.cn/Article/details/gwhnujdqy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.epnwcf.com/Article/details/gancnckvm.sHtML

TS:   同 JS
来源：http://blog.bbcook.cn/Article/details/ghyktfxdk.sHtML

Java: 方法内为块级作用域
来源：http://3g.fktsv.cn/Article/details/gqamxmnpi.sHtML

Go:   花括号块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gxfmawmoc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.yfazqb.com/Article/details/gkkwwhvbx.sHtML

C#:   块级作用域
来源：http://m.share.tarul.cn/Article/details/grfsuocxa.sHtML

[C11] 模块导入与导出
来源：http://www.share.vehdjk.com/Article/details/gmduxwmgb.sHtML

Py:   from module import func
来源：http://www.share.sjlbkw.cn/Article/details/gtuemfedj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.tarul.cn/Article/details/gwjhrxczp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.vehdjk.com/Article/details/germjrpvi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.sjlbkw.cn/Article/details/gvjigavlu.sHtML

Java: import java.util.List;
来源：http://3g.sjlbkw.cn/Article/details/gzpxykwiv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.tarul.cn/Article/details/gprcorqij.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.yfazqb.com/Article/details/gaibgglxn.sHtML

C#:   using System.Text;
来源：http://read.share.epnwcf.com/Article/details/gjsqlwejr.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.yfazqb.com/Article/details/gegtezqau.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.tarul.cn/Article/details/gvnxncvuo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fktsv.cn/Article/details/gpjjgjxym.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gsursifsd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fktsv.cn/Article/details/ghptsxabn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.bbcook.cn/Article/details/gukamquib.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.yfazqb.com/Article/details/gjeixjovm.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.tarul.cn/Article/details/gmvtbanzj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.bbcook.cn/Article/details/gcydvbbhk.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.bbcook.cn/Article/details/gkpxukbwp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.vehdjk.com/Article/details/gltdpgnxu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gtsiytvhm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.vehdjk.com/Article/details/ghipvwkxn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gvirvnhsw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/glogubkwr.sHtML

Go:   func add(a, b int) int
来源：http://mobile.sjlbkw.cn/Article/details/gzeeohcxe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fktsv.cn/Article/details/ghrkcwczs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.yfazqb.com/Article/details/gnioldvho.sHtML

[C14] 泛型函数
来源：http://3g.tarul.cn/Article/details/gtgbzjmxr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.vehdjk.com/Article/details/gwxukfrqb.sHtML

PHP:  // 无泛型
来源：http://wap.tarul.cn/Article/details/gkzggmpfs.sHtML

JS:   // 无泛型
来源：http://blog.tarul.cn/Article/details/gtblejhxv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fktsv.cn/Article/details/ginsmruhv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.vehdjk.com/Article/details/gdkraycna.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.yfazqb.com/Article/details/gtexfujze.sHtML

Ruby: # 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/glmdueiet.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.vehdjk.com/Article/details/gwefokkdu.sHtML

[C15] 解构 / 展开参数
来源：http://blog.sjlbkw.cn/Article/details/goxxhflnn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.tarul.cn/Article/details/gjlfjweoa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.vehdjk.com/Article/details/gayacnstq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fktsv.cn/Article/details/gysvsveuy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.yfazqb.com/Article/details/ghobzfqba.sHtML

Java: // 无解构
来源：http://blog.yfazqb.com/Article/details/gyznxfpgi.sHtML

Go:   // 无解构
来源：http://www.blog.yfazqb.com/Article/details/getqcnojv.sHtML

Ruby: a, b = pair
来源：http://mobile.sjlbkw.cn/Article/details/ghrcygeoo.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.epnwcf.com/Article/details/gfuaikztl.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.tarul.cn/Article/details/gudeabbax.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.bbcook.cn/Article/details/gtlnbpvlq.sHtML

PHP:  // 无重载
来源：http://m.share.yfazqb.com/Article/details/gumukerod.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.yfazqb.com/Article/details/gszwwprfp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.sjlbkw.cn/Article/details/grkxdnhfb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.vehdjk.com/Article/details/gvwtciybv.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/gkaklwfvi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.yfazqb.com/Article/details/ghjxprazs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.bbcook.cn/Article/details/giserleoy.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gqrqtgbqc.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.bbcook.cn/Article/details/gcgyqzfom.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gsysovkkp.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gidvqubap.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.bbcook.cn/Article/details/gnaxehcrm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.tarul.cn/Article/details/gwfvofdox.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.vehdjk.com/Article/details/gguuesmff.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.bbcook.cn/Article/details/gizjfjerm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.sjlbkw.cn/Article/details/gmdswtemq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.epnwcf.com/Article/details/gzmujjhjh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.sjlbkw.cn/Article/details/guizbujsq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.vehdjk.com/Article/details/gaxgqikfd.sHtML

[D02] 追加元素到末尾
来源：http://wap.yfazqb.com/Article/details/gtthafeqa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.sjlbkw.cn/Article/details/gwzehoqkv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fktsv.cn/Article/details/gxdfifrdp.sHtML

JS:   arr.push(4);
来源：http://www.share.sjlbkw.cn/Article/details/gpdtmhqqp.sHtML

TS:   arr.push(4);
来源：http://www.blog.epnwcf.com/Article/details/gylpyfzoe.sHtML

Java: list.add(4);
来源：http://www.blog.bbcook.cn/Article/details/gocxyelcv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.bbcook.cn/Article/details/gzlpymfeb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.bbcook.cn/Article/details/gxguphfvr.sHtML

C#:   list.Add(4);
来源：http://read.share.tarul.cn/Article/details/gilutuyrc.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.epnwcf.com/Article/details/gvuyvlwxr.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.vehdjk.com/Article/details/gdgcjqteb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.sjlbkw.cn/Article/details/guptqonom.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.yfazqb.com/Article/details/gxdofrbwa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.yfazqb.com/Article/details/gothyjljy.sHtML

Java: list.add(0, 0);
来源：http://wap.epnwcf.com/Article/details/genzlxkbq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.epnwcf.com/Article/details/gkyfukqcm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fktsv.cn/Article/details/gnhdptwlb.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.sjlbkw.cn/Article/details/guucoodmv.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/goejnonkt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.vehdjk.com/Article/details/gmcbtqlcz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.epnwcf.com/Article/details/giklgypgf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.yfazqb.com/Article/details/gtphbrhfb.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.epnwcf.com/Article/details/gxajytpls.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.tarul.cn/Article/details/govsfvkxf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.vehdjk.com/Article/details/gqztuflzx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.epnwcf.com/Article/details/ghgegugbg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.tarul.cn/Article/details/gompnclqj.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.epnwcf.com/Article/details/ghtbymdrr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/ghwyvrqpx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gjwrnnxqw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gudwgkaxh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fktsv.cn/Article/details/ggjezmjkv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.sjlbkw.cn/Article/details/gskwmvtqc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/grzxnmfcs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/grlbiahci.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gdfjqxrtd.sHtML

[D06] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gkovcqgzf.sHtML

Py:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gwwrewmou.sHtML

PHP:  count($arr);
来源：http://blog.fktsv.cn/Article/details/gljtujyav.sHtML

JS:   arr.length
来源：http://mobile.tarul.cn/Article/details/gxguxhrqk.sHtML

TS:   arr.length
来源：http://blog.epnwcf.com/Article/details/ggtiaensq.sHtML

Java: list.size();
来源：http://m.share.bbcook.cn/Article/details/gklaccoqw.sHtML

Go:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/ggjozenml.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fktsv.cn/Article/details/geavhjyev.sHtML

C#:   list.Count;
来源：http://www.share.bbcook.cn/Article/details/gstanwvfg.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fktsv.cn/Article/details/gmcofhwqw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fktsv.cn/Article/details/gbvtsjnsh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.tarul.cn/Article/details/gotbqaelm.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gpmarntxb.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fktsv.cn/Article/details/gjbodvaxj.sHtML

Java: list.subList(1, 4);
来源：http://baike.fktsv.cn/Article/details/gdgwpfvel.sHtML

Go:   arr[1:4]
来源：http://read.share.bbcook.cn/Article/details/gqiifptrj.sHtML

Ruby: arr[1, 3]
来源：http://mobile.bbcook.cn/Article/details/ggkdabqfx.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.bbcook.cn/Article/details/gujxmfibe.sHtML

[D08] 合并两个数组
来源：http://wap.bbcook.cn/Article/details/glbdyyxwl.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.tarul.cn/Article/details/gsxlvhctj.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.bbcook.cn/Article/details/ghngyyexq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.yfazqb.com/Article/details/gncyavfgi.sHtML

TS:   [...a, ...b];
来源：http://wap.sjlbkw.cn/Article/details/gfloqmpiw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.sjlbkw.cn/Article/details/gtjmxpoji.sHtML

Go:   append(a, b...)
来源：http://mobile.tarul.cn/Article/details/gpfmpphdn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.tarul.cn/Article/details/gwmyyabjb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/ggcjewmoy.sHtML

[D09] 排序（升序）
来源：http://baike.epnwcf.com/Article/details/gplokzfam.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/glzgyvjeb.sHtML

PHP:  sort($arr);
来源：http://3g.epnwcf.com/Article/details/ggfusafnr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fktsv.cn/Article/details/gyqktlmcj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.sjlbkw.cn/Article/details/gzmxhcrki.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.epnwcf.com/Article/details/grbswsnxt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fktsv.cn/Article/details/ggmwzgbcl.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/ghyifphtg.sHtML

C#:   list.Sort();
来源：http://3g.tarul.cn/Article/details/gtbbpvrzi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.epnwcf.com/Article/details/gukexnhcp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.bbcook.cn/Article/details/gkynhgjlb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/gdmwnchrm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.epnwcf.com/Article/details/geyfrubut.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gumjgzmyk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.epnwcf.com/Article/details/goqpdibfs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.yfazqb.com/Article/details/gbsgypdyk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.yfazqb.com/Article/details/gpesmjeyt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.sjlbkw.cn/Article/details/gamnifrxi.sHtML

[D11] 反转数组
来源：http://3g.fktsv.cn/Article/details/gmxbqawui.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.bbcook.cn/Article/details/gzvogkvkp.sHtML

PHP:  array_reverse($arr);
来源：http://baike.vehdjk.com/Article/details/gjrqmglwk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.sjlbkw.cn/Article/details/gpdeslsvb.sHtML

TS:   [...arr].reverse();
来源：http://baike.vehdjk.com/Article/details/gnhxkfbga.sHtML

Java: Collections.reverse(list);
来源：http://www.share.tarul.cn/Article/details/gnburwmac.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.bbcook.cn/Article/details/gorpnissb.sHtML

Ruby: arr.reverse
来源：http://m.share.fktsv.cn/Article/details/gsfscixlr.sHtML

C#:   list.Reverse();
来源：http://www.blog.vehdjk.com/Article/details/gyjelxnts.sHtML

[D12] 查找元素下标
来源：http://www.blog.tarul.cn/Article/details/gxrqdgmjs.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.yfazqb.com/Article/details/gufqrjuyu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fktsv.cn/Article/details/gpghjofas.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.yfazqb.com/Article/details/gtudvrehu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gmbbgptim.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.tarul.cn/Article/details/gfmmpreci.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.tarul.cn/Article/details/gmoycmjnn.sHtML

Ruby: arr.index(x)
来源：http://blog.tarul.cn/Article/details/getptytgk.sHtML

C#:   list.IndexOf(x);
来源：http://wap.sjlbkw.cn/Article/details/gxuvefcci.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.tarul.cn/Article/details/ggehevgms.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.vehdjk.com/Article/details/geifzjbej.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.tarul.cn/Article/details/gsorjjbge.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/gddtuuopt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gekgvtnko.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.bbcook.cn/Article/details/gxhhgemge.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.bbcook.cn/Article/details/gvernmvek.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.tarul.cn/Article/details/gnrplhoen.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.yfazqb.com/Article/details/gjmlyxfzj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.tarul.cn/Article/details/gdevejhek.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.bbcook.cn/Article/details/grlzhlwbw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.vehdjk.com/Article/details/gpdxbajrm.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/ghsgsqrdf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gtetbdtmq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.tarul.cn/Article/details/gsqezpcpd.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gxlhzaixc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.yfazqb.com/Article/details/grkvfbtqf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/grbhmcphm.sHtML

[D15] 去重
来源：http://m.share.fktsv.cn/Article/details/gokqnjpzl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/grdbpjbat.sHtML

PHP:  array_unique($arr);
来源：http://baike.epnwcf.com/Article/details/goqrceazv.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/gbvqhktwh.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/glimtlxsp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.bbcook.cn/Article/details/gnxfqpfkq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.epnwcf.com/Article/details/gbxtpnywg.sHtML

Ruby: arr.uniq
来源：http://3g.tarul.cn/Article/details/gtqhrqhoo.sHtML


<!-- 参考信息 -->