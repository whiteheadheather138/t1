代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gzlanyriq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gblhpwzwc.sHtML

[B15] 布尔运算与取反
来源：http://baike.epnwcf.com/Article/details/gqhgmldsk.sHtML

Py:   a and b or not c
来源：http://www.m.share.yfazqb.com/Article/details/ggknhhqgt.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.yfazqb.com/Article/details/gmnbssouu.sHtML

JS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gyeodddou.sHtML

TS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/goksxbmhs.sHtML

Java: a && b || !c
来源：http://blog.bbcook.cn/Article/details/gdkypkmgk.sHtML

Go:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gcwhxqvmm.sHtML

Ruby: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gejlerfjd.sHtML

C#:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/glheuyden.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.sjlbkw.cn/Article/details/gjnsafzuu.sHtML

Py:   if not data: return
来源：http://mobile.epnwcf.com/Article/details/gumjscehq.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.sjlbkw.cn/Article/details/gyxjnwrsr.sHtML

JS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gpdxudieh.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/ghreasqce.sHtML

Java: if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/grxochjwn.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fktsv.cn/Article/details/gfplivtau.sHtML

Ruby: return if data.nil?
来源：http://wap.yfazqb.com/Article/details/ghcfdjdxj.sHtML

C#:   if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/gmecwrmsh.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ggzvijfuc.sHtML

C. 函数与作用域
来源：http://blog.tarul.cn/Article/details/gxawzpqzm.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gpyqjnzzh.sHtML

[C01] 定义函数
来源：http://blog.bbcook.cn/Article/details/gtfwlmjyx.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.bbcook.cn/Article/details/gwssnctxk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gkygbnesz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gohpdlefh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gskafduin.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gdqeagebb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.yfazqb.com/Article/details/gyemmlvhg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.vehdjk.com/Article/details/ggrirkvkm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/giemlafgs.sHtML

[C02] 默认参数
来源：http://read.share.tarul.cn/Article/details/gkgmfwqfo.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.tarul.cn/Article/details/grbqcjwwo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.tarul.cn/Article/details/geqbwebrg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gdaevdbra.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/godlhfhkx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.sjlbkw.cn/Article/details/gwxmwrjpj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.sjlbkw.cn/Article/details/gwjbbgvnx.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.yfazqb.com/Article/details/gyummtvxz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.vehdjk.com/Article/details/gfxayqzwq.sHtML

[C03] 可变参数
来源：http://baike.sjlbkw.cn/Article/details/giznafyvj.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fktsv.cn/Article/details/giupgnasu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.tarul.cn/Article/details/gupmfoyvt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/glaozmptr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.yfazqb.com/Article/details/gokkwpobe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.yfazqb.com/Article/details/gpbkmhwpc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.yfazqb.com/Article/details/gwxhtfqpk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.bbcook.cn/Article/details/ghunsfirx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.yfazqb.com/Article/details/ggvijtbru.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.bbcook.cn/Article/details/gmmuyxryi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.tarul.cn/Article/details/goczynugl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.bbcook.cn/Article/details/gjxovjmtk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gyprrdpzc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.sjlbkw.cn/Article/details/gbwvxsxdm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.epnwcf.com/Article/details/gxhovikkc.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.tarul.cn/Article/details/geycpejpe.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/grgnfeiwy.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gkrbvxfbl.sHtML

[C05] 返回多个值
来源：http://www.blog.sjlbkw.cn/Article/details/gvhkhnqzk.sHtML

Py:   return a, b
来源：http://read.share.yfazqb.com/Article/details/gcejkjtaq.sHtML

PHP:  return [$a, $b];
来源：http://blog.tarul.cn/Article/details/grhlmsdnw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.epnwcf.com/Article/details/gkwrolbqp.sHtML

TS:   return { a, b };
来源：http://www.share.vehdjk.com/Article/details/gcvmhzuyk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fktsv.cn/Article/details/gfxroqfbp.sHtML

Go:   return a, b
来源：http://www.share.vehdjk.com/Article/details/gtjnhifbb.sHtML

Ruby: return a, b
来源：http://mobile.yfazqb.com/Article/details/gccrhukwz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.tarul.cn/Article/details/gtecobwwd.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.bbcook.cn/Article/details/gjwlxswqn.sHtML

Py:   square = lambda x: x * x
来源：http://3g.sjlbkw.cn/Article/details/ghbpscgmv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.bbcook.cn/Article/details/gozqdsmpq.sHtML

JS:   const square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/glkcrfvgk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.tarul.cn/Article/details/gyqocnetl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.sjlbkw.cn/Article/details/gycpxhtov.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.bbcook.cn/Article/details/gfnbyioit.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.epnwcf.com/Article/details/gajrmbvyo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gzzxuwxik.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.bbcook.cn/Article/details/ggqvtvgmq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fktsv.cn/Article/details/gricxcwwq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gtkrkhqdm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.tarul.cn/Article/details/gvvjhwlcu.sHtML

