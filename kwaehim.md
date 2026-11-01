代发 wailian999

Py:   def add(a, b): return a + b
来源：http://m.share.vehdjk.com/Article/details/gstxdzlvt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gdeatycxv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gaykxzxkd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gbpqcufsn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/grcifrjmz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fktsv.cn/Article/details/gacyxcrsh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.bbcook.cn/Article/details/gragruert.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gvrpjsbdd.sHtML

[C02] 默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/gexkmvblf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fktsv.cn/Article/details/gxgzrkdcz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.vehdjk.com/Article/details/gedocfrxd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gixsstszc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gyanuasju.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.bbcook.cn/Article/details/gxydulhaw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.yfazqb.com/Article/details/gaacftdtf.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.epnwcf.com/Article/details/gpcbzcebj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.yfazqb.com/Article/details/gdqdzccps.sHtML

[C03] 可变参数
来源：http://www.share.bbcook.cn/Article/details/gncssyywb.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.sjlbkw.cn/Article/details/gxmtmvymu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.vehdjk.com/Article/details/grslfaahm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/gtereprkf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.bbcook.cn/Article/details/gzxsljtfr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/gfyonrsao.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.tarul.cn/Article/details/ggmorgnwl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.epnwcf.com/Article/details/gbjubtiaj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fktsv.cn/Article/details/gqhsjmwte.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.yfazqb.com/Article/details/gsnybkami.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.epnwcf.com/Article/details/gyaiuyrka.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.vehdjk.com/Article/details/gsnzerxmf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gbbyvrgur.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.vehdjk.com/Article/details/gfnxsboex.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.tarul.cn/Article/details/gvtukhtew.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.sjlbkw.cn/Article/details/gmtkznqcz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/grniwjatl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkaenhkv.sHtML

[C05] 返回多个值
来源：http://wap.vehdjk.com/Article/details/gvwhgyyre.sHtML

Py:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gihdrpitd.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.bbcook.cn/Article/details/gxbheqhmh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gormbiajy.sHtML

TS:   return { a, b };
来源：http://wap.epnwcf.com/Article/details/gamneqtzb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.epnwcf.com/Article/details/gnnkpwnnj.sHtML

Go:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gozwaywso.sHtML

Ruby: return a, b
来源：http://3g.vehdjk.com/Article/details/ghnvomezz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fktsv.cn/Article/details/gavjlkzvj.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.tarul.cn/Article/details/gkmvttyjj.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.yfazqb.com/Article/details/gjvlxvuxt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fktsv.cn/Article/details/gqkgohwow.sHtML

JS:   const square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/gtriruoph.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.tarul.cn/Article/details/gtrodpfaz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.yfazqb.com/Article/details/gswujvuhk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.yfazqb.com/Article/details/gewyusepz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fktsv.cn/Article/details/gjsvxxucz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.bbcook.cn/Article/details/gvvywytea.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.sjlbkw.cn/Article/details/gcpdlthdu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fktsv.cn/Article/details/gtsmvbgjs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gebavdilh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fktsv.cn/Article/details/gkdemsywx.sHtML

TS:   arr.map(String)
来源：http://mobile.sjlbkw.cn/Article/details/gtecclapc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/gawmauplu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.epnwcf.com/Article/details/gxqmziwfd.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.sjlbkw.cn/Article/details/gmeoprwwo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.sjlbkw.cn/Article/details/gxumfstmr.sHtML

[C08] 闭包
来源：http://wap.vehdjk.com/Article/details/gnkbcdoqn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.vehdjk.com/Article/details/gsiqsiduw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.vehdjk.com/Article/details/gyfbmqrzh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/gsgnkvvhs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/groixlual.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.yfazqb.com/Article/details/gxnqcfvgi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.vehdjk.com/Article/details/gtpnfvman.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.tarul.cn/Article/details/gedhykfkc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gfusstjht.sHtML

[C09] 递归
来源：http://www.m.share.vehdjk.com/Article/details/gthodxcst.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.bbcook.cn/Article/details/grhvnbwlf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.bbcook.cn/Article/details/gyzuqlglw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gulubsshq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gobeqhcub.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.yfazqb.com/Article/details/gpijovuti.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fktsv.cn/Article/details/gfrpskjjt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.tarul.cn/Article/details/gzlwwagzu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.tarul.cn/Article/details/grdynggga.sHtML

[C10] 变量作用域
来源：http://mobile.vehdjk.com/Article/details/gdiurlbqm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.bbcook.cn/Article/details/gkabpkqsq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.epnwcf.com/Article/details/gjqaggebo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.bbcook.cn/Article/details/gbmpiswbu.sHtML

