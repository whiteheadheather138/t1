代发 wailian999

Java: if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/gmwbhjscv.sHtML

Go:   if data == nil { return }
来源：http://mobile.sjlbkw.cn/Article/details/gvyrcyskc.sHtML

Ruby: return if data.nil?
来源：http://www.blog.epnwcf.com/Article/details/gtbovqrwn.sHtML

C#:   if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gjccolodo.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbuuiecsy.sHtML

C. 函数与作用域
来源：http://blog.vehdjk.com/Article/details/guuqhgjas.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/goidxccgc.sHtML

[C01] 定义函数
来源：http://read.share.yfazqb.com/Article/details/ghfhtedel.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.bbcook.cn/Article/details/geqdfdqyn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/ghvkhydch.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/ggiwndiqd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/guhtebhhg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gbiwryaxr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fktsv.cn/Article/details/gkgsxegio.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.vehdjk.com/Article/details/gacscyveu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gvdwyiomz.sHtML

[C02] 默认参数
来源：http://wap.fktsv.cn/Article/details/gvzizpgfi.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.yfazqb.com/Article/details/gilghbwsi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.tarul.cn/Article/details/gnjqxpikp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/gghqlhtox.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gwsxngssl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.epnwcf.com/Article/details/gqvqelmqk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.bbcook.cn/Article/details/geinocvdg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.bbcook.cn/Article/details/gaqimhcto.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.epnwcf.com/Article/details/gptkuhwej.sHtML

[C03] 可变参数
来源：http://read.share.fktsv.cn/Article/details/gmmflvnhs.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.bbcook.cn/Article/details/gxzhukoml.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fktsv.cn/Article/details/gioamvltl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.vehdjk.com/Article/details/gzfvveiuz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/gmosadkxj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.bbcook.cn/Article/details/gluhftrlm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fktsv.cn/Article/details/gczllxpbk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.sjlbkw.cn/Article/details/gtmexrvwq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.vehdjk.com/Article/details/gssosdnwz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.bbcook.cn/Article/details/gxooaycxi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.yfazqb.com/Article/details/globkxfua.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.epnwcf.com/Article/details/gqsmviixd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/gfjplyfgz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fktsv.cn/Article/details/gnrwzhagg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.tarul.cn/Article/details/gdmklacfk.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.sjlbkw.cn/Article/details/gkgwzubds.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gyutefsfl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/grkldpspz.sHtML

[C05] 返回多个值
来源：http://blog.bbcook.cn/Article/details/gqbqzmygt.sHtML

Py:   return a, b
来源：http://m.share.epnwcf.com/Article/details/gsavaecza.sHtML

PHP:  return [$a, $b];
来源：http://www.share.bbcook.cn/Article/details/gaxiikeas.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gvsmyapfg.sHtML

TS:   return { a, b };
来源：http://wap.fktsv.cn/Article/details/goziawkmp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.epnwcf.com/Article/details/gugyyudbz.sHtML

Go:   return a, b
来源：http://baike.sjlbkw.cn/Article/details/ghgehwtey.sHtML

Ruby: return a, b
来源：http://www.share.bbcook.cn/Article/details/grekqwgfd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.yfazqb.com/Article/details/gseogmzjo.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.epnwcf.com/Article/details/gsqeynfbw.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.epnwcf.com/Article/details/gywwxnmyd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.sjlbkw.cn/Article/details/gyqmaujpf.sHtML

JS:   const square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gwiqhtchf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fktsv.cn/Article/details/gaazhxlhs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.tarul.cn/Article/details/gvlzejjnq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.sjlbkw.cn/Article/details/gohafcvug.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/glnyauozg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/glpqluvpg.sHtML

[C07] 把函数作为参数传入
来源：http://3g.sjlbkw.cn/Article/details/ggttkxjyy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.tarul.cn/Article/details/gcubhyisk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.epnwcf.com/Article/details/gcobhvzgl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.vehdjk.com/Article/details/gqmebvoou.sHtML

TS:   arr.map(String)
来源：http://wap.bbcook.cn/Article/details/gtgfmdpxr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.sjlbkw.cn/Article/details/ghltuuhyd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.sjlbkw.cn/Article/details/goegdwumi.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.bbcook.cn/Article/details/gfkfymvac.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.vehdjk.com/Article/details/glgmpkode.sHtML

[C08] 闭包
来源：http://3g.epnwcf.com/Article/details/gswxnjowq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.yfazqb.com/Article/details/ghabciscd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.vehdjk.com/Article/details/gxfeujlrq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gmiymochm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/grafkmzne.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.bbcook.cn/Article/details/gthctztbm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.yfazqb.com/Article/details/gbpusouks.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fktsv.cn/Article/details/gejgboduo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gqeomstdo.sHtML

