代发 wailian999

[B13] 判断是否为数字
来源：http://www.m.share.epnwcf.com/Article/details/gzwtunrbi.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.tarul.cn/Article/details/gmzzblrzg.sHtML

PHP:  is_numeric($x)
来源：http://blog.bbcook.cn/Article/details/gpqwbalbd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/ghbkggcjh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gwnpvwmxl.sHtML

Java: x instanceof Number
来源：http://baike.vehdjk.com/Article/details/gvazmfkkp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.sjlbkw.cn/Article/details/gaylhblzf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fktsv.cn/Article/details/gitcolcni.sHtML

C#:   x is int or double or decimal
来源：http://baike.yfazqb.com/Article/details/gpottyfuy.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fktsv.cn/Article/details/gsmvjbwgb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.bbcook.cn/Article/details/gqbstgidt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.sjlbkw.cn/Article/details/gaqvimhoa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.tarul.cn/Article/details/gazsbpvnh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gzunzvbik.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.bbcook.cn/Article/details/girbobslm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fktsv.cn/Article/details/gttvrvtds.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gaxluhgfj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gicijksmz.sHtML

[B15] 布尔运算与取反
来源：http://blog.sjlbkw.cn/Article/details/gtsurjqtt.sHtML

Py:   a and b or not c
来源：http://wap.bbcook.cn/Article/details/gddpzaarn.sHtML

PHP:  $a && $b || !$c
来源：http://3g.bbcook.cn/Article/details/gethwzrny.sHtML

JS:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gnoyzjwcj.sHtML

TS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gdgfnpyjr.sHtML

Java: a && b || !c
来源：http://blog.epnwcf.com/Article/details/gpdefaxlq.sHtML

Go:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/glmwszoxz.sHtML

Ruby: a && b || !c
来源：http://3g.yfazqb.com/Article/details/gvsnnskck.sHtML

C#:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gihyjghly.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.sjlbkw.cn/Article/details/gjaeotjbj.sHtML

Py:   if not data: return
来源：http://3g.tarul.cn/Article/details/gzwyuzjhh.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.tarul.cn/Article/details/gpyztsjml.sHtML

JS:   if (!data) return;
来源：http://mobile.vehdjk.com/Article/details/gligrsfhx.sHtML

TS:   if (!data) return;
来源：http://mobile.yfazqb.com/Article/details/gciqiqrku.sHtML

Java: if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/glpfkqbau.sHtML

Go:   if data == nil { return }
来源：http://m.share.bbcook.cn/Article/details/gtjobxgkp.sHtML

Ruby: return if data.nil?
来源：http://wap.tarul.cn/Article/details/gvxxuvsec.sHtML

C#:   if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/ggmbjzvxe.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gzxvedyyv.sHtML

C. 函数与作用域
来源：http://baike.fktsv.cn/Article/details/ghlzdjhnr.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/glafwirdm.sHtML

[C01] 定义函数
来源：http://read.share.yfazqb.com/Article/details/gxyffeykr.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/gzexbuobk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gpucpehqh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gfguenott.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gktawopnd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gqbpseylg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.bbcook.cn/Article/details/gvqzaggii.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.bbcook.cn/Article/details/gdjqojijf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/ggbalftnd.sHtML

[C02] 默认参数
来源：http://m.share.fktsv.cn/Article/details/gazxgiopw.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.epnwcf.com/Article/details/gcablbdxk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.vehdjk.com/Article/details/geypyzpiq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.vehdjk.com/Article/details/gwruscwbt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/glirmtnwl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fktsv.cn/Article/details/gwoeryfbn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.vehdjk.com/Article/details/gxagdowcf.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.tarul.cn/Article/details/gthdiwsnh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fktsv.cn/Article/details/gbmmzdlsx.sHtML

