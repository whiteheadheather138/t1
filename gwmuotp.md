代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.vehdjk.com/Article/details/gifwkfdyp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gmeoadmkv.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnzkuoeh.sHtML

Py:   a and b or not c
来源：http://m.share.vehdjk.com/Article/details/gtdjlppam.sHtML

PHP:  $a && $b || !$c
来源：http://baike.yfazqb.com/Article/details/gkbcyrlnu.sHtML

JS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/germmfkhg.sHtML

TS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gkbenyekf.sHtML

Java: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gjclelldm.sHtML

Go:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/ghvvedfto.sHtML

Ruby: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gkobtzuzb.sHtML

C#:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gzclrccop.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fktsv.cn/Article/details/grbodxraj.sHtML

Py:   if not data: return
来源：http://3g.tarul.cn/Article/details/gqudsikpz.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.epnwcf.com/Article/details/gtbaaenkv.sHtML

JS:   if (!data) return;
来源：http://read.share.fktsv.cn/Article/details/gjdyzdhup.sHtML

TS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/gpoeiqmqa.sHtML

Java: if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/garljcaxa.sHtML

Go:   if data == nil { return }
来源：http://baike.epnwcf.com/Article/details/gvylckcqa.sHtML

Ruby: return if data.nil?
来源：http://3g.vehdjk.com/Article/details/gasbfiotk.sHtML

C#:   if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gtcopmnax.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gmnnmjqzo.sHtML

C. 函数与作用域
来源：http://www.share.yfazqb.com/Article/details/gmqtlzkoy.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gayzbdznv.sHtML

[C01] 定义函数
来源：http://wap.vehdjk.com/Article/details/gczzzctmm.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.epnwcf.com/Article/details/gezsihgrc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gaakrfdkk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gkfpzxzfv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gpxfffzxn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/grufopmbp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.epnwcf.com/Article/details/gbqcgkbjz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.yfazqb.com/Article/details/gzsfjdlqx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gaamuuxhp.sHtML

[C02] 默认参数
来源：http://www.m.share.sjlbkw.cn/Article/details/grukabsdz.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.epnwcf.com/Article/details/gdmhjyldv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.vehdjk.com/Article/details/gbebobzll.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gmtylnckx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/ggjxryrsb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.bbcook.cn/Article/details/gwymlpzmg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.tarul.cn/Article/details/gwnqssckc.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.vehdjk.com/Article/details/ghnwsmbeg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.epnwcf.com/Article/details/gbjfeyemb.sHtML

[C03] 可变参数
来源：http://baike.yfazqb.com/Article/details/gupvvqwod.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.tarul.cn/Article/details/guojurosh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.epnwcf.com/Article/details/gyyugewvc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/gbalfsioe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gydqbiodr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.bbcook.cn/Article/details/gjvlcgpuj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.sjlbkw.cn/Article/details/gldqpxymo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.yfazqb.com/Article/details/gewwkllky.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.yfazqb.com/Article/details/geqkewjzq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.epnwcf.com/Article/details/gpjvzookq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.vehdjk.com/Article/details/gnwzpdmoy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fktsv.cn/Article/details/gewloehvi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/gzrbzrrmd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gwdzaundf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.tarul.cn/Article/details/gogzsbmqg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.yfazqb.com/Article/details/gvrlydqtx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/grgcnthux.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/gukwkyivx.sHtML

[C05] 返回多个值
来源：http://read.share.bbcook.cn/Article/details/gudjgihxc.sHtML

Py:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gmrrlkeky.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.bbcook.cn/Article/details/gfphsmfwc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.vehdjk.com/Article/details/gavtbzbjv.sHtML

TS:   return { a, b };
来源：http://m.share.fktsv.cn/Article/details/grplayzuy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.tarul.cn/Article/details/gbvxtwivr.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gmzxegrtm.sHtML

Ruby: return a, b
来源：http://wap.bbcook.cn/Article/details/gsyromqru.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.yfazqb.com/Article/details/gagkaqcwq.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.tarul.cn/Article/details/gvdmmuerp.sHtML

Py:   square = lambda x: x * x
来源：http://3g.epnwcf.com/Article/details/gesipaoep.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fktsv.cn/Article/details/gwzxkkomr.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.tarul.cn/Article/details/gapcrojqb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.yfazqb.com/Article/details/gfrlhnxst.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gvrzuwzte.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.yfazqb.com/Article/details/gpyjfvqky.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.yfazqb.com/Article/details/gdmunbyfo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gttogcxmt.sHtML

[C07] 把函数作为参数传入
来源：http://baike.yfazqb.com/Article/details/geitbpqlx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.yfazqb.com/Article/details/gmjmnltei.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gpysntosj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.epnwcf.com/Article/details/gbplyksae.sHtML