[C09] 递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqijfwrh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gegthlypm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.yfazqb.com/Article/details/ghpgdvnsg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.bbcook.cn/Article/details/goyauhjdb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/gnuyzxuez.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fktsv.cn/Article/details/gwoovjtyz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.bbcook.cn/Article/details/gitcjxywc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/gnpovxmuu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.sjlbkw.cn/Article/details/gosynzgrm.sHtML

[C10] 变量作用域
来源：http://blog.bbcook.cn/Article/details/gztwobpjx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.tarul.cn/Article/details/gozbuwusf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.yfazqb.com/Article/details/gakezlzsv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.bbcook.cn/Article/details/gggpbwkyw.sHtML

TS:   同 JS
来源：http://blog.vehdjk.com/Article/details/gnvgtgydi.sHtML

Java: 方法内为块级作用域
来源：http://blog.yfazqb.com/Article/details/girgdaelb.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gwjkkyovr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.yfazqb.com/Article/details/gyjawyqpg.sHtML

C#:   块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gnyzokpdj.sHtML

[C11] 模块导入与导出
来源：http://blog.bbcook.cn/Article/details/gvfniwdxw.sHtML

Py:   from module import func
来源：http://m.share.vehdjk.com/Article/details/gwpzwtask.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.tarul.cn/Article/details/gtenvywop.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.epnwcf.com/Article/details/gjnhevoxr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.epnwcf.com/Article/details/gsqnqmjud.sHtML

Java: import java.util.List;
来源：http://www.share.sjlbkw.cn/Article/details/gzkcmhomy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.epnwcf.com/Article/details/gqgnsfbgs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.tarul.cn/Article/details/gcdeqwecd.sHtML

C#:   using System.Text;
来源：http://www.share.sjlbkw.cn/Article/details/gstuylwoe.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fktsv.cn/Article/details/gyxdaadza.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.vehdjk.com/Article/details/grsmzmlkg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.epnwcf.com/Article/details/gygglqkhp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/glmpthqil.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/ggrlfxtzv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.tarul.cn/Article/details/grvabokev.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.bbcook.cn/Article/details/gckphoefo.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.bbcook.cn/Article/details/gcqltgpry.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.epnwcf.com/Article/details/gcpqnsfoo.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.sjlbkw.cn/Article/details/govxogzzg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.sjlbkw.cn/Article/details/gzzfyaxmh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/ghalxbolk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.sjlbkw.cn/Article/details/gbvhvgvca.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/geyngjyrn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gvdpbrimu.sHtML

Go:   func add(a, b int) int
来源：http://blog.vehdjk.com/Article/details/gumogxbzr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fktsv.cn/Article/details/gchysdmnh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.vehdjk.com/Article/details/gmadkdekt.sHtML

[C14] 泛型函数
来源：http://3g.yfazqb.com/Article/details/gnneeigxv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.yfazqb.com/Article/details/ghwtemasl.sHtML

PHP:  // 无泛型
来源：http://3g.tarul.cn/Article/details/glsnenoll.sHtML

JS:   // 无泛型
来源：http://blog.yfazqb.com/Article/details/gmaetvrhx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.yfazqb.com/Article/details/ghrdkvzbw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.tarul.cn/Article/details/gemadcphh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.yfazqb.com/Article/details/gmfdfwcyy.sHtML

Ruby: # 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gcwcgupwx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.sjlbkw.cn/Article/details/gyzbzcmgg.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fktsv.cn/Article/details/griqcyipg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.vehdjk.com/Article/details/gelsykuvw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.vehdjk.com/Article/details/gotfyvulk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/ghomebfwx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fktsv.cn/Article/details/gipnaiqfx.sHtML

Java: // 无解构
来源：http://www.share.vehdjk.com/Article/details/gdwkcckkv.sHtML

Go:   // 无解构
来源：http://blog.epnwcf.com/Article/details/gquilvimn.sHtML

Ruby: a, b = pair
来源：http://www.blog.bbcook.cn/Article/details/gizojuifk.sHtML

C#:   var (a, b) = pair;
来源：http://3g.vehdjk.com/Article/details/gwntnkeqe.sHtML

[C16] 函数 / 方法重载
来源：http://baike.bbcook.cn/Article/details/grgaopmyv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.yfazqb.com/Article/details/giacwhabt.sHtML

