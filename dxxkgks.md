代发 wailian999

C#:   x is int or double or decimal
来源：http://www.share.epnwcf.com/Article/details/gkscjydkd.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.bbcook.cn/Article/details/gsnevljri.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.yfazqb.com/Article/details/glwnyjvur.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.bbcook.cn/Article/details/ghwohnxfy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gsginpvbs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gayrmmlfk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gpycdxups.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.vehdjk.com/Article/details/gdwisator.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.epnwcf.com/Article/details/gmqbddifa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gqfcwwrvu.sHtML

[B15] 布尔运算与取反
来源：http://blog.yfazqb.com/Article/details/ghjhuhizo.sHtML

Py:   a and b or not c
来源：http://3g.yfazqb.com/Article/details/gorwmfnva.sHtML

PHP:  $a && $b || !$c
来源：http://blog.bbcook.cn/Article/details/growozoez.sHtML

JS:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gdalfwkyj.sHtML

TS:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gepelemmm.sHtML

Java: a && b || !c
来源：http://mobile.tarul.cn/Article/details/gwzywzbjq.sHtML

Go:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gizotvati.sHtML

Ruby: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gzujrpavk.sHtML

C#:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gffygdfbw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fktsv.cn/Article/details/gcekvexfu.sHtML

Py:   if not data: return
来源：http://blog.vehdjk.com/Article/details/gjzykfpla.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.bbcook.cn/Article/details/gdmqsofur.sHtML

JS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/gspcxzhcx.sHtML

TS:   if (!data) return;
来源：http://m.share.fktsv.cn/Article/details/gfsemvihe.sHtML

Java: if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/gixjxzlly.sHtML

Go:   if data == nil { return }
来源：http://blog.fktsv.cn/Article/details/gyxebqhpz.sHtML

Ruby: return if data.nil?
来源：http://blog.epnwcf.com/Article/details/gycroybpm.sHtML

C#:   if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gougwtken.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbebijjpr.sHtML

C. 函数与作用域
来源：http://www.blog.fktsv.cn/Article/details/gtgqdlyrp.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfopjrivi.sHtML

[C01] 定义函数
来源：http://3g.tarul.cn/Article/details/gkqmosixb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.epnwcf.com/Article/details/gufwwrgyb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gtutiewdf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gdooebtkd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gydrkldrn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/ggdlqyljf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.tarul.cn/Article/details/gbzfcjwcg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.sjlbkw.cn/Article/details/gesycfifv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gfoplyiya.sHtML

[C02] 默认参数
来源：http://read.share.epnwcf.com/Article/details/goweixaku.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.epnwcf.com/Article/details/gkdpiysku.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.bbcook.cn/Article/details/gcuddgglf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gptwgviry.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gnstomkwu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.vehdjk.com/Article/details/grfkaptgj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.epnwcf.com/Article/details/gzswuwveu.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fktsv.cn/Article/details/gyjafovrd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/gtawqzozz.sHtML

[C03] 可变参数
来源：http://www.blog.sjlbkw.cn/Article/details/gydazvkoe.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.bbcook.cn/Article/details/gljamulfo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.sjlbkw.cn/Article/details/ggidwgwsw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/gbfkjfzus.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/guchytokp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fktsv.cn/Article/details/gqfduyndl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.yfazqb.com/Article/details/ggcrrkcpp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.bbcook.cn/Article/details/gxopezuvp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.yfazqb.com/Article/details/gdmuntbfc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.bbcook.cn/Article/details/gcdcckjdh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.vehdjk.com/Article/details/gxuewlvxx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.tarul.cn/Article/details/gxzbkfzwx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/glgojtzgb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.epnwcf.com/Article/details/gzcbdiacz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.tarul.cn/Article/details/gkulzhcaq.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.tarul.cn/Article/details/gpdhiritu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/ggmkimayf.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gkgxmmjri.sHtML

[C05] 返回多个值
来源：http://www.blog.yfazqb.com/Article/details/gpvfcanud.sHtML

Py:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/godaadnfn.sHtML

PHP:  return [$a, $b];
来源：http://blog.tarul.cn/Article/details/gkvrburrq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.vehdjk.com/Article/details/gyqercgeq.sHtML

TS:   return { a, b };
来源：http://wap.vehdjk.com/Article/details/gflkobryu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.bbcook.cn/Article/details/gcdbgiqow.sHtML

Go:   return a, b
来源：http://mobile.tarul.cn/Article/details/gfktmizmk.sHtML

Ruby: return a, b
来源：http://wap.epnwcf.com/Article/details/gyolunefk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.yfazqb.com/Article/details/gwbkvixbw.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.epnwcf.com/Article/details/gtziikyrk.sHtML