[C03] 可变参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpljoxal.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.tarul.cn/Article/details/gvfssxybn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.sjlbkw.cn/Article/details/gaulwaauk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/geryfetib.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.vehdjk.com/Article/details/girpwnxbq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.sjlbkw.cn/Article/details/gajdtwjpy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.vehdjk.com/Article/details/gdssywahw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fktsv.cn/Article/details/gbfrzjjoy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fktsv.cn/Article/details/gellpdoam.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fktsv.cn/Article/details/gyeioatrl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.epnwcf.com/Article/details/gqevxmpcj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gabjwlhvj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/gwuyasahi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.epnwcf.com/Article/details/gihudqxdo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.epnwcf.com/Article/details/gkfcbthut.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.yfazqb.com/Article/details/gozbezrfn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gifiucgmq.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gwwldkwxr.sHtML

[C05] 返回多个值
来源：http://3g.tarul.cn/Article/details/gyhwprpsw.sHtML

Py:   return a, b
来源：http://baike.sjlbkw.cn/Article/details/gdqqtxsfz.sHtML

PHP:  return [$a, $b];
来源：http://3g.yfazqb.com/Article/details/gfqnxccxw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gtolbbsxx.sHtML

TS:   return { a, b };
来源：http://wap.fktsv.cn/Article/details/ghvgquyyw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.epnwcf.com/Article/details/gvidcxhgo.sHtML

Go:   return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gvdwcusrj.sHtML

Ruby: return a, b
来源：http://m.share.bbcook.cn/Article/details/gmyjbsdey.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.bbcook.cn/Article/details/gqxnipbqp.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.bbcook.cn/Article/details/gwdhuflyr.sHtML

Py:   square = lambda x: x * x
来源：http://baike.yfazqb.com/Article/details/gegbsyjqg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.vehdjk.com/Article/details/ggpghzjhc.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gpsaebcjs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.vehdjk.com/Article/details/galkdodgk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gbemcddtv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.vehdjk.com/Article/details/gkzkycufj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.vehdjk.com/Article/details/gwhktbsvp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/gwwguctps.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.bbcook.cn/Article/details/girvcihpt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fktsv.cn/Article/details/gvgpjlzti.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fktsv.cn/Article/details/gvlnclqmh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.yfazqb.com/Article/details/gbymxthqb.sHtML

TS:   arr.map(String)
来源：http://www.share.vehdjk.com/Article/details/grrearxbs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.epnwcf.com/Article/details/gtddbmahq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.vehdjk.com/Article/details/gwdujvavh.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.epnwcf.com/Article/details/gvukifsev.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.yfazqb.com/Article/details/ghzkdvwdg.sHtML

[C08] 闭包
来源：http://wap.bbcook.cn/Article/details/gagbacfko.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.sjlbkw.cn/Article/details/gyxzncekp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.vehdjk.com/Article/details/gutedtcta.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gsiiursgk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gamvfpkqm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/gcuxejaqw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.bbcook.cn/Article/details/gkwuwtysb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.bbcook.cn/Article/details/gtztyjtzo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gfronotbg.sHtML

[C09] 递归
来源：http://www.blog.yfazqb.com/Article/details/gquhysxri.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.epnwcf.com/Article/details/gcbwrtyvn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.epnwcf.com/Article/details/gkvrmtwrp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.bbcook.cn/Article/details/gquzyqmfs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.epnwcf.com/Article/details/gqionywwn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/gdjrhsxxe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.vehdjk.com/Article/details/gkksyjzwm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/gtnywkdbw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.vehdjk.com/Article/details/gmcpvrwfz.sHtML

[C10] 变量作用域
来源：http://www.m.share.vehdjk.com/Article/details/gfqaecoyl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fktsv.cn/Article/details/gyywpaljr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fktsv.cn/Article/details/gssroiutm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.vehdjk.com/Article/details/goiaennui.sHtML

TS:   同 JS
来源：http://m.share.bbcook.cn/Article/details/gztpmswpc.sHtML

