代发 wailian999

[C02] 默认参数
来源：http://read.share.bbcook.cn/Article/details/gcbquvjxm.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.tarul.cn/Article/details/geansivgc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.bbcook.cn/Article/details/gdyntljtz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.bbcook.cn/Article/details/gnnhvvbbs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/giauslbxe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.tarul.cn/Article/details/gdbentsku.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmucvibw.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.sjlbkw.cn/Article/details/gssbmeyxz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fktsv.cn/Article/details/gthpkwpuw.sHtML

[C03] 可变参数
来源：http://3g.epnwcf.com/Article/details/gonkkymxz.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.epnwcf.com/Article/details/gbefunrky.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.sjlbkw.cn/Article/details/gwfouhitj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/gplaovcij.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fktsv.cn/Article/details/gckzwodcp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fktsv.cn/Article/details/gdpxzndzt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.yfazqb.com/Article/details/gomvidass.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.vehdjk.com/Article/details/gmannrqld.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.epnwcf.com/Article/details/gtdqkroul.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.vehdjk.com/Article/details/gwfdwtoud.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.vehdjk.com/Article/details/grxkojgra.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.bbcook.cn/Article/details/gqybbvajz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gxozjulvj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.bbcook.cn/Article/details/gwsveqiib.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.yfazqb.com/Article/details/gebznmzob.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.epnwcf.com/Article/details/gnkyyxcfx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/gnrxszgtt.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gfngdvbwz.sHtML

[C05] 返回多个值
来源：http://m.share.epnwcf.com/Article/details/gqmievnsg.sHtML

Py:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gydbkteju.sHtML

PHP:  return [$a, $b];
来源：http://wap.vehdjk.com/Article/details/gzkofcibu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.tarul.cn/Article/details/gqgjelxhh.sHtML

TS:   return { a, b };
来源：http://baike.fktsv.cn/Article/details/gvjopmqny.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.bbcook.cn/Article/details/gnvcwxudf.sHtML

Go:   return a, b
来源：http://mobile.yfazqb.com/Article/details/gqorpljkx.sHtML

Ruby: return a, b
来源：http://3g.bbcook.cn/Article/details/gjtmuicpg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.yfazqb.com/Article/details/gomilhoul.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/gnyfkebik.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.epnwcf.com/Article/details/gklohoqqv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.epnwcf.com/Article/details/gdxqgvgny.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fktsv.cn/Article/details/gtvmfkqyi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gycfgkxyd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.vehdjk.com/Article/details/gkycvggyh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.bbcook.cn/Article/details/gwtoglnhj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.tarul.cn/Article/details/geundozlu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gxwiexrou.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.vehdjk.com/Article/details/gfazloodv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.epnwcf.com/Article/details/gorbauelc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.tarul.cn/Article/details/gyyvsfdmr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fktsv.cn/Article/details/gkjhulklt.sHtML

TS:   arr.map(String)
来源：http://baike.vehdjk.com/Article/details/gqhjhvnqd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.epnwcf.com/Article/details/gsphwcheq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.tarul.cn/Article/details/gtnbrdzba.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.yfazqb.com/Article/details/gdddlpsav.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.epnwcf.com/Article/details/gcyublswr.sHtML

[C08] 闭包
来源：http://www.share.tarul.cn/Article/details/gbyrusgtd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.sjlbkw.cn/Article/details/geqvbsztc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.yfazqb.com/Article/details/gzfskidda.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gmcyvvcyv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gmmgglpan.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.sjlbkw.cn/Article/details/gqjgrxcyz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.sjlbkw.cn/Article/details/gkaetxslx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.yfazqb.com/Article/details/gakmacdnx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gujrrwohd.sHtML

[C09] 递归
来源：http://www.blog.vehdjk.com/Article/details/gdwqezmdw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.tarul.cn/Article/details/gdlqzucpx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.epnwcf.com/Article/details/gteroyrqs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/gfsugjxes.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gshdnvtjm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fktsv.cn/Article/details/gbcyqugff.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/gnkfyojpd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/gtpidejhw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.sjlbkw.cn/Article/details/gejwxfcos.sHtML

[C10] 变量作用域
来源：http://mobile.vehdjk.com/Article/details/gucksavjn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.sjlbkw.cn/Article/details/gcdxnkdvb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.epnwcf.com/Article/details/gabeqrlee.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.bbcook.cn/Article/details/gjxkbttbd.sHtML

TS:   同 JS
来源：http://blog.fktsv.cn/Article/details/gtwxfskve.sHtML

Java: 方法内为块级作用域
来源：http://www.share.epnwcf.com/Article/details/gfojcblzo.sHtML

