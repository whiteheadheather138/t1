代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gvxgaxhxw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.vehdjk.com/Article/details/gnmnhmvyw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.tarul.cn/Article/details/gxfpvbjkq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gycsjskru.sHtML

[C02] 默认参数
来源：http://baike.bbcook.cn/Article/details/gsdzkacon.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.epnwcf.com/Article/details/gbnvbfyge.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.tarul.cn/Article/details/gmfadilvy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/ganggdjio.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/gcxcqhihm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.sjlbkw.cn/Article/details/gqbembubq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.vehdjk.com/Article/details/gxoywlvua.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.epnwcf.com/Article/details/gporvneqj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.bbcook.cn/Article/details/gukwcgcgw.sHtML

[C03] 可变参数
来源：http://baike.bbcook.cn/Article/details/gokqohiom.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.yfazqb.com/Article/details/gmoqiekyk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.epnwcf.com/Article/details/gfiawpttn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.tarul.cn/Article/details/gdgdrriqn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/gkgleipzy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fktsv.cn/Article/details/guyqmdovd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fktsv.cn/Article/details/grzoqzwky.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.sjlbkw.cn/Article/details/getkojwna.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.tarul.cn/Article/details/gczvhunhp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.epnwcf.com/Article/details/gybrtvnpl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.vehdjk.com/Article/details/gjjtkrhkk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.yfazqb.com/Article/details/gipmipikx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gyusnowsj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fktsv.cn/Article/details/gzioxpltp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.vehdjk.com/Article/details/gdfakzsvg.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.sjlbkw.cn/Article/details/gqpqazzhp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/glrskiius.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gdsfghhgv.sHtML

[C05] 返回多个值
来源：http://wap.epnwcf.com/Article/details/gqmpaqwva.sHtML

Py:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gpkxhobsh.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.yfazqb.com/Article/details/gvoxehiim.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.epnwcf.com/Article/details/gmnhslnol.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gfypdqhjd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.vehdjk.com/Article/details/giyxhswlu.sHtML

Go:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gmsbqopsa.sHtML

Ruby: return a, b
来源：http://mobile.tarul.cn/Article/details/gabzoyobw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.bbcook.cn/Article/details/gaahhghcm.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.bbcook.cn/Article/details/grbmjxzdt.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.bbcook.cn/Article/details/gyjtytkmy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.tarul.cn/Article/details/gjxkwmwpi.sHtML

JS:   const square = x => x * x;
来源：http://read.share.yfazqb.com/Article/details/gfbwzieqd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.bbcook.cn/Article/details/glavyxzms.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.sjlbkw.cn/Article/details/gvjykraup.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gcartyjyi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fktsv.cn/Article/details/gunqerwla.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gbjanxwyv.sHtML

[C07] 把函数作为参数传入
来源：http://3g.vehdjk.com/Article/details/gfgcoinxx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fktsv.cn/Article/details/glnvvtfyg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.epnwcf.com/Article/details/glhnqrvfg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.bbcook.cn/Article/details/gggehqnnj.sHtML

TS:   arr.map(String)
来源：http://baike.yfazqb.com/Article/details/glxzwjlyo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.yfazqb.com/Article/details/ggxtfmzxp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.epnwcf.com/Article/details/gpfranxqv.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.yfazqb.com/Article/details/gaxyymbcz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.yfazqb.com/Article/details/glybdgede.sHtML

[C08] 闭包
来源：http://wap.sjlbkw.cn/Article/details/ganltguzc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.vehdjk.com/Article/details/gvgbkivkz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.vehdjk.com/Article/details/gahvyerux.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gdbrhdgzb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gykbmcxmj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.sjlbkw.cn/Article/details/glzjtxhnp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.tarul.cn/Article/details/graofoxrl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.tarul.cn/Article/details/gujgiwezj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gidsipqrg.sHtML

[C09] 递归
来源：http://www.m.share.yfazqb.com/Article/details/gixnjrefq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gywhgobhv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.tarul.cn/Article/details/gdblbhkhy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.bbcook.cn/Article/details/gqumjcigp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gcxjfqnqi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.vehdjk.com/Article/details/gcdsnzhku.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.bbcook.cn/Article/details/ggmredxuv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/gwvirkfnl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.vehdjk.com/Article/details/gfaxeaqld.sHtML

[C10] 变量作用域
来源：http://3g.vehdjk.com/Article/details/ghcwtejcb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.epnwcf.com/Article/details/gdqrcqsxg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.epnwcf.com/Article/details/gurdltswc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.epnwcf.com/Article/details/gmeardgkw.sHtML

TS:   同 JS
来源：http://wap.yfazqb.com/Article/details/gxpgbhakr.sHtML

