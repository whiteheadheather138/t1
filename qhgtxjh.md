代发 wailian999

Py:   if not data: return
来源：http://www.blog.sjlbkw.cn/Article/details/glmrhyhaz.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.sjlbkw.cn/Article/details/gqoljpclg.sHtML

JS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gfldtfnlx.sHtML

TS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/guxurlsms.sHtML

Java: if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gotswkhit.sHtML

Go:   if data == nil { return }
来源：http://wap.epnwcf.com/Article/details/gtfwpmoka.sHtML

Ruby: return if data.nil?
来源：http://read.share.epnwcf.com/Article/details/ggrorrbpf.sHtML

C#:   if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gmnpbpfif.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gxgimacvk.sHtML

C. 函数与作用域
来源：http://www.share.bbcook.cn/Article/details/gjhxiborr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtnrgzqzx.sHtML

[C01] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/gwamuwgji.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fktsv.cn/Article/details/gylomrlki.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gnfofkvsl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gydebbbjl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gqdyjartg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gfczernum.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gukwqugvh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.epnwcf.com/Article/details/gmnytyxts.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/ghnkztiex.sHtML

[C02] 默认参数
来源：http://www.m.share.epnwcf.com/Article/details/grnbjmsit.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.vehdjk.com/Article/details/gsjmhoque.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.yfazqb.com/Article/details/gnencmaqr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gsrlafeaz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/grcqmjzbp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.vehdjk.com/Article/details/gfvniqlpj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.tarul.cn/Article/details/gmxwtffjl.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.bbcook.cn/Article/details/gspxfymbs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.yfazqb.com/Article/details/gbmvxrbla.sHtML

[C03] 可变参数
来源：http://blog.vehdjk.com/Article/details/gteonuqoa.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fktsv.cn/Article/details/guxcdpogj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlblfjaq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.tarul.cn/Article/details/goepfumts.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gafevpbnn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fktsv.cn/Article/details/gdiknbnla.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.sjlbkw.cn/Article/details/gbubweowx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.tarul.cn/Article/details/gcfaxggua.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.tarul.cn/Article/details/gspfroasm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.tarul.cn/Article/details/gonlyxkbz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.bbcook.cn/Article/details/gsjtwrbop.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fktsv.cn/Article/details/gjiqwifjd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/gefqqumvy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fktsv.cn/Article/details/gdwfwixth.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fktsv.cn/Article/details/gbcvvfczl.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fktsv.cn/Article/details/ghyezealt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gpcgatnis.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gkkvfnihf.sHtML

[C05] 返回多个值
来源：http://wap.fktsv.cn/Article/details/gorriygvi.sHtML

Py:   return a, b
来源：http://blog.vehdjk.com/Article/details/gperqqaws.sHtML

PHP:  return [$a, $b];
来源：http://m.share.bbcook.cn/Article/details/gzsifrpjw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gfyoxwgir.sHtML

TS:   return { a, b };
来源：http://www.blog.tarul.cn/Article/details/glbbqthxe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.yfazqb.com/Article/details/gosuzuffw.sHtML

Go:   return a, b
来源：http://wap.yfazqb.com/Article/details/gaxeozdpd.sHtML

Ruby: return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gvhcwqooh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.epnwcf.com/Article/details/gxgkymycw.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/gihhusire.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fktsv.cn/Article/details/grptsrkwd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.vehdjk.com/Article/details/gkmmwuttr.sHtML

JS:   const square = x => x * x;
来源：http://blog.bbcook.cn/Article/details/gijmjqxlu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.sjlbkw.cn/Article/details/guqxadzhw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.epnwcf.com/Article/details/gilfoyatw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.vehdjk.com/Article/details/giofwufmy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fktsv.cn/Article/details/grdmlqlic.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gbhupdiwx.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvfmcuse.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.tarul.cn/Article/details/gszrsdgnr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.bbcook.cn/Article/details/gkxpwycvi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fktsv.cn/Article/details/geldjzklm.sHtML

TS:   arr.map(String)
来源：http://www.blog.tarul.cn/Article/details/gkoqsxgqq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.vehdjk.com/Article/details/gynavcqil.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.vehdjk.com/Article/details/giydtdyaw.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fktsv.cn/Article/details/gvqvzkuca.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.bbcook.cn/Article/details/glcijdayz.sHtML

[C08] 闭包
来源：http://blog.sjlbkw.cn/Article/details/gyydnsljd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.epnwcf.com/Article/details/ggmwfqxhu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.vehdjk.com/Article/details/ghgalhcsq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gcqymrhol.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gjehuftrq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.sjlbkw.cn/Article/details/gukmsbuzs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fktsv.cn/Article/details/gzvpbniyf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.bbcook.cn/Article/details/ghupumgsv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gkoalyjiw.sHtML

