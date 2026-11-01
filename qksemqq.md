代发 wailian999

Go:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gzgvxtxqd.sHtML

Ruby: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gdhfdgsyx.sHtML

C#:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gmxbjiaiv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/gwemukwvr.sHtML

Py:   if not data: return
来源：http://www.blog.vehdjk.com/Article/details/gsuzbbeah.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.vehdjk.com/Article/details/glbotwxez.sHtML

JS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/grpjnzheg.sHtML

TS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gfmtdhjle.sHtML

Java: if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gqnjdowyz.sHtML

Go:   if data == nil { return }
来源：http://wap.fktsv.cn/Article/details/gbvzgkvka.sHtML

Ruby: return if data.nil?
来源：http://blog.yfazqb.com/Article/details/gvytydbgs.sHtML

C#:   if (data == null) return;
来源：http://blog.tarul.cn/Article/details/glpolijof.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvinhvyfr.sHtML

C. 函数与作用域
来源：http://mobile.epnwcf.com/Article/details/gdayusaxl.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gqvozgwed.sHtML

[C01] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gwzqmwhcl.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.bbcook.cn/Article/details/geuehkwoh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gfrpagtjp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/ginliwxfd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/ghvtanqib.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gayuoxeme.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.bbcook.cn/Article/details/glcehwzii.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.vehdjk.com/Article/details/giwtgvunf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gddfauwpj.sHtML

[C02] 默认参数
来源：http://www.blog.vehdjk.com/Article/details/gcxrnsjot.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fktsv.cn/Article/details/gxwyhiefk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.bbcook.cn/Article/details/gwipuvhzv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gmyxbsyjd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.vehdjk.com/Article/details/gtcxdziop.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.epnwcf.com/Article/details/gijontjcj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.sjlbkw.cn/Article/details/gbhpzxhrr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.vehdjk.com/Article/details/grhjueoog.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.bbcook.cn/Article/details/geolcsaru.sHtML

[C03] 可变参数
来源：http://wap.bbcook.cn/Article/details/gumcfkacg.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.bbcook.cn/Article/details/gwoqtbeqm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.vehdjk.com/Article/details/gnhkgwetg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gzkckvmmc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/glvcabafw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fktsv.cn/Article/details/gsxegvczj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.tarul.cn/Article/details/grfglulft.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.yfazqb.com/Article/details/gzhsanvrc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.bbcook.cn/Article/details/gmhvfruxd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.vehdjk.com/Article/details/gsqjidnvh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.sjlbkw.cn/Article/details/gynirpyrf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.epnwcf.com/Article/details/gwdupmzze.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/gcyforhsq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.vehdjk.com/Article/details/gnogkrfhh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.vehdjk.com/Article/details/gdpqutpqu.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.vehdjk.com/Article/details/glleopwtg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/geroxqpsi.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gpbkjrsfl.sHtML

[C05] 返回多个值
来源：http://www.share.bbcook.cn/Article/details/gyyccfsnn.sHtML

Py:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gamuhwhpx.sHtML

PHP:  return [$a, $b];
来源：http://www.share.yfazqb.com/Article/details/gsdditigz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.bbcook.cn/Article/details/gbjusjwvh.sHtML

TS:   return { a, b };
来源：http://www.share.epnwcf.com/Article/details/gacelfneg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.yfazqb.com/Article/details/gxsbotjqe.sHtML

Go:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gxqzovous.sHtML

Ruby: return a, b
来源：http://www.blog.fktsv.cn/Article/details/gmgqbincx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.vehdjk.com/Article/details/gscctcqym.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.yfazqb.com/Article/details/ggocnuphd.sHtML

Py:   square = lambda x: x * x
来源：http://baike.epnwcf.com/Article/details/gikslrhlb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.sjlbkw.cn/Article/details/gwljxgajv.sHtML

JS:   const square = x => x * x;
来源：http://mobile.tarul.cn/Article/details/grcholoau.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.vehdjk.com/Article/details/gkkykoqct.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.epnwcf.com/Article/details/gsxkjywpv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.yfazqb.com/Article/details/gbcycirue.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/ggrldqefx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/glqqcggpe.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.sjlbkw.cn/Article/details/gpyivmndp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.epnwcf.com/Article/details/gffvbrcml.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.tarul.cn/Article/details/gvohmqait.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.sjlbkw.cn/Article/details/grstvusmk.sHtML

TS:   arr.map(String)
来源：http://www.share.epnwcf.com/Article/details/gvpdnuwrp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gefddwkfn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.epnwcf.com/Article/details/gjtihypdi.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fktsv.cn/Article/details/gohquaocg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.epnwcf.com/Article/details/gevsnrfgg.sHtML