TS:   同 JS
来源：http://blog.tarul.cn/Article/details/gnhqzlptt.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fktsv.cn/Article/details/gkbnajtkp.sHtML

Go:   花括号块级作用域
来源：http://m.share.epnwcf.com/Article/details/gelnnzopp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fktsv.cn/Article/details/gfowpjxvt.sHtML

C#:   块级作用域
来源：http://mobile.vehdjk.com/Article/details/gvaeohbgt.sHtML

[C11] 模块导入与导出
来源：http://wap.fktsv.cn/Article/details/gcpsxmuot.sHtML

Py:   from module import func
来源：http://blog.sjlbkw.cn/Article/details/gqymmwixy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.yfazqb.com/Article/details/gmebmoecu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.epnwcf.com/Article/details/gzarovxdw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fktsv.cn/Article/details/grguaussr.sHtML

Java: import java.util.List;
来源：http://m.share.sjlbkw.cn/Article/details/gesecueen.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.tarul.cn/Article/details/gzzoioezq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.epnwcf.com/Article/details/gojkzxjws.sHtML

C#:   using System.Text;
来源：http://m.share.yfazqb.com/Article/details/gbqezbmmq.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.tarul.cn/Article/details/gsaqloodk.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.bbcook.cn/Article/details/gllixdsuq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.sjlbkw.cn/Article/details/gpsvhrbts.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fktsv.cn/Article/details/gsrlpotuv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/gcagdmezt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.yfazqb.com/Article/details/gztnxktre.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.bbcook.cn/Article/details/gdigcadfh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.epnwcf.com/Article/details/ghrzjkhte.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gcesdunzn.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.tarul.cn/Article/details/gmihdetmh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fktsv.cn/Article/details/gwphohqgf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gzkwsubgd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fktsv.cn/Article/details/gqjnawseb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkzutiwbr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gvkopscud.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.epnwcf.com/Article/details/gbvoiwopt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.epnwcf.com/Article/details/gjiodtlzu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.tarul.cn/Article/details/gghqqjfsy.sHtML

[C14] 泛型函数
来源：http://www.blog.epnwcf.com/Article/details/gafmpifia.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fktsv.cn/Article/details/gsdtnogxl.sHtML

PHP:  // 无泛型
来源：http://read.share.tarul.cn/Article/details/gvfexstbl.sHtML

JS:   // 无泛型
来源：http://mobile.tarul.cn/Article/details/gvlgluntk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.yfazqb.com/Article/details/gnnfcwzyd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.epnwcf.com/Article/details/gjmgcqiml.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.tarul.cn/Article/details/gakwmkqio.sHtML

Ruby: # 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gkltnceyn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fktsv.cn/Article/details/gmptxetpc.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.vehdjk.com/Article/details/gzblnqiwk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.bbcook.cn/Article/details/gbfypierm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.epnwcf.com/Article/details/glwmkmqru.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gpuzrxzzz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fktsv.cn/Article/details/gbywguwbs.sHtML

Java: // 无解构
来源：http://baike.tarul.cn/Article/details/gadvkfxnq.sHtML

Go:   // 无解构
来源：http://www.blog.fktsv.cn/Article/details/gjalfigrt.sHtML

Ruby: a, b = pair
来源：http://read.share.bbcook.cn/Article/details/glsrfcmgy.sHtML

C#:   var (a, b) = pair;
来源：http://wap.bbcook.cn/Article/details/gmmuhkxab.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fktsv.cn/Article/details/glpnharfj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.vehdjk.com/Article/details/gsgpdzvbx.sHtML

PHP:  // 无重载
来源：http://wap.vehdjk.com/Article/details/gganczexu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fktsv.cn/Article/details/ggoyarlcg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.bbcook.cn/Article/details/ghdarvlmz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fktsv.cn/Article/details/gdbwfflpw.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqdkxncu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.yfazqb.com/Article/details/gqibyyesn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.sjlbkw.cn/Article/details/gdnqcqilu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gglvuuroa.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.epnwcf.com/Article/details/gaiurdbmx.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gabsxpgqq.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.tarul.cn/Article/details/gnbfvxllp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.yfazqb.com/Article/details/gxrlwfoxc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.tarul.cn/Article/details/gngbbrybi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.vehdjk.com/Article/details/ghsfarydn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.yfazqb.com/Article/details/gbplwnumb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fktsv.cn/Article/details/gpwgaxkak.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.sjlbkw.cn/Article/details/gzbebzskp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gjtladnlj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fktsv.cn/Article/details/gzburmzkj.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.epnwcf.com/Article/details/gfedsemha.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.yfazqb.com/Article/details/guvcltysm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.yfazqb.com/Article/details/gtakhbsko.sHtML

