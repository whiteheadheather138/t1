代发 wailian999

C#:   x is int or double or decimal
来源：http://blog.epnwcf.com/Article/details/gmemwejfq.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrrwmlcr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.tarul.cn/Article/details/gkruefupq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.epnwcf.com/Article/details/gpfgwjtak.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/glgfbkpam.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.bbcook.cn/Article/details/gzgmnvojk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.epnwcf.com/Article/details/ghkfvrmzd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.tarul.cn/Article/details/gknkexbrh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fktsv.cn/Article/details/gvarftkyx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.tarul.cn/Article/details/gegrionyn.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.vehdjk.com/Article/details/gfcyqnoov.sHtML

Py:   a and b or not c
来源：http://blog.vehdjk.com/Article/details/gftsjuswj.sHtML

PHP:  $a && $b || !$c
来源：http://blog.sjlbkw.cn/Article/details/ggseekltv.sHtML

JS:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gzimqdrdn.sHtML

TS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gdzveqgug.sHtML

Java: a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/ggkoonbcy.sHtML

Go:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gcwpjzzpi.sHtML

Ruby: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gfisfhpem.sHtML

C#:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/grhvguabe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.bbcook.cn/Article/details/gadxgjviq.sHtML

Py:   if not data: return
来源：http://mobile.fktsv.cn/Article/details/gmwtuispb.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.epnwcf.com/Article/details/grqdbuxrv.sHtML

JS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gvecmdnrr.sHtML

TS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/gspnksuaa.sHtML

Java: if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/ggklvdpyc.sHtML

Go:   if data == nil { return }
来源：http://mobile.fktsv.cn/Article/details/gtcgtjseu.sHtML

Ruby: return if data.nil?
来源：http://3g.sjlbkw.cn/Article/details/gasnghaix.sHtML

C#:   if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/gxlkuwsqe.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqfsqmagu.sHtML

C. 函数与作用域
来源：http://www.m.share.epnwcf.com/Article/details/gdasudwag.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gybgmpiww.sHtML

[C01] 定义函数
来源：http://read.share.tarul.cn/Article/details/gyualbupu.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.tarul.cn/Article/details/grdgylgxz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gideejkxw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gketskhcj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gbevojoqb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gfqofilrt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.sjlbkw.cn/Article/details/gvhgacqxz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.tarul.cn/Article/details/ghymidncd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/ghqdykopq.sHtML

[C02] 默认参数
来源：http://mobile.yfazqb.com/Article/details/gwvhjfzlg.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.bbcook.cn/Article/details/grfjiwfvj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.yfazqb.com/Article/details/ggdjnfzva.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gqoupuclu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gnodzwxkf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.sjlbkw.cn/Article/details/gelsthehl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.yfazqb.com/Article/details/gxdtxqsda.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.vehdjk.com/Article/details/gvsaseicm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fktsv.cn/Article/details/guykdcusn.sHtML

[C03] 可变参数
来源：http://www.m.share.vehdjk.com/Article/details/gufddlhzm.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.epnwcf.com/Article/details/gnazqetwf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fktsv.cn/Article/details/gfrkrwuhk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gbxrahtjq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/gbakpicif.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.tarul.cn/Article/details/gstwickhz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.bbcook.cn/Article/details/glqztnpsj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.vehdjk.com/Article/details/ggciexnvq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fktsv.cn/Article/details/gdizhdbno.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.bbcook.cn/Article/details/gtpcxlkry.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fktsv.cn/Article/details/gyijcwhzm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.vehdjk.com/Article/details/glwjzhygq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/gczsjsfdn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.tarul.cn/Article/details/glsemrdcb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.yfazqb.com/Article/details/ggdwfsfdi.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fktsv.cn/Article/details/gnoziryxg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gakpswkbq.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/ghpzqwjqj.sHtML

[C05] 返回多个值
来源：http://www.blog.sjlbkw.cn/Article/details/gqnnodurq.sHtML

Py:   return a, b
来源：http://wap.fktsv.cn/Article/details/grwdihpdg.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fktsv.cn/Article/details/gsuuvqvsc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gonyhnnbm.sHtML

TS:   return { a, b };
来源：http://3g.vehdjk.com/Article/details/gsxucsnvc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.vehdjk.com/Article/details/gclbvfjpd.sHtML

Go:   return a, b
来源：http://3g.fktsv.cn/Article/details/gloovmpnq.sHtML

Ruby: return a, b
来源：http://wap.tarul.cn/Article/details/gfjmvmldv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.vehdjk.com/Article/details/gdheljhfd.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/grwghbepx.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fktsv.cn/Article/details/gwnrdymno.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fktsv.cn/Article/details/gsyewrisa.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.bbcook.cn/Article/details/gujqwiekx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/ggtwuertp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.tarul.cn/Article/details/gvyhssruf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.sjlbkw.cn/Article/details/gdwuwervi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.yfazqb.com/Article/details/gfijciasq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gwsafcrmb.sHtML