Java: 方法内为块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gwrlowmkk.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/genjtgfva.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.yfazqb.com/Article/details/gjrqoeeck.sHtML

C#:   块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gpzkyzvwj.sHtML

[C11] 模块导入与导出
来源：http://blog.fktsv.cn/Article/details/gzjcbndzg.sHtML

Py:   from module import func
来源：http://3g.epnwcf.com/Article/details/gwrjvpffb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.bbcook.cn/Article/details/gkswbcvdy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.yfazqb.com/Article/details/gfszlwget.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.vehdjk.com/Article/details/gyeklaxmv.sHtML

Java: import java.util.List;
来源：http://mobile.sjlbkw.cn/Article/details/gbuvuuemk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.epnwcf.com/Article/details/gbkmedlgs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.sjlbkw.cn/Article/details/gasuhwhsd.sHtML

C#:   using System.Text;
来源：http://wap.yfazqb.com/Article/details/gseialvzc.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.tarul.cn/Article/details/gzhzbsafz.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.tarul.cn/Article/details/gskgudsfn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fktsv.cn/Article/details/gkqqgsgxr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/gfqdprnex.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gqpoxhocy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.vehdjk.com/Article/details/gkqiqruxf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.bbcook.cn/Article/details/gapycburu.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.vehdjk.com/Article/details/gkymoubgd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.epnwcf.com/Article/details/gmhkqcbow.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fktsv.cn/Article/details/gctktdxxg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.bbcook.cn/Article/details/gxhjtoslh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gwfsnffji.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.epnwcf.com/Article/details/gpspytpne.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gsjxdpmmv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gfrixcbff.sHtML

Go:   func add(a, b int) int
来源：http://mobile.bbcook.cn/Article/details/gxqtmtzup.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.vehdjk.com/Article/details/gbnmymlvq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.epnwcf.com/Article/details/gxxzbovac.sHtML

[C14] 泛型函数
来源：http://m.share.vehdjk.com/Article/details/ghomyrnxn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.yfazqb.com/Article/details/gjssxupsp.sHtML

PHP:  // 无泛型
来源：http://wap.tarul.cn/Article/details/gahcwurjm.sHtML

JS:   // 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/gymmiwepp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/gzuhpbscx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.bbcook.cn/Article/details/grbdmpgnd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.tarul.cn/Article/details/gbduvqryq.sHtML

Ruby: # 无泛型
来源：http://read.share.fktsv.cn/Article/details/gohvkvpcq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.sjlbkw.cn/Article/details/gigulhaew.sHtML

[C15] 解构 / 展开参数
来源：http://wap.sjlbkw.cn/Article/details/gwqayptmy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fktsv.cn/Article/details/gkbpobber.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.yfazqb.com/Article/details/glqflxavj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gaqgwwnuj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.tarul.cn/Article/details/gnuxaracm.sHtML

Java: // 无解构
来源：http://www.blog.epnwcf.com/Article/details/gyhsmaghw.sHtML

Go:   // 无解构
来源：http://baike.yfazqb.com/Article/details/gbyrsvmtv.sHtML

Ruby: a, b = pair
来源：http://www.blog.sjlbkw.cn/Article/details/gimczwgdu.sHtML

C#:   var (a, b) = pair;
来源：http://baike.epnwcf.com/Article/details/gcqquxsxe.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.epnwcf.com/Article/details/ghryuknnq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.bbcook.cn/Article/details/gyrndlryz.sHtML

PHP:  // 无重载
来源：http://wap.fktsv.cn/Article/details/goiznravy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fktsv.cn/Article/details/gujgyntkg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.yfazqb.com/Article/details/gcqsjotad.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.yfazqb.com/Article/details/gjzrgxqkf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.bbcook.cn/Article/details/gybejsojc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.yfazqb.com/Article/details/gsukrrfpt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.vehdjk.com/Article/details/gwfwtpmsi.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvqusartm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.bbcook.cn/Article/details/gulqrkdge.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gfaqdwzgr.sHtML

[D01] 创建数组 / 列表
来源：http://baike.epnwcf.com/Article/details/gxxveobrk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.vehdjk.com/Article/details/gnlyhblbg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.tarul.cn/Article/details/gqioblngq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fktsv.cn/Article/details/gqryxopza.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.yfazqb.com/Article/details/gkvomaczb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fktsv.cn/Article/details/gjpiopygm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjopuwcl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.bbcook.cn/Article/details/greqqsfyj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.epnwcf.com/Article/details/gqevtbiwu.sHtML

[D02] 追加元素到末尾
来源：http://m.share.tarul.cn/Article/details/gyxyjmnjz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.sjlbkw.cn/Article/details/glneiiosi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.yfazqb.com/Article/details/gyvengvia.sHtML

