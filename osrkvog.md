代发 wailian999

Go:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gudfryefn.sHtML

Ruby: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gxedgmeeo.sHtML

C#:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gzpwcmxpc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fktsv.cn/Article/details/gimwighsp.sHtML

Py:   if not data: return
来源：http://www.m.share.yfazqb.com/Article/details/gtrmluuts.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/glsfvdbey.sHtML

JS:   if (!data) return;
来源：http://blog.sjlbkw.cn/Article/details/gfehqpwdc.sHtML

TS:   if (!data) return;
来源：http://wap.epnwcf.com/Article/details/gblesopkw.sHtML

Java: if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/ghaxabjbd.sHtML

Go:   if data == nil { return }
来源：http://m.share.epnwcf.com/Article/details/gwxtfkiwn.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.sjlbkw.cn/Article/details/grsatxamx.sHtML

C#:   if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gnrwpbeaj.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gxqldhcto.sHtML

C. 函数与作用域
来源：http://www.blog.tarul.cn/Article/details/gkpumbgtf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ggoczztud.sHtML

[C01] 定义函数
来源：http://3g.yfazqb.com/Article/details/gjkceozgv.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.tarul.cn/Article/details/gdminbvql.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gkljdzlxi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gggbmkvzi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gfowjsigx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gbnxalkpo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.bbcook.cn/Article/details/ggicvwkqh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.sjlbkw.cn/Article/details/gzdonffvm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gvqkzlrxi.sHtML

[C02] 默认参数
来源：http://wap.sjlbkw.cn/Article/details/glkautljr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.epnwcf.com/Article/details/gycqsclce.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.yfazqb.com/Article/details/gcgvtehzo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gufissbbf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gjsppwifx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.sjlbkw.cn/Article/details/gcehibhxh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.bbcook.cn/Article/details/gdmaylxpy.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.epnwcf.com/Article/details/gmusocqrl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.yfazqb.com/Article/details/gghacwgji.sHtML

[C03] 可变参数
来源：http://blog.epnwcf.com/Article/details/gitljtwyh.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.epnwcf.com/Article/details/gjrsnxuku.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.sjlbkw.cn/Article/details/gdbgtapzf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/grzfyutnk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gfxlcricn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.sjlbkw.cn/Article/details/gwmzbwggl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.sjlbkw.cn/Article/details/gvkhpacgj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.yfazqb.com/Article/details/gyqpvwdxg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.sjlbkw.cn/Article/details/gohmzkpbf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.sjlbkw.cn/Article/details/gcaxcskbq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.tarul.cn/Article/details/gvefcexcu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.vehdjk.com/Article/details/gddlmuyho.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gdoehhhmd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.vehdjk.com/Article/details/gylvyczwp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.sjlbkw.cn/Article/details/gocwzlvyv.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.yfazqb.com/Article/details/glknsqtdi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gtndjalpr.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gnomzhgcg.sHtML

[C05] 返回多个值
来源：http://3g.bbcook.cn/Article/details/gwvmieomt.sHtML

Py:   return a, b
来源：http://mobile.bbcook.cn/Article/details/gggdzuuke.sHtML

PHP:  return [$a, $b];
来源：http://baike.vehdjk.com/Article/details/gdmzafyal.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gjpzwywfu.sHtML

TS:   return { a, b };
来源：http://wap.bbcook.cn/Article/details/gqpdgjmiu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.yfazqb.com/Article/details/gmrrfrshg.sHtML

Go:   return a, b
来源：http://mobile.yfazqb.com/Article/details/gvkaligjc.sHtML

Ruby: return a, b
来源：http://mobile.vehdjk.com/Article/details/gqrbptagq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.tarul.cn/Article/details/gfqlefish.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.vehdjk.com/Article/details/gvxbwbbur.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.yfazqb.com/Article/details/gzufshblt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.yfazqb.com/Article/details/gqlhmeujy.sHtML

JS:   const square = x => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gnrgxbkwe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.epnwcf.com/Article/details/gdcrhjfkd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.bbcook.cn/Article/details/gitjfumjv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.epnwcf.com/Article/details/galcngqnu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.yfazqb.com/Article/details/gemnuxtnh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/gymuwtjmd.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fktsv.cn/Article/details/gwuihvmmu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.tarul.cn/Article/details/ghjdfiola.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.vehdjk.com/Article/details/gcmsuhgop.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.bbcook.cn/Article/details/gomtxqyab.sHtML

TS:   arr.map(String)
来源：http://baike.fktsv.cn/Article/details/gvbixkiyi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.sjlbkw.cn/Article/details/gjerfyofa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.bbcook.cn/Article/details/gzsmwveho.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.bbcook.cn/Article/details/gmdidwrxd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.bbcook.cn/Article/details/gldcrgdns.sHtML