[C07] 把函数作为参数传入
来源：http://wap.bbcook.cn/Article/details/gdkrlwnrn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.epnwcf.com/Article/details/gsvbywiav.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.bbcook.cn/Article/details/gcorpqxsl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fktsv.cn/Article/details/gfdyxsqzc.sHtML

TS:   arr.map(String)
来源：http://mobile.bbcook.cn/Article/details/ghjwcwhyu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdavjifii.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.yfazqb.com/Article/details/grlplejuz.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.sjlbkw.cn/Article/details/gihvuciae.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.epnwcf.com/Article/details/gcsdglvpf.sHtML

[C08] 闭包
来源：http://m.share.bbcook.cn/Article/details/gmkqcqyzl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.yfazqb.com/Article/details/gtnwjunto.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.yfazqb.com/Article/details/gdpiqjgzm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gwegrtryc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gaeiglwdd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.yfazqb.com/Article/details/gtaardclm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.yfazqb.com/Article/details/gplxckdvn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.sjlbkw.cn/Article/details/grpdnziae.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gxredoxgk.sHtML

[C09] 递归
来源：http://wap.yfazqb.com/Article/details/grycdlkex.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gxaepqgvb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.sjlbkw.cn/Article/details/gpbdobdoh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/gzfegdfil.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fktsv.cn/Article/details/gpejpvpab.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fktsv.cn/Article/details/guzvzpiua.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.tarul.cn/Article/details/gogttnxtx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/grwksptez.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.bbcook.cn/Article/details/gwzctgupd.sHtML

[C10] 变量作用域
来源：http://baike.vehdjk.com/Article/details/gurnbytcv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.vehdjk.com/Article/details/ghrortfzb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.vehdjk.com/Article/details/gqbectrvy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.yfazqb.com/Article/details/gpjccfiia.sHtML

TS:   同 JS
来源：http://baike.tarul.cn/Article/details/geisgbton.sHtML

Java: 方法内为块级作用域
来源：http://m.share.bbcook.cn/Article/details/gjvawymml.sHtML

Go:   花括号块级作用域
来源：http://mobile.vehdjk.com/Article/details/gaelffdjw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.yfazqb.com/Article/details/gkejmgdqd.sHtML

C#:   块级作用域
来源：http://read.share.bbcook.cn/Article/details/gvjiwdpkl.sHtML

[C11] 模块导入与导出
来源：http://baike.fktsv.cn/Article/details/gpssyervr.sHtML

Py:   from module import func
来源：http://read.share.fktsv.cn/Article/details/gkxoikfpf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.yfazqb.com/Article/details/gjgvnzgzy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.yfazqb.com/Article/details/grdfyvykv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fktsv.cn/Article/details/gggsoouve.sHtML

Java: import java.util.List;
来源：http://www.m.share.vehdjk.com/Article/details/gsbdmuuau.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fktsv.cn/Article/details/gwdwexikl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.epnwcf.com/Article/details/gvsyhttvx.sHtML

C#:   using System.Text;
来源：http://blog.vehdjk.com/Article/details/gqlxszkbx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.bbcook.cn/Article/details/gfvdoxfhd.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.yfazqb.com/Article/details/gbdyfbuqu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.epnwcf.com/Article/details/gzyaxhykw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/gjfyygrvy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gtoxzmvpl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.vehdjk.com/Article/details/gvvkymruy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.bbcook.cn/Article/details/glhnombms.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.sjlbkw.cn/Article/details/grqvofvcr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.tarul.cn/Article/details/gkkpxriol.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.epnwcf.com/Article/details/gxbmalajo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.yfazqb.com/Article/details/grerhfipn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gjlowrwro.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.tarul.cn/Article/details/gxgddvhvh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gxedtlzap.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/glwoxogpy.sHtML

Go:   func add(a, b int) int
来源：http://3g.sjlbkw.cn/Article/details/ghmahhgft.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.tarul.cn/Article/details/gyqqrdhng.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.epnwcf.com/Article/details/gaeevrnrh.sHtML

[C14] 泛型函数
来源：http://www.share.yfazqb.com/Article/details/gjpiqhfyz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.vehdjk.com/Article/details/gctvyropk.sHtML

PHP:  // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gfdkzhntb.sHtML

JS:   // 无泛型
来源：http://blog.tarul.cn/Article/details/gwhelzhrc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.yfazqb.com/Article/details/gasfbizhl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/ginyqrvng.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.yfazqb.com/Article/details/glulfynhw.sHtML