TS:   arr.map(String)
来源：http://www.blog.vehdjk.com/Article/details/gktjhcnai.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.bbcook.cn/Article/details/glytedyjx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.vehdjk.com/Article/details/gbuwlsnds.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.tarul.cn/Article/details/gihgdvipd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.sjlbkw.cn/Article/details/gzzoeszca.sHtML

[C08] 闭包
来源：http://blog.epnwcf.com/Article/details/gdkddfpqe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.vehdjk.com/Article/details/gxljailmx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.epnwcf.com/Article/details/gjtnueivk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/garvnflrm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gidlijimu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/gesmsltku.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.yfazqb.com/Article/details/gftcbijbw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.yfazqb.com/Article/details/gocjzvjem.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gobixjhtd.sHtML

[C09] 递归
来源：http://www.blog.yfazqb.com/Article/details/gpusfmaaw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gbrjmyxup.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/grmabqkhb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fktsv.cn/Article/details/gblxiflnr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fktsv.cn/Article/details/gnvxjlhuv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.epnwcf.com/Article/details/goydrnhjo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.yfazqb.com/Article/details/ghwkposuk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.epnwcf.com/Article/details/gjfckluge.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fktsv.cn/Article/details/gkncdthan.sHtML

[C10] 变量作用域
来源：http://blog.sjlbkw.cn/Article/details/gyvwnfnmw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.yfazqb.com/Article/details/gkxjaqsjf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.vehdjk.com/Article/details/gdliapjfa.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.tarul.cn/Article/details/gxalbuaxe.sHtML

TS:   同 JS
来源：http://3g.bbcook.cn/Article/details/gcerytusv.sHtML

Java: 方法内为块级作用域
来源：http://mobile.tarul.cn/Article/details/gopgzflkp.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gmkdmwdad.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.vehdjk.com/Article/details/goszknjjl.sHtML

C#:   块级作用域
来源：http://www.share.vehdjk.com/Article/details/gklebajsq.sHtML

[C11] 模块导入与导出
来源：http://www.share.bbcook.cn/Article/details/gohmaflcw.sHtML

Py:   from module import func
来源：http://mobile.sjlbkw.cn/Article/details/gbbgyxgnp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.tarul.cn/Article/details/gdrkfsyvm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fktsv.cn/Article/details/gwmnkjvqp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.epnwcf.com/Article/details/gzvlhrynn.sHtML

Java: import java.util.List;
来源：http://mobile.fktsv.cn/Article/details/gbakvdlgu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.yfazqb.com/Article/details/gzsahejbk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.epnwcf.com/Article/details/gevqgbbtt.sHtML

C#:   using System.Text;
来源：http://read.share.bbcook.cn/Article/details/gfvhekfib.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.sjlbkw.cn/Article/details/gdnzjrvks.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.tarul.cn/Article/details/gpeohfend.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.bbcook.cn/Article/details/gjiokhxza.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.yfazqb.com/Article/details/gntthaelb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.epnwcf.com/Article/details/gmvmndlcx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.epnwcf.com/Article/details/gthlpwhmw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.tarul.cn/Article/details/ghjeqkxov.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.yfazqb.com/Article/details/gkdwldoru.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.bbcook.cn/Article/details/gyqcuydnt.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.vehdjk.com/Article/details/ggogatrrl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.yfazqb.com/Article/details/gqetxighg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gyraiking.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.tarul.cn/Article/details/gfdjgdgjc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gnyxtsebq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gdqojuupp.sHtML

Go:   func add(a, b int) int
来源：http://baike.vehdjk.com/Article/details/gfzhlelrk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fktsv.cn/Article/details/gpvzkofjh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.bbcook.cn/Article/details/gqsskgtae.sHtML

[C14] 泛型函数
来源：http://wap.epnwcf.com/Article/details/gxmwkxxuc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.yfazqb.com/Article/details/gqxwjnnxb.sHtML

PHP:  // 无泛型
来源：http://blog.epnwcf.com/Article/details/gfwpooedm.sHtML

JS:   // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gilwbapvs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.sjlbkw.cn/Article/details/gomoredhd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.tarul.cn/Article/details/gwlzivxxq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.epnwcf.com/Article/details/gyiuqyrek.sHtML

Ruby: # 无泛型
来源：http://baike.fktsv.cn/Article/details/gyjaimjcz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.epnwcf.com/Article/details/goanosglr.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.tarul.cn/Article/details/gsnpbdfft.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.vehdjk.com/Article/details/gxrzeptkb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.sjlbkw.cn/Article/details/gpjmbfdqy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.epnwcf.com/Article/details/gizbcwkdg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fktsv.cn/Article/details/gchnggaot.sHtML

Java: // 无解构
来源：http://www.blog.fktsv.cn/Article/details/gqjgrjyhq.sHtML

