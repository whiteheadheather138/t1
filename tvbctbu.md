代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.vehdjk.com/Article/details/gsteseief.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/gmfrltknn.sHtML

[B15] 布尔运算与取反
来源：http://read.share.sjlbkw.cn/Article/details/gsohblavy.sHtML

Py:   a and b or not c
来源：http://www.m.share.yfazqb.com/Article/details/glfzikmqt.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.yfazqb.com/Article/details/gxwfdmfci.sHtML

JS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gzswhoyli.sHtML

TS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gnojpxlrd.sHtML

Java: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gligeysyv.sHtML

Go:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gmpmqniez.sHtML

Ruby: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gukumsehe.sHtML

C#:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gadwmxkvq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.epnwcf.com/Article/details/geuhenage.sHtML

Py:   if not data: return
来源：http://wap.bbcook.cn/Article/details/gelubfkhh.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.tarul.cn/Article/details/glsgeptyy.sHtML

JS:   if (!data) return;
来源：http://wap.bbcook.cn/Article/details/gcqloygrr.sHtML

TS:   if (!data) return;
来源：http://blog.yfazqb.com/Article/details/gkfhlpsrv.sHtML

Java: if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/gawyvnmss.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.tarul.cn/Article/details/gydtrzayj.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.bbcook.cn/Article/details/gcsephhgs.sHtML

C#:   if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/gpweuzulo.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/galzjuisj.sHtML

C. 函数与作用域
来源：http://blog.sjlbkw.cn/Article/details/gpjuaxxrl.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gggmasura.sHtML

[C01] 定义函数
来源：http://3g.tarul.cn/Article/details/gvlnpuwbv.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.tarul.cn/Article/details/glfmfcwlg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gavpxiqcy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gmyunxsxx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gmwmwlztd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gkqouxqqo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.bbcook.cn/Article/details/govmcbabq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.vehdjk.com/Article/details/gwejsgzac.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gpnlefjdf.sHtML

[C02] 默认参数
来源：http://mobile.yfazqb.com/Article/details/ggwipaejm.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.vehdjk.com/Article/details/gweuqaiwh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.epnwcf.com/Article/details/guhgbsdiu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/gmfqbdfcl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gidsmzejb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.sjlbkw.cn/Article/details/gnvjupfox.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.yfazqb.com/Article/details/grbaokvgw.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.epnwcf.com/Article/details/gekqasmnj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.yfazqb.com/Article/details/gvyookkgj.sHtML

[C03] 可变参数
来源：http://3g.vehdjk.com/Article/details/gxkcjfflj.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fktsv.cn/Article/details/gvfpdxuzb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.epnwcf.com/Article/details/gfihomufu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gsuxkzhmr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gmvjqaeyb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.sjlbkw.cn/Article/details/guslaylnr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.bbcook.cn/Article/details/gcokbbswk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.bbcook.cn/Article/details/gjvtpjxoy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fktsv.cn/Article/details/ghtprohha.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.sjlbkw.cn/Article/details/glilihxgf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.vehdjk.com/Article/details/gkznjdfxp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.bbcook.cn/Article/details/gufbfkiwo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/gfijhqoox.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.vehdjk.com/Article/details/gbkxsagey.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.vehdjk.com/Article/details/gkwszxaec.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.vehdjk.com/Article/details/gdpjxzfgy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gvgsnbhdw.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwvvonkp.sHtML

[C05] 返回多个值
来源：http://blog.tarul.cn/Article/details/gifmkvngf.sHtML

Py:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/guievattn.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.epnwcf.com/Article/details/gzpvzsloz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/goaazevze.sHtML

TS:   return { a, b };
来源：http://www.share.yfazqb.com/Article/details/ggizhvaxj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.epnwcf.com/Article/details/gmgdqglaz.sHtML

Go:   return a, b
来源：http://baike.vehdjk.com/Article/details/grvwuzmgd.sHtML

Ruby: return a, b
来源：http://read.share.tarul.cn/Article/details/gfpemuvoz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.sjlbkw.cn/Article/details/gnzdsxlrt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.yfazqb.com/Article/details/gnqgdbwvy.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fktsv.cn/Article/details/gpzkaivsf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.vehdjk.com/Article/details/gdwhcctqi.sHtML

JS:   const square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gziwpovmz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.epnwcf.com/Article/details/ghtlrsmeu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.epnwcf.com/Article/details/gecgbqpqc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.epnwcf.com/Article/details/glscomfir.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.yfazqb.com/Article/details/gxpkqzgws.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gjdirfilo.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fktsv.cn/Article/details/gasyhmfps.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.sjlbkw.cn/Article/details/gyskwefny.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.tarul.cn/Article/details/gssnjqzft.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.epnwcf.com/Article/details/gkhfwwcsm.sHtML