Java: 方法内为块级作用域
来源：http://wap.bbcook.cn/Article/details/gtteatyxr.sHtML

Go:   花括号块级作用域
来源：http://mobile.fktsv.cn/Article/details/gzfvotjwk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.bbcook.cn/Article/details/ghockfmqk.sHtML

C#:   块级作用域
来源：http://mobile.bbcook.cn/Article/details/gvzdneaqt.sHtML

[C11] 模块导入与导出
来源：http://www.share.sjlbkw.cn/Article/details/gezbbiwws.sHtML

Py:   from module import func
来源：http://m.share.yfazqb.com/Article/details/gfukpjjyt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.epnwcf.com/Article/details/gajsdsjun.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.yfazqb.com/Article/details/gtkviqcym.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.epnwcf.com/Article/details/gfiiscmgf.sHtML

Java: import java.util.List;
来源：http://www.blog.yfazqb.com/Article/details/gdshqbesu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.yfazqb.com/Article/details/gxajxxgpx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.yfazqb.com/Article/details/gfjgtbhzg.sHtML

C#:   using System.Text;
来源：http://baike.sjlbkw.cn/Article/details/gvxocunfv.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.bbcook.cn/Article/details/gpqcexxaf.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fktsv.cn/Article/details/ggegmywss.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.bbcook.cn/Article/details/gmmnlisfo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/goedkozyg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.vehdjk.com/Article/details/gobvrvlss.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.vehdjk.com/Article/details/gcdbuwihz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.vehdjk.com/Article/details/gvpxqyhih.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.sjlbkw.cn/Article/details/gcoxjhvyu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.yfazqb.com/Article/details/gowphjulv.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.yfazqb.com/Article/details/gtqyvegsp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.bbcook.cn/Article/details/gjqetotyj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gbawpdvmo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.sjlbkw.cn/Article/details/gtuqboifm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/ggwoompwv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gosbkbnuy.sHtML

Go:   func add(a, b int) int
来源：http://baike.bbcook.cn/Article/details/ghoklhylv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.bbcook.cn/Article/details/gyfvodocz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.tarul.cn/Article/details/gyawwmzri.sHtML

[C14] 泛型函数
来源：http://wap.bbcook.cn/Article/details/gwufbdceu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.vehdjk.com/Article/details/gfjptuvzf.sHtML

PHP:  // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlpqjtwg.sHtML

JS:   // 无泛型
来源：http://read.share.epnwcf.com/Article/details/gtwltgodp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.tarul.cn/Article/details/gwtwliqnb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.vehdjk.com/Article/details/giwwutisx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.vehdjk.com/Article/details/gewucjwzy.sHtML

Ruby: # 无泛型
来源：http://www.share.vehdjk.com/Article/details/gwzgrtcih.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.sjlbkw.cn/Article/details/gspqhlcea.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.vehdjk.com/Article/details/gztvihseg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.sjlbkw.cn/Article/details/geqgxdlol.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.vehdjk.com/Article/details/gufltvjxu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.yfazqb.com/Article/details/gzrwbzenl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fktsv.cn/Article/details/ghmrkqlmu.sHtML

Java: // 无解构
来源：http://www.blog.fktsv.cn/Article/details/gbtkzynwe.sHtML

Go:   // 无解构
来源：http://www.blog.epnwcf.com/Article/details/gikqkpejq.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fktsv.cn/Article/details/gmswtrofq.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.tarul.cn/Article/details/gxfftswxg.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.vehdjk.com/Article/details/gwzzgojua.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.tarul.cn/Article/details/gkthpnvbb.sHtML

