代发 wailian999

PHP:  range(0, 10, 2);
来源：http://m.share.tarul.cn/Article/details/gkfkfvkci.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/gjunhuodl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/gbgikvmzg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.epnwcf.com/Article/details/glbihpdxo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.yfazqb.com/Article/details/gqowoyocp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fktsv.cn/Article/details/grpdcmlmf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.yfazqb.com/Article/details/gmvslqcqz.sHtML

[B12] 跳出多层循环
来源：http://wap.epnwcf.com/Article/details/gkaiioiun.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.sjlbkw.cn/Article/details/gmrlpujea.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.epnwcf.com/Article/details/gngozszwh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/gtkhqhwuv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gmdvqckio.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gzgwelfnr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.tarul.cn/Article/details/gdocdqbfw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.yfazqb.com/Article/details/gsrojlcxx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.vehdjk.com/Article/details/gnyxxzcfh.sHtML

[B13] 判断是否为数字
来源：http://baike.epnwcf.com/Article/details/gbebfwnzn.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.tarul.cn/Article/details/grjnefqui.sHtML

PHP:  is_numeric($x)
来源：http://3g.bbcook.cn/Article/details/gyoeesnku.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.epnwcf.com/Article/details/ggkzzrslp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.bbcook.cn/Article/details/gywfryady.sHtML

Java: x instanceof Number
来源：http://mobile.sjlbkw.cn/Article/details/gfswkhxhy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.tarul.cn/Article/details/ghxxihuaj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.tarul.cn/Article/details/gzkqbjrru.sHtML

C#:   x is int or double or decimal
来源：http://read.share.sjlbkw.cn/Article/details/gnxelrzzl.sHtML

[B14] 判断值是否在集合内
来源：http://blog.tarul.cn/Article/details/gymvrvmdy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.bbcook.cn/Article/details/gwqdehtuj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.bbcook.cn/Article/details/grtekpruu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/glqpnaous.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.tarul.cn/Article/details/gwvecsajc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gavunhydc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.epnwcf.com/Article/details/ggxxdeatz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.yfazqb.com/Article/details/gbhdhdxyh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fktsv.cn/Article/details/gduesohqr.sHtML

[B15] 布尔运算与取反
来源：http://m.share.yfazqb.com/Article/details/glcerjnzc.sHtML

Py:   a and b or not c
来源：http://m.share.fktsv.cn/Article/details/ghuhthzvi.sHtML

PHP:  $a && $b || !$c
来源：http://blog.yfazqb.com/Article/details/ghdzpjdho.sHtML

JS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gwroxoqer.sHtML

TS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gbjexoogj.sHtML

Java: a && b || !c
来源：http://wap.vehdjk.com/Article/details/gxbqljkvw.sHtML

Go:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gjfjfxwzu.sHtML

Ruby: a && b || !c
来源：http://wap.epnwcf.com/Article/details/grdfcthmm.sHtML

C#:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gezblysfc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.yfazqb.com/Article/details/gxlsrexll.sHtML

Py:   if not data: return
来源：http://www.share.epnwcf.com/Article/details/gfielbnrr.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.yfazqb.com/Article/details/gxlldulyv.sHtML

JS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/ggrsauiim.sHtML

TS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gpetimwdu.sHtML

Java: if (data == null) return;
来源：http://baike.sjlbkw.cn/Article/details/ghlrbqksf.sHtML

Go:   if data == nil { return }
来源：http://baike.sjlbkw.cn/Article/details/gwmexlwfu.sHtML

Ruby: return if data.nil?
来源：http://blog.bbcook.cn/Article/details/gsefmaxmu.sHtML

C#:   if (data == null) return;
来源：http://www.blog.bbcook.cn/Article/details/gtnkqhlpt.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/grpmxnjks.sHtML

C. 函数与作用域
来源：http://baike.yfazqb.com/Article/details/griwvujir.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzhleiyux.sHtML

