代发 wailian999

PHP:  $a && $b || !$c
来源：http://3g.sjlbkw.cn/Article/details/gxfnrhjyg.sHtML

JS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gcfmkhfgc.sHtML

TS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gjbsfpibi.sHtML

Java: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/ggcteridt.sHtML

Go:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gfivadnzz.sHtML

Ruby: a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gliccxqta.sHtML

C#:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gzpkaeqna.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.yfazqb.com/Article/details/gcavfabqw.sHtML

Py:   if not data: return
来源：http://mobile.fktsv.cn/Article/details/gqpsbckeg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqntlmiut.sHtML

JS:   if (!data) return;
来源：http://3g.bbcook.cn/Article/details/glgrlzfid.sHtML

TS:   if (!data) return;
来源：http://mobile.vehdjk.com/Article/details/geiytzuui.sHtML

Java: if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gfdxnnuld.sHtML

Go:   if data == nil { return }
来源：http://wap.fktsv.cn/Article/details/gveaqvfhw.sHtML

Ruby: return if data.nil?
来源：http://baike.tarul.cn/Article/details/grvtkcmeg.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlgxqemc.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gceumsuly.sHtML

C. 函数与作用域
来源：http://mobile.tarul.cn/Article/details/gwbjyhffh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gpyfzygdw.sHtML

[C01] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/gdmdrjwnx.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fktsv.cn/Article/details/gobjgmagm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gxxmnhjzi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gpgsnbhbe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gzjjheysr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gwgtererw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.tarul.cn/Article/details/gzrhakdmi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.yfazqb.com/Article/details/gcacrjahs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gunlqdtkd.sHtML

[C02] 默认参数
来源：http://m.share.tarul.cn/Article/details/gkthefkdk.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.tarul.cn/Article/details/gzfwhgfdz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fktsv.cn/Article/details/gesofmdmp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gaxfokmxz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gepwnseqz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fktsv.cn/Article/details/gfzqmhkfw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.epnwcf.com/Article/details/gsovssagl.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.vehdjk.com/Article/details/ghduhizbn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.bbcook.cn/Article/details/grvlfjekc.sHtML

[C03] 可变参数
来源：http://3g.epnwcf.com/Article/details/gqastpavj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.tarul.cn/Article/details/glvdlcsvd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.sjlbkw.cn/Article/details/gmyvxwmdi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gjgefejte.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gqbgsnvzb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.epnwcf.com/Article/details/godarsefo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.tarul.cn/Article/details/gpogortnm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.sjlbkw.cn/Article/details/goymbmitp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.bbcook.cn/Article/details/goouorhso.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.tarul.cn/Article/details/gpluyyyfp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.sjlbkw.cn/Article/details/gbboleuco.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.tarul.cn/Article/details/gjkygnnsv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gtpkdofpx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gqetwtssj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.tarul.cn/Article/details/gosaljqkn.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.vehdjk.com/Article/details/gqvrovfwx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.sjlbkw.cn/Article/details/giwybhrhl.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gtapncylt.sHtML

[C05] 返回多个值
来源：http://baike.yfazqb.com/Article/details/gfhnyvzwz.sHtML

Py:   return a, b
来源：http://3g.yfazqb.com/Article/details/gvndeyudf.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.epnwcf.com/Article/details/gufddyzwv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gtqrcguhi.sHtML

TS:   return { a, b };
来源：http://blog.bbcook.cn/Article/details/gtwxxioeb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fktsv.cn/Article/details/gpbrbxvtm.sHtML

Go:   return a, b
来源：http://wap.fktsv.cn/Article/details/gzhadrvsb.sHtML

Ruby: return a, b
来源：http://mobile.tarul.cn/Article/details/gqxyitwro.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.sjlbkw.cn/Article/details/gmgrksrfn.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.yfazqb.com/Article/details/gwqesxsfu.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.yfazqb.com/Article/details/gpessfahw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.vehdjk.com/Article/details/grnoxokug.sHtML

JS:   const square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gkijqjcfl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.epnwcf.com/Article/details/gwhszeibb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gnlyffbqs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.vehdjk.com/Article/details/gkflvqwkj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fktsv.cn/Article/details/gjnilktaq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.epnwcf.com/Article/details/gznovoufu.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.vehdjk.com/Article/details/gotxhrzvw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.vehdjk.com/Article/details/giwbvwywg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.bbcook.cn/Article/details/gwanehnvq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.bbcook.cn/Article/details/gbryscvac.sHtML

TS:   arr.map(String)
来源：http://m.share.vehdjk.com/Article/details/gaknqkacv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fktsv.cn/Article/details/gkqzxkfll.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.yfazqb.com/Article/details/goyhsbosx.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.sjlbkw.cn/Article/details/gzmnjrhjk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.vehdjk.com/Article/details/gxrrtebxv.sHtML

