代发 wailian999

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsgmopkpe.sHtML

C. 函数与作用域
来源：http://read.share.fktsv.cn/Article/details/gcuyirkzo.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gjcyazkbi.sHtML

[C01] 定义函数
来源：http://www.share.fktsv.cn/Article/details/glujafjqg.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.vehdjk.com/Article/details/gfixwciqc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gduqurxtt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gikaqzyzw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gctxuxahi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gqlguwqrg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/goriaistk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.sjlbkw.cn/Article/details/gzvbfgcau.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gbswctseh.sHtML

[C02] 默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gkovazidg.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.bbcook.cn/Article/details/gmjtqiwwl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.yfazqb.com/Article/details/gouzkbcyp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.vehdjk.com/Article/details/gbfienhvn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gyhxzjumf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.yfazqb.com/Article/details/gtqbiaand.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fktsv.cn/Article/details/gtjzxxgqr.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.yfazqb.com/Article/details/gfmeqlwuu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.tarul.cn/Article/details/gvywdjaqa.sHtML

[C03] 可变参数
来源：http://baike.fktsv.cn/Article/details/giseocjec.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.yfazqb.com/Article/details/gvnkscwfq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.yfazqb.com/Article/details/gkjzmifzx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/gkxigyfai.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/guwsiiibq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.sjlbkw.cn/Article/details/ghjcvcetw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fktsv.cn/Article/details/glapojzrw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fktsv.cn/Article/details/gytkotnjb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.epnwcf.com/Article/details/gbmtdcxan.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.bbcook.cn/Article/details/giveratgi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.vehdjk.com/Article/details/gyfsxzwhc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.epnwcf.com/Article/details/gjbkmwjfk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/gaxninooj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.vehdjk.com/Article/details/gdududohv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fktsv.cn/Article/details/gznzrmdiy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.vehdjk.com/Article/details/gnxjyqlwp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.vehdjk.com/Article/details/grwjtkpov.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gdflzxzoo.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/gznljpzvz.sHtML

Py:   return a, b
来源：http://baike.epnwcf.com/Article/details/gtkxmeclx.sHtML

PHP:  return [$a, $b];
来源：http://m.share.bbcook.cn/Article/details/grpuekdqh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gwydtevcw.sHtML

TS:   return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/gwjxkizux.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fktsv.cn/Article/details/gavmzvwnd.sHtML

Go:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/gfewgxvkv.sHtML

Ruby: return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gizhgwjne.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.epnwcf.com/Article/details/gbvqhvbbm.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/gmyveajgq.sHtML

Py:   square = lambda x: x * x
来源：http://baike.tarul.cn/Article/details/gqjdqrqqr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.epnwcf.com/Article/details/gtfkbcmlw.sHtML

JS:   const square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/gudetaosb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.epnwcf.com/Article/details/gabiycobo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.tarul.cn/Article/details/gcvlhxszk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.tarul.cn/Article/details/gxxfwxyfr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.tarul.cn/Article/details/gxpszuhll.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/gcqlqsmkw.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fktsv.cn/Article/details/gugwebopc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.bbcook.cn/Article/details/gqazxpqzz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.epnwcf.com/Article/details/gcwtgisgu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.bbcook.cn/Article/details/gnpgiahhe.sHtML

TS:   arr.map(String)
来源：http://www.blog.tarul.cn/Article/details/gsrfuotqw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.tarul.cn/Article/details/givkmtxml.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.tarul.cn/Article/details/grhvjxtkq.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.sjlbkw.cn/Article/details/glcqmzhnx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.tarul.cn/Article/details/gzggidykk.sHtML

[C08] 闭包
来源：http://www.m.share.epnwcf.com/Article/details/gfyirxmte.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.yfazqb.com/Article/details/ggugtugnp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.tarul.cn/Article/details/guflwqwfn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gosapokkf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gufuytnmb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.vehdjk.com/Article/details/gnyphqeqj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.bbcook.cn/Article/details/gnzkfqute.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.vehdjk.com/Article/details/guwpezotk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/gspccxoom.sHtML

[C09] 递归
来源：http://baike.vehdjk.com/Article/details/gogxtttiu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/ghcrmnfwg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gwqgczozi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/gpztogxrf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.tarul.cn/Article/details/gzttwnmid.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/gatrauxho.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fktsv.cn/Article/details/gblbgfuwn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.tarul.cn/Article/details/grbtzbudr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.bbcook.cn/Article/details/guczvltcd.sHtML

[C10] 变量作用域
来源：http://mobile.vehdjk.com/Article/details/gzccwixgg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.vehdjk.com/Article/details/godrlmndv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.sjlbkw.cn/Article/details/grewgxluv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fktsv.cn/Article/details/gtcpptnuc.sHtML

