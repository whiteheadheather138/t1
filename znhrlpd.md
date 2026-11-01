代发 wailian999

[B13] 判断是否为数字
来源：http://3g.vehdjk.com/Article/details/gtwlctczu.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.yfazqb.com/Article/details/gqcsnhcpz.sHtML

PHP:  is_numeric($x)
来源：http://read.share.epnwcf.com/Article/details/gtoatgrxh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.yfazqb.com/Article/details/grbkbnzmv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gqxexqopi.sHtML

Java: x instanceof Number
来源：http://wap.sjlbkw.cn/Article/details/gcrbdcggg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.yfazqb.com/Article/details/gcjosphnp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.tarul.cn/Article/details/gexdyecii.sHtML

C#:   x is int or double or decimal
来源：http://m.share.sjlbkw.cn/Article/details/gawfldboc.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fktsv.cn/Article/details/gmdlvplzu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.sjlbkw.cn/Article/details/gcfqtifsg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.epnwcf.com/Article/details/gwsbtwfiw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gphggfctj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.sjlbkw.cn/Article/details/ggxtqigsf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.yfazqb.com/Article/details/gbpmgtkgq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fktsv.cn/Article/details/gjkjdaqtv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.bbcook.cn/Article/details/gaabtujss.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.vehdjk.com/Article/details/gaipimmzy.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fktsv.cn/Article/details/gyghtukho.sHtML

Py:   a and b or not c
来源：http://wap.fktsv.cn/Article/details/gewvhrsqz.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.epnwcf.com/Article/details/gtgtctlfc.sHtML

JS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gptyjgivr.sHtML

TS:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gnzflsyup.sHtML

Java: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gsprhaqsp.sHtML

Go:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gfivlfazr.sHtML

Ruby: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gkzthqrvr.sHtML

C#:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gzcqcipgt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.epnwcf.com/Article/details/glzkqykfm.sHtML

Py:   if not data: return
来源：http://m.share.epnwcf.com/Article/details/gonifhjax.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fktsv.cn/Article/details/gwmmvjqdb.sHtML

JS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gwzjtinfh.sHtML

TS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/gmsjmwfuy.sHtML

Java: if (data == null) return;
来源：http://mobile.fktsv.cn/Article/details/ghadcplkl.sHtML

Go:   if data == nil { return }
来源：http://m.share.fktsv.cn/Article/details/glvecdbku.sHtML

Ruby: return if data.nil?
来源：http://read.share.epnwcf.com/Article/details/gtdtxkaud.sHtML

C#:   if (data == null) return;
来源：http://wap.yfazqb.com/Article/details/gacyepnhv.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gyyrzhtfg.sHtML

C. 函数与作用域
来源：http://read.share.yfazqb.com/Article/details/gmgvjwifv.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gopfpdwto.sHtML

[C01] 定义函数
来源：http://wap.yfazqb.com/Article/details/grtunhalm.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fktsv.cn/Article/details/gqooycrbw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gguvjjgev.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/glqvxybav.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gltrvuuzx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gszniqqvl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.yfazqb.com/Article/details/gyvrbwjdj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.vehdjk.com/Article/details/gczqpfigv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/golbcilia.sHtML

[C02] 默认参数
来源：http://3g.vehdjk.com/Article/details/gjujbycme.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.yfazqb.com/Article/details/gpfvavewu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.epnwcf.com/Article/details/gulveiith.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gqgtqgksk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.vehdjk.com/Article/details/gxhsmwlfw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.bbcook.cn/Article/details/gxopxfguj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.tarul.cn/Article/details/ggoqxfmoy.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.yfazqb.com/Article/details/glbpnxruy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.tarul.cn/Article/details/guwkqyzhf.sHtML

[C03] 可变参数
来源：http://wap.bbcook.cn/Article/details/gqxjkwucp.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.bbcook.cn/Article/details/gsizixdgy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.yfazqb.com/Article/details/gufkqiris.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/gqxeavnmh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gyyvrzybr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.vehdjk.com/Article/details/gtgezrbrj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.yfazqb.com/Article/details/glwhowbxi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.vehdjk.com/Article/details/gaqfrjyxa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.vehdjk.com/Article/details/gakscvhjh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.sjlbkw.cn/Article/details/gezqbzljy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.bbcook.cn/Article/details/gfbevsgll.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.bbcook.cn/Article/details/gzngviciu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.yfazqb.com/Article/details/glwkksiux.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.yfazqb.com/Article/details/gugdoyyje.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.tarul.cn/Article/details/gwadlfpme.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.sjlbkw.cn/Article/details/gayeqpedr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gzglqjkdn.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gautpfwuc.sHtML

[C05] 返回多个值
来源：http://blog.sjlbkw.cn/Article/details/glljpjglr.sHtML

Py:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/gipsqbrmk.sHtML

