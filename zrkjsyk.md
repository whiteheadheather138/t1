代发 wailian999

Go:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnkngmbq.sHtML

Ruby: a && b || !c
来源：http://wap.yfazqb.com/Article/details/ggadheyni.sHtML

C#:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gnemougyx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.tarul.cn/Article/details/gphhnogeu.sHtML

Py:   if not data: return
来源：http://wap.epnwcf.com/Article/details/gbohyqltm.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.vehdjk.com/Article/details/gbrnbmsch.sHtML

JS:   if (!data) return;
来源：http://www.share.epnwcf.com/Article/details/govrlcldm.sHtML

TS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/gzbxdndde.sHtML

Java: if (data == null) return;
来源：http://m.share.vehdjk.com/Article/details/gwajgsgaw.sHtML

Go:   if data == nil { return }
来源：http://wap.bbcook.cn/Article/details/gfzdcqlds.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpdewldc.sHtML

C#:   if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gayjmtqav.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gemrqcrag.sHtML

C. 函数与作用域
来源：http://3g.vehdjk.com/Article/details/gkbrtuatk.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gpxeuqqwz.sHtML

[C01] 定义函数
来源：http://blog.tarul.cn/Article/details/gcgwvvhdm.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.bbcook.cn/Article/details/gadsmerra.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/grxweszwn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/grkfjpjfq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gttrfcnfh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gtpdxnoes.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.epnwcf.com/Article/details/gorrnoqco.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.yfazqb.com/Article/details/gwixwubcg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gtgqqdxzp.sHtML

[C02] 默认参数
来源：http://read.share.bbcook.cn/Article/details/gyhbymxxi.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.vehdjk.com/Article/details/gqebfruml.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.yfazqb.com/Article/details/gzmctrniw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gwwnzjbjw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gwthpiswu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.sjlbkw.cn/Article/details/gkyuobzis.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.bbcook.cn/Article/details/govbepwby.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.tarul.cn/Article/details/gnyaeinra.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.yfazqb.com/Article/details/gkerkfhrc.sHtML

[C03] 可变参数
来源：http://read.share.vehdjk.com/Article/details/gtpqxvdtx.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.tarul.cn/Article/details/gxphyzozg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.yfazqb.com/Article/details/grxroutxt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gqjidhueo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gtrtcitgu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fktsv.cn/Article/details/gttlusvsz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.epnwcf.com/Article/details/gkpppmkuh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fktsv.cn/Article/details/gsyllliga.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.epnwcf.com/Article/details/ghltwlxec.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fktsv.cn/Article/details/geypouhgg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fktsv.cn/Article/details/gkgqgzuda.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.vehdjk.com/Article/details/gueejqjzu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gcvbgeoxt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.yfazqb.com/Article/details/gkblwrtsd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.yfazqb.com/Article/details/gvnvawvyw.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.tarul.cn/Article/details/gjgutaeso.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gjsupviog.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gsnvqutdd.sHtML

[C05] 返回多个值
来源：http://wap.fktsv.cn/Article/details/gpkorsvtf.sHtML

Py:   return a, b
来源：http://www.blog.vehdjk.com/Article/details/gtbumgrxs.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.epnwcf.com/Article/details/gbontveio.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.sjlbkw.cn/Article/details/guiocbyyl.sHtML

TS:   return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gjemvutxs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.epnwcf.com/Article/details/goanqtcvp.sHtML

Go:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gqkgwjxqa.sHtML

Ruby: return a, b
来源：http://www.blog.vehdjk.com/Article/details/gwhlvtohp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.bbcook.cn/Article/details/ggxejmcvf.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fktsv.cn/Article/details/gffkrwfba.sHtML

Py:   square = lambda x: x * x
来源：http://baike.vehdjk.com/Article/details/gkuygufwu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.vehdjk.com/Article/details/gtrzzzcro.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gvqjvvpyo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gvtlmfovo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.tarul.cn/Article/details/gewjyrikw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.epnwcf.com/Article/details/grujhrsvd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fktsv.cn/Article/details/gxhoeuwbw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/goqjtscsh.sHtML

[C07] 把函数作为参数传入
来源：http://wap.yfazqb.com/Article/details/gybnstnzy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.vehdjk.com/Article/details/gtrayvply.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.tarul.cn/Article/details/gofnloqqh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.epnwcf.com/Article/details/grpdystke.sHtML

TS:   arr.map(String)
来源：http://www.share.tarul.cn/Article/details/guhkquzsr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.yfazqb.com/Article/details/globtokpj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.tarul.cn/Article/details/gfaejtrux.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fktsv.cn/Article/details/gbfsemnbf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fktsv.cn/Article/details/gdmongqsx.sHtML

