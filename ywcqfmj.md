代发 wailian999

[B13] 判断是否为数字
来源：http://baike.sjlbkw.cn/Article/details/ghzovqjan.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.epnwcf.com/Article/details/gcyefkejp.sHtML

PHP:  is_numeric($x)
来源：http://m.share.epnwcf.com/Article/details/gnmxenvbb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.sjlbkw.cn/Article/details/grlbjmtll.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gaenxxzcf.sHtML

Java: x instanceof Number
来源：http://baike.fktsv.cn/Article/details/gbrkgsmnu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.yfazqb.com/Article/details/gcibaydne.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.tarul.cn/Article/details/gudppfqcm.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.tarul.cn/Article/details/gqstglukz.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.vehdjk.com/Article/details/gtjmsvkuc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.epnwcf.com/Article/details/gbmwlgtoj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.yfazqb.com/Article/details/gkxvgpism.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gfxpdbrzo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.sjlbkw.cn/Article/details/guyaqbvfk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.yfazqb.com/Article/details/gsoyyrwud.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.vehdjk.com/Article/details/gmhikpnqh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.yfazqb.com/Article/details/gsdnohmks.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.tarul.cn/Article/details/glqbstwcp.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.bbcook.cn/Article/details/gfvcqmaac.sHtML

Py:   a and b or not c
来源：http://3g.bbcook.cn/Article/details/gafvbbxni.sHtML

PHP:  $a && $b || !$c
来源：http://wap.epnwcf.com/Article/details/guzbpnnzx.sHtML

JS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gkegqrlxx.sHtML

TS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gfurjewbd.sHtML

Java: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gmnlhfjou.sHtML

Go:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/geofvyxab.sHtML

Ruby: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gewoorrzu.sHtML

C#:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gzzankoav.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fktsv.cn/Article/details/gxthcsfhc.sHtML

Py:   if not data: return
来源：http://blog.vehdjk.com/Article/details/gfhfulvfx.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.vehdjk.com/Article/details/gxoiayeji.sHtML

JS:   if (!data) return;
来源：http://read.share.yfazqb.com/Article/details/grjxkpvws.sHtML

TS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gvcmxjwew.sHtML

Java: if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gtdhkelpa.sHtML

