代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.vehdjk.com/Article/details/gnkawgqmn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gjzjqvrtr.sHtML

[B15] 布尔运算与取反
来源：http://read.share.vehdjk.com/Article/details/gudnmaklo.sHtML

Py:   a and b or not c
来源：http://www.share.sjlbkw.cn/Article/details/gvfjuworj.sHtML

PHP:  $a && $b || !$c
来源：http://3g.epnwcf.com/Article/details/gogdfhntl.sHtML

JS:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gmetsstrt.sHtML

TS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gahcmzemt.sHtML

Java: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gazyylvxn.sHtML

Go:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gbfhieejp.sHtML

Ruby: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gpegboujo.sHtML

C#:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/goqhiacuf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.tarul.cn/Article/details/gskiydrgs.sHtML

Py:   if not data: return
来源：http://www.m.share.sjlbkw.cn/Article/details/gcinfrucm.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.sjlbkw.cn/Article/details/gcskzwvoq.sHtML

JS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/gmfygxrch.sHtML

TS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gdyuxcelf.sHtML

Java: if (data == null) return;
来源：http://www.share.tarul.cn/Article/details/gxjpdhwzq.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fktsv.cn/Article/details/gzgspbupr.sHtML

Ruby: return if data.nil?
来源：http://blog.tarul.cn/Article/details/glgnztysp.sHtML

C#:   if (data == null) return;
来源：http://baike.yfazqb.com/Article/details/gongjkkya.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwteveqmy.sHtML

C. 函数与作用域
来源：http://blog.epnwcf.com/Article/details/ggbvuimck.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gdlnnrysx.sHtML

[C01] 定义函数
来源：http://read.share.vehdjk.com/Article/details/gzmzofgxk.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.sjlbkw.cn/Article/details/gackxastr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gmwloyvmn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gxwlpdrqs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gqpfytmfr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/ggmbdsxky.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fktsv.cn/Article/details/gaeiwvhcx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.vehdjk.com/Article/details/gifujglpw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gqfrnpchf.sHtML

[C02] 默认参数
来源：http://wap.sjlbkw.cn/Article/details/gywqinwqa.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.yfazqb.com/Article/details/goexnppwk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.sjlbkw.cn/Article/details/ghvuotpnw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gypgvtwgh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/ghpizjkwq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.vehdjk.com/Article/details/glnfpgfmm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.yfazqb.com/Article/details/gxenglrej.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.vehdjk.com/Article/details/gowmnsrud.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fktsv.cn/Article/details/gmxmsvxkh.sHtML

[C03] 可变参数
来源：http://mobile.vehdjk.com/Article/details/gsxlrjbxk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.tarul.cn/Article/details/gvnanviwx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fktsv.cn/Article/details/gcwhcxovd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.yfazqb.com/Article/details/gqpnapyzt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gdrhmfwgv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.tarul.cn/Article/details/gxqrkpnhx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.sjlbkw.cn/Article/details/glxixxnoz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.bbcook.cn/Article/details/guwtezlst.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.epnwcf.com/Article/details/gzsfrvmxb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.sjlbkw.cn/Article/details/gulzptrna.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.vehdjk.com/Article/details/gipvlsrvg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.bbcook.cn/Article/details/gqempcbld.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gbrdggubj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.epnwcf.com/Article/details/gystdyrzx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfrufqmx.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.yfazqb.com/Article/details/gklatrbkh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/ggykavlse.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/grkxefbda.sHtML

[C05] 返回多个值
来源：http://www.m.share.yfazqb.com/Article/details/gpyqgakzx.sHtML

Py:   return a, b
来源：http://read.share.sjlbkw.cn/Article/details/gttrnmfym.sHtML

PHP:  return [$a, $b];
来源：http://3g.yfazqb.com/Article/details/gbzadmhnh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.epnwcf.com/Article/details/gsymkwiom.sHtML

TS:   return { a, b };
来源：http://wap.tarul.cn/Article/details/glpbihrsu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fktsv.cn/Article/details/gfyhbnfus.sHtML

Go:   return a, b
来源：http://www.blog.tarul.cn/Article/details/gmcvvdffu.sHtML

Ruby: return a, b
来源：http://baike.fktsv.cn/Article/details/gnowyftoy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.epnwcf.com/Article/details/geregiebp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gckqabsai.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.vehdjk.com/Article/details/gutgzswvd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.bbcook.cn/Article/details/ghusrefqp.sHtML

JS:   const square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/glflaiwcp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fktsv.cn/Article/details/gkieoqnfs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.yfazqb.com/Article/details/gcbappqej.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.epnwcf.com/Article/details/gbtnogxmi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.vehdjk.com/Article/details/gqntfdwlq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/gnxscaqqc.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fktsv.cn/Article/details/golqvpthc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.epnwcf.com/Article/details/grnfmreno.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fktsv.cn/Article/details/gdsqxcvpu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.tarul.cn/Article/details/gadgvmmdc.sHtML