TS:   同 JS
来源：http://mobile.yfazqb.com/Article/details/gmkzplmkn.sHtML

Java: 方法内为块级作用域
来源：http://m.share.bbcook.cn/Article/details/gpfrqkanj.sHtML

Go:   花括号块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gcvldaroq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.vehdjk.com/Article/details/gxysdbwqq.sHtML

C#:   块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gpphueudo.sHtML

[C11] 模块导入与导出
来源：http://read.share.fktsv.cn/Article/details/gujjwuhwa.sHtML

Py:   from module import func
来源：http://3g.yfazqb.com/Article/details/glqtemcim.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fktsv.cn/Article/details/glsjbndbm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.yfazqb.com/Article/details/gsdefrman.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.bbcook.cn/Article/details/griqioxuu.sHtML

Java: import java.util.List;
来源：http://www.share.tarul.cn/Article/details/guirojvyh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.sjlbkw.cn/Article/details/gvxsxpmlm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.epnwcf.com/Article/details/gagayiray.sHtML

C#:   using System.Text;
来源：http://read.share.vehdjk.com/Article/details/gknkuocrv.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.tarul.cn/Article/details/gfhwwoaph.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.epnwcf.com/Article/details/gpidtahsv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fktsv.cn/Article/details/gcuytwjlz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/grfyosryr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/gpmdtwink.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.epnwcf.com/Article/details/gtembqlut.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.tarul.cn/Article/details/grjasopac.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.tarul.cn/Article/details/gljhhtueh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fktsv.cn/Article/details/gmzxkhcci.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.bbcook.cn/Article/details/gpzkmyxxu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.sjlbkw.cn/Article/details/gpergxbth.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gbxqzllln.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.tarul.cn/Article/details/gaypvncjs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gurujtfim.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gmvgbugpk.sHtML

Go:   func add(a, b int) int
来源：http://wap.sjlbkw.cn/Article/details/gfkrgpmjd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.epnwcf.com/Article/details/gnkoxoirh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.sjlbkw.cn/Article/details/gxgpdacjo.sHtML

[C14] 泛型函数
来源：http://read.share.sjlbkw.cn/Article/details/gyjaupqbq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.tarul.cn/Article/details/gzpwosuyw.sHtML

PHP:  // 无泛型
来源：http://3g.tarul.cn/Article/details/gxgakmwfg.sHtML

JS:   // 无泛型
来源：http://m.share.epnwcf.com/Article/details/gfdkoizkf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.tarul.cn/Article/details/gbrqwsykr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.yfazqb.com/Article/details/gahaedpmu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fktsv.cn/Article/details/gupzsvtaz.sHtML

Ruby: # 无泛型
来源：http://m.share.vehdjk.com/Article/details/grzqrltgk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.bbcook.cn/Article/details/gatdnshag.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.yfazqb.com/Article/details/gvgflhkon.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.vehdjk.com/Article/details/gzehbudju.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.bbcook.cn/Article/details/grnakavrg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.epnwcf.com/Article/details/gjbugwafy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gvpskbkfv.sHtML

Java: // 无解构
来源：http://read.share.tarul.cn/Article/details/gkmvxianc.sHtML

Go:   // 无解构
来源：http://www.share.sjlbkw.cn/Article/details/gofflfxxu.sHtML

Ruby: a, b = pair
来源：http://mobile.fktsv.cn/Article/details/gxawsxxkt.sHtML

C#:   var (a, b) = pair;
来源：http://baike.tarul.cn/Article/details/gwxhpqweg.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.epnwcf.com/Article/details/gvtrovadg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fktsv.cn/Article/details/gzvdosmse.sHtML

PHP:  // 无重载
来源：http://baike.bbcook.cn/Article/details/gqzwctqtr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.tarul.cn/Article/details/gtffczjcv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.sjlbkw.cn/Article/details/gdszxfnkd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.vehdjk.com/Article/details/gfezobczp.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.bbcook.cn/Article/details/glfvpennn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.sjlbkw.cn/Article/details/gpymuxafm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.sjlbkw.cn/Article/details/gkhfrtjfx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gywvpuubx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fktsv.cn/Article/details/glcifbrhs.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmhamelak.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fktsv.cn/Article/details/gxqpzdgpe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.vehdjk.com/Article/details/ghoeiarwk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/gefynaasd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.bbcook.cn/Article/details/gqtcjjhyu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fktsv.cn/Article/details/gaosmgbot.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.epnwcf.com/Article/details/gevyxofif.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.sjlbkw.cn/Article/details/gzgysrxck.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.yfazqb.com/Article/details/ggiaroidl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.vehdjk.com/Article/details/gsbctcjyx.sHtML

