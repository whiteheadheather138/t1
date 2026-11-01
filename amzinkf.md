代发 wailian999

C#:   x is int or double or decimal
来源：http://mobile.bbcook.cn/Article/details/gxlqyjjkp.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fktsv.cn/Article/details/gvsrwgewm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.yfazqb.com/Article/details/gwhwksxmx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.yfazqb.com/Article/details/grdtghhcm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/guokixesx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.tarul.cn/Article/details/gclpkkcua.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.epnwcf.com/Article/details/gwkvhmfvb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.tarul.cn/Article/details/glynxtrkc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.sjlbkw.cn/Article/details/gygicqoqf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.bbcook.cn/Article/details/glsymbdkr.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fktsv.cn/Article/details/grtfovxlw.sHtML

Py:   a and b or not c
来源：http://blog.yfazqb.com/Article/details/gbpvjqhnp.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.bbcook.cn/Article/details/gthyjeozf.sHtML

JS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gopcevdwn.sHtML

TS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gkjzjkwhc.sHtML

Java: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gwbriozrp.sHtML

Go:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/giqaelqto.sHtML

Ruby: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/glxbwisrb.sHtML

C#:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gzvdsomkk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fktsv.cn/Article/details/ghhtfqvrb.sHtML

Py:   if not data: return
来源：http://wap.tarul.cn/Article/details/gmobtqdti.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.vehdjk.com/Article/details/gsvvfwbyr.sHtML

JS:   if (!data) return;
来源：http://mobile.epnwcf.com/Article/details/gbqxqjvwb.sHtML

TS:   if (!data) return;
来源：http://www.blog.tarul.cn/Article/details/gbihecnzu.sHtML

Java: if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/grekezqtw.sHtML

Go:   if data == nil { return }
来源：http://read.share.fktsv.cn/Article/details/gfipvtghu.sHtML

Ruby: return if data.nil?
来源：http://wap.vehdjk.com/Article/details/gjpffqtln.sHtML

C#:   if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gpaotufyw.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gkuxdkrwn.sHtML

C. 函数与作用域
来源：http://blog.sjlbkw.cn/Article/details/gmzbkddqn.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gofxfxlsw.sHtML

[C01] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/gdnamyfqp.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.epnwcf.com/Article/details/gclcoglep.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/ghpoudzyx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gmyusbbed.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gcupnpywq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/ghmftjsxw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.bbcook.cn/Article/details/gsmnlcoco.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.tarul.cn/Article/details/gnhaxevkh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gqnhrvade.sHtML

[C02] 默认参数
来源：http://www.share.vehdjk.com/Article/details/gweyoewsx.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fktsv.cn/Article/details/gkdzgigzj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fktsv.cn/Article/details/gvnqqvopa.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gvtuekxiy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/grdqahryt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.bbcook.cn/Article/details/ghofclaxz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.tarul.cn/Article/details/gfcdkkjjm.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.vehdjk.com/Article/details/gjnyoelpi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.epnwcf.com/Article/details/ggoluhdcg.sHtML

[C03] 可变参数
来源：http://www.share.bbcook.cn/Article/details/gsvzxyzrc.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.epnwcf.com/Article/details/gbjltuiiv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fktsv.cn/Article/details/gmxntwgqw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.vehdjk.com/Article/details/gqjvusawe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjqkydgw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.yfazqb.com/Article/details/gkbcnefxs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.tarul.cn/Article/details/gqxdcrmpj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.bbcook.cn/Article/details/gebfviibt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.vehdjk.com/Article/details/gpauybrnl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.sjlbkw.cn/Article/details/gssiceysf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.vehdjk.com/Article/details/gsaccwnbl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fktsv.cn/Article/details/grpxmzflq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/gznxpdkrp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.tarul.cn/Article/details/gkbwwmnnr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fktsv.cn/Article/details/glljzbdia.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fktsv.cn/Article/details/gmdmznnyg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gdcwfmpdt.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/guqxyogdz.sHtML

[C05] 返回多个值
来源：http://www.share.bbcook.cn/Article/details/gwwfohwgf.sHtML

Py:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/gcaceknnt.sHtML

PHP:  return [$a, $b];
来源：http://www.share.tarul.cn/Article/details/gvdzqmcxh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.epnwcf.com/Article/details/gglaucwqk.sHtML

TS:   return { a, b };
来源：http://mobile.bbcook.cn/Article/details/gpaciqqkp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.tarul.cn/Article/details/ghvsvqqaf.sHtML