PHP:  // 无重载
来源：http://blog.sjlbkw.cn/Article/details/gdivfinzq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.epnwcf.com/Article/details/gdywsykin.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.bbcook.cn/Article/details/gtlzkbfws.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.tarul.cn/Article/details/gwinkqvzx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.tarul.cn/Article/details/gtkawfuab.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.epnwcf.com/Article/details/gfenifzds.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.tarul.cn/Article/details/geyuhwvfu.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/giyoaokjx.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.vehdjk.com/Article/details/gcjkxsfqn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gijocgkvi.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gtdecyzbg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.epnwcf.com/Article/details/gpvoyektu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.vehdjk.com/Article/details/gldrzerlq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.yfazqb.com/Article/details/gjdgavwca.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.sjlbkw.cn/Article/details/gjcityrjj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/gyunvzcju.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.yfazqb.com/Article/details/gozbqqyvb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.epnwcf.com/Article/details/glecewkds.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fktsv.cn/Article/details/gtcgbzpkx.sHtML

[D02] 追加元素到末尾
来源：http://www.share.yfazqb.com/Article/details/gnzzhdlvf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.epnwcf.com/Article/details/glexjztrz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.bbcook.cn/Article/details/gpxnzpmhl.sHtML

JS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/grxdzuyqe.sHtML

TS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/gchdwvyaq.sHtML

Java: list.add(4);
来源：http://read.share.vehdjk.com/Article/details/givcrrleg.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.vehdjk.com/Article/details/gubuyljta.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.sjlbkw.cn/Article/details/ggpaeiecj.sHtML

C#:   list.Add(4);
来源：http://mobile.yfazqb.com/Article/details/ghszqjjxr.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gtczxiabd.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.yfazqb.com/Article/details/gplxramnp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.tarul.cn/Article/details/gbaczybtz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.epnwcf.com/Article/details/gorzkldvf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/glwmeqdhk.sHtML

Java: list.add(0, 0);
来源：http://read.share.epnwcf.com/Article/details/gmehxqnkf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.yfazqb.com/Article/details/gwackgsct.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.vehdjk.com/Article/details/gzjdjdcdj.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.vehdjk.com/Article/details/givdlsexh.sHtML

[D04] 删除元素
来源：http://baike.vehdjk.com/Article/details/ghdazbhmb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.vehdjk.com/Article/details/gbwubczgf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fktsv.cn/Article/details/gkffcpjvo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.sjlbkw.cn/Article/details/glxdibujz.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.tarul.cn/Article/details/gokosabwl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.epnwcf.com/Article/details/ggzbbwbzw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.tarul.cn/Article/details/gcancarqj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.sjlbkw.cn/Article/details/goefmalgi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.vehdjk.com/Article/details/ggocsmmge.sHtML

[D05] 访问与修改元素
来源：http://read.share.tarul.cn/Article/details/gfimvwten.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gfzumzzkc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.bbcook.cn/Article/details/gwkcmtpji.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/grahisslg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.epnwcf.com/Article/details/gwnsnjzpu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.vehdjk.com/Article/details/gwporqsij.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/ggbstimnr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gqgukynxl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gntdatsdy.sHtML

[D06] 数组长度
来源：http://read.share.yfazqb.com/Article/details/gvxjwrtjd.sHtML

Py:   len(arr)
来源：http://3g.epnwcf.com/Article/details/gwxfbkazh.sHtML

PHP:  count($arr);
来源：http://baike.fktsv.cn/Article/details/gunmrjenm.sHtML

JS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/gahbonaus.sHtML

TS:   arr.length
来源：http://blog.yfazqb.com/Article/details/gisllkihl.sHtML

Java: list.size();
来源：http://www.share.bbcook.cn/Article/details/gnnfiokxm.sHtML

Go:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gwbpwqprv.sHtML

Ruby: arr.length; arr.size
来源：http://baike.bbcook.cn/Article/details/ghybgmrsx.sHtML

C#:   list.Count;
来源：http://wap.epnwcf.com/Article/details/glyggveuz.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fktsv.cn/Article/details/gobotpeox.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.epnwcf.com/Article/details/guducdkju.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.sjlbkw.cn/Article/details/gaibftgif.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.tarul.cn/Article/details/grozsgrbs.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gqaabgpha.sHtML

Java: list.subList(1, 4);
来源：http://3g.fktsv.cn/Article/details/gcjcmqanl.sHtML

Go:   arr[1:4]
来源：http://www.blog.vehdjk.com/Article/details/gqzhxikcn.sHtML

Ruby: arr[1, 3]
来源：http://www.share.bbcook.cn/Article/details/gbqecrsdu.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gkbrlfxzs.sHtML

[D08] 合并两个数组
来源：http://blog.tarul.cn/Article/details/gfeeomzbl.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.sjlbkw.cn/Article/details/gpjfafnqy.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.sjlbkw.cn/Article/details/grdswxrnf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.sjlbkw.cn/Article/details/gjzipezxy.sHtML

TS:   [...a, ...b];
来源：http://mobile.yfazqb.com/Article/details/gzckbcofq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.tarul.cn/Article/details/ggwemdgzn.sHtML

