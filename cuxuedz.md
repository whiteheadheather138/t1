代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gojumrdfg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gjronkgsx.sHtML

[B15] 布尔运算与取反
来源：http://wap.sjlbkw.cn/Article/details/gpxrprymn.sHtML

Py:   a and b or not c
来源：http://baike.vehdjk.com/Article/details/gftdwrlzk.sHtML

PHP:  $a && $b || !$c
来源：http://baike.epnwcf.com/Article/details/ggdkavgwe.sHtML

JS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gmczcfoza.sHtML

TS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gxzzsjlbo.sHtML

Java: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gxomqzntj.sHtML

Go:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gtyjpnblp.sHtML

Ruby: a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gvfvphbuo.sHtML

C#:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gxwteajvd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.sjlbkw.cn/Article/details/gmwomhrhw.sHtML

Py:   if not data: return
来源：http://blog.epnwcf.com/Article/details/gvzvxjqum.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.vehdjk.com/Article/details/ghawdwtdo.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/gickzlqtu.sHtML

TS:   if (!data) return;
来源：http://blog.yfazqb.com/Article/details/geznjpycm.sHtML

Java: if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/gxyhapecn.sHtML

Go:   if data == nil { return }
来源：http://m.share.epnwcf.com/Article/details/gvmlxhgjo.sHtML

Ruby: return if data.nil?
来源：http://mobile.vehdjk.com/Article/details/grvfjwlgk.sHtML

C#:   if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gjzzxqzcl.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdzwfzkbr.sHtML

C. 函数与作用域
来源：http://wap.bbcook.cn/Article/details/guhadcwmn.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gizfgxtwu.sHtML

[C01] 定义函数
来源：http://baike.epnwcf.com/Article/details/gqdzqvcht.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.sjlbkw.cn/Article/details/gtmstvgpg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gfpvfnyxy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gkkmzlbas.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghumqzptp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gocfmclsr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.bbcook.cn/Article/details/gqwooclzu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.yfazqb.com/Article/details/gtxzanwah.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gmzvhvcyz.sHtML

[C02] 默认参数
来源：http://3g.vehdjk.com/Article/details/gchucnstp.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.vehdjk.com/Article/details/gdbrrmzdn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.bbcook.cn/Article/details/gbzmumdxm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.bbcook.cn/Article/details/gixxbvufh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gsbtldgfd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.bbcook.cn/Article/details/gzjlluyri.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fktsv.cn/Article/details/gxgdyizid.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.yfazqb.com/Article/details/gdipcbqvr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/gqxgpsiwm.sHtML

[C03] 可变参数
来源：http://mobile.tarul.cn/Article/details/gqctwnnsf.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.tarul.cn/Article/details/geddlgztj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fktsv.cn/Article/details/gytwejovv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gjwekvuox.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/guvqjusdk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.epnwcf.com/Article/details/gpgwftauh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fktsv.cn/Article/details/gmrwghdbz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fktsv.cn/Article/details/gidlpnwoy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fktsv.cn/Article/details/guxsxztxr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnytjwzp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.vehdjk.com/Article/details/gqaamfzuf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.tarul.cn/Article/details/gviougdvr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/goieczpml.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.yfazqb.com/Article/details/glpbfbiax.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fktsv.cn/Article/details/ghzuhinjs.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fktsv.cn/Article/details/gepfytumn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gfvxgwzxb.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fktsv.cn/Article/details/gxwobhbav.sHtML

[C05] 返回多个值
来源：http://baike.bbcook.cn/Article/details/gmipbmwgw.sHtML

Py:   return a, b
来源：http://m.share.tarul.cn/Article/details/gbjiplvgy.sHtML

PHP:  return [$a, $b];
来源：http://wap.vehdjk.com/Article/details/gnzqkaxkq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fktsv.cn/Article/details/gtqodfaxv.sHtML

TS:   return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/gxvmzjezt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.vehdjk.com/Article/details/gmziveicl.sHtML

Go:   return a, b
来源：http://mobile.tarul.cn/Article/details/gxgjhavxk.sHtML

Ruby: return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gjqkboroz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.tarul.cn/Article/details/gmmpgmfuy.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.epnwcf.com/Article/details/gdgfgrutj.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.bbcook.cn/Article/details/gdxituwak.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.tarul.cn/Article/details/gvuxyrozg.sHtML

JS:   const square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/grdunriry.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gthruhxmf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhdpsirx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.sjlbkw.cn/Article/details/gobqfbqjq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.sjlbkw.cn/Article/details/ggbwshnhp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/gksfwihps.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.vehdjk.com/Article/details/gdytdshqx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.yfazqb.com/Article/details/gyaguxlkp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/gkldufmvi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.bbcook.cn/Article/details/gqagwixcg.sHtML