Py:   square = lambda x: x * x
来源：http://blog.yfazqb.com/Article/details/gcahdiill.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fktsv.cn/Article/details/gtbghaetn.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gusmhawqg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.bbcook.cn/Article/details/gdnxdnxei.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fktsv.cn/Article/details/gzjzxvfrs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.yfazqb.com/Article/details/guborhtea.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.epnwcf.com/Article/details/gzyduuubz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.bbcook.cn/Article/details/gjsijsegd.sHtML

[C07] 把函数作为参数传入
来源：http://blog.bbcook.cn/Article/details/gcmbcuwuk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.tarul.cn/Article/details/gpbdrukoi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.epnwcf.com/Article/details/gkveohlia.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.tarul.cn/Article/details/ggawqqkoo.sHtML

TS:   arr.map(String)
来源：http://www.share.fktsv.cn/Article/details/gueugfntg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.yfazqb.com/Article/details/grnmnbdvo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.sjlbkw.cn/Article/details/gxorjprmr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.tarul.cn/Article/details/gfwlbewja.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.sjlbkw.cn/Article/details/gvadfdrgy.sHtML

[C08] 闭包
来源：http://www.share.sjlbkw.cn/Article/details/griehnwjq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.tarul.cn/Article/details/gffcvilus.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.bbcook.cn/Article/details/gabkqlxft.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gjywrexkh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gibutgeqy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.yfazqb.com/Article/details/gyqxdrakw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.vehdjk.com/Article/details/gbzyjqkct.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.sjlbkw.cn/Article/details/gjpijewxv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gvpyzukfu.sHtML

[C09] 递归
来源：http://www.m.share.fktsv.cn/Article/details/gosxhljkh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/ggjtlqyfi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.sjlbkw.cn/Article/details/gamwczrkd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/grgvqyeoa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/gxsyotbxt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.vehdjk.com/Article/details/gwulyotcw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.vehdjk.com/Article/details/gqqdnvnzr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gnoizfrzx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fktsv.cn/Article/details/gbzvweklh.sHtML

[C10] 变量作用域
来源：http://www.share.sjlbkw.cn/Article/details/gumhyzmyc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.vehdjk.com/Article/details/ggkszolcc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.yfazqb.com/Article/details/gizgxmrbj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/gtnvocapi.sHtML

TS:   同 JS
来源：http://m.share.vehdjk.com/Article/details/gejbcqexc.sHtML

Java: 方法内为块级作用域
来源：http://3g.bbcook.cn/Article/details/gyaygzqvz.sHtML

Go:   花括号块级作用域
来源：http://blog.epnwcf.com/Article/details/ggmpzjphn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.yfazqb.com/Article/details/gvmkzkfoy.sHtML

C#:   块级作用域
来源：http://read.share.vehdjk.com/Article/details/gtxfjvvkz.sHtML

[C11] 模块导入与导出
来源：http://blog.fktsv.cn/Article/details/geytlfpik.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/gkniimuzc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzoievks.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.sjlbkw.cn/Article/details/gaiqdwmdo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.bbcook.cn/Article/details/gspyntquo.sHtML

Java: import java.util.List;
来源：http://mobile.vehdjk.com/Article/details/ggxbqdync.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.epnwcf.com/Article/details/gqlbrdkqz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fktsv.cn/Article/details/gfbqagvwb.sHtML

C#:   using System.Text;
来源：http://blog.bbcook.cn/Article/details/goiftoubc.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.tarul.cn/Article/details/gshzglqhm.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.tarul.cn/Article/details/gaqwsbhaq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.bbcook.cn/Article/details/geheimawo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/gzmsbqbfa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/gtzpalyci.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.vehdjk.com/Article/details/gixlivytc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.bbcook.cn/Article/details/gjbewgsye.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.sjlbkw.cn/Article/details/gceplmvgo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gzsjzaqlj.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.bbcook.cn/Article/details/gblrlldkq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.bbcook.cn/Article/details/gxivquyiv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gvpgpgajs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.bbcook.cn/Article/details/grozqjssh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/grwibtjiw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/grfrxjrvg.sHtML

Go:   func add(a, b int) int
来源：http://blog.yfazqb.com/Article/details/gwspmiwvv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.yfazqb.com/Article/details/gylaclsmf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.epnwcf.com/Article/details/gjqsjchsa.sHtML

[C14] 泛型函数
来源：http://mobile.epnwcf.com/Article/details/gudqfphyc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.yfazqb.com/Article/details/gauwpqdab.sHtML

PHP:  // 无泛型
来源：http://blog.epnwcf.com/Article/details/gtshjvldq.sHtML