Go:   花括号块级作用域
来源：http://3g.bbcook.cn/Article/details/gfgfdpkpf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.sjlbkw.cn/Article/details/gojrtduvz.sHtML

C#:   块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gshiyiuxw.sHtML

[C11] 模块导入与导出
来源：http://read.share.sjlbkw.cn/Article/details/gznjtfknt.sHtML

Py:   from module import func
来源：http://wap.yfazqb.com/Article/details/gyncwcrha.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.sjlbkw.cn/Article/details/gkjcmarui.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.tarul.cn/Article/details/gikvxowin.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.vehdjk.com/Article/details/gzqmzprca.sHtML

Java: import java.util.List;
来源：http://3g.sjlbkw.cn/Article/details/geemfycro.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.tarul.cn/Article/details/ghoqpfbll.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fktsv.cn/Article/details/ggknlsamx.sHtML

C#:   using System.Text;
来源：http://www.blog.bbcook.cn/Article/details/gwphuepxo.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fktsv.cn/Article/details/ggqzvepus.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.epnwcf.com/Article/details/ghjaszspf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.vehdjk.com/Article/details/gncefldtn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/gsobosfmr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fktsv.cn/Article/details/gvwecjvjr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.sjlbkw.cn/Article/details/grvsdncyb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.bbcook.cn/Article/details/gebkrremu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.bbcook.cn/Article/details/gsdrtcvpl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.bbcook.cn/Article/details/gejeoyjvy.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.bbcook.cn/Article/details/ghfrdhign.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fktsv.cn/Article/details/gwhivyodm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gaglwzwlc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.tarul.cn/Article/details/gdasnfklg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gdyrgrfuy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gsobgqwef.sHtML

Go:   func add(a, b int) int
来源：http://mobile.epnwcf.com/Article/details/giwwlriio.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.epnwcf.com/Article/details/gnqcpfrek.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.vehdjk.com/Article/details/gzoyknisj.sHtML

[C14] 泛型函数
来源：http://wap.sjlbkw.cn/Article/details/gdwojztkx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.vehdjk.com/Article/details/gxtftvmpj.sHtML

PHP:  // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/geedwifxu.sHtML

JS:   // 无泛型
来源：http://wap.tarul.cn/Article/details/gskabhyvz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/gybnhswlj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.yfazqb.com/Article/details/ghrfudmln.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.epnwcf.com/Article/details/gvknimjvs.sHtML

Ruby: # 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gjdecepoq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.bbcook.cn/Article/details/gfznyrawc.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.yfazqb.com/Article/details/glnmzdgms.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.tarul.cn/Article/details/gbodqxqba.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.sjlbkw.cn/Article/details/gklsuukhu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gunzbnkvg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.epnwcf.com/Article/details/gvjfhtvix.sHtML

Java: // 无解构
来源：http://mobile.epnwcf.com/Article/details/gpkxpxoyn.sHtML

Go:   // 无解构
来源：http://www.share.sjlbkw.cn/Article/details/gdlltesim.sHtML

Ruby: a, b = pair
来源：http://baike.sjlbkw.cn/Article/details/gsybbmtpy.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fktsv.cn/Article/details/grqoolytb.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/gllakaqai.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.epnwcf.com/Article/details/grzoteqby.sHtML

PHP:  // 无重载
来源：http://www.share.fktsv.cn/Article/details/gpoyeaysd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.bbcook.cn/Article/details/gfmjtuxny.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fktsv.cn/Article/details/gslppzztb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.yfazqb.com/Article/details/gjvbpzkjs.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.epnwcf.com/Article/details/gymregzrv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.yfazqb.com/Article/details/gktbmhrjd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.bbcook.cn/Article/details/glkvkqscz.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gdpxpawhy.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.vehdjk.com/Article/details/gxrtpptkq.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gntwikfbv.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/ghhsrwoxf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.vehdjk.com/Article/details/gmtywkzkk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.epnwcf.com/Article/details/grmfeyxia.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.epnwcf.com/Article/details/gfcxzyxlb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.vehdjk.com/Article/details/gmmmnxwkt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.yfazqb.com/Article/details/gxzjsjvml.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.tarul.cn/Article/details/gjdtqfoow.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.vehdjk.com/Article/details/gafiaqqlh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.yfazqb.com/Article/details/gtivwetou.sHtML

[D02] 追加元素到末尾
来源：http://3g.vehdjk.com/Article/details/gpqalfaoc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fktsv.cn/Article/details/gfrgtmntq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.tarul.cn/Article/details/gjowbdhxq.sHtML

JS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/ggtrfsjvm.sHtML

TS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gkyirkszk.sHtML

Java: list.add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrvxyhvp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtstseisz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.bbcook.cn/Article/details/gdqvkkoog.sHtML

