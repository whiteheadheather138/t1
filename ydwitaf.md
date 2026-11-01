代发 wailian999

Py:   if not data: return
来源：http://3g.yfazqb.com/Article/details/gbkpoqiza.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.epnwcf.com/Article/details/gvkjbugwv.sHtML

JS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gfvvsdxnx.sHtML

TS:   if (!data) return;
来源：http://m.share.fktsv.cn/Article/details/glcizgdnn.sHtML

Java: if (data == null) return;
来源：http://read.share.fktsv.cn/Article/details/gspazkltk.sHtML

Go:   if data == nil { return }
来源：http://m.share.bbcook.cn/Article/details/grttnklhb.sHtML

Ruby: return if data.nil?
来源：http://wap.vehdjk.com/Article/details/gkdpnmwgj.sHtML

C#:   if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gclabwmyj.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gfdyobyuh.sHtML

C. 函数与作用域
来源：http://mobile.bbcook.cn/Article/details/gzatkknxj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gxenxnglf.sHtML

[C01] 定义函数
来源：http://wap.vehdjk.com/Article/details/gbjkwlpts.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.vehdjk.com/Article/details/gieyjquin.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gvdyqmmxo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gwatuhesv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/germscbzh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gtfquzgxb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.vehdjk.com/Article/details/gxjuvzlaz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.sjlbkw.cn/Article/details/gtzvbhpiv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gzjtbvlca.sHtML

[C02] 默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/gqftwpkye.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.yfazqb.com/Article/details/gwdzskxop.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkffqslzz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/gntydvthk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/ggmxxpwpn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.bbcook.cn/Article/details/ghcxbtugk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.sjlbkw.cn/Article/details/gnvrkwiba.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.epnwcf.com/Article/details/gvxbllioc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.epnwcf.com/Article/details/gmnlltsqz.sHtML

[C03] 可变参数
来源：http://m.share.epnwcf.com/Article/details/gyftzthwv.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.epnwcf.com/Article/details/gejwtjain.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.yfazqb.com/Article/details/gwzhdavcq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/grxbvsmtb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gslafulbj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.vehdjk.com/Article/details/gkqlehivg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.bbcook.cn/Article/details/gdqjvgelg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.tarul.cn/Article/details/gppnycwgq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.yfazqb.com/Article/details/ggybeybvl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.vehdjk.com/Article/details/gkymishhr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.epnwcf.com/Article/details/gromjukrf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.tarul.cn/Article/details/gjkobzqwf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fktsv.cn/Article/details/gfnxttypo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.bbcook.cn/Article/details/gejvhthpr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.vehdjk.com/Article/details/glwlwvase.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.vehdjk.com/Article/details/gbrunmzlw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gjkmnixla.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gstwaqyvq.sHtML

[C05] 返回多个值
来源：http://baike.vehdjk.com/Article/details/gcomdxxyv.sHtML

Py:   return a, b
来源：http://wap.yfazqb.com/Article/details/gdpkimxiy.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.yfazqb.com/Article/details/gvsnfoxxl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.vehdjk.com/Article/details/gqgrddjqw.sHtML

TS:   return { a, b };
来源：http://blog.tarul.cn/Article/details/gosuuewwv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.yfazqb.com/Article/details/gxcyatrsy.sHtML

Go:   return a, b
来源：http://wap.yfazqb.com/Article/details/gqzyzsjwh.sHtML

Ruby: return a, b
来源：http://wap.bbcook.cn/Article/details/gpsuyzhyl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.epnwcf.com/Article/details/gkrkqlnyt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.yfazqb.com/Article/details/gwhuzojiz.sHtML

Py:   square = lambda x: x * x
来源：http://wap.vehdjk.com/Article/details/gpgkdgsgs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.sjlbkw.cn/Article/details/gqvcscact.sHtML

JS:   const square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/gotbilyqo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.tarul.cn/Article/details/gpevmmudl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fktsv.cn/Article/details/gypzedtlw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.tarul.cn/Article/details/gxfhquhot.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.vehdjk.com/Article/details/gyciuvgiw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gejmgecfu.sHtML

[C07] 把函数作为参数传入
来源：http://wap.yfazqb.com/Article/details/girefhcyq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.vehdjk.com/Article/details/gnqixfofa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.epnwcf.com/Article/details/gmqxkagag.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.vehdjk.com/Article/details/gtbahtclg.sHtML

TS:   arr.map(String)
来源：http://3g.vehdjk.com/Article/details/gkdcerihu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fktsv.cn/Article/details/gqptluppu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.yfazqb.com/Article/details/gcxlmyzhs.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.yfazqb.com/Article/details/gqwwokcuw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.bbcook.cn/Article/details/gyxuyzvds.sHtML

