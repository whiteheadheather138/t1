代发 wailian999

Py:   if not data: return
来源：http://wap.fktsv.cn/Article/details/grccgkmig.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.yfazqb.com/Article/details/gvegxjyvt.sHtML

JS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gghinynrs.sHtML

TS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gmpjyonnw.sHtML

Java: if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/gcgyepphi.sHtML

Go:   if data == nil { return }
来源：http://m.share.sjlbkw.cn/Article/details/gvgfkitym.sHtML

Ruby: return if data.nil?
来源：http://baike.fktsv.cn/Article/details/gbimxirjo.sHtML

C#:   if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gouwxykwi.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdonbapam.sHtML

C. 函数与作用域
来源：http://wap.tarul.cn/Article/details/gqnuwowir.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/giathbtly.sHtML

[C01] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/gbgetbahc.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.vehdjk.com/Article/details/gtejbnhki.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gsewgcljc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gwwenvkjy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gchhymast.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gxergrqlk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.bbcook.cn/Article/details/giawcezdu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.sjlbkw.cn/Article/details/gwpgaxxuo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gpsncpyil.sHtML

[C02] 默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gkwigfllr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.bbcook.cn/Article/details/gzbwhbqro.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.epnwcf.com/Article/details/gbyqwimdb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gncbaubtk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/ghceliwtp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.tarul.cn/Article/details/gywgoinmq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fktsv.cn/Article/details/ghplutxnn.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fktsv.cn/Article/details/gyvdgtfjj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.sjlbkw.cn/Article/details/gpsmkpoor.sHtML

[C03] 可变参数
来源：http://3g.tarul.cn/Article/details/gxszmddcv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.tarul.cn/Article/details/gwhgktbnq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzdtctip.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gzatktdpe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.tarul.cn/Article/details/gvyafzylc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.vehdjk.com/Article/details/gnghuzydo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.tarul.cn/Article/details/guvbsrnaz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.vehdjk.com/Article/details/gricprlkm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.bbcook.cn/Article/details/ginpdcmzk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.epnwcf.com/Article/details/gktqtjewn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.sjlbkw.cn/Article/details/gevrggltm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.yfazqb.com/Article/details/gooarazlr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/gxwqldmqb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gaxmydjyq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.sjlbkw.cn/Article/details/ggwzibtdw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/grabmdgbi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gomkfuzbp.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/grniukszf.sHtML

[C05] 返回多个值
来源：http://www.m.share.vehdjk.com/Article/details/glfigikui.sHtML

Py:   return a, b
来源：http://3g.tarul.cn/Article/details/glwwtlpjz.sHtML

PHP:  return [$a, $b];
来源：http://www.share.vehdjk.com/Article/details/gkaoutghf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fktsv.cn/Article/details/golpqxerc.sHtML

TS:   return { a, b };
来源：http://m.share.sjlbkw.cn/Article/details/gnrmkrebz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.bbcook.cn/Article/details/gnofjitzn.sHtML

Go:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gekmxtnxg.sHtML

Ruby: return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gtxavbkor.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.sjlbkw.cn/Article/details/grdlkgszi.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.sjlbkw.cn/Article/details/gsaeaocyr.sHtML

Py:   square = lambda x: x * x
来源：http://3g.tarul.cn/Article/details/gbvlhvolu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.vehdjk.com/Article/details/gjodqytqk.sHtML

JS:   const square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gvndmunjb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.bbcook.cn/Article/details/gmmxyhazl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.bbcook.cn/Article/details/gethhvsuy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fktsv.cn/Article/details/ggrtwpcsa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fktsv.cn/Article/details/gnyrjlggl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/gogreqofy.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fktsv.cn/Article/details/gqyyegbth.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.tarul.cn/Article/details/grtjqwtlt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gbzypdphq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.tarul.cn/Article/details/gymxzvlvi.sHtML

TS:   arr.map(String)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbrtzadv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.tarul.cn/Article/details/gpcmtezek.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.epnwcf.com/Article/details/gsvzxlrwr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.tarul.cn/Article/details/gwqtzeubb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.vehdjk.com/Article/details/gyuaxriya.sHtML

[C08] 闭包
来源：http://www.share.vehdjk.com/Article/details/genmlyhkx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fktsv.cn/Article/details/glxjfurlb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.vehdjk.com/Article/details/gxrwcvakz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gtkueatdf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/guxlpsfzr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.tarul.cn/Article/details/ggjlakjbj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.sjlbkw.cn/Article/details/gzcbuaioz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.epnwcf.com/Article/details/gojkupwvc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gkahuyhhc.sHtML