[C09] 递归
来源：http://read.share.bbcook.cn/Article/details/gpfootztf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.tarul.cn/Article/details/grqiwvaoj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.yfazqb.com/Article/details/gjuprtiqz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gepbohaig.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/gvnteluuq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.bbcook.cn/Article/details/guuecocfz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.vehdjk.com/Article/details/ggrglnjlb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.tarul.cn/Article/details/gguydvqzn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.sjlbkw.cn/Article/details/ggkshfnyf.sHtML

[C10] 变量作用域
来源：http://read.share.yfazqb.com/Article/details/gixzndohe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.tarul.cn/Article/details/gcnjvgued.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fktsv.cn/Article/details/gqlyfibft.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/ghizypzwy.sHtML

TS:   同 JS
来源：http://wap.bbcook.cn/Article/details/gujoflltr.sHtML

Java: 方法内为块级作用域
来源：http://3g.yfazqb.com/Article/details/gnpcqjwwr.sHtML

Go:   花括号块级作用域
来源：http://m.share.yfazqb.com/Article/details/gaudvncti.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.sjlbkw.cn/Article/details/gpgxtuwxm.sHtML

C#:   块级作用域
来源：http://m.share.yfazqb.com/Article/details/gbffsolap.sHtML

[C11] 模块导入与导出
来源：http://read.share.vehdjk.com/Article/details/gajlwmjmu.sHtML

Py:   from module import func
来源：http://m.share.epnwcf.com/Article/details/gpohbujes.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.bbcook.cn/Article/details/grplydicb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.bbcook.cn/Article/details/gpxqcmvqz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.epnwcf.com/Article/details/grkghenwv.sHtML

Java: import java.util.List;
来源：http://read.share.bbcook.cn/Article/details/gdhugimws.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.yfazqb.com/Article/details/gumweaipc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/gnrxbtedo.sHtML

C#:   using System.Text;
来源：http://www.share.sjlbkw.cn/Article/details/gzfqujmjn.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fktsv.cn/Article/details/gsmxbtwxv.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.tarul.cn/Article/details/gesfrksrt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.bbcook.cn/Article/details/gnmhgeytj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/ggmusnlvm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/gwlnpedrw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.vehdjk.com/Article/details/gpdgmakdn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcohaczvm.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.yfazqb.com/Article/details/gfzgvduzq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.vehdjk.com/Article/details/gqewzlfap.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.sjlbkw.cn/Article/details/gdainjeft.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.tarul.cn/Article/details/gspzjmdpw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gczktngmn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.bbcook.cn/Article/details/gpzskgjdx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/ginyxilst.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gpkjhvdjm.sHtML

Go:   func add(a, b int) int
来源：http://baike.sjlbkw.cn/Article/details/gbdlczrih.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.yfazqb.com/Article/details/glburtllz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.yfazqb.com/Article/details/gppjnwwxm.sHtML

[C14] 泛型函数
来源：http://www.m.share.yfazqb.com/Article/details/gykxpfnem.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.vehdjk.com/Article/details/gytmqfdks.sHtML

PHP:  // 无泛型
来源：http://blog.vehdjk.com/Article/details/givtthkuy.sHtML

JS:   // 无泛型
来源：http://3g.tarul.cn/Article/details/ggkczztmv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.yfazqb.com/Article/details/gsbutdfyb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.tarul.cn/Article/details/ggxyvnaje.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.bbcook.cn/Article/details/gltxdtgzx.sHtML

Ruby: # 无泛型
来源：http://www.blog.bbcook.cn/Article/details/ghigeqxjm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.yfazqb.com/Article/details/gbvfanefp.sHtML

[C15] 解构 / 展开参数
来源：http://blog.bbcook.cn/Article/details/godchsare.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.yfazqb.com/Article/details/gyfgkdrvi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.epnwcf.com/Article/details/gztpeyrmh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gnnirbhcp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gyukmmzen.sHtML

Java: // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gbyqgnkzc.sHtML

Go:   // 无解构
来源：http://read.share.vehdjk.com/Article/details/gqdefhcae.sHtML

Ruby: a, b = pair
来源：http://m.share.epnwcf.com/Article/details/gpbwuttsj.sHtML

C#:   var (a, b) = pair;
来源：http://blog.epnwcf.com/Article/details/gdfejsjgb.sHtML

[C16] 函数 / 方法重载
来源：http://wap.bbcook.cn/Article/details/gkfszsmgz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.tarul.cn/Article/details/geqaabkty.sHtML

