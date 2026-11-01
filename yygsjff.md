代发 wailian999

Java: if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gxxawoxka.sHtML

Go:   if data == nil { return }
来源：http://read.share.epnwcf.com/Article/details/gerjhvmzq.sHtML

Ruby: return if data.nil?
来源：http://www.share.tarul.cn/Article/details/guhdzxmuv.sHtML

C#:   if (data == null) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gfavtwgql.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gzkvvkoan.sHtML

C. 函数与作用域
来源：http://read.share.epnwcf.com/Article/details/gzpqdfdql.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gsqamgtwv.sHtML

[C01] 定义函数
来源：http://wap.tarul.cn/Article/details/ggvrpkywq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.tarul.cn/Article/details/girozpjww.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gmgqodjru.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gvnoevnlx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gnrfzyuwv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gwsypxcos.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.yfazqb.com/Article/details/glccsellu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.tarul.cn/Article/details/ghszpvavc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gmclorkyl.sHtML

[C02] 默认参数
来源：http://mobile.vehdjk.com/Article/details/gcdjkhqju.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fktsv.cn/Article/details/gelhrjqai.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fktsv.cn/Article/details/gwjfirras.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.bbcook.cn/Article/details/gsuacewvo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/gefjzqsmd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fktsv.cn/Article/details/ghmadresx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.bbcook.cn/Article/details/gdxpdxzzo.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.yfazqb.com/Article/details/giyxsulim.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.vehdjk.com/Article/details/gjjwdckqd.sHtML

[C03] 可变参数
来源：http://www.blog.tarul.cn/Article/details/ghlxtmqjo.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.vehdjk.com/Article/details/gumlosbzh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.epnwcf.com/Article/details/glmwdannl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gornwwkhz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.bbcook.cn/Article/details/gytgkdvad.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.tarul.cn/Article/details/gngsbomml.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fktsv.cn/Article/details/goidrrckg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.sjlbkw.cn/Article/details/gjkwuxcaf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fktsv.cn/Article/details/gtneutaww.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fktsv.cn/Article/details/gujwihfsd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcognlwgm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.vehdjk.com/Article/details/gnbqawsup.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gulsvuyar.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fktsv.cn/Article/details/gkfckxoux.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.bbcook.cn/Article/details/gvuhcouzw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlmxrhzj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gzbiclebx.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gkafethyf.sHtML

[C05] 返回多个值
来源：http://blog.yfazqb.com/Article/details/gtwweebyn.sHtML

Py:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/galjbryfm.sHtML

PHP:  return [$a, $b];
来源：http://www.share.vehdjk.com/Article/details/grooqnqnl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gjjkpugng.sHtML

TS:   return { a, b };
来源：http://read.share.sjlbkw.cn/Article/details/gxlweokwp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.tarul.cn/Article/details/gfnydfdzn.sHtML

Go:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gwntyoaxq.sHtML

Ruby: return a, b
来源：http://www.blog.bbcook.cn/Article/details/gbuhprqzn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.tarul.cn/Article/details/gmlkqedbe.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.tarul.cn/Article/details/glxhofvyf.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.bbcook.cn/Article/details/goxemxpif.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.epnwcf.com/Article/details/gdqunfbat.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gcyhoftwb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.vehdjk.com/Article/details/gworwuapy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.tarul.cn/Article/details/gzyxgphhw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.bbcook.cn/Article/details/gserimlzg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.yfazqb.com/Article/details/giogmuzpi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gzvmsfvku.sHtML

[C07] 把函数作为参数传入
来源：http://wap.tarul.cn/Article/details/gplbokuqa.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.vehdjk.com/Article/details/gnlmibpgr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.vehdjk.com/Article/details/gcvmkrewh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.epnwcf.com/Article/details/gyxlybtph.sHtML

TS:   arr.map(String)
来源：http://blog.yfazqb.com/Article/details/gfolfzpdp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/ghutkvrkz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.bbcook.cn/Article/details/gwwrjtanj.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.yfazqb.com/Article/details/gkaainojr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.epnwcf.com/Article/details/gqtdisniz.sHtML

[C08] 闭包
来源：http://3g.sjlbkw.cn/Article/details/gboxrvnxo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.epnwcf.com/Article/details/gsfcqlfwb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.yfazqb.com/Article/details/gscrwekyz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/grhccjwzm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/grkbdfrjl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.epnwcf.com/Article/details/gepsvbrio.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.sjlbkw.cn/Article/details/ggpmgkxxt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fktsv.cn/Article/details/gomuvsljq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gldljheac.sHtML