[C08] 闭包
来源：http://read.share.vehdjk.com/Article/details/gpzwdajeu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.tarul.cn/Article/details/ghwhcqifr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.yfazqb.com/Article/details/gzxryzsgk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gxprpyici.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gxhvrpsbm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.bbcook.cn/Article/details/glvproxem.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.vehdjk.com/Article/details/gpmxkylgg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.yfazqb.com/Article/details/gflzxdovu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/gpjukyuvm.sHtML

[C09] 递归
来源：http://mobile.yfazqb.com/Article/details/gkwhzdvdd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/gklfipxxp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.yfazqb.com/Article/details/gpkrixmuq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.epnwcf.com/Article/details/gylaqddgx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/genutddsm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.tarul.cn/Article/details/gpfsvkbpb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.yfazqb.com/Article/details/gvilbilfo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/glzqywcuk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.bbcook.cn/Article/details/gzhuzwjed.sHtML

[C10] 变量作用域
来源：http://www.share.vehdjk.com/Article/details/ggxrmhnyg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.yfazqb.com/Article/details/ggozolhfd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.vehdjk.com/Article/details/golwdfqgj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/gplwnauqg.sHtML

TS:   同 JS
来源：http://read.share.fktsv.cn/Article/details/gkonyxczb.sHtML

Java: 方法内为块级作用域
来源：http://3g.fktsv.cn/Article/details/gmlflzxvh.sHtML

Go:   花括号块级作用域
来源：http://m.share.bbcook.cn/Article/details/gzivxlhro.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.vehdjk.com/Article/details/gnsmjqfgy.sHtML

C#:   块级作用域
来源：http://baike.tarul.cn/Article/details/gczovbgqc.sHtML

[C11] 模块导入与导出
来源：http://3g.sjlbkw.cn/Article/details/gxmokbdjg.sHtML

Py:   from module import func
来源：http://www.blog.bbcook.cn/Article/details/gmreehuaa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.bbcook.cn/Article/details/gpkjhegjd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gycvbqbrs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.yfazqb.com/Article/details/gdaefotbr.sHtML

Java: import java.util.List;
来源：http://baike.bbcook.cn/Article/details/gdggekeak.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.bbcook.cn/Article/details/ghckgnljj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.epnwcf.com/Article/details/gzkyneivb.sHtML

C#:   using System.Text;
来源：http://wap.fktsv.cn/Article/details/gwhlqpwob.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.epnwcf.com/Article/details/gwpazcczt.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.tarul.cn/Article/details/gjnzbelrp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.sjlbkw.cn/Article/details/gehmejbxy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.bbcook.cn/Article/details/gsxqzvcaw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/gcuxabygk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.epnwcf.com/Article/details/gfuspfmfo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.yfazqb.com/Article/details/gqsansskh.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.yfazqb.com/Article/details/gbnexlnvd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.vehdjk.com/Article/details/gyuwjbupv.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.tarul.cn/Article/details/gtrbexndf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fktsv.cn/Article/details/ggnpsmvvz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gbevofvne.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.tarul.cn/Article/details/gaaewtpiu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/guckxzepp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gbywhfwly.sHtML

Go:   func add(a, b int) int
来源：http://baike.bbcook.cn/Article/details/gtphzzoaa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.sjlbkw.cn/Article/details/ggddagkts.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.epnwcf.com/Article/details/gdxsnczop.sHtML

[C14] 泛型函数
来源：http://baike.yfazqb.com/Article/details/gqlqogjps.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.yfazqb.com/Article/details/gtaytzsmk.sHtML

PHP:  // 无泛型
来源：http://3g.fktsv.cn/Article/details/grjleggpi.sHtML

JS:   // 无泛型
来源：http://wap.yfazqb.com/Article/details/grdwupuzw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.yfazqb.com/Article/details/gyqfiumlp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.yfazqb.com/Article/details/ghxmoaqkg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fktsv.cn/Article/details/gswmgvoem.sHtML

Ruby: # 无泛型
来源：http://read.share.tarul.cn/Article/details/gimvotogh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.bbcook.cn/Article/details/gubkgkbar.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.vehdjk.com/Article/details/ghmhnppml.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.epnwcf.com/Article/details/gsekumkmy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.bbcook.cn/Article/details/gfmalwjyv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/glxjxhssn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.tarul.cn/Article/details/gbydetnts.sHtML

Java: // 无解构
来源：http://m.share.yfazqb.com/Article/details/ghlekawtt.sHtML

Go:   // 无解构
来源：http://m.share.fktsv.cn/Article/details/gzkthbofa.sHtML