PHP:  // 无重载
来源：http://3g.tarul.cn/Article/details/gdxtmbyxx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.tarul.cn/Article/details/ggvriscan.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.yfazqb.com/Article/details/gbhdjjntl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.epnwcf.com/Article/details/gqedofric.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.sjlbkw.cn/Article/details/gzaqiobsl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.bbcook.cn/Article/details/glxbvrfqd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqetdpiax.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gsqewdphz.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.yfazqb.com/Article/details/glzyopscq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gxtmttnny.sHtML

[D01] 创建数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gmcijuzfq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.yfazqb.com/Article/details/gquixplos.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.vehdjk.com/Article/details/gcxksnqff.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.yfazqb.com/Article/details/gafekrfgm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.vehdjk.com/Article/details/gbllhbshx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fktsv.cn/Article/details/gucmdumnw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.tarul.cn/Article/details/guyesuaif.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.yfazqb.com/Article/details/gxgmpyaok.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.vehdjk.com/Article/details/gonpkesix.sHtML

[D02] 追加元素到末尾
来源：http://m.share.sjlbkw.cn/Article/details/glvduoxze.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.epnwcf.com/Article/details/gqpqsazpp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fktsv.cn/Article/details/gobksfznn.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/ggwlcsdxk.sHtML

TS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/gkyipmkdu.sHtML

Java: list.add(4);
来源：http://www.m.share.epnwcf.com/Article/details/gfruwdovn.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.vehdjk.com/Article/details/gjzsqrqmk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.vehdjk.com/Article/details/gnxtfaioq.sHtML

C#:   list.Add(4);
来源：http://wap.bbcook.cn/Article/details/gqkftdiwh.sHtML

[D03] 在指定位置插入元素
来源：http://wap.sjlbkw.cn/Article/details/gzoliiygt.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fktsv.cn/Article/details/gsmplbspd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.epnwcf.com/Article/details/gfefbhgby.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fktsv.cn/Article/details/ghqkeabzb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.tarul.cn/Article/details/guluwplzq.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fktsv.cn/Article/details/grqjrqomn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fktsv.cn/Article/details/glvqgvgpm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.tarul.cn/Article/details/gfwxcvnxd.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.vehdjk.com/Article/details/gpjjwisvl.sHtML

[D04] 删除元素
来源：http://m.share.bbcook.cn/Article/details/ggbelljzd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.yfazqb.com/Article/details/gdyxxwwrv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/gkqmrwkcc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.sjlbkw.cn/Article/details/gpbfobohf.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.tarul.cn/Article/details/gztqdudhr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrnvqdlc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.yfazqb.com/Article/details/gsdyythcr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.tarul.cn/Article/details/gxswmvfbm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.bbcook.cn/Article/details/gkzteaodp.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fktsv.cn/Article/details/gskmumnef.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gqodyxsxf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gxhkliivo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gunxefivt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.bbcook.cn/Article/details/gfsdobrfb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.tarul.cn/Article/details/gphaylwok.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gsvkhjnjg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/gmwzhykbk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gnyqvmgno.sHtML

[D06] 数组长度
来源：http://mobile.epnwcf.com/Article/details/goeeaugng.sHtML

Py:   len(arr)
来源：http://blog.bbcook.cn/Article/details/gfnxeivpr.sHtML

