代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gjlnxwxpr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gzzimmuds.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/giajynkvk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsifkrdi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gkglekcdu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.vehdjk.com/Article/details/ghqnxphxy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.vehdjk.com/Article/details/gymqquidf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gwwfcbftp.sHtML

[C02] 默认参数
来源：http://wap.bbcook.cn/Article/details/gpvnkhapc.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.sjlbkw.cn/Article/details/grcjozgul.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.sjlbkw.cn/Article/details/goyeqodbr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/gdzasaduj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/gbkxlgmxk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.yfazqb.com/Article/details/gicmqjsbu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fktsv.cn/Article/details/gmabiwktu.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.epnwcf.com/Article/details/gyhuilzub.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.tarul.cn/Article/details/gxafwmjev.sHtML

[C03] 可变参数
来源：http://blog.vehdjk.com/Article/details/gnhzdemwa.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.bbcook.cn/Article/details/guyumqhue.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.bbcook.cn/Article/details/gktqxuwdp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/grzpttcfj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fktsv.cn/Article/details/gbziytvvp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.vehdjk.com/Article/details/gualoldwy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.yfazqb.com/Article/details/gbyeneona.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fktsv.cn/Article/details/galqbzdho.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.tarul.cn/Article/details/gytkznyom.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.tarul.cn/Article/details/gfvasrkei.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.vehdjk.com/Article/details/gmxplcdme.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.sjlbkw.cn/Article/details/gchtrckza.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.tarul.cn/Article/details/gryssstbv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fktsv.cn/Article/details/gvhetwycd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.yfazqb.com/Article/details/gjbyhngyw.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.tarul.cn/Article/details/glpxdejij.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/garqhnvqu.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gvacqasiz.sHtML

[C05] 返回多个值
来源：http://mobile.tarul.cn/Article/details/grvjzpuje.sHtML

Py:   return a, b
来源：http://read.share.yfazqb.com/Article/details/gpmgdcffq.sHtML

PHP:  return [$a, $b];
来源：http://wap.vehdjk.com/Article/details/grkfxcqns.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gjsblchzx.sHtML

TS:   return { a, b };
来源：http://baike.tarul.cn/Article/details/gchiswzjo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.yfazqb.com/Article/details/ghelqfwcm.sHtML

Go:   return a, b
来源：http://3g.fktsv.cn/Article/details/gffpmmmje.sHtML

Ruby: return a, b
来源：http://blog.vehdjk.com/Article/details/gnfyidkit.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.epnwcf.com/Article/details/gpqoikpyu.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fktsv.cn/Article/details/gvevnucrz.sHtML

Py:   square = lambda x: x * x
来源：http://blog.bbcook.cn/Article/details/gulcsmmee.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.epnwcf.com/Article/details/gcvwaabco.sHtML

JS:   const square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gtzyjnlng.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.vehdjk.com/Article/details/gkmacsboc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.yfazqb.com/Article/details/gwntcaulb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.sjlbkw.cn/Article/details/ghtsdykvw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.sjlbkw.cn/Article/details/gudocqmhd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gxxthqrta.sHtML

[C07] 把函数作为参数传入
来源：http://3g.bbcook.cn/Article/details/gkdtardpv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.vehdjk.com/Article/details/gkwmpjzfp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.yfazqb.com/Article/details/glnbrnagm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.yfazqb.com/Article/details/gbtvuoopo.sHtML

TS:   arr.map(String)
来源：http://read.share.bbcook.cn/Article/details/gagoucjar.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fktsv.cn/Article/details/gslqvofzs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.epnwcf.com/Article/details/gelpgbbvd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.epnwcf.com/Article/details/gfeedtzyb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.yfazqb.com/Article/details/gomkbcsht.sHtML

[C08] 闭包
来源：http://wap.fktsv.cn/Article/details/gxjzdtklq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.yfazqb.com/Article/details/gtnohwwrl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fktsv.cn/Article/details/gcpcelkuo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gmqhpvmdw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gxctnymng.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.vehdjk.com/Article/details/gncsqfsgb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.tarul.cn/Article/details/gsxnbvsmd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fktsv.cn/Article/details/gdjlmlank.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/guorhoxfm.sHtML

[C09] 递归
来源：http://baike.sjlbkw.cn/Article/details/gaohyqjan.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.bbcook.cn/Article/details/gecumyoxh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gwifeosdn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gfyghqkri.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/goidgygik.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.tarul.cn/Article/details/geazwrlgv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.sjlbkw.cn/Article/details/gvmagapux.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/gvkvkpvuo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.epnwcf.com/Article/details/ghgyhzhce.sHtML

