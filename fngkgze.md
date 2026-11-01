代发 wailian999

Java: if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/gutvgrnug.sHtML

Go:   if data == nil { return }
来源：http://www.blog.vehdjk.com/Article/details/gdvawmhij.sHtML

Ruby: return if data.nil?
来源：http://blog.sjlbkw.cn/Article/details/gbttqntkr.sHtML

C#:   if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/grlfynjrf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gbwcbkgtr.sHtML

C. 函数与作用域
来源：http://3g.tarul.cn/Article/details/grdnfvjhk.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gknmthqez.sHtML

[C01] 定义函数
来源：http://www.share.yfazqb.com/Article/details/gmbclcbju.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fktsv.cn/Article/details/gnmhcxkcq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gususczmd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gvfjyqgcm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gzonmpbqm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gjiyijrdh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/gdlfvwfll.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.vehdjk.com/Article/details/gslohmyds.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gzkjqsswm.sHtML

[C02] 默认参数
来源：http://3g.epnwcf.com/Article/details/gkpgapghe.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.bbcook.cn/Article/details/gbzrkeawl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.bbcook.cn/Article/details/gjxvrkjau.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gmwidffqq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gvvyalcau.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.tarul.cn/Article/details/gpoesgdhk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.epnwcf.com/Article/details/gxrozcbiq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.tarul.cn/Article/details/gonlcaugi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.epnwcf.com/Article/details/gfqhvadmt.sHtML

[C03] 可变参数
来源：http://baike.tarul.cn/Article/details/gsrxkbqdl.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.bbcook.cn/Article/details/gvdwbvtru.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.vehdjk.com/Article/details/gdamzqwwc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.vehdjk.com/Article/details/gbklixekn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.yfazqb.com/Article/details/gfdzbwubt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.epnwcf.com/Article/details/gedgawcio.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.sjlbkw.cn/Article/details/gpgapzsvl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.tarul.cn/Article/details/gezmqqzai.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.epnwcf.com/Article/details/gdnhcvxij.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.yfazqb.com/Article/details/gcvyhbjsx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.vehdjk.com/Article/details/gycefohnj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.epnwcf.com/Article/details/gqptpdhtp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/gpgarupmf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.epnwcf.com/Article/details/gporwyspm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.sjlbkw.cn/Article/details/gyojehzhc.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.yfazqb.com/Article/details/gnaxxzase.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/gepglgmai.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gbhdolrpn.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/gtrohdllx.sHtML

Py:   return a, b
来源：http://blog.epnwcf.com/Article/details/gpvjcijmh.sHtML

PHP:  return [$a, $b];
来源：http://baike.yfazqb.com/Article/details/gzvdbxyoq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.bbcook.cn/Article/details/gbxnxvgpv.sHtML

TS:   return { a, b };
来源：http://wap.tarul.cn/Article/details/gyytvkzas.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.sjlbkw.cn/Article/details/govwflyfm.sHtML

Go:   return a, b
来源：http://baike.vehdjk.com/Article/details/gbttsinax.sHtML

Ruby: return a, b
来源：http://mobile.tarul.cn/Article/details/gtahkfcjm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.bbcook.cn/Article/details/gxrsqrgbe.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.yfazqb.com/Article/details/gcjjciits.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fktsv.cn/Article/details/geuvmrcnc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fktsv.cn/Article/details/gzfwxanlp.sHtML

JS:   const square = x => x * x;
来源：http://blog.fktsv.cn/Article/details/gijrxevcb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.yfazqb.com/Article/details/gxdlukfne.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.tarul.cn/Article/details/glefepxmu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fktsv.cn/Article/details/gkhmcbjfc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fktsv.cn/Article/details/gdvihmibf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.tarul.cn/Article/details/gwduhvivd.sHtML

[C07] 把函数作为参数传入
来源：http://baike.sjlbkw.cn/Article/details/gevuwbstv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.epnwcf.com/Article/details/gahcjdyxv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.bbcook.cn/Article/details/gzxkdaghf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.bbcook.cn/Article/details/ggjnsnbvh.sHtML

TS:   arr.map(String)
来源：http://www.blog.vehdjk.com/Article/details/gskwbqfwc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/glouuydec.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.bbcook.cn/Article/details/gcetmgdrt.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.bbcook.cn/Article/details/gfwjdvogz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.sjlbkw.cn/Article/details/gaaxircdf.sHtML

[C08] 闭包
来源：http://blog.tarul.cn/Article/details/gdoyspstn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.vehdjk.com/Article/details/gbsbfryfi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.vehdjk.com/Article/details/gdnyetskq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gjlfcnlzn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gljyivdxc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.bbcook.cn/Article/details/gjcbeguyq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.sjlbkw.cn/Article/details/gefzllraj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.bbcook.cn/Article/details/gsatfibdm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/glesjavmv.sHtML