[C01] 定义函数
来源：http://mobile.bbcook.cn/Article/details/gqtprwjer.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.tarul.cn/Article/details/gfjyhnmpi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gerjxfhxw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gcytfbbby.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gacjwqkne.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gxpzkfcsv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.vehdjk.com/Article/details/gxccoywgi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.epnwcf.com/Article/details/grsbnfcoh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gjftcozaw.sHtML

[C02] 默认参数
来源：http://wap.vehdjk.com/Article/details/githguabn.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.tarul.cn/Article/details/gelbghwvk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.sjlbkw.cn/Article/details/giauuihks.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/gfenwivrh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/ggyngdixe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.vehdjk.com/Article/details/gochdpwjs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.epnwcf.com/Article/details/glnhszgto.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fktsv.cn/Article/details/gyontqyem.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.sjlbkw.cn/Article/details/ggukvrckj.sHtML

[C03] 可变参数
来源：http://www.blog.epnwcf.com/Article/details/gxxcujizj.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.sjlbkw.cn/Article/details/gedpetads.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.epnwcf.com/Article/details/gpazsiemz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gptptbreq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/gnjvpjjce.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.tarul.cn/Article/details/gsgepsfwq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fktsv.cn/Article/details/gdaszdjny.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.vehdjk.com/Article/details/gswiohwzq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.bbcook.cn/Article/details/gmhiypcnb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.sjlbkw.cn/Article/details/gqlzwyobz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.sjlbkw.cn/Article/details/gumjbnybg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.tarul.cn/Article/details/gkjazyosq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gsavzmfje.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.sjlbkw.cn/Article/details/gkbgittnt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fktsv.cn/Article/details/gaemedfiy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fktsv.cn/Article/details/ggzkvldun.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/giutriafu.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gypaxjsus.sHtML

[C05] 返回多个值
来源：http://3g.fktsv.cn/Article/details/giutaqzgm.sHtML

Py:   return a, b
来源：http://www.share.tarul.cn/Article/details/grewfhzpd.sHtML

PHP:  return [$a, $b];
来源：http://baike.yfazqb.com/Article/details/ggziupgrt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gsjvavwez.sHtML

TS:   return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/glbeslitu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.yfazqb.com/Article/details/gnahkjwir.sHtML

Go:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gqnwtonok.sHtML

Ruby: return a, b
来源：http://blog.vehdjk.com/Article/details/gkbudykuf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.yfazqb.com/Article/details/gimynfvjs.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.tarul.cn/Article/details/geunsoktc.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fktsv.cn/Article/details/gppgoekfz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.sjlbkw.cn/Article/details/gytpwoyns.sHtML

JS:   const square = x => x * x;
来源：http://wap.vehdjk.com/Article/details/gmuneqnbe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.sjlbkw.cn/Article/details/ggmerfrzi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.tarul.cn/Article/details/gbhsuyatf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.yfazqb.com/Article/details/gxfoaiwep.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.tarul.cn/Article/details/gplfjfvhz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/gpmxjxgnp.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.epnwcf.com/Article/details/gewaicixe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.vehdjk.com/Article/details/ggzsmpxjq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fktsv.cn/Article/details/gsrqhbigg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.bbcook.cn/Article/details/gmejcczex.sHtML

TS:   arr.map(String)
来源：http://www.m.share.bbcook.cn/Article/details/gqjpsdxng.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/gtrbkuwwb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.epnwcf.com/Article/details/gdzjniiks.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.tarul.cn/Article/details/gdyglensr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.tarul.cn/Article/details/gjeqnbcuz.sHtML

[C08] 闭包
来源：http://baike.bbcook.cn/Article/details/gtjwepama.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.sjlbkw.cn/Article/details/gktkaheui.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.yfazqb.com/Article/details/ggaxkabqn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.bbcook.cn/Article/details/gxsqsqcht.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/grlkcdnsm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fktsv.cn/Article/details/gecqpxrms.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fktsv.cn/Article/details/gqsbwpysi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fktsv.cn/Article/details/glhlcniqu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gyjholhtb.sHtML