[C09] 递归
来源：http://blog.tarul.cn/Article/details/gynoedujb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/glfvqaxww.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.bbcook.cn/Article/details/gtldhlhpc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/grwllcdyb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.epnwcf.com/Article/details/glyuskbam.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.tarul.cn/Article/details/gblpzbxpr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.epnwcf.com/Article/details/gsxzdnvpq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.vehdjk.com/Article/details/glvrvplen.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.epnwcf.com/Article/details/grzkuextn.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/gcwlqjqyt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.sjlbkw.cn/Article/details/gmppccndi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.sjlbkw.cn/Article/details/gpndjvspf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fktsv.cn/Article/details/gmotebidx.sHtML

TS:   同 JS
来源：http://wap.yfazqb.com/Article/details/gwzerlvoj.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.yfazqb.com/Article/details/gvfloqajy.sHtML

Go:   花括号块级作用域
来源：http://blog.tarul.cn/Article/details/gdblzvlrq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fktsv.cn/Article/details/gnppippwz.sHtML

C#:   块级作用域
来源：http://www.blog.tarul.cn/Article/details/goqalryei.sHtML

[C11] 模块导入与导出
来源：http://baike.vehdjk.com/Article/details/gvjtjgkqk.sHtML

Py:   from module import func
来源：http://www.share.sjlbkw.cn/Article/details/gvbhwxdbj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fktsv.cn/Article/details/gwftyzlyw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/gsarvmcru.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.sjlbkw.cn/Article/details/gdcjzvgxu.sHtML

Java: import java.util.List;
来源：http://www.m.share.yfazqb.com/Article/details/gooubtver.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.epnwcf.com/Article/details/gixmnqqlt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.tarul.cn/Article/details/gyqtckyrg.sHtML

C#:   using System.Text;
来源：http://mobile.fktsv.cn/Article/details/guqlxrezk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.sjlbkw.cn/Article/details/giconfuef.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fktsv.cn/Article/details/gsgryefcl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.vehdjk.com/Article/details/gphhvxcps.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.epnwcf.com/Article/details/gqwdxabkd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gsupfaoat.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.bbcook.cn/Article/details/gezszzsnv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.sjlbkw.cn/Article/details/glpkupily.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.epnwcf.com/Article/details/ggxekmcqt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gyvftfbnm.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.vehdjk.com/Article/details/gwaaycxaw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.bbcook.cn/Article/details/gbgxcjjii.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gayjfehoq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.epnwcf.com/Article/details/gdevmldcb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gthcceptn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/geqgjkfty.sHtML

Go:   func add(a, b int) int
来源：http://mobile.tarul.cn/Article/details/grpzufhmf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fktsv.cn/Article/details/gjgxsxjqd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.tarul.cn/Article/details/gpvzshjtr.sHtML

[C14] 泛型函数
来源：http://wap.sjlbkw.cn/Article/details/gvfogbypn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.vehdjk.com/Article/details/gmkxqgoup.sHtML

PHP:  // 无泛型
来源：http://m.share.bbcook.cn/Article/details/gjfophvzc.sHtML

JS:   // 无泛型
来源：http://baike.tarul.cn/Article/details/gqyikyymq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.vehdjk.com/Article/details/gnzdrynpp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.bbcook.cn/Article/details/ghnumowjr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.yfazqb.com/Article/details/geihvrkbg.sHtML

Ruby: # 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gchldsqhi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.epnwcf.com/Article/details/gkhkoculn.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.bbcook.cn/Article/details/ghuefgpzo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.vehdjk.com/Article/details/guutjnfqn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.epnwcf.com/Article/details/geghgcjhh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/ggeofngtc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.tarul.cn/Article/details/gutkjzkzk.sHtML

Java: // 无解构
来源：http://read.share.fktsv.cn/Article/details/glsgjsetk.sHtML

Go:   // 无解构
来源：http://3g.vehdjk.com/Article/details/geglmnpgo.sHtML

Ruby: a, b = pair
来源：http://www.share.vehdjk.com/Article/details/gnnjaghnl.sHtML

C#:   var (a, b) = pair;
来源：http://3g.vehdjk.com/Article/details/gnutsiipu.sHtML

[C16] 函数 / 方法重载
来源：http://3g.epnwcf.com/Article/details/gmxzjtcnb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.tarul.cn/Article/details/gmhdqxjsp.sHtML

PHP:  // 无重载
来源：http://www.blog.fktsv.cn/Article/details/gzgngfzje.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.sjlbkw.cn/Article/details/gmqfwoian.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.epnwcf.com/Article/details/gohwljrfu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.vehdjk.com/Article/details/gjwrnoydr.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.vehdjk.com/Article/details/ggzhrphre.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.sjlbkw.cn/Article/details/grcppreay.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.bbcook.cn/Article/details/gojzzxunv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/grlofhvyb.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.bbcook.cn/Article/details/gnrjtqfsa.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gcncolvyi.sHtML