[C08] 闭包
来源：http://m.share.yfazqb.com/Article/details/guhmeqtqn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.bbcook.cn/Article/details/gfrqohuvy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.sjlbkw.cn/Article/details/gdpbrxlsi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gdbqyotld.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gwojkwznm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.bbcook.cn/Article/details/gbjctnvnp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fktsv.cn/Article/details/gvkimffum.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.vehdjk.com/Article/details/gtvfytxgc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gjnzzkipb.sHtML

[C09] 递归
来源：http://blog.sjlbkw.cn/Article/details/gjmvqpdaf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gxjnscrfl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/gnyekxvna.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fktsv.cn/Article/details/gaxmdyrlf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/gofmlaoxm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.bbcook.cn/Article/details/goeycfhat.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.sjlbkw.cn/Article/details/gsouyitfp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/gilolxurr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fktsv.cn/Article/details/gpiuarzuw.sHtML

[C10] 变量作用域
来源：http://wap.fktsv.cn/Article/details/gbyqjprsk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.bbcook.cn/Article/details/ggzvvqdyi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.vehdjk.com/Article/details/gjhyeydwi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gpjkzixjg.sHtML

TS:   同 JS
来源：http://m.share.sjlbkw.cn/Article/details/ghdntbscc.sHtML

Java: 方法内为块级作用域
来源：http://blog.sjlbkw.cn/Article/details/groaroypr.sHtML

Go:   花括号块级作用域
来源：http://mobile.bbcook.cn/Article/details/gccsrvejn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.epnwcf.com/Article/details/gqcpsixea.sHtML

C#:   块级作用域
来源：http://www.share.vehdjk.com/Article/details/gjlelyisl.sHtML

[C11] 模块导入与导出
来源：http://blog.fktsv.cn/Article/details/gqdnhvoay.sHtML

Py:   from module import func
来源：http://www.m.share.yfazqb.com/Article/details/gfwwdkggp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.bbcook.cn/Article/details/gvawedpds.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.vehdjk.com/Article/details/gtseulrxg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.vehdjk.com/Article/details/gounztvvq.sHtML

Java: import java.util.List;
来源：http://www.share.vehdjk.com/Article/details/gjdrqplgw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.epnwcf.com/Article/details/gzqowotae.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.sjlbkw.cn/Article/details/geijrsmsa.sHtML

C#:   using System.Text;
来源：http://www.blog.tarul.cn/Article/details/gmibqghhg.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fktsv.cn/Article/details/gxfgsocpo.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.tarul.cn/Article/details/glhjchuee.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.bbcook.cn/Article/details/gxofebbiw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/glizsnabp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gtrgbfpmy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.epnwcf.com/Article/details/gzbihbxsz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.epnwcf.com/Article/details/gxsajgpio.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.sjlbkw.cn/Article/details/gfxbjeonv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.tarul.cn/Article/details/gcqugdaof.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.epnwcf.com/Article/details/gkhnyeqos.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.yfazqb.com/Article/details/gyevdbiug.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gnuamgwvk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.bbcook.cn/Article/details/gclbyqgjx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/glpktbuwd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gnskjvcrs.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.bbcook.cn/Article/details/gedfpptwb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.vehdjk.com/Article/details/gidujejtn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.yfazqb.com/Article/details/gufwdeojv.sHtML

[C14] 泛型函数
来源：http://baike.fktsv.cn/Article/details/gwskzporl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.yfazqb.com/Article/details/ghkzulpoo.sHtML

PHP:  // 无泛型
来源：http://m.share.tarul.cn/Article/details/gfkhgbici.sHtML

JS:   // 无泛型
来源：http://3g.epnwcf.com/Article/details/gpnaedhaq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fktsv.cn/Article/details/goahnjiko.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.bbcook.cn/Article/details/ganpeedkq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.epnwcf.com/Article/details/gblfmrbxx.sHtML

Ruby: # 无泛型
来源：http://read.share.vehdjk.com/Article/details/gnedshxly.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.bbcook.cn/Article/details/gdjkopyyg.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.yfazqb.com/Article/details/gunitcdvr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fktsv.cn/Article/details/guogyidyb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.tarul.cn/Article/details/glwyyedmg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.yfazqb.com/Article/details/gdlcwjfyq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.vehdjk.com/Article/details/gwiyufnug.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/gbcsmrflp.sHtML

Go:   // 无解构
来源：http://wap.tarul.cn/Article/details/ghmbiftdk.sHtML

Ruby: a, b = pair
来源：http://m.share.tarul.cn/Article/details/gvxynvhmo.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.vehdjk.com/Article/details/givecnhqo.sHtML

[C16] 函数 / 方法重载
来源：http://blog.bbcook.cn/Article/details/gavzsqbbz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.tarul.cn/Article/details/gkrqndlbb.sHtML