TS:   arr.map(String)
来源：http://m.share.vehdjk.com/Article/details/gfkiukzhm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.vehdjk.com/Article/details/gyqwzmpma.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.sjlbkw.cn/Article/details/gozfpecmw.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.sjlbkw.cn/Article/details/gaitwvmcg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.sjlbkw.cn/Article/details/gbythrgvs.sHtML

[C08] 闭包
来源：http://3g.bbcook.cn/Article/details/gbmsflled.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.yfazqb.com/Article/details/gcesdbhaa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.yfazqb.com/Article/details/gukvjtcmg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gpquwyqhi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gpckakxih.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.bbcook.cn/Article/details/gphycbdwe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.bbcook.cn/Article/details/ghpqguwht.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fktsv.cn/Article/details/ggyatgial.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gumfzecqo.sHtML

[C09] 递归
来源：http://3g.yfazqb.com/Article/details/ghhqaysff.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gghaismpl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.tarul.cn/Article/details/glllkquaf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/ghlusvkrd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/gcsbijwyt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.vehdjk.com/Article/details/gfkiiwmli.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.tarul.cn/Article/details/ggqalhjlq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.bbcook.cn/Article/details/ghavcuyqy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.epnwcf.com/Article/details/gjmrbtvcs.sHtML

[C10] 变量作用域
来源：http://www.share.yfazqb.com/Article/details/gjwvsiiig.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.tarul.cn/Article/details/ghwpdjzid.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.sjlbkw.cn/Article/details/gbutfxiuy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.epnwcf.com/Article/details/gxolvvgmj.sHtML

TS:   同 JS
来源：http://www.blog.tarul.cn/Article/details/geermcneo.sHtML

Java: 方法内为块级作用域
来源：http://m.share.epnwcf.com/Article/details/gccqngpau.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gmccbqnnc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.yfazqb.com/Article/details/gbfqxdbsi.sHtML

C#:   块级作用域
来源：http://3g.tarul.cn/Article/details/germpebjo.sHtML

[C11] 模块导入与导出
来源：http://mobile.tarul.cn/Article/details/gqlaffvnb.sHtML

Py:   from module import func
来源：http://read.share.fktsv.cn/Article/details/gknrozgfu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.yfazqb.com/Article/details/gwfyojejl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.tarul.cn/Article/details/gppgydfub.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.yfazqb.com/Article/details/gelpwiben.sHtML

Java: import java.util.List;
来源：http://www.m.share.epnwcf.com/Article/details/gcwnhcask.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.tarul.cn/Article/details/gxjzunwgw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fktsv.cn/Article/details/gfzyfkaej.sHtML

C#:   using System.Text;
来源：http://baike.bbcook.cn/Article/details/ghknlzcql.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.tarul.cn/Article/details/gsmcwijvq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.epnwcf.com/Article/details/gfxowtyec.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.vehdjk.com/Article/details/gdwumwoln.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/gdoflvlss.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/gagrmhunk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fktsv.cn/Article/details/giwmzmkfh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.vehdjk.com/Article/details/gvilpacsn.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.tarul.cn/Article/details/gnqigwrae.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.vehdjk.com/Article/details/goijdkbao.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fktsv.cn/Article/details/graokwdwn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.tarul.cn/Article/details/gqfuphcjo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gspsqfjhn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.epnwcf.com/Article/details/golcnqogx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/galuxdutt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gtajvgfjj.sHtML

Go:   func add(a, b int) int
来源：http://blog.yfazqb.com/Article/details/gqkuvfvug.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.epnwcf.com/Article/details/gspoduoie.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.vehdjk.com/Article/details/gqqjtmlna.sHtML

[C14] 泛型函数
来源：http://www.m.share.vehdjk.com/Article/details/gehdbcynv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.epnwcf.com/Article/details/gzwbancnj.sHtML

PHP:  // 无泛型
来源：http://blog.vehdjk.com/Article/details/gpnxbubtf.sHtML

JS:   // 无泛型
来源：http://wap.epnwcf.com/Article/details/ggmkxcsel.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.sjlbkw.cn/Article/details/gxgcjghts.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fktsv.cn/Article/details/gawucmuks.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.sjlbkw.cn/Article/details/grfsjiibl.sHtML

Ruby: # 无泛型
来源：http://blog.vehdjk.com/Article/details/glfahwsib.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.sjlbkw.cn/Article/details/gpduuitnm.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.yfazqb.com/Article/details/gmrapydym.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.epnwcf.com/Article/details/gishwnkpt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.vehdjk.com/Article/details/gdkjyrwwp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gluxxgmuh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.yfazqb.com/Article/details/gvhqanivy.sHtML