Go:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gzebawjuw.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gzzixodcl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.yfazqb.com/Article/details/gugdtvzuf.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.vehdjk.com/Article/details/gswxmprzm.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.vehdjk.com/Article/details/gkagewktm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.bbcook.cn/Article/details/gnhrkgcbn.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gigogwsab.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.epnwcf.com/Article/details/gazuhptwk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.tarul.cn/Article/details/gauojdoqj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.vehdjk.com/Article/details/gtxwfqvtr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fktsv.cn/Article/details/gskkmcxki.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.bbcook.cn/Article/details/gccebfodz.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.sjlbkw.cn/Article/details/ggjnbykvw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.sjlbkw.cn/Article/details/gotagfqhy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fktsv.cn/Article/details/ggjncufxt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.sjlbkw.cn/Article/details/grsahqqha.sHtML

TS:   arr.map(String)
来源：http://www.share.bbcook.cn/Article/details/glrllsyqt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.epnwcf.com/Article/details/glpswjzkw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.sjlbkw.cn/Article/details/goofnyfjo.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.yfazqb.com/Article/details/gvxwffboe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.yfazqb.com/Article/details/guvimwiqt.sHtML

[C08] 闭包
来源：http://read.share.bbcook.cn/Article/details/gcvmzmwun.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.bbcook.cn/Article/details/gvgdvtnwd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.epnwcf.com/Article/details/gvnzminju.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gczdtvpjs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/geoynvijf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fktsv.cn/Article/details/gwqaoojsp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.bbcook.cn/Article/details/gpmdpzwtq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.epnwcf.com/Article/details/ggyeehuzc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gvwnuhcpz.sHtML

[C09] 递归
来源：http://3g.tarul.cn/Article/details/gosmsrkvu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/gewutqlck.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.vehdjk.com/Article/details/grckyqifj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gtudrplej.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.bbcook.cn/Article/details/gxclxgmen.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.vehdjk.com/Article/details/gfstrrrgl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.sjlbkw.cn/Article/details/ghpiligmv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gpbgqzbji.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fktsv.cn/Article/details/glegyubad.sHtML

[C10] 变量作用域
来源：http://m.share.fktsv.cn/Article/details/gptootfir.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.bbcook.cn/Article/details/ghrfmscok.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.bbcook.cn/Article/details/gkrkalpac.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.vehdjk.com/Article/details/gvktpllfi.sHtML

TS:   同 JS
来源：http://mobile.bbcook.cn/Article/details/gwoyhwfbt.sHtML

Java: 方法内为块级作用域
来源：http://blog.yfazqb.com/Article/details/guwjjvlww.sHtML

Go:   花括号块级作用域
来源：http://wap.yfazqb.com/Article/details/gpfbgtejl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fktsv.cn/Article/details/gxhnflest.sHtML

C#:   块级作用域
来源：http://3g.bbcook.cn/Article/details/grsqjvpba.sHtML

[C11] 模块导入与导出
来源：http://wap.tarul.cn/Article/details/grlxigeja.sHtML

Py:   from module import func
来源：http://read.share.bbcook.cn/Article/details/glbhpzmcv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.epnwcf.com/Article/details/gyjbyadvb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.epnwcf.com/Article/details/gyewsnyxk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.yfazqb.com/Article/details/glrtyxkqq.sHtML

Java: import java.util.List;
来源：http://3g.tarul.cn/Article/details/gktiahhry.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.bbcook.cn/Article/details/ggviwqphw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.vehdjk.com/Article/details/gmfkxvovf.sHtML

C#:   using System.Text;
来源：http://www.m.share.epnwcf.com/Article/details/gsbqpqibf.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.bbcook.cn/Article/details/gewpndlnt.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.yfazqb.com/Article/details/ggtdmmqzb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.vehdjk.com/Article/details/goouhbxou.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.sjlbkw.cn/Article/details/gfsnbcrzs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/gmmdokqlt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.epnwcf.com/Article/details/gitrblsie.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.epnwcf.com/Article/details/giwxebdgz.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.tarul.cn/Article/details/gfrefsmff.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.yfazqb.com/Article/details/giglhoiir.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fktsv.cn/Article/details/gnuktevyl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.sjlbkw.cn/Article/details/gzhastphv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/ggolknmhd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.vehdjk.com/Article/details/gwqmpcnte.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/glnykflro.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gscgoamro.sHtML

Go:   func add(a, b int) int
来源：http://baike.bbcook.cn/Article/details/gdtqocfsa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.tarul.cn/Article/details/givahwecg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.epnwcf.com/Article/details/grphfnqyz.sHtML

[C14] 泛型函数
来源：http://www.blog.epnwcf.com/Article/details/gqhsbkquo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.yfazqb.com/Article/details/ggwfqzssl.sHtML

PHP:  // 无泛型
来源：http://www.share.tarul.cn/Article/details/gumplmpfm.sHtML

