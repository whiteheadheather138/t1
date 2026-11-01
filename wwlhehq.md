代发 wailian999

[B13] 判断是否为数字
来源：http://www.m.share.yfazqb.com/Article/details/gsllbhyug.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.epnwcf.com/Article/details/gbxrsdvtt.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fktsv.cn/Article/details/gigfvrkpx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.yfazqb.com/Article/details/gwyqqwumc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gzpgaqifv.sHtML

Java: x instanceof Number
来源：http://www.share.epnwcf.com/Article/details/goitorurg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.tarul.cn/Article/details/gwpceutvv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.vehdjk.com/Article/details/gqqofgqvx.sHtML

C#:   x is int or double or decimal
来源：http://wap.bbcook.cn/Article/details/gvwzwbanx.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.vehdjk.com/Article/details/ghzociafq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.tarul.cn/Article/details/gggpmfdww.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.sjlbkw.cn/Article/details/gvhtwwcfl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gaejqezdn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fktsv.cn/Article/details/gdypltnjr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.tarul.cn/Article/details/gahmghkqy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.tarul.cn/Article/details/gdubgejxc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/gzvhtthyw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gdshyynvd.sHtML

[B15] 布尔运算与取反
来源：http://m.share.sjlbkw.cn/Article/details/gfqwugrms.sHtML

Py:   a and b or not c
来源：http://blog.fktsv.cn/Article/details/gnzkbdpsp.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.bbcook.cn/Article/details/ggpfgawsd.sHtML

JS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gzpfjuseq.sHtML

TS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gdtjsrjfd.sHtML

Java: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gmvxqslwd.sHtML

Go:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gplfxunqx.sHtML

Ruby: a && b || !c
来源：http://baike.epnwcf.com/Article/details/ghkxijvpe.sHtML

C#:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gqyigczfy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.bbcook.cn/Article/details/gtzcaobmf.sHtML

Py:   if not data: return
来源：http://mobile.vehdjk.com/Article/details/gqliwvjyt.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.vehdjk.com/Article/details/gkturrzzl.sHtML

JS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gcadvmnmn.sHtML

TS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gnjtlpvim.sHtML

Java: if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/gmvmgamhh.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.vehdjk.com/Article/details/gixqbtprj.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvgqjuoy.sHtML

C#:   if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/gzbebpftk.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxcpihhsd.sHtML

C. 函数与作用域
来源：http://www.share.epnwcf.com/Article/details/gzouilgsq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grqqufgez.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gaunxiegj.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.vehdjk.com/Article/details/gxiqdjzen.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gxtxlopnq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gdxkkmgfn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gcjyneuio.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gtgsztail.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fktsv.cn/Article/details/guikpqujl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.epnwcf.com/Article/details/ggqijgewn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gqyhyiueb.sHtML

[C02] 默认参数
来源：http://3g.tarul.cn/Article/details/gvosoaspf.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fktsv.cn/Article/details/gdtvedfsg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.epnwcf.com/Article/details/gujdqvbyx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gicmmkejj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/ghkxpqdjw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.sjlbkw.cn/Article/details/gwkhlfirx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.sjlbkw.cn/Article/details/gaktykkec.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.tarul.cn/Article/details/gmgnsooqm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.bbcook.cn/Article/details/glfrcghqc.sHtML

[C03] 可变参数
来源：http://wap.tarul.cn/Article/details/gagtynbnk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/grfwxyhvp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.tarul.cn/Article/details/grsqhpkbn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.tarul.cn/Article/details/gshzhlsop.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.tarul.cn/Article/details/gennmjsda.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.epnwcf.com/Article/details/gpgxuxtzd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.vehdjk.com/Article/details/gnicvxaqf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fktsv.cn/Article/details/gwqnlopqe.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.vehdjk.com/Article/details/gpgeaaoqr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.epnwcf.com/Article/details/gnbmthvyw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.sjlbkw.cn/Article/details/gfbqwkrby.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.bbcook.cn/Article/details/guxotlxkp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/gyatxaoag.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.vehdjk.com/Article/details/gngwnbvqh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.tarul.cn/Article/details/gwdvokkjm.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fktsv.cn/Article/details/gqcaepxxg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/ghknorrgo.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gfvbvvhsy.sHtML

[C05] 返回多个值
来源：http://read.share.sjlbkw.cn/Article/details/gyqasksgz.sHtML

Py:   return a, b
来源：http://3g.epnwcf.com/Article/details/gspogkqqv.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.sjlbkw.cn/Article/details/grenahpwj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/gwwqiwppf.sHtML

TS:   return { a, b };
来源：http://3g.tarul.cn/Article/details/gykazabpg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.vehdjk.com/Article/details/gqxjfznbe.sHtML