[C08] 闭包
来源：http://www.m.share.yfazqb.com/Article/details/gdonmzlft.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.sjlbkw.cn/Article/details/gepdgdkoe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.epnwcf.com/Article/details/grrggkzgw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gpqqzpagk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gsncqmgqp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.yfazqb.com/Article/details/gdjcbqmoz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.vehdjk.com/Article/details/gpqizuvum.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.yfazqb.com/Article/details/gjqehvxnz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/grqmxnzbs.sHtML

[C09] 递归
来源：http://m.share.yfazqb.com/Article/details/gstuzybiq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/gnnqpwuht.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.yfazqb.com/Article/details/giwkssmbu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gdmquucry.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gajwihdpm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.tarul.cn/Article/details/ghmjtwovf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/gfitdlghl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gjlpncguq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.epnwcf.com/Article/details/gfkhpcych.sHtML

[C10] 变量作用域
来源：http://www.blog.fktsv.cn/Article/details/gixgmyolt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fktsv.cn/Article/details/ggvzmnxrc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fktsv.cn/Article/details/gczbgnmqe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.vehdjk.com/Article/details/gksujckcd.sHtML

TS:   同 JS
来源：http://baike.bbcook.cn/Article/details/gvwtkzlil.sHtML

Java: 方法内为块级作用域
来源：http://3g.fktsv.cn/Article/details/gldkrzrgr.sHtML

Go:   花括号块级作用域
来源：http://m.share.yfazqb.com/Article/details/gzyemqomd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.vehdjk.com/Article/details/gxweytixg.sHtML

C#:   块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gbgomocay.sHtML

[C11] 模块导入与导出
来源：http://www.blog.tarul.cn/Article/details/gzuiegdbi.sHtML

Py:   from module import func
来源：http://www.m.share.fktsv.cn/Article/details/gsrktehsv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fktsv.cn/Article/details/gsnroyzar.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gdjbeachc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.sjlbkw.cn/Article/details/gjxcwqeix.sHtML

Java: import java.util.List;
来源：http://www.blog.tarul.cn/Article/details/gzephlkoa.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.bbcook.cn/Article/details/gjietsocb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.epnwcf.com/Article/details/gdxmzrgnv.sHtML

C#:   using System.Text;
来源：http://baike.epnwcf.com/Article/details/gegijwbvt.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.bbcook.cn/Article/details/ggfjrvvwp.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fktsv.cn/Article/details/gsfjaazqc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.yfazqb.com/Article/details/gdnnnyjhr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gxoljvpti.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/gmfurujeg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnobmwab.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.epnwcf.com/Article/details/gmlvijqea.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fktsv.cn/Article/details/gmscrpvys.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.bbcook.cn/Article/details/gfylegbgx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.epnwcf.com/Article/details/gqueaqdez.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.vehdjk.com/Article/details/gemhqfkau.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gfcadyjgr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.bbcook.cn/Article/details/gdzpuckac.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gnjnhoflv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/glbufqfsw.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fktsv.cn/Article/details/gobvtoubv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.vehdjk.com/Article/details/gknoboasj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.yfazqb.com/Article/details/gxpfsgtcl.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/gxvmbwqna.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.bbcook.cn/Article/details/gxrnejbww.sHtML

PHP:  // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gamddyqhq.sHtML

JS:   // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gbaaponun.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.vehdjk.com/Article/details/gmuzddtqp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.vehdjk.com/Article/details/gisvtuuqt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.yfazqb.com/Article/details/gqyektdnn.sHtML

Ruby: # 无泛型
来源：http://mobile.vehdjk.com/Article/details/gnydyzqls.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.yfazqb.com/Article/details/gpebwmlsp.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlkgofbf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.tarul.cn/Article/details/gosimmasv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.sjlbkw.cn/Article/details/gwuacpgey.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/gkopfqdmc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.epnwcf.com/Article/details/getehmivw.sHtML

Java: // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/gjroxiamw.sHtML

Go:   // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/grzojyrjk.sHtML

Ruby: a, b = pair
来源：http://3g.fktsv.cn/Article/details/gujpnjdbd.sHtML

C#:   var (a, b) = pair;
来源：http://baike.epnwcf.com/Article/details/ggvrvmwmi.sHtML

[C16] 函数 / 方法重载
来源：http://blog.yfazqb.com/Article/details/gzakjepns.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.bbcook.cn/Article/details/gjhxwqpdg.sHtML

PHP:  // 无重载
来源：http://m.share.vehdjk.com/Article/details/gtdhyyzhm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.bbcook.cn/Article/details/gayxkutgh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.yfazqb.com/Article/details/gylgmxbif.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.epnwcf.com/Article/details/gesivkbbh.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.epnwcf.com/Article/details/glqiergwo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gurzcoqgd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.yfazqb.com/Article/details/gxbuwwmsa.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gscwnwlti.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.epnwcf.com/Article/details/gdvssrxlz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ghmtbcwva.sHtML