[D01] 创建数组 / 列表
来源：http://3g.vehdjk.com/Article/details/gvmihwkbp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.vehdjk.com/Article/details/gwbhhpeuz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.yfazqb.com/Article/details/gokxaqdzx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.yfazqb.com/Article/details/gmbortfve.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.sjlbkw.cn/Article/details/gdfgaubxd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.yfazqb.com/Article/details/gavqwptmz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.sjlbkw.cn/Article/details/gkvzxojox.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fktsv.cn/Article/details/gyuxhohzv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.bbcook.cn/Article/details/gvmasquez.sHtML

[D02] 追加元素到末尾
来源：http://blog.sjlbkw.cn/Article/details/gqmdglqtd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.bbcook.cn/Article/details/gilrjwshq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdiqdgbwv.sHtML

JS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gruzsvmuu.sHtML

TS:   arr.push(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdfllhzd.sHtML

Java: list.add(4);
来源：http://wap.epnwcf.com/Article/details/gzwhocrjz.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.yfazqb.com/Article/details/glsxkzlll.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fktsv.cn/Article/details/grykvdaft.sHtML

C#:   list.Add(4);
来源：http://blog.vehdjk.com/Article/details/gpkserzng.sHtML

[D03] 在指定位置插入元素
来源：http://blog.bbcook.cn/Article/details/gkbepxqtn.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.tarul.cn/Article/details/gsmmhjgrm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.sjlbkw.cn/Article/details/gvacccusw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.vehdjk.com/Article/details/gqbzsvsry.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fktsv.cn/Article/details/gmzkuogps.sHtML

Java: list.add(0, 0);
来源：http://read.share.bbcook.cn/Article/details/gwfnisjas.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.sjlbkw.cn/Article/details/guzyteqdo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.tarul.cn/Article/details/gqgwpyzzz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gljlzcwku.sHtML

[D04] 删除元素
来源：http://read.share.vehdjk.com/Article/details/gzgemdqvi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.yfazqb.com/Article/details/goonzwrba.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.yfazqb.com/Article/details/gnvjtyjim.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.epnwcf.com/Article/details/gwmudhosc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fktsv.cn/Article/details/gcuxbovfy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.yfazqb.com/Article/details/ggbiizkor.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.sjlbkw.cn/Article/details/gwdeoqeuc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.yfazqb.com/Article/details/gkjvjppdj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gibryndme.sHtML

[D05] 访问与修改元素
来源：http://www.blog.tarul.cn/Article/details/gfurkgyoi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gfjbztzhr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.tarul.cn/Article/details/grjewzkcm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gnxdbhadb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.yfazqb.com/Article/details/guvvvossh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.tarul.cn/Article/details/grabmsqqw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gygjnfsko.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gmpikzpqo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.vehdjk.com/Article/details/gcbdqtoyr.sHtML

[D06] 数组长度
来源：http://wap.fktsv.cn/Article/details/ggxnladwp.sHtML

Py:   len(arr)
来源：http://wap.bbcook.cn/Article/details/gponvkyxd.sHtML

PHP:  count($arr);
来源：http://baike.epnwcf.com/Article/details/gkljoauiq.sHtML

JS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/glziuachg.sHtML

TS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/ghckvnsvs.sHtML

Java: list.size();
来源：http://baike.sjlbkw.cn/Article/details/gtrxbbptc.sHtML

Go:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gqqmtlgdd.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.bbcook.cn/Article/details/gtfnsorqa.sHtML

C#:   list.Count;
来源：http://mobile.vehdjk.com/Article/details/gblndzkhh.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.yfazqb.com/Article/details/gnvdbztwf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.yfazqb.com/Article/details/gqqruodwk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gdbrnkzpk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/glnlduetq.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gomovdpga.sHtML

Java: list.subList(1, 4);
来源：http://m.share.tarul.cn/Article/details/gsatrfypy.sHtML

Go:   arr[1:4]
来源：http://mobile.yfazqb.com/Article/details/gyjdtxyht.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fktsv.cn/Article/details/gkbhfetta.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fktsv.cn/Article/details/gcsanbkcg.sHtML

[D08] 合并两个数组
来源：http://m.share.bbcook.cn/Article/details/gzlyoqljb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.vehdjk.com/Article/details/gdfkypaee.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fktsv.cn/Article/details/gdnfnaphf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.vehdjk.com/Article/details/gjewjvwpu.sHtML

TS:   [...a, ...b];
来源：http://wap.sjlbkw.cn/Article/details/gjvronvsw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.vehdjk.com/Article/details/gukhumctt.sHtML

Go:   append(a, b...)
来源：http://m.share.epnwcf.com/Article/details/gzihbaakq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.bbcook.cn/Article/details/gixbkxohb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.tarul.cn/Article/details/gmzqrwiyk.sHtML

[D09] 排序（升序）
来源：http://mobile.vehdjk.com/Article/details/giuuptaly.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.bbcook.cn/Article/details/gqfmdpvrz.sHtML

PHP:  sort($arr);
来源：http://read.share.epnwcf.com/Article/details/gdypqhnni.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.bbcook.cn/Article/details/ggpmscapl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fktsv.cn/Article/details/gjqugdpuu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.vehdjk.com/Article/details/gfpjhqlck.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/guumcgeue.sHtML

Ruby: arr.sort
来源：http://www.share.bbcook.cn/Article/details/gseeiyueo.sHtML

C#:   list.Sort();
来源：http://blog.vehdjk.com/Article/details/gyfsbmocc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.tarul.cn/Article/details/gvmdwmnjd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fktsv.cn/Article/details/gwoiwgoqg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/gnfdccizx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/gmuindmgf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gtsuaphyb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.epnwcf.com/Article/details/gskyjglom.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.vehdjk.com/Article/details/gdxacjerl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.sjlbkw.cn/Article/details/glcmxzwiz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.sjlbkw.cn/Article/details/gdyldxafi.sHtML

[D11] 反转数组
来源：http://read.share.tarul.cn/Article/details/gjueckwbe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.tarul.cn/Article/details/gvpcvahgh.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.vehdjk.com/Article/details/gbcldzmdy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.yfazqb.com/Article/details/gbogitpkn.sHtML

TS:   [...arr].reverse();
来源：http://mobile.yfazqb.com/Article/details/goaligbeg.sHtML

Java: Collections.reverse(list);
来源：http://mobile.yfazqb.com/Article/details/goygnchit.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.vehdjk.com/Article/details/gecmwcuyd.sHtML

Ruby: arr.reverse
来源：http://baike.epnwcf.com/Article/details/gulzjroga.sHtML

C#:   list.Reverse();
来源：http://baike.yfazqb.com/Article/details/gqpcvskee.sHtML

[D12] 查找元素下标
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlkuwbjd.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.sjlbkw.cn/Article/details/gsdlbdwrh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.epnwcf.com/Article/details/gjfblyxlw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.sjlbkw.cn/Article/details/guxnwvmdh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gxsrfoiyh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.vehdjk.com/Article/details/ggswdllbk.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/ggavsirfa.sHtML

Ruby: arr.index(x)
来源：http://www.share.sjlbkw.cn/Article/details/gubhfohar.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.tarul.cn/Article/details/gcoefyluf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.epnwcf.com/Article/details/gdiedjkfy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.bbcook.cn/Article/details/gdkbbwlqc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fktsv.cn/Article/details/gyphafiji.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gyrdxxsib.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/gsuasrfsi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.vehdjk.com/Article/details/gitypwaed.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.tarul.cn/Article/details/gilqpljhk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.yfazqb.com/Article/details/gvgspujoc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.bbcook.cn/Article/details/gwgapaffm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.epnwcf.com/Article/details/gdskpgrdy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.sjlbkw.cn/Article/details/gbfdzpvlc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.bbcook.cn/Article/details/glkijcvhb.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/gtqxicywr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gngffwrde.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.bbcook.cn/Article/details/gcmucufxv.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/gvaywsfgb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fktsv.cn/Article/details/gqwqygijz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.bbcook.cn/Article/details/gpboielpj.sHtML

[D15] 去重
来源：http://www.blog.fktsv.cn/Article/details/gjmosdjtq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.bbcook.cn/Article/details/ghtxyyiwt.sHtML

PHP:  array_unique($arr);
来源：http://baike.sjlbkw.cn/Article/details/gqcjnndgj.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/geoguzjff.sHtML

TS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/gxwbcqhyo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fktsv.cn/Article/details/gfeunnebg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.vehdjk.com/Article/details/gvytwabzq.sHtML

Ruby: arr.uniq
来源：http://www.blog.fktsv.cn/Article/details/gufxyzhpg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.epnwcf.com/Article/details/gpsmtrpxa.sHtML

[D16] 求和与平均值
来源：http://m.share.epnwcf.com/Article/details/gzzopuiam.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.epnwcf.com/Article/details/gvounsrfi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.epnwcf.com/Article/details/gzcmfsydq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fktsv.cn/Article/details/gyhuquiur.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.bbcook.cn/Article/details/gyckhfdnu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.vehdjk.com/Article/details/gjvytuxsl.sHtML

Go:   // 手写循环累加
来源：http://blog.sjlbkw.cn/Article/details/gwiwcpexm.sHtML


<!-- 参考信息 -->