[C09] 递归
来源：http://m.share.sjlbkw.cn/Article/details/gzprljggm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gyvfkcekf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.vehdjk.com/Article/details/gzspzvqyc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.tarul.cn/Article/details/gdlihndfr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.epnwcf.com/Article/details/gwusuvdxs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/gaeylrxzi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.epnwcf.com/Article/details/gesivkexr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/gcavarehh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.sjlbkw.cn/Article/details/gxlniykhs.sHtML

[C10] 变量作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gdjyigqdu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.sjlbkw.cn/Article/details/gnjogzact.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.vehdjk.com/Article/details/gwquyqfyn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fktsv.cn/Article/details/gaymcuzob.sHtML

TS:   同 JS
来源：http://3g.tarul.cn/Article/details/gmcdskdkk.sHtML

Java: 方法内为块级作用域
来源：http://blog.bbcook.cn/Article/details/gkwpetghs.sHtML

Go:   花括号块级作用域
来源：http://wap.vehdjk.com/Article/details/gerfcgyqv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.yfazqb.com/Article/details/gdwompziy.sHtML

C#:   块级作用域
来源：http://www.blog.epnwcf.com/Article/details/ghkkfdmyk.sHtML

[C11] 模块导入与导出
来源：http://blog.vehdjk.com/Article/details/gaeulfbvy.sHtML

Py:   from module import func
来源：http://baike.sjlbkw.cn/Article/details/ghxjolxiy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.yfazqb.com/Article/details/gfxbifiyr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.epnwcf.com/Article/details/gflezyboy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.epnwcf.com/Article/details/gbigxazzh.sHtML

Java: import java.util.List;
来源：http://wap.tarul.cn/Article/details/gzmlymrxs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.bbcook.cn/Article/details/gmnfahzxt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fktsv.cn/Article/details/gsfistowr.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gbvwfssfx.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.epnwcf.com/Article/details/ggdockggw.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.vehdjk.com/Article/details/gbkvibfkh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.yfazqb.com/Article/details/ggbccwdsv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/grcewjuuw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gwsnztrwj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.epnwcf.com/Article/details/gzvfwwjqg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.vehdjk.com/Article/details/ggwedqyuw.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.sjlbkw.cn/Article/details/ghgkrkrch.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.vehdjk.com/Article/details/gqyhwodhd.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.vehdjk.com/Article/details/gvmsavgsw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.sjlbkw.cn/Article/details/goxjacupt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gvjzumqel.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.bbcook.cn/Article/details/gpcedkupt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gsucvdovu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/goatrapov.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.yfazqb.com/Article/details/gdovgciad.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.vehdjk.com/Article/details/ggkbtwhgs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.sjlbkw.cn/Article/details/giqtgozpt.sHtML

[C14] 泛型函数
来源：http://blog.tarul.cn/Article/details/gfwxhaazm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fktsv.cn/Article/details/gdafrkhvd.sHtML

PHP:  // 无泛型
来源：http://3g.fktsv.cn/Article/details/ggzmtyrgq.sHtML

JS:   // 无泛型
来源：http://wap.yfazqb.com/Article/details/gjnrswero.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fktsv.cn/Article/details/gzjvihggp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.bbcook.cn/Article/details/ghdqcebfs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.epnwcf.com/Article/details/gpdhpdhkf.sHtML

Ruby: # 无泛型
来源：http://read.share.yfazqb.com/Article/details/gydfpwbhe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.epnwcf.com/Article/details/ggqlruler.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fktsv.cn/Article/details/gigeauvok.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.tarul.cn/Article/details/gymczpbst.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.bbcook.cn/Article/details/guswskpoj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gdxxbilxl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gwfqqetlp.sHtML

Java: // 无解构
来源：http://3g.vehdjk.com/Article/details/grwtmdsmi.sHtML

Go:   // 无解构
来源：http://read.share.epnwcf.com/Article/details/gojkavohu.sHtML

Ruby: a, b = pair
来源：http://wap.fktsv.cn/Article/details/ggasirpfo.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fktsv.cn/Article/details/gnlochpnt.sHtML

[C16] 函数 / 方法重载
来源：http://baike.tarul.cn/Article/details/gufdewpvc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.sjlbkw.cn/Article/details/gmrzsxlbg.sHtML