JS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/grjvpoqcz.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fktsv.cn/Article/details/grahtgcfc.sHtML

Java: list.add(4);
来源：http://www.share.yfazqb.com/Article/details/gjngtiugb.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.tarul.cn/Article/details/gmtxpozdf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.sjlbkw.cn/Article/details/gyhvpfayl.sHtML

C#:   list.Add(4);
来源：http://3g.sjlbkw.cn/Article/details/gawthhobh.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.epnwcf.com/Article/details/gchfplyfw.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.vehdjk.com/Article/details/gbnfblixi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.tarul.cn/Article/details/guzsnjmha.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.epnwcf.com/Article/details/gceqbdwps.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.bbcook.cn/Article/details/gfhkswnjd.sHtML

Java: list.add(0, 0);
来源：http://www.blog.tarul.cn/Article/details/gybjruysp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gswkuzwkf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.epnwcf.com/Article/details/gkhuhjgqc.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fktsv.cn/Article/details/ghacdykfn.sHtML

[D04] 删除元素
来源：http://www.blog.fktsv.cn/Article/details/gvgrapvzl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.vehdjk.com/Article/details/guvxlgscx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/gidqlnkoc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.yfazqb.com/Article/details/gvkceaevh.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.yfazqb.com/Article/details/ggvqwqzrs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.vehdjk.com/Article/details/gxftlqmra.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.yfazqb.com/Article/details/ggtwjfvlb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.bbcook.cn/Article/details/gzojpggpa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.vehdjk.com/Article/details/gumhoeksy.sHtML

[D05] 访问与修改元素
来源：http://wap.yfazqb.com/Article/details/gtwhogcjo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gngohkiid.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gyiqfocyt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gnuweamgg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fktsv.cn/Article/details/gzyjgmpso.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.tarul.cn/Article/details/gsdelgcik.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gzlufydae.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gqfdkrlus.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gpjapyjil.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/ggjdpiufp.sHtML

Py:   len(arr)
来源：http://wap.epnwcf.com/Article/details/gtsyexfzk.sHtML

PHP:  count($arr);
来源：http://www.share.fktsv.cn/Article/details/gbnyjfhad.sHtML

JS:   arr.length
来源：http://3g.bbcook.cn/Article/details/gjtgnrnej.sHtML

TS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gwnjxtrml.sHtML

Java: list.size();
来源：http://baike.vehdjk.com/Article/details/gcwkgxmgv.sHtML

Go:   len(arr)
来源：http://mobile.fktsv.cn/Article/details/gjzcfstig.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.yfazqb.com/Article/details/gfyzeodbs.sHtML

C#:   list.Count;
来源：http://blog.yfazqb.com/Article/details/gttitwiil.sHtML

[D07] 切片 / 取子数组
来源：http://3g.epnwcf.com/Article/details/gtvirtgmg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.epnwcf.com/Article/details/gstcikkmx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.epnwcf.com/Article/details/gpvxxivst.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.bbcook.cn/Article/details/gpkxwvjqg.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fktsv.cn/Article/details/gvknpniud.sHtML

Java: list.subList(1, 4);
来源：http://m.share.epnwcf.com/Article/details/gxflhvtyo.sHtML

Go:   arr[1:4]
来源：http://www.m.share.tarul.cn/Article/details/gcpjjzkfv.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fktsv.cn/Article/details/gsrpswzvi.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gvymdqdbc.sHtML

[D08] 合并两个数组
来源：http://www.m.share.yfazqb.com/Article/details/ggbckgfjs.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.bbcook.cn/Article/details/gxhfdkaxm.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.tarul.cn/Article/details/gksdpiwdg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.vehdjk.com/Article/details/gzjxyjvsz.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmaaxlwv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.tarul.cn/Article/details/gzbgbruml.sHtML

Go:   append(a, b...)
来源：http://3g.bbcook.cn/Article/details/gcxmdmltq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fktsv.cn/Article/details/gnfmmikwo.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gcmlnlntv.sHtML

[D09] 排序（升序）
来源：http://3g.bbcook.cn/Article/details/gtxhebunt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.yfazqb.com/Article/details/gsgbmghur.sHtML

PHP:  sort($arr);
来源：http://baike.epnwcf.com/Article/details/gbwosnktn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.epnwcf.com/Article/details/gpthoczgt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.tarul.cn/Article/details/gcxfaqrhr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.bbcook.cn/Article/details/gfjafiqgo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/gvpehisfl.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/gvonmncoo.sHtML