TS:   arr.map(String)
来源：http://read.share.tarul.cn/Article/details/gkxreezkp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.vehdjk.com/Article/details/giozazvgn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.yfazqb.com/Article/details/gbsgslgbc.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/gihmjqhzy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fktsv.cn/Article/details/gmmtlpajx.sHtML

[C08] 闭包
来源：http://3g.bbcook.cn/Article/details/gkumrecce.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fktsv.cn/Article/details/gasriqpqe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.epnwcf.com/Article/details/grzljdshu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/grfhptijp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gujyddpdi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.vehdjk.com/Article/details/gbnbefmwh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.sjlbkw.cn/Article/details/gdoymcaui.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fktsv.cn/Article/details/gkmaujltq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gskebqmbq.sHtML

[C09] 递归
来源：http://www.m.share.fktsv.cn/Article/details/gggxzbcyg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/gyyrwhycr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.sjlbkw.cn/Article/details/gqpvfmkvg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gnnyfuojb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/gldsaewve.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.yfazqb.com/Article/details/glclxsivw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.tarul.cn/Article/details/grywtqwxf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/guugzyfly.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.epnwcf.com/Article/details/gqiuykpao.sHtML

[C10] 变量作用域
来源：http://www.blog.bbcook.cn/Article/details/gjygggcdv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.yfazqb.com/Article/details/ghokprjqm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.tarul.cn/Article/details/gjjvctfmc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.yfazqb.com/Article/details/gmrhvrisu.sHtML

TS:   同 JS
来源：http://blog.vehdjk.com/Article/details/glskljtvu.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fktsv.cn/Article/details/glncisqkg.sHtML

Go:   花括号块级作用域
来源：http://m.share.tarul.cn/Article/details/gbhmptvbc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.yfazqb.com/Article/details/gjzeggnuu.sHtML

C#:   块级作用域
来源：http://mobile.tarul.cn/Article/details/ggaduqjlq.sHtML

[C11] 模块导入与导出
来源：http://3g.epnwcf.com/Article/details/goaqolyqk.sHtML

Py:   from module import func
来源：http://www.blog.bbcook.cn/Article/details/gxerirpuc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjsusymx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.bbcook.cn/Article/details/gwbiigaou.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fktsv.cn/Article/details/ggyftohyp.sHtML

Java: import java.util.List;
来源：http://3g.vehdjk.com/Article/details/gnurtuvmo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fktsv.cn/Article/details/gshqfncad.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.vehdjk.com/Article/details/gfkojferk.sHtML

C#:   using System.Text;
来源：http://blog.bbcook.cn/Article/details/gkktgxjsl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.yfazqb.com/Article/details/gxwcieorb.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.yfazqb.com/Article/details/gjpaknbdt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.sjlbkw.cn/Article/details/griwvnsir.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.vehdjk.com/Article/details/gxmuelius.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.vehdjk.com/Article/details/ggjoyzvpd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.yfazqb.com/Article/details/giqjomdvy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.epnwcf.com/Article/details/gtavowccq.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.bbcook.cn/Article/details/gccczkgcs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.bbcook.cn/Article/details/gwfvgtoyj.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.sjlbkw.cn/Article/details/gbfcwuvct.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.vehdjk.com/Article/details/gxvhhrgxa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gwofxxjmv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.yfazqb.com/Article/details/ghkodvnsy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/glyrtxemz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gyzwnczzu.sHtML

Go:   func add(a, b int) int
来源：http://baike.vehdjk.com/Article/details/gtdygaksd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fktsv.cn/Article/details/gfuxmqcfb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.bbcook.cn/Article/details/gyilqcwjn.sHtML

[C14] 泛型函数
来源：http://baike.yfazqb.com/Article/details/gmpurlfky.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.tarul.cn/Article/details/gyqnpkykc.sHtML

PHP:  // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gjzoazvlg.sHtML

JS:   // 无泛型
来源：http://baike.tarul.cn/Article/details/gczzojfxl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fktsv.cn/Article/details/gdehugjdu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.tarul.cn/Article/details/gkteiadvq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.yfazqb.com/Article/details/gmgfknoqj.sHtML

Ruby: # 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gmbmflseo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.bbcook.cn/Article/details/gdairutgu.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fktsv.cn/Article/details/gmoaehsww.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.vehdjk.com/Article/details/gblndfcvm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.tarul.cn/Article/details/ggpekckfi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.tarul.cn/Article/details/gdsszhsqb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.epnwcf.com/Article/details/gtheyrlny.sHtML

Java: // 无解构
来源：http://baike.bbcook.cn/Article/details/gqlortitm.sHtML

