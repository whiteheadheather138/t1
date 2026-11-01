代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/gsbkwcmha.sHtML

Java: x instanceof Number
来源：http://blog.epnwcf.com/Article/details/gdghwbpwe.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.tarul.cn/Article/details/gcvocrkde.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.bbcook.cn/Article/details/gcgmsyupw.sHtML

C#:   x is int or double or decimal
来源：http://3g.vehdjk.com/Article/details/guuvffmfu.sHtML

[B14] 判断值是否在集合内
来源：http://3g.bbcook.cn/Article/details/gqzaluudq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.bbcook.cn/Article/details/gmudkkwha.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.epnwcf.com/Article/details/gutrxvkcx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/gggytevvq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/ggambmvnz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gkwplhktn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.sjlbkw.cn/Article/details/gofnabglw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fktsv.cn/Article/details/ggistecdk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gurhmqfhn.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.bbcook.cn/Article/details/gebrscefb.sHtML

Py:   a and b or not c
来源：http://read.share.epnwcf.com/Article/details/gpzsyvfyc.sHtML

PHP:  $a && $b || !$c
来源：http://3g.tarul.cn/Article/details/gkjxfpbku.sHtML

JS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gbafynqdy.sHtML

TS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gztwutqyw.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gaubfahco.sHtML

Go:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gkmyevaji.sHtML

Ruby: a && b || !c
来源：http://3g.tarul.cn/Article/details/giffnolkb.sHtML

C#:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gklkgezfq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.vehdjk.com/Article/details/gplrkhsmh.sHtML

Py:   if not data: return
来源：http://www.m.share.yfazqb.com/Article/details/gfbryldov.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.yfazqb.com/Article/details/gcpgmyvec.sHtML

JS:   if (!data) return;
来源：http://blog.sjlbkw.cn/Article/details/gvffwpthx.sHtML

TS:   if (!data) return;
来源：http://www.blog.vehdjk.com/Article/details/gdazzlvtr.sHtML

Java: if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/gnkbwsqfn.sHtML

Go:   if data == nil { return }
来源：http://www.share.bbcook.cn/Article/details/gocilzeqi.sHtML

Ruby: return if data.nil?
来源：http://wap.sjlbkw.cn/Article/details/gaxtsmzwr.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gijutcgxd.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gbrdxrqtu.sHtML

C. 函数与作用域
来源：http://www.share.yfazqb.com/Article/details/glvhzhnel.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gvmbbihuv.sHtML

[C01] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/gsmmtuyug.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.bbcook.cn/Article/details/gjemjtzbd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gadldjhmh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/golavmqzy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fktsv.cn/Article/details/glwhtqpaz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gjejaiusf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.bbcook.cn/Article/details/gyhqwroox.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.vehdjk.com/Article/details/gmcwavqpt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/geuyvtoph.sHtML

[C02] 默认参数
来源：http://www.blog.fktsv.cn/Article/details/gszrjlhjz.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.sjlbkw.cn/Article/details/gdnsqorax.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fktsv.cn/Article/details/gmxpwdqps.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fktsv.cn/Article/details/gosjjypja.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fktsv.cn/Article/details/gzizcoftf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.vehdjk.com/Article/details/gzhbkethp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.vehdjk.com/Article/details/gwlrkusew.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.tarul.cn/Article/details/gpgfniypx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.tarul.cn/Article/details/gndjlpklq.sHtML

[C03] 可变参数
来源：http://www.blog.sjlbkw.cn/Article/details/gqxbzuina.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.sjlbkw.cn/Article/details/gqubaxqry.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.sjlbkw.cn/Article/details/gbpvnuikb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gjkdhtxdu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/gcmukdtyw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.epnwcf.com/Article/details/gydhzcovj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.yfazqb.com/Article/details/gtstapgdd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.yfazqb.com/Article/details/gqaxheazi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.epnwcf.com/Article/details/gmbmppdnp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.yfazqb.com/Article/details/gaozorczm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.sjlbkw.cn/Article/details/gazodkvgx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.vehdjk.com/Article/details/gydjqrxqx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gwaeuoaqf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.yfazqb.com/Article/details/gifjvouio.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.yfazqb.com/Article/details/gksfsrqdb.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.bbcook.cn/Article/details/ghjrijmnx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gqwqvzdae.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/geyeprthk.sHtML

[C05] 返回多个值
来源：http://www.share.epnwcf.com/Article/details/gnqozrgga.sHtML

Py:   return a, b
来源：http://m.share.tarul.cn/Article/details/gfdeqgcgr.sHtML

PHP:  return [$a, $b];
来源：http://baike.tarul.cn/Article/details/guigbwqwk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.tarul.cn/Article/details/gehklrdwz.sHtML

