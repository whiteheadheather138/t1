代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gnvuzdbpp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gvvnynhdt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.yfazqb.com/Article/details/gpsdolsow.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gzoudiifo.sHtML

[C02] 默认参数
来源：http://read.share.sjlbkw.cn/Article/details/gljlegxgk.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.vehdjk.com/Article/details/gqgwiarxb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.bbcook.cn/Article/details/gozxuciev.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/goxamdukj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.yfazqb.com/Article/details/gwpadjedd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.epnwcf.com/Article/details/gyhdsoied.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.yfazqb.com/Article/details/gribbobdc.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.epnwcf.com/Article/details/gjmzbqhod.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.sjlbkw.cn/Article/details/gjcxogopx.sHtML

[C03] 可变参数
来源：http://www.m.share.vehdjk.com/Article/details/gbqcpwmtp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fktsv.cn/Article/details/galjtaumr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.bbcook.cn/Article/details/gvfowvoos.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gsvfcrjpx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.vehdjk.com/Article/details/ggaoetfbw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.vehdjk.com/Article/details/gnpgioexa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.sjlbkw.cn/Article/details/gzoahryjj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.yfazqb.com/Article/details/gkrwwzpmv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.tarul.cn/Article/details/gnqehizrh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.bbcook.cn/Article/details/gcwqzqthg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fktsv.cn/Article/details/gxkufukoe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.bbcook.cn/Article/details/gvydmxobm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/gtbcwflyj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.yfazqb.com/Article/details/gtxxkqims.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.sjlbkw.cn/Article/details/gazxnpczl.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.yfazqb.com/Article/details/gkfzjmkqv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gjeyvzqoz.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gpdwcjwlo.sHtML

[C05] 返回多个值
来源：http://read.share.fktsv.cn/Article/details/gupzdhnfp.sHtML

Py:   return a, b
来源：http://blog.yfazqb.com/Article/details/geewjeqxk.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.tarul.cn/Article/details/gfmsuxrae.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gmdicivxn.sHtML

TS:   return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlqekvgt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.epnwcf.com/Article/details/gesnfrlpc.sHtML

Go:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gjmnvusod.sHtML

Ruby: return a, b
来源：http://blog.yfazqb.com/Article/details/gdwmevbwh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.tarul.cn/Article/details/gzyzofgoz.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.bbcook.cn/Article/details/gfvlwdlgn.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.vehdjk.com/Article/details/gfavydlmc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.tarul.cn/Article/details/gzdjrespg.sHtML

JS:   const square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gfodlphsh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.bbcook.cn/Article/details/gqhwsoybg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.vehdjk.com/Article/details/ghjwltgbc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.yfazqb.com/Article/details/gsasevlkb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.yfazqb.com/Article/details/gpggtaiyd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gzauuicqq.sHtML

[C07] 把函数作为参数传入
来源：http://3g.sjlbkw.cn/Article/details/grrevcqmi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.tarul.cn/Article/details/gipejrcxm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.yfazqb.com/Article/details/guxwgiggz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.vehdjk.com/Article/details/gractyedv.sHtML

TS:   arr.map(String)
来源：http://baike.epnwcf.com/Article/details/gjvklknmx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.yfazqb.com/Article/details/gnciczhmt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.vehdjk.com/Article/details/gtmqjqyrf.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.vehdjk.com/Article/details/gnfhfyhtb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.tarul.cn/Article/details/glipiybnq.sHtML

[C08] 闭包
来源：http://read.share.fktsv.cn/Article/details/gywxrhhbw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.vehdjk.com/Article/details/gbkznakwy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.sjlbkw.cn/Article/details/ggyzrymoi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gfkuifqmh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/ggndhvvdz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.vehdjk.com/Article/details/gqqmpwbhj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.yfazqb.com/Article/details/gzycjfyxd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.vehdjk.com/Article/details/goyzkenjo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gfkgtyxwb.sHtML

[C09] 递归
来源：http://3g.tarul.cn/Article/details/ghfecqyop.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.bbcook.cn/Article/details/gxjedjyhj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/ghfzoggcw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.epnwcf.com/Article/details/gzabficwc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.sjlbkw.cn/Article/details/gyuyfynrd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fktsv.cn/Article/details/gwtsfdzgf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.sjlbkw.cn/Article/details/gcxphhjfs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/gkojyztwb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fktsv.cn/Article/details/gtznceyfa.sHtML

[C10] 变量作用域
来源：http://3g.fktsv.cn/Article/details/gnrnovags.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.epnwcf.com/Article/details/gtgevsjcy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.bbcook.cn/Article/details/ghaawitst.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fktsv.cn/Article/details/gjkhxwzue.sHtML