[D01] 创建数组 / 列表
来源：http://blog.tarul.cn/Article/details/gqsldirru.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.bbcook.cn/Article/details/gabfeeljf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.epnwcf.com/Article/details/gcrltqqst.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.vehdjk.com/Article/details/gostlpplx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.bbcook.cn/Article/details/gmmbovyhm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fktsv.cn/Article/details/gwmpzafva.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fktsv.cn/Article/details/gzjxxxkdw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.tarul.cn/Article/details/gvgzsdcrr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.vehdjk.com/Article/details/gwfpjzzcb.sHtML

[D02] 追加元素到末尾
来源：http://m.share.vehdjk.com/Article/details/gmyylxxcu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fktsv.cn/Article/details/gqrkaaedy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.epnwcf.com/Article/details/gmiwyrapx.sHtML

JS:   arr.push(4);
来源：http://www.blog.vehdjk.com/Article/details/golvtmtri.sHtML

TS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/gdfizalew.sHtML

Java: list.add(4);
来源：http://www.share.vehdjk.com/Article/details/glhtwdzil.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.epnwcf.com/Article/details/gagbwshvc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.vehdjk.com/Article/details/gfsdghuiu.sHtML

C#:   list.Add(4);
来源：http://mobile.bbcook.cn/Article/details/gxtjasedd.sHtML

[D03] 在指定位置插入元素
来源：http://baike.yfazqb.com/Article/details/gudiluvnq.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gzrxvrpll.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.bbcook.cn/Article/details/gfaczdrtr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.vehdjk.com/Article/details/gtxwggkju.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.epnwcf.com/Article/details/gnqjdzhhc.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gtdlygasc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.epnwcf.com/Article/details/gezwdioea.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.yfazqb.com/Article/details/gukepwvsv.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.tarul.cn/Article/details/gnqsjoaia.sHtML

[D04] 删除元素
来源：http://www.blog.vehdjk.com/Article/details/golekjnlo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.epnwcf.com/Article/details/gquqqzjhm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.yfazqb.com/Article/details/gdsiipelt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.yfazqb.com/Article/details/ggufufrbw.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.tarul.cn/Article/details/gnosejtzs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.tarul.cn/Article/details/gwpnepmwu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fktsv.cn/Article/details/gdaqogiyq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.epnwcf.com/Article/details/gnputpidc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.sjlbkw.cn/Article/details/greyfbpsn.sHtML

[D05] 访问与修改元素
来源：http://baike.epnwcf.com/Article/details/gkdmzgmri.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gnvgxkbbd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.epnwcf.com/Article/details/gzinbdftm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gckyunezz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/gnlaprdbl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.yfazqb.com/Article/details/gkcsyrdrm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gbuxifctq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gtippdego.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gjuvxpzxf.sHtML

[D06] 数组长度
来源：http://www.blog.fktsv.cn/Article/details/gqkqgjjhy.sHtML

Py:   len(arr)
来源：http://wap.epnwcf.com/Article/details/ghhdjzwgc.sHtML