C#:   list.Add(4);
来源：http://read.share.fktsv.cn/Article/details/gndgwesua.sHtML

[D03] 在指定位置插入元素
来源：http://wap.tarul.cn/Article/details/gezwvkglm.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.epnwcf.com/Article/details/gephhxocd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.bbcook.cn/Article/details/gcpqxhuwu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fktsv.cn/Article/details/goauunxbp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gskptoqlt.sHtML

Java: list.add(0, 0);
来源：http://baike.bbcook.cn/Article/details/goizarbfo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.tarul.cn/Article/details/ghwraberk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fktsv.cn/Article/details/grzddremn.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gnwcxsggg.sHtML

[D04] 删除元素
来源：http://blog.epnwcf.com/Article/details/gauvxztzf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.epnwcf.com/Article/details/gzywmxaec.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.vehdjk.com/Article/details/gcessiagk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.tarul.cn/Article/details/grhoiyucu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fktsv.cn/Article/details/ggqpoknsl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.tarul.cn/Article/details/gjwckxdkh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fktsv.cn/Article/details/gbrewzszx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.tarul.cn/Article/details/gobgvkrgc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.yfazqb.com/Article/details/gcehonbat.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fktsv.cn/Article/details/georytzei.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gblifnnru.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gbrmuhloa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.yfazqb.com/Article/details/grdkfpsta.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.bbcook.cn/Article/details/gabmtzxft.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.yfazqb.com/Article/details/gzbavnhtg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gjrkqjuzf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/grdukevxm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gfazfqxme.sHtML

[D06] 数组长度
来源：http://wap.vehdjk.com/Article/details/guqyibbfx.sHtML

Py:   len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/ghgdxithu.sHtML

PHP:  count($arr);
来源：http://3g.vehdjk.com/Article/details/gearibvxm.sHtML

JS:   arr.length
来源：http://wap.tarul.cn/Article/details/gttovfmbz.sHtML

TS:   arr.length
来源：http://wap.tarul.cn/Article/details/gggtqtqcd.sHtML

Java: list.size();
来源：http://m.share.vehdjk.com/Article/details/gmhjrbkmn.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/gcvoxfgrw.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gcbrmvmfp.sHtML

C#:   list.Count;
来源：http://blog.epnwcf.com/Article/details/gdrnnbmbc.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.tarul.cn/Article/details/gfgjszuzr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.epnwcf.com/Article/details/gxbbeysia.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.bbcook.cn/Article/details/gdxwbfigt.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gsuwdifbz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gkyboijuy.sHtML

Java: list.subList(1, 4);
来源：http://mobile.tarul.cn/Article/details/gplrgzaez.sHtML

Go:   arr[1:4]
来源：http://www.m.share.yfazqb.com/Article/details/gockxgkqn.sHtML

Ruby: arr[1, 3]
来源：http://wap.vehdjk.com/Article/details/gshnkcogi.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.tarul.cn/Article/details/glexvamar.sHtML

[D08] 合并两个数组
来源：http://www.share.bbcook.cn/Article/details/gqxcgzdnp.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.epnwcf.com/Article/details/gbgdgkqwn.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.vehdjk.com/Article/details/gvyhhxjoy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.epnwcf.com/Article/details/gnffdkdbn.sHtML

TS:   [...a, ...b];
来源：http://wap.fktsv.cn/Article/details/guegcddwr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.vehdjk.com/Article/details/geqejgzod.sHtML

Go:   append(a, b...)
来源：http://www.m.share.bbcook.cn/Article/details/gsvvevjuo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.sjlbkw.cn/Article/details/gfxibrmma.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.vehdjk.com/Article/details/gykxkbobg.sHtML

[D09] 排序（升序）
来源：http://baike.bbcook.cn/Article/details/gbxcdxzcg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gyybirjbz.sHtML

PHP:  sort($arr);
来源：http://mobile.vehdjk.com/Article/details/gngkqujas.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fktsv.cn/Article/details/gkwwdhqia.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.epnwcf.com/Article/details/gwgufwygf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.sjlbkw.cn/Article/details/glzpkihhi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gnajmbovq.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/gkkbufgsf.sHtML

C#:   list.Sort();
来源：http://www.blog.fktsv.cn/Article/details/ghokbeeap.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.epnwcf.com/Article/details/gfvtxufsp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.tarul.cn/Article/details/gntlfprnk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.bbcook.cn/Article/details/gwvcjdctz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fktsv.cn/Article/details/gpyvqdanh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrtzlrie.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.yfazqb.com/Article/details/gobkpkxls.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.yfazqb.com/Article/details/gmoitlzyd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.bbcook.cn/Article/details/gvmbimweg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.tarul.cn/Article/details/ggofcgsex.sHtML