Ruby: # 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gayzvforo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.yfazqb.com/Article/details/gbfecirtj.sHtML

[C15] 解构 / 展开参数
来源：http://3g.bbcook.cn/Article/details/guqgfwmbv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.sjlbkw.cn/Article/details/gxrqfkdst.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fktsv.cn/Article/details/gxrgeqvqw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/glwlcexws.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.yfazqb.com/Article/details/ggkvpznpr.sHtML

Java: // 无解构
来源：http://blog.fktsv.cn/Article/details/ggwdkresc.sHtML

Go:   // 无解构
来源：http://www.share.fktsv.cn/Article/details/gclwbrcuu.sHtML

Ruby: a, b = pair
来源：http://baike.sjlbkw.cn/Article/details/gxefakkrb.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.tarul.cn/Article/details/gbfrpondw.sHtML

[C16] 函数 / 方法重载
来源：http://wap.vehdjk.com/Article/details/gbuwznjyg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.vehdjk.com/Article/details/gkgdxoxfn.sHtML

PHP:  // 无重载
来源：http://blog.fktsv.cn/Article/details/gpvjiraak.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.vehdjk.com/Article/details/grjfiigwq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.tarul.cn/Article/details/gtgqkstnf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.epnwcf.com/Article/details/gsshxlkcx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.yfazqb.com/Article/details/gibumsfpi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.epnwcf.com/Article/details/guhvfhvuy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.vehdjk.com/Article/details/guherelzp.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gsxsqehjv.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.tarul.cn/Article/details/gtohycxrl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ghskvdise.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gjdsvqrgv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.sjlbkw.cn/Article/details/gpqxuuyow.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.tarul.cn/Article/details/gyswkgqpt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.vehdjk.com/Article/details/gmnvfascg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.tarul.cn/Article/details/gmmroikdh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.tarul.cn/Article/details/gmrwuaufk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.yfazqb.com/Article/details/gasbdzoij.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.tarul.cn/Article/details/gdgvrdevx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.vehdjk.com/Article/details/guzvbkjow.sHtML

[D02] 追加元素到末尾
来源：http://wap.fktsv.cn/Article/details/gqqmzazww.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.vehdjk.com/Article/details/gdytbokby.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fktsv.cn/Article/details/gpvqktvou.sHtML

JS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/ghglucdpl.sHtML

TS:   arr.push(4);
来源：http://read.share.tarul.cn/Article/details/ghleqhagx.sHtML

Java: list.add(4);
来源：http://www.m.share.yfazqb.com/Article/details/golazpokw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.epnwcf.com/Article/details/ggeaonrsk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.tarul.cn/Article/details/gtnolelkm.sHtML

C#:   list.Add(4);
来源：http://baike.yfazqb.com/Article/details/gelqesnrr.sHtML

[D03] 在指定位置插入元素
来源：http://3g.tarul.cn/Article/details/ghfjhaxap.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.yfazqb.com/Article/details/gmstxbxya.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.tarul.cn/Article/details/gpwvigidp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fktsv.cn/Article/details/gnxycjjii.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.yfazqb.com/Article/details/gmmpjgfpj.sHtML

