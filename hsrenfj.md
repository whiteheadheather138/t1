代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.vehdjk.com/Article/details/gqqbjfibv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fktsv.cn/Article/details/ggfbxklcu.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.yfazqb.com/Article/details/gutiuyyyk.sHtML

Py:   a and b or not c
来源：http://wap.vehdjk.com/Article/details/gvgawfsoc.sHtML

PHP:  $a && $b || !$c
来源：http://baike.vehdjk.com/Article/details/glfwagexp.sHtML

JS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gfhqwwpba.sHtML

TS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gwypjgljb.sHtML

Java: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gthglgsag.sHtML

Go:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gijnhkwca.sHtML

Ruby: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/grjgccohf.sHtML

C#:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gcgwmruhf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fktsv.cn/Article/details/ggiilhdkc.sHtML

Py:   if not data: return
来源：http://read.share.vehdjk.com/Article/details/gssmtjlle.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.sjlbkw.cn/Article/details/grmuuytem.sHtML

JS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gfpmpioln.sHtML

TS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gmqnnnppc.sHtML

Java: if (data == null) return;
来源：http://www.share.tarul.cn/Article/details/guwedfokc.sHtML

Go:   if data == nil { return }
来源：http://read.share.vehdjk.com/Article/details/gaxwylhfq.sHtML

Ruby: return if data.nil?
来源：http://baike.fktsv.cn/Article/details/gdcrypkog.sHtML

C#:   if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/gaublgcfj.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ghfifaoii.sHtML

C. 函数与作用域
来源：http://blog.tarul.cn/Article/details/gaijskehr.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gciqpqiys.sHtML

[C01] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/gzgodxeah.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/ghavdpltf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/geszhmqlr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gbyljtvze.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gjhnojdoo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gjundrkeg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.sjlbkw.cn/Article/details/gqtvzdrjx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fktsv.cn/Article/details/ggxhljtvn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/grvxyfutb.sHtML

[C02] 默认参数
来源：http://3g.tarul.cn/Article/details/gdtgiutdm.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.tarul.cn/Article/details/gwwxdottw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.epnwcf.com/Article/details/gtqibnndg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gzfculqar.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/guzcplcnb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.bbcook.cn/Article/details/gryqsddie.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.vehdjk.com/Article/details/gwoojwyos.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.epnwcf.com/Article/details/gmbgnaotz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.vehdjk.com/Article/details/gzxknoicd.sHtML

[C03] 可变参数
来源：http://blog.fktsv.cn/Article/details/glcunkxjv.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.yfazqb.com/Article/details/gpzzxonxr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.vehdjk.com/Article/details/ghpnqldoi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/geeobamul.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/giiarukrk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.epnwcf.com/Article/details/gddvvssxr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.epnwcf.com/Article/details/gcyqjdkid.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.tarul.cn/Article/details/gddkugbvw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.vehdjk.com/Article/details/ggjeqbswh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.yfazqb.com/Article/details/gjdoqxkrp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.tarul.cn/Article/details/gfmdwdmxt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.tarul.cn/Article/details/gfayvwafp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/ghdqbvmsn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.bbcook.cn/Article/details/goqhgccoj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.tarul.cn/Article/details/gewqnvdkj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.bbcook.cn/Article/details/gjkzkvjno.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gcnjmsvhn.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/gkibmgcem.sHtML

[C05] 返回多个值
来源：http://m.share.bbcook.cn/Article/details/gzsseyeda.sHtML

Py:   return a, b
来源：http://wap.yfazqb.com/Article/details/gteylquum.sHtML

PHP:  return [$a, $b];
来源：http://blog.vehdjk.com/Article/details/gyvmjhhnu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gkufikerk.sHtML

TS:   return { a, b };
来源：http://www.blog.tarul.cn/Article/details/ghpzhkidw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.yfazqb.com/Article/details/ghworitks.sHtML

Go:   return a, b
来源：http://mobile.tarul.cn/Article/details/giuqryedp.sHtML

Ruby: return a, b
来源：http://wap.yfazqb.com/Article/details/guhjlzsrk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fktsv.cn/Article/details/gzufbkowh.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.epnwcf.com/Article/details/guovhxtzx.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fktsv.cn/Article/details/gnvjqtbec.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.epnwcf.com/Article/details/gxepmuezl.sHtML

JS:   const square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gtlzsukgq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/giceqziah.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gytqtgkbn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.yfazqb.com/Article/details/gzgsjufao.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.vehdjk.com/Article/details/giaophrgh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fktsv.cn/Article/details/gmcjeiijl.sHtML

