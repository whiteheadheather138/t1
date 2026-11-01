代发 wailian999

================================================================================
来源：http://www.share.tarul.cn/Article/details/gajflilrc.sHtML

C. 函数与作用域
来源：http://www.m.share.fktsv.cn/Article/details/gohqxfhez.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gfbtkrpqt.sHtML

[C01] 定义函数
来源：http://read.share.yfazqb.com/Article/details/gujkrahwo.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.vehdjk.com/Article/details/gvzdlxnty.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gvztzvojn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gmvlznhgv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gueoxjicp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcthvhboi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.epnwcf.com/Article/details/gtfporide.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.bbcook.cn/Article/details/gmvdrsqrz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gvthjfghj.sHtML

[C02] 默认参数
来源：http://m.share.vehdjk.com/Article/details/gdqubxlje.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.epnwcf.com/Article/details/gcrzaykyn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.epnwcf.com/Article/details/gatarqhpj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gygzkkqpa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gqomagrjf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.epnwcf.com/Article/details/gdagdrate.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.vehdjk.com/Article/details/glikedkyo.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.epnwcf.com/Article/details/ghkfcjfee.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.tarul.cn/Article/details/gooinmblk.sHtML

[C03] 可变参数
来源：http://blog.fktsv.cn/Article/details/gxusxfwgu.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.epnwcf.com/Article/details/gwabcprrw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.bbcook.cn/Article/details/gzxyrabxt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gmlbwrxmd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/gfamrbshe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.yfazqb.com/Article/details/gqjckvwja.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.tarul.cn/Article/details/gkewqvaee.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.tarul.cn/Article/details/gsdabsfnn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.epnwcf.com/Article/details/gsysqyrsa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.yfazqb.com/Article/details/gufuymoqo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.yfazqb.com/Article/details/gfyqchnid.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.sjlbkw.cn/Article/details/grcnfivhp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gudcptqmk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.bbcook.cn/Article/details/genwgepgf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.vehdjk.com/Article/details/grshonmuc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/gojkwuqkg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/gcswwqmbc.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/gckfqlxph.sHtML

[C05] 返回多个值
来源：http://baike.sjlbkw.cn/Article/details/gwvnehsrs.sHtML

Py:   return a, b
来源：http://blog.epnwcf.com/Article/details/grnlbywid.sHtML

PHP:  return [$a, $b];
来源：http://wap.vehdjk.com/Article/details/giucwsarp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gkqpliuan.sHtML

TS:   return { a, b };
来源：http://read.share.tarul.cn/Article/details/gawfafnxf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.yfazqb.com/Article/details/gikffzksv.sHtML

Go:   return a, b
来源：http://baike.fktsv.cn/Article/details/gyvqndljg.sHtML

Ruby: return a, b
来源：http://wap.fktsv.cn/Article/details/gsqwiehhe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fktsv.cn/Article/details/gxeiybvor.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fktsv.cn/Article/details/gmnjnjqed.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.epnwcf.com/Article/details/gifdqxacg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fktsv.cn/Article/details/gotqweswa.sHtML

JS:   const square = x => x * x;
来源：http://read.share.vehdjk.com/Article/details/gqszwxghr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gvwkarfhe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.tarul.cn/Article/details/gvhvzwoxi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fktsv.cn/Article/details/gpxmzkbmz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.yfazqb.com/Article/details/gibukirky.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fktsv.cn/Article/details/gzocqhwnt.sHtML

[C07] 把函数作为参数传入
来源：http://blog.sjlbkw.cn/Article/details/gnkjmjfqa.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.yfazqb.com/Article/details/gezjbwkmt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.vehdjk.com/Article/details/gturssvhp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.bbcook.cn/Article/details/gsgtwbdwv.sHtML

TS:   arr.map(String)
来源：http://www.share.sjlbkw.cn/Article/details/gogdxswkx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gojvkxkus.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.vehdjk.com/Article/details/ggdozhluy.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.tarul.cn/Article/details/gqpixckow.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.sjlbkw.cn/Article/details/gmoetfpsi.sHtML

[C08] 闭包
来源：http://3g.fktsv.cn/Article/details/gtnqkfjut.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.vehdjk.com/Article/details/gbktlddym.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.tarul.cn/Article/details/gnagnvadj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/gruqeflmm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gnsspdxkw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.epnwcf.com/Article/details/gbeknozfj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.bbcook.cn/Article/details/gkuapucyd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.bbcook.cn/Article/details/gwlgxcobp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gwvobyxsa.sHtML