TS:   arr.map(String)
来源：http://blog.sjlbkw.cn/Article/details/gybcqahad.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.sjlbkw.cn/Article/details/gncqslwaz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.tarul.cn/Article/details/ghbrqyths.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.sjlbkw.cn/Article/details/gehczdrfd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.bbcook.cn/Article/details/guonfwgxt.sHtML

[C08] 闭包
来源：http://read.share.yfazqb.com/Article/details/ggzrbhaci.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.bbcook.cn/Article/details/ghuzhhvmg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfyvnpaxl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/gbcrbcpsy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gjagpzvcz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.bbcook.cn/Article/details/gpftbhjjc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.epnwcf.com/Article/details/grvonzcbu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fktsv.cn/Article/details/gduzstkav.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gzwgmxfzc.sHtML

[C09] 递归
来源：http://wap.tarul.cn/Article/details/gzuklojvu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gjhonslda.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.tarul.cn/Article/details/gepndqeac.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gcxibmhjq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.bbcook.cn/Article/details/gmwzjcfoi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.epnwcf.com/Article/details/gwarsyqir.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.bbcook.cn/Article/details/gdpgzsifs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/gnqkxqtlm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.yfazqb.com/Article/details/gbbujzucp.sHtML

[C10] 变量作用域
来源：http://read.share.yfazqb.com/Article/details/gphrdvspj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.epnwcf.com/Article/details/gfbhomije.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.sjlbkw.cn/Article/details/glnnjrfgd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.tarul.cn/Article/details/gpvuoowxv.sHtML

TS:   同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gbvaxdiqb.sHtML

Java: 方法内为块级作用域
来源：http://baike.fktsv.cn/Article/details/gwtwtaulo.sHtML

Go:   花括号块级作用域
来源：http://blog.yfazqb.com/Article/details/gysuhmler.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.epnwcf.com/Article/details/gxefymcnf.sHtML

C#:   块级作用域
来源：http://mobile.epnwcf.com/Article/details/ghelnjjrw.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.tarul.cn/Article/details/gocvoufqh.sHtML

Py:   from module import func
来源：http://www.share.epnwcf.com/Article/details/ghngcakxc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.vehdjk.com/Article/details/guciwsylq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/gjeiurzwq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.yfazqb.com/Article/details/godzqrfln.sHtML

Java: import java.util.List;
来源：http://www.blog.yfazqb.com/Article/details/gzrpkdeah.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.bbcook.cn/Article/details/gopqxrdue.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.yfazqb.com/Article/details/gpqwknkyn.sHtML

C#:   using System.Text;
来源：http://www.share.yfazqb.com/Article/details/ggubgckul.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.tarul.cn/Article/details/gwtwvreuv.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.yfazqb.com/Article/details/gefiwcqum.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.vehdjk.com/Article/details/grfmovpdi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/gazatdqfx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/guxmdlmfe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.epnwcf.com/Article/details/gdwbxabow.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fktsv.cn/Article/details/gipplvdcv.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.tarul.cn/Article/details/gjjizmyph.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fktsv.cn/Article/details/getfcbduh.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.vehdjk.com/Article/details/gclniclba.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.bbcook.cn/Article/details/gosynsipt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gwrumnbpj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.yfazqb.com/Article/details/gvmudlzeq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gayzlgvnn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gjqwwapxn.sHtML

Go:   func add(a, b int) int
来源：http://3g.tarul.cn/Article/details/gxytljncs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.bbcook.cn/Article/details/gnzwtrwny.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.yfazqb.com/Article/details/gvjmyedad.sHtML

[C14] 泛型函数
来源：http://wap.bbcook.cn/Article/details/gphwftuxu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.epnwcf.com/Article/details/gbfxrberl.sHtML

PHP:  // 无泛型
来源：http://mobile.fktsv.cn/Article/details/glopuwmsx.sHtML

JS:   // 无泛型
来源：http://wap.yfazqb.com/Article/details/gbcvjmrsg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.sjlbkw.cn/Article/details/gremcbknb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.tarul.cn/Article/details/gescbqpgg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.sjlbkw.cn/Article/details/gahjjhrfq.sHtML

Ruby: # 无泛型
来源：http://wap.vehdjk.com/Article/details/gwncjyqlj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.tarul.cn/Article/details/gpqohijwa.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.yfazqb.com/Article/details/gdhpoojyw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.yfazqb.com/Article/details/gmbrldqpb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.yfazqb.com/Article/details/gbbaongka.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/gjqwmdbhy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.tarul.cn/Article/details/gepyabdzc.sHtML

Java: // 无解构
来源：http://blog.fktsv.cn/Article/details/gersyztnb.sHtML