Go:   // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/glilagcuy.sHtML

Ruby: a, b = pair
来源：http://baike.tarul.cn/Article/details/gbtgjjqhy.sHtML

C#:   var (a, b) = pair;
来源：http://blog.yfazqb.com/Article/details/gvnzfgazm.sHtML

[C16] 函数 / 方法重载
来源：http://baike.sjlbkw.cn/Article/details/gzxoqcusc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.epnwcf.com/Article/details/grcntueys.sHtML

PHP:  // 无重载
来源：http://www.blog.tarul.cn/Article/details/glrtdszxe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fktsv.cn/Article/details/gbkxmnqxl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fktsv.cn/Article/details/gjlkxcxlh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fktsv.cn/Article/details/gvpueqqwn.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.bbcook.cn/Article/details/gsuagmfst.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fktsv.cn/Article/details/gnxoyhybk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.vehdjk.com/Article/details/gtsqsrsfe.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqijbunda.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.tarul.cn/Article/details/garxklgel.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gcrxrfxap.sHtML

[D01] 创建数组 / 列表
来源：http://wap.epnwcf.com/Article/details/gbmhmvdhl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fktsv.cn/Article/details/gcwdniypg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.vehdjk.com/Article/details/gupwjayqy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.bbcook.cn/Article/details/giirqhghq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.sjlbkw.cn/Article/details/ggsqgekap.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.bbcook.cn/Article/details/gtopqyfus.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/guznzocud.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.tarul.cn/Article/details/gyypijxbs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.tarul.cn/Article/details/gqtkpuwum.sHtML

[D02] 追加元素到末尾
来源：http://3g.vehdjk.com/Article/details/gtbyigtqx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.tarul.cn/Article/details/gakejydru.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.sjlbkw.cn/Article/details/gbavvhrye.sHtML

JS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/gxvmaefcp.sHtML

TS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/goqbkrzhw.sHtML

Java: list.add(4);
来源：http://mobile.vehdjk.com/Article/details/gxvwbytkx.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gwiporxkt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.epnwcf.com/Article/details/grfdvdtfh.sHtML

C#:   list.Add(4);
来源：http://www.blog.yfazqb.com/Article/details/ghngdhdfr.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.tarul.cn/Article/details/gywfboclu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gfuvjcmnj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.tarul.cn/Article/details/gyfcpxodu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.epnwcf.com/Article/details/gbbmpaqsz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.tarul.cn/Article/details/gzyfmlkut.sHtML

Java: list.add(0, 0);
来源：http://baike.yfazqb.com/Article/details/gbfijfmjv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fktsv.cn/Article/details/gosgejczf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.bbcook.cn/Article/details/gkuqulzuu.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.bbcook.cn/Article/details/gleeawnpt.sHtML

[D04] 删除元素
来源：http://www.share.vehdjk.com/Article/details/gpqfgidog.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.vehdjk.com/Article/details/gqmolwybm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/geqqehzli.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.epnwcf.com/Article/details/gbpofqzhe.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.epnwcf.com/Article/details/gkvtfcxdj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.bbcook.cn/Article/details/gffnalcfe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.tarul.cn/Article/details/gifcypvkm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.yfazqb.com/Article/details/gtqfcxios.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fktsv.cn/Article/details/gjasqanaq.sHtML

[D05] 访问与修改元素
来源：http://m.share.fktsv.cn/Article/details/gbvvxsjrv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gxvcacmln.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gbvfavlnv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.yfazqb.com/Article/details/gqyvwwfku.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.bbcook.cn/Article/details/gqwrqrlup.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.yfazqb.com/Article/details/gywpyvkeh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gavmodssq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gdrycnwme.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/ggafoknzg.sHtML

[D06] 数组长度
来源：http://3g.epnwcf.com/Article/details/gxmhjtuld.sHtML

Py:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gkogkfbra.sHtML

PHP:  count($arr);
来源：http://www.share.bbcook.cn/Article/details/gceygosba.sHtML

JS:   arr.length
来源：http://3g.sjlbkw.cn/Article/details/geciivbkd.sHtML

TS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/giewmuhsf.sHtML

Java: list.size();
来源：http://www.share.bbcook.cn/Article/details/gkrnyvawt.sHtML

Go:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gwqftdfsf.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.tarul.cn/Article/details/gddzswqkp.sHtML

C#:   list.Count;
来源：http://read.share.epnwcf.com/Article/details/gstmjrjyw.sHtML

[D07] 切片 / 取子数组
来源：http://baike.sjlbkw.cn/Article/details/gkzexanzn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.bbcook.cn/Article/details/gqymbqmut.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.bbcook.cn/Article/details/gqdxrvsnu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/ghadhfvbp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/gyoxjerdv.sHtML