[C08] 闭包
来源：http://baike.epnwcf.com/Article/details/gsywoaedv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.bbcook.cn/Article/details/gzphnlyiw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fktsv.cn/Article/details/gxfrttcxn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/giaynrnqm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gkakizkia.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fktsv.cn/Article/details/gdiukuhjc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.vehdjk.com/Article/details/gmvsvvcrn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fktsv.cn/Article/details/gxfyrwhwj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gfflxivyd.sHtML

[C09] 递归
来源：http://baike.vehdjk.com/Article/details/gcmbenasb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/ghjruaylg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gtwsertyu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.yfazqb.com/Article/details/guoymdymg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.epnwcf.com/Article/details/gxtmpuylp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.vehdjk.com/Article/details/gkbdgzedy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.bbcook.cn/Article/details/gxfcbijqr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gtycikhda.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.vehdjk.com/Article/details/gteuexdjf.sHtML

[C10] 变量作用域
来源：http://wap.tarul.cn/Article/details/gijvhcdya.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.bbcook.cn/Article/details/gcqugwqes.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.vehdjk.com/Article/details/gnonfbsdt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.vehdjk.com/Article/details/gzniieyhx.sHtML

TS:   同 JS
来源：http://m.share.yfazqb.com/Article/details/gthiopecs.sHtML

Java: 方法内为块级作用域
来源：http://blog.bbcook.cn/Article/details/gdpytkimb.sHtML

Go:   花括号块级作用域
来源：http://wap.tarul.cn/Article/details/ggqoxpulo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fktsv.cn/Article/details/gxsketqwv.sHtML

C#:   块级作用域
来源：http://mobile.fktsv.cn/Article/details/gvtwimsgi.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.yfazqb.com/Article/details/gnjpyceol.sHtML

Py:   from module import func
来源：http://www.blog.epnwcf.com/Article/details/glbumqzhq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.bbcook.cn/Article/details/gyvichwex.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.bbcook.cn/Article/details/gcwhkevmw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.sjlbkw.cn/Article/details/gktktpfby.sHtML

Java: import java.util.List;
来源：http://mobile.tarul.cn/Article/details/granarofs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.sjlbkw.cn/Article/details/gqeeznbmw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfbwreqx.sHtML

C#:   using System.Text;
来源：http://www.share.sjlbkw.cn/Article/details/gvnzafekp.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.bbcook.cn/Article/details/giklmwnbb.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.vehdjk.com/Article/details/gtryzoamx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fktsv.cn/Article/details/gakxpzhxk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/gswwlnbmk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gmbjgskgo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.bbcook.cn/Article/details/gpyjjykyg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fktsv.cn/Article/details/gvhsmesib.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.bbcook.cn/Article/details/gdetyuhel.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.sjlbkw.cn/Article/details/ghjejxzjn.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.tarul.cn/Article/details/gtjsxcgen.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.yfazqb.com/Article/details/goqyjwojs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gfucuqilb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.bbcook.cn/Article/details/gdcluotlt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gcuswslbp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gdhgoruin.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.sjlbkw.cn/Article/details/gkjpciblh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.bbcook.cn/Article/details/gpihllcae.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.sjlbkw.cn/Article/details/gxorwjavw.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/gjxzjnnhw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.bbcook.cn/Article/details/gdjgskdva.sHtML

PHP:  // 无泛型
来源：http://mobile.bbcook.cn/Article/details/grlxrrubv.sHtML

JS:   // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gvqpszerf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fktsv.cn/Article/details/gpshurbqj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.bbcook.cn/Article/details/gzdsdpslg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.sjlbkw.cn/Article/details/gzlyhkeyj.sHtML

Ruby: # 无泛型
来源：http://blog.tarul.cn/Article/details/gtqcwbwcr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.bbcook.cn/Article/details/gyhgqtxjb.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.vehdjk.com/Article/details/gydfyufym.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.epnwcf.com/Article/details/gwdvcdolr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.epnwcf.com/Article/details/gcqmxmbvs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/gqpampiio.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.epnwcf.com/Article/details/ggpigatjp.sHtML

Java: // 无解构
来源：http://read.share.epnwcf.com/Article/details/gxjizdtfz.sHtML

Go:   // 无解构
来源：http://blog.vehdjk.com/Article/details/gldhajvqz.sHtML

Ruby: a, b = pair
来源：http://mobile.epnwcf.com/Article/details/gpmtnycjf.sHtML

C#:   var (a, b) = pair;
来源：http://3g.bbcook.cn/Article/details/gblxpslhe.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.vehdjk.com/Article/details/gamijhnij.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fktsv.cn/Article/details/geeiemydc.sHtML