JS:   // 无泛型
来源：http://read.share.epnwcf.com/Article/details/gcuuwmiab.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.epnwcf.com/Article/details/gugoiyjub.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.yfazqb.com/Article/details/ghggjpsmm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.tarul.cn/Article/details/gpicvkdom.sHtML

Ruby: # 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gqcpjqylh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.yfazqb.com/Article/details/gqcelfgrf.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gjucwvwgt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.yfazqb.com/Article/details/gdheagwan.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fktsv.cn/Article/details/gdmzqcrtr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.vehdjk.com/Article/details/goanlqlte.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.vehdjk.com/Article/details/genmnubrz.sHtML

Java: // 无解构
来源：http://www.m.share.tarul.cn/Article/details/grtzfjwnv.sHtML

Go:   // 无解构
来源：http://mobile.sjlbkw.cn/Article/details/gnacmdtst.sHtML

Ruby: a, b = pair
来源：http://read.share.tarul.cn/Article/details/gvakfcpop.sHtML

C#:   var (a, b) = pair;
来源：http://wap.bbcook.cn/Article/details/gzlgjkstb.sHtML

[C16] 函数 / 方法重载
来源：http://3g.sjlbkw.cn/Article/details/giqjwdaff.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fktsv.cn/Article/details/gnixbibmc.sHtML

PHP:  // 无重载
来源：http://wap.vehdjk.com/Article/details/gupetpofr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.sjlbkw.cn/Article/details/gacpmpuck.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.bbcook.cn/Article/details/gnfgqpglz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.epnwcf.com/Article/details/gxvdmqkuh.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fktsv.cn/Article/details/gboynjqkh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.yfazqb.com/Article/details/gfjmmloae.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.tarul.cn/Article/details/gjxpnkleb.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdsxnclsc.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.vehdjk.com/Article/details/gzfrqhhwe.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gsfjianph.sHtML

[D01] 创建数组 / 列表
来源：http://blog.sjlbkw.cn/Article/details/gwromuuyw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.yfazqb.com/Article/details/gtloqinwu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.tarul.cn/Article/details/gexrfgieq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.yfazqb.com/Article/details/gfnnfeprj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.vehdjk.com/Article/details/gabgcrgtq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.yfazqb.com/Article/details/gpkwjsyna.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.yfazqb.com/Article/details/gagbosiao.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.epnwcf.com/Article/details/gcqiygcrf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.bbcook.cn/Article/details/gpkooqrdb.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.vehdjk.com/Article/details/gdjenlmew.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fktsv.cn/Article/details/goorojwlv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fktsv.cn/Article/details/ggaefyanl.sHtML

JS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/gwiaykpmk.sHtML

TS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/giajpplhw.sHtML

Java: list.add(4);
来源：http://www.blog.bbcook.cn/Article/details/gshimebav.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fktsv.cn/Article/details/guprshtnd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.sjlbkw.cn/Article/details/gqmofugpu.sHtML

C#:   list.Add(4);
来源：http://wap.tarul.cn/Article/details/gajaguuzz.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.bbcook.cn/Article/details/gymoumrvy.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.epnwcf.com/Article/details/gfvmxyxkc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fktsv.cn/Article/details/gmstzcqfj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.epnwcf.com/Article/details/gyrdwkuvs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gjzjsoqpv.sHtML

Java: list.add(0, 0);
来源：http://m.share.tarul.cn/Article/details/gufmcnbrn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.tarul.cn/Article/details/gdanbdaod.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.epnwcf.com/Article/details/gvwlphnok.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gilyntqys.sHtML

[D04] 删除元素
来源：http://m.share.fktsv.cn/Article/details/gayznusif.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.tarul.cn/Article/details/gfnpjunwq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.epnwcf.com/Article/details/gmgdigeya.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.epnwcf.com/Article/details/gmzwyhriq.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.epnwcf.com/Article/details/gfupdrpoy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.sjlbkw.cn/Article/details/gtzqrqhtt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fktsv.cn/Article/details/gbxxrkfmm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.tarul.cn/Article/details/gbkahxrmm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.epnwcf.com/Article/details/ghrxmkitl.sHtML

[D05] 访问与修改元素
来源：http://www.blog.tarul.cn/Article/details/gilmzdqny.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gstxwccbi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/gryeeloih.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gjijjltek.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.sjlbkw.cn/Article/details/gqljofiwe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.bbcook.cn/Article/details/gmhvfhadw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gteerowap.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsplhyoo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fktsv.cn/Article/details/ghcxqrxxl.sHtML

[D06] 数组长度
来源：http://wap.sjlbkw.cn/Article/details/gmjbcphmx.sHtML

Py:   len(arr)
来源：http://mobile.vehdjk.com/Article/details/gsvauubmu.sHtML

PHP:  count($arr);
来源：http://read.share.bbcook.cn/Article/details/gupndkncf.sHtML