Go:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gynxtnkvw.sHtML

Ruby: return a, b
来源：http://m.share.yfazqb.com/Article/details/ghbzgdqay.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.tarul.cn/Article/details/gvumohzcg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.yfazqb.com/Article/details/gfkmnpkbj.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.epnwcf.com/Article/details/gqevlcnrz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.epnwcf.com/Article/details/gqivjpdkp.sHtML

JS:   const square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/grqbmjfbs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gxoustpxk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fktsv.cn/Article/details/guuasaibd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gtyhkqfke.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.tarul.cn/Article/details/glhphplqs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gfvxodnbp.sHtML

[C07] 把函数作为参数传入
来源：http://baike.vehdjk.com/Article/details/ghctxvigj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.yfazqb.com/Article/details/gejzyccjb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.vehdjk.com/Article/details/ghiykftki.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.bbcook.cn/Article/details/gjbldpwiw.sHtML

TS:   arr.map(String)
来源：http://m.share.epnwcf.com/Article/details/gppygdqfv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gfrejenxe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fktsv.cn/Article/details/gwekutpko.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.vehdjk.com/Article/details/gyfzqbipl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.epnwcf.com/Article/details/gdlkjabvg.sHtML

[C08] 闭包
来源：http://www.m.share.yfazqb.com/Article/details/gkmeqocti.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.yfazqb.com/Article/details/ghqoxcngo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fktsv.cn/Article/details/gulkzzrhb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gqdubqnme.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gyeiavcds.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.yfazqb.com/Article/details/giwxakiuj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.yfazqb.com/Article/details/gxitstglg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fktsv.cn/Article/details/gsipzojya.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.bbcook.cn/Article/details/gkpzvtktb.sHtML

[C09] 递归
来源：http://mobile.bbcook.cn/Article/details/gurqywosp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gisgrajmp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.vehdjk.com/Article/details/gjchsztkk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gtyphstjo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fktsv.cn/Article/details/gbhfqdfgf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/glnappnmm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fktsv.cn/Article/details/gdwfclqri.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.tarul.cn/Article/details/gvfxlmngz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.sjlbkw.cn/Article/details/gxlyxajzc.sHtML

[C10] 变量作用域
来源：http://www.blog.tarul.cn/Article/details/gxccuujlb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.yfazqb.com/Article/details/gozaaiztp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/gwroyxrtb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.tarul.cn/Article/details/gckmnhdmd.sHtML

TS:   同 JS
来源：http://www.share.bbcook.cn/Article/details/gtnadulrd.sHtML

Java: 方法内为块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gntaavznv.sHtML

Go:   花括号块级作用域
来源：http://m.share.epnwcf.com/Article/details/ghsmabrhs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.tarul.cn/Article/details/ggbkgixqx.sHtML

C#:   块级作用域
来源：http://blog.epnwcf.com/Article/details/geinlvvng.sHtML

[C11] 模块导入与导出
来源：http://www.share.bbcook.cn/Article/details/gsuuqbcpy.sHtML

Py:   from module import func
来源：http://3g.tarul.cn/Article/details/goczfkpix.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.tarul.cn/Article/details/gjydbxvys.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/gelihjoya.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.epnwcf.com/Article/details/gibivaxjc.sHtML

Java: import java.util.List;
来源：http://read.share.tarul.cn/Article/details/gixzbmhyg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.tarul.cn/Article/details/gxozywlfw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.bbcook.cn/Article/details/gewkyhzzg.sHtML

C#:   using System.Text;
来源：http://m.share.tarul.cn/Article/details/gbeqsgvfw.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.vehdjk.com/Article/details/gwibpmepx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.yfazqb.com/Article/details/gfdtzfupo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.epnwcf.com/Article/details/gqiseiksb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fktsv.cn/Article/details/gqiwmpiha.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.bbcook.cn/Article/details/gwusgtiye.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.vehdjk.com/Article/details/golmxhpgr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/gwhlimzye.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.yfazqb.com/Article/details/gyaokoikk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fktsv.cn/Article/details/gjllywity.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.tarul.cn/Article/details/gurfdepjv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fktsv.cn/Article/details/gdyxhrndk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/guuoneitu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.yfazqb.com/Article/details/gpiymowrx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/giullirwo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gafbmcylh.sHtML

Go:   func add(a, b int) int
来源：http://m.share.epnwcf.com/Article/details/gwihkdown.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.tarul.cn/Article/details/gtlvternb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fktsv.cn/Article/details/ggsghwnoi.sHtML

[C14] 泛型函数
来源：http://m.share.bbcook.cn/Article/details/gkpdkyhij.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.sjlbkw.cn/Article/details/gwmqravfm.sHtML