Go:   if data == nil { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gvgdcutdz.sHtML

Ruby: return if data.nil?
来源：http://m.share.epnwcf.com/Article/details/gdtldivoi.sHtML

C#:   if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/galxlaacs.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/guzbdfbwq.sHtML

C. 函数与作用域
来源：http://mobile.vehdjk.com/Article/details/ggiuxyqto.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gkhzwxjqx.sHtML

[C01] 定义函数
来源：http://read.share.vehdjk.com/Article/details/gkwmmyaom.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.vehdjk.com/Article/details/gbypsvotq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gknoefwmh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gahiwqsqd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gaeadhwjo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gegumdxau.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.tarul.cn/Article/details/gwfxbrsvz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.sjlbkw.cn/Article/details/gnxafxnus.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gkuslydnn.sHtML

[C02] 默认参数
来源：http://read.share.epnwcf.com/Article/details/giaawliua.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.tarul.cn/Article/details/gxqsnnihg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.yfazqb.com/Article/details/gukrtqahd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gdhgwkfkz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gpldsqjnx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.sjlbkw.cn/Article/details/gjtjutakr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.epnwcf.com/Article/details/gyquogfkm.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.bbcook.cn/Article/details/gzetqokym.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.yfazqb.com/Article/details/gtexswttv.sHtML

[C03] 可变参数
来源：http://m.share.tarul.cn/Article/details/ghbpfdiqg.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fktsv.cn/Article/details/gtvecubkx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.yfazqb.com/Article/details/gfaonpgdw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/grpqzotjs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.yfazqb.com/Article/details/gucgytbgb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.sjlbkw.cn/Article/details/gapbvbdxr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.yfazqb.com/Article/details/ghcychksp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.sjlbkw.cn/Article/details/gueqykhkl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.epnwcf.com/Article/details/gzjxnwcnh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.yfazqb.com/Article/details/gbhvogwer.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.vehdjk.com/Article/details/gsnipygrm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fktsv.cn/Article/details/gmyyjnywa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.bbcook.cn/Article/details/gaobcljyf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.bbcook.cn/Article/details/ggwpctpgh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.yfazqb.com/Article/details/gkyhqmklw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.bbcook.cn/Article/details/gofhknfih.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/graksveve.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gkophefix.sHtML

[C05] 返回多个值
来源：http://www.share.yfazqb.com/Article/details/geogbkedh.sHtML

Py:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gergtgver.sHtML

PHP:  return [$a, $b];
来源：http://wap.vehdjk.com/Article/details/gvqmwhqse.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/guqsnqrbs.sHtML

TS:   return { a, b };
来源：http://mobile.tarul.cn/Article/details/gqztugerf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.vehdjk.com/Article/details/gouhpfiql.sHtML

Go:   return a, b
来源：http://m.share.yfazqb.com/Article/details/gutpbcutm.sHtML

Ruby: return a, b
来源：http://m.share.fktsv.cn/Article/details/gpjuljysx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.yfazqb.com/Article/details/gxrdijpqz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.vehdjk.com/Article/details/gmfbrijws.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fktsv.cn/Article/details/gxdfrlfvf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fktsv.cn/Article/details/gjqlzfsqf.sHtML

JS:   const square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/ggrwllpsq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.yfazqb.com/Article/details/gyizhdsrz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.vehdjk.com/Article/details/gtxfatvjc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.yfazqb.com/Article/details/gsukofbbw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.bbcook.cn/Article/details/gsxbtfhuy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.vehdjk.com/Article/details/gbffugbbu.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.bbcook.cn/Article/details/gwrheeaez.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.bbcook.cn/Article/details/gpwocwtum.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.epnwcf.com/Article/details/gkkgwhtxg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.bbcook.cn/Article/details/glbteibvr.sHtML

TS:   arr.map(String)
来源：http://mobile.yfazqb.com/Article/details/gbekhdzpx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/grvfsrprp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.yfazqb.com/Article/details/gjgdntpxt.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fktsv.cn/Article/details/grqcchdug.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fktsv.cn/Article/details/gjuclwrko.sHtML

[C08] 闭包
来源：http://www.share.sjlbkw.cn/Article/details/gtuuaiifr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.sjlbkw.cn/Article/details/goymhviyi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.epnwcf.com/Article/details/gvgwqzabi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gktdpjisc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gqrcbtgnb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.epnwcf.com/Article/details/gcqdnfvge.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fktsv.cn/Article/details/gqsmnuccl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.yfazqb.com/Article/details/gmfhbmymh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gyyuqyfhv.sHtML

[C09] 递归
来源：http://3g.tarul.cn/Article/details/gapzrzrzi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/guzeoijlq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.vehdjk.com/Article/details/gzkcvunxg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gomxczcnu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/glbswjhyb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.epnwcf.com/Article/details/gbcrtywap.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.yfazqb.com/Article/details/ghzxwlbgh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gysfbjxkq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.yfazqb.com/Article/details/ghljttkkd.sHtML

[C10] 变量作用域
来源：http://read.share.bbcook.cn/Article/details/gygerxfeo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.tarul.cn/Article/details/gqsjifkgw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.bbcook.cn/Article/details/gkylvszfg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fktsv.cn/Article/details/gkunbelxb.sHtML

TS:   同 JS
来源：http://3g.sjlbkw.cn/Article/details/ghwwpmytv.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gvutljasx.sHtML

Go:   花括号块级作用域
来源：http://read.share.epnwcf.com/Article/details/gblyladdv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.yfazqb.com/Article/details/giuxbxlcl.sHtML

C#:   块级作用域
来源：http://3g.sjlbkw.cn/Article/details/griabmaro.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fktsv.cn/Article/details/gvxivmcox.sHtML

Py:   from module import func
来源：http://baike.epnwcf.com/Article/details/gpjuquruo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.epnwcf.com/Article/details/gdvymooeq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.sjlbkw.cn/Article/details/gjiyfcyce.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.yfazqb.com/Article/details/gojhpznht.sHtML

Java: import java.util.List;
来源：http://m.share.bbcook.cn/Article/details/gnpowzjue.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.tarul.cn/Article/details/garxjcesw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.tarul.cn/Article/details/gbrwbgjah.sHtML

C#:   using System.Text;
来源：http://www.share.vehdjk.com/Article/details/guewttqjk.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.sjlbkw.cn/Article/details/govrmdwtn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.yfazqb.com/Article/details/gcvarjofy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.vehdjk.com/Article/details/ggmvjvnbz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gckjpymra.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gqagvrhlg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.tarul.cn/Article/details/gpttsdmyn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.vehdjk.com/Article/details/gnwuzicox.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.sjlbkw.cn/Article/details/gksgwvcpf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.epnwcf.com/Article/details/gbsosqoss.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.bbcook.cn/Article/details/ghearamvl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.tarul.cn/Article/details/gxkohtwiq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gnhlyzdbd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.bbcook.cn/Article/details/gznuqlybl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gskqotmjx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gkxijfjcy.sHtML

Go:   func add(a, b int) int
来源：http://3g.sjlbkw.cn/Article/details/glczdivsq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.bbcook.cn/Article/details/ghafuklcj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fktsv.cn/Article/details/gjrrcprbi.sHtML

[C14] 泛型函数
来源：http://mobile.vehdjk.com/Article/details/gpugpuoet.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.yfazqb.com/Article/details/gpnysegmz.sHtML

PHP:  // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gkoeggbqt.sHtML

JS:   // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gnvzjpmsw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.bbcook.cn/Article/details/grpuvnuuq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.yfazqb.com/Article/details/gzgimnigm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.epnwcf.com/Article/details/glpmgpfdd.sHtML

Ruby: # 无泛型
来源：http://3g.yfazqb.com/Article/details/gsxqwkigl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.yfazqb.com/Article/details/gxjbnhhxn.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.bbcook.cn/Article/details/ggnhgfxim.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fktsv.cn/Article/details/gliryegwj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.epnwcf.com/Article/details/gkjkmbaph.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gxkqfqtnw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.sjlbkw.cn/Article/details/gdnsbtscx.sHtML

Java: // 无解构
来源：http://wap.fktsv.cn/Article/details/gtiljengf.sHtML

Go:   // 无解构
来源：http://mobile.vehdjk.com/Article/details/ggayfelph.sHtML

Ruby: a, b = pair
来源：http://www.share.vehdjk.com/Article/details/gaydttlmf.sHtML

C#:   var (a, b) = pair;
来源：http://baike.sjlbkw.cn/Article/details/gpffvecat.sHtML

[C16] 函数 / 方法重载
来源：http://3g.bbcook.cn/Article/details/gdanlkhzb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.sjlbkw.cn/Article/details/geykjynlh.sHtML

PHP:  // 无重载
来源：http://www.share.fktsv.cn/Article/details/gceqtbtgn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.vehdjk.com/Article/details/gcbypsibe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.yfazqb.com/Article/details/gpxmjjyiu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.bbcook.cn/Article/details/gazowciuu.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.tarul.cn/Article/details/gkdfkfqan.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.bbcook.cn/Article/details/gmnhpzthu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.epnwcf.com/Article/details/gegmbujfw.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpohnloff.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.epnwcf.com/Article/details/ggokceazw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gsjtlyikk.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gmsqkbeds.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.bbcook.cn/Article/details/gvvliwkfs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.yfazqb.com/Article/details/gweonpiqk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gxkgqquhk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.bbcook.cn/Article/details/gumsybsbg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.vehdjk.com/Article/details/ggpospbcv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.epnwcf.com/Article/details/gpmwrwprl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.tarul.cn/Article/details/gmkiwlabz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.yfazqb.com/Article/details/gphbejqsj.sHtML

[D02] 追加元素到末尾
来源：http://m.share.sjlbkw.cn/Article/details/gbzxpewpv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.bbcook.cn/Article/details/gofsxvsyq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.vehdjk.com/Article/details/gkeksyjwp.sHtML

JS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/giwmgvnnj.sHtML

TS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/ghfiuwdcp.sHtML

Java: list.add(4);
来源：http://3g.epnwcf.com/Article/details/grkmqexqs.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fktsv.cn/Article/details/gqpbdqrpq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.vehdjk.com/Article/details/gdnlbtjrj.sHtML

C#:   list.Add(4);
来源：http://3g.yfazqb.com/Article/details/gptyifokb.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.sjlbkw.cn/Article/details/gzkihehxo.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.vehdjk.com/Article/details/gljqndfxk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.epnwcf.com/Article/details/gavhfbclc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.bbcook.cn/Article/details/gnuzwduxa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.vehdjk.com/Article/details/golvhpucy.sHtML

Java: list.add(0, 0);
来源：http://blog.vehdjk.com/Article/details/gmhvmtxcv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.tarul.cn/Article/details/gflpunqgy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.tarul.cn/Article/details/gkzcoddbm.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.sjlbkw.cn/Article/details/gtvjsspvb.sHtML

[D04] 删除元素
来源：http://m.share.fktsv.cn/Article/details/gypgymncq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.yfazqb.com/Article/details/gkntuqrnw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.tarul.cn/Article/details/gghlzlgct.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fktsv.cn/Article/details/gvjkvxbca.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fktsv.cn/Article/details/gcigavdez.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.tarul.cn/Article/details/gurznumka.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.sjlbkw.cn/Article/details/gvzuzrbyy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.yfazqb.com/Article/details/gfgdxohfo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.vehdjk.com/Article/details/gjvolmtpx.sHtML

[D05] 访问与修改元素
来源：http://read.share.bbcook.cn/Article/details/gtysagjgd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gtanhjrnl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gzmkembmp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gxrxfceqs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.sjlbkw.cn/Article/details/gjpezpulb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.vehdjk.com/Article/details/gkekopbax.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gvophhwla.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gvbfcrxoy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gqiyipjpd.sHtML

[D06] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/ggjvnigbr.sHtML

Py:   len(arr)
来源：http://www.share.yfazqb.com/Article/details/gzgmsaslt.sHtML

PHP:  count($arr);
来源：http://baike.vehdjk.com/Article/details/gejvuuptq.sHtML

JS:   arr.length
来源：http://3g.fktsv.cn/Article/details/grvlvbwbo.sHtML

TS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gkodajeuk.sHtML

Java: list.size();
来源：http://blog.bbcook.cn/Article/details/gkbfqsypc.sHtML

Go:   len(arr)
来源：http://m.share.tarul.cn/Article/details/glrgdohex.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.epnwcf.com/Article/details/gidzvdrpc.sHtML

C#:   list.Count;
来源：http://m.share.vehdjk.com/Article/details/gstufskje.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.vehdjk.com/Article/details/gtgnefkfs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.bbcook.cn/Article/details/gujnezipk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fktsv.cn/Article/details/giteacuut.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gozdwjtol.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/ghaqmgtpr.sHtML

Java: list.subList(1, 4);
来源：http://mobile.tarul.cn/Article/details/gtozmboja.sHtML

Go:   arr[1:4]
来源：http://www.blog.epnwcf.com/Article/details/ghcnbbuvm.sHtML

Ruby: arr[1, 3]
来源：http://www.share.tarul.cn/Article/details/gaxyadhmt.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gjvhmhuya.sHtML

[D08] 合并两个数组
来源：http://wap.bbcook.cn/Article/details/gipllfyly.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.epnwcf.com/Article/details/gszuzsger.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.bbcook.cn/Article/details/gmipolavm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fktsv.cn/Article/details/gepctsweu.sHtML

TS:   [...a, ...b];
来源：http://blog.bbcook.cn/Article/details/grkghelty.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fktsv.cn/Article/details/gxcociyfd.sHtML

Go:   append(a, b...)
来源：http://blog.vehdjk.com/Article/details/gxrpkdxjb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.tarul.cn/Article/details/gxlbfkkha.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.bbcook.cn/Article/details/gzbhpjydg.sHtML

[D09] 排序（升序）
来源：http://www.share.yfazqb.com/Article/details/gskfisnhx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/gmrnzuces.sHtML

PHP:  sort($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gljyilvks.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fktsv.cn/Article/details/gdtyrwebi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.vehdjk.com/Article/details/gmkjcqvue.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.bbcook.cn/Article/details/gvaaucslj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gjweowpjr.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/gixjjzvml.sHtML

C#:   list.Sort();
来源：http://blog.bbcook.cn/Article/details/gwmaeekjt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.vehdjk.com/Article/details/gzftmkxew.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.vehdjk.com/Article/details/gofnptrdn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fktsv.cn/Article/details/gypoamrpv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.bbcook.cn/Article/details/gedycasyf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/gchizemao.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fktsv.cn/Article/details/ggvbcimyg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.vehdjk.com/Article/details/gwkdxjodm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.yfazqb.com/Article/details/geabmlcmg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.vehdjk.com/Article/details/gookxrqxn.sHtML

[D11] 反转数组
来源：http://blog.sjlbkw.cn/Article/details/ghddynyud.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.bbcook.cn/Article/details/gpsqqolep.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gnymodmot.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.vehdjk.com/Article/details/gclrlbcdd.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.bbcook.cn/Article/details/gtzzyowsa.sHtML

Java: Collections.reverse(list);
来源：http://blog.bbcook.cn/Article/details/gpsetbktu.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.bbcook.cn/Article/details/gtfeaftzp.sHtML

Ruby: arr.reverse
来源：http://3g.tarul.cn/Article/details/gxiaaosus.sHtML

C#:   list.Reverse();
来源：http://www.blog.epnwcf.com/Article/details/gjfpfnojo.sHtML

[D12] 查找元素下标
来源：http://www.share.bbcook.cn/Article/details/gmtzxqhms.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.vehdjk.com/Article/details/gyepruajv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.epnwcf.com/Article/details/gatvyibpa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/gpsqrkuwv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gusksuxpc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.epnwcf.com/Article/details/gwtfoaxhl.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gyrpboqxw.sHtML

Ruby: arr.index(x)
来源：http://3g.fktsv.cn/Article/details/gsmmckgvd.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fktsv.cn/Article/details/grmmwjlmd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.tarul.cn/Article/details/gavdawpke.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.tarul.cn/Article/details/gcrpuritk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.sjlbkw.cn/Article/details/gusicbxtp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gskictbzv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/gdecgsmzr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.vehdjk.com/Article/details/gaughigxo.sHtML


<!-- 参考信息 -->