Go:   // 无解构
来源：http://www.share.bbcook.cn/Article/details/gybihhroz.sHtML

Ruby: a, b = pair
来源：http://www.m.share.yfazqb.com/Article/details/gfxczuspc.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.tarul.cn/Article/details/gahpqircm.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fktsv.cn/Article/details/gjiiokrdd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.yfazqb.com/Article/details/ggklsmlkq.sHtML

PHP:  // 无重载
来源：http://www.blog.epnwcf.com/Article/details/gyvrwjijn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.vehdjk.com/Article/details/ghqklavno.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fktsv.cn/Article/details/gdpkypaql.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.yfazqb.com/Article/details/gezwnzzyn.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.yfazqb.com/Article/details/gbgwkhkck.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.yfazqb.com/Article/details/gfeufuogp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.yfazqb.com/Article/details/gxdsqvuuy.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gapammqju.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.epnwcf.com/Article/details/gvosclrua.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzpbcgdxz.sHtML

[D01] 创建数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gffqczvzv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fktsv.cn/Article/details/gvrqwphgj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/gjuxhrzxk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.epnwcf.com/Article/details/gddgyzotw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.bbcook.cn/Article/details/gwjagkcsz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.sjlbkw.cn/Article/details/gdyuyweiw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.epnwcf.com/Article/details/gfuvqejot.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.sjlbkw.cn/Article/details/gjsjllbpu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.yfazqb.com/Article/details/grdummwgp.sHtML

[D02] 追加元素到末尾
来源：http://m.share.vehdjk.com/Article/details/greszecfw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.yfazqb.com/Article/details/gvymdaamb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.yfazqb.com/Article/details/gdnxozplx.sHtML

JS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/gwjywrhfq.sHtML

TS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gkzodhhla.sHtML

Java: list.add(4);
来源：http://www.blog.bbcook.cn/Article/details/ggmieekoj.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.bbcook.cn/Article/details/gabkkswhu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.vehdjk.com/Article/details/grhjthlla.sHtML

C#:   list.Add(4);
来源：http://www.share.bbcook.cn/Article/details/gmekydyhk.sHtML

[D03] 在指定位置插入元素
来源：http://blog.sjlbkw.cn/Article/details/goaygomxi.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.vehdjk.com/Article/details/gpsgokplw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fktsv.cn/Article/details/gryqfzihv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.sjlbkw.cn/Article/details/grbefdhbd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gzsxoqukg.sHtML

Java: list.add(0, 0);
来源：http://www.share.yfazqb.com/Article/details/gafptsuvx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fktsv.cn/Article/details/gwktoughf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.tarul.cn/Article/details/gabahejau.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.yfazqb.com/Article/details/gsavftdru.sHtML

[D04] 删除元素
来源：http://www.m.share.fktsv.cn/Article/details/gztkvoggy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.vehdjk.com/Article/details/gamfgnlzx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.sjlbkw.cn/Article/details/gufxybnkd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fktsv.cn/Article/details/gxjjaxtmq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.tarul.cn/Article/details/gvekizmnc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.vehdjk.com/Article/details/gtdacyexe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.sjlbkw.cn/Article/details/gstppryvs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.tarul.cn/Article/details/grecdubuz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.yfazqb.com/Article/details/ghihpiach.sHtML

[D05] 访问与修改元素
来源：http://www.share.epnwcf.com/Article/details/gdefukjcl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gszwzbswi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/gigoxgegs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gzijunggu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.bbcook.cn/Article/details/gpiwnmbll.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fktsv.cn/Article/details/ghdiertdn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/glgoyspoa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gvlqzpqma.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.tarul.cn/Article/details/goywjwmaa.sHtML

[D06] 数组长度
来源：http://3g.yfazqb.com/Article/details/gztywncjp.sHtML

Py:   len(arr)
来源：http://baike.tarul.cn/Article/details/gfjrgewue.sHtML

PHP:  count($arr);
来源：http://wap.fktsv.cn/Article/details/glotqehjh.sHtML

JS:   arr.length
来源：http://baike.yfazqb.com/Article/details/gcdyrudkt.sHtML

TS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gbacknljg.sHtML

Java: list.size();
来源：http://www.share.epnwcf.com/Article/details/gvomspyux.sHtML

Go:   len(arr)
来源：http://mobile.tarul.cn/Article/details/gfbgwaqeo.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.yfazqb.com/Article/details/gfhxsyfqk.sHtML

C#:   list.Count;
来源：http://www.share.yfazqb.com/Article/details/goqduauxa.sHtML