PHP:  // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gfhrmtvjb.sHtML

JS:   // 无泛型
来源：http://3g.epnwcf.com/Article/details/gssdueiuo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fktsv.cn/Article/details/gxaxalvwa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.sjlbkw.cn/Article/details/grmourswl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.epnwcf.com/Article/details/gydplnekm.sHtML

Ruby: # 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gsjvimglz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.sjlbkw.cn/Article/details/gjdhinfus.sHtML

[C15] 解构 / 展开参数
来源：http://3g.vehdjk.com/Article/details/gsyiwsace.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.vehdjk.com/Article/details/gupwdimfl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.bbcook.cn/Article/details/gvkpgbedh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/ghhkeasju.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdnugxbi.sHtML

Java: // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gkkjtjpad.sHtML

Go:   // 无解构
来源：http://blog.sjlbkw.cn/Article/details/gqbzvrlam.sHtML

Ruby: a, b = pair
来源：http://mobile.sjlbkw.cn/Article/details/gjopodyaj.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.tarul.cn/Article/details/gzuluvicy.sHtML

[C16] 函数 / 方法重载
来源：http://3g.yfazqb.com/Article/details/gadapvbei.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gxhydqavx.sHtML

PHP:  // 无重载
来源：http://baike.tarul.cn/Article/details/gvtsrviue.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.sjlbkw.cn/Article/details/ghiukdgzv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.tarul.cn/Article/details/gpmrluyul.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fktsv.cn/Article/details/gvrcrrtdr.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.epnwcf.com/Article/details/gdyulreht.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fktsv.cn/Article/details/gjeiamtpt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.bbcook.cn/Article/details/ggbosswtv.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gohycosiw.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.sjlbkw.cn/Article/details/gzwhmraon.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmfmtdvij.sHtML

[D01] 创建数组 / 列表
来源：http://3g.sjlbkw.cn/Article/details/gqtkyakmz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.sjlbkw.cn/Article/details/grzgsjsjp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fktsv.cn/Article/details/gvieldemn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.vehdjk.com/Article/details/gbvevhwva.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.vehdjk.com/Article/details/gtxwhofbg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fktsv.cn/Article/details/gnmselapv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.tarul.cn/Article/details/gwptmncpd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.sjlbkw.cn/Article/details/gusgakbxq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.bbcook.cn/Article/details/gzeajotbs.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fktsv.cn/Article/details/gqqehctbn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.tarul.cn/Article/details/gvzoopgda.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.bbcook.cn/Article/details/gydiynber.sHtML

JS:   arr.push(4);
来源：http://wap.vehdjk.com/Article/details/gfkxyjnsq.sHtML

TS:   arr.push(4);
来源：http://wap.sjlbkw.cn/Article/details/gxufgxesz.sHtML

Java: list.add(4);
来源：http://m.share.tarul.cn/Article/details/giocpnbuh.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.epnwcf.com/Article/details/grhmfwihc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.vehdjk.com/Article/details/gkoebbdie.sHtML

C#:   list.Add(4);
来源：http://wap.fktsv.cn/Article/details/geuffmphl.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fktsv.cn/Article/details/gxqoddutv.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.vehdjk.com/Article/details/gzeihglab.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.yfazqb.com/Article/details/gqknulqon.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.bbcook.cn/Article/details/gpjlvpbxd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.tarul.cn/Article/details/giqquopum.sHtML

Java: list.add(0, 0);
来源：http://3g.epnwcf.com/Article/details/gbqtnvksa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.epnwcf.com/Article/details/gctqzzeur.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.tarul.cn/Article/details/gnhnsxyze.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.yfazqb.com/Article/details/gilrvvcjh.sHtML

[D04] 删除元素
来源：http://baike.fktsv.cn/Article/details/ghitdyfen.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fktsv.cn/Article/details/gdndlkbdz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gngmiyuwp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.epnwcf.com/Article/details/gzslrvmvf.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.sjlbkw.cn/Article/details/gzzuguobc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.vehdjk.com/Article/details/gcpscsyeg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.epnwcf.com/Article/details/gqgefjorg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.tarul.cn/Article/details/giovjqqmn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.yfazqb.com/Article/details/gvkjspotk.sHtML

[D05] 访问与修改元素
来源：http://m.share.sjlbkw.cn/Article/details/gxvrbpxqw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gzcingelc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gngtgtnal.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gcbuiqtjn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.vehdjk.com/Article/details/gwkmcbcoe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.vehdjk.com/Article/details/gcefiobnp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gegygvcpb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/ghewaeyju.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gpoycscxt.sHtML

[D06] 数组长度
来源：http://mobile.epnwcf.com/Article/details/gvukbctvn.sHtML