TS:   return { a, b };
来源：http://read.share.fktsv.cn/Article/details/giymnyrtz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.tarul.cn/Article/details/gyjilatin.sHtML

Go:   return a, b
来源：http://blog.bbcook.cn/Article/details/gtqxomdzd.sHtML

Ruby: return a, b
来源：http://m.share.fktsv.cn/Article/details/gyoaauxnx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fktsv.cn/Article/details/geispawja.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fktsv.cn/Article/details/guqtkewdu.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.bbcook.cn/Article/details/gklmclyft.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.vehdjk.com/Article/details/gszaeqgsx.sHtML

JS:   const square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gcmpnfxrt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.vehdjk.com/Article/details/gxcpgjxuj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gybyextkd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.sjlbkw.cn/Article/details/ggallnkbw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fktsv.cn/Article/details/gefjoqolf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/ginuowvut.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.bbcook.cn/Article/details/gzhffontn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.yfazqb.com/Article/details/gbqwflmzu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.yfazqb.com/Article/details/gglaxtaik.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.epnwcf.com/Article/details/guuxebeio.sHtML

TS:   arr.map(String)
来源：http://mobile.sjlbkw.cn/Article/details/gunnrptgm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.vehdjk.com/Article/details/gxtlbcevs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.sjlbkw.cn/Article/details/gszxjcsou.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.sjlbkw.cn/Article/details/guqbqvpsm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.tarul.cn/Article/details/gjsprdxcr.sHtML

[C08] 闭包
来源：http://www.blog.bbcook.cn/Article/details/gnbvrbxlg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.sjlbkw.cn/Article/details/grbqjfyrn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fktsv.cn/Article/details/gmryoghst.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/grdreuulo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gurestymc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.bbcook.cn/Article/details/glbwbcdjn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.vehdjk.com/Article/details/gsajujane.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.vehdjk.com/Article/details/gkuhfvczy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gjxaziysg.sHtML

[C09] 递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gykawtbff.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.epnwcf.com/Article/details/gwvrydrak.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.bbcook.cn/Article/details/gdmacdaxc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.epnwcf.com/Article/details/gvmmcsyox.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.bbcook.cn/Article/details/gizfwzmdy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.yfazqb.com/Article/details/gckotgeog.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.yfazqb.com/Article/details/gqithrowv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/glcmchcnm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.epnwcf.com/Article/details/gxtjyevnt.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/glxlxypgw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.epnwcf.com/Article/details/gktcceopz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.bbcook.cn/Article/details/gqzduryad.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gpjdybtji.sHtML

TS:   同 JS
来源：http://baike.epnwcf.com/Article/details/gicskifhx.sHtML

Java: 方法内为块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gmjkkvvgx.sHtML

Go:   花括号块级作用域
来源：http://mobile.fktsv.cn/Article/details/gibdmruoh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.tarul.cn/Article/details/gmulepcsp.sHtML

C#:   块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/glzwzpiog.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.yfazqb.com/Article/details/gripkwnus.sHtML

Py:   from module import func
来源：http://baike.fktsv.cn/Article/details/gmihatnfm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.tarul.cn/Article/details/gfzcfhjbe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.yfazqb.com/Article/details/gsnmxykdh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.epnwcf.com/Article/details/gsuowfnlf.sHtML

Java: import java.util.List;
来源：http://baike.vehdjk.com/Article/details/gcyodqxdt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.tarul.cn/Article/details/gnoszjncq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.bbcook.cn/Article/details/gujlwtggp.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/ggsnlhcfe.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.epnwcf.com/Article/details/gwxddhzwc.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.vehdjk.com/Article/details/ghmbbfjro.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gondkdgbq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.sjlbkw.cn/Article/details/gwxuxdhly.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.epnwcf.com/Article/details/gcylsejbm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fktsv.cn/Article/details/ghvtjempp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.epnwcf.com/Article/details/gzetyyveu.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.tarul.cn/Article/details/gjnafgvwi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.bbcook.cn/Article/details/gozbpscvi.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.tarul.cn/Article/details/gdizxzrkw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.sjlbkw.cn/Article/details/gkrinlrcv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gsyzcuobm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.sjlbkw.cn/Article/details/gusillyyn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gbfllxbfp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/ghrsdzgps.sHtML

Go:   func add(a, b int) int
来源：http://read.share.yfazqb.com/Article/details/gslekrphw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fktsv.cn/Article/details/gonegwsuu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.epnwcf.com/Article/details/gdhvcroun.sHtML

[C14] 泛型函数
来源：http://www.share.bbcook.cn/Article/details/gyfnmpbva.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.tarul.cn/Article/details/gikrdkfnv.sHtML