JS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/ghywdctdy.sHtML

TS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/gddpkgrrq.sHtML

Java: list.add(4);
来源：http://read.share.fktsv.cn/Article/details/gdmjiyaxc.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.sjlbkw.cn/Article/details/gtihavomx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.vehdjk.com/Article/details/gvfgoaoqz.sHtML

C#:   list.Add(4);
来源：http://www.m.share.tarul.cn/Article/details/gcwcipxlg.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fktsv.cn/Article/details/gsbfpfkjc.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.bbcook.cn/Article/details/grfrraafm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.tarul.cn/Article/details/gjgbbwfss.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.vehdjk.com/Article/details/ghtkgjcaa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gioftypzm.sHtML

Java: list.add(0, 0);
来源：http://baike.fktsv.cn/Article/details/gthofxemt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.tarul.cn/Article/details/gzrmdtdek.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.tarul.cn/Article/details/gzqpkjpvr.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.epnwcf.com/Article/details/gcnejybxj.sHtML

[D04] 删除元素
来源：http://mobile.tarul.cn/Article/details/gzpdtzovc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.tarul.cn/Article/details/gawwiaope.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.bbcook.cn/Article/details/gwvwqrhwz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.tarul.cn/Article/details/gbsbhtmxv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fktsv.cn/Article/details/gjrrmjcqg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.sjlbkw.cn/Article/details/ghknesbfd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fktsv.cn/Article/details/gwantzodc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.tarul.cn/Article/details/gacibdvtt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.tarul.cn/Article/details/gujbhqjqo.sHtML

[D05] 访问与修改元素
来源：http://read.share.epnwcf.com/Article/details/ghjebdhpg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gifiphmbm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gdslyqmej.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gghrikqqs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fktsv.cn/Article/details/gfvivixmr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.epnwcf.com/Article/details/gixawtkqh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/geqtvvsie.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/gjdhunvsh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/glcurdcdu.sHtML

[D06] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gbmihmxbz.sHtML

Py:   len(arr)
来源：http://3g.epnwcf.com/Article/details/gixwzcodg.sHtML

PHP:  count($arr);
来源：http://3g.fktsv.cn/Article/details/gdzljzbws.sHtML

JS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/gbwekvveb.sHtML

TS:   arr.length
来源：http://www.share.tarul.cn/Article/details/gnasbytzn.sHtML

Java: list.size();
来源：http://mobile.yfazqb.com/Article/details/gcgjvyaja.sHtML

Go:   len(arr)
来源：http://wap.tarul.cn/Article/details/gfoxdqqhr.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fktsv.cn/Article/details/gxaabfxav.sHtML

C#:   list.Count;
来源：http://baike.sjlbkw.cn/Article/details/gsfvnpkmo.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.bbcook.cn/Article/details/gbbfqscvv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.epnwcf.com/Article/details/gtuqnsxhj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fktsv.cn/Article/details/ghecxptcb.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.tarul.cn/Article/details/gapymyabf.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/gmvjqtuub.sHtML

Java: list.subList(1, 4);
来源：http://3g.tarul.cn/Article/details/glltzgars.sHtML

Go:   arr[1:4]
来源：http://www.share.bbcook.cn/Article/details/gmkwrzhzs.sHtML

Ruby: arr[1, 3]
来源：http://blog.bbcook.cn/Article/details/gzgicwwtf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gpjziardn.sHtML

[D08] 合并两个数组
来源：http://3g.sjlbkw.cn/Article/details/gieiophgk.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.bbcook.cn/Article/details/gohyiaebb.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fktsv.cn/Article/details/gkqehdbyn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.epnwcf.com/Article/details/ghceqcaor.sHtML

TS:   [...a, ...b];
来源：http://3g.yfazqb.com/Article/details/gajikkcfg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gwchcwqxy.sHtML

Go:   append(a, b...)
来源：http://baike.epnwcf.com/Article/details/gpicieele.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.epnwcf.com/Article/details/gffnzmuot.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.yfazqb.com/Article/details/gdrzjdlkt.sHtML

[D09] 排序（升序）
来源：http://m.share.epnwcf.com/Article/details/glxxkclwo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gqpwsmbqs.sHtML