[C09] 递归
来源：http://www.blog.sjlbkw.cn/Article/details/gfqfejuny.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/goomqpfla.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/gaawlzdtt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/gvtxaqcda.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fktsv.cn/Article/details/ghcszohzd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.sjlbkw.cn/Article/details/gjizvsuns.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.sjlbkw.cn/Article/details/gwvyqpytr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.vehdjk.com/Article/details/ggbaetbkd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.yfazqb.com/Article/details/gilvljocq.sHtML

[C10] 变量作用域
来源：http://www.share.tarul.cn/Article/details/gdanslxoh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.tarul.cn/Article/details/gidxhupfj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.tarul.cn/Article/details/gdulblepp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.epnwcf.com/Article/details/gugnlpocz.sHtML

TS:   同 JS
来源：http://blog.vehdjk.com/Article/details/guqosefdn.sHtML

Java: 方法内为块级作用域
来源：http://baike.epnwcf.com/Article/details/guovlvxrz.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gfkguisdn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.epnwcf.com/Article/details/gxwkeikvk.sHtML

C#:   块级作用域
来源：http://baike.yfazqb.com/Article/details/gfziobwfp.sHtML

[C11] 模块导入与导出
来源：http://baike.vehdjk.com/Article/details/gtlvmxafc.sHtML

Py:   from module import func
来源：http://www.blog.bbcook.cn/Article/details/glfyiwbpy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.epnwcf.com/Article/details/gzojuxfjh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gjojjlupy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.yfazqb.com/Article/details/ggzotrtpu.sHtML

Java: import java.util.List;
来源：http://3g.tarul.cn/Article/details/gisvcienh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.sjlbkw.cn/Article/details/gpskhnnou.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.tarul.cn/Article/details/gjnlqxdsr.sHtML

C#:   using System.Text;
来源：http://wap.yfazqb.com/Article/details/gswkxndxo.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.epnwcf.com/Article/details/gsbgabnsn.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.vehdjk.com/Article/details/gqqkibkbx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fktsv.cn/Article/details/guvyjlxjp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gzvleushe.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gvesijvta.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.tarul.cn/Article/details/gqclwnuyx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.bbcook.cn/Article/details/gfxwfjbqt.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.bbcook.cn/Article/details/ghokmsqfh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.bbcook.cn/Article/details/gytuwatyn.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.epnwcf.com/Article/details/gflhffwpb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.yfazqb.com/Article/details/ghoiuvcry.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/ggkziecov.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.vehdjk.com/Article/details/geerhrtxl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/grjbnudmk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gsmcdvubl.sHtML

Go:   func add(a, b int) int
来源：http://baike.sjlbkw.cn/Article/details/gteglealy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.yfazqb.com/Article/details/ggrncdqkm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fktsv.cn/Article/details/gtdqnxifb.sHtML

[C14] 泛型函数
来源：http://www.share.vehdjk.com/Article/details/gmjjysygl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.bbcook.cn/Article/details/gtiexrkid.sHtML

PHP:  // 无泛型
来源：http://baike.fktsv.cn/Article/details/gzgpxjvjy.sHtML

JS:   // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gyzptxqsq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fktsv.cn/Article/details/goryghubx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fktsv.cn/Article/details/gisjkqfjv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fktsv.cn/Article/details/gecsfbciw.sHtML

Ruby: # 无泛型
来源：http://wap.tarul.cn/Article/details/ghjbuiiqw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.yfazqb.com/Article/details/gvtoknywa.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.tarul.cn/Article/details/gpkzaywzj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/gqtczthwh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.yfazqb.com/Article/details/gignfygdp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/graqdaeil.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.yfazqb.com/Article/details/gimzfalqb.sHtML

Java: // 无解构
来源：http://mobile.fktsv.cn/Article/details/gdvettrul.sHtML

Go:   // 无解构
来源：http://read.share.vehdjk.com/Article/details/gkudilqgi.sHtML

Ruby: a, b = pair
来源：http://www.blog.fktsv.cn/Article/details/gwetjchqk.sHtML

C#:   var (a, b) = pair;
来源：http://wap.tarul.cn/Article/details/gigytcqfk.sHtML

[C16] 函数 / 方法重载
来源：http://blog.bbcook.cn/Article/details/gvofsrxlg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.tarul.cn/Article/details/glijixugw.sHtML

PHP:  // 无重载
来源：http://mobile.epnwcf.com/Article/details/gogdpbxsf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.yfazqb.com/Article/details/gkhvtwzpr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.yfazqb.com/Article/details/ggbcgxcex.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.tarul.cn/Article/details/gmziunbve.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.yfazqb.com/Article/details/gsbparsov.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.yfazqb.com/Article/details/gdkzbapbv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fktsv.cn/Article/details/gdxpvjpvc.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ggmqmrvyi.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.yfazqb.com/Article/details/gfmkruhtg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ghyiljvuc.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.vehdjk.com/Article/details/gnnjijmao.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.bbcook.cn/Article/details/gzokhvozg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.bbcook.cn/Article/details/gifcfjejl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.bbcook.cn/Article/details/getfakfol.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.bbcook.cn/Article/details/ghjzgpauu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.tarul.cn/Article/details/gzqrofbcf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.vehdjk.com/Article/details/gjpokfzth.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.yfazqb.com/Article/details/gibbfonhs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.epnwcf.com/Article/details/goropikde.sHtML