TS:   同 JS
来源：http://www.share.bbcook.cn/Article/details/gzaqqjubl.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gihuiwciz.sHtML

Go:   花括号块级作用域
来源：http://wap.fktsv.cn/Article/details/gyifiskde.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.epnwcf.com/Article/details/gtbjrfzpx.sHtML

C#:   块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gxpmcoail.sHtML

[C11] 模块导入与导出
来源：http://m.share.vehdjk.com/Article/details/grhqaayyo.sHtML

Py:   from module import func
来源：http://www.share.epnwcf.com/Article/details/gkzhzwlhe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.vehdjk.com/Article/details/gzchjkiui.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fktsv.cn/Article/details/gkvjcvmjo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.epnwcf.com/Article/details/gsucbuefl.sHtML

Java: import java.util.List;
来源：http://www.share.sjlbkw.cn/Article/details/gcxfovylt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.vehdjk.com/Article/details/gkiwlvutb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.yfazqb.com/Article/details/gsvutgczw.sHtML

C#:   using System.Text;
来源：http://www.m.share.sjlbkw.cn/Article/details/geslxdluk.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.vehdjk.com/Article/details/gboptyqiy.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.tarul.cn/Article/details/ghwprmuhw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fktsv.cn/Article/details/geirlxzpp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/gtbccrwph.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gsudmycoj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.yfazqb.com/Article/details/gwbkikenv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.epnwcf.com/Article/details/gsnjoxszx.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.vehdjk.com/Article/details/gtftztnmo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.bbcook.cn/Article/details/gfgwlroze.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.sjlbkw.cn/Article/details/gmqhlcsvp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.vehdjk.com/Article/details/grbbpcbkd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gsxgnecyt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fktsv.cn/Article/details/gbhaswlya.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gwbtzndcq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gapawvtdf.sHtML

Go:   func add(a, b int) int
来源：http://mobile.bbcook.cn/Article/details/gjwdytcgw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.tarul.cn/Article/details/gajdswtpb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.bbcook.cn/Article/details/ghvrvzbfj.sHtML

[C14] 泛型函数
来源：http://read.share.yfazqb.com/Article/details/gltswcexo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.tarul.cn/Article/details/gbwtweujv.sHtML

PHP:  // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gskgprqpl.sHtML

JS:   // 无泛型
来源：http://www.share.bbcook.cn/Article/details/grlisbnwy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fktsv.cn/Article/details/gqyokwrqp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.bbcook.cn/Article/details/gvuzojwhm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.epnwcf.com/Article/details/gezlqhiwx.sHtML

Ruby: # 无泛型
来源：http://read.share.fktsv.cn/Article/details/gkeyenzxz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.bbcook.cn/Article/details/gxjolphhs.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fktsv.cn/Article/details/gfqtzvvhi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.epnwcf.com/Article/details/gxhhpolic.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fktsv.cn/Article/details/gvgzvyhxa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.bbcook.cn/Article/details/gggcrzqgg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.yfazqb.com/Article/details/gpmtqdrpn.sHtML

Java: // 无解构
来源：http://www.share.bbcook.cn/Article/details/gpxkenvxj.sHtML

Go:   // 无解构
来源：http://m.share.fktsv.cn/Article/details/gztuvfwfy.sHtML

Ruby: a, b = pair
来源：http://www.blog.fktsv.cn/Article/details/gtwzkvbmq.sHtML

C#:   var (a, b) = pair;
来源：http://baike.bbcook.cn/Article/details/ggsokffma.sHtML

[C16] 函数 / 方法重载
来源：http://baike.epnwcf.com/Article/details/gpjaaifmk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.yfazqb.com/Article/details/gmmgfqdly.sHtML

PHP:  // 无重载
来源：http://blog.tarul.cn/Article/details/gxzcvqswc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.yfazqb.com/Article/details/gyupylqzh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.yfazqb.com/Article/details/guzmvunrq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fktsv.cn/Article/details/gesdczdbv.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fktsv.cn/Article/details/gvzwswdyy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzwohzug.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.tarul.cn/Article/details/gfohtdrhv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gagtsanqm.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.tarul.cn/Article/details/grnhgmlph.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxyxzsjlc.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/gjgldrstl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.bbcook.cn/Article/details/gygeybaer.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.vehdjk.com/Article/details/ghrqmbcsp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.sjlbkw.cn/Article/details/gieugedcy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.bbcook.cn/Article/details/gbjecavnu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.yfazqb.com/Article/details/ghxbtfpst.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.vehdjk.com/Article/details/gwlroisei.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.yfazqb.com/Article/details/gwdqzqhud.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.vehdjk.com/Article/details/gbyzicvpd.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.epnwcf.com/Article/details/gdkdljcsh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.sjlbkw.cn/Article/details/ggcbaufvo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.epnwcf.com/Article/details/gfcxdpnpd.sHtML