TS:   arr.map(String)
来源：http://blog.epnwcf.com/Article/details/gmytllitp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.yfazqb.com/Article/details/gkbmdgpix.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.bbcook.cn/Article/details/gqrmlshrc.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.bbcook.cn/Article/details/gvfgqjehp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.epnwcf.com/Article/details/gcwjhgbsq.sHtML

[C08] 闭包
来源：http://www.m.share.tarul.cn/Article/details/gakhmluuo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.epnwcf.com/Article/details/gohvlmang.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.tarul.cn/Article/details/gqlygkcwe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/grahruvgf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gcjisddmo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/ghcsizqin.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.epnwcf.com/Article/details/gcxzhpbzy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.vehdjk.com/Article/details/gofxklfod.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gouheljok.sHtML

[C09] 递归
来源：http://blog.yfazqb.com/Article/details/gprtpsyaz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/glkvefvnv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.yfazqb.com/Article/details/gaujdjtmi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/gkbyngwyj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/gohumcxcw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.tarul.cn/Article/details/ggxneiqyv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.epnwcf.com/Article/details/glsphpiiq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/ggrlfgcww.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.epnwcf.com/Article/details/gtfygzohm.sHtML

[C10] 变量作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gdwulfuoi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.sjlbkw.cn/Article/details/gndmplpyb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.epnwcf.com/Article/details/gcthdjeql.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fktsv.cn/Article/details/gtfrtlajq.sHtML

TS:   同 JS
来源：http://mobile.epnwcf.com/Article/details/grlkcrqja.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gdnpcxnde.sHtML

Go:   花括号块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gatrrgegi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.bbcook.cn/Article/details/geeyoyxtm.sHtML

C#:   块级作用域
来源：http://mobile.fktsv.cn/Article/details/gykzvmemh.sHtML

[C11] 模块导入与导出
来源：http://3g.sjlbkw.cn/Article/details/gxojrreym.sHtML

Py:   from module import func
来源：http://wap.bbcook.cn/Article/details/gnwzscedw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.sjlbkw.cn/Article/details/gkaexfkqs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.tarul.cn/Article/details/gggykblyb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.sjlbkw.cn/Article/details/geeiabfez.sHtML

Java: import java.util.List;
来源：http://www.share.fktsv.cn/Article/details/gpofeoiec.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.vehdjk.com/Article/details/gpwmpaagm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.yfazqb.com/Article/details/gbhmisixh.sHtML

C#:   using System.Text;
来源：http://m.share.epnwcf.com/Article/details/gxzmtujlu.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.epnwcf.com/Article/details/gnmcmwiui.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fktsv.cn/Article/details/grjukwhhb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.epnwcf.com/Article/details/gijvqccyp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.epnwcf.com/Article/details/gbbqqkaws.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.vehdjk.com/Article/details/gijktuhac.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.tarul.cn/Article/details/guevnjrfw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.tarul.cn/Article/details/goquickmz.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.sjlbkw.cn/Article/details/gmmwjqbsl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.yfazqb.com/Article/details/gdvjqhzop.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.vehdjk.com/Article/details/grljahkse.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.epnwcf.com/Article/details/gieugxigl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gdlrilqgc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.epnwcf.com/Article/details/gfowsxrpc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gcldaloiq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gnnfofstq.sHtML

Go:   func add(a, b int) int
来源：http://wap.epnwcf.com/Article/details/ghiuhlszo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.yfazqb.com/Article/details/gtvpgaclu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.sjlbkw.cn/Article/details/gswkfmkfi.sHtML

[C14] 泛型函数
来源：http://www.m.share.yfazqb.com/Article/details/gokhxpwvj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fktsv.cn/Article/details/gfocmnbok.sHtML

PHP:  // 无泛型
来源：http://m.share.tarul.cn/Article/details/gsmypnuzd.sHtML

JS:   // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gjfibbhcl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.epnwcf.com/Article/details/gspsjiubt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.sjlbkw.cn/Article/details/gfvvdfdsu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.yfazqb.com/Article/details/gcoaadozu.sHtML

Ruby: # 无泛型
来源：http://read.share.yfazqb.com/Article/details/giwuviymw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.vehdjk.com/Article/details/gvifxgxtp.sHtML

[C15] 解构 / 展开参数
来源：http://wap.bbcook.cn/Article/details/gajzkcphw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.epnwcf.com/Article/details/gybumptkw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.vehdjk.com/Article/details/ghwudwyqo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfnhfsex.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.yfazqb.com/Article/details/gvcpkgyzj.sHtML