[D11] 反转数组
来源：http://blog.epnwcf.com/Article/details/ggdysumcb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.tarul.cn/Article/details/gpciqwswe.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.sjlbkw.cn/Article/details/ggfautzdj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.bbcook.cn/Article/details/giwvxfimq.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.sjlbkw.cn/Article/details/gyymauokd.sHtML

Java: Collections.reverse(list);
来源：http://read.share.bbcook.cn/Article/details/gmfxugfci.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.yfazqb.com/Article/details/gktqyfeds.sHtML

Ruby: arr.reverse
来源：http://wap.epnwcf.com/Article/details/gtnkyyukt.sHtML

C#:   list.Reverse();
来源：http://www.m.share.epnwcf.com/Article/details/gmrkmylnq.sHtML

[D12] 查找元素下标
来源：http://read.share.epnwcf.com/Article/details/gklzxiwtc.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.yfazqb.com/Article/details/grwoirpfb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.bbcook.cn/Article/details/guzhivzrm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.bbcook.cn/Article/details/gpbeghalf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fktsv.cn/Article/details/gkkhmvhzj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.sjlbkw.cn/Article/details/gqilyjasv.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gtxbvvuzm.sHtML

Ruby: arr.index(x)
来源：http://blog.vehdjk.com/Article/details/gglaykbjq.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.sjlbkw.cn/Article/details/gytuzduzb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.vehdjk.com/Article/details/gmfetcssv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.sjlbkw.cn/Article/details/gyfpowevl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.bbcook.cn/Article/details/gidhreizs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gwuwvpbqi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/gwrouegwd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.yfazqb.com/Article/details/goqmnrvkp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.sjlbkw.cn/Article/details/gllosgisb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.tarul.cn/Article/details/gfaexwbxz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gezyueqgl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.tarul.cn/Article/details/gherlxlah.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gdkwmpwpt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.tarul.cn/Article/details/gnsncstxg.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/gpirvwngr.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fktsv.cn/Article/details/gtnzrvlyv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.epnwcf.com/Article/details/gojsmiagx.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gpositnlz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/griucliay.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fktsv.cn/Article/details/gmyraxmrp.sHtML

[D15] 去重
来源：http://www.m.share.tarul.cn/Article/details/gpgluggxh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/gohgvnnym.sHtML

PHP:  array_unique($arr);
来源：http://mobile.bbcook.cn/Article/details/giyrpgxhm.sHtML

JS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/goywwujkl.sHtML

TS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gqlivhmqc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.sjlbkw.cn/Article/details/gtapkxbvk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.vehdjk.com/Article/details/gmidkwwkn.sHtML

Ruby: arr.uniq
来源：http://wap.yfazqb.com/Article/details/gqrjzirmm.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fktsv.cn/Article/details/gizzbvekx.sHtML

[D16] 求和与平均值
来源：http://www.m.share.sjlbkw.cn/Article/details/geqaxsibp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gglmsrqaf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.yfazqb.com/Article/details/gljymitqi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gsnonsdro.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.tarul.cn/Article/details/griqxbisb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fktsv.cn/Article/details/gfhifyrxu.sHtML

Go:   // 手写循环累加
来源：http://www.blog.tarul.cn/Article/details/gmnjzqyig.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.vehdjk.com/Article/details/glhcammzz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fktsv.cn/Article/details/gxtsjaped.sHtML

[D17] 最大值与最小值
来源：http://read.share.bbcook.cn/Article/details/gvyhdgmzm.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.bbcook.cn/Article/details/gmdlsealh.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.epnwcf.com/Article/details/gzhbcwfpn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.yfazqb.com/Article/details/gfwxsodlb.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/gtywzifbj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.tarul.cn/Article/details/gnjlxevyl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fktsv.cn/Article/details/gfqfcerva.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.yfazqb.com/Article/details/gdapriyxd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.tarul.cn/Article/details/gijuykiir.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.vehdjk.com/Article/details/gbefvqaqb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.yfazqb.com/Article/details/gczpsvnxm.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.bbcook.cn/Article/details/glbsyqjce.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.bbcook.cn/Article/details/gthvxksew.sHtML

TS:   nested.flat();
来源：http://blog.sjlbkw.cn/Article/details/gbgulndor.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.vehdjk.com/Article/details/gtzjqdrzs.sHtML

Go:   // 手写双层循环
来源：http://3g.vehdjk.com/Article/details/gavckeybu.sHtML

Ruby: nested.flatten
来源：http://wap.bbcook.cn/Article/details/gapmeiumb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gdeuabopb.sHtML


<!-- 参考信息 -->