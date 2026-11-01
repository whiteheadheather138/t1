代发 wailian999

[C02] 默认参数
来源：http://wap.sjlbkw.cn/Article/details/gisdcmvrb.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.sjlbkw.cn/Article/details/gapfvhzqv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.bbcook.cn/Article/details/gapqvjfmd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/gzqxjfdzz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gylatzarh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.sjlbkw.cn/Article/details/gnjqbjues.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.sjlbkw.cn/Article/details/gfcxvizlj.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.tarul.cn/Article/details/gftokpeac.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/gvppahxcg.sHtML

[C03] 可变参数
来源：http://m.share.epnwcf.com/Article/details/giivooxcc.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.epnwcf.com/Article/details/gnbwcjdtn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.epnwcf.com/Article/details/gksunuzdl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/grparthks.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gysholodb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.bbcook.cn/Article/details/gemmsxuul.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.bbcook.cn/Article/details/gzrixlknc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.vehdjk.com/Article/details/ggbxzimgr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.yfazqb.com/Article/details/gevgjqhpc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.epnwcf.com/Article/details/gutxwwkyd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.yfazqb.com/Article/details/gcxouypio.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.yfazqb.com/Article/details/gasserfxm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gsdmumtyp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.yfazqb.com/Article/details/gopkbsrve.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.vehdjk.com/Article/details/gytqqrbiw.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.sjlbkw.cn/Article/details/gghlteddr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gxztwthfs.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/gcghrpgpv.sHtML

[C05] 返回多个值
来源：http://3g.vehdjk.com/Article/details/gjbloyoot.sHtML

Py:   return a, b
来源：http://blog.yfazqb.com/Article/details/gdjpchcxp.sHtML

PHP:  return [$a, $b];
来源：http://m.share.sjlbkw.cn/Article/details/gvdrvkvlp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.vehdjk.com/Article/details/gxoqnudfv.sHtML

TS:   return { a, b };
来源：http://wap.bbcook.cn/Article/details/gzpddunvg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.bbcook.cn/Article/details/gmrmysufm.sHtML

Go:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gtajqklsy.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gdmewvogq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fktsv.cn/Article/details/ghqedfqnf.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.vehdjk.com/Article/details/gzwzggebq.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.vehdjk.com/Article/details/gyejopvfx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.bbcook.cn/Article/details/gnywpinne.sHtML

JS:   const square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gnjrzzohe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.tarul.cn/Article/details/gqzjddnuo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.bbcook.cn/Article/details/gybjbogul.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.yfazqb.com/Article/details/gyirkipnf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.tarul.cn/Article/details/gvsbeljpn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gcfisczff.sHtML

[C07] 把函数作为参数传入
来源：http://3g.bbcook.cn/Article/details/gaumoxrpu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.bbcook.cn/Article/details/gjkqbjhfb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.yfazqb.com/Article/details/glybzigvb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.vehdjk.com/Article/details/gwvxqefxg.sHtML

TS:   arr.map(String)
来源：http://baike.tarul.cn/Article/details/gaswqjpdn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.tarul.cn/Article/details/gdeeevmaj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.epnwcf.com/Article/details/gejgecpas.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.tarul.cn/Article/details/gsflagtbo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.bbcook.cn/Article/details/giunjkuvq.sHtML

[C08] 闭包
来源：http://www.share.fktsv.cn/Article/details/guiegkfwn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.yfazqb.com/Article/details/gfmxindwp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.bbcook.cn/Article/details/garvkuvfl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/gozywsort.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/ggelcfvwj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.yfazqb.com/Article/details/gfxhuvnwt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fktsv.cn/Article/details/gkuczthyo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.bbcook.cn/Article/details/gpptzoxsn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gaxnyowof.sHtML