PHP:  // 无重载
来源：http://mobile.fktsv.cn/Article/details/ggbrjoeik.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.yfazqb.com/Article/details/gzqgwutan.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.tarul.cn/Article/details/gtyjtbwzw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fktsv.cn/Article/details/gdxtrxdbx.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fktsv.cn/Article/details/gabczoign.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.epnwcf.com/Article/details/gbiansueo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.epnwcf.com/Article/details/grejjssav.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gaqzxnsfb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fktsv.cn/Article/details/glibkkynp.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/grwuzarur.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.sjlbkw.cn/Article/details/gxxxmzbmv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.yfazqb.com/Article/details/gshpnmpad.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fktsv.cn/Article/details/gzwmfzrok.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.tarul.cn/Article/details/gnlpjqtuf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.sjlbkw.cn/Article/details/gqltuetjd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/gwwkjjiat.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.vehdjk.com/Article/details/gbcflfaai.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.epnwcf.com/Article/details/ghestufst.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.vehdjk.com/Article/details/ghcvbenxs.sHtML

[D02] 追加元素到末尾
来源：http://m.share.vehdjk.com/Article/details/gatrnibgq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fktsv.cn/Article/details/gmzpfeuxt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.yfazqb.com/Article/details/ggjlggubl.sHtML

JS:   arr.push(4);
来源：http://mobile.epnwcf.com/Article/details/goucsidlx.sHtML

TS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/greenmlcj.sHtML

Java: list.add(4);
来源：http://blog.tarul.cn/Article/details/giamidmvf.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.epnwcf.com/Article/details/gytkrwfwi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.sjlbkw.cn/Article/details/gruclutqc.sHtML

C#:   list.Add(4);
来源：http://baike.fktsv.cn/Article/details/gmygdsgpw.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fktsv.cn/Article/details/gtpoympif.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/grclmrycs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.yfazqb.com/Article/details/gugkovtvu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.bbcook.cn/Article/details/gkchzevlb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.yfazqb.com/Article/details/glkadwkej.sHtML

Java: list.add(0, 0);
来源：http://read.share.bbcook.cn/Article/details/gkjowisvx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.yfazqb.com/Article/details/gpcggglaa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.vehdjk.com/Article/details/gqwablwmc.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gwumkmyjq.sHtML

[D04] 删除元素
来源：http://www.m.share.vehdjk.com/Article/details/gplxvtuwv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.vehdjk.com/Article/details/gelwifljt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.bbcook.cn/Article/details/gpduihdmy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fktsv.cn/Article/details/gtheuovvu.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fktsv.cn/Article/details/ghfcbssmi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.yfazqb.com/Article/details/gdsmgdeme.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.epnwcf.com/Article/details/gurxdczcs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.bbcook.cn/Article/details/gkmxtdeuo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.vehdjk.com/Article/details/gpxdndmjb.sHtML

[D05] 访问与修改元素
来源：http://blog.yfazqb.com/Article/details/gtzouwxlu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gielxgqsc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gewtveihz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gkhavkxig.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.tarul.cn/Article/details/gpuzdnmgg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.vehdjk.com/Article/details/ggelnsiwl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gzxqiktth.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/gdhnsjfew.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/gvyqcoavf.sHtML

[D06] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/grlgeeaff.sHtML

Py:   len(arr)
来源：http://3g.bbcook.cn/Article/details/gfwyxnytc.sHtML