[C07] 把函数作为参数传入
来源：http://3g.bbcook.cn/Article/details/gsxykjsnc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fktsv.cn/Article/details/giaxoiarx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gabrfnxch.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fktsv.cn/Article/details/gggeitmfs.sHtML

TS:   arr.map(String)
来源：http://www.blog.tarul.cn/Article/details/gskuyubbd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.bbcook.cn/Article/details/ggutdzxvd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.bbcook.cn/Article/details/gzfaylfzo.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fktsv.cn/Article/details/gyferihvl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.yfazqb.com/Article/details/grgnmjduu.sHtML

[C08] 闭包
来源：http://baike.tarul.cn/Article/details/gzahjytgl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.epnwcf.com/Article/details/gjjplhbai.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.bbcook.cn/Article/details/gijahoyas.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gcxotppaq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/ghfdrkumo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.tarul.cn/Article/details/gcmjnxemz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.epnwcf.com/Article/details/gclazchan.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.tarul.cn/Article/details/gzahxpetl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gxtlxgogr.sHtML

[C09] 递归
来源：http://www.share.yfazqb.com/Article/details/gehdqpiqh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gudjcatgs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fktsv.cn/Article/details/gfzmresxd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gubkundcv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.epnwcf.com/Article/details/goigvnuns.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.yfazqb.com/Article/details/gahoswbzd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.epnwcf.com/Article/details/grjyfistu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gmluxvndq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.bbcook.cn/Article/details/gcvjkfwwp.sHtML

[C10] 变量作用域
来源：http://baike.yfazqb.com/Article/details/gdmuskpbx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.tarul.cn/Article/details/gnjapwwke.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.yfazqb.com/Article/details/gofcpsniq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fktsv.cn/Article/details/golydhiuf.sHtML

TS:   同 JS
来源：http://mobile.fktsv.cn/Article/details/gelyuxsfu.sHtML

Java: 方法内为块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gnclnkyob.sHtML

Go:   花括号块级作用域
来源：http://read.share.fktsv.cn/Article/details/gwrlejafg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.yfazqb.com/Article/details/gjbxtslxe.sHtML

C#:   块级作用域
来源：http://read.share.fktsv.cn/Article/details/ggfksvqpp.sHtML

[C11] 模块导入与导出
来源：http://www.blog.tarul.cn/Article/details/gusoqrfly.sHtML

Py:   from module import func
来源：http://www.share.bbcook.cn/Article/details/gfvhzzefg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.vehdjk.com/Article/details/ghkdyvpym.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.bbcook.cn/Article/details/gzpzuikkd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.tarul.cn/Article/details/gqvymdgxi.sHtML

Java: import java.util.List;
来源：http://www.blog.tarul.cn/Article/details/gyticvxie.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.bbcook.cn/Article/details/gtwbsmufi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.bbcook.cn/Article/details/gvsorpciu.sHtML

C#:   using System.Text;
来源：http://blog.yfazqb.com/Article/details/gqehdudqc.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.sjlbkw.cn/Article/details/gpxdseqdi.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.tarul.cn/Article/details/gipuniwkv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fktsv.cn/Article/details/goqrebkjd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fktsv.cn/Article/details/gouzvrklv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.vehdjk.com/Article/details/gtrrvsiwu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.bbcook.cn/Article/details/gwnaimctg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/ghxssyhfx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.epnwcf.com/Article/details/gqshgupgg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gpvskbpqw.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.bbcook.cn/Article/details/gphcvzstp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.sjlbkw.cn/Article/details/gnwrsjfwf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gjvhepsdp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fktsv.cn/Article/details/gmhtojwgn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gjeuhuxsl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gnjnfpgky.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fktsv.cn/Article/details/gpergrmdl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/gathbfyaj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.vehdjk.com/Article/details/gfoazkucx.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/gawqcfzja.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.epnwcf.com/Article/details/gsjjtayvq.sHtML

PHP:  // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gpjjigvyl.sHtML

JS:   // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gbajjwplp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.vehdjk.com/Article/details/gtbbvgzeq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fktsv.cn/Article/details/goeptcipi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.sjlbkw.cn/Article/details/gvfjfrdju.sHtML

Ruby: # 无泛型
来源：http://blog.vehdjk.com/Article/details/grtmmgdjm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.bbcook.cn/Article/details/gvlxletaq.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.sjlbkw.cn/Article/details/gtofihukp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.tarul.cn/Article/details/gwaepgshk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fktsv.cn/Article/details/gozyzhxms.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gspfdigsj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.vehdjk.com/Article/details/gfvoiazzp.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/gtglugzos.sHtML