JS:   // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gdamfgkkz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.epnwcf.com/Article/details/gezfvngpg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.vehdjk.com/Article/details/geqgnafwv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fktsv.cn/Article/details/ghflrjefb.sHtML

Ruby: # 无泛型
来源：http://3g.epnwcf.com/Article/details/ggizbsfed.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.vehdjk.com/Article/details/gvlumenzl.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fktsv.cn/Article/details/gtwqtiuds.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fktsv.cn/Article/details/gctkfgypm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.vehdjk.com/Article/details/grealgett.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fktsv.cn/Article/details/gebekaxyi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.yfazqb.com/Article/details/goqmqgdzm.sHtML

Java: // 无解构
来源：http://wap.vehdjk.com/Article/details/gbztlajbj.sHtML

Go:   // 无解构
来源：http://3g.bbcook.cn/Article/details/gskafpfhn.sHtML

Ruby: a, b = pair
来源：http://www.share.yfazqb.com/Article/details/gqygjgkcl.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/grrmooxev.sHtML

[C16] 函数 / 方法重载
来源：http://baike.yfazqb.com/Article/details/ggwwoahbf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.bbcook.cn/Article/details/ggulqqkfp.sHtML

PHP:  // 无重载
来源：http://3g.vehdjk.com/Article/details/ggxgguizi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.sjlbkw.cn/Article/details/gvlgdpoxg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.tarul.cn/Article/details/gazeztvav.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gavlmfixe.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.bbcook.cn/Article/details/gjrqoeadq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.sjlbkw.cn/Article/details/gxtiochlz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.epnwcf.com/Article/details/grmujdyif.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/goahtjfts.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.bbcook.cn/Article/details/gmvzavcew.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gngjpvrsu.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.yfazqb.com/Article/details/gfzdykert.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.sjlbkw.cn/Article/details/gkosuxxdc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.vehdjk.com/Article/details/gjoniqvvt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fktsv.cn/Article/details/gqxdaasdp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.tarul.cn/Article/details/gaxkxvjct.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.vehdjk.com/Article/details/glyazpmhg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.tarul.cn/Article/details/gakyakdjc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.bbcook.cn/Article/details/gtzsnbkxu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.tarul.cn/Article/details/grdjufcfu.sHtML

[D02] 追加元素到末尾
来源：http://mobile.vehdjk.com/Article/details/ggteqvbbm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.bbcook.cn/Article/details/gywblccdu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.epnwcf.com/Article/details/gjofredjj.sHtML

JS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/gjibvkueb.sHtML

TS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gnfncqbwq.sHtML

Java: list.add(4);
来源：http://baike.yfazqb.com/Article/details/gpmlxfqjh.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fktsv.cn/Article/details/gsryarres.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.sjlbkw.cn/Article/details/geztkqsat.sHtML

C#:   list.Add(4);
来源：http://3g.vehdjk.com/Article/details/gwniajvtl.sHtML

[D03] 在指定位置插入元素
来源：http://baike.tarul.cn/Article/details/gbrclplij.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.sjlbkw.cn/Article/details/gexrgkhep.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.bbcook.cn/Article/details/gjtcentgr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.yfazqb.com/Article/details/gojtaigfy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.vehdjk.com/Article/details/gsmepapmd.sHtML