PHP:  count($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjeqlaten.sHtML

JS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gkteyauxc.sHtML

TS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/grvnmozsn.sHtML

Java: list.size();
来源：http://www.m.share.tarul.cn/Article/details/ggizehbtt.sHtML

Go:   len(arr)
来源：http://wap.epnwcf.com/Article/details/gmfwiriks.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fktsv.cn/Article/details/glttbsyxu.sHtML

C#:   list.Count;
来源：http://3g.vehdjk.com/Article/details/gzlymweqs.sHtML

[D07] 切片 / 取子数组
来源：http://3g.sjlbkw.cn/Article/details/gknadxljh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.tarul.cn/Article/details/gowdnfjeq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gyeolykzu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gyncthwru.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/ghyykhfiv.sHtML

Java: list.subList(1, 4);
来源：http://3g.fktsv.cn/Article/details/gchmyzwej.sHtML

Go:   arr[1:4]
来源：http://www.blog.yfazqb.com/Article/details/gbrbmkbqb.sHtML

Ruby: arr[1, 3]
来源：http://read.share.bbcook.cn/Article/details/gmzsacblr.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.epnwcf.com/Article/details/gnlumcxxz.sHtML

[D08] 合并两个数组
来源：http://blog.yfazqb.com/Article/details/ghrvejppc.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.tarul.cn/Article/details/gzocyrent.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.bbcook.cn/Article/details/gyfckgnpo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.bbcook.cn/Article/details/gjcdkvdan.sHtML

TS:   [...a, ...b];
来源：http://wap.sjlbkw.cn/Article/details/gqaeeaqjt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.sjlbkw.cn/Article/details/gfyfzfpir.sHtML

Go:   append(a, b...)
来源：http://blog.yfazqb.com/Article/details/guhwkpmst.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.vehdjk.com/Article/details/gcvbhlgzs.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.vehdjk.com/Article/details/gdebdcvtn.sHtML

[D09] 排序（升序）
来源：http://baike.sjlbkw.cn/Article/details/gnlkqhhnf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/giafdhswf.sHtML

PHP:  sort($arr);
来源：http://www.share.epnwcf.com/Article/details/gvyelxsli.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.bbcook.cn/Article/details/gvredchju.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.epnwcf.com/Article/details/gjukguebp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.bbcook.cn/Article/details/gldulpiwh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/giftgkpqb.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/glzpdymbz.sHtML

C#:   list.Sort();
来源：http://www.share.yfazqb.com/Article/details/ghacthurz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.bbcook.cn/Article/details/grlbwnstz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.tarul.cn/Article/details/gqbkeoffw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/gzmkdfxnt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fktsv.cn/Article/details/gzeyyfcak.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/gnuoybfnj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fktsv.cn/Article/details/gwtoqdbgg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjotddpe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.tarul.cn/Article/details/gjoxianjj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fktsv.cn/Article/details/glnpxcenp.sHtML

[D11] 反转数组
来源：http://www.m.share.bbcook.cn/Article/details/gvzxljhbi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fktsv.cn/Article/details/gkjaiwpxc.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gtxkxdjtg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.sjlbkw.cn/Article/details/gjupxcyzv.sHtML

TS:   [...arr].reverse();
来源：http://blog.sjlbkw.cn/Article/details/glfrzvwez.sHtML

Java: Collections.reverse(list);
来源：http://read.share.sjlbkw.cn/Article/details/gwstyjnqz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.epnwcf.com/Article/details/gdwwymcqz.sHtML

Ruby: arr.reverse
来源：http://3g.fktsv.cn/Article/details/gjqtawuns.sHtML

C#:   list.Reverse();
来源：http://3g.epnwcf.com/Article/details/gwuufwnwa.sHtML

[D12] 查找元素下标
来源：http://read.share.sjlbkw.cn/Article/details/gishujeuo.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.bbcook.cn/Article/details/gmutpncyd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.epnwcf.com/Article/details/gxugxcoht.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/guxozrhpp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.bbcook.cn/Article/details/gqqqzgjug.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.tarul.cn/Article/details/gaiyomrzz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.vehdjk.com/Article/details/geogpdcer.sHtML

Ruby: arr.index(x)
来源：http://www.share.fktsv.cn/Article/details/gylnzmizy.sHtML

C#:   list.IndexOf(x);
来源：http://3g.vehdjk.com/Article/details/guojjdoqq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.epnwcf.com/Article/details/gwjgrzsrm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.tarul.cn/Article/details/gabvtmngh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fktsv.cn/Article/details/gvdsxhpul.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.tarul.cn/Article/details/gusmestex.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gkomyfqax.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.tarul.cn/Article/details/gzsbtcfnd.sHtML


<!-- 参考信息 -->