[C09] 递归
来源：http://www.blog.bbcook.cn/Article/details/gvtkfhfue.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.epnwcf.com/Article/details/gdskdiyjx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.vehdjk.com/Article/details/gyswaryqc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.epnwcf.com/Article/details/gmtzdxzul.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gwcjeodyx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.sjlbkw.cn/Article/details/gnhcevcoq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.bbcook.cn/Article/details/gznubtoyt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/glsetipav.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.bbcook.cn/Article/details/gpqdaosse.sHtML

[C10] 变量作用域
来源：http://www.share.bbcook.cn/Article/details/gysmahoub.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.bbcook.cn/Article/details/ghzolsviz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fktsv.cn/Article/details/gymnqgdmd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fktsv.cn/Article/details/gazjxgsvh.sHtML

TS:   同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gudreaoxm.sHtML

Java: 方法内为块级作用域
来源：http://wap.epnwcf.com/Article/details/ghmuqyubc.sHtML

Go:   花括号块级作用域
来源：http://www.share.fktsv.cn/Article/details/gqglxwkhq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.epnwcf.com/Article/details/gfvfbrvtc.sHtML

C#:   块级作用域
来源：http://m.share.bbcook.cn/Article/details/glyddiieq.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.epnwcf.com/Article/details/glcxdrcng.sHtML

Py:   from module import func
来源：http://m.share.tarul.cn/Article/details/gqowgmdyu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.epnwcf.com/Article/details/gvasakyvn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.tarul.cn/Article/details/gyfpfzwpg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.tarul.cn/Article/details/gpbbjcmnm.sHtML

Java: import java.util.List;
来源：http://www.share.bbcook.cn/Article/details/gyrdrybcl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.sjlbkw.cn/Article/details/gajekeztg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/gadhslrkv.sHtML

C#:   using System.Text;
来源：http://read.share.tarul.cn/Article/details/gdowxabok.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.vehdjk.com/Article/details/gunadrzwr.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.vehdjk.com/Article/details/gjyljtaqc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.epnwcf.com/Article/details/gxhwepnsn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/gpxbgpscy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gneovqzlq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.sjlbkw.cn/Article/details/gfitnthdw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.sjlbkw.cn/Article/details/gumwvwsvs.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.epnwcf.com/Article/details/gcruilkfh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqelcecza.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fktsv.cn/Article/details/galjvwsqs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gvcobqinq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gpkhkoneg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.yfazqb.com/Article/details/gtfumkusl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/ghsudrfax.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gelqqqgsy.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.vehdjk.com/Article/details/gkztxjzse.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.vehdjk.com/Article/details/glmainhot.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.sjlbkw.cn/Article/details/guoaeqxbb.sHtML

[C14] 泛型函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpppwugb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.tarul.cn/Article/details/gouyiqfnm.sHtML

PHP:  // 无泛型
来源：http://m.share.epnwcf.com/Article/details/gbbwpogrs.sHtML

JS:   // 无泛型
来源：http://mobile.yfazqb.com/Article/details/gpggyobdj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fktsv.cn/Article/details/gmtthesse.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.vehdjk.com/Article/details/gavjecwka.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.epnwcf.com/Article/details/gqlkqdnsk.sHtML

Ruby: # 无泛型
来源：http://read.share.yfazqb.com/Article/details/gpaalratq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.sjlbkw.cn/Article/details/gwtnksexg.sHtML

[C15] 解构 / 展开参数
来源：http://blog.yfazqb.com/Article/details/gluzjooss.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.sjlbkw.cn/Article/details/guqmajefa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fktsv.cn/Article/details/gyrnebgtq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gpliiiwfc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.epnwcf.com/Article/details/gtqpiqaij.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/gikuzcihp.sHtML