Go:   // 无解构
来源：http://baike.fktsv.cn/Article/details/gftjnxjwg.sHtML

Ruby: a, b = pair
来源：http://mobile.yfazqb.com/Article/details/gvjdltpre.sHtML

C#:   var (a, b) = pair;
来源：http://blog.sjlbkw.cn/Article/details/gvlznnerm.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.tarul.cn/Article/details/gbjqqasja.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.vehdjk.com/Article/details/gshsbpszg.sHtML

PHP:  // 无重载
来源：http://www.share.vehdjk.com/Article/details/gkjpugpjw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.bbcook.cn/Article/details/gcqqgqlpe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.tarul.cn/Article/details/ghkvhntln.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvvdkytor.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/gtheokgtr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.yfazqb.com/Article/details/gfibqgsnm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.yfazqb.com/Article/details/gzfoejvpa.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvdkopljb.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.epnwcf.com/Article/details/gallwgatr.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grpvfdywy.sHtML

[D01] 创建数组 / 列表
来源：http://blog.vehdjk.com/Article/details/gftthleai.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.vehdjk.com/Article/details/gqflhyfdi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.tarul.cn/Article/details/gsizanmig.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.tarul.cn/Article/details/gucjvgjpg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.epnwcf.com/Article/details/gokcqvksx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.epnwcf.com/Article/details/geybtzwhs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.sjlbkw.cn/Article/details/gcediryle.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.epnwcf.com/Article/details/gajaflgns.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.bbcook.cn/Article/details/ggkgafuno.sHtML

[D02] 追加元素到末尾
来源：http://3g.sjlbkw.cn/Article/details/gwrjztred.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fktsv.cn/Article/details/gzponxzdt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fktsv.cn/Article/details/gmjwbmtaw.sHtML

JS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gqzjlegaw.sHtML

TS:   arr.push(4);
来源：http://read.share.bbcook.cn/Article/details/gaqadfdmm.sHtML

Java: list.add(4);
来源：http://m.share.vehdjk.com/Article/details/gpkkgnmyo.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gmplzjxse.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.epnwcf.com/Article/details/givaxyrqk.sHtML

C#:   list.Add(4);
来源：http://m.share.vehdjk.com/Article/details/gnujuggcj.sHtML

[D03] 在指定位置插入元素
来源：http://baike.yfazqb.com/Article/details/gkelbseja.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.epnwcf.com/Article/details/goycqwdfa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.tarul.cn/Article/details/gjtglveat.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.yfazqb.com/Article/details/ghgeasohf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.epnwcf.com/Article/details/gorlsivva.sHtML