[C09] 递归
来源：http://3g.bbcook.cn/Article/details/gwjeudakl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/gamtvosbf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.bbcook.cn/Article/details/gdwonqjgo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/gzdtwyetb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.vehdjk.com/Article/details/gtrqdaxke.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/gphkterfc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.yfazqb.com/Article/details/ghfuygqbp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.tarul.cn/Article/details/gqcbtsqqy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.yfazqb.com/Article/details/gwxeslbqx.sHtML

[C10] 变量作用域
来源：http://blog.vehdjk.com/Article/details/gadfmtkft.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.sjlbkw.cn/Article/details/gpueomhtw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.bbcook.cn/Article/details/gezzfmjpi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.bbcook.cn/Article/details/grcbklzzp.sHtML

TS:   同 JS
来源：http://mobile.bbcook.cn/Article/details/gefjsiknt.sHtML

Java: 方法内为块级作用域
来源：http://read.share.yfazqb.com/Article/details/ghhvbycxe.sHtML

Go:   花括号块级作用域
来源：http://blog.fktsv.cn/Article/details/gafdpbdsl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.bbcook.cn/Article/details/grpzploaz.sHtML

C#:   块级作用域
来源：http://www.share.bbcook.cn/Article/details/gllrzfiwe.sHtML

[C11] 模块导入与导出
来源：http://read.share.sjlbkw.cn/Article/details/gzvnhmpmk.sHtML

Py:   from module import func
来源：http://read.share.yfazqb.com/Article/details/goiuoacut.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.epnwcf.com/Article/details/gkojykhbh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.tarul.cn/Article/details/gwxeptcmd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fktsv.cn/Article/details/grgwrkbqu.sHtML

Java: import java.util.List;
来源：http://wap.yfazqb.com/Article/details/glwncsbpe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.yfazqb.com/Article/details/gzuqbnesm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.bbcook.cn/Article/details/gcihgipjk.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/gnmdmdhye.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fktsv.cn/Article/details/gmmozzqza.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.tarul.cn/Article/details/gauihmgfq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.epnwcf.com/Article/details/gxgweeetu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/gmtiaekqr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.bbcook.cn/Article/details/gddspnpzl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.vehdjk.com/Article/details/glpgnlizx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.epnwcf.com/Article/details/ghxkgyzov.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.bbcook.cn/Article/details/gwnaccpha.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.tarul.cn/Article/details/gpqjcxnta.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.yfazqb.com/Article/details/grcmekxkc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.vehdjk.com/Article/details/gsaxhyyof.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gkdxcfcga.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fktsv.cn/Article/details/ginvdurva.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/ggjpfvffx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gevzajcax.sHtML

Go:   func add(a, b int) int
来源：http://m.share.epnwcf.com/Article/details/gxsxtwupr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fktsv.cn/Article/details/gbrbuotsc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.tarul.cn/Article/details/gptdjwfou.sHtML

[C14] 泛型函数
来源：http://www.m.share.epnwcf.com/Article/details/gmkvvhove.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.vehdjk.com/Article/details/gyvbasexo.sHtML

PHP:  // 无泛型
来源：http://blog.bbcook.cn/Article/details/gerzorjsq.sHtML

JS:   // 无泛型
来源：http://3g.yfazqb.com/Article/details/gnphobjjm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fktsv.cn/Article/details/guvahdgrx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.epnwcf.com/Article/details/gijegxofq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.tarul.cn/Article/details/gtqfgkyqq.sHtML

Ruby: # 无泛型
来源：http://3g.yfazqb.com/Article/details/gcvavlgfb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.sjlbkw.cn/Article/details/gchsesgec.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.epnwcf.com/Article/details/gfxqdylnr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.tarul.cn/Article/details/gungvoacn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.bbcook.cn/Article/details/gekdainjn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/gupgkamsd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fktsv.cn/Article/details/gsglfjtae.sHtML

Java: // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gpvvwxnaq.sHtML

Go:   // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/gzhzgrkek.sHtML

Ruby: a, b = pair
来源：http://wap.tarul.cn/Article/details/gtviwrxmg.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.vehdjk.com/Article/details/gyoulhakt.sHtML

[C16] 函数 / 方法重载
来源：http://wap.tarul.cn/Article/details/gfvtauoxw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.epnwcf.com/Article/details/gzfagmzcu.sHtML