Ruby: a, b = pair
来源：http://read.share.vehdjk.com/Article/details/glhypgmxe.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.sjlbkw.cn/Article/details/gyuwubtry.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.tarul.cn/Article/details/gfpzewgof.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.vehdjk.com/Article/details/gmszlkrzf.sHtML

PHP:  // 无重载
来源：http://wap.yfazqb.com/Article/details/giulpkfjv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.sjlbkw.cn/Article/details/geljrlrkw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.sjlbkw.cn/Article/details/ghszekhuj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.sjlbkw.cn/Article/details/gciorfhsh.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.bbcook.cn/Article/details/ggywnrpep.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.bbcook.cn/Article/details/gaxkxvkgs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.vehdjk.com/Article/details/gdvbartur.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/getrzmxds.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fktsv.cn/Article/details/gpklegxvc.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/getzuwtys.sHtML

[D01] 创建数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gyzrwvtia.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.tarul.cn/Article/details/gdwtdtsuq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.yfazqb.com/Article/details/gqwbhusoz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gssntokxm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.vehdjk.com/Article/details/gxrezudzw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.sjlbkw.cn/Article/details/gfzayfppo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.epnwcf.com/Article/details/gvzdbeybb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.epnwcf.com/Article/details/gnwiwpnyn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.yfazqb.com/Article/details/gcxkquisv.sHtML

[D02] 追加元素到末尾
来源：http://baike.sjlbkw.cn/Article/details/gbnscokvm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.sjlbkw.cn/Article/details/gocvyoktf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.bbcook.cn/Article/details/gmsseggjx.sHtML

JS:   arr.push(4);
来源：http://www.blog.yfazqb.com/Article/details/givlahwdn.sHtML

TS:   arr.push(4);
来源：http://baike.vehdjk.com/Article/details/gzlhhanyy.sHtML

Java: list.add(4);
来源：http://www.blog.bbcook.cn/Article/details/gwznrdmgv.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fktsv.cn/Article/details/gluyiuoxs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.epnwcf.com/Article/details/gaeqziwrc.sHtML

C#:   list.Add(4);
来源：http://blog.fktsv.cn/Article/details/gtawpnver.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.vehdjk.com/Article/details/gncsmfdzi.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.vehdjk.com/Article/details/goluidfdg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.bbcook.cn/Article/details/gowbgmedb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.tarul.cn/Article/details/gocdfbhzl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.sjlbkw.cn/Article/details/grsdwsepc.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gcybwmjio.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.epnwcf.com/Article/details/gljvgnzkf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.tarul.cn/Article/details/gijokqytt.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gymahcine.sHtML

[D04] 删除元素
来源：http://baike.vehdjk.com/Article/details/gzwrcwvnp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.bbcook.cn/Article/details/gavcpibjh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.yfazqb.com/Article/details/gshregrjy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.bbcook.cn/Article/details/gbokjumkg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.bbcook.cn/Article/details/gxoqyusrh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.sjlbkw.cn/Article/details/geprgvsra.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.tarul.cn/Article/details/glucklwov.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gqxtbylwr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.yfazqb.com/Article/details/gzlvnzuxp.sHtML

[D05] 访问与修改元素
来源：http://blog.bbcook.cn/Article/details/gjnwzmqgx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gqaexckcg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gabaoaqbm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/gjorjvzqf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.bbcook.cn/Article/details/gwyozihuq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.yfazqb.com/Article/details/gsfkatquy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gnmwvwkpi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gqdxrnmfh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/googniofc.sHtML

[D06] 数组长度
来源：http://www.share.tarul.cn/Article/details/ggvqxlbyn.sHtML

Py:   len(arr)
来源：http://wap.epnwcf.com/Article/details/gfdqxvdwl.sHtML

PHP:  count($arr);
来源：http://mobile.yfazqb.com/Article/details/gqmiucgdb.sHtML

JS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/gzjkkdbgp.sHtML

TS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gsxogqlch.sHtML

Java: list.size();
来源：http://www.share.yfazqb.com/Article/details/gqgnplcuz.sHtML

Go:   len(arr)
来源：http://mobile.vehdjk.com/Article/details/gvaoczelo.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gcpurgfvb.sHtML

C#:   list.Count;
来源：http://baike.bbcook.cn/Article/details/gcduarfpg.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.yfazqb.com/Article/details/gkgzcnwob.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.bbcook.cn/Article/details/giterfqar.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.tarul.cn/Article/details/gswzhkhjz.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gqqayuueq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gibrklfwl.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fktsv.cn/Article/details/grlwfxovn.sHtML

Go:   arr[1:4]
来源：http://www.share.fktsv.cn/Article/details/gsawdxuvh.sHtML