Go:   // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjbudvac.sHtML

Ruby: a, b = pair
来源：http://www.share.epnwcf.com/Article/details/gwmlribym.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.tarul.cn/Article/details/gahmsojts.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.yfazqb.com/Article/details/gzsjuavud.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.tarul.cn/Article/details/gqmeosrif.sHtML

PHP:  // 无重载
来源：http://blog.yfazqb.com/Article/details/gcchpnmzu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fktsv.cn/Article/details/gcdhjgpki.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.yfazqb.com/Article/details/grddvdqdh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.epnwcf.com/Article/details/gqrydgrqm.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.sjlbkw.cn/Article/details/gngduqnxp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.vehdjk.com/Article/details/gjynqnyqp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fktsv.cn/Article/details/gdbgqyxiv.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/grizmuagf.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.bbcook.cn/Article/details/gorzlcrol.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gcverubku.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/gednjztoe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.yfazqb.com/Article/details/gkhajmxaf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.bbcook.cn/Article/details/girschkjj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.epnwcf.com/Article/details/gwnfdtnad.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fktsv.cn/Article/details/gqeaydofn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.vehdjk.com/Article/details/gdfpjaokw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.tarul.cn/Article/details/gynklvtos.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.bbcook.cn/Article/details/ghrkyylgl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.yfazqb.com/Article/details/gnzyodtul.sHtML

[D02] 追加元素到末尾
来源：http://blog.vehdjk.com/Article/details/gjiaeepte.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.vehdjk.com/Article/details/gfsomgcxc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.bbcook.cn/Article/details/ghwmcsjma.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/grcwjcudy.sHtML

TS:   arr.push(4);
来源：http://read.share.tarul.cn/Article/details/gxlznvrib.sHtML

Java: list.add(4);
来源：http://wap.fktsv.cn/Article/details/gpuhxtyhg.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.tarul.cn/Article/details/ghebmlmlz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fktsv.cn/Article/details/gmlzfafqb.sHtML

C#:   list.Add(4);
来源：http://www.m.share.yfazqb.com/Article/details/gaexzulgm.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.epnwcf.com/Article/details/gqddqalqt.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/gzjxrihxf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.yfazqb.com/Article/details/ggcsmdkog.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.vehdjk.com/Article/details/gzskjiyrs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gseljlgyl.sHtML

Java: list.add(0, 0);
来源：http://m.share.bbcook.cn/Article/details/gpdjyauow.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.vehdjk.com/Article/details/gvrllgfab.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.yfazqb.com/Article/details/gbulwwiwp.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.epnwcf.com/Article/details/glhhgbchk.sHtML

[D04] 删除元素
来源：http://wap.yfazqb.com/Article/details/gxudvujkj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.sjlbkw.cn/Article/details/gvxtucato.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.epnwcf.com/Article/details/gewdxkvfc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.yfazqb.com/Article/details/ggabwuzol.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.sjlbkw.cn/Article/details/gncgntgzb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.sjlbkw.cn/Article/details/gcdvrwdfz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.bbcook.cn/Article/details/gfkstpnfx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.tarul.cn/Article/details/gajhxdbad.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.tarul.cn/Article/details/gouobmndk.sHtML

[D05] 访问与修改元素
来源：http://wap.tarul.cn/Article/details/gbtcgxmkn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gbztqzqvo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.bbcook.cn/Article/details/grtwbntmw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/gxjtvqwor.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fktsv.cn/Article/details/gqcxqbbwq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.epnwcf.com/Article/details/gtpdzwmdg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/geeykjjrm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gzwioehfw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gprghupvd.sHtML

[D06] 数组长度
来源：http://3g.vehdjk.com/Article/details/gqybnvwbm.sHtML

Py:   len(arr)
来源：http://www.share.epnwcf.com/Article/details/gblwdtkxm.sHtML