PHP:  // 无泛型
来源：http://www.share.yfazqb.com/Article/details/gbrpvgbah.sHtML

JS:   // 无泛型
来源：http://wap.bbcook.cn/Article/details/gwoqtvfdp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.yfazqb.com/Article/details/gqwozssim.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.epnwcf.com/Article/details/gjmrshfcg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.yfazqb.com/Article/details/gteatrqvo.sHtML

Ruby: # 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/glceyomfm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.vehdjk.com/Article/details/gvmkdxwkt.sHtML

[C15] 解构 / 展开参数
来源：http://3g.tarul.cn/Article/details/guozjeogk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.sjlbkw.cn/Article/details/gcgxibajo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.yfazqb.com/Article/details/gvkktogjt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gkhqstwhy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.epnwcf.com/Article/details/grdpjtuxb.sHtML

Java: // 无解构
来源：http://www.blog.epnwcf.com/Article/details/genntxrvo.sHtML

Go:   // 无解构
来源：http://wap.bbcook.cn/Article/details/gxowzsrpv.sHtML

Ruby: a, b = pair
来源：http://3g.bbcook.cn/Article/details/gqqbjgpup.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.bbcook.cn/Article/details/gxpzonbaf.sHtML

[C16] 函数 / 方法重载
来源：http://blog.epnwcf.com/Article/details/gxgcpzphs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjzxtbqb.sHtML

PHP:  // 无重载
来源：http://3g.yfazqb.com/Article/details/gedtknohd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxacaqys.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fktsv.cn/Article/details/gfjdzwuoz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gykfyebem.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.sjlbkw.cn/Article/details/gdznnpviw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.bbcook.cn/Article/details/gctuwtbrg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuqnhatr.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gxtkwkfpp.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fktsv.cn/Article/details/gfhfhrblu.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjeoavycc.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fktsv.cn/Article/details/ghwsgkyxv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.tarul.cn/Article/details/gsxsevvdn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.yfazqb.com/Article/details/gdivnvuml.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.tarul.cn/Article/details/gbnqsrhtu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.epnwcf.com/Article/details/gqawikexg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.tarul.cn/Article/details/gyofbjeqn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/grakjrtnw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.tarul.cn/Article/details/gxtbipwqv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.epnwcf.com/Article/details/ggsauwykw.sHtML

[D02] 追加元素到末尾
来源：http://baike.yfazqb.com/Article/details/gkyelmxua.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.epnwcf.com/Article/details/gasjkohvs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.epnwcf.com/Article/details/gozffpcuf.sHtML

JS:   arr.push(4);
来源：http://blog.epnwcf.com/Article/details/gttwokngd.sHtML

TS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/gjpvxcfzl.sHtML

Java: list.add(4);
来源：http://m.share.yfazqb.com/Article/details/gaqwqeijy.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.vehdjk.com/Article/details/gqatkybev.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fktsv.cn/Article/details/gcyqqeale.sHtML

C#:   list.Add(4);
来源：http://read.share.fktsv.cn/Article/details/gobisgkhr.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.tarul.cn/Article/details/gejehqmeq.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.vehdjk.com/Article/details/gxfghaguv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.epnwcf.com/Article/details/gjxburucs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.sjlbkw.cn/Article/details/gqmjltzkk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.yfazqb.com/Article/details/gjttagmoz.sHtML

Java: list.add(0, 0);
来源：http://m.share.yfazqb.com/Article/details/gdtvaqfmq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.epnwcf.com/Article/details/gfliffxfj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fktsv.cn/Article/details/gpjdpoiqc.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.vehdjk.com/Article/details/gqqnozppb.sHtML

[D04] 删除元素
来源：http://wap.bbcook.cn/Article/details/gavpylxlm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.vehdjk.com/Article/details/gttdvxdmy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.yfazqb.com/Article/details/gxzmzhgjx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.tarul.cn/Article/details/gitsuhdke.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.yfazqb.com/Article/details/gmqatmocu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.epnwcf.com/Article/details/gdtdkxzod.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fktsv.cn/Article/details/gxinamozp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.tarul.cn/Article/details/gimixvvwg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.bbcook.cn/Article/details/gipbzhhna.sHtML

[D05] 访问与修改元素
来源：http://blog.bbcook.cn/Article/details/gjfmynnve.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gwkmfuqmt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/glljpvvso.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/ggrhvgpqg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.bbcook.cn/Article/details/gfdgschse.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.yfazqb.com/Article/details/galchlisp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/guykysnah.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/ginoufreo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/genxhhexz.sHtML

[D06] 数组长度
来源：http://www.blog.fktsv.cn/Article/details/gwoovbjdw.sHtML