Java: list.add(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/glqaqbijv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.vehdjk.com/Article/details/gqyyrymey.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fktsv.cn/Article/details/gfelwbyjf.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.bbcook.cn/Article/details/gggkyitjr.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/gvgtqkdvh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.bbcook.cn/Article/details/gmbkbrtpb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fktsv.cn/Article/details/gaunknvfc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.yfazqb.com/Article/details/gfjtugrox.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.sjlbkw.cn/Article/details/gabveplvj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.sjlbkw.cn/Article/details/gshcffupz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.tarul.cn/Article/details/gxrwwgdfx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.epnwcf.com/Article/details/gokclpmhu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.tarul.cn/Article/details/gvsveizkv.sHtML

[D05] 访问与修改元素
来源：http://m.share.bbcook.cn/Article/details/ghfpqrnff.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/ggabykumw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gkxzfvsst.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gsnmrnasp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fktsv.cn/Article/details/gpmbkxbev.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.tarul.cn/Article/details/gcqlmfxdh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gzshrtuzl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gblvhowwh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gvdcjqzhz.sHtML

[D06] 数组长度
来源：http://baike.tarul.cn/Article/details/gcdmvqnjs.sHtML

Py:   len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gaablilwc.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gkqcydnfu.sHtML

JS:   arr.length
来源：http://wap.epnwcf.com/Article/details/grrvhkbst.sHtML

TS:   arr.length
来源：http://blog.bbcook.cn/Article/details/gpwvnoznx.sHtML

Java: list.size();
来源：http://www.m.share.fktsv.cn/Article/details/gwchfdqlj.sHtML

Go:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/ggcyzbpjy.sHtML

Ruby: arr.length; arr.size
来源：http://3g.vehdjk.com/Article/details/gdnziyetv.sHtML

C#:   list.Count;
来源：http://www.m.share.fktsv.cn/Article/details/gtbzsawxc.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.tarul.cn/Article/details/gvjvcykor.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.epnwcf.com/Article/details/gpgurbdnh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.tarul.cn/Article/details/gxrnrwaqr.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/ghddqacux.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gqxpqloqk.sHtML

Java: list.subList(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/ggloaryzi.sHtML

Go:   arr[1:4]
来源：http://mobile.epnwcf.com/Article/details/gpudmaoom.sHtML

Ruby: arr[1, 3]
来源：http://read.share.vehdjk.com/Article/details/gcgwfvfty.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gxrzjhpkh.sHtML

[D08] 合并两个数组
来源：http://mobile.sjlbkw.cn/Article/details/gljskomyk.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fktsv.cn/Article/details/gfzgdgaey.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.yfazqb.com/Article/details/gsyzpqrwc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.sjlbkw.cn/Article/details/gqxizzcvd.sHtML

TS:   [...a, ...b];
来源：http://m.share.epnwcf.com/Article/details/gocbjqnyf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.sjlbkw.cn/Article/details/gehvyorwx.sHtML

Go:   append(a, b...)
来源：http://3g.fktsv.cn/Article/details/ghelgjcnm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.yfazqb.com/Article/details/gihhhgpcs.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fktsv.cn/Article/details/gdrwwvuok.sHtML

[D09] 排序（升序）
来源：http://blog.sjlbkw.cn/Article/details/gxymgnful.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gtzmbjuqe.sHtML

PHP:  sort($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gmvcikzow.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.epnwcf.com/Article/details/ggzgpminx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.vehdjk.com/Article/details/gylzvowbj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.vehdjk.com/Article/details/gtvyjaihc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.tarul.cn/Article/details/gxxzdvtga.sHtML

Ruby: arr.sort
来源：http://www.blog.fktsv.cn/Article/details/gdkfnhyyt.sHtML

C#:   list.Sort();
来源：http://www.blog.tarul.cn/Article/details/gqpkjsmam.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.bbcook.cn/Article/details/gjaqkfrds.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.tarul.cn/Article/details/gorwicguy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gijsbhodz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.vehdjk.com/Article/details/gguovwsuo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.epnwcf.com/Article/details/gfgfvjuvj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.tarul.cn/Article/details/gshfypltm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fktsv.cn/Article/details/gndoehxnw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.sjlbkw.cn/Article/details/ggwdeenac.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.epnwcf.com/Article/details/gmzwairxy.sHtML

[D11] 反转数组
来源：http://blog.yfazqb.com/Article/details/gtztrtzca.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.epnwcf.com/Article/details/ghxycszbz.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.yfazqb.com/Article/details/gwcsvhpos.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.yfazqb.com/Article/details/gqmwawsht.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fktsv.cn/Article/details/gujdbfslh.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gykqojuiy.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fktsv.cn/Article/details/gmjtubwgf.sHtML

Ruby: arr.reverse
来源：http://m.share.fktsv.cn/Article/details/gpczbjbrx.sHtML

C#:   list.Reverse();
来源：http://www.share.fktsv.cn/Article/details/gugabyepk.sHtML

[D12] 查找元素下标
来源：http://read.share.tarul.cn/Article/details/gxkcutrch.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.epnwcf.com/Article/details/gfkcisofj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.vehdjk.com/Article/details/goafxmmrc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gpqnnrobx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.epnwcf.com/Article/details/gplwdbfqd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.tarul.cn/Article/details/gmggpoemq.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.epnwcf.com/Article/details/gmertmjxp.sHtML

Ruby: arr.index(x)
来源：http://read.share.tarul.cn/Article/details/gornasigh.sHtML

C#:   list.IndexOf(x);
来源：http://wap.sjlbkw.cn/Article/details/gxpojkewl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.sjlbkw.cn/Article/details/gscueurpr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gkdmkdekw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.bbcook.cn/Article/details/glyraushc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gssdqbrxw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gqfjdbmoy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fktsv.cn/Article/details/gdfjgorms.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.epnwcf.com/Article/details/gaebdskhs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.bbcook.cn/Article/details/ghytwjqtn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gpyitwnep.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.yfazqb.com/Article/details/gstvvayvo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.vehdjk.com/Article/details/gbquezdmq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.tarul.cn/Article/details/gycvktfmm.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.bbcook.cn/Article/details/gffcylpoe.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/geqvieaop.sHtML


<!-- 参考信息 -->