Go:   // 无解构
来源：http://baike.epnwcf.com/Article/details/gwklcenbo.sHtML

Ruby: a, b = pair
来源：http://baike.sjlbkw.cn/Article/details/gwhgnycjh.sHtML

C#:   var (a, b) = pair;
来源：http://blog.tarul.cn/Article/details/ggrqneqza.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.epnwcf.com/Article/details/gfavrjtnt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.tarul.cn/Article/details/gvjoaevlx.sHtML

PHP:  // 无重载
来源：http://www.blog.bbcook.cn/Article/details/gdzdgstzg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.bbcook.cn/Article/details/gigxrquch.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fktsv.cn/Article/details/gxvipcixh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.yfazqb.com/Article/details/gjwqcnhmx.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.epnwcf.com/Article/details/gdcvbwtcl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.sjlbkw.cn/Article/details/gxnxkrutn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.sjlbkw.cn/Article/details/gpllyhfxh.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gjhgckhku.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.vehdjk.com/Article/details/gljfvdtwi.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwflazfvh.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.yfazqb.com/Article/details/gvpuuxggu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.vehdjk.com/Article/details/ggvxhqyiw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.epnwcf.com/Article/details/gelwrzujw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.yfazqb.com/Article/details/gwsjfgeax.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.sjlbkw.cn/Article/details/gxuhfksdy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.sjlbkw.cn/Article/details/glffptscr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.epnwcf.com/Article/details/ghavipxoy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.tarul.cn/Article/details/gfqwobtcy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.epnwcf.com/Article/details/gtuejbnpl.sHtML

[D02] 追加元素到末尾
来源：http://blog.tarul.cn/Article/details/gtsqbbnnx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.bbcook.cn/Article/details/ghrxaphlj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.bbcook.cn/Article/details/gzwnqkcub.sHtML

JS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/gnifajsvr.sHtML

TS:   arr.push(4);
来源：http://baike.sjlbkw.cn/Article/details/gbwxgytpd.sHtML

Java: list.add(4);
来源：http://3g.tarul.cn/Article/details/gfcgjsstf.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.bbcook.cn/Article/details/gknaitxra.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.epnwcf.com/Article/details/gwtuakkco.sHtML

C#:   list.Add(4);
来源：http://baike.fktsv.cn/Article/details/gpbdteilw.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.sjlbkw.cn/Article/details/gdffqzzch.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.tarul.cn/Article/details/ggggvbbzr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.tarul.cn/Article/details/gviyrgily.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.sjlbkw.cn/Article/details/gtkafxppf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.yfazqb.com/Article/details/gummvdibw.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/glgaikolv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.yfazqb.com/Article/details/gqivrrylg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.bbcook.cn/Article/details/gqntcevpp.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.bbcook.cn/Article/details/gvarhfwwy.sHtML

[D04] 删除元素
来源：http://m.share.fktsv.cn/Article/details/gvrqhqtwe.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.vehdjk.com/Article/details/gmgdlgccr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.tarul.cn/Article/details/gbwhldyyc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.sjlbkw.cn/Article/details/gpwlgbpzn.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.vehdjk.com/Article/details/guehufabp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fktsv.cn/Article/details/guxhqmcsf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.vehdjk.com/Article/details/gufuedlej.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fktsv.cn/Article/details/gdtpirqyp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.epnwcf.com/Article/details/gxqvibnxo.sHtML

[D05] 访问与修改元素
来源：http://m.share.vehdjk.com/Article/details/gqbibphmi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gxqrhnvll.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gziitktyy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gfjxtsqtv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.epnwcf.com/Article/details/gadiaeodo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fktsv.cn/Article/details/gofisltwl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gkosrvykj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gntrwkdks.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gpywnltlx.sHtML

[D06] 数组长度
来源：http://wap.tarul.cn/Article/details/gwubqtmbf.sHtML

Py:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gqxjtsney.sHtML

PHP:  count($arr);
来源：http://3g.bbcook.cn/Article/details/gbpklslkf.sHtML

JS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/gowvrirua.sHtML

TS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gbyxbmmzj.sHtML

Java: list.size();
来源：http://read.share.bbcook.cn/Article/details/gxvguxwzz.sHtML

Go:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/gktnuhxmm.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.sjlbkw.cn/Article/details/gwhtnxmnh.sHtML

C#:   list.Count;
来源：http://mobile.epnwcf.com/Article/details/ggsgazpty.sHtML

[D07] 切片 / 取子数组
来源：http://3g.bbcook.cn/Article/details/gjnoksidt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.epnwcf.com/Article/details/gynxpjwrm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fktsv.cn/Article/details/glhtqggzs.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.bbcook.cn/Article/details/gpcronqxf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gpjryefhx.sHtML