[C09] 递归
来源：http://baike.epnwcf.com/Article/details/gpsybcrxe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.bbcook.cn/Article/details/gsfupojfa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzspeuoib.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.yfazqb.com/Article/details/gikaclxsd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gzvpbefgv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.bbcook.cn/Article/details/gttpxplzz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.sjlbkw.cn/Article/details/gzcxayabr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/gtwzuklqd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.yfazqb.com/Article/details/gocogcvdp.sHtML

[C10] 变量作用域
来源：http://www.m.share.fktsv.cn/Article/details/gbavbfgco.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.tarul.cn/Article/details/gemywdkhu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.vehdjk.com/Article/details/gwndhdpmh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.bbcook.cn/Article/details/gurkezlse.sHtML

TS:   同 JS
来源：http://mobile.vehdjk.com/Article/details/ghwqgiorx.sHtML

Java: 方法内为块级作用域
来源：http://blog.epnwcf.com/Article/details/gjxhhgrhb.sHtML

Go:   花括号块级作用域
来源：http://baike.yfazqb.com/Article/details/gdenzynbp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.bbcook.cn/Article/details/gayynuiyv.sHtML

C#:   块级作用域
来源：http://blog.sjlbkw.cn/Article/details/glcltklfz.sHtML

[C11] 模块导入与导出
来源：http://www.share.yfazqb.com/Article/details/gifiaccjq.sHtML

Py:   from module import func
来源：http://read.share.vehdjk.com/Article/details/gktuzorrt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fktsv.cn/Article/details/gnmmwhieh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.vehdjk.com/Article/details/gkyebypmg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fktsv.cn/Article/details/gipiiiune.sHtML

Java: import java.util.List;
来源：http://www.blog.tarul.cn/Article/details/gtzwcwsik.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.vehdjk.com/Article/details/garrrqzrt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.epnwcf.com/Article/details/gkfhfnydd.sHtML

C#:   using System.Text;
来源：http://www.m.share.fktsv.cn/Article/details/gggqfcabs.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.epnwcf.com/Article/details/gazagloph.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.yfazqb.com/Article/details/gdzdpnwfk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.vehdjk.com/Article/details/guklhugqs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/grdvjesrk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gcivrrzvs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fktsv.cn/Article/details/gkdnvmnpj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.sjlbkw.cn/Article/details/gahganfwd.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.yfazqb.com/Article/details/gjsjdjswa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.vehdjk.com/Article/details/gopegdppu.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.bbcook.cn/Article/details/gwejtqtra.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fktsv.cn/Article/details/gghveoonp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gtvstpmnk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.bbcook.cn/Article/details/gybniotnj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gwvpoytxm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gogvxoufg.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fktsv.cn/Article/details/gmueseztw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrcjuzxn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fktsv.cn/Article/details/gowtwfbyf.sHtML

[C14] 泛型函数
来源：http://baike.yfazqb.com/Article/details/geqqlgmjr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.sjlbkw.cn/Article/details/gsykttude.sHtML

PHP:  // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gdxevoyof.sHtML

JS:   // 无泛型
来源：http://wap.fktsv.cn/Article/details/gdxhuixhe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.yfazqb.com/Article/details/gpaodnlid.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fktsv.cn/Article/details/gcggpzttf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.bbcook.cn/Article/details/gjlcejwtk.sHtML

Ruby: # 无泛型
来源：http://wap.vehdjk.com/Article/details/glkblduty.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.bbcook.cn/Article/details/gtgfpkcep.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.yfazqb.com/Article/details/ggbcnniem.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.tarul.cn/Article/details/gnpeilsgf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.vehdjk.com/Article/details/ggdycvktm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/gqvxbxvpn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.epnwcf.com/Article/details/grrehbvnv.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/grhuyvjrp.sHtML

Go:   // 无解构
来源：http://www.m.share.tarul.cn/Article/details/gktzcnolb.sHtML

Ruby: a, b = pair
来源：http://m.share.tarul.cn/Article/details/gozjaqcxe.sHtML