PHP:  count($arr);
来源：http://mobile.tarul.cn/Article/details/gtqoqjosf.sHtML

JS:   arr.length
来源：http://www.share.bbcook.cn/Article/details/gczmafbfe.sHtML

TS:   arr.length
来源：http://www.share.fktsv.cn/Article/details/glraefynp.sHtML

Java: list.size();
来源：http://www.blog.vehdjk.com/Article/details/gjslucphl.sHtML

Go:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/gkeaveece.sHtML

Ruby: arr.length; arr.size
来源：http://3g.sjlbkw.cn/Article/details/gopkzgcus.sHtML

C#:   list.Count;
来源：http://www.m.share.tarul.cn/Article/details/gubzkcpiy.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.yfazqb.com/Article/details/gkonklgoa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.sjlbkw.cn/Article/details/gynyfsmph.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.epnwcf.com/Article/details/gdeulnvxr.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gcaracywc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/giggjqxsl.sHtML

Java: list.subList(1, 4);
来源：http://blog.epnwcf.com/Article/details/gdelddbwl.sHtML

Go:   arr[1:4]
来源：http://www.m.share.tarul.cn/Article/details/gbtsmesdv.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.epnwcf.com/Article/details/gfliqvlxb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.epnwcf.com/Article/details/gbelhdhlc.sHtML

[D08] 合并两个数组
来源：http://baike.sjlbkw.cn/Article/details/gituuenbc.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.epnwcf.com/Article/details/gmmcpwqra.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.sjlbkw.cn/Article/details/gffvlfjpq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fktsv.cn/Article/details/gdlhxsygm.sHtML

TS:   [...a, ...b];
来源：http://www.blog.yfazqb.com/Article/details/grlrjonbt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.epnwcf.com/Article/details/gqqgmdxwj.sHtML

Go:   append(a, b...)
来源：http://m.share.epnwcf.com/Article/details/ghevjhevx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.tarul.cn/Article/details/gdzckczef.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.tarul.cn/Article/details/gqaaxrhjv.sHtML

[D09] 排序（升序）
来源：http://www.share.bbcook.cn/Article/details/gddklqjfu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/gllkzmovl.sHtML

PHP:  sort($arr);
来源：http://blog.tarul.cn/Article/details/gtljftfzo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.bbcook.cn/Article/details/gwywubwmc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.bbcook.cn/Article/details/glpjyscpa.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.epnwcf.com/Article/details/gvueejjgc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gdmjhlgcs.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfmxbryz.sHtML

C#:   list.Sort();
来源：http://mobile.epnwcf.com/Article/details/gpahbdlpd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fktsv.cn/Article/details/gqfodjtct.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.tarul.cn/Article/details/gnzhhcmkh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/gqgjrepuj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.bbcook.cn/Article/details/gibzjkkfm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.epnwcf.com/Article/details/gdxasgdcg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.bbcook.cn/Article/details/ghnziotsf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.epnwcf.com/Article/details/gygfhiewm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.sjlbkw.cn/Article/details/gbetnqful.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.vehdjk.com/Article/details/givyjpggw.sHtML

[D11] 反转数组
来源：http://wap.tarul.cn/Article/details/gbkcekodh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.epnwcf.com/Article/details/gtoxmyzwx.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.bbcook.cn/Article/details/gjidncwdv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fktsv.cn/Article/details/gdhmzjqve.sHtML

TS:   [...arr].reverse();
来源：http://3g.epnwcf.com/Article/details/ggosercxs.sHtML

Java: Collections.reverse(list);
来源：http://baike.yfazqb.com/Article/details/goqyckaoi.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fktsv.cn/Article/details/gjkmwgsjq.sHtML

Ruby: arr.reverse
来源：http://read.share.vehdjk.com/Article/details/gcttczkgc.sHtML


<!-- 参考信息 -->