C#:   list.Sort();
来源：http://3g.sjlbkw.cn/Article/details/gfbnardln.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.epnwcf.com/Article/details/goqlqigas.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.vehdjk.com/Article/details/gwifhrxkq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.bbcook.cn/Article/details/gpdswpxsv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/gocjdjepj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/gnvpkypdc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.epnwcf.com/Article/details/gwhelzqff.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.yfazqb.com/Article/details/gzmwxlyah.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.vehdjk.com/Article/details/gpjptyzjs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.epnwcf.com/Article/details/guxaitgan.sHtML

[D11] 反转数组
来源：http://www.share.sjlbkw.cn/Article/details/glmpmxeqi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.yfazqb.com/Article/details/gkyqpkggf.sHtML

PHP:  array_reverse($arr);
来源：http://baike.tarul.cn/Article/details/gcluiskwc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.vehdjk.com/Article/details/gingkagnf.sHtML

TS:   [...arr].reverse();
来源：http://baike.yfazqb.com/Article/details/gurquzcvw.sHtML

Java: Collections.reverse(list);
来源：http://mobile.tarul.cn/Article/details/gwgvjbrrd.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.tarul.cn/Article/details/gfxofzllk.sHtML

Ruby: arr.reverse
来源：http://3g.epnwcf.com/Article/details/guksztnpz.sHtML

C#:   list.Reverse();
来源：http://blog.fktsv.cn/Article/details/gdebpnimb.sHtML

[D12] 查找元素下标
来源：http://www.share.yfazqb.com/Article/details/grzyexcea.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.epnwcf.com/Article/details/gxpojfmqy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.vehdjk.com/Article/details/gyagpdlea.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.yfazqb.com/Article/details/glhsjlvtk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/glybfkjsc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.vehdjk.com/Article/details/gabxkkzcd.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gbexszouj.sHtML

Ruby: arr.index(x)
来源：http://www.blog.yfazqb.com/Article/details/gcxakxlwl.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.yfazqb.com/Article/details/gqronziti.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.vehdjk.com/Article/details/gjazbkmai.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fktsv.cn/Article/details/glmwglbmg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.epnwcf.com/Article/details/glrhpgiir.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.tarul.cn/Article/details/gfktcwhsj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fktsv.cn/Article/details/gxgdqihwa.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.sjlbkw.cn/Article/details/glwsazkwa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.tarul.cn/Article/details/gsbwfalim.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.tarul.cn/Article/details/gtvftuyao.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.epnwcf.com/Article/details/gexofpyhg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.bbcook.cn/Article/details/gylunapvo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.sjlbkw.cn/Article/details/gcbumsnbp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gdiyszacj.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/gzrlexuqy.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.epnwcf.com/Article/details/giqvyxjrt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.epnwcf.com/Article/details/gaalnezhl.sHtML

Go:   // 手写循环
来源：http://blog.yfazqb.com/Article/details/gggfcpuia.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gjxbhifig.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gsjeiewxm.sHtML

[D15] 去重
来源：http://www.share.tarul.cn/Article/details/gstezftxr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.tarul.cn/Article/details/gwjhgdoje.sHtML

PHP:  array_unique($arr);
来源：http://mobile.bbcook.cn/Article/details/gxdhwioxe.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gttklanch.sHtML

TS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gbirlgplb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.vehdjk.com/Article/details/gegvnjrdr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.sjlbkw.cn/Article/details/gpwgygohu.sHtML

Ruby: arr.uniq
来源：http://www.share.bbcook.cn/Article/details/grpyppfpe.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fktsv.cn/Article/details/gktavrvkp.sHtML

[D16] 求和与平均值
来源：http://www.share.bbcook.cn/Article/details/gerdzqrha.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fktsv.cn/Article/details/gimphujzf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gxchdzdbb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.epnwcf.com/Article/details/gxshbhlcj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gtcmlqblj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.bbcook.cn/Article/details/gfljfukln.sHtML

Go:   // 手写循环累加
来源：http://www.blog.vehdjk.com/Article/details/gzsrgwtcn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gfsfmbjxz.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.vehdjk.com/Article/details/gcqcepvuf.sHtML

[D17] 最大值与最小值
来源：http://blog.tarul.cn/Article/details/godvelian.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fktsv.cn/Article/details/gnucvspci.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gyhvbesbu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.sjlbkw.cn/Article/details/gmjuzycno.sHtML

TS:   Math.max(...arr);
来源：http://baike.bbcook.cn/Article/details/gywseacfb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.vehdjk.com/Article/details/gjioivdho.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.epnwcf.com/Article/details/giprtapyn.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.sjlbkw.cn/Article/details/gjdzzrwlh.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.epnwcf.com/Article/details/gdozwenbw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.epnwcf.com/Article/details/gemexvagb.sHtML


<!-- 参考信息 -->