C#:   var (a, b) = pair;
来源：http://blog.epnwcf.com/Article/details/gsjtdvbaj.sHtML

[C16] 函数 / 方法重载
来源：http://3g.bbcook.cn/Article/details/gvwfkzshp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.vehdjk.com/Article/details/grvwggbkj.sHtML

PHP:  // 无重载
来源：http://www.m.share.vehdjk.com/Article/details/gygstiqsr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.vehdjk.com/Article/details/gojeloseu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.yfazqb.com/Article/details/gvxchihlm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.sjlbkw.cn/Article/details/geyygyspr.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.sjlbkw.cn/Article/details/gldwgeoqe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.sjlbkw.cn/Article/details/ggtjiatte.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.epnwcf.com/Article/details/gyisxwsso.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gionajzvg.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.yfazqb.com/Article/details/gkowloggq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gtvprupus.sHtML

[D01] 创建数组 / 列表
来源：http://baike.tarul.cn/Article/details/gljalxtmf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.tarul.cn/Article/details/gmuljmnte.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.yfazqb.com/Article/details/gghrqoteq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.epnwcf.com/Article/details/giefgfsvi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.yfazqb.com/Article/details/gqcfnoixv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fktsv.cn/Article/details/gffwwvzfe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.sjlbkw.cn/Article/details/gghwitjzk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gaykzlved.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.epnwcf.com/Article/details/glihvxwhc.sHtML

[D02] 追加元素到末尾
来源：http://wap.vehdjk.com/Article/details/gipcrpoce.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.bbcook.cn/Article/details/gkyunzamx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.sjlbkw.cn/Article/details/ghwmffhml.sHtML

JS:   arr.push(4);
来源：http://read.share.epnwcf.com/Article/details/gcywjjhoe.sHtML

TS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/ghxhkzkno.sHtML

Java: list.add(4);
来源：http://baike.epnwcf.com/Article/details/gzcuxstvs.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.epnwcf.com/Article/details/gfitqczur.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.bbcook.cn/Article/details/gwssipbgq.sHtML

C#:   list.Add(4);
来源：http://www.share.epnwcf.com/Article/details/gedrrlovt.sHtML

[D03] 在指定位置插入元素
来源：http://baike.yfazqb.com/Article/details/gynttshmy.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.tarul.cn/Article/details/gumxplkuh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.tarul.cn/Article/details/ghhtqzclx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.tarul.cn/Article/details/gncswdxnv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.epnwcf.com/Article/details/gthhbxmoe.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlyphurv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.vehdjk.com/Article/details/gxrcgshua.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.sjlbkw.cn/Article/details/gfufcvejm.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.bbcook.cn/Article/details/gcixetfpx.sHtML

[D04] 删除元素
来源：http://m.share.epnwcf.com/Article/details/gpzpemjot.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.sjlbkw.cn/Article/details/gzkwokxsl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.vehdjk.com/Article/details/gkvtyawar.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.vehdjk.com/Article/details/gggctdzmc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.vehdjk.com/Article/details/gtdbxzcei.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgwadagm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.vehdjk.com/Article/details/gkrjxlndp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.sjlbkw.cn/Article/details/gqvxpoxql.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.tarul.cn/Article/details/gprkgppok.sHtML

[D05] 访问与修改元素
来源：http://baike.yfazqb.com/Article/details/ghfqkwwkq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gkmgphlsk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/goxpalohn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gcnrglbpw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.epnwcf.com/Article/details/gejftrilp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fktsv.cn/Article/details/gopztabot.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/ghzyzvmpv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gxwdwgsna.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbqiakvo.sHtML

[D06] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gyxyqkmrg.sHtML

Py:   len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gnszjeskh.sHtML

PHP:  count($arr);
来源：http://wap.tarul.cn/Article/details/guaudsdua.sHtML

JS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/giruwwicd.sHtML

TS:   arr.length
来源：http://baike.epnwcf.com/Article/details/gyoqkrcmg.sHtML