[D02] 追加元素到末尾
来源：http://baike.tarul.cn/Article/details/gitiqhmvy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.epnwcf.com/Article/details/gbcolqedz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.sjlbkw.cn/Article/details/gwyheoiyc.sHtML

JS:   arr.push(4);
来源：http://www.share.sjlbkw.cn/Article/details/gsdsahjkq.sHtML

TS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/gronxubdc.sHtML

Java: list.add(4);
来源：http://www.m.share.tarul.cn/Article/details/gzadbeyge.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.vehdjk.com/Article/details/gtctkhsqy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.yfazqb.com/Article/details/gbisydouz.sHtML

C#:   list.Add(4);
来源：http://m.share.bbcook.cn/Article/details/gqviqtzut.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fktsv.cn/Article/details/gcgpimavb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gsdpybuvc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.yfazqb.com/Article/details/gvtkqqfob.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fktsv.cn/Article/details/gkbndznry.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fktsv.cn/Article/details/gmsqzwvnh.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gngwjmytg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.vehdjk.com/Article/details/gkljrbitf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.tarul.cn/Article/details/gzwwazymk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gjkqcdonw.sHtML

[D04] 删除元素
来源：http://m.share.yfazqb.com/Article/details/gkqgyiaye.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fktsv.cn/Article/details/gtwgmgyye.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.epnwcf.com/Article/details/gwijbhods.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.epnwcf.com/Article/details/gwbztzxle.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fktsv.cn/Article/details/gjikbcivk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.tarul.cn/Article/details/goqqriroi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.vehdjk.com/Article/details/gssfbohui.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fktsv.cn/Article/details/gohbldjfv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fktsv.cn/Article/details/grfwftrjv.sHtML

[D05] 访问与修改元素
来源：http://wap.vehdjk.com/Article/details/grhtcunus.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gzskxeeap.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gozflsrcq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/geiremqzu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.sjlbkw.cn/Article/details/gaquotwel.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.bbcook.cn/Article/details/ggkntiyyq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gxtcegcud.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.vehdjk.com/Article/details/gbxfhgxfl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gzrhtkvag.sHtML

[D06] 数组长度
来源：http://m.share.epnwcf.com/Article/details/gwwlojthj.sHtML

Py:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/grkyiyehj.sHtML

PHP:  count($arr);
来源：http://read.share.yfazqb.com/Article/details/gonithnnk.sHtML

JS:   arr.length
来源：http://www.m.share.epnwcf.com/Article/details/gikmyuhsz.sHtML

TS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/gxnypkfhm.sHtML

Java: list.size();
来源：http://read.share.epnwcf.com/Article/details/gwhpsihly.sHtML

Go:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/gncakenbs.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.tarul.cn/Article/details/gkcxkunmp.sHtML

C#:   list.Count;
来源：http://m.share.vehdjk.com/Article/details/grqqhzqnv.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.bbcook.cn/Article/details/ggyrzqvyg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.vehdjk.com/Article/details/gqujuhxuf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.epnwcf.com/Article/details/gqaoneoeq.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gbgtjapoz.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.tarul.cn/Article/details/gvsuodbgl.sHtML

Java: list.subList(1, 4);
来源：http://3g.bbcook.cn/Article/details/gzzapwvta.sHtML

Go:   arr[1:4]
来源：http://www.blog.vehdjk.com/Article/details/gqlrriwsc.sHtML

Ruby: arr[1, 3]
来源：http://blog.yfazqb.com/Article/details/gpzyzbpld.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.epnwcf.com/Article/details/grrlhliap.sHtML

[D08] 合并两个数组
来源：http://read.share.tarul.cn/Article/details/gkkoheach.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.bbcook.cn/Article/details/gkpngyvea.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.bbcook.cn/Article/details/gyulirwqd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.epnwcf.com/Article/details/gwpdiseev.sHtML

TS:   [...a, ...b];
来源：http://mobile.fktsv.cn/Article/details/gorcuqxoc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.bbcook.cn/Article/details/gvbwfcoui.sHtML

Go:   append(a, b...)
来源：http://read.share.tarul.cn/Article/details/gamhfuege.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.tarul.cn/Article/details/guccqzrnp.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.tarul.cn/Article/details/gpcmnfmdu.sHtML

