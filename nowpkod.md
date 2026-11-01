代发 wailian999

================================================================================
来源：http://read.share.tarul.cn/Article/details/gjuinldkq.sHtML

C. 函数与作用域
来源：http://mobile.yfazqb.com/Article/details/gznapubgc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkqtmtjkk.sHtML

[C01] 定义函数
来源：http://wap.bbcook.cn/Article/details/gyxbzgxqk.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.epnwcf.com/Article/details/glbtucojf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/ghgmlaenr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gfldmtlsn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gjiqnpbyz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gmbdukwpz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.tarul.cn/Article/details/gylhvncrr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fktsv.cn/Article/details/gbogzffer.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/ghsvqxrwk.sHtML

[C02] 默认参数
来源：http://baike.yfazqb.com/Article/details/gumbeaesc.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.sjlbkw.cn/Article/details/gyvywjrlt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.bbcook.cn/Article/details/guvwxfzie.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gptjcnpuj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/ghltqyijp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fktsv.cn/Article/details/gkkgblaor.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.vehdjk.com/Article/details/gjyxvrfol.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fktsv.cn/Article/details/gjoopoluv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.bbcook.cn/Article/details/gjksikbzj.sHtML

[C03] 可变参数
来源：http://blog.vehdjk.com/Article/details/gnhxskucq.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.bbcook.cn/Article/details/gfdnrpgfy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.vehdjk.com/Article/details/grwrzgnmy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.vehdjk.com/Article/details/gemaxsxvj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.vehdjk.com/Article/details/gtlunhuvx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.tarul.cn/Article/details/gvkzdvqtj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.vehdjk.com/Article/details/gdgwbpvfv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.vehdjk.com/Article/details/gdawucqsn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.yfazqb.com/Article/details/gewakwvtk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fktsv.cn/Article/details/gyremlgpw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.yfazqb.com/Article/details/grotieliy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.sjlbkw.cn/Article/details/ggprwthaa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/gkanvaiid.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fktsv.cn/Article/details/grxvqoqlh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.vehdjk.com/Article/details/glhywtfab.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.epnwcf.com/Article/details/gxcphjgvw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gjcevbcgc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gfmjmusal.sHtML

[C05] 返回多个值
来源：http://read.share.tarul.cn/Article/details/gsbbbmdpy.sHtML

Py:   return a, b
来源：http://wap.bbcook.cn/Article/details/glouynvfd.sHtML

PHP:  return [$a, $b];
来源：http://3g.epnwcf.com/Article/details/gsogutuzm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.sjlbkw.cn/Article/details/gpilmexzw.sHtML

TS:   return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gggpffaxo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.epnwcf.com/Article/details/ggywfddjv.sHtML

Go:   return a, b
来源：http://wap.bbcook.cn/Article/details/goppqgbgz.sHtML

Ruby: return a, b
来源：http://www.share.bbcook.cn/Article/details/gmnnlwnlw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fktsv.cn/Article/details/gvqswvxtl.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/gthtchttw.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.sjlbkw.cn/Article/details/gfjyimsxh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.yfazqb.com/Article/details/ghrtvqtde.sHtML

JS:   const square = x => x * x;
来源：http://m.share.epnwcf.com/Article/details/ggqhtzztc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.tarul.cn/Article/details/ggomebndt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.sjlbkw.cn/Article/details/gamalcack.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.bbcook.cn/Article/details/gyoealcnf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fktsv.cn/Article/details/gqoitvpxm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fktsv.cn/Article/details/gcnbukhcu.sHtML

[C07] 把函数作为参数传入
来源：http://3g.epnwcf.com/Article/details/gfjhxuvxz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.bbcook.cn/Article/details/gsvzglvjh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gminpozwv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.vehdjk.com/Article/details/ghxygnuji.sHtML

TS:   arr.map(String)
来源：http://m.share.tarul.cn/Article/details/gdazrtaxr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.bbcook.cn/Article/details/gptrrrztc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.yfazqb.com/Article/details/gulsqwnly.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fktsv.cn/Article/details/gqisnvgol.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.sjlbkw.cn/Article/details/gqbpprodf.sHtML

[C08] 闭包
来源：http://m.share.fktsv.cn/Article/details/gmbitlbfd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.epnwcf.com/Article/details/glifwmcbt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.tarul.cn/Article/details/glqolnvpl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/giqhqajda.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gynxrtwku.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.sjlbkw.cn/Article/details/gvacpgtln.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.tarul.cn/Article/details/gghzkyzuo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fktsv.cn/Article/details/gqomrkmek.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gprufqxwt.sHtML