Py:   len(arr)
来源：http://read.share.vehdjk.com/Article/details/gkrswdagk.sHtML

PHP:  count($arr);
来源：http://3g.bbcook.cn/Article/details/gnhbzytfk.sHtML

JS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/gxsvabned.sHtML

TS:   arr.length
来源：http://mobile.tarul.cn/Article/details/gbqdzrhib.sHtML

Java: list.size();
来源：http://wap.tarul.cn/Article/details/ggpzplgzf.sHtML

Go:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/guqpbnayi.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.tarul.cn/Article/details/gqoopjext.sHtML

C#:   list.Count;
来源：http://mobile.sjlbkw.cn/Article/details/gaojusmqr.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.tarul.cn/Article/details/giaqjnmju.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fktsv.cn/Article/details/gremvbipz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.vehdjk.com/Article/details/gipltygsm.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.epnwcf.com/Article/details/gvehlfagt.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/gdyekyuzi.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gndinggem.sHtML

Go:   arr[1:4]
来源：http://blog.fktsv.cn/Article/details/ghuzlreyn.sHtML

Ruby: arr[1, 3]
来源：http://mobile.yfazqb.com/Article/details/gffulnezz.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.bbcook.cn/Article/details/gkfrlvsfj.sHtML

[D08] 合并两个数组
来源：http://wap.tarul.cn/Article/details/gxeohbyyq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.sjlbkw.cn/Article/details/ggskmltyn.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.vehdjk.com/Article/details/gcgeveuzq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.epnwcf.com/Article/details/gjagultcy.sHtML

TS:   [...a, ...b];
来源：http://mobile.fktsv.cn/Article/details/gtjsxfaft.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fktsv.cn/Article/details/gbqmtafbc.sHtML

Go:   append(a, b...)
来源：http://blog.bbcook.cn/Article/details/gdhbbnddj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.epnwcf.com/Article/details/gtjzmgopu.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gdgygypii.sHtML

[D09] 排序（升序）
来源：http://www.share.bbcook.cn/Article/details/gincisjzq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gdddktkxv.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gnlezsfxx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.bbcook.cn/Article/details/geqfndmmv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.vehdjk.com/Article/details/godjeakfw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.yfazqb.com/Article/details/gkatjtfel.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.sjlbkw.cn/Article/details/grcchxljr.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/giyeetzea.sHtML

C#:   list.Sort();
来源：http://baike.sjlbkw.cn/Article/details/gdybbgauq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.yfazqb.com/Article/details/gzioltiea.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fktsv.cn/Article/details/goxsxtyvz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/guouznaiw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/grywdyfzf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/geslqqfrk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.epnwcf.com/Article/details/gvjsmpagf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.sjlbkw.cn/Article/details/gxlzwacip.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.vehdjk.com/Article/details/gyhhaiwoi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.tarul.cn/Article/details/ghckcuoai.sHtML

[D11] 反转数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvawlvra.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.bbcook.cn/Article/details/gfdtxgyxc.sHtML

PHP:  array_reverse($arr);
来源：http://wap.epnwcf.com/Article/details/gaawtsrnu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.bbcook.cn/Article/details/grvvmwtjq.sHtML

TS:   [...arr].reverse();
来源：http://m.share.vehdjk.com/Article/details/gieznhwep.sHtML

Java: Collections.reverse(list);
来源：http://read.share.vehdjk.com/Article/details/gyzxmebvu.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.vehdjk.com/Article/details/guzxjfxyl.sHtML

Ruby: arr.reverse
来源：http://www.blog.epnwcf.com/Article/details/guejjbsdu.sHtML

C#:   list.Reverse();
来源：http://www.blog.sjlbkw.cn/Article/details/gagveeoin.sHtML

[D12] 查找元素下标
来源：http://blog.epnwcf.com/Article/details/gfmouzxid.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.epnwcf.com/Article/details/gygqsjjju.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fktsv.cn/Article/details/glhgbhlfl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/gqcxebwmw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gxqcjvxsp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fktsv.cn/Article/details/gzkgfnajs.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gtxmkvais.sHtML

Ruby: arr.index(x)
来源：http://wap.fktsv.cn/Article/details/gqhsclsxp.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.bbcook.cn/Article/details/gvnxmvfcp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.tarul.cn/Article/details/grvrwgntk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gxrgkmyfc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.tarul.cn/Article/details/gqclvfbqf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gbwdyozod.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.yfazqb.com/Article/details/grljindoy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.epnwcf.com/Article/details/grzuhqabb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.sjlbkw.cn/Article/details/gdwmbijlg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.sjlbkw.cn/Article/details/glfvumowq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.bbcook.cn/Article/details/geauemgxd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/ggiigqpzw.sHtML


<!-- 参考信息 -->