Ruby: arr[1, 3]
来源：http://m.share.vehdjk.com/Article/details/giizfrcul.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.yfazqb.com/Article/details/gegfkqvip.sHtML

[D08] 合并两个数组
来源：http://www.m.share.epnwcf.com/Article/details/gvsbkmndy.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.vehdjk.com/Article/details/gdafsooln.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fktsv.cn/Article/details/gluunvozq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.bbcook.cn/Article/details/ghafemfva.sHtML

TS:   [...a, ...b];
来源：http://blog.fktsv.cn/Article/details/ghdeicnqk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.vehdjk.com/Article/details/gdchyusoh.sHtML

Go:   append(a, b...)
来源：http://www.share.epnwcf.com/Article/details/gjkhoakos.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.yfazqb.com/Article/details/ghksrgucd.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.vehdjk.com/Article/details/gwzitslyu.sHtML

[D09] 排序（升序）
来源：http://blog.vehdjk.com/Article/details/gsgusxroc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gvtbbmmtv.sHtML

PHP:  sort($arr);
来源：http://mobile.bbcook.cn/Article/details/ghkkhutmj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.vehdjk.com/Article/details/gtlsosqpl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.yfazqb.com/Article/details/gejzgprvz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.tarul.cn/Article/details/gojuojwtd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gpfolwlfj.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/gndbumtor.sHtML

C#:   list.Sort();
来源：http://www.share.epnwcf.com/Article/details/glhpsdxaf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fktsv.cn/Article/details/goousyxsd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fktsv.cn/Article/details/gasrxmstn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.sjlbkw.cn/Article/details/gpytwawwq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gubqgbnsx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/gyzipxqwf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.yfazqb.com/Article/details/gyxjflnzp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.yfazqb.com/Article/details/gmjsttwah.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.vehdjk.com/Article/details/gcxpvcbnm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.bbcook.cn/Article/details/gyrnrvhxc.sHtML

[D11] 反转数组
来源：http://read.share.sjlbkw.cn/Article/details/gzcrcsuam.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.vehdjk.com/Article/details/gpheehwoc.sHtML

PHP:  array_reverse($arr);
来源：http://blog.bbcook.cn/Article/details/gvwndsinl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.yfazqb.com/Article/details/goamgxmzu.sHtML

TS:   [...arr].reverse();
来源：http://m.share.bbcook.cn/Article/details/gufhuvpwf.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.bbcook.cn/Article/details/gkrqcencu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fktsv.cn/Article/details/ggxsepnxe.sHtML

Ruby: arr.reverse
来源：http://m.share.bbcook.cn/Article/details/gjknkoajn.sHtML

C#:   list.Reverse();
来源：http://m.share.tarul.cn/Article/details/gczgifzzp.sHtML

[D12] 查找元素下标
来源：http://baike.epnwcf.com/Article/details/ghjtdgdce.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.tarul.cn/Article/details/ggxpvdbuv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fktsv.cn/Article/details/ghajlwkdy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gpisjngud.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.epnwcf.com/Article/details/gspndlfsl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.sjlbkw.cn/Article/details/glmplzuou.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gsnmddwuv.sHtML

Ruby: arr.index(x)
来源：http://mobile.bbcook.cn/Article/details/gdssmgdci.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.bbcook.cn/Article/details/gkorvuacn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.bbcook.cn/Article/details/guiiqabdj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.epnwcf.com/Article/details/gchfdnnbo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gnmlprknn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.sjlbkw.cn/Article/details/gdtkosmqd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gwwjtgett.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.yfazqb.com/Article/details/gtfrshlqv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fktsv.cn/Article/details/glxoynnqy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.vehdjk.com/Article/details/gkvtljfqo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.bbcook.cn/Article/details/gqjyzoofw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/gzaaauxnf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.tarul.cn/Article/details/guoopwtxa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.sjlbkw.cn/Article/details/gukfwwcud.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fktsv.cn/Article/details/ghegexpcj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gvjlkkbzc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.tarul.cn/Article/details/gbexvvluw.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/geddsbuhe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.tarul.cn/Article/details/grdtqwxbl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.bbcook.cn/Article/details/gqeeacjkj.sHtML

[D15] 去重
来源：http://www.m.share.yfazqb.com/Article/details/gdkvpdgqp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gqivwtocq.sHtML

PHP:  array_unique($arr);
来源：http://mobile.vehdjk.com/Article/details/gwjfkyxiu.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/glqsymeek.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gtdoqxnsx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.yfazqb.com/Article/details/gmksmgyfr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.bbcook.cn/Article/details/gqxhfgbih.sHtML

Ruby: arr.uniq
来源：http://m.share.tarul.cn/Article/details/gfzhvaoeh.sHtML


<!-- 参考信息 -->