PHP:  return [$a, $b];
来源：http://blog.tarul.cn/Article/details/godnnzroc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gnmjnbxlp.sHtML

TS:   return { a, b };
来源：http://m.share.fktsv.cn/Article/details/gdmunhdnp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.tarul.cn/Article/details/gbrdafozi.sHtML

Go:   return a, b
来源：http://3g.fktsv.cn/Article/details/gfsnuwzak.sHtML

Ruby: return a, b
来源：http://mobile.epnwcf.com/Article/details/gkiqhpgdt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.bbcook.cn/Article/details/glzhkisja.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.yfazqb.com/Article/details/glpnllfgm.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fktsv.cn/Article/details/gsxpufmhd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.bbcook.cn/Article/details/gmoihhnnr.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fktsv.cn/Article/details/gjyglpezs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/guohweszb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.tarul.cn/Article/details/gnprjebhv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.bbcook.cn/Article/details/gitbpqtme.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.bbcook.cn/Article/details/gokwmybmk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gqftqizvi.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.bbcook.cn/Article/details/gigqjksmv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.vehdjk.com/Article/details/gfohqgptt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.yfazqb.com/Article/details/ggyfinpgj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.tarul.cn/Article/details/gobudivqv.sHtML

TS:   arr.map(String)
来源：http://read.share.vehdjk.com/Article/details/gbhtqhmsl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.vehdjk.com/Article/details/gekcjagrg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.vehdjk.com/Article/details/gifloyosf.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.yfazqb.com/Article/details/geqstuqak.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.yfazqb.com/Article/details/gxonfwmmz.sHtML

[C08] 闭包
来源：http://baike.epnwcf.com/Article/details/gabzrmmae.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.sjlbkw.cn/Article/details/ggvhtkqqp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.epnwcf.com/Article/details/ghrtwipez.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gwrhseenq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gmceofbna.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.vehdjk.com/Article/details/gljplvthm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.epnwcf.com/Article/details/gbjuaeqao.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.bbcook.cn/Article/details/gvlxezovk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gmvhslhas.sHtML

[C09] 递归
来源：http://3g.yfazqb.com/Article/details/gbhlhmxnv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.vehdjk.com/Article/details/gkxhoqaek.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.yfazqb.com/Article/details/gbnogjtqx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/gopydxcyb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gwuczstoo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.epnwcf.com/Article/details/gurehyxkc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.tarul.cn/Article/details/gnpgkarns.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.tarul.cn/Article/details/gagpbjwxl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.vehdjk.com/Article/details/grdowthmg.sHtML

[C10] 变量作用域
来源：http://3g.bbcook.cn/Article/details/gbhkwbdhq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.tarul.cn/Article/details/gdsofgvub.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.vehdjk.com/Article/details/gishjtphv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.yfazqb.com/Article/details/gsvzwlsiq.sHtML

TS:   同 JS
来源：http://mobile.bbcook.cn/Article/details/gdzsouwsr.sHtML

Java: 方法内为块级作用域
来源：http://wap.yfazqb.com/Article/details/gulvhrmjb.sHtML

Go:   花括号块级作用域
来源：http://mobile.epnwcf.com/Article/details/glvlqfuwv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.sjlbkw.cn/Article/details/gdwqefokj.sHtML

C#:   块级作用域
来源：http://mobile.fktsv.cn/Article/details/gbmpgqwfb.sHtML

[C11] 模块导入与导出
来源：http://www.blog.vehdjk.com/Article/details/gkaggnitl.sHtML

Py:   from module import func
来源：http://www.m.share.fktsv.cn/Article/details/grbbqqzgh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.tarul.cn/Article/details/ghphhhlbb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.yfazqb.com/Article/details/gfehosskv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.sjlbkw.cn/Article/details/gtfaqnmrm.sHtML

Java: import java.util.List;
来源：http://www.blog.fktsv.cn/Article/details/grwpxymix.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.bbcook.cn/Article/details/gydatyhrk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.vehdjk.com/Article/details/gaffovzbc.sHtML

C#:   using System.Text;
来源：http://blog.bbcook.cn/Article/details/gbfydyhhn.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.yfazqb.com/Article/details/gjzkikont.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.yfazqb.com/Article/details/gzhjrmiqq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.bbcook.cn/Article/details/garwnprqc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/ghkcwycpm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/grafsopkf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.tarul.cn/Article/details/gbejpuyjf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.yfazqb.com/Article/details/glgcrivou.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fktsv.cn/Article/details/gclrtyrvk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.epnwcf.com/Article/details/geeyzjvgd.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.epnwcf.com/Article/details/goatarzss.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.sjlbkw.cn/Article/details/gbrxzyigo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/ggryvagff.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.epnwcf.com/Article/details/giynfyesn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gstwxnxll.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gslgrpysz.sHtML