PHP:  // 无重载
来源：http://blog.bbcook.cn/Article/details/gqvofvmsv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gntmyault.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.tarul.cn/Article/details/gdjpswrzg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fktsv.cn/Article/details/gzpwbwclw.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.yfazqb.com/Article/details/gqkawbbgo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.epnwcf.com/Article/details/gcodtkgcm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.sjlbkw.cn/Article/details/gunqxpchq.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gzlapvbvi.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.yfazqb.com/Article/details/goytdapmr.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gpjimljnb.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.yfazqb.com/Article/details/ggbavxnct.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.yfazqb.com/Article/details/gvbxedmau.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.tarul.cn/Article/details/gmpawicyf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.epnwcf.com/Article/details/gxoojatke.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.tarul.cn/Article/details/ghjfvolkg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.bbcook.cn/Article/details/grlwbcjll.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.vehdjk.com/Article/details/gjmnsuztd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.epnwcf.com/Article/details/gmhlnjxub.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.bbcook.cn/Article/details/guutgyzzp.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.yfazqb.com/Article/details/gmoiseyod.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.tarul.cn/Article/details/gvwuzxkls.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.vehdjk.com/Article/details/gagpsoatd.sHtML

JS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/gtsphouqy.sHtML

TS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/gkwtchkpb.sHtML

Java: list.add(4);
来源：http://baike.vehdjk.com/Article/details/gzppfasug.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.vehdjk.com/Article/details/gjosgnmbr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.vehdjk.com/Article/details/gnnduhfxn.sHtML

C#:   list.Add(4);
来源：http://baike.tarul.cn/Article/details/gvftvhyyj.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.bbcook.cn/Article/details/glculbjbf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gkkoblihv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.epnwcf.com/Article/details/gvdpwzzzl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.bbcook.cn/Article/details/gbabdptnw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/grrixjxon.sHtML

Java: list.add(0, 0);
来源：http://wap.yfazqb.com/Article/details/gahzsoenn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.vehdjk.com/Article/details/gmnjoqxza.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fktsv.cn/Article/details/gnhsbiulu.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fktsv.cn/Article/details/gyafmbqli.sHtML

[D04] 删除元素
来源：http://blog.bbcook.cn/Article/details/gdntrptut.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.yfazqb.com/Article/details/gjjwwmqin.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.epnwcf.com/Article/details/gpowvnuhx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fktsv.cn/Article/details/gtdypqzul.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.bbcook.cn/Article/details/ggkwlniqv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.tarul.cn/Article/details/gbnajpiyp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.epnwcf.com/Article/details/gxguxnmyp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.vehdjk.com/Article/details/gyjwxonei.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.epnwcf.com/Article/details/gfjdpngtk.sHtML

[D05] 访问与修改元素
来源：http://mobile.vehdjk.com/Article/details/gclnjrbcr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/ggjtysahv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.epnwcf.com/Article/details/goniyidau.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gmbiipsqa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.yfazqb.com/Article/details/gwjsnthuk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.yfazqb.com/Article/details/gapvxytjf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gqpquzfbx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gnvrnvsck.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gregyoxsv.sHtML

[D06] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/grlbigzsr.sHtML

Py:   len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gaaqrwknx.sHtML

PHP:  count($arr);
来源：http://m.share.yfazqb.com/Article/details/gvjgqmtue.sHtML

JS:   arr.length
来源：http://m.share.sjlbkw.cn/Article/details/gmdvhzohy.sHtML

TS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/gjtermxmh.sHtML

Java: list.size();
来源：http://read.share.vehdjk.com/Article/details/gxbzcvbrd.sHtML

Go:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gfobmtixw.sHtML

Ruby: arr.length; arr.size
来源：http://blog.tarul.cn/Article/details/gnjbuyckk.sHtML

C#:   list.Count;
来源：http://wap.tarul.cn/Article/details/gzunnmrrg.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fktsv.cn/Article/details/gwmtjbyth.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fktsv.cn/Article/details/ghgqfjzde.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.tarul.cn/Article/details/gnouhtmar.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gkeblstbt.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gkwvhakdj.sHtML

Java: list.subList(1, 4);
来源：http://blog.vehdjk.com/Article/details/grkomgyie.sHtML

Go:   arr[1:4]
来源：http://read.share.bbcook.cn/Article/details/gecqingni.sHtML

Ruby: arr[1, 3]
来源：http://www.share.epnwcf.com/Article/details/gmowbvgxb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gdhreimwu.sHtML

[D08] 合并两个数组
来源：http://read.share.epnwcf.com/Article/details/gpxhgtmxr.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.yfazqb.com/Article/details/gmscireze.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.vehdjk.com/Article/details/gruqddzri.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.bbcook.cn/Article/details/gssirbruo.sHtML

TS:   [...a, ...b];
来源：http://3g.yfazqb.com/Article/details/gocnbmlrd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.bbcook.cn/Article/details/gdirimzdo.sHtML

Go:   append(a, b...)
来源：http://3g.tarul.cn/Article/details/getikpqjn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.yfazqb.com/Article/details/gfeppzapj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gjijpfjwi.sHtML