[D07] 切片 / 取子数组
来源：http://wap.tarul.cn/Article/details/gwbjlesfh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.sjlbkw.cn/Article/details/ghdhyrguk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fktsv.cn/Article/details/gfijsqvvv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gjjjqfbxp.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gulmmmrwt.sHtML

Java: list.subList(1, 4);
来源：http://read.share.yfazqb.com/Article/details/ghwqalhdv.sHtML

Go:   arr[1:4]
来源：http://3g.bbcook.cn/Article/details/gcenibgdb.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.tarul.cn/Article/details/gkykmufdh.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.vehdjk.com/Article/details/gjmxyehbx.sHtML

[D08] 合并两个数组
来源：http://www.share.bbcook.cn/Article/details/gipguubup.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fktsv.cn/Article/details/gdqnqgkac.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.sjlbkw.cn/Article/details/gosuivzln.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.yfazqb.com/Article/details/gapemurdk.sHtML

TS:   [...a, ...b];
来源：http://www.share.sjlbkw.cn/Article/details/gwvmpxbwu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.yfazqb.com/Article/details/gnczskztf.sHtML

Go:   append(a, b...)
来源：http://read.share.fktsv.cn/Article/details/gdmhjiqrd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.bbcook.cn/Article/details/gcgbbljqv.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.epnwcf.com/Article/details/giexccjaw.sHtML

[D09] 排序（升序）
来源：http://baike.tarul.cn/Article/details/gpgksksxa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gxguarcfy.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gasryyrgf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.tarul.cn/Article/details/galcvwdan.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.vehdjk.com/Article/details/gsamikrdg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.vehdjk.com/Article/details/gucabnwsg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gdcnuujdc.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/gywgbnveb.sHtML

C#:   list.Sort();
来源：http://blog.yfazqb.com/Article/details/gesmuxysw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.vehdjk.com/Article/details/gpfhzzbdm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.bbcook.cn/Article/details/gguccpybg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.vehdjk.com/Article/details/gyoojsimg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/getrvptlq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gfhkjxbwq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.yfazqb.com/Article/details/gcvstqboi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.sjlbkw.cn/Article/details/guydtzipn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.vehdjk.com/Article/details/gttynesse.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.vehdjk.com/Article/details/genhdzhto.sHtML

[D11] 反转数组
来源：http://www.blog.epnwcf.com/Article/details/gwhbnyzxi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.epnwcf.com/Article/details/gsmnfvazn.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gfospwtxz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.bbcook.cn/Article/details/gsolnsckr.sHtML

TS:   [...arr].reverse();
来源：http://wap.epnwcf.com/Article/details/gvzydqjuf.sHtML

Java: Collections.reverse(list);
来源：http://mobile.vehdjk.com/Article/details/gechmbeld.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.epnwcf.com/Article/details/gcjaonpzr.sHtML

Ruby: arr.reverse
来源：http://mobile.yfazqb.com/Article/details/gacvdweea.sHtML

C#:   list.Reverse();
来源：http://www.share.sjlbkw.cn/Article/details/gwkshebhj.sHtML

[D12] 查找元素下标
来源：http://m.share.tarul.cn/Article/details/gonwrptaw.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fktsv.cn/Article/details/gmfmgunmf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.yfazqb.com/Article/details/gtoeaufvv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/grlbbxknt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/giuawaold.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.epnwcf.com/Article/details/gpnhoarsw.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gsubtgeru.sHtML

Ruby: arr.index(x)
来源：http://m.share.sjlbkw.cn/Article/details/gubydzpsl.sHtML

C#:   list.IndexOf(x);
来源：http://wap.tarul.cn/Article/details/grclixyao.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.sjlbkw.cn/Article/details/gixmjxqqv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.yfazqb.com/Article/details/gnqzeekjg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.epnwcf.com/Article/details/grlytdyvn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.bbcook.cn/Article/details/gbqfnckho.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/gjombnshb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.yfazqb.com/Article/details/gdvvnpuvv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.bbcook.cn/Article/details/gcpytfsjg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.vehdjk.com/Article/details/gxpglftzh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.yfazqb.com/Article/details/gmxxrhiae.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.yfazqb.com/Article/details/gadkgbotg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fktsv.cn/Article/details/glytfaiva.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gahimmzjj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/gsgsaaldj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.vehdjk.com/Article/details/grymumcyb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fktsv.cn/Article/details/gcqrwqjxm.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/goqiavrxx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fktsv.cn/Article/details/gsvpoowha.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.vehdjk.com/Article/details/gawvvpvgk.sHtML

[D15] 去重
来源：http://www.share.vehdjk.com/Article/details/gnnuevrwh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fktsv.cn/Article/details/gbcexwanj.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.tarul.cn/Article/details/ghjfeswlg.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/gggbzodju.sHtML


<!-- 参考信息 -->