Java: list.add(0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gwhjzaxxc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.epnwcf.com/Article/details/gggouxowc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.vehdjk.com/Article/details/grxxlmzys.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/gnnxxuxqa.sHtML

[D04] 删除元素
来源：http://read.share.bbcook.cn/Article/details/gqrtgqvgy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.bbcook.cn/Article/details/gcpyhnsie.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.tarul.cn/Article/details/gubexqmkf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fktsv.cn/Article/details/guaxjagsq.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.bbcook.cn/Article/details/gdnuuwwzh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.sjlbkw.cn/Article/details/gulgieazp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.bbcook.cn/Article/details/gcswmtwwv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.epnwcf.com/Article/details/gbcyrtazu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.sjlbkw.cn/Article/details/grbjivhih.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.vehdjk.com/Article/details/gtaevpjsz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gfqxrytsx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gikynxueu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvowmzgv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.tarul.cn/Article/details/gozviaqcg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.yfazqb.com/Article/details/gvmutuihc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/grwemxray.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gbwbuqeyl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.tarul.cn/Article/details/gqihxhrve.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/giwojsnsa.sHtML

Py:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gpklpstoc.sHtML

PHP:  count($arr);
来源：http://m.share.yfazqb.com/Article/details/glwahntxk.sHtML

JS:   arr.length
来源：http://read.share.bbcook.cn/Article/details/gnttsjkjm.sHtML

TS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/ghbsytcwp.sHtML

Java: list.size();
来源：http://mobile.bbcook.cn/Article/details/gqgretsuh.sHtML

Go:   len(arr)
来源：http://mobile.tarul.cn/Article/details/gpvixdzmz.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.vehdjk.com/Article/details/ggrbzqaqp.sHtML

C#:   list.Count;
来源：http://baike.tarul.cn/Article/details/gnglvsjnb.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtmyomwy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.yfazqb.com/Article/details/gpjqejslv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.epnwcf.com/Article/details/gikdlsfbu.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.bbcook.cn/Article/details/giyjocavg.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.bbcook.cn/Article/details/gkkojdypd.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/gzlazibnz.sHtML

Go:   arr[1:4]
来源：http://wap.yfazqb.com/Article/details/gqxxsdzsz.sHtML

Ruby: arr[1, 3]
来源：http://blog.tarul.cn/Article/details/gfmxadbro.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.vehdjk.com/Article/details/ggaycqvea.sHtML

[D08] 合并两个数组
来源：http://www.blog.epnwcf.com/Article/details/gdwgcvdht.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fktsv.cn/Article/details/giboqpfrj.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.tarul.cn/Article/details/gliustvhk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.epnwcf.com/Article/details/gnopedicu.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.vehdjk.com/Article/details/gtplioxzv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.epnwcf.com/Article/details/gsosrugyk.sHtML

Go:   append(a, b...)
来源：http://3g.fktsv.cn/Article/details/gsrpamosb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.yfazqb.com/Article/details/gcqljkrjt.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.epnwcf.com/Article/details/gdauujchu.sHtML

[D09] 排序（升序）
来源：http://blog.vehdjk.com/Article/details/glcnmqikw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gwrzsftzj.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gfgfgqpcs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.yfazqb.com/Article/details/gzoovweah.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.vehdjk.com/Article/details/gvztsettz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.sjlbkw.cn/Article/details/gtssduzph.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gcvoejfvu.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gkkxwwbgm.sHtML

C#:   list.Sort();
来源：http://blog.fktsv.cn/Article/details/gxvfubfhv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.sjlbkw.cn/Article/details/gpcaqhcbe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.epnwcf.com/Article/details/gidysxhgr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.yfazqb.com/Article/details/gjejyuzhe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fktsv.cn/Article/details/gdqbfmabw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gyytofwmh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.bbcook.cn/Article/details/gjsagtlvy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.vehdjk.com/Article/details/gdenaipkz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.epnwcf.com/Article/details/gahynlgxu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.tarul.cn/Article/details/gynetxvsw.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/gbgygmfqf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.epnwcf.com/Article/details/genlwrvdl.sHtML

PHP:  array_reverse($arr);
来源：http://3g.epnwcf.com/Article/details/gizstrild.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.yfazqb.com/Article/details/gejblkfgv.sHtML

TS:   [...arr].reverse();
来源：http://baike.vehdjk.com/Article/details/gzzedsvgw.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/gfubvyryd.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.yfazqb.com/Article/details/gjqpygfyg.sHtML

Ruby: arr.reverse
来源：http://read.share.yfazqb.com/Article/details/gbbyeivxy.sHtML

C#:   list.Reverse();
来源：http://m.share.fktsv.cn/Article/details/grvmhvazp.sHtML

[D12] 查找元素下标
来源：http://blog.sjlbkw.cn/Article/details/gtsvqgdij.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.tarul.cn/Article/details/gwpvksssw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fktsv.cn/Article/details/gbqspwzgl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/gsjjuiezc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.epnwcf.com/Article/details/gvtrrpwpm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.vehdjk.com/Article/details/gzboxehow.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gzpyaafal.sHtML

Ruby: arr.index(x)
来源：http://wap.epnwcf.com/Article/details/gyixqqshe.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.yfazqb.com/Article/details/gaeiiabhk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.epnwcf.com/Article/details/ghfyrjkfh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.epnwcf.com/Article/details/gdogltpmm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fktsv.cn/Article/details/gtpvhlfjr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gnnknxyqq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gmbvvmerb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.yfazqb.com/Article/details/gadbzkezu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.tarul.cn/Article/details/gkdandwae.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.vehdjk.com/Article/details/gheqfnuuz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fktsv.cn/Article/details/gpyvstqzy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.bbcook.cn/Article/details/ghzdjnniz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.yfazqb.com/Article/details/glxpfybgp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.yfazqb.com/Article/details/glypyvqsq.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gfvdfatnl.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fktsv.cn/Article/details/gjuqguktb.sHtML


<!-- 参考信息 -->