[D02] 追加元素到末尾
来源：http://wap.tarul.cn/Article/details/gbpatdvpm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/gbgyhvtug.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.sjlbkw.cn/Article/details/gxlugdehc.sHtML

JS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/gzitqxgbc.sHtML

TS:   arr.push(4);
来源：http://www.blog.fktsv.cn/Article/details/gcqalnvxa.sHtML

Java: list.add(4);
来源：http://www.share.epnwcf.com/Article/details/gtfdmhaof.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.bbcook.cn/Article/details/gpvskdaww.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fktsv.cn/Article/details/gcfryvzyy.sHtML

C#:   list.Add(4);
来源：http://www.share.sjlbkw.cn/Article/details/gcbiqrcai.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.tarul.cn/Article/details/gyczwgody.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.bbcook.cn/Article/details/ggqnhqpdg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.bbcook.cn/Article/details/gmsdcpeot.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.sjlbkw.cn/Article/details/gezjjxoxb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.epnwcf.com/Article/details/gjnqeaqpt.sHtML

Java: list.add(0, 0);
来源：http://3g.yfazqb.com/Article/details/goxsyqigc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.bbcook.cn/Article/details/gelqbrlrp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.tarul.cn/Article/details/gbesdoxxw.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.yfazqb.com/Article/details/gockbezil.sHtML

[D04] 删除元素
来源：http://read.share.fktsv.cn/Article/details/gtruxfgqb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.sjlbkw.cn/Article/details/gjubfbgnl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.yfazqb.com/Article/details/gczwiovuy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.yfazqb.com/Article/details/gpbsmyomv.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.sjlbkw.cn/Article/details/gedciwmrd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fktsv.cn/Article/details/gdmjmndod.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fktsv.cn/Article/details/gvbyxyels.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.yfazqb.com/Article/details/gikozqppd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fktsv.cn/Article/details/gbewzkqdp.sHtML

[D05] 访问与修改元素
来源：http://m.share.fktsv.cn/Article/details/gzwhbidsu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gzqcautmj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gghoupefh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.bbcook.cn/Article/details/gdgukfgld.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fktsv.cn/Article/details/gimjuqqmr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.vehdjk.com/Article/details/gxsivjzte.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gwvmbvarz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gfvwwbyps.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/glagyaxmj.sHtML

[D06] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/gcbfhbanc.sHtML

Py:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gsgevauhq.sHtML

PHP:  count($arr);
来源：http://blog.epnwcf.com/Article/details/gfygfrnju.sHtML

JS:   arr.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpnlfxej.sHtML

TS:   arr.length
来源：http://blog.bbcook.cn/Article/details/goilgvwkd.sHtML

Java: list.size();
来源：http://www.share.fktsv.cn/Article/details/gjfutxhok.sHtML

Go:   len(arr)
来源：http://3g.fktsv.cn/Article/details/gyoamwmyb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.bbcook.cn/Article/details/gtliurdss.sHtML

C#:   list.Count;
来源：http://m.share.tarul.cn/Article/details/gxugsqygr.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.tarul.cn/Article/details/gxamuxujd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.bbcook.cn/Article/details/gkyhfyxvx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gupbesajz.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gudquwfnq.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/gubixapzw.sHtML

Java: list.subList(1, 4);
来源：http://3g.vehdjk.com/Article/details/gabkutpxq.sHtML

Go:   arr[1:4]
来源：http://blog.vehdjk.com/Article/details/gsbjamcrk.sHtML

Ruby: arr[1, 3]
来源：http://blog.sjlbkw.cn/Article/details/gknpxmcpd.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.yfazqb.com/Article/details/gmqvfisky.sHtML

[D08] 合并两个数组
来源：http://www.m.share.yfazqb.com/Article/details/gmmfxxeia.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.tarul.cn/Article/details/ghlvwjlbu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.bbcook.cn/Article/details/grpovetim.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.sjlbkw.cn/Article/details/grinsiyvo.sHtML

TS:   [...a, ...b];
来源：http://read.share.sjlbkw.cn/Article/details/gqtqsvvvy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gkooqcywd.sHtML

Go:   append(a, b...)
来源：http://www.share.sjlbkw.cn/Article/details/gohamhwns.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.bbcook.cn/Article/details/ghnoqmcwc.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fktsv.cn/Article/details/gqtkmooto.sHtML

[D09] 排序（升序）
来源：http://baike.epnwcf.com/Article/details/guodlnieq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/ggxcwuusm.sHtML