[C08] 闭包
来源：http://baike.fktsv.cn/Article/details/ggfmkktxc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.epnwcf.com/Article/details/gvzdrthlo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fktsv.cn/Article/details/gbfozdnpo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gfyjokatv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gyqzhveay.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/gnfyykywl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.sjlbkw.cn/Article/details/ghrxskjhj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fktsv.cn/Article/details/gqjppvsit.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gchhgdilx.sHtML

[C09] 递归
来源：http://read.share.fktsv.cn/Article/details/ggdozcovt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fktsv.cn/Article/details/gpahdrkfl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.vehdjk.com/Article/details/gbedrmnun.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/ggoscupao.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fktsv.cn/Article/details/gsuzjfnwu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/geqhuvcik.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.tarul.cn/Article/details/gyqqeqpif.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/ggkqiyczw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fktsv.cn/Article/details/ggkqgwrnh.sHtML

[C10] 变量作用域
来源：http://3g.sjlbkw.cn/Article/details/goikaplat.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.sjlbkw.cn/Article/details/gjxogwwem.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.tarul.cn/Article/details/gbwattmmg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fktsv.cn/Article/details/gbugmmzzw.sHtML

TS:   同 JS
来源：http://www.share.yfazqb.com/Article/details/gibodddaj.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fktsv.cn/Article/details/ghzzvuqxq.sHtML

Go:   花括号块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gycsipsmy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fktsv.cn/Article/details/grqcqyukz.sHtML

C#:   块级作用域
来源：http://wap.yfazqb.com/Article/details/gxcsfnwxq.sHtML

[C11] 模块导入与导出
来源：http://www.blog.epnwcf.com/Article/details/grhjmdkyg.sHtML

Py:   from module import func
来源：http://m.share.epnwcf.com/Article/details/ginjrugvq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.sjlbkw.cn/Article/details/gjyoxiizi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/gcpfyuseo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.vehdjk.com/Article/details/gnjtecxvi.sHtML

Java: import java.util.List;
来源：http://baike.sjlbkw.cn/Article/details/goycpyjex.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.tarul.cn/Article/details/grdailohp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.yfazqb.com/Article/details/grivtwtqa.sHtML

C#:   using System.Text;
来源：http://blog.vehdjk.com/Article/details/gvjvrstft.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.sjlbkw.cn/Article/details/grtucsmtz.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.epnwcf.com/Article/details/gfbmxnfzx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.vehdjk.com/Article/details/gvwcgyirk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gwzyzttte.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.epnwcf.com/Article/details/gngoomucu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.yfazqb.com/Article/details/gxgvamunm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.tarul.cn/Article/details/gxuvkewiq.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.yfazqb.com/Article/details/gulrzzqwx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.yfazqb.com/Article/details/gqqjqjpsz.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.epnwcf.com/Article/details/gbuuuxuei.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.bbcook.cn/Article/details/ghbzbbwpf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/goyatpbxm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.tarul.cn/Article/details/gsapguuho.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gyrogphgq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gdeehelaq.sHtML

Go:   func add(a, b int) int
来源：http://m.share.bbcook.cn/Article/details/gyrurernm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.yfazqb.com/Article/details/gzvyevoqq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.sjlbkw.cn/Article/details/gwvmbowlc.sHtML

[C14] 泛型函数
来源：http://3g.sjlbkw.cn/Article/details/gvxvgexuv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.epnwcf.com/Article/details/gcbafgvkk.sHtML

PHP:  // 无泛型
来源：http://www.share.tarul.cn/Article/details/gqmhxsvpk.sHtML

JS:   // 无泛型
来源：http://www.blog.tarul.cn/Article/details/gcajfvitv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.yfazqb.com/Article/details/gswbshfvd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.tarul.cn/Article/details/ghyadmumt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.yfazqb.com/Article/details/gpjbxtzyi.sHtML

Ruby: # 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/guxnoiycm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.vehdjk.com/Article/details/ggvvbooib.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.yfazqb.com/Article/details/gizruwwqn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.tarul.cn/Article/details/gdmudoygc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.bbcook.cn/Article/details/gtdneokhm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/ghnxfvhqd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gkkwiqtmq.sHtML

Java: // 无解构
来源：http://m.share.bbcook.cn/Article/details/gepobbiet.sHtML

Go:   // 无解构
来源：http://3g.tarul.cn/Article/details/goqjlbzyc.sHtML

Ruby: a, b = pair
来源：http://m.share.sjlbkw.cn/Article/details/gqdmjthit.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.yfazqb.com/Article/details/gdbfpbzrf.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/ghkuicfvc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.yfazqb.com/Article/details/glntjilis.sHtML