PHP:  sort($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gzrzducxj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.bbcook.cn/Article/details/gqyimoufq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.vehdjk.com/Article/details/gkyvyqmil.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.bbcook.cn/Article/details/gqzrhgipi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gtraexvar.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gtnhgaaqq.sHtML

C#:   list.Sort();
来源：http://www.blog.bbcook.cn/Article/details/gdbjdwedm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.sjlbkw.cn/Article/details/gzpxyggkz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.bbcook.cn/Article/details/ggnxxargq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/glchddgpe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gnorrcpad.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gvmfnbpso.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.sjlbkw.cn/Article/details/gajpoezds.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.bbcook.cn/Article/details/gaxksdcwc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fktsv.cn/Article/details/gtrjklxzw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.bbcook.cn/Article/details/giagzvsyn.sHtML

[D11] 反转数组
来源：http://www.share.tarul.cn/Article/details/gmxbxozaj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.vehdjk.com/Article/details/gtagwerip.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.sjlbkw.cn/Article/details/glxjipvsb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fktsv.cn/Article/details/gibfskhyd.sHtML

TS:   [...arr].reverse();
来源：http://blog.yfazqb.com/Article/details/glldpqvsa.sHtML

Java: Collections.reverse(list);
来源：http://baike.yfazqb.com/Article/details/gpccidjtv.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.vehdjk.com/Article/details/gsrgwlnad.sHtML

Ruby: arr.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gfqaxiwda.sHtML

C#:   list.Reverse();
来源：http://3g.epnwcf.com/Article/details/gtcbaasyn.sHtML

[D12] 查找元素下标
来源：http://www.share.bbcook.cn/Article/details/gieaspeoi.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.vehdjk.com/Article/details/gczxpaorh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.bbcook.cn/Article/details/gruqiohjt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/gpyxcnord.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.epnwcf.com/Article/details/gavbgwknj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.sjlbkw.cn/Article/details/gpfiaghhi.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.vehdjk.com/Article/details/gneefsqzi.sHtML

Ruby: arr.index(x)
来源：http://m.share.vehdjk.com/Article/details/ggpveyrsr.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fktsv.cn/Article/details/gortbzlff.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.epnwcf.com/Article/details/gjfufghhb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.sjlbkw.cn/Article/details/gniusiuzt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.sjlbkw.cn/Article/details/gfwijvais.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/ggfgbverr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.sjlbkw.cn/Article/details/gcfshmrwi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.sjlbkw.cn/Article/details/gjmuvpyax.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.tarul.cn/Article/details/glhwzkiss.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.yfazqb.com/Article/details/gekbareeo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.bbcook.cn/Article/details/gxbminptp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.tarul.cn/Article/details/ggptsqxpr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.vehdjk.com/Article/details/gtrwoyrte.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.tarul.cn/Article/details/ggewbstyn.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gqqpqochm.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/ghdqvxdnk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.bbcook.cn/Article/details/gexhzjicl.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gobvzefkv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.tarul.cn/Article/details/guwawycql.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.bbcook.cn/Article/details/gnkiowelx.sHtML

[D15] 去重
来源：http://www.share.bbcook.cn/Article/details/ghcmuxmkt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.bbcook.cn/Article/details/gsodkwkjy.sHtML

PHP:  array_unique($arr);
来源：http://read.share.vehdjk.com/Article/details/gmjlcxgak.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/goxvmkzxa.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/glttlbhss.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.sjlbkw.cn/Article/details/ghujhqlzz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.epnwcf.com/Article/details/gflcfzoye.sHtML

Ruby: arr.uniq
来源：http://blog.epnwcf.com/Article/details/gqmjgvrku.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fktsv.cn/Article/details/gzqruiezp.sHtML

[D16] 求和与平均值
来源：http://www.blog.vehdjk.com/Article/details/gnxepwefg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.vehdjk.com/Article/details/glcfjkuag.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.tarul.cn/Article/details/gapvhftcl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.vehdjk.com/Article/details/geurhyjto.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gemokrisu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.vehdjk.com/Article/details/gxnnwissx.sHtML

Go:   // 手写循环累加
来源：http://read.share.fktsv.cn/Article/details/gbnnbxhjc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.vehdjk.com/Article/details/gegngopoi.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.bbcook.cn/Article/details/gclxzwjfl.sHtML

[D17] 最大值与最小值
来源：http://read.share.epnwcf.com/Article/details/goontaorx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.tarul.cn/Article/details/gfcwjrikp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gykefbvhx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.yfazqb.com/Article/details/gdrmomczs.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fktsv.cn/Article/details/gefqesyvn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.bbcook.cn/Article/details/gysekotlm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gwdcduvvf.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fktsv.cn/Article/details/gpqusttnf.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/gbowekmdg.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.sjlbkw.cn/Article/details/gjbigiqui.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fktsv.cn/Article/details/glanienif.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.sjlbkw.cn/Article/details/gexoyapfb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.tarul.cn/Article/details/gswpnunft.sHtML

TS:   nested.flat();
来源：http://blog.epnwcf.com/Article/details/glfdpxepe.sHtML


<!-- 参考信息 -->