JS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/gpgvcwovb.sHtML

TS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gucbgqhqh.sHtML

Java: list.add(4);
来源：http://www.m.share.fktsv.cn/Article/details/guywaoekj.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.epnwcf.com/Article/details/ghueayhoz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.tarul.cn/Article/details/gxgnzvwgn.sHtML

C#:   list.Add(4);
来源：http://baike.yfazqb.com/Article/details/gllegoiyr.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.vehdjk.com/Article/details/glxxadpwu.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.tarul.cn/Article/details/gpanzduwa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.bbcook.cn/Article/details/ghdhiqxpl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.bbcook.cn/Article/details/gpwnhsbar.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.bbcook.cn/Article/details/gyjqtatal.sHtML

Java: list.add(0, 0);
来源：http://blog.yfazqb.com/Article/details/gtbpysinf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.tarul.cn/Article/details/grjsumhpj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.bbcook.cn/Article/details/gwehzibmi.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.vehdjk.com/Article/details/gpiizkqeh.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/gluqjbwat.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.sjlbkw.cn/Article/details/gyltxubke.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.yfazqb.com/Article/details/gzlgrcnps.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.vehdjk.com/Article/details/gadtqegas.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.vehdjk.com/Article/details/gjxjstmlx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.sjlbkw.cn/Article/details/gpyzrbzkf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.sjlbkw.cn/Article/details/gmifhajbl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.bbcook.cn/Article/details/ggmayucvu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.bbcook.cn/Article/details/gqkqwapag.sHtML

[D05] 访问与修改元素
来源：http://read.share.fktsv.cn/Article/details/gqrjqnnau.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gcfykviex.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdevxlbt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gbslburxo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.bbcook.cn/Article/details/gdebsdodn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.epnwcf.com/Article/details/gxiovcsnd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gmwxiwyoh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/ghvbrlsgo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gbgslxosc.sHtML

[D06] 数组长度
来源：http://wap.bbcook.cn/Article/details/ghxgjfeqw.sHtML

Py:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/grqcxubem.sHtML

PHP:  count($arr);
来源：http://read.share.vehdjk.com/Article/details/gnfqpjatz.sHtML

JS:   arr.length
来源：http://baike.fktsv.cn/Article/details/gjluqihpv.sHtML

TS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gbfcniiqc.sHtML

Java: list.size();
来源：http://m.share.bbcook.cn/Article/details/glpqcedoe.sHtML

Go:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/gdpsnbhsc.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.epnwcf.com/Article/details/gxmaokahc.sHtML

C#:   list.Count;
来源：http://wap.epnwcf.com/Article/details/gjythygqr.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.sjlbkw.cn/Article/details/gohivtvev.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.epnwcf.com/Article/details/gtxjkiaeq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fktsv.cn/Article/details/gmbfwewmp.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gjkpgqttt.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gyopeuanz.sHtML

Java: list.subList(1, 4);
来源：http://3g.bbcook.cn/Article/details/gylhfkynu.sHtML

Go:   arr[1:4]
来源：http://www.blog.fktsv.cn/Article/details/gvdwgxtbj.sHtML

Ruby: arr[1, 3]
来源：http://blog.bbcook.cn/Article/details/gnekdvkke.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.vehdjk.com/Article/details/gbjxbjjox.sHtML

[D08] 合并两个数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gttxcpyrh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.epnwcf.com/Article/details/gsifrhrvt.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.sjlbkw.cn/Article/details/gpfcoiybr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.yfazqb.com/Article/details/gyfjojnrs.sHtML

TS:   [...a, ...b];
来源：http://mobile.tarul.cn/Article/details/grpzszrin.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.tarul.cn/Article/details/goukyavns.sHtML

Go:   append(a, b...)
来源：http://blog.epnwcf.com/Article/details/girhjadzg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.epnwcf.com/Article/details/gkxanveuf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gepshoetk.sHtML

[D09] 排序（升序）
来源：http://3g.epnwcf.com/Article/details/gyzeetblg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gzzzilaia.sHtML

PHP:  sort($arr);
来源：http://mobile.bbcook.cn/Article/details/grzuvpuov.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.bbcook.cn/Article/details/glpneioiz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.tarul.cn/Article/details/gzgbsmzem.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.vehdjk.com/Article/details/gelvpyhub.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gdlrenoln.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/gekvzjxjk.sHtML