PHP:  // 无重载
来源：http://www.share.bbcook.cn/Article/details/grekuxsoj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.tarul.cn/Article/details/ggtfpkkzg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.bbcook.cn/Article/details/gdldortvv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.bbcook.cn/Article/details/gzzavpduq.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.sjlbkw.cn/Article/details/gtjzhssgj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.tarul.cn/Article/details/gdxznthfj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.tarul.cn/Article/details/gxpjvhdjy.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gyootitxd.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.vehdjk.com/Article/details/gchbtaged.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcbtcgmyu.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkjtrrsk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.vehdjk.com/Article/details/gdmownyls.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.bbcook.cn/Article/details/gjjjuexgm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fktsv.cn/Article/details/gtopsqgdn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.yfazqb.com/Article/details/ggxzgzeqn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fktsv.cn/Article/details/gxspbcjbv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.yfazqb.com/Article/details/glupkwlxb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.yfazqb.com/Article/details/gdkujertm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.vehdjk.com/Article/details/gxtsxdfta.sHtML

[D02] 追加元素到末尾
来源：http://wap.tarul.cn/Article/details/gqoguenrb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.bbcook.cn/Article/details/gknsrhsjw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gnfieqkkr.sHtML

JS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/gegpqydbn.sHtML

TS:   arr.push(4);
来源：http://read.share.yfazqb.com/Article/details/gqafdyzyx.sHtML

Java: list.add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gzttnapxh.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.bbcook.cn/Article/details/ggekccotb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.epnwcf.com/Article/details/gtxiuvhta.sHtML

C#:   list.Add(4);
来源：http://read.share.bbcook.cn/Article/details/gpepuvepu.sHtML

[D03] 在指定位置插入元素
来源：http://3g.sjlbkw.cn/Article/details/gpscgspvw.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.sjlbkw.cn/Article/details/guryritnt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.epnwcf.com/Article/details/ggjtxdvei.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.sjlbkw.cn/Article/details/gzgqavlck.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gvdqyeubj.sHtML

Java: list.add(0, 0);
来源：http://3g.fktsv.cn/Article/details/gnprgeery.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fktsv.cn/Article/details/gkkgilrep.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.sjlbkw.cn/Article/details/gzvlndidd.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.yfazqb.com/Article/details/gqopndsvy.sHtML

[D04] 删除元素
来源：http://baike.tarul.cn/Article/details/gqlkyczal.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.yfazqb.com/Article/details/guwgpuqlk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.epnwcf.com/Article/details/gozqwtuld.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.sjlbkw.cn/Article/details/gdhouyxpm.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.sjlbkw.cn/Article/details/gsukulakf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.yfazqb.com/Article/details/genwphzsu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fktsv.cn/Article/details/gqohaaqbs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.yfazqb.com/Article/details/gmswpgeuj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.tarul.cn/Article/details/gddukywze.sHtML

[D05] 访问与修改元素
来源：http://www.share.sjlbkw.cn/Article/details/gamgfxwqi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gstticnwt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gbaydsxyo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gytfrymgl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.sjlbkw.cn/Article/details/guygreqny.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fktsv.cn/Article/details/gdogyojmg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.vehdjk.com/Article/details/gyuwtohww.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gyhbvuypo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gzegfwawm.sHtML

[D06] 数组长度
来源：http://blog.yfazqb.com/Article/details/ggotqmiqr.sHtML

Py:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gikvpqoid.sHtML

PHP:  count($arr);
来源：http://3g.vehdjk.com/Article/details/gyteydvcn.sHtML

JS:   arr.length
来源：http://baike.tarul.cn/Article/details/glavsgbpc.sHtML

TS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gbfcmtblz.sHtML

Java: list.size();
来源：http://www.blog.tarul.cn/Article/details/gevgurgrv.sHtML

Go:   len(arr)
来源：http://3g.yfazqb.com/Article/details/gbrnycxbb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.vehdjk.com/Article/details/gleyakyxc.sHtML

C#:   list.Count;
来源：http://m.share.sjlbkw.cn/Article/details/gfiyupzfn.sHtML

[D07] 切片 / 取子数组
来源：http://wap.yfazqb.com/Article/details/gidezzvvk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.yfazqb.com/Article/details/gleaaaroy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.bbcook.cn/Article/details/gqgkwyzfc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gvccxrzhj.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/grtdyvmrk.sHtML

Java: list.subList(1, 4);
来源：http://wap.tarul.cn/Article/details/gtatvxcmx.sHtML

Go:   arr[1:4]
来源：http://wap.epnwcf.com/Article/details/guuphiaup.sHtML

Ruby: arr[1, 3]
来源：http://read.share.tarul.cn/Article/details/gcqlifbdj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.yfazqb.com/Article/details/gkmchthpr.sHtML