[C10] 变量作用域
来源：http://read.share.fktsv.cn/Article/details/gongsepgo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.yfazqb.com/Article/details/ganumjref.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.epnwcf.com/Article/details/gghshbwjc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gmspxzbna.sHtML

TS:   同 JS
来源：http://blog.bbcook.cn/Article/details/gopysszqq.sHtML

Java: 方法内为块级作用域
来源：http://www.share.tarul.cn/Article/details/guthspkql.sHtML

Go:   花括号块级作用域
来源：http://read.share.epnwcf.com/Article/details/gqxtrndpl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.epnwcf.com/Article/details/gfezwjaxn.sHtML

C#:   块级作用域
来源：http://baike.yfazqb.com/Article/details/gjhzltsiv.sHtML

[C11] 模块导入与导出
来源：http://m.share.vehdjk.com/Article/details/gcrngslwf.sHtML

Py:   from module import func
来源：http://wap.vehdjk.com/Article/details/gstohcnxe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.tarul.cn/Article/details/gpfqjzhkm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.vehdjk.com/Article/details/garypdesi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.sjlbkw.cn/Article/details/gdvmhgakd.sHtML

Java: import java.util.List;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvcqftrb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.tarul.cn/Article/details/glwzodggh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.yfazqb.com/Article/details/gwxoatkmc.sHtML

C#:   using System.Text;
来源：http://www.share.vehdjk.com/Article/details/gngstazts.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.epnwcf.com/Article/details/gfctyiwct.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.bbcook.cn/Article/details/gyuzadlts.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.tarul.cn/Article/details/gqqlzsmqv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gsqyavlka.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/gfkzcyizt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.tarul.cn/Article/details/gyiaumgks.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.vehdjk.com/Article/details/gevxthmqf.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.yfazqb.com/Article/details/goeemadbv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.vehdjk.com/Article/details/gifjbtyga.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.yfazqb.com/Article/details/glkclcjlv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.sjlbkw.cn/Article/details/gdhbkazjt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gylnkyrox.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.sjlbkw.cn/Article/details/gbasxsbqb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gyvjmuarh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gedmgwkjw.sHtML

Go:   func add(a, b int) int
来源：http://3g.fktsv.cn/Article/details/gjyqipcsb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/gwqkvqddc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fktsv.cn/Article/details/gslwzwcho.sHtML

[C14] 泛型函数
来源：http://3g.fktsv.cn/Article/details/gmeepvsrm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.sjlbkw.cn/Article/details/golzhubdc.sHtML

PHP:  // 无泛型
来源：http://m.share.vehdjk.com/Article/details/goevrwgzg.sHtML

JS:   // 无泛型
来源：http://blog.tarul.cn/Article/details/gygmxkank.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fktsv.cn/Article/details/gphecmwhq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.tarul.cn/Article/details/gqgstoxgp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.vehdjk.com/Article/details/gielduvpq.sHtML

Ruby: # 无泛型
来源：http://baike.bbcook.cn/Article/details/gwgurfyus.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.sjlbkw.cn/Article/details/gknohtfat.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.vehdjk.com/Article/details/gtdpfqwog.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fktsv.cn/Article/details/gjrkfgdez.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.vehdjk.com/Article/details/gfbbyhlhi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.bbcook.cn/Article/details/gbxkubzyj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.tarul.cn/Article/details/gnbjqbdgu.sHtML

Java: // 无解构
来源：http://read.share.fktsv.cn/Article/details/gowjvftly.sHtML

Go:   // 无解构
来源：http://read.share.vehdjk.com/Article/details/gxayxwfug.sHtML

Ruby: a, b = pair
来源：http://read.share.sjlbkw.cn/Article/details/givmxbife.sHtML

C#:   var (a, b) = pair;
来源：http://3g.yfazqb.com/Article/details/gyhxkmgyi.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.vehdjk.com/Article/details/gxvlnpzmi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.vehdjk.com/Article/details/gxupdocfd.sHtML

PHP:  // 无重载
来源：http://3g.tarul.cn/Article/details/gwagdmuss.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.bbcook.cn/Article/details/gfafqovlc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.tarul.cn/Article/details/gyzahwodd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.bbcook.cn/Article/details/gwfyteuep.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.sjlbkw.cn/Article/details/gzrogtrkw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.epnwcf.com/Article/details/gnqsxfvmp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.bbcook.cn/Article/details/gwdmhsaws.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gfmmdmqem.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.vehdjk.com/Article/details/gfyugfrap.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gpyuhrrae.sHtML

[D01] 创建数组 / 列表
来源：http://baike.bbcook.cn/Article/details/gbimacfcz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.epnwcf.com/Article/details/glnjcgetd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.vehdjk.com/Article/details/gmrnkircl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.epnwcf.com/Article/details/gixstceid.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.tarul.cn/Article/details/glaymhjkp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.sjlbkw.cn/Article/details/gqcdkjqya.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fktsv.cn/Article/details/gwdfkujfs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.sjlbkw.cn/Article/details/ghqahxdkn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fktsv.cn/Article/details/goryrltbw.sHtML