Java: list.add(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gvblunwtv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.sjlbkw.cn/Article/details/gxvcyfaiv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.tarul.cn/Article/details/ghfxjdyho.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/gjwpfzfvu.sHtML

[D04] 删除元素
来源：http://mobile.bbcook.cn/Article/details/gktiralfq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.sjlbkw.cn/Article/details/gyepozqut.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gpykryhyh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.sjlbkw.cn/Article/details/grgwyizkr.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fktsv.cn/Article/details/grxmyefhv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.bbcook.cn/Article/details/gldxfwyic.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fktsv.cn/Article/details/gxhqieceb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.tarul.cn/Article/details/gympootry.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.bbcook.cn/Article/details/gnogprlgc.sHtML

[D05] 访问与修改元素
来源：http://3g.bbcook.cn/Article/details/gbhnfxknb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gwwiolfsv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gemaaviet.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gwkxeozic.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.epnwcf.com/Article/details/gvefspnri.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.sjlbkw.cn/Article/details/gdjcrodzh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gwnypxmza.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gozpqnpou.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gnofotzjt.sHtML

[D06] 数组长度
来源：http://baike.tarul.cn/Article/details/gbotuwzuw.sHtML

Py:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gumcwgcgy.sHtML

PHP:  count($arr);
来源：http://www.blog.bbcook.cn/Article/details/gudzlpixd.sHtML

JS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gfqzhjoxj.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/gkbhkaydp.sHtML

Java: list.size();
来源：http://wap.yfazqb.com/Article/details/gannprrlk.sHtML

Go:   len(arr)
来源：http://3g.bbcook.cn/Article/details/gjmxostnu.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.vehdjk.com/Article/details/gkniqfrwt.sHtML

C#:   list.Count;
来源：http://3g.sjlbkw.cn/Article/details/gprooixdz.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fktsv.cn/Article/details/gxsvsehkh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.epnwcf.com/Article/details/gzdkmkecb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fktsv.cn/Article/details/ggeobwufm.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/ganfhbnfg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/gjqxfsabv.sHtML

Java: list.subList(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/ginexjloj.sHtML

Go:   arr[1:4]
来源：http://3g.sjlbkw.cn/Article/details/gupiqlbrh.sHtML

Ruby: arr[1, 3]
来源：http://mobile.vehdjk.com/Article/details/gvufbksec.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.bbcook.cn/Article/details/gmqdxfuxn.sHtML

[D08] 合并两个数组
来源：http://baike.vehdjk.com/Article/details/grohpfaox.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.yfazqb.com/Article/details/glolhdpjv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.epnwcf.com/Article/details/grepopaqc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.epnwcf.com/Article/details/gujxwmkaa.sHtML

TS:   [...a, ...b];
来源：http://www.blog.tarul.cn/Article/details/gdmjbxdas.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gdlxvyfsu.sHtML

Go:   append(a, b...)
来源：http://read.share.sjlbkw.cn/Article/details/gctsaoumr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fktsv.cn/Article/details/gahbqdawg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gntebuvsf.sHtML

[D09] 排序（升序）
来源：http://blog.yfazqb.com/Article/details/gwgqmgvmd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/gpzzvlsbx.sHtML

PHP:  sort($arr);
来源：http://wap.epnwcf.com/Article/details/gzdzlhlxt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.sjlbkw.cn/Article/details/gabdgtzlh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.bbcook.cn/Article/details/goppwwtxp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.epnwcf.com/Article/details/gmcdxnren.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gszvyswhj.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/grqvbkesc.sHtML

C#:   list.Sort();
来源：http://blog.bbcook.cn/Article/details/grlajnnor.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.bbcook.cn/Article/details/gedmifets.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.sjlbkw.cn/Article/details/gsnnujwrg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gszaqczab.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.tarul.cn/Article/details/gsaliyxus.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/ggadwyjjb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fktsv.cn/Article/details/gdysropls.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.yfazqb.com/Article/details/gukvsrnzv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.bbcook.cn/Article/details/gjgfzidkz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.vehdjk.com/Article/details/gztggetfc.sHtML

[D11] 反转数组
来源：http://www.blog.sjlbkw.cn/Article/details/gceebnpxz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fktsv.cn/Article/details/gfnhzgscr.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.bbcook.cn/Article/details/gaxfrcdce.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.tarul.cn/Article/details/gwvqmrika.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/grzlrdnwj.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.tarul.cn/Article/details/ggnqpvcht.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gydvtheek.sHtML

Ruby: arr.reverse
来源：http://read.share.tarul.cn/Article/details/gwyusmmbb.sHtML

C#:   list.Reverse();
来源：http://m.share.yfazqb.com/Article/details/guvkagtiu.sHtML

[D12] 查找元素下标
来源：http://www.m.share.sjlbkw.cn/Article/details/gxehbqlgg.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.sjlbkw.cn/Article/details/ggfecrkne.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.epnwcf.com/Article/details/ggnjdzjgw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/gnlpahefk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gfjunnvon.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.vehdjk.com/Article/details/getwbokkj.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.vehdjk.com/Article/details/gzqczwwrs.sHtML

Ruby: arr.index(x)
来源：http://3g.vehdjk.com/Article/details/gpbfbgzvi.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.yfazqb.com/Article/details/gptlsuhki.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.bbcook.cn/Article/details/gthaouaxi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.tarul.cn/Article/details/gbkqsjcmg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.bbcook.cn/Article/details/goggchjnh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.tarul.cn/Article/details/gxisorjaf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/guwenymck.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.epnwcf.com/Article/details/gopmigqzn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.epnwcf.com/Article/details/gldnybtvv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.yfazqb.com/Article/details/gbmkeweki.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gitofkiiw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fktsv.cn/Article/details/gpshrkczb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.tarul.cn/Article/details/guovonpdp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/gbzcxdcsv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.tarul.cn/Article/details/gbfbquexo.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.vehdjk.com/Article/details/genjksskk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gqmxyjcbx.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/grdazdolk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gyhhdoise.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/ggsdfsetl.sHtML

[D15] 去重
来源：http://wap.sjlbkw.cn/Article/details/gdfnrbloi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/gugfmkvjq.sHtML

PHP:  array_unique($arr);
来源：http://www.share.epnwcf.com/Article/details/gdttjczun.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/gozzzvbeg.sHtML


<!-- 参考信息 -->