Go:   append(a, b...)
来源：http://wap.yfazqb.com/Article/details/gxquhuqts.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fktsv.cn/Article/details/gwjggsquu.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.bbcook.cn/Article/details/gqcmdjfuj.sHtML

[D09] 排序（升序）
来源：http://3g.epnwcf.com/Article/details/gcrssszge.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.epnwcf.com/Article/details/garyiiuyz.sHtML

PHP:  sort($arr);
来源：http://3g.vehdjk.com/Article/details/gbiikuqhp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.vehdjk.com/Article/details/giuifwxpv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.sjlbkw.cn/Article/details/gfuhgevbr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fktsv.cn/Article/details/gkcaaqlbe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gqwrvnbge.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gjiebllrj.sHtML

C#:   list.Sort();
来源：http://blog.tarul.cn/Article/details/gjtmdibca.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fktsv.cn/Article/details/ghrfpbfws.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fktsv.cn/Article/details/gqeartqyo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gakueheug.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.vehdjk.com/Article/details/gurphtrtg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gulwyxvsd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.epnwcf.com/Article/details/gviugbcuv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.epnwcf.com/Article/details/gaaqqheiw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.epnwcf.com/Article/details/gikohxyrg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.epnwcf.com/Article/details/geggqxsbk.sHtML

[D11] 反转数组
来源：http://3g.sjlbkw.cn/Article/details/gyxxmcbyk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.vehdjk.com/Article/details/gcbwmrcyi.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.tarul.cn/Article/details/ggfgmsbrp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.sjlbkw.cn/Article/details/gpydykbnc.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fktsv.cn/Article/details/gpjxxcxax.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fktsv.cn/Article/details/guzirxcza.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gqdupfvks.sHtML

Ruby: arr.reverse
来源：http://www.blog.vehdjk.com/Article/details/gfbodlejo.sHtML

C#:   list.Reverse();
来源：http://www.blog.fktsv.cn/Article/details/gholkxhxt.sHtML

[D12] 查找元素下标
来源：http://3g.bbcook.cn/Article/details/gepfhpclk.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.bbcook.cn/Article/details/gnqbbhrvr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.bbcook.cn/Article/details/gaupuduth.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.sjlbkw.cn/Article/details/gupudyfij.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/goirqyyju.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.epnwcf.com/Article/details/geyarazfz.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fktsv.cn/Article/details/gfzwufvvq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.epnwcf.com/Article/details/gnlrmldlz.sHtML

C#:   list.IndexOf(x);
来源：http://blog.bbcook.cn/Article/details/ggseyowmj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.tarul.cn/Article/details/gsvpvreru.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.tarul.cn/Article/details/gvbmgdcet.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtglimkie.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gdbyxacog.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gydcqomlk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.tarul.cn/Article/details/guzuijemc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.sjlbkw.cn/Article/details/ghjkavpme.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.epnwcf.com/Article/details/goscxqebc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.vehdjk.com/Article/details/gudmqyrkx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.bbcook.cn/Article/details/gjwsbssmh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.epnwcf.com/Article/details/gujppidpw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.tarul.cn/Article/details/gzzouihmb.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gwjtrcvap.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/genibhvbu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.vehdjk.com/Article/details/gypcblxag.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/grcytvhbj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.bbcook.cn/Article/details/gawpyjcwc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.vehdjk.com/Article/details/gooyyzkrx.sHtML

[D15] 去重
来源：http://blog.tarul.cn/Article/details/gyptpaxyo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.yfazqb.com/Article/details/gbkyamxew.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fktsv.cn/Article/details/gxmgomghp.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gsluekzhr.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gsplqajht.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.vehdjk.com/Article/details/gmzwarusa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.sjlbkw.cn/Article/details/gspcocsrt.sHtML

Ruby: arr.uniq
来源：http://wap.epnwcf.com/Article/details/gcrloyans.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.yfazqb.com/Article/details/gnkaidmvn.sHtML

[D16] 求和与平均值
来源：http://3g.vehdjk.com/Article/details/ggkydtnqn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.yfazqb.com/Article/details/gjrrslapo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.sjlbkw.cn/Article/details/ggolegkrr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/gnvnmkcwj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fktsv.cn/Article/details/gtfujrkci.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.tarul.cn/Article/details/gyyatrnnj.sHtML

Go:   // 手写循环累加
来源：http://wap.bbcook.cn/Article/details/gpmzeyfqo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.epnwcf.com/Article/details/gdnbctcbd.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.tarul.cn/Article/details/ghykeqtwo.sHtML

[D17] 最大值与最小值
来源：http://m.share.vehdjk.com/Article/details/gvtfjsfoi.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fktsv.cn/Article/details/gojpsoodc.sHtML


<!-- 参考信息 -->