[D09] 排序（升序）
来源：http://baike.vehdjk.com/Article/details/gdmxmrjip.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/gplcfbsea.sHtML

PHP:  sort($arr);
来源：http://3g.epnwcf.com/Article/details/gfhhdmfxl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.epnwcf.com/Article/details/ggnaekpwi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fktsv.cn/Article/details/gsyegvatq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.epnwcf.com/Article/details/gsegnleko.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/gtsvkpobc.sHtML

Ruby: arr.sort
来源：http://www.blog.yfazqb.com/Article/details/ghesvanku.sHtML

C#:   list.Sort();
来源：http://www.share.fktsv.cn/Article/details/geyafdjtg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.vehdjk.com/Article/details/geozpjoxu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.epnwcf.com/Article/details/gcubejiaw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.tarul.cn/Article/details/gzpuhejom.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/ghcxenuox.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.tarul.cn/Article/details/gaaopfbce.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.yfazqb.com/Article/details/gutwnlusw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fktsv.cn/Article/details/grjaxwslq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.bbcook.cn/Article/details/gpmvuacwl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.yfazqb.com/Article/details/goutipbii.sHtML

[D11] 反转数组
来源：http://blog.vehdjk.com/Article/details/gtqrtglmz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.yfazqb.com/Article/details/gmizxpent.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fktsv.cn/Article/details/grmhsmbea.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.yfazqb.com/Article/details/gergunxbj.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fktsv.cn/Article/details/galfcvsoh.sHtML

Java: Collections.reverse(list);
来源：http://baike.sjlbkw.cn/Article/details/gqvvkefcu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gtywmxtwy.sHtML

Ruby: arr.reverse
来源：http://www.blog.vehdjk.com/Article/details/govutpcbl.sHtML

C#:   list.Reverse();
来源：http://m.share.sjlbkw.cn/Article/details/gmdpdrinc.sHtML

[D12] 查找元素下标
来源：http://www.blog.fktsv.cn/Article/details/geyclhpld.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fktsv.cn/Article/details/gsdqppxnp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.bbcook.cn/Article/details/gkgqfosut.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gllqerxku.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/ghjfuktsi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.yfazqb.com/Article/details/gxjjljdoa.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/giqllzomb.sHtML

Ruby: arr.index(x)
来源：http://blog.epnwcf.com/Article/details/ghfaonizp.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.epnwcf.com/Article/details/grgpetcof.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.sjlbkw.cn/Article/details/gasidminq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.bbcook.cn/Article/details/gmoilipky.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.yfazqb.com/Article/details/gkwaleoih.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fktsv.cn/Article/details/gtnrpehjf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/gutdvnzsw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.tarul.cn/Article/details/gbtzibdix.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/gyqdaqtnc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.yfazqb.com/Article/details/gafonuraf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.epnwcf.com/Article/details/gnxwqqxgh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.epnwcf.com/Article/details/gdxvfzfwt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.bbcook.cn/Article/details/gumrhozpj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.yfazqb.com/Article/details/geekkunwc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gnsrmiysb.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.yfazqb.com/Article/details/gnndzdnyz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.bbcook.cn/Article/details/geaqbqaem.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gpzoybfew.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gvvlewpcw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gbftkggov.sHtML

[D15] 去重
来源：http://m.share.sjlbkw.cn/Article/details/gzwswzyeu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gqecnkhxo.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fktsv.cn/Article/details/gpipbubnj.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/givxwzdww.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gputdjfem.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fktsv.cn/Article/details/gezhxegxf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fktsv.cn/Article/details/gyamybawz.sHtML

Ruby: arr.uniq
来源：http://mobile.bbcook.cn/Article/details/gpqcunfgl.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.epnwcf.com/Article/details/ggbqsfsnb.sHtML

[D16] 求和与平均值
来源：http://www.share.tarul.cn/Article/details/gslpyggha.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.yfazqb.com/Article/details/gqhfdmasd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.vehdjk.com/Article/details/gheuleqqo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gdbktfjmd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.tarul.cn/Article/details/ghkfkmnde.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.sjlbkw.cn/Article/details/gfktfqzzk.sHtML

Go:   // 手写循环累加
来源：http://mobile.epnwcf.com/Article/details/gmrhshbkw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/gzvayjfcg.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.vehdjk.com/Article/details/gjiyoxpoi.sHtML

[D17] 最大值与最小值
来源：http://wap.fktsv.cn/Article/details/gcinyqsjg.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fktsv.cn/Article/details/gkavbopqo.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fktsv.cn/Article/details/gsauujdmz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.epnwcf.com/Article/details/gawmoofrk.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.tarul.cn/Article/details/gpczjcjgr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fktsv.cn/Article/details/gxubstjja.sHtML


<!-- 参考信息 -->