Java: list.subList(1, 4);
来源：http://3g.tarul.cn/Article/details/giaovnadj.sHtML

Go:   arr[1:4]
来源：http://www.blog.fktsv.cn/Article/details/gngkzzkde.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.tarul.cn/Article/details/gxlcfcwpz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.tarul.cn/Article/details/grhqjhtgq.sHtML

[D08] 合并两个数组
来源：http://read.share.epnwcf.com/Article/details/geqdqtklh.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.sjlbkw.cn/Article/details/ghwnejzec.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.vehdjk.com/Article/details/gnrhhztmj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.tarul.cn/Article/details/gbuhmjvis.sHtML

TS:   [...a, ...b];
来源：http://m.share.epnwcf.com/Article/details/gqjpceuob.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.sjlbkw.cn/Article/details/gydsmjmex.sHtML

Go:   append(a, b...)
来源：http://blog.bbcook.cn/Article/details/gdbmckyys.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.tarul.cn/Article/details/gkevpmofc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gtsrlcvux.sHtML

[D09] 排序（升序）
来源：http://mobile.sjlbkw.cn/Article/details/gogmpxuag.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gwqleljyg.sHtML

PHP:  sort($arr);
来源：http://3g.vehdjk.com/Article/details/gpcigpiwq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.tarul.cn/Article/details/gmklvrxcu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.vehdjk.com/Article/details/gszuhvgsh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.yfazqb.com/Article/details/gkxgjguak.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gopufdxze.sHtML

Ruby: arr.sort
来源：http://baike.vehdjk.com/Article/details/gtzpjqkmi.sHtML

C#:   list.Sort();
来源：http://www.blog.tarul.cn/Article/details/gobnsusoz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.yfazqb.com/Article/details/gyriaxclu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.vehdjk.com/Article/details/gxhuusvxs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/gqtifhoke.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fktsv.cn/Article/details/gjdniykwj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/gyfmszsnr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.yfazqb.com/Article/details/gnayktynk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.epnwcf.com/Article/details/gzsiyntbp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.tarul.cn/Article/details/gcnzqinea.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.epnwcf.com/Article/details/gdbdkgldc.sHtML

[D11] 反转数组
来源：http://www.blog.bbcook.cn/Article/details/gjwkepapx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.bbcook.cn/Article/details/givrbulys.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gljdvlylm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.vehdjk.com/Article/details/govdddjhb.sHtML

TS:   [...arr].reverse();
来源：http://3g.yfazqb.com/Article/details/gglrhmigu.sHtML

Java: Collections.reverse(list);
来源：http://m.share.tarul.cn/Article/details/gtrsoikfv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.yfazqb.com/Article/details/gksnjpntl.sHtML

Ruby: arr.reverse
来源：http://3g.sjlbkw.cn/Article/details/gyluarxxl.sHtML

C#:   list.Reverse();
来源：http://m.share.sjlbkw.cn/Article/details/gllneujpe.sHtML

[D12] 查找元素下标
来源：http://baike.vehdjk.com/Article/details/gaqslzhfv.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fktsv.cn/Article/details/gofdeuete.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.vehdjk.com/Article/details/gaarnkkoz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/ghzvapxzo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/ggvyntwex.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.sjlbkw.cn/Article/details/gmxbtgkpf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gmydlxnej.sHtML

Ruby: arr.index(x)
来源：http://www.share.sjlbkw.cn/Article/details/gomymfpne.sHtML

C#:   list.IndexOf(x);
来源：http://3g.yfazqb.com/Article/details/gznnlcygn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.bbcook.cn/Article/details/gbwhcegis.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.yfazqb.com/Article/details/gwxpfnvpv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.yfazqb.com/Article/details/gfsbvuicg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.bbcook.cn/Article/details/ghqotrsmf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gqntkyprj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.vehdjk.com/Article/details/gzznyorjx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.bbcook.cn/Article/details/gnjhcoxbt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.vehdjk.com/Article/details/glovktxie.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.vehdjk.com/Article/details/gqetxiwqd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.vehdjk.com/Article/details/gbbzownyt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrdlwqju.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.yfazqb.com/Article/details/gbmznnkfn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/ggcyeycfy.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.yfazqb.com/Article/details/ghklodvrq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.epnwcf.com/Article/details/gdnimesug.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/gtmvsflsy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.epnwcf.com/Article/details/gydkyhbsx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gruxxwqdr.sHtML

[D15] 去重
来源：http://blog.tarul.cn/Article/details/gmmcsyoya.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/ghtrggsjy.sHtML

PHP:  array_unique($arr);
来源：http://www.share.vehdjk.com/Article/details/glnqwnqyh.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gfuokvkwg.sHtML


<!-- 参考信息 -->