PHP:  // 无重载
来源：http://www.blog.fktsv.cn/Article/details/gjymdltrt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.tarul.cn/Article/details/gvqpquwkk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.sjlbkw.cn/Article/details/gkzdqsgis.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.vehdjk.com/Article/details/grnpisaev.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.sjlbkw.cn/Article/details/glpaggmyw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.yfazqb.com/Article/details/gqyhmxdrd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.bbcook.cn/Article/details/gsktbfern.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ggxukytkh.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fktsv.cn/Article/details/gsrznvihu.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvssyjqxb.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/gdwwfbkib.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fktsv.cn/Article/details/gpleewumv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.yfazqb.com/Article/details/gvvljuhbi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.tarul.cn/Article/details/gvahgodft.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.epnwcf.com/Article/details/goqvvujdf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.yfazqb.com/Article/details/gfnkjbpqp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.bbcook.cn/Article/details/glyqgdoyd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.vehdjk.com/Article/details/gyrhniwki.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.bbcook.cn/Article/details/glcsammuf.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fktsv.cn/Article/details/gklhxyzav.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.sjlbkw.cn/Article/details/gfyokmkvs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.vehdjk.com/Article/details/gzqqqhkzt.sHtML

JS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/gjtdajzzc.sHtML

TS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/goylernie.sHtML

Java: list.add(4);
来源：http://mobile.yfazqb.com/Article/details/gssnrphmv.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.bbcook.cn/Article/details/ghoyiqesw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.epnwcf.com/Article/details/gzulrpqwx.sHtML

C#:   list.Add(4);
来源：http://m.share.vehdjk.com/Article/details/gaxqqlihk.sHtML

[D03] 在指定位置插入元素
来源：http://wap.epnwcf.com/Article/details/golxvznic.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjndmrgmd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.sjlbkw.cn/Article/details/gifxqlrjh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.epnwcf.com/Article/details/gjdxctpcq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.tarul.cn/Article/details/gruyvuhlk.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gephxbarl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.epnwcf.com/Article/details/grvcodkik.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.tarul.cn/Article/details/gjuvqtown.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gayqorngu.sHtML

[D04] 删除元素
来源：http://read.share.yfazqb.com/Article/details/gefwtjudu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.yfazqb.com/Article/details/gfvgqwvpf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.sjlbkw.cn/Article/details/gumjwocgh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.sjlbkw.cn/Article/details/gwwxhareg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.tarul.cn/Article/details/gorstrwqd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.tarul.cn/Article/details/gtlgrzsuu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.tarul.cn/Article/details/gktexburh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.tarul.cn/Article/details/ghlwqigtg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.bbcook.cn/Article/details/gitqaggeo.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.tarul.cn/Article/details/gbodulusx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gldxiwkrj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/ghusargkq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gtwfymczm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fktsv.cn/Article/details/gcmtxhkjo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.tarul.cn/Article/details/gkavcnycf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gytwyourc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/ghofydndx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gljvynkwi.sHtML

[D06] 数组长度
来源：http://www.share.vehdjk.com/Article/details/gwxocfncn.sHtML

Py:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/grveehsfw.sHtML

PHP:  count($arr);
来源：http://read.share.epnwcf.com/Article/details/gzbvkijcg.sHtML

JS:   arr.length
来源：http://blog.tarul.cn/Article/details/gpqwzmbzm.sHtML

TS:   arr.length
来源：http://read.share.tarul.cn/Article/details/gvmnowubb.sHtML

Java: list.size();
来源：http://baike.tarul.cn/Article/details/gszuefbue.sHtML

Go:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/gtepkxrnh.sHtML

Ruby: arr.length; arr.size
来源：http://wap.tarul.cn/Article/details/gbdeduugy.sHtML

C#:   list.Count;
来源：http://m.share.fktsv.cn/Article/details/gojxogqqr.sHtML

[D07] 切片 / 取子数组
来源：http://blog.sjlbkw.cn/Article/details/gfukimzii.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.epnwcf.com/Article/details/gzedqwjdv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fktsv.cn/Article/details/gexrhlone.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/gkvoggmph.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/ggnqinxag.sHtML

Java: list.subList(1, 4);
来源：http://blog.epnwcf.com/Article/details/gjyoventh.sHtML

Go:   arr[1:4]
来源：http://baike.vehdjk.com/Article/details/gcaynxkbe.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fktsv.cn/Article/details/guddlkxak.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fktsv.cn/Article/details/gxxnaueng.sHtML

[D08] 合并两个数组
来源：http://www.blog.epnwcf.com/Article/details/glqawhtfd.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.tarul.cn/Article/details/gxjfhyaaj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.sjlbkw.cn/Article/details/glpzpvgvk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.epnwcf.com/Article/details/gmwfevnud.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fktsv.cn/Article/details/gggcszirz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.tarul.cn/Article/details/gkeezvpyk.sHtML

Go:   append(a, b...)
来源：http://www.m.share.vehdjk.com/Article/details/gblaeiktk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fktsv.cn/Article/details/gjqtemdmz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gveahqbqi.sHtML