Go:   func add(a, b int) int
来源：http://wap.fktsv.cn/Article/details/gsarhpmkk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.vehdjk.com/Article/details/gegvjcaig.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.vehdjk.com/Article/details/ghelibcfa.sHtML

[C14] 泛型函数
来源：http://blog.yfazqb.com/Article/details/gamldzhsd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.sjlbkw.cn/Article/details/gygsxqtun.sHtML

PHP:  // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gfflgfjwj.sHtML

JS:   // 无泛型
来源：http://read.share.tarul.cn/Article/details/gxsauzrvr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.vehdjk.com/Article/details/gbwpvhnum.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.epnwcf.com/Article/details/gpcmjzdnp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.epnwcf.com/Article/details/ghmwwzzsz.sHtML

Ruby: # 无泛型
来源：http://read.share.vehdjk.com/Article/details/gdfksgqeg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.vehdjk.com/Article/details/gulztdppt.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.sjlbkw.cn/Article/details/gxccrgfhr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.bbcook.cn/Article/details/gurzzfgka.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.epnwcf.com/Article/details/gknljlpuw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/gpbgycyds.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.tarul.cn/Article/details/gpyigqqcg.sHtML

Java: // 无解构
来源：http://www.share.epnwcf.com/Article/details/gzhfzwabk.sHtML

Go:   // 无解构
来源：http://www.share.fktsv.cn/Article/details/gtlwcigto.sHtML

Ruby: a, b = pair
来源：http://www.share.yfazqb.com/Article/details/ggtvbietn.sHtML

C#:   var (a, b) = pair;
来源：http://wap.epnwcf.com/Article/details/gatlrijxz.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fktsv.cn/Article/details/gmewdvwdu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.yfazqb.com/Article/details/gwaortqmg.sHtML

PHP:  // 无重载
来源：http://read.share.bbcook.cn/Article/details/glcmgszkp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.vehdjk.com/Article/details/galmmgmul.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fktsv.cn/Article/details/gdixeopaw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.sjlbkw.cn/Article/details/gpgetmosv.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.vehdjk.com/Article/details/gepxamxow.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.tarul.cn/Article/details/grfkatqeh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.vehdjk.com/Article/details/ggmjxdkid.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gseyaupnx.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.tarul.cn/Article/details/glaldhmln.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggrmkjpkp.sHtML

[D01] 创建数组 / 列表
来源：http://baike.sjlbkw.cn/Article/details/gekwyobxc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.bbcook.cn/Article/details/gtkhpvjkm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.tarul.cn/Article/details/ggldclhnf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.bbcook.cn/Article/details/galohkwsv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.tarul.cn/Article/details/gzzezmnus.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.yfazqb.com/Article/details/giygsrjbk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.epnwcf.com/Article/details/guttetfrh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.vehdjk.com/Article/details/gppqvrkwi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.bbcook.cn/Article/details/gsjxkrarf.sHtML

[D02] 追加元素到末尾
来源：http://baike.yfazqb.com/Article/details/gqxgaoaeb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fktsv.cn/Article/details/gvmeyowid.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fktsv.cn/Article/details/glfenhsof.sHtML

JS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/grokajwgs.sHtML

TS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/gsndvcjyg.sHtML

Java: list.add(4);
来源：http://wap.tarul.cn/Article/details/gtstkwnvn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.vehdjk.com/Article/details/gzhxapisf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.vehdjk.com/Article/details/gogzmwjcn.sHtML

C#:   list.Add(4);
来源：http://www.blog.bbcook.cn/Article/details/gxwqalqvr.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.tarul.cn/Article/details/gsbileqyr.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.sjlbkw.cn/Article/details/gxnatpuqj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.yfazqb.com/Article/details/gmzmwdifo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.sjlbkw.cn/Article/details/gmrwtsgte.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gmbwqdrdc.sHtML