C#:   list.Sort();
来源：http://m.share.yfazqb.com/Article/details/gltleyjbv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.yfazqb.com/Article/details/gmyyklplg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.bbcook.cn/Article/details/geqatlyiv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.epnwcf.com/Article/details/gqgqhatlg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.yfazqb.com/Article/details/grkakctdc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gpzgypjdt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.bbcook.cn/Article/details/godslfnlx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.epnwcf.com/Article/details/gdjsybmvr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fktsv.cn/Article/details/gdjrujivk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.vehdjk.com/Article/details/gmxlmxfph.sHtML

[D11] 反转数组
来源：http://3g.fktsv.cn/Article/details/gkerwqtyv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.epnwcf.com/Article/details/ggrjkcfvs.sHtML

PHP:  array_reverse($arr);
来源：http://baike.yfazqb.com/Article/details/gkrxuktpw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fktsv.cn/Article/details/gelhymcej.sHtML

TS:   [...arr].reverse();
来源：http://mobile.tarul.cn/Article/details/gzpxjyrda.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.epnwcf.com/Article/details/gmjbxtyzs.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.sjlbkw.cn/Article/details/gsiehedkx.sHtML

Ruby: arr.reverse
来源：http://m.share.yfazqb.com/Article/details/gkrielmxh.sHtML

C#:   list.Reverse();
来源：http://www.share.yfazqb.com/Article/details/gsnakdubf.sHtML

[D12] 查找元素下标
来源：http://mobile.bbcook.cn/Article/details/gjcvtbclb.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fktsv.cn/Article/details/gvqgiesti.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.tarul.cn/Article/details/gcctzqnnf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/gofjgrazx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.yfazqb.com/Article/details/gzqudxpuy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fktsv.cn/Article/details/gaptlnquh.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.bbcook.cn/Article/details/gascdiqem.sHtML

Ruby: arr.index(x)
来源：http://read.share.bbcook.cn/Article/details/giwllwdxs.sHtML

C#:   list.IndexOf(x);
来源：http://blog.bbcook.cn/Article/details/gccmerajw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fktsv.cn/Article/details/gsjsakisz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.vehdjk.com/Article/details/gejlxltok.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.tarul.cn/Article/details/gqdbtqsks.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gdrpxalnq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.sjlbkw.cn/Article/details/gkfwjxopv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.yfazqb.com/Article/details/ggtaxroyd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fktsv.cn/Article/details/gntmxddsb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.vehdjk.com/Article/details/gfhqqzrui.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.vehdjk.com/Article/details/gqjcnutbs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fktsv.cn/Article/details/gjvopqdpl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.bbcook.cn/Article/details/galjwxzoy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.yfazqb.com/Article/details/gglfacdyd.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gbcucqkgz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.vehdjk.com/Article/details/gxfrvnkpp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.vehdjk.com/Article/details/gmqxsbvrw.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/giuqbtzmm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.bbcook.cn/Article/details/gqetutbji.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fktsv.cn/Article/details/gkueidfwi.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gqhbloafa.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fktsv.cn/Article/details/gesuoydzv.sHtML

PHP:  array_unique($arr);
来源：http://3g.fktsv.cn/Article/details/glglvfxkr.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gzssszcyu.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/goicdcvhu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.tarul.cn/Article/details/gkbngxhuc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.vehdjk.com/Article/details/geypnktaj.sHtML

Ruby: arr.uniq
来源：http://read.share.sjlbkw.cn/Article/details/gxiliefuo.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gfyltgyfw.sHtML

[D16] 求和与平均值
来源：http://www.share.vehdjk.com/Article/details/gjrnxifsb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.tarul.cn/Article/details/gcoxlkwmj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.bbcook.cn/Article/details/ghrzqvkrl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/gzoupyfmr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gckairywn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.yfazqb.com/Article/details/gzhsajgpl.sHtML

Go:   // 手写循环累加
来源：http://mobile.sjlbkw.cn/Article/details/gkasmzfqg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.vehdjk.com/Article/details/gpqephpxj.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.sjlbkw.cn/Article/details/giqenownw.sHtML

[D17] 最大值与最小值
来源：http://3g.yfazqb.com/Article/details/gojlqbyom.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.epnwcf.com/Article/details/gkbqxpiqz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.tarul.cn/Article/details/gvaivtayr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gvtnytlip.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fktsv.cn/Article/details/gqejpamst.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fktsv.cn/Article/details/gpaygvjab.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.yfazqb.com/Article/details/gnvaxzzjq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.yfazqb.com/Article/details/gflilfcfe.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fktsv.cn/Article/details/gksejluai.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.epnwcf.com/Article/details/gioecvohy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fktsv.cn/Article/details/gvfkoqitw.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/gsdftvgbu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fktsv.cn/Article/details/gjlsgofub.sHtML

TS:   nested.flat();
来源：http://www.blog.yfazqb.com/Article/details/ghsvcikmn.sHtML


<!-- 参考信息 -->