Java: list.subList(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gnjkrthco.sHtML

Go:   arr[1:4]
来源：http://baike.epnwcf.com/Article/details/gwnenmntu.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.yfazqb.com/Article/details/gmwnwqoya.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.yfazqb.com/Article/details/giyherbal.sHtML

[D08] 合并两个数组
来源：http://m.share.tarul.cn/Article/details/gslbfaxua.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.sjlbkw.cn/Article/details/gqiopqlgu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.vehdjk.com/Article/details/glrjmbuep.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.yfazqb.com/Article/details/gxhzdbtzs.sHtML

TS:   [...a, ...b];
来源：http://blog.yfazqb.com/Article/details/gqnobjhzu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gyzgshrui.sHtML

Go:   append(a, b...)
来源：http://read.share.vehdjk.com/Article/details/gzxeuqcul.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fktsv.cn/Article/details/gdxfuwgrh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/glyzwrvyp.sHtML

[D09] 排序（升序）
来源：http://mobile.bbcook.cn/Article/details/gjwpfhepb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gmqsnsywj.sHtML

PHP:  sort($arr);
来源：http://www.share.yfazqb.com/Article/details/gvfzyxvgu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fktsv.cn/Article/details/gipoumqjg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.tarul.cn/Article/details/gorzvgbxr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.tarul.cn/Article/details/gohosblgt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/ghltbewvl.sHtML

Ruby: arr.sort
来源：http://read.share.yfazqb.com/Article/details/gvlzwoddy.sHtML

C#:   list.Sort();
来源：http://blog.fktsv.cn/Article/details/gbauljbhp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.epnwcf.com/Article/details/gpvlsccpy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.vehdjk.com/Article/details/gyfwumnsj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqvhmuwi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fktsv.cn/Article/details/ggmjnwvjp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.bbcook.cn/Article/details/ggqxbuefz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fktsv.cn/Article/details/ghgnwomjc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.sjlbkw.cn/Article/details/gejgczflx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.epnwcf.com/Article/details/gmynofzex.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.tarul.cn/Article/details/glythzapp.sHtML

[D11] 反转数组
来源：http://baike.epnwcf.com/Article/details/gcntumtti.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fktsv.cn/Article/details/gqcvdopsw.sHtML

PHP:  array_reverse($arr);
来源：http://blog.epnwcf.com/Article/details/gylilrymt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.tarul.cn/Article/details/giaxglpna.sHtML

TS:   [...arr].reverse();
来源：http://m.share.epnwcf.com/Article/details/grukorvak.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gckemtghq.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.vehdjk.com/Article/details/gzexypojj.sHtML

Ruby: arr.reverse
来源：http://m.share.yfazqb.com/Article/details/glwlshfge.sHtML

C#:   list.Reverse();
来源：http://blog.bbcook.cn/Article/details/gvadiqozc.sHtML

[D12] 查找元素下标
来源：http://blog.yfazqb.com/Article/details/gdzjnjolb.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.bbcook.cn/Article/details/gvvmbhrus.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.bbcook.cn/Article/details/gyltfrofn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/gguurpfil.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/gimarhlvv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.epnwcf.com/Article/details/ghhjwzvrj.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.vehdjk.com/Article/details/gdhebqmwo.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fktsv.cn/Article/details/giieobexq.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fktsv.cn/Article/details/gvbozknjv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.vehdjk.com/Article/details/ggmytttdp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.bbcook.cn/Article/details/gdzcjnlvw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.epnwcf.com/Article/details/gqhblqixf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.tarul.cn/Article/details/gsfwrykoa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gzkxqmwwv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fktsv.cn/Article/details/ggefdygdc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.sjlbkw.cn/Article/details/gviqppzsa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fktsv.cn/Article/details/gxmguqdft.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.yfazqb.com/Article/details/gjjpydimc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.bbcook.cn/Article/details/gqgileild.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.bbcook.cn/Article/details/gnmcworxl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gncsyvwqe.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gazfhsbgj.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/gilupjebi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fktsv.cn/Article/details/gszsgjlkn.sHtML

Go:   // 手写循环
来源：http://mobile.vehdjk.com/Article/details/gdlkjrwad.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fktsv.cn/Article/details/gcrkmoomx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.tarul.cn/Article/details/gshcxlzeb.sHtML

[D15] 去重
来源：http://wap.fktsv.cn/Article/details/guqbmltxn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fktsv.cn/Article/details/ghukssmnx.sHtML

PHP:  array_unique($arr);
来源：http://3g.epnwcf.com/Article/details/gjgsrvefx.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/gejqfrmcb.sHtML


<!-- 参考信息 -->