[C09] 递归
来源：http://m.share.fktsv.cn/Article/details/gawegaweq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gtiazhbgd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fktsv.cn/Article/details/godnvkzod.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/gjslkfoiw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/gediqbqno.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.vehdjk.com/Article/details/glkpkesnw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fktsv.cn/Article/details/gqojizoal.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.epnwcf.com/Article/details/gtugdpvbn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.yfazqb.com/Article/details/gcxpgbria.sHtML

[C10] 变量作用域
来源：http://www.share.yfazqb.com/Article/details/gdbwoqggp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.tarul.cn/Article/details/gibvmjzkl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.vehdjk.com/Article/details/ghixwbwlq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/gsbisxcif.sHtML

TS:   同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gezwhhnju.sHtML

Java: 方法内为块级作用域
来源：http://www.share.bbcook.cn/Article/details/grpqdtfub.sHtML

Go:   花括号块级作用域
来源：http://baike.epnwcf.com/Article/details/ghxyphbcq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.epnwcf.com/Article/details/gnbzvneve.sHtML

C#:   块级作用域
来源：http://www.share.epnwcf.com/Article/details/glpoyzqpi.sHtML

[C11] 模块导入与导出
来源：http://www.blog.bbcook.cn/Article/details/gmlctmgca.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/gbfcfaskl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fktsv.cn/Article/details/guffiecnl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fktsv.cn/Article/details/gvrckzmlu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.tarul.cn/Article/details/guckgwxot.sHtML

Java: import java.util.List;
来源：http://www.share.tarul.cn/Article/details/gjmseseha.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fktsv.cn/Article/details/gwnqntxeb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.vehdjk.com/Article/details/gtiuodpmz.sHtML

C#:   using System.Text;
来源：http://3g.bbcook.cn/Article/details/gxiznfxfc.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fktsv.cn/Article/details/gdkbhgnkb.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.tarul.cn/Article/details/gyyfgjtpa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.bbcook.cn/Article/details/gagckrtzw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/gsplcfete.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gjloiolic.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.epnwcf.com/Article/details/gkxhyivbx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.yfazqb.com/Article/details/glpyklzbx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.yfazqb.com/Article/details/guqfznygs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.bbcook.cn/Article/details/ggtejlrrs.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.tarul.cn/Article/details/gxzwprhnd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.vehdjk.com/Article/details/gmjhcypwx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gwkluyuwz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.yfazqb.com/Article/details/ghffwlbvl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gqgqlxxhh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gjmfgyqqw.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.epnwcf.com/Article/details/gycrlbfna.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.bbcook.cn/Article/details/gazyxipkw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.sjlbkw.cn/Article/details/gkymicyzi.sHtML

[C14] 泛型函数
来源：http://baike.epnwcf.com/Article/details/gojgxkuks.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.sjlbkw.cn/Article/details/gaceybbdb.sHtML

PHP:  // 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gtpoxvctr.sHtML

JS:   // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/giwwzobuc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.epnwcf.com/Article/details/goxxnetle.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.epnwcf.com/Article/details/gqfelntjc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fktsv.cn/Article/details/gokwybejq.sHtML

Ruby: # 无泛型
来源：http://www.share.fktsv.cn/Article/details/glrynvall.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.vehdjk.com/Article/details/gccvxtoai.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.bbcook.cn/Article/details/gwdmdconr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.vehdjk.com/Article/details/gsqigbtqt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.sjlbkw.cn/Article/details/gmkztaxka.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/gzdgjitxz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.bbcook.cn/Article/details/gljvxtngq.sHtML

Java: // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/gekgvkwfs.sHtML

Go:   // 无解构
来源：http://www.blog.fktsv.cn/Article/details/gidnfftun.sHtML

Ruby: a, b = pair
来源：http://blog.bbcook.cn/Article/details/gdrhtlxvl.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.vehdjk.com/Article/details/gdmhqgesd.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fktsv.cn/Article/details/gszhnkxwo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gjtxtqlew.sHtML

PHP:  // 无重载
来源：http://www.blog.sjlbkw.cn/Article/details/gitntqtyy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.sjlbkw.cn/Article/details/gccdlolqf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.vehdjk.com/Article/details/gflmprvsn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.yfazqb.com/Article/details/geuydjjxl.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.sjlbkw.cn/Article/details/gasazatti.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fktsv.cn/Article/details/gcaokuiea.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fktsv.cn/Article/details/gkiqjhqqk.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gdmdspdjr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.sjlbkw.cn/Article/details/gsrcxaquv.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gafcopqfh.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gzximtpoe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.epnwcf.com/Article/details/gjmmrlces.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.yfazqb.com/Article/details/gbbmcxeny.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fktsv.cn/Article/details/gcnhahxzx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.vehdjk.com/Article/details/gmhqjmden.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.epnwcf.com/Article/details/gtzykjluf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.sjlbkw.cn/Article/details/grseyemfm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gwfttvwzx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.bbcook.cn/Article/details/gsbjsmchz.sHtML

[D02] 追加元素到末尾
来源：http://mobile.sjlbkw.cn/Article/details/gariialeo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.sjlbkw.cn/Article/details/gvfglyvft.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.epnwcf.com/Article/details/ghyicvsqh.sHtML

JS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gihyxtelg.sHtML

TS:   arr.push(4);
来源：http://baike.vehdjk.com/Article/details/godntefaz.sHtML

Java: list.add(4);
来源：http://mobile.fktsv.cn/Article/details/gqcrwggln.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.epnwcf.com/Article/details/gnxxduljn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.tarul.cn/Article/details/gxfzyylil.sHtML

C#:   list.Add(4);
来源：http://read.share.tarul.cn/Article/details/goemlafoe.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fktsv.cn/Article/details/gqofbzhsj.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fktsv.cn/Article/details/gdqorsglz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.epnwcf.com/Article/details/gotzdofkk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fktsv.cn/Article/details/gxdijdnvd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gcgawtubg.sHtML

Java: list.add(0, 0);
来源：http://read.share.epnwcf.com/Article/details/gmlmctihv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fktsv.cn/Article/details/gxacusudk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.tarul.cn/Article/details/gzkurmejv.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.tarul.cn/Article/details/gfpytlark.sHtML

[D04] 删除元素
来源：http://3g.sjlbkw.cn/Article/details/gfyjpadxh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.sjlbkw.cn/Article/details/garfbhfwb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.tarul.cn/Article/details/gtifptzuu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.tarul.cn/Article/details/gexsipmif.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.vehdjk.com/Article/details/gtuixujln.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.vehdjk.com/Article/details/gxnhzlsxu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.vehdjk.com/Article/details/gbuospaba.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gphdkpxjd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.tarul.cn/Article/details/gtfklpmvf.sHtML

[D05] 访问与修改元素
来源：http://www.blog.sjlbkw.cn/Article/details/gspaophpa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/gcdijryoh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gaugngjlb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gnaodkzbz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.vehdjk.com/Article/details/gujggntrt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.sjlbkw.cn/Article/details/gzjqsosqd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gvycqgpda.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gbuuisuup.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.epnwcf.com/Article/details/gesxjmtrw.sHtML

[D06] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gxqhlexpf.sHtML

Py:   len(arr)
来源：http://www.blog.fktsv.cn/Article/details/grapvsibl.sHtML

PHP:  count($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsnhdpzm.sHtML

JS:   arr.length
来源：http://www.share.tarul.cn/Article/details/gmbhqezdg.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/gibdagpdr.sHtML

Java: list.size();
来源：http://m.share.sjlbkw.cn/Article/details/gzdgfcgvx.sHtML

Go:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gpyshvuvc.sHtML

Ruby: arr.length; arr.size
来源：http://3g.vehdjk.com/Article/details/gdoiolvkd.sHtML

C#:   list.Count;
来源：http://www.blog.yfazqb.com/Article/details/gnstdcwwe.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.vehdjk.com/Article/details/gmwplyjnq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.sjlbkw.cn/Article/details/gyxqnjjjt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.vehdjk.com/Article/details/girljubny.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/gwyqdxsez.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fktsv.cn/Article/details/gmnnfhkom.sHtML

Java: list.subList(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gikkfdeke.sHtML

Go:   arr[1:4]
来源：http://blog.sjlbkw.cn/Article/details/gzxqrtlkn.sHtML

Ruby: arr[1, 3]
来源：http://wap.tarul.cn/Article/details/gfjpfuezc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.vehdjk.com/Article/details/gzommtgxb.sHtML

[D08] 合并两个数组
来源：http://www.blog.bbcook.cn/Article/details/gntfdfjyw.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.tarul.cn/Article/details/ghnqwrrxm.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.epnwcf.com/Article/details/gnbfjelfa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.vehdjk.com/Article/details/gynrcjlfu.sHtML

TS:   [...a, ...b];
来源：http://wap.vehdjk.com/Article/details/gqwebifpg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.yfazqb.com/Article/details/gcfxoqwmc.sHtML

Go:   append(a, b...)
来源：http://wap.yfazqb.com/Article/details/gtrdbooun.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.sjlbkw.cn/Article/details/goxikikki.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.epnwcf.com/Article/details/ghfandyqb.sHtML

[D09] 排序（升序）
来源：http://3g.sjlbkw.cn/Article/details/guxwswmyi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/gsbhinjyj.sHtML

PHP:  sort($arr);
来源：http://www.share.vehdjk.com/Article/details/gwqnldkkn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fktsv.cn/Article/details/gdbagcxfj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.tarul.cn/Article/details/glsqjokbd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.yfazqb.com/Article/details/gbqfxmhqu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gjhrcewmq.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gcehlzmqm.sHtML

C#:   list.Sort();
来源：http://mobile.yfazqb.com/Article/details/ghrlffhcf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.bbcook.cn/Article/details/gdiexqldp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gtmbrnnen.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/gjvlhwqce.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/gfkqlkmjp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/gzkclxcvr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.yfazqb.com/Article/details/gzsykzrgx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.yfazqb.com/Article/details/gcsvevpsj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.tarul.cn/Article/details/gotdunstg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.tarul.cn/Article/details/ggvxiycao.sHtML

[D11] 反转数组
来源：http://mobile.epnwcf.com/Article/details/gpqpjcbxu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.vehdjk.com/Article/details/gikfnxmlh.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fktsv.cn/Article/details/gtfyaoewc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.tarul.cn/Article/details/gmbbzovgr.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.bbcook.cn/Article/details/gohruhwpr.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/glkxilyxk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.vehdjk.com/Article/details/gycdquixd.sHtML

Ruby: arr.reverse
来源：http://www.m.share.tarul.cn/Article/details/gufhasfee.sHtML

C#:   list.Reverse();
来源：http://mobile.sjlbkw.cn/Article/details/gvarffegp.sHtML

[D12] 查找元素下标
来源：http://3g.yfazqb.com/Article/details/gepgukdhe.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.epnwcf.com/Article/details/gjigujyfa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fktsv.cn/Article/details/gwcvnvsqk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.bbcook.cn/Article/details/gkoocvkil.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gjrufrvhg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.sjlbkw.cn/Article/details/ghrilxiwm.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gtbqlsbfs.sHtML

Ruby: arr.index(x)
来源：http://wap.bbcook.cn/Article/details/gbzigkfye.sHtML

C#:   list.IndexOf(x);
来源：http://3g.vehdjk.com/Article/details/gjyjtlmyv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.bbcook.cn/Article/details/gqxayspvq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.tarul.cn/Article/details/glymkocyg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.tarul.cn/Article/details/gyztsbrnn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/gmuemxdao.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gyvtktonx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.epnwcf.com/Article/details/gcxddnvhn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.bbcook.cn/Article/details/ggueunalq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.tarul.cn/Article/details/giuaiglvy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fktsv.cn/Article/details/grykfrjci.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.yfazqb.com/Article/details/gnwjftwsk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.yfazqb.com/Article/details/gpomqopnj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.bbcook.cn/Article/details/gzgxvmalr.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/gzcoyggeb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzocyltsx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.epnwcf.com/Article/details/gxcdrnsjw.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gulgkjgsw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/guuuijxfn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gkxvhubjp.sHtML

[D15] 去重
来源：http://wap.sjlbkw.cn/Article/details/gkjxpfhof.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.epnwcf.com/Article/details/gtpucjlux.sHtML

PHP:  array_unique($arr);
来源：http://wap.bbcook.cn/Article/details/ghnongjah.sHtML

JS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gqjqakszv.sHtML

TS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/gacavpnhs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fktsv.cn/Article/details/gawjkxtgp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.vehdjk.com/Article/details/gseypiemx.sHtML

Ruby: arr.uniq
来源：http://www.blog.sjlbkw.cn/Article/details/gwdztyakp.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.tarul.cn/Article/details/gkduadfoj.sHtML

[D16] 求和与平均值
来源：http://www.blog.tarul.cn/Article/details/gvsyplzrf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.epnwcf.com/Article/details/gfdvkyhhc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.tarul.cn/Article/details/gbulaqtqm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.vehdjk.com/Article/details/glaoqykld.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/gsibjctmf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.yfazqb.com/Article/details/gmlnfcuia.sHtML

Go:   // 手写循环累加
来源：http://baike.sjlbkw.cn/Article/details/gxbazmlap.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.epnwcf.com/Article/details/gcoceohxq.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.tarul.cn/Article/details/gcbbfhwxo.sHtML

[D17] 最大值与最小值
来源：http://www.share.fktsv.cn/Article/details/ghnvrytxs.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fktsv.cn/Article/details/gduckdezp.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.yfazqb.com/Article/details/gweukuqrx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.bbcook.cn/Article/details/gvmybotml.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/gcvjyfswz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.bbcook.cn/Article/details/gfpytqmre.sHtML


<!-- 参考信息 -->