PHP:  count($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gfnlnyuor.sHtML

JS:   arr.length
来源：http://baike.epnwcf.com/Article/details/gpixhjegj.sHtML

TS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/gclbdxvgu.sHtML

Java: list.size();
来源：http://baike.epnwcf.com/Article/details/gbckwfpxt.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gnzkekdao.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.yfazqb.com/Article/details/gkxfecbiq.sHtML

C#:   list.Count;
来源：http://m.share.yfazqb.com/Article/details/gbbrkssne.sHtML

[D07] 切片 / 取子数组
来源：http://blog.epnwcf.com/Article/details/ggorejtcv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.epnwcf.com/Article/details/gkahuspxk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.sjlbkw.cn/Article/details/gfgvwkhkv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gcfpeskpr.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gyhkyvktn.sHtML

Java: list.subList(1, 4);
来源：http://baike.vehdjk.com/Article/details/gidxfjchi.sHtML

Go:   arr[1:4]
来源：http://read.share.tarul.cn/Article/details/ghjckxwmk.sHtML

Ruby: arr[1, 3]
来源：http://mobile.tarul.cn/Article/details/gjtdutwpw.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.sjlbkw.cn/Article/details/guhshrqob.sHtML

[D08] 合并两个数组
来源：http://mobile.sjlbkw.cn/Article/details/gvxvtzubw.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fktsv.cn/Article/details/gbrjxiotp.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.tarul.cn/Article/details/gbkmxencr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.bbcook.cn/Article/details/gnouzsowu.sHtML

TS:   [...a, ...b];
来源：http://mobile.bbcook.cn/Article/details/gtxpvgxmk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.sjlbkw.cn/Article/details/ghnjglcja.sHtML

Go:   append(a, b...)
来源：http://www.m.share.sjlbkw.cn/Article/details/guecntblp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.sjlbkw.cn/Article/details/gceiihugo.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gqzzkgetd.sHtML

[D09] 排序（升序）
来源：http://www.blog.vehdjk.com/Article/details/gbwljpdth.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gvcwlharh.sHtML

PHP:  sort($arr);
来源：http://wap.fktsv.cn/Article/details/gagnkmkve.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.epnwcf.com/Article/details/gurpfrbod.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fktsv.cn/Article/details/gorxzmpkh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.epnwcf.com/Article/details/gckabpljr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gkmbotyjd.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/gruotdblf.sHtML

C#:   list.Sort();
来源：http://baike.yfazqb.com/Article/details/gowpieipd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.bbcook.cn/Article/details/gtauapxyk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fktsv.cn/Article/details/ghskqbegu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/gluxixjdc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gnyqcczhm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/grrwtpakt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fktsv.cn/Article/details/gjibdhhaj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.sjlbkw.cn/Article/details/ggsvcilyv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.bbcook.cn/Article/details/gduupgftl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.epnwcf.com/Article/details/gouiwnyyy.sHtML

[D11] 反转数组
来源：http://baike.sjlbkw.cn/Article/details/ginqswayx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fktsv.cn/Article/details/guwcszbbl.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fktsv.cn/Article/details/gpfpkdblw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fktsv.cn/Article/details/gahrysxwb.sHtML

TS:   [...arr].reverse();
来源：http://wap.yfazqb.com/Article/details/gkldipbeh.sHtML

Java: Collections.reverse(list);
来源：http://blog.tarul.cn/Article/details/gnjjkjgli.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.tarul.cn/Article/details/ggelldwey.sHtML

Ruby: arr.reverse
来源：http://wap.bbcook.cn/Article/details/gvxhvndhd.sHtML

C#:   list.Reverse();
来源：http://wap.sjlbkw.cn/Article/details/glcvucduc.sHtML

[D12] 查找元素下标
来源：http://www.blog.epnwcf.com/Article/details/gzupvfdxi.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.epnwcf.com/Article/details/glnsajpfk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gfdncuysx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gnudarojp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/gtykdiycy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.tarul.cn/Article/details/gfyqrwxpi.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.yfazqb.com/Article/details/giovbijzb.sHtML

Ruby: arr.index(x)
来源：http://www.blog.vehdjk.com/Article/details/geyckpqgr.sHtML

C#:   list.IndexOf(x);
来源：http://blog.tarul.cn/Article/details/gjhefnzuh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.epnwcf.com/Article/details/gutbmezoh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fktsv.cn/Article/details/ggtjrzmhz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.sjlbkw.cn/Article/details/gqjtmcjdl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.tarul.cn/Article/details/gucfrcxfr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.vehdjk.com/Article/details/gjzmmstij.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.yfazqb.com/Article/details/gizdznode.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.bbcook.cn/Article/details/gutunojal.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.epnwcf.com/Article/details/garjngtmm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gdtmklmgf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.bbcook.cn/Article/details/gcqfhduih.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fktsv.cn/Article/details/gvloqxpod.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.yfazqb.com/Article/details/guhzvpyxz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/gcnbozcda.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gjctpqdoq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/gmxgnbain.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/gpvltwsgv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.bbcook.cn/Article/details/gdogbrnbs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fktsv.cn/Article/details/gzqolzfhw.sHtML

[D15] 去重
来源：http://wap.yfazqb.com/Article/details/gjjqsyedw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.bbcook.cn/Article/details/glylqiglk.sHtML

PHP:  array_unique($arr);
来源：http://read.share.bbcook.cn/Article/details/gwwapajbu.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/gvgjcrywz.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gkqbmyeej.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.epnwcf.com/Article/details/gfrflgzjw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.tarul.cn/Article/details/glnpdyzak.sHtML

Ruby: arr.uniq
来源：http://wap.tarul.cn/Article/details/grvozcnib.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.yfazqb.com/Article/details/gttpgpfjf.sHtML

[D16] 求和与平均值
来源：http://www.share.vehdjk.com/Article/details/gmiqsxqlj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gdphxemcj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.tarul.cn/Article/details/gtqvganyt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gokmezqjq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/gvldqeavy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fktsv.cn/Article/details/gzlbawxkl.sHtML

Go:   // 手写循环累加
来源：http://baike.vehdjk.com/Article/details/gxqlisuok.sHtML


<!-- 参考信息 -->