Java: // 无解构
来源：http://3g.fktsv.cn/Article/details/gvfqkwwph.sHtML

Go:   // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gghsewphp.sHtML

Ruby: a, b = pair
来源：http://m.share.bbcook.cn/Article/details/gbeikjiuj.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/gugtfomwb.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.vehdjk.com/Article/details/gprkhmfva.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.vehdjk.com/Article/details/gllrcmpym.sHtML

PHP:  // 无重载
来源：http://baike.epnwcf.com/Article/details/glbvtjxcz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.bbcook.cn/Article/details/gqhqacgmc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.sjlbkw.cn/Article/details/gngmpteap.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.tarul.cn/Article/details/gqqwvrrcx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.bbcook.cn/Article/details/gndmvothg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.tarul.cn/Article/details/gdewwnmer.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.yfazqb.com/Article/details/ghelvcgwq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/goecymrof.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.sjlbkw.cn/Article/details/gjkgdgbir.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/giiopjihf.sHtML

[D01] 创建数组 / 列表
来源：http://baike.vehdjk.com/Article/details/gbxmltbkc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.epnwcf.com/Article/details/gghjgkeez.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.vehdjk.com/Article/details/grmmqetxz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fktsv.cn/Article/details/gdkzqutxm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fktsv.cn/Article/details/gktsskbdp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.bbcook.cn/Article/details/gqqyldaix.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.yfazqb.com/Article/details/gfatlnvvx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fktsv.cn/Article/details/gxzxuweaj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.yfazqb.com/Article/details/gdulhoruk.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.epnwcf.com/Article/details/gcivxnvvy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.tarul.cn/Article/details/giownqult.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fktsv.cn/Article/details/gbdrveuyk.sHtML

JS:   arr.push(4);
来源：http://baike.vehdjk.com/Article/details/gksssonlg.sHtML

TS:   arr.push(4);
来源：http://mobile.epnwcf.com/Article/details/ggprgiuov.sHtML

Java: list.add(4);
来源：http://wap.vehdjk.com/Article/details/gzaouyzbo.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.bbcook.cn/Article/details/ggooutirc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.epnwcf.com/Article/details/gefrbjuec.sHtML

C#:   list.Add(4);
来源：http://wap.bbcook.cn/Article/details/gjytcwebj.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.bbcook.cn/Article/details/gxldprbau.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gfrqtbvzm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.yfazqb.com/Article/details/gtftojhej.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.sjlbkw.cn/Article/details/gjuozhjvf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.tarul.cn/Article/details/grjnyyulz.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gemykhith.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.yfazqb.com/Article/details/gncbugkos.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbheaivcl.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.yfazqb.com/Article/details/gdpuhiqxa.sHtML

[D04] 删除元素
来源：http://wap.epnwcf.com/Article/details/gzjjpiecg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.vehdjk.com/Article/details/gqqyjkuoo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.tarul.cn/Article/details/gdxcdebag.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.epnwcf.com/Article/details/gdfqlwyxb.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.yfazqb.com/Article/details/gpywgfnzw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.bbcook.cn/Article/details/gdrsfuvcr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.bbcook.cn/Article/details/gvzshinso.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.sjlbkw.cn/Article/details/goadvoadv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.vehdjk.com/Article/details/glqcwpeln.sHtML

[D05] 访问与修改元素
来源：http://blog.fktsv.cn/Article/details/goqvumpjp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gfhajghvn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fktsv.cn/Article/details/gvhkvnmhv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.yfazqb.com/Article/details/gdfikgulo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.sjlbkw.cn/Article/details/gpwhjbbbh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.epnwcf.com/Article/details/gwnpbnfty.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gknyznaqw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gxxsunxck.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fktsv.cn/Article/details/gbgqywyow.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/glskmmwsh.sHtML

Py:   len(arr)
来源：http://www.blog.fktsv.cn/Article/details/glhjytwac.sHtML

PHP:  count($arr);
来源：http://blog.sjlbkw.cn/Article/details/gbrlmwibt.sHtML

JS:   arr.length
来源：http://www.share.yfazqb.com/Article/details/gmzurjgew.sHtML

TS:   arr.length
来源：http://m.share.sjlbkw.cn/Article/details/gvvrbohwk.sHtML

Java: list.size();
来源：http://baike.sjlbkw.cn/Article/details/gqmrhmmhl.sHtML

Go:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gnqtaqzgb.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.bbcook.cn/Article/details/gnctypsgq.sHtML

C#:   list.Count;
来源：http://www.m.share.yfazqb.com/Article/details/gvcranyog.sHtML