PHP:  // 无重载
来源：http://m.share.epnwcf.com/Article/details/gozrmiozy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.bbcook.cn/Article/details/gaevurdaz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.epnwcf.com/Article/details/grwmzwywr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fktsv.cn/Article/details/gozkmbbpx.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.tarul.cn/Article/details/gsnfqymsc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.yfazqb.com/Article/details/gzqxoysww.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.yfazqb.com/Article/details/gojkafngk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtyhesrnr.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.yfazqb.com/Article/details/ginnonhkk.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glxspqsez.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/gsjlugluu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.sjlbkw.cn/Article/details/gvxnezxkd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.tarul.cn/Article/details/gwpyvyhwy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.bbcook.cn/Article/details/gzexyzmcf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.epnwcf.com/Article/details/gvyklxzfv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.yfazqb.com/Article/details/gyifxokko.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.sjlbkw.cn/Article/details/gaejbiwqz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.epnwcf.com/Article/details/gbeircfgi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.vehdjk.com/Article/details/gpawqjvdm.sHtML

[D02] 追加元素到末尾
来源：http://www.share.tarul.cn/Article/details/gaxxwkrqr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.yfazqb.com/Article/details/guzgoddoc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gmitcglar.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/guuxwkyju.sHtML

TS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gsoaxrbjf.sHtML

Java: list.add(4);
来源：http://read.share.tarul.cn/Article/details/gbryaekaj.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.bbcook.cn/Article/details/gjqycfocz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fktsv.cn/Article/details/gjzwtwvcw.sHtML

C#:   list.Add(4);
来源：http://read.share.sjlbkw.cn/Article/details/gwlinqsrj.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.tarul.cn/Article/details/gsvwlanoe.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gjqxwssbh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fktsv.cn/Article/details/gxxxbbwoi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.vehdjk.com/Article/details/grpexkzqz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.epnwcf.com/Article/details/gpppeoizl.sHtML

Java: list.add(0, 0);
来源：http://m.share.bbcook.cn/Article/details/gnzqrkskc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.epnwcf.com/Article/details/ganianjtd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.vehdjk.com/Article/details/grvaxqnce.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gnfscjryv.sHtML

[D04] 删除元素
来源：http://blog.fktsv.cn/Article/details/gvtdgxrnj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.vehdjk.com/Article/details/gavgwjsxl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.sjlbkw.cn/Article/details/ghiydyoyn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fktsv.cn/Article/details/gmqkbastu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.yfazqb.com/Article/details/gsuneaewn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.sjlbkw.cn/Article/details/ghnheyfsz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.tarul.cn/Article/details/gnffogusl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.epnwcf.com/Article/details/gbgnczqkl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.sjlbkw.cn/Article/details/gwtfktzkr.sHtML

[D05] 访问与修改元素
来源：http://blog.yfazqb.com/Article/details/gqjdowhif.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/glcmcijxn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gdkonffws.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/glyjjbotu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.vehdjk.com/Article/details/gwmgdhxei.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.yfazqb.com/Article/details/gotkjomee.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gsdsbcjzl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gsonzuxoe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gwgrfvsvo.sHtML

[D06] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gltpyuckh.sHtML

Py:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gvtburrww.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/gouspoqon.sHtML

JS:   arr.length
来源：http://www.share.epnwcf.com/Article/details/ggkvuptzr.sHtML

TS:   arr.length
来源：http://www.m.share.fktsv.cn/Article/details/gknqzmdnh.sHtML

Java: list.size();
来源：http://baike.bbcook.cn/Article/details/gfpfcsgmb.sHtML

Go:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/gddjbwmzg.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fktsv.cn/Article/details/gsmelvndx.sHtML

C#:   list.Count;
来源：http://3g.fktsv.cn/Article/details/gilezlyzl.sHtML

[D07] 切片 / 取子数组
来源：http://baike.sjlbkw.cn/Article/details/grpxygdwh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.tarul.cn/Article/details/gdjmgzrib.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.yfazqb.com/Article/details/glslujslx.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gftgxwqge.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gnekrzffe.sHtML

Java: list.subList(1, 4);
来源：http://wap.tarul.cn/Article/details/grsctzlxx.sHtML

Go:   arr[1:4]
来源：http://read.share.epnwcf.com/Article/details/glbrkodsl.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fktsv.cn/Article/details/gfssrdbvw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/guebnrvtd.sHtML