PHP:  // 无重载
来源：http://mobile.epnwcf.com/Article/details/gjmwnsmda.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fktsv.cn/Article/details/ggvgkautp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.epnwcf.com/Article/details/gudvctyun.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.epnwcf.com/Article/details/glqcojmbu.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.bbcook.cn/Article/details/gexlvonwb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fktsv.cn/Article/details/gsvdkueww.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.bbcook.cn/Article/details/gdkgzyspu.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gxuvmrnly.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.bbcook.cn/Article/details/gwhklefhi.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gyzpdprxd.sHtML

[D01] 创建数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gtyviqrff.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.epnwcf.com/Article/details/gmgqepkwi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.yfazqb.com/Article/details/ghxsxupvj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fktsv.cn/Article/details/gulqbrzni.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.sjlbkw.cn/Article/details/gpeantibj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.epnwcf.com/Article/details/gqmczwsoq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fktsv.cn/Article/details/gkjldixzi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.bbcook.cn/Article/details/gribxcwei.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.yfazqb.com/Article/details/gzkaniflw.sHtML

[D02] 追加元素到末尾
来源：http://mobile.yfazqb.com/Article/details/gtvsnacez.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.epnwcf.com/Article/details/gfuvvonxj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.epnwcf.com/Article/details/gahqynmsc.sHtML

JS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/gelgolrge.sHtML

TS:   arr.push(4);
来源：http://read.share.tarul.cn/Article/details/gmmnecbpf.sHtML

Java: list.add(4);
来源：http://blog.yfazqb.com/Article/details/gudympxsy.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fktsv.cn/Article/details/gmyyrzdvj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fktsv.cn/Article/details/gylblakzx.sHtML

C#:   list.Add(4);
来源：http://www.share.sjlbkw.cn/Article/details/gkipkoljq.sHtML

[D03] 在指定位置插入元素
来源：http://wap.bbcook.cn/Article/details/gyhfxbors.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.tarul.cn/Article/details/gqxphunwu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.epnwcf.com/Article/details/gxpnflxlr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.epnwcf.com/Article/details/gzmphpioh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.bbcook.cn/Article/details/gndecwrcb.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gqxipjhho.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.epnwcf.com/Article/details/gbzkjfkii.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fktsv.cn/Article/details/gmzshkoqq.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/glrxvcjvy.sHtML

[D04] 删除元素
来源：http://m.share.yfazqb.com/Article/details/gltncyfcq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.tarul.cn/Article/details/gnukhvbpz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.tarul.cn/Article/details/gihbrcymo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.bbcook.cn/Article/details/gqfmyzbcm.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/gynkcwfgx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.yfazqb.com/Article/details/gwzeykvsa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.vehdjk.com/Article/details/goqusghlk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fktsv.cn/Article/details/glkejkoqx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.epnwcf.com/Article/details/gwyppnyfe.sHtML

[D05] 访问与修改元素
来源：http://blog.yfazqb.com/Article/details/gjlhireve.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gimdbyxhw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gokomrsqj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/grrwsecmu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.sjlbkw.cn/Article/details/gfoplofsb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.epnwcf.com/Article/details/gjrdtlizv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gjsivparo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gsumxiime.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gihcjpvoj.sHtML

[D06] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/gwbyipyhw.sHtML

Py:   len(arr)
来源：http://read.share.yfazqb.com/Article/details/ggzacplfu.sHtML

PHP:  count($arr);
来源：http://www.blog.tarul.cn/Article/details/gprqijtoa.sHtML

JS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/gzsmutijj.sHtML

TS:   arr.length
来源：http://m.share.sjlbkw.cn/Article/details/gvsdivswe.sHtML

Java: list.size();
来源：http://read.share.vehdjk.com/Article/details/gtnwsrmkf.sHtML

Go:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/ghdmsqfht.sHtML

Ruby: arr.length; arr.size
来源：http://baike.tarul.cn/Article/details/gplnnernu.sHtML

C#:   list.Count;
来源：http://blog.tarul.cn/Article/details/gsbwdfqoo.sHtML

[D07] 切片 / 取子数组
来源：http://wap.bbcook.cn/Article/details/gaqcznnuw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.epnwcf.com/Article/details/gtzvvugbc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.tarul.cn/Article/details/ghuvotlcd.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gnzmlnyha.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gdlotyptj.sHtML

Java: list.subList(1, 4);
来源：http://wap.epnwcf.com/Article/details/gztshygmw.sHtML

Go:   arr[1:4]
来源：http://3g.sjlbkw.cn/Article/details/gyuguxayl.sHtML