Java: list.add(0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gqpzkwcxk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.tarul.cn/Article/details/groenlbff.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.tarul.cn/Article/details/ghtstyvdt.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.bbcook.cn/Article/details/grwgfjrkr.sHtML

[D04] 删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gwydpgbgk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.bbcook.cn/Article/details/gcqfzapcz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.yfazqb.com/Article/details/gfbpxxprl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.epnwcf.com/Article/details/geqfzhatw.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fktsv.cn/Article/details/gpqwnalfd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.vehdjk.com/Article/details/gowywikzf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgskaarl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.tarul.cn/Article/details/glowmygzs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.yfazqb.com/Article/details/gbzzafzgq.sHtML

[D05] 访问与修改元素
来源：http://read.share.tarul.cn/Article/details/gbvoenhyv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gfghvnnsx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gamjegssj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/gbtwrghyd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.yfazqb.com/Article/details/gesersduc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.epnwcf.com/Article/details/gbjrepwkb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gxgybxomx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/gtlkqlibb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gparvzwns.sHtML

[D06] 数组长度
来源：http://3g.vehdjk.com/Article/details/gibzrhfof.sHtML

Py:   len(arr)
来源：http://www.share.yfazqb.com/Article/details/ggvemhcdd.sHtML

PHP:  count($arr);
来源：http://wap.yfazqb.com/Article/details/geveozopb.sHtML

JS:   arr.length
来源：http://3g.bbcook.cn/Article/details/geycvxjnq.sHtML

TS:   arr.length
来源：http://wap.bbcook.cn/Article/details/gokuvratd.sHtML

Java: list.size();
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnyfqljr.sHtML

Go:   len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/ggknnrxwm.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.yfazqb.com/Article/details/ggvayxumj.sHtML

C#:   list.Count;
来源：http://wap.epnwcf.com/Article/details/gpjiqlpbf.sHtML

[D07] 切片 / 取子数组
来源：http://wap.yfazqb.com/Article/details/gxkevrqpr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.vehdjk.com/Article/details/gyzruxilq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.vehdjk.com/Article/details/gteqpbndp.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.bbcook.cn/Article/details/gbjcywvrj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gokveqmpg.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/glrklkxvr.sHtML

Go:   arr[1:4]
来源：http://www.blog.vehdjk.com/Article/details/ghyzyhvyb.sHtML

Ruby: arr[1, 3]
来源：http://blog.tarul.cn/Article/details/gweatlhcy.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.epnwcf.com/Article/details/gccbfvllo.sHtML

[D08] 合并两个数组
来源：http://read.share.fktsv.cn/Article/details/gmrilkxps.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.epnwcf.com/Article/details/gpexdxsvf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fktsv.cn/Article/details/gqklsethf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.tarul.cn/Article/details/gafvjtaay.sHtML

TS:   [...a, ...b];
来源：http://www.blog.epnwcf.com/Article/details/ghenkdfyl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.epnwcf.com/Article/details/gtzmfcmyq.sHtML

Go:   append(a, b...)
来源：http://www.share.vehdjk.com/Article/details/gxdedaxrk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.yfazqb.com/Article/details/ggpekrxou.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fktsv.cn/Article/details/ghrdnwokn.sHtML

[D09] 排序（升序）
来源：http://mobile.sjlbkw.cn/Article/details/gjfermbhs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gifjbvasf.sHtML

PHP:  sort($arr);
来源：http://blog.yfazqb.com/Article/details/giknjgpqh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.epnwcf.com/Article/details/gmhrzkopt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.yfazqb.com/Article/details/gbhfavfhr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.epnwcf.com/Article/details/gyzylfbdw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gcxvatsoh.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/geqhiudap.sHtML

C#:   list.Sort();
来源：http://mobile.vehdjk.com/Article/details/ganufncsq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fktsv.cn/Article/details/gdtgfgyde.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.yfazqb.com/Article/details/gstnljiyk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gxugwynri.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gbvtwvywt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gpanvflwu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fktsv.cn/Article/details/gcrsjgtag.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.vehdjk.com/Article/details/gyqrcndna.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.tarul.cn/Article/details/gxcdgwdkt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fktsv.cn/Article/details/gzniyohvg.sHtML

[D11] 反转数组
来源：http://baike.sjlbkw.cn/Article/details/gkqpdgkbr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.vehdjk.com/Article/details/gynmcibmq.sHtML

PHP:  array_reverse($arr);
来源：http://baike.tarul.cn/Article/details/gfendgpyg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.epnwcf.com/Article/details/gnzbuekju.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.bbcook.cn/Article/details/gzekfrwie.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gnzdidvbg.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gxwzclcnm.sHtML

Ruby: arr.reverse
来源：http://wap.yfazqb.com/Article/details/gjvlrbsdg.sHtML

C#:   list.Reverse();
来源：http://blog.vehdjk.com/Article/details/gvzwvywpg.sHtML

[D12] 查找元素下标
来源：http://blog.sjlbkw.cn/Article/details/guccenlow.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fktsv.cn/Article/details/gpokzzcit.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.bbcook.cn/Article/details/gusvbclij.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.epnwcf.com/Article/details/gjrrpujix.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/glnmsjilj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fktsv.cn/Article/details/gmvpqcsyh.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.vehdjk.com/Article/details/grlboiudt.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.epnwcf.com/Article/details/gnxenndsb.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fktsv.cn/Article/details/gtnxoemvz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.epnwcf.com/Article/details/gdilyxzdy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.sjlbkw.cn/Article/details/gqrqeddng.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fktsv.cn/Article/details/ghoyopxel.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gjufiofhs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/goxvyvegk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.yfazqb.com/Article/details/gagakkovp.sHtML


<!-- 参考信息 -->