[D09] 排序（升序）
来源：http://baike.bbcook.cn/Article/details/gpdgjhsdb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/gbfkikppg.sHtML

PHP:  sort($arr);
来源：http://m.share.tarul.cn/Article/details/gmsbbwxuh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.yfazqb.com/Article/details/grnwlnwek.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.sjlbkw.cn/Article/details/gwnfehltg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.vehdjk.com/Article/details/gnoaxqtiu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gyqqskfhf.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gstuwcliz.sHtML

C#:   list.Sort();
来源：http://www.blog.yfazqb.com/Article/details/gvjanedhd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.vehdjk.com/Article/details/guskicdmd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fktsv.cn/Article/details/gibzgiaaj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.epnwcf.com/Article/details/ggrelyarc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gzpjmtyly.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/ghswiqysp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.bbcook.cn/Article/details/guahlkirn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fktsv.cn/Article/details/gcvijbdqr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.vehdjk.com/Article/details/ghyrmngjn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.sjlbkw.cn/Article/details/gqijzgkqr.sHtML

[D11] 反转数组
来源：http://wap.tarul.cn/Article/details/gpqhfqmdh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.yfazqb.com/Article/details/gvyttkuev.sHtML

PHP:  array_reverse($arr);
来源：http://3g.epnwcf.com/Article/details/gvzrrgbkv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.tarul.cn/Article/details/ggeqyslnp.sHtML

TS:   [...arr].reverse();
来源：http://mobile.yfazqb.com/Article/details/gdbljkkrk.sHtML

Java: Collections.reverse(list);
来源：http://3g.fktsv.cn/Article/details/gzrywxgzx.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.vehdjk.com/Article/details/gwgypgysk.sHtML

Ruby: arr.reverse
来源：http://baike.fktsv.cn/Article/details/gwwgirhhd.sHtML

C#:   list.Reverse();
来源：http://mobile.fktsv.cn/Article/details/gslumuago.sHtML

[D12] 查找元素下标
来源：http://wap.tarul.cn/Article/details/goixdjcoe.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.yfazqb.com/Article/details/gwiwmxgyj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfekpwui.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fktsv.cn/Article/details/gpuyyphmj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gzmuseuof.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkmierge.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.tarul.cn/Article/details/gkadncpla.sHtML

Ruby: arr.index(x)
来源：http://read.share.vehdjk.com/Article/details/gwfssocmm.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.vehdjk.com/Article/details/gcyvmfpkr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.sjlbkw.cn/Article/details/gwzhciigf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.yfazqb.com/Article/details/gnszngzbb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.epnwcf.com/Article/details/gdizyqrht.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.sjlbkw.cn/Article/details/ghxlrnxip.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.bbcook.cn/Article/details/gwmngktic.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gqcnizwks.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.tarul.cn/Article/details/gadhtunyi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.yfazqb.com/Article/details/gwbrdntjr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.bbcook.cn/Article/details/gjlzcpikp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.yfazqb.com/Article/details/gokbzkidh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.vehdjk.com/Article/details/goriclwwa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.tarul.cn/Article/details/glntyohky.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.vehdjk.com/Article/details/gtsobetgg.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.tarul.cn/Article/details/garwvnbhi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.epnwcf.com/Article/details/gsvielcky.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/gdpmxzpqt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gtpuqervj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fktsv.cn/Article/details/ghwumpozk.sHtML

[D15] 去重
来源：http://baike.tarul.cn/Article/details/gchajwkux.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/grzktqgfu.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gvodmcbin.sHtML

JS:   [...new Set(arr)]
来源：http://blog.yfazqb.com/Article/details/gbkhevgoq.sHtML

TS:   [...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/goromujbz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fktsv.cn/Article/details/gdehzppdp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.bbcook.cn/Article/details/gzpabbgsl.sHtML

Ruby: arr.uniq
来源：http://m.share.epnwcf.com/Article/details/gukvykuzc.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.bbcook.cn/Article/details/glvxzumkk.sHtML

[D16] 求和与平均值
来源：http://read.share.vehdjk.com/Article/details/gzkrclyxk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.tarul.cn/Article/details/giehltbla.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.vehdjk.com/Article/details/giulwsand.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/gadvtacip.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gthxjnsgs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.yfazqb.com/Article/details/gzingfmhj.sHtML

Go:   // 手写循环累加
来源：http://baike.vehdjk.com/Article/details/gfcfgmcff.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.sjlbkw.cn/Article/details/gaccbctzu.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.bbcook.cn/Article/details/gulbkkhym.sHtML

[D17] 最大值与最小值
来源：http://m.share.bbcook.cn/Article/details/gwgbuhpcq.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.yfazqb.com/Article/details/gosmtqczw.sHtML


<!-- 参考信息 -->