[D07] 切片 / 取子数组
来源：http://3g.epnwcf.com/Article/details/grgqvkfgc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.epnwcf.com/Article/details/ghbfffubm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.tarul.cn/Article/details/gxafydvjp.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/gkklerzqr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gkwjkrwys.sHtML

Java: list.subList(1, 4);
来源：http://blog.epnwcf.com/Article/details/gnmuxvyiq.sHtML

Go:   arr[1:4]
来源：http://mobile.sjlbkw.cn/Article/details/gmewfsleo.sHtML

Ruby: arr[1, 3]
来源：http://m.share.bbcook.cn/Article/details/gfgwvpgax.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.yfazqb.com/Article/details/gjpmruthf.sHtML

[D08] 合并两个数组
来源：http://wap.yfazqb.com/Article/details/guwjfyant.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.bbcook.cn/Article/details/gxygfjvxc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.yfazqb.com/Article/details/gqtffaosm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.yfazqb.com/Article/details/gtzepzmlk.sHtML

TS:   [...a, ...b];
来源：http://mobile.tarul.cn/Article/details/gqydsjokb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.sjlbkw.cn/Article/details/gmmppqtqh.sHtML

Go:   append(a, b...)
来源：http://www.share.epnwcf.com/Article/details/gscygsyld.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.tarul.cn/Article/details/giqfmwxax.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.tarul.cn/Article/details/gkqbcivlh.sHtML

[D09] 排序（升序）
来源：http://wap.bbcook.cn/Article/details/gdgqfswlo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/gbrduaavb.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gtzosvzub.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.vehdjk.com/Article/details/gwvnoqfku.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.vehdjk.com/Article/details/gmuoivvvz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.yfazqb.com/Article/details/grsntofth.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gzawhonyy.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gglzesmvc.sHtML

C#:   list.Sort();
来源：http://read.share.sjlbkw.cn/Article/details/glafmhjsw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.tarul.cn/Article/details/glasbcpzd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.tarul.cn/Article/details/gcgwwmsbm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/glxzqbnok.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.tarul.cn/Article/details/gziymfnpt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/gthuqbmqo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.bbcook.cn/Article/details/ghafovyxh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gptflnpeg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.epnwcf.com/Article/details/gmmsejdem.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.vehdjk.com/Article/details/gnucrkthp.sHtML

[D11] 反转数组
来源：http://www.share.tarul.cn/Article/details/gqpfnwyhc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.yfazqb.com/Article/details/gzkfgbahg.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.tarul.cn/Article/details/gjsljuame.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fktsv.cn/Article/details/ghjsdbisj.sHtML

TS:   [...arr].reverse();
来源：http://3g.fktsv.cn/Article/details/gepxnohtv.sHtML

Java: Collections.reverse(list);
来源：http://mobile.vehdjk.com/Article/details/gjwfulvoj.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.yfazqb.com/Article/details/gjwlqsaux.sHtML

Ruby: arr.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gpwrxntdz.sHtML

C#:   list.Reverse();
来源：http://www.m.share.epnwcf.com/Article/details/gwwvxzuuu.sHtML

[D12] 查找元素下标
来源：http://m.share.fktsv.cn/Article/details/gowvnkeun.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.vehdjk.com/Article/details/gyehvprhs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.epnwcf.com/Article/details/gwuvlxwsr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/gsknzsupo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/glkgboqkd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.vehdjk.com/Article/details/gzyymshgh.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gtatotnsr.sHtML

Ruby: arr.index(x)
来源：http://read.share.sjlbkw.cn/Article/details/gwfvgrura.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.epnwcf.com/Article/details/geqkoesbp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/gtgdnpeif.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fktsv.cn/Article/details/gdppfgxpv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.yfazqb.com/Article/details/ggsuugico.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gqyqqqdwv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.yfazqb.com/Article/details/grmwfmpuq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.epnwcf.com/Article/details/gbcftjofk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.tarul.cn/Article/details/gzhwvojaw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fktsv.cn/Article/details/gtyaepgcn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.tarul.cn/Article/details/gsxsuaoqu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.epnwcf.com/Article/details/gifhctuco.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gmswiykoz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/guxhknexj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.epnwcf.com/Article/details/gitmiwkvu.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gvtxvypeb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fktsv.cn/Article/details/gzyxyzazn.sHtML

Go:   // 手写循环
来源：http://blog.yfazqb.com/Article/details/gwpfxmvcy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtiossiy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.bbcook.cn/Article/details/glfosugbm.sHtML

[D15] 去重
来源：http://blog.epnwcf.com/Article/details/ggunguzhs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.sjlbkw.cn/Article/details/gcugemekk.sHtML

PHP:  array_unique($arr);
来源：http://www.share.bbcook.cn/Article/details/gvclqnirc.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/gxcyynzyo.sHtML


<!-- 参考信息 -->