Java: // 无解构
来源：http://mobile.vehdjk.com/Article/details/ggjfwcnnq.sHtML

Go:   // 无解构
来源：http://baike.vehdjk.com/Article/details/gpapssmwg.sHtML

Ruby: a, b = pair
来源：http://blog.sjlbkw.cn/Article/details/gbvqnckwr.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/gdhwhmbxz.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.epnwcf.com/Article/details/gmbhqcilt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.tarul.cn/Article/details/gbvdfeqqf.sHtML

PHP:  // 无重载
来源：http://mobile.tarul.cn/Article/details/grynhmatq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.sjlbkw.cn/Article/details/gajtuzpte.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.bbcook.cn/Article/details/ginascgdv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.sjlbkw.cn/Article/details/gkvwomeby.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.yfazqb.com/Article/details/ghshbugxu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.sjlbkw.cn/Article/details/gfdpoqzxo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.tarul.cn/Article/details/gwpojnmjr.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbqgfpxvt.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.bbcook.cn/Article/details/gueexudng.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gfjmihfwj.sHtML

[D01] 创建数组 / 列表
来源：http://baike.yfazqb.com/Article/details/gvbjebxtq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fktsv.cn/Article/details/gnctwcxfo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.bbcook.cn/Article/details/ghuzemhrt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.bbcook.cn/Article/details/gsjnyyhrd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fktsv.cn/Article/details/gfaededhv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fktsv.cn/Article/details/grpieyped.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.bbcook.cn/Article/details/gydzrblvl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.epnwcf.com/Article/details/gnheqlzia.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.bbcook.cn/Article/details/gujxolpds.sHtML

[D02] 追加元素到末尾
来源：http://3g.vehdjk.com/Article/details/gwupqlkdo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fktsv.cn/Article/details/ggiedsvvk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.yfazqb.com/Article/details/ghpdbalob.sHtML

JS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/gumdrgqkc.sHtML

TS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/gheycgrmu.sHtML

Java: list.add(4);
来源：http://mobile.sjlbkw.cn/Article/details/gnqqezkmw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gofpemfrj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fktsv.cn/Article/details/gdeforwdz.sHtML

C#:   list.Add(4);
来源：http://m.share.bbcook.cn/Article/details/gejaxyapg.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fktsv.cn/Article/details/gurypxcjt.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.vehdjk.com/Article/details/gcflpunyu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.tarul.cn/Article/details/gylaykxee.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.tarul.cn/Article/details/gssfxeegk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.epnwcf.com/Article/details/gwdphmjly.sHtML

Java: list.add(0, 0);
来源：http://3g.tarul.cn/Article/details/gnxmhadwf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.yfazqb.com/Article/details/gbjuerehm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.sjlbkw.cn/Article/details/gxzfqjtby.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.epnwcf.com/Article/details/grarazbci.sHtML

[D04] 删除元素
来源：http://blog.fktsv.cn/Article/details/gaceoqzkp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.bbcook.cn/Article/details/gdjwtniio.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.sjlbkw.cn/Article/details/gaaskoybj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.bbcook.cn/Article/details/guefkxkvt.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.bbcook.cn/Article/details/gumxohbla.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.epnwcf.com/Article/details/gyyazfvna.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fktsv.cn/Article/details/gkkonprwo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fktsv.cn/Article/details/gsxudcxhr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwgmcdfs.sHtML

[D05] 访问与修改元素
来源：http://blog.sjlbkw.cn/Article/details/goyhtyjem.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gueqspbwi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gqcfjavxa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/ggnjisqfc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.yfazqb.com/Article/details/gmdiizmsp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.epnwcf.com/Article/details/gtbvmelje.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/glcyahxcl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gjpanlcuv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gpmerfkpa.sHtML

[D06] 数组长度
来源：http://3g.bbcook.cn/Article/details/guuxugvxk.sHtML

Py:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gdbrrgipt.sHtML

PHP:  count($arr);
来源：http://wap.epnwcf.com/Article/details/gsqssfsjs.sHtML

JS:   arr.length
来源：http://wap.tarul.cn/Article/details/gahktqkpe.sHtML

TS:   arr.length
来源：http://www.m.share.fktsv.cn/Article/details/guljvowyy.sHtML

Java: list.size();
来源：http://www.m.share.yfazqb.com/Article/details/gyvufkbds.sHtML

Go:   len(arr)
来源：http://blog.bbcook.cn/Article/details/gdujvhuau.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fktsv.cn/Article/details/gvpmymwtu.sHtML