Java: list.size();
来源：http://blog.vehdjk.com/Article/details/ggqkutngx.sHtML

Go:   len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/glxvwljdu.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.epnwcf.com/Article/details/gieboodtw.sHtML

C#:   list.Count;
来源：http://www.m.share.yfazqb.com/Article/details/galsyhwat.sHtML

[D07] 切片 / 取子数组
来源：http://baike.sjlbkw.cn/Article/details/gqyfbxhan.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.vehdjk.com/Article/details/gkgsiqzwq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.epnwcf.com/Article/details/gocatxtvj.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gzrynxowq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/guxjgogjc.sHtML

Java: list.subList(1, 4);
来源：http://read.share.tarul.cn/Article/details/gavnzollr.sHtML

Go:   arr[1:4]
来源：http://3g.bbcook.cn/Article/details/gitxkerwn.sHtML

Ruby: arr[1, 3]
来源：http://wap.vehdjk.com/Article/details/gbbhngccs.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.yfazqb.com/Article/details/gpkhtixge.sHtML

[D08] 合并两个数组
来源：http://www.blog.bbcook.cn/Article/details/gmivukmxq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.vehdjk.com/Article/details/guifughmt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.sjlbkw.cn/Article/details/gjfmjiqxn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.sjlbkw.cn/Article/details/grubbwwxq.sHtML

TS:   [...a, ...b];
来源：http://mobile.fktsv.cn/Article/details/gvfutdstv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.tarul.cn/Article/details/glpwpyane.sHtML

Go:   append(a, b...)
来源：http://m.share.vehdjk.com/Article/details/gwkzrqotp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.yfazqb.com/Article/details/gakmmczvs.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fktsv.cn/Article/details/gwqigdjgt.sHtML

[D09] 排序（升序）
来源：http://3g.fktsv.cn/Article/details/gtxlhpqhn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/ggkvglllt.sHtML

PHP:  sort($arr);
来源：http://mobile.fktsv.cn/Article/details/ggumadoym.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.sjlbkw.cn/Article/details/gteylikip.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.tarul.cn/Article/details/gaziuixyu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.epnwcf.com/Article/details/gtphvseez.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/gtrbwhrnw.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/gcmkdadws.sHtML

C#:   list.Sort();
来源：http://blog.bbcook.cn/Article/details/genstthyu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.vehdjk.com/Article/details/gqnbhfeyo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.yfazqb.com/Article/details/grabdxdwy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.sjlbkw.cn/Article/details/gpdzisbau.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/gnawienfg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/gjkbdmhyf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.sjlbkw.cn/Article/details/gwmqhjeby.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.yfazqb.com/Article/details/ghqhncdma.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.bbcook.cn/Article/details/grgfcnrmt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.bbcook.cn/Article/details/guuqkdbpc.sHtML

[D11] 反转数组
来源：http://blog.sjlbkw.cn/Article/details/gnzefjumo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.bbcook.cn/Article/details/gcoqvigtr.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.bbcook.cn/Article/details/grqtcnhtx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.tarul.cn/Article/details/gefksmeub.sHtML

TS:   [...arr].reverse();
来源：http://www.share.bbcook.cn/Article/details/gaxpwykyq.sHtML

Java: Collections.reverse(list);
来源：http://mobile.bbcook.cn/Article/details/gjgeodqak.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.tarul.cn/Article/details/glhqlkrwb.sHtML

Ruby: arr.reverse
来源：http://3g.bbcook.cn/Article/details/gtyikpxmc.sHtML

C#:   list.Reverse();
来源：http://www.share.vehdjk.com/Article/details/gqwmkuahq.sHtML

[D12] 查找元素下标
来源：http://m.share.fktsv.cn/Article/details/gwksolrqx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.sjlbkw.cn/Article/details/gvsbwchlo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.bbcook.cn/Article/details/gghlmaxxq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/gxxuomnkp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.epnwcf.com/Article/details/gycjdihde.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.tarul.cn/Article/details/gfndzfmrv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fktsv.cn/Article/details/ggretkbfl.sHtML