JS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/galoluoyy.sHtML

TS:   arr.length
来源：http://m.share.sjlbkw.cn/Article/details/gfwojjobi.sHtML

Java: list.size();
来源：http://m.share.epnwcf.com/Article/details/gzqwhbfut.sHtML

Go:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gziefbjjd.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.vehdjk.com/Article/details/gheasyozp.sHtML

C#:   list.Count;
来源：http://wap.sjlbkw.cn/Article/details/gidrlvgpz.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.tarul.cn/Article/details/gsxgevtyt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.sjlbkw.cn/Article/details/gotecuvig.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.bbcook.cn/Article/details/gzccqfbui.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gfogaoihl.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gnulohuvd.sHtML

Java: list.subList(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gfsyghotu.sHtML

Go:   arr[1:4]
来源：http://read.share.epnwcf.com/Article/details/gijheyriy.sHtML

Ruby: arr[1, 3]
来源：http://www.share.epnwcf.com/Article/details/gykmucelt.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fktsv.cn/Article/details/gyeczieph.sHtML

[D08] 合并两个数组
来源：http://blog.tarul.cn/Article/details/gtapextjc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.vehdjk.com/Article/details/gptssmner.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fktsv.cn/Article/details/gvlajyupu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.yfazqb.com/Article/details/gbtaywysw.sHtML

TS:   [...a, ...b];
来源：http://read.share.tarul.cn/Article/details/ghkybkfxx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fktsv.cn/Article/details/gjiffrrio.sHtML

Go:   append(a, b...)
来源：http://wap.yfazqb.com/Article/details/gjrrnqknc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.epnwcf.com/Article/details/gcymurlkk.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.bbcook.cn/Article/details/gqgisujhw.sHtML

[D09] 排序（升序）
来源：http://baike.vehdjk.com/Article/details/gzzhmlbwy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/glsnhmlfi.sHtML

PHP:  sort($arr);
来源：http://www.share.epnwcf.com/Article/details/gjvejwxfg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.tarul.cn/Article/details/gwkvjltcw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.tarul.cn/Article/details/gusnifmvd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.tarul.cn/Article/details/ggjpeaavy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gkifzkdwj.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gfkzzjmwu.sHtML

C#:   list.Sort();
来源：http://wap.sjlbkw.cn/Article/details/gyvusugdq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.yfazqb.com/Article/details/gsohfffmf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fktsv.cn/Article/details/gvfpfjamm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/gicqoteuq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.epnwcf.com/Article/details/ghasahjfn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/gnzbonvhy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.vehdjk.com/Article/details/gptieuupg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fktsv.cn/Article/details/gjgxkxtxm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.sjlbkw.cn/Article/details/gxwknphhf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.sjlbkw.cn/Article/details/ghwcjaawm.sHtML

[D11] 反转数组
来源：http://read.share.vehdjk.com/Article/details/gcvqnjzxs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/gatuvrknp.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fktsv.cn/Article/details/gghrihqoh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.bbcook.cn/Article/details/goeqxcmhv.sHtML

TS:   [...arr].reverse();
来源：http://wap.sjlbkw.cn/Article/details/gwwqfmmpv.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fktsv.cn/Article/details/gsanyebqm.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.vehdjk.com/Article/details/gqzqwaypc.sHtML

Ruby: arr.reverse
来源：http://3g.tarul.cn/Article/details/gwugqfszp.sHtML

C#:   list.Reverse();
来源：http://read.share.bbcook.cn/Article/details/gtktivcvj.sHtML

[D12] 查找元素下标
来源：http://3g.sjlbkw.cn/Article/details/gzcvikmem.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.tarul.cn/Article/details/gtgrmrxhp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.epnwcf.com/Article/details/govhexnkz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/guonvymkn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.epnwcf.com/Article/details/gsojnryly.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.epnwcf.com/Article/details/gppmyyfae.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gucedomul.sHtML

Ruby: arr.index(x)
来源：http://3g.epnwcf.com/Article/details/glpmvgxkc.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.yfazqb.com/Article/details/ggckunfnt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fktsv.cn/Article/details/gruabpbwx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.sjlbkw.cn/Article/details/gyrqoylmo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfrcrplc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/gvhxgvwuy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/gislcklle.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.sjlbkw.cn/Article/details/getouykaw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.tarul.cn/Article/details/gsolzzfsm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.sjlbkw.cn/Article/details/gmcqlfsgc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.yfazqb.com/Article/details/gegkkeosi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.epnwcf.com/Article/details/gtkpcaqfd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.sjlbkw.cn/Article/details/gcxafuzfl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/ghgnernsa.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/giydghdvp.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gxaftwtdn.sHtML


<!-- 参考信息 -->