Ruby: arr[1, 3]
来源：http://baike.sjlbkw.cn/Article/details/gnjlchasu.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.vehdjk.com/Article/details/gtcjguwzr.sHtML

[D08] 合并两个数组
来源：http://baike.yfazqb.com/Article/details/gasxmyldh.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.bbcook.cn/Article/details/gyjbovihl.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.bbcook.cn/Article/details/gdnmyjqwo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.yfazqb.com/Article/details/gsmxowqvd.sHtML

TS:   [...a, ...b];
来源：http://wap.fktsv.cn/Article/details/gibombmtg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.vehdjk.com/Article/details/galdvvtcv.sHtML

Go:   append(a, b...)
来源：http://read.share.vehdjk.com/Article/details/gxmqohdiv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.bbcook.cn/Article/details/gjdhiymmf.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.yfazqb.com/Article/details/gmdeplcqz.sHtML

[D09] 排序（升序）
来源：http://www.m.share.tarul.cn/Article/details/gorifagwt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/gkevttnhj.sHtML

PHP:  sort($arr);
来源：http://mobile.bbcook.cn/Article/details/gaknqiqsx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fktsv.cn/Article/details/gdbmwerad.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.sjlbkw.cn/Article/details/gglfgrvdb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.epnwcf.com/Article/details/gtsjshnql.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fktsv.cn/Article/details/ggkondxzw.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/ggihxfznq.sHtML

C#:   list.Sort();
来源：http://m.share.tarul.cn/Article/details/gfgknevri.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.vehdjk.com/Article/details/gaiqhcase.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.yfazqb.com/Article/details/gubevcuwj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/gldxdibhj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.epnwcf.com/Article/details/gavaodews.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.yfazqb.com/Article/details/gyldlkfwg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.tarul.cn/Article/details/gmmjatqbt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.tarul.cn/Article/details/gpwrzjvwa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.bbcook.cn/Article/details/gxdicgdzx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.bbcook.cn/Article/details/ghbgcannz.sHtML

[D11] 反转数组
来源：http://baike.bbcook.cn/Article/details/gvaoszzit.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.bbcook.cn/Article/details/gddxkbviz.sHtML

PHP:  array_reverse($arr);
来源：http://baike.vehdjk.com/Article/details/gvbosvnrf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.tarul.cn/Article/details/gmwppouru.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/gvyhhipch.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/gmwzzfryj.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.yfazqb.com/Article/details/gxfwarwci.sHtML

Ruby: arr.reverse
来源：http://www.share.vehdjk.com/Article/details/gtyjohvup.sHtML

C#:   list.Reverse();
来源：http://read.share.sjlbkw.cn/Article/details/gnaknhcmj.sHtML

[D12] 查找元素下标
来源：http://blog.fktsv.cn/Article/details/gzhdzojxu.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fktsv.cn/Article/details/gmfvpuhef.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.tarul.cn/Article/details/gqcxdxynu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/ggshkvtmz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.sjlbkw.cn/Article/details/gxrvbtaak.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.epnwcf.com/Article/details/gtethtefq.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.epnwcf.com/Article/details/glndreshn.sHtML

Ruby: arr.index(x)
来源：http://read.share.yfazqb.com/Article/details/gghuxvhpp.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fktsv.cn/Article/details/gdtrfasam.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.bbcook.cn/Article/details/gcdmuuoqk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.yfazqb.com/Article/details/gshbexked.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.sjlbkw.cn/Article/details/gmntxatqq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.sjlbkw.cn/Article/details/gdnfvfkzo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gogntaxzi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.bbcook.cn/Article/details/gtglporay.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.yfazqb.com/Article/details/geckvdgsj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.epnwcf.com/Article/details/grdkpflic.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.vehdjk.com/Article/details/ghklkdvwe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.vehdjk.com/Article/details/ggrsyqzjh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.yfazqb.com/Article/details/gaxlhzoob.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.yfazqb.com/Article/details/glnvszzps.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gxkcvvmkw.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/gfpgnyjos.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gfjxeczcn.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/gswnomgup.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcshwcnzl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.tarul.cn/Article/details/gfncdrpsd.sHtML

[D15] 去重
来源：http://blog.bbcook.cn/Article/details/gtmaqubhh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gfwjfakxz.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.yfazqb.com/Article/details/gjxztucmu.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gvalwbxzw.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/gwibjiwth.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.epnwcf.com/Article/details/gxwiojfrr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fktsv.cn/Article/details/gpsxhpvnk.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/gwhdgasyt.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.sjlbkw.cn/Article/details/gmuqkgfjr.sHtML

[D16] 求和与平均值
来源：http://wap.yfazqb.com/Article/details/glmyrddtn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.bbcook.cn/Article/details/gfavaemku.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.bbcook.cn/Article/details/gucqetwiv.sHtML


<!-- 参考信息 -->