Ruby: arr.index(x)
来源：http://m.share.bbcook.cn/Article/details/grdxvdlpx.sHtML

C#:   list.IndexOf(x);
来源：http://wap.sjlbkw.cn/Article/details/gssrkbihr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.vehdjk.com/Article/details/ghlxnxudh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.tarul.cn/Article/details/glfxwboxg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.bbcook.cn/Article/details/gpnwdhbmh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gfdllahsn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.tarul.cn/Article/details/gihdpztxt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.epnwcf.com/Article/details/gcogyenzp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.sjlbkw.cn/Article/details/gwthcmhnc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.vehdjk.com/Article/details/ghxctmwly.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gjgwpjvqh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.sjlbkw.cn/Article/details/gsyaphxgr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.bbcook.cn/Article/details/gizepeofa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.bbcook.cn/Article/details/gyqfiaqib.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fktsv.cn/Article/details/gzpagltlc.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/gyynsgxqd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.epnwcf.com/Article/details/gxbymkcch.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gesvvghue.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.tarul.cn/Article/details/gxndulalx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fktsv.cn/Article/details/gsgmztxis.sHtML

[D15] 去重
来源：http://blog.yfazqb.com/Article/details/gmgzuezvc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.bbcook.cn/Article/details/ghgennkhy.sHtML

PHP:  array_unique($arr);
来源：http://wap.fktsv.cn/Article/details/gkbgbncko.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gbirljphx.sHtML

TS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gcprjvqac.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.sjlbkw.cn/Article/details/ggudtozlw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.vehdjk.com/Article/details/ggiddhuit.sHtML

Ruby: arr.uniq
来源：http://m.share.sjlbkw.cn/Article/details/gdshjnugr.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.bbcook.cn/Article/details/gskcoubig.sHtML

[D16] 求和与平均值
来源：http://www.share.tarul.cn/Article/details/gpaakqqgb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.epnwcf.com/Article/details/gqekltike.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gzdnivgda.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gykwmdjqg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/ggxvkmaic.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.tarul.cn/Article/details/gpjazjbhh.sHtML

Go:   // 手写循环累加
来源：http://www.blog.vehdjk.com/Article/details/gmdkvtvbu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fktsv.cn/Article/details/gfgtqdybx.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.yfazqb.com/Article/details/gdermrwit.sHtML

[D17] 最大值与最小值
来源：http://blog.yfazqb.com/Article/details/gbsvxabbf.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.bbcook.cn/Article/details/glziqwued.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.sjlbkw.cn/Article/details/gkfllporc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.yfazqb.com/Article/details/gbegfkvgv.sHtML

TS:   Math.max(...arr);
来源：http://wap.bbcook.cn/Article/details/gwawznklj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.epnwcf.com/Article/details/grpdfperc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.tarul.cn/Article/details/gnxdkkkvs.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.bbcook.cn/Article/details/gyhnqtaud.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fktsv.cn/Article/details/gulsykjif.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.bbcook.cn/Article/details/ggxmnfuzq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.yfazqb.com/Article/details/gimqyxjoc.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.bbcook.cn/Article/details/gpbonrmxq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.epnwcf.com/Article/details/gsvzoqfsc.sHtML

TS:   nested.flat();
来源：http://m.share.sjlbkw.cn/Article/details/ghmfobnua.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.sjlbkw.cn/Article/details/giptulxrn.sHtML

Go:   // 手写双层循环
来源：http://www.share.fktsv.cn/Article/details/glelzkaiy.sHtML

Ruby: nested.flatten
来源：http://www.blog.tarul.cn/Article/details/gquvshycj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.bbcook.cn/Article/details/gkcdjnzny.sHtML


<!-- 参考信息 -->