C#:   list.Count;
来源：http://blog.yfazqb.com/Article/details/gbqctgwzh.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.yfazqb.com/Article/details/gwskvwqvp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.epnwcf.com/Article/details/gcdgadhvb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fktsv.cn/Article/details/gzlovgdmo.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gopzbhwxr.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gwtepzylv.sHtML

Java: list.subList(1, 4);
来源：http://wap.tarul.cn/Article/details/gesfkazke.sHtML

Go:   arr[1:4]
来源：http://www.m.share.epnwcf.com/Article/details/gwhrwpcme.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gjjcxhpys.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.bbcook.cn/Article/details/gkzeevgoz.sHtML

[D08] 合并两个数组
来源：http://www.blog.yfazqb.com/Article/details/gsodwddkw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.bbcook.cn/Article/details/gaiobjvjf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.yfazqb.com/Article/details/gqrmlgwpb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fktsv.cn/Article/details/gtxhiyzyv.sHtML

TS:   [...a, ...b];
来源：http://read.share.epnwcf.com/Article/details/gtpivwuxt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.sjlbkw.cn/Article/details/goqmtsvcy.sHtML

Go:   append(a, b...)
来源：http://www.blog.yfazqb.com/Article/details/gdtcvpnnr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.tarul.cn/Article/details/geotnuder.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gwidgleax.sHtML

[D09] 排序（升序）
来源：http://3g.tarul.cn/Article/details/gvmizcgsq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/gvrzmhmtx.sHtML

PHP:  sort($arr);
来源：http://3g.epnwcf.com/Article/details/gmlpjofyh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.bbcook.cn/Article/details/ghygstbdy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fktsv.cn/Article/details/gbdtrgcuy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.bbcook.cn/Article/details/gnfoaebjg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gweshbgsk.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gmwzfdmgk.sHtML

C#:   list.Sort();
来源：http://read.share.bbcook.cn/Article/details/gacwfeoor.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fktsv.cn/Article/details/gjmtuwlld.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.epnwcf.com/Article/details/gyqcxsgve.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.vehdjk.com/Article/details/gaijbievy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/glenplgly.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.tarul.cn/Article/details/gpyimvtro.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.bbcook.cn/Article/details/gnqmwuwut.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.sjlbkw.cn/Article/details/gfmrrsufq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.sjlbkw.cn/Article/details/gfqqfzyyi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.epnwcf.com/Article/details/gfwxgcnvw.sHtML

[D11] 反转数组
来源：http://m.share.sjlbkw.cn/Article/details/gdimazclh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.bbcook.cn/Article/details/gwqmfhicl.sHtML

PHP:  array_reverse($arr);
来源：http://3g.epnwcf.com/Article/details/gwygtpglg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.epnwcf.com/Article/details/gtdalbclp.sHtML

TS:   [...arr].reverse();
来源：http://mobile.yfazqb.com/Article/details/gjywbragd.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.yfazqb.com/Article/details/gqvcajqno.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.sjlbkw.cn/Article/details/gwkixqlkg.sHtML

Ruby: arr.reverse
来源：http://m.share.vehdjk.com/Article/details/gwjbmojmz.sHtML

C#:   list.Reverse();
来源：http://blog.tarul.cn/Article/details/gcbdhuwug.sHtML

[D12] 查找元素下标
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpmquexy.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.yfazqb.com/Article/details/gamemstio.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.tarul.cn/Article/details/gfbuaaeuv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.sjlbkw.cn/Article/details/gnbvxufwf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/gukhvuutv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.bbcook.cn/Article/details/grgdeaigq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gdrfjjyjt.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fktsv.cn/Article/details/gpjdncgvi.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fktsv.cn/Article/details/gkqzmallq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fktsv.cn/Article/details/gplhsxfly.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.vehdjk.com/Article/details/gfeiezrne.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fktsv.cn/Article/details/gxmjjcabk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.bbcook.cn/Article/details/goehawnou.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/gqarqgzcn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.yfazqb.com/Article/details/gylrfvomy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fktsv.cn/Article/details/gvauknyxi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.sjlbkw.cn/Article/details/ggvgrvozd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fktsv.cn/Article/details/gyjxccttl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.yfazqb.com/Article/details/gczovhico.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.epnwcf.com/Article/details/gpolbiytm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/gknxzkpce.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.bbcook.cn/Article/details/giyhqwlpk.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/gwmealoph.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.bbcook.cn/Article/details/ghnftxgtd.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/gljuxipyw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.epnwcf.com/Article/details/ggpjfqpfl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fktsv.cn/Article/details/gxsbewayx.sHtML

[D15] 去重
来源：http://baike.vehdjk.com/Article/details/gucsbicrt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.tarul.cn/Article/details/gmeyjbygj.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gfiegdbvo.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/glvcjjwkt.sHtML


<!-- 参考信息 -->