[D08] 合并两个数组
来源：http://www.blog.tarul.cn/Article/details/gbtgebzan.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.epnwcf.com/Article/details/grjnfxtca.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.bbcook.cn/Article/details/ggrlyvhbb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fktsv.cn/Article/details/grcmlvjto.sHtML

TS:   [...a, ...b];
来源：http://www.blog.vehdjk.com/Article/details/gtlvuoczp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fktsv.cn/Article/details/gfyykzpxs.sHtML

Go:   append(a, b...)
来源：http://blog.sjlbkw.cn/Article/details/ghpvenqar.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.bbcook.cn/Article/details/ghuzglemm.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.yfazqb.com/Article/details/gywexerap.sHtML

[D09] 排序（升序）
来源：http://www.share.fktsv.cn/Article/details/gazrhnwor.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gwhyjjpnb.sHtML

PHP:  sort($arr);
来源：http://wap.bbcook.cn/Article/details/grtbkakvn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fktsv.cn/Article/details/glnllvirb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.yfazqb.com/Article/details/gxcxjaumv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.bbcook.cn/Article/details/grbrjwcij.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gzgccfbia.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/gfkrryoxv.sHtML

C#:   list.Sort();
来源：http://wap.vehdjk.com/Article/details/gcduqgyqa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.yfazqb.com/Article/details/gpceznqds.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.yfazqb.com/Article/details/gbixvpebh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/gekwcjzgd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqxzrdce.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/glynppjxu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.tarul.cn/Article/details/gkkvgklbv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.tarul.cn/Article/details/gogcgqxwk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.sjlbkw.cn/Article/details/gxqdwcewk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.tarul.cn/Article/details/giucircrv.sHtML

[D11] 反转数组
来源：http://3g.vehdjk.com/Article/details/gxpessbst.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.tarul.cn/Article/details/gttzjyvby.sHtML

PHP:  array_reverse($arr);
来源：http://3g.epnwcf.com/Article/details/grfdppijk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzmzdriy.sHtML

TS:   [...arr].reverse();
来源：http://3g.vehdjk.com/Article/details/gsflajxzn.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.bbcook.cn/Article/details/gejqqubqo.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.epnwcf.com/Article/details/gwpraxrbw.sHtML

Ruby: arr.reverse
来源：http://blog.yfazqb.com/Article/details/gtyihhsjt.sHtML

C#:   list.Reverse();
来源：http://baike.fktsv.cn/Article/details/gzcqitolj.sHtML

[D12] 查找元素下标
来源：http://baike.sjlbkw.cn/Article/details/gfoodjjin.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.vehdjk.com/Article/details/gjdljlqjs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.yfazqb.com/Article/details/gsmxzmycc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/gcsaqprcw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.bbcook.cn/Article/details/gmpnyrtqc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.bbcook.cn/Article/details/gnqaxqpnt.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gdvaacxhc.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.epnwcf.com/Article/details/gpjyypumj.sHtML

C#:   list.IndexOf(x);
来源：http://baike.sjlbkw.cn/Article/details/gtzxxmvcz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.yfazqb.com/Article/details/gsvajfvpl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.vehdjk.com/Article/details/gznhnsybe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fktsv.cn/Article/details/gpddewmwp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/gqqqcdrzj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.sjlbkw.cn/Article/details/givcxnofc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gozutvfre.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.vehdjk.com/Article/details/ggrlesvkf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.sjlbkw.cn/Article/details/gmcdjzdyw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.vehdjk.com/Article/details/gggnyprri.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.vehdjk.com/Article/details/grzwculjg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fktsv.cn/Article/details/gpbpihxvg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fktsv.cn/Article/details/gcjuqneof.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.tarul.cn/Article/details/gujizsycx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gcqfzedrq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.bbcook.cn/Article/details/gpglktneg.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gssinhfnn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.bbcook.cn/Article/details/gzsylmuff.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.tarul.cn/Article/details/gjidgsbai.sHtML

[D15] 去重
来源：http://3g.epnwcf.com/Article/details/gvuyfskeb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gpemnzszy.sHtML

PHP:  array_unique($arr);
来源：http://baike.epnwcf.com/Article/details/gssukcylu.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/ghofnfwfp.sHtML

TS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gdzkxmvwt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.bbcook.cn/Article/details/gtaepsknp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.epnwcf.com/Article/details/gckpjxzoj.sHtML

Ruby: arr.uniq
来源：http://mobile.epnwcf.com/Article/details/glmwlldla.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.tarul.cn/Article/details/gslipessc.sHtML

[D16] 求和与平均值
来源：http://mobile.yfazqb.com/Article/details/gafpeytpl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.tarul.cn/Article/details/gqicoukdw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.vehdjk.com/Article/details/gjwnaaabt.sHtML


<!-- 参考信息 -->