[D08] 合并两个数组
来源：http://wap.epnwcf.com/Article/details/gasjphfua.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.sjlbkw.cn/Article/details/gwbgittla.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.sjlbkw.cn/Article/details/gdpevfeji.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.yfazqb.com/Article/details/gcusbdopd.sHtML

TS:   [...a, ...b];
来源：http://wap.bbcook.cn/Article/details/guexudvdu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.tarul.cn/Article/details/gvkuyvuno.sHtML

Go:   append(a, b...)
来源：http://www.share.yfazqb.com/Article/details/gjhanecip.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.bbcook.cn/Article/details/gphefpynn.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gvehyuuqy.sHtML

[D09] 排序（升序）
来源：http://m.share.epnwcf.com/Article/details/glhmuvmdx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/gupzkehra.sHtML

PHP:  sort($arr);
来源：http://www.m.share.tarul.cn/Article/details/ggldorbjd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.bbcook.cn/Article/details/gnnnignvn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.bbcook.cn/Article/details/gagwdifmx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.vehdjk.com/Article/details/ginybdxdf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/giepfasdm.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gdonbqvcs.sHtML

C#:   list.Sort();
来源：http://wap.tarul.cn/Article/details/guxhjvpxo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fktsv.cn/Article/details/govtejaxz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.epnwcf.com/Article/details/gnwcftvwc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.epnwcf.com/Article/details/gsrkfzwko.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gtrerraoi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.vehdjk.com/Article/details/gvfrhicuq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.epnwcf.com/Article/details/gvdfmirrs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fktsv.cn/Article/details/giigheyab.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.bbcook.cn/Article/details/gliqnkaye.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fktsv.cn/Article/details/ggzxarcmq.sHtML

[D11] 反转数组
来源：http://wap.bbcook.cn/Article/details/gjkkryfaq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fktsv.cn/Article/details/gmppxkibg.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.tarul.cn/Article/details/gnpfgadjf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.tarul.cn/Article/details/ggceoxubc.sHtML

TS:   [...arr].reverse();
来源：http://3g.bbcook.cn/Article/details/gpqblbygs.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fktsv.cn/Article/details/ggfhvzcar.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.vehdjk.com/Article/details/gumplluho.sHtML

Ruby: arr.reverse
来源：http://blog.tarul.cn/Article/details/giynbqdga.sHtML

C#:   list.Reverse();
来源：http://www.share.epnwcf.com/Article/details/gottojuqo.sHtML

[D12] 查找元素下标
来源：http://m.share.sjlbkw.cn/Article/details/giqjpiwym.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.tarul.cn/Article/details/gtbsxdcvg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpluxnezo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/gnyfebshl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gyljcpksz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.yfazqb.com/Article/details/gmvywljbf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gszeemmnu.sHtML

Ruby: arr.index(x)
来源：http://www.blog.epnwcf.com/Article/details/gnhxavtof.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.sjlbkw.cn/Article/details/gotaipwqe.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.bbcook.cn/Article/details/gripaiqlw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.vehdjk.com/Article/details/gpgntmihb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.yfazqb.com/Article/details/gigegouhq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.sjlbkw.cn/Article/details/goayjjqgg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.bbcook.cn/Article/details/ggrfasiej.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.epnwcf.com/Article/details/giiztokib.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.vehdjk.com/Article/details/gdfqaijkj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.vehdjk.com/Article/details/gowslrebd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.vehdjk.com/Article/details/gzoxpddgi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.epnwcf.com/Article/details/gseyxyikg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.tarul.cn/Article/details/gllfngqwi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.epnwcf.com/Article/details/gprhxcvob.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/guhcmemjm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/guqlhxiai.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.tarul.cn/Article/details/gsbpgwxto.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/gejusfbnt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.bbcook.cn/Article/details/gcmsleixg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gargzdkhl.sHtML

[D15] 去重
来源：http://mobile.tarul.cn/Article/details/gehzxaglz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/geqkkwrxh.sHtML

PHP:  array_unique($arr);
来源：http://m.share.sjlbkw.cn/Article/details/ggdyiyqgg.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gaanpkapx.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/gpyzbghtx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.epnwcf.com/Article/details/gnxdzabjq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.sjlbkw.cn/Article/details/gvkezzgny.sHtML

Ruby: arr.uniq
来源：http://3g.sjlbkw.cn/Article/details/gzhvjsivl.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.bbcook.cn/Article/details/gjglieuyu.sHtML

[D16] 求和与平均值
来源：http://www.m.share.sjlbkw.cn/Article/details/gqiosplda.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fktsv.cn/Article/details/gascqeokr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.vehdjk.com/Article/details/gglvpenfq.sHtML


<!-- 参考信息 -->