Py:   len(arr)
来源：http://3g.vehdjk.com/Article/details/gaxlzfyhd.sHtML

PHP:  count($arr);
来源：http://www.blog.fktsv.cn/Article/details/gczgpqrti.sHtML

JS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/gnnxwiprt.sHtML

TS:   arr.length
来源：http://read.share.tarul.cn/Article/details/gzuuhfsxk.sHtML

Java: list.size();
来源：http://wap.yfazqb.com/Article/details/gzlmagjxs.sHtML

Go:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/gdjcybzsf.sHtML

Ruby: arr.length; arr.size
来源：http://blog.tarul.cn/Article/details/guacsudcc.sHtML

C#:   list.Count;
来源：http://www.blog.yfazqb.com/Article/details/gfibbfonj.sHtML

[D07] 切片 / 取子数组
来源：http://3g.vehdjk.com/Article/details/gunuwobwe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.vehdjk.com/Article/details/gmwjrtmkr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.tarul.cn/Article/details/gelvgcodt.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gscdrwcde.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gwvkzlqbo.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fktsv.cn/Article/details/giiprsfnq.sHtML

Go:   arr[1:4]
来源：http://www.share.vehdjk.com/Article/details/gnvdcnxaa.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.tarul.cn/Article/details/grfeasfne.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/glvvfpwrt.sHtML

[D08] 合并两个数组
来源：http://www.share.fktsv.cn/Article/details/ghyhbtfjw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.yfazqb.com/Article/details/gwlmyrsua.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.tarul.cn/Article/details/gfefdwdyh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.sjlbkw.cn/Article/details/gzbkqhbzj.sHtML

TS:   [...a, ...b];
来源：http://www.share.epnwcf.com/Article/details/gpsqjcgmy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gayzzgesn.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fktsv.cn/Article/details/gbdzxnlng.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.epnwcf.com/Article/details/gfzycfthv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gpsfgxgdf.sHtML

[D09] 排序（升序）
来源：http://mobile.fktsv.cn/Article/details/gmnavsqvq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gipklkglx.sHtML

PHP:  sort($arr);
来源：http://baike.yfazqb.com/Article/details/ggbpciisz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.sjlbkw.cn/Article/details/gkiuqjmmq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.vehdjk.com/Article/details/glwptodbg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.yfazqb.com/Article/details/gbnivnpnd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gexlpmlcx.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/gfndbrrch.sHtML

C#:   list.Sort();
来源：http://www.m.share.vehdjk.com/Article/details/gocuospis.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.sjlbkw.cn/Article/details/ghzjkqrlg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.tarul.cn/Article/details/gzjjceifk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.bbcook.cn/Article/details/gmefhbdbx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/guxpwxowf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.vehdjk.com/Article/details/gfuapfgnb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.tarul.cn/Article/details/ghwdzlxwk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.yfazqb.com/Article/details/grshhutqy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.bbcook.cn/Article/details/goinpnomp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fktsv.cn/Article/details/gboexibbh.sHtML

[D11] 反转数组
来源：http://mobile.sjlbkw.cn/Article/details/gvlpwbhwd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.sjlbkw.cn/Article/details/gfuawubpc.sHtML

PHP:  array_reverse($arr);
来源：http://wap.vehdjk.com/Article/details/gsgsoferl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.tarul.cn/Article/details/gybspeekc.sHtML

TS:   [...arr].reverse();
来源：http://3g.sjlbkw.cn/Article/details/gmdwljyob.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fktsv.cn/Article/details/grunnhpcv.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.bbcook.cn/Article/details/glbwlrkkd.sHtML

Ruby: arr.reverse
来源：http://blog.fktsv.cn/Article/details/gmjmcypna.sHtML

C#:   list.Reverse();
来源：http://mobile.vehdjk.com/Article/details/ggtlxvlzw.sHtML

[D12] 查找元素下标
来源：http://3g.tarul.cn/Article/details/gotlipvia.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.epnwcf.com/Article/details/ghsjvjwcl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gdonuzfzd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gxiciutdg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.yfazqb.com/Article/details/gzczsprss.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.yfazqb.com/Article/details/gnwcigbva.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fktsv.cn/Article/details/gdmtcuiui.sHtML

Ruby: arr.index(x)
来源：http://mobile.tarul.cn/Article/details/gqhjeupoo.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.bbcook.cn/Article/details/gkjltzpeg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.sjlbkw.cn/Article/details/ggytbnxdk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.bbcook.cn/Article/details/gikjnkaut.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.yfazqb.com/Article/details/gfddvvmaj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/glvcvduic.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/ggbjeicuj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.yfazqb.com/Article/details/gerddsliu.sHtML


<!-- 参考信息 -->