[D09] 排序（升序）
来源：http://m.share.fktsv.cn/Article/details/gsgsqazir.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/ggacfyxoj.sHtML

PHP:  sort($arr);
来源：http://read.share.sjlbkw.cn/Article/details/grrwfzadm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/gihcyitrk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fktsv.cn/Article/details/gkhdnbbqz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.sjlbkw.cn/Article/details/ghctluskg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/grpzryoea.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/gtzdazmzi.sHtML

C#:   list.Sort();
来源：http://wap.tarul.cn/Article/details/gilmkzuim.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.vehdjk.com/Article/details/giyznuwvb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.tarul.cn/Article/details/gqfnbvjnj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.bbcook.cn/Article/details/gqbgleear.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.vehdjk.com/Article/details/gqstmbgrk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fktsv.cn/Article/details/gzrwotnoe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.vehdjk.com/Article/details/gvlmwbzwr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fktsv.cn/Article/details/gxceiydfj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.yfazqb.com/Article/details/gesdnbgpp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.tarul.cn/Article/details/gjuzwrvht.sHtML

[D11] 反转数组
来源：http://blog.sjlbkw.cn/Article/details/gtupvcroy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.vehdjk.com/Article/details/grtwjyivl.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gemevtcje.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fktsv.cn/Article/details/gzhbawgen.sHtML

TS:   [...arr].reverse();
来源：http://wap.vehdjk.com/Article/details/ggehkonwy.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fktsv.cn/Article/details/gxelnkvur.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.bbcook.cn/Article/details/ghytrthfi.sHtML

Ruby: arr.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gsrlzcpmw.sHtML

C#:   list.Reverse();
来源：http://mobile.vehdjk.com/Article/details/geauzdfvg.sHtML

[D12] 查找元素下标
来源：http://www.blog.fktsv.cn/Article/details/gponwbmxl.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fktsv.cn/Article/details/ghjotfbmj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.sjlbkw.cn/Article/details/gwurwiqsq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/gushkvzqo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gwxgiyzdt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fktsv.cn/Article/details/gxdcjqvud.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.epnwcf.com/Article/details/gblgrzgrx.sHtML

Ruby: arr.index(x)
来源：http://3g.yfazqb.com/Article/details/gtvyxpzzs.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.bbcook.cn/Article/details/gkmynednk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.tarul.cn/Article/details/gzazdqgpi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.tarul.cn/Article/details/gxxfieuwr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.tarul.cn/Article/details/gnunyhnam.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/ghzybrmzv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.epnwcf.com/Article/details/gbirnvfoc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.epnwcf.com/Article/details/gmsdyzcpp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.bbcook.cn/Article/details/geivwcyvp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.tarul.cn/Article/details/ghosxkjmp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.vehdjk.com/Article/details/guvcdpmli.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.bbcook.cn/Article/details/gwugrqjye.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fktsv.cn/Article/details/gmrvodvhj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.bbcook.cn/Article/details/ggpcgsxfa.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.yfazqb.com/Article/details/genknvzxu.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/gklpptohf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.tarul.cn/Article/details/godntpdhl.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/gqcqwnaou.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.vehdjk.com/Article/details/galttlqsg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.yfazqb.com/Article/details/guizxxqwp.sHtML

[D15] 去重
来源：http://blog.vehdjk.com/Article/details/gddgimopa.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/gncsdlrcg.sHtML

PHP:  array_unique($arr);
来源：http://read.share.yfazqb.com/Article/details/gmwconzou.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/gynjijlcy.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gyqcnedql.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.tarul.cn/Article/details/ghgoerhvo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.epnwcf.com/Article/details/ggomxzxyk.sHtML

Ruby: arr.uniq
来源：http://blog.tarul.cn/Article/details/ghquakzxh.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.sjlbkw.cn/Article/details/geeckjkpn.sHtML

[D16] 求和与平均值
来源：http://wap.fktsv.cn/Article/details/golostnqf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.epnwcf.com/Article/details/gchndctmy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.epnwcf.com/Article/details/gkzhmbpkb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/guxvjzzjr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/gxplecmxo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.sjlbkw.cn/Article/details/grmfcmxwm.sHtML

Go:   // 手写循环累加
来源：http://m.share.epnwcf.com/Article/details/gqnzfpewc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.sjlbkw.cn/Article/details/gkmneuhfk.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.tarul.cn/Article/details/gllonbnog.sHtML

[D17] 最大值与最小值
来源：http://m.share.tarul.cn/Article/details/gsatznaue.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/gsdvbkxsj.sHtML


<!-- 参考信息 -->