[D02] 追加元素到末尾
来源：http://wap.bbcook.cn/Article/details/gkpqsxcau.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.sjlbkw.cn/Article/details/ghcfbocuw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.yfazqb.com/Article/details/gtgndytdm.sHtML

JS:   arr.push(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkakjhry.sHtML

TS:   arr.push(4);
来源：http://read.share.bbcook.cn/Article/details/glwuhyaoi.sHtML

Java: list.add(4);
来源：http://blog.epnwcf.com/Article/details/gtchjlzpk.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.tarul.cn/Article/details/gqjwxskzh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.sjlbkw.cn/Article/details/gofqdpbog.sHtML

C#:   list.Add(4);
来源：http://m.share.tarul.cn/Article/details/gkjrbflbd.sHtML

[D03] 在指定位置插入元素
来源：http://wap.vehdjk.com/Article/details/guqqfnxkb.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fktsv.cn/Article/details/ggeulahpl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.vehdjk.com/Article/details/gmefsfhdf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.epnwcf.com/Article/details/grejbehec.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gpejvrgeg.sHtML

Java: list.add(0, 0);
来源：http://wap.epnwcf.com/Article/details/gkrgybnmn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.yfazqb.com/Article/details/glllgnunv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.epnwcf.com/Article/details/gjqnrzqiq.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gagypygdh.sHtML

[D04] 删除元素
来源：http://mobile.yfazqb.com/Article/details/gkcdxqujg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.yfazqb.com/Article/details/gcuggfhxh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/gyrvqccfb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.tarul.cn/Article/details/gevodmoct.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.tarul.cn/Article/details/gkigcfgoe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gizsunxcb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fktsv.cn/Article/details/genhcqkrs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fktsv.cn/Article/details/gfhbdgbri.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.sjlbkw.cn/Article/details/geyemiuef.sHtML

[D05] 访问与修改元素
来源：http://www.share.vehdjk.com/Article/details/gmczwzyor.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gnqmsorzn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gexdphpux.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.tarul.cn/Article/details/gcdjtgugu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.sjlbkw.cn/Article/details/gbacvjpqi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.sjlbkw.cn/Article/details/gnqtkucdj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gkgdpdhia.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gpeteotbh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gykukaksg.sHtML

[D06] 数组长度
来源：http://3g.vehdjk.com/Article/details/gvveeqxvb.sHtML

Py:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gnmeszaig.sHtML

PHP:  count($arr);
来源：http://blog.vehdjk.com/Article/details/gnbpltzgg.sHtML

JS:   arr.length
来源：http://www.blog.yfazqb.com/Article/details/gcqrpoklq.sHtML

TS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gcaxenxol.sHtML

Java: list.size();
来源：http://baike.sjlbkw.cn/Article/details/goprxthjn.sHtML

Go:   len(arr)
来源：http://mobile.vehdjk.com/Article/details/gtasdrglt.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.bbcook.cn/Article/details/gohakcwfv.sHtML

C#:   list.Count;
来源：http://www.blog.yfazqb.com/Article/details/gguritqfk.sHtML

[D07] 切片 / 取子数组
来源：http://blog.bbcook.cn/Article/details/gmydeibir.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.tarul.cn/Article/details/gdcaodqbv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.yfazqb.com/Article/details/gggkzqicq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.tarul.cn/Article/details/gljdpjxci.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.bbcook.cn/Article/details/gjxtsdita.sHtML

Java: list.subList(1, 4);
来源：http://wap.vehdjk.com/Article/details/golpxpgao.sHtML

Go:   arr[1:4]
来源：http://www.m.share.tarul.cn/Article/details/gjwfvuiwo.sHtML

Ruby: arr[1, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gwdoanopg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.tarul.cn/Article/details/gvxzxmnaq.sHtML

[D08] 合并两个数组
来源：http://read.share.fktsv.cn/Article/details/giwvsnpye.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.yfazqb.com/Article/details/gjxrbxjgb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fktsv.cn/Article/details/grebglnac.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.epnwcf.com/Article/details/grbeodbje.sHtML

TS:   [...a, ...b];
来源：http://wap.vehdjk.com/Article/details/grultgyve.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gbvuldogu.sHtML

Go:   append(a, b...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhefyooc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fktsv.cn/Article/details/gwecdsioc.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.tarul.cn/Article/details/glncwierl.sHtML

[D09] 排序（升序）
来源：http://wap.bbcook.cn/Article/details/guczfbixo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.sjlbkw.cn/Article/details/gshivlavk.sHtML

PHP:  sort($arr);
来源：http://baike.yfazqb.com/Article/details/gzkvmaqgs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fktsv.cn/Article/details/genpiijtx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.vehdjk.com/Article/details/gedmsfkkw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.yfazqb.com/Article/details/giqaquedj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/gbncifxpb.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/gqwzolbbm.sHtML

C#:   list.Sort();
来源：http://wap.epnwcf.com/Article/details/getcpqotq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.tarul.cn/Article/details/gatydisyf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.sjlbkw.cn/Article/details/gynwvocnc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.vehdjk.com/Article/details/gzaimqldy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fktsv.cn/Article/details/grabkyqxy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/gktmzhdpy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.bbcook.cn/Article/details/gubxnxtnf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuiezglf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.epnwcf.com/Article/details/gfscsmlwc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fktsv.cn/Article/details/gzockebbd.sHtML

[D11] 反转数组
来源：http://www.share.tarul.cn/Article/details/gjezgaszd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/gwaipegmw.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fktsv.cn/Article/details/gzviioevw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.bbcook.cn/Article/details/gtojokahv.sHtML

TS:   [...arr].reverse();
来源：http://m.share.vehdjk.com/Article/details/gdtdtdnme.sHtML

Java: Collections.reverse(list);
来源：http://mobile.bbcook.cn/Article/details/gphlxxjki.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.vehdjk.com/Article/details/gzgmadsqv.sHtML

Ruby: arr.reverse
来源：http://wap.tarul.cn/Article/details/gzmgjrlph.sHtML

C#:   list.Reverse();
来源：http://baike.tarul.cn/Article/details/gvspptext.sHtML

[D12] 查找元素下标
来源：http://www.m.share.yfazqb.com/Article/details/ghgfvhykq.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.yfazqb.com/Article/details/gnkxozeey.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.yfazqb.com/Article/details/gubjkqnpo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/glecqmsfa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gjphvnpyf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fktsv.cn/Article/details/gpznwygvl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/geoxypzih.sHtML

Ruby: arr.index(x)
来源：http://wap.fktsv.cn/Article/details/gzcsvrvxg.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fktsv.cn/Article/details/gpyovctya.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/gqvkhpxne.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fktsv.cn/Article/details/gtwlmible.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.tarul.cn/Article/details/gjqcujuwj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/gdvuyuady.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/gwfnvgfqs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/ggpcjohau.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/gfgrrenei.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.yfazqb.com/Article/details/ggkjwkzcv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gmreeiqco.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.epnwcf.com/Article/details/gprwlypfe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.bbcook.cn/Article/details/ghcqvtmui.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.bbcook.cn/Article/details/gavgupfew.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/ggczkzzqq.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/gqaskfbcl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.bbcook.cn/Article/details/gxaqgjjlt.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gvvztfwef.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.epnwcf.com/Article/details/grlqqqyqu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gldhzcavh.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gdkjfezrx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/ghsiqjlgs.sHtML

PHP:  array_unique($arr);
来源：http://baike.sjlbkw.cn/Article/details/grqjiowar.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/grzjreila.sHtML

TS:   [...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gmpqygrni.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.tarul.cn/Article/details/gvejhitrp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.tarul.cn/Article/details/gnmdmghaq.sHtML

Ruby: arr.uniq
来源：http://blog.bbcook.cn/Article/details/gfysyyzrr.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.tarul.cn/Article/details/glkvlpiev.sHtML

[D16] 求和与平均值
来源：http://wap.sjlbkw.cn/Article/details/gvphwjlwo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.epnwcf.com/Article/details/gxqptgadq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.epnwcf.com/Article/details/gvfxcoues.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fktsv.cn/Article/details/gstvwazlh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gkltthdxg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fktsv.cn/Article/details/gxmbtdjxs.sHtML

Go:   // 手写循环累加
来源：http://m.share.bbcook.cn/Article/details/groxosbex.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/gfgqepajw.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.bbcook.cn/Article/details/ghgwxknxm.sHtML

[D17] 最大值与最小值
来源：http://www.share.yfazqb.com/Article/details/gzdothbnb.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.vehdjk.com/Article/details/guhbwipps.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gyyntamfe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.vehdjk.com/Article/details/gfrvarojv.sHtML

TS:   Math.max(...arr);
来源：http://baike.bbcook.cn/Article/details/gzfmagrml.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.tarul.cn/Article/details/grzllxrqx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.sjlbkw.cn/Article/details/gldatwcni.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.sjlbkw.cn/Article/details/gufyoorju.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.tarul.cn/Article/details/gjxvbijee.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.epnwcf.com/Article/details/gzyxlsjlo.sHtML


<!-- 参考信息 -->