PHP:  count($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gngmhxejh.sHtML

JS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/gwrywnhks.sHtML

TS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gzthvxmle.sHtML

Java: list.size();
来源：http://www.blog.epnwcf.com/Article/details/gnowojpih.sHtML

Go:   len(arr)
来源：http://blog.epnwcf.com/Article/details/gelocljlk.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.tarul.cn/Article/details/ghmygsbhj.sHtML

C#:   list.Count;
来源：http://www.share.vehdjk.com/Article/details/gxeczqfjb.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.sjlbkw.cn/Article/details/gzihbdiac.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fktsv.cn/Article/details/gxhmcvohg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/gavssmjzu.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gzhfnzkhl.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gyraqglav.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gyvwhkwtu.sHtML

Go:   arr[1:4]
来源：http://baike.fktsv.cn/Article/details/gwqshferz.sHtML

Ruby: arr[1, 3]
来源：http://read.share.sjlbkw.cn/Article/details/gqyerwila.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.sjlbkw.cn/Article/details/gxvomrram.sHtML

[D08] 合并两个数组
来源：http://m.share.bbcook.cn/Article/details/gewfeiqqf.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.yfazqb.com/Article/details/gesntbxhi.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.sjlbkw.cn/Article/details/gbdorydaq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.vehdjk.com/Article/details/gehhoewqe.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.epnwcf.com/Article/details/gznefotqp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.bbcook.cn/Article/details/gfnhmgmun.sHtML

Go:   append(a, b...)
来源：http://mobile.sjlbkw.cn/Article/details/gvcfceoel.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.bbcook.cn/Article/details/gwqsbhcwg.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.vehdjk.com/Article/details/gnbatoeba.sHtML

[D09] 排序（升序）
来源：http://baike.sjlbkw.cn/Article/details/gcloeghlz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gqdpoyuoi.sHtML

PHP:  sort($arr);
来源：http://baike.tarul.cn/Article/details/gssieopyr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/gvlwplctd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.yfazqb.com/Article/details/ghoyhldwp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.yfazqb.com/Article/details/gdjqwrdhy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/ghiycayfh.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/gkbegxwri.sHtML

C#:   list.Sort();
来源：http://mobile.sjlbkw.cn/Article/details/gktlztwnu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.sjlbkw.cn/Article/details/gbixvghdy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.vehdjk.com/Article/details/gzkcsjirk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.epnwcf.com/Article/details/ghomzinkd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.sjlbkw.cn/Article/details/gnvfrextj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/gxtrsbjgu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.bbcook.cn/Article/details/gptishjik.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.sjlbkw.cn/Article/details/gjkuxqmig.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.vehdjk.com/Article/details/gawfeanie.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.yfazqb.com/Article/details/gkfuponkw.sHtML

[D11] 反转数组
来源：http://blog.sjlbkw.cn/Article/details/gglrpmgft.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.bbcook.cn/Article/details/gmgkcqsii.sHtML

PHP:  array_reverse($arr);
来源：http://baike.sjlbkw.cn/Article/details/gxosohscj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.tarul.cn/Article/details/gtxmxodtp.sHtML

TS:   [...arr].reverse();
来源：http://blog.yfazqb.com/Article/details/gwnvenvxj.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fktsv.cn/Article/details/gtcuboczw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gagxcmzcs.sHtML

Ruby: arr.reverse
来源：http://3g.bbcook.cn/Article/details/giqhypmjs.sHtML

C#:   list.Reverse();
来源：http://mobile.bbcook.cn/Article/details/gtahawerm.sHtML

[D12] 查找元素下标
来源：http://3g.vehdjk.com/Article/details/grhhonqpd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.tarul.cn/Article/details/gnqrtjuxe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.epnwcf.com/Article/details/gceaxnfqd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/ghdydhkkv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.bbcook.cn/Article/details/gkdwizjqz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.bbcook.cn/Article/details/gmvikiczk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gqfspchcj.sHtML

Ruby: arr.index(x)
来源：http://blog.yfazqb.com/Article/details/gjuishhgz.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.vehdjk.com/Article/details/gtdyupmsy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.yfazqb.com/Article/details/gtjugnphp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.tarul.cn/Article/details/gxdnnrmix.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fktsv.cn/Article/details/gbxeclnes.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.sjlbkw.cn/Article/details/gvxitqgfn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.vehdjk.com/Article/details/gcloirygn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gcicgomti.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.tarul.cn/Article/details/gztcmxkui.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fktsv.cn/Article/details/gusjgmlcw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.epnwcf.com/Article/details/gchmvljkl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/gvjjxllks.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.vehdjk.com/Article/details/gfdpodlic.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.yfazqb.com/Article/details/gwoitccmd.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/gwdducien.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fktsv.cn/Article/details/glnkilgrm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.bbcook.cn/Article/details/gxqhovxyy.sHtML

Go:   // 手写循环
来源：http://www.share.tarul.cn/Article/details/gbmhsvhwm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.vehdjk.com/Article/details/gkspawnju.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.vehdjk.com/Article/details/gtpdaztbs.sHtML

[D15] 去重
来源：http://blog.fktsv.cn/Article/details/gkcpoxoiu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.sjlbkw.cn/Article/details/gpoknufeg.sHtML

PHP:  array_unique($arr);
来源：http://baike.fktsv.cn/Article/details/gyrjupiwi.sHtML

JS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/gjgafoooy.sHtML

TS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/guehypkir.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.yfazqb.com/Article/details/gptnneexr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.vehdjk.com/Article/details/gpwbpfezp.sHtML

Ruby: arr.uniq
来源：http://www.blog.epnwcf.com/Article/details/gfegzropa.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fktsv.cn/Article/details/gajkyufsv.sHtML

[D16] 求和与平均值
来源：http://m.share.fktsv.cn/Article/details/giyvaacic.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.yfazqb.com/Article/details/gonhbqmes.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.vehdjk.com/Article/details/gwfylwqdv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/gscrdbjnw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gllnqispo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fktsv.cn/Article/details/gpsbfdjes.sHtML

Go:   // 手写循环累加
来源：http://3g.tarul.cn/Article/details/gkhmwgjep.sHtML


<!-- 参考信息 -->