PHP:  sort($arr);
来源：http://baike.epnwcf.com/Article/details/guikorhsq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.epnwcf.com/Article/details/gyvnyjfem.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.epnwcf.com/Article/details/gglygxtmf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.tarul.cn/Article/details/glswlgvzg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gjsuruwgf.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gpcixuxfs.sHtML

C#:   list.Sort();
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzrqfozq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.yfazqb.com/Article/details/gyflwpaki.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.tarul.cn/Article/details/gvcmmkyjb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/goigyygsw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gmihguupf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.epnwcf.com/Article/details/gdahlvmtz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.epnwcf.com/Article/details/gxzlctojv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.bbcook.cn/Article/details/ghkhdgwqu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.bbcook.cn/Article/details/gbankvfts.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.vehdjk.com/Article/details/gkickmujf.sHtML

[D11] 反转数组
来源：http://read.share.fktsv.cn/Article/details/gxztpqdwn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.yfazqb.com/Article/details/giziciayl.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fktsv.cn/Article/details/gvnrqlrtj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.bbcook.cn/Article/details/gnxnisiyn.sHtML

TS:   [...arr].reverse();
来源：http://3g.tarul.cn/Article/details/gcagwrfns.sHtML

Java: Collections.reverse(list);
来源：http://baike.vehdjk.com/Article/details/gloahjyet.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gfqrbzpho.sHtML

Ruby: arr.reverse
来源：http://mobile.fktsv.cn/Article/details/gvdmaksrf.sHtML

C#:   list.Reverse();
来源：http://3g.fktsv.cn/Article/details/grzffuggo.sHtML

[D12] 查找元素下标
来源：http://mobile.yfazqb.com/Article/details/gwgidneey.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.sjlbkw.cn/Article/details/gebyltcsj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.tarul.cn/Article/details/guyfltdhm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/gpjxmbvya.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gkgcerqed.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.vehdjk.com/Article/details/gzpematuc.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gcbmpjumz.sHtML

Ruby: arr.index(x)
来源：http://baike.tarul.cn/Article/details/gdamhuahs.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.tarul.cn/Article/details/gzunqjfby.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.vehdjk.com/Article/details/ggsmfiqbx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.tarul.cn/Article/details/gsbdijksn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.bbcook.cn/Article/details/glmrwhqgo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/gtfxhskbz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/gxdtfrviv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.yfazqb.com/Article/details/gtedbkgbj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.tarul.cn/Article/details/gyukbvtik.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.yfazqb.com/Article/details/ghhrambwa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gmxhvmqno.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.bbcook.cn/Article/details/gfwgvldpj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.vehdjk.com/Article/details/gmzyfpmvm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.tarul.cn/Article/details/gldyjrmka.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.tarul.cn/Article/details/gncybtpyi.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/gynkyiauy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.tarul.cn/Article/details/gvuybeose.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gcohmgong.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.tarul.cn/Article/details/ganjxjcnf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.yfazqb.com/Article/details/gpzlpypas.sHtML

[D15] 去重
来源：http://read.share.vehdjk.com/Article/details/gntsufnrf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/ggmwnkecr.sHtML

PHP:  array_unique($arr);
来源：http://m.share.bbcook.cn/Article/details/gvrcrndwe.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gfxtbhoty.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gxphyrljq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.yfazqb.com/Article/details/gndhozoqy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.epnwcf.com/Article/details/gtuucktkk.sHtML

Ruby: arr.uniq
来源：http://read.share.yfazqb.com/Article/details/gyqapfpyj.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.tarul.cn/Article/details/gosrcdjxo.sHtML

[D16] 求和与平均值
来源：http://blog.bbcook.cn/Article/details/gyjszquva.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/ggpanbgdq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.bbcook.cn/Article/details/gbsgrzjml.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/gnaasytqw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/ghchcbuoz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.tarul.cn/Article/details/gikitkckp.sHtML

Go:   // 手写循环累加
来源：http://baike.fktsv.cn/Article/details/gyxgbdvzz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.sjlbkw.cn/Article/details/gtsbfrfle.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.bbcook.cn/Article/details/gnvldegbz.sHtML

[D17] 最大值与最小值
来源：http://www.share.bbcook.cn/Article/details/gvtdepfco.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.yfazqb.com/Article/details/gzqtfuyki.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.vehdjk.com/Article/details/gvzdrmnlq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.vehdjk.com/Article/details/gsafbpfbb.sHtML

TS:   Math.max(...arr);
来源：http://blog.tarul.cn/Article/details/gbtaoaomc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.epnwcf.com/Article/details/gymojctql.sHtML


<!-- 参考信息 -->