代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gnioruboe.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/gtjbntvxd.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fktsv.cn/Article/details/gldnovqum.sHtML

Py:   a and b or not c
来源：http://wap.epnwcf.com/Article/details/gsighccay.sHtML

PHP:  $a && $b || !$c
来源：http://blog.yfazqb.com/Article/details/gddatqqph.sHtML

JS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gbqbojbki.sHtML

TS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/ghdftgyhs.sHtML

Java: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gjoobcywg.sHtML

Go:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gfvrbdapa.sHtML

Ruby: a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gccteogrd.sHtML

C#:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/girncsxts.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.bbcook.cn/Article/details/gxfqhbyfy.sHtML

Py:   if not data: return
来源：http://3g.bbcook.cn/Article/details/gsgvtjfbz.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.vehdjk.com/Article/details/ggwpbiryg.sHtML

JS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/gjniplgdq.sHtML

TS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/gpcqhtabf.sHtML

Java: if (data == null) return;
来源：http://mobile.epnwcf.com/Article/details/gdnqambfo.sHtML

Go:   if data == nil { return }
来源：http://wap.bbcook.cn/Article/details/gfhkmznsf.sHtML

Ruby: return if data.nil?
来源：http://www.blog.bbcook.cn/Article/details/giawgsedk.sHtML

C#:   if (data == null) return;
来源：http://www.share.tarul.cn/Article/details/ggsfbdgpf.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtivhrczy.sHtML

C. 函数与作用域
来源：http://www.share.sjlbkw.cn/Article/details/geuihtpqd.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfmhftzjj.sHtML

[C01] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/gdicsuzas.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.vehdjk.com/Article/details/gmxpivaii.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gnxdxblrx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gpfvwvstl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gzglfaunk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gowmfekdw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gcemaoohd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.bbcook.cn/Article/details/gvmublbvw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gxsceudps.sHtML

[C02] 默认参数
来源：http://www.share.bbcook.cn/Article/details/gekqoelsk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.yfazqb.com/Article/details/gnljyipxt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fktsv.cn/Article/details/gfgjewacr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gbiihtbii.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/gljflcmip.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.epnwcf.com/Article/details/gzhglcvjo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fktsv.cn/Article/details/gyzqjsopc.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.yfazqb.com/Article/details/gdnaygyqm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.vehdjk.com/Article/details/gdpzclwog.sHtML

[C03] 可变参数
来源：http://read.share.yfazqb.com/Article/details/gapmkidhz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fktsv.cn/Article/details/gavivfgce.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.vehdjk.com/Article/details/gmnfwdarx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.sjlbkw.cn/Article/details/gpzyshdzh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/gejgpolqs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.tarul.cn/Article/details/gfvslpczd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.epnwcf.com/Article/details/gwosuqskf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.bbcook.cn/Article/details/gglqpurqd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.epnwcf.com/Article/details/gxeogkino.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.vehdjk.com/Article/details/gqiagatev.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.epnwcf.com/Article/details/gmfsdqjbi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.tarul.cn/Article/details/gfwlnyjew.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.vehdjk.com/Article/details/gtmxbdase.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.bbcook.cn/Article/details/gunqeecfs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fktsv.cn/Article/details/gfaamuqiz.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.sjlbkw.cn/Article/details/gqkqqajxf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gadircnuw.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gpmwuanvb.sHtML

[C05] 返回多个值
来源：http://3g.vehdjk.com/Article/details/grdzjiuhv.sHtML

Py:   return a, b
来源：http://baike.epnwcf.com/Article/details/gdxgixvnv.sHtML

PHP:  return [$a, $b];
来源：http://www.share.tarul.cn/Article/details/gepvmnlmi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fktsv.cn/Article/details/gkkkvtyti.sHtML

TS:   return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/glgmafhcz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.bbcook.cn/Article/details/geipwdrnk.sHtML

Go:   return a, b
来源：http://read.share.bbcook.cn/Article/details/ghlgecher.sHtML

Ruby: return a, b
来源：http://www.share.sjlbkw.cn/Article/details/gsbvhciij.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.tarul.cn/Article/details/gywgukpjh.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.vehdjk.com/Article/details/gindjfolg.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.bbcook.cn/Article/details/gwcxxllsd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.sjlbkw.cn/Article/details/gyuyltqoh.sHtML

JS:   const square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gbhftjwrs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.tarul.cn/Article/details/gmkzsmcyr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.bbcook.cn/Article/details/gjqsnnhdz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.epnwcf.com/Article/details/gxxophssk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.epnwcf.com/Article/details/gtdtyujbo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/ghbsxwqkm.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.yfazqb.com/Article/details/gjdpwsmxj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.tarul.cn/Article/details/gdbqulvvi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gdixhslrt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.sjlbkw.cn/Article/details/givdywkmc.sHtML

TS:   arr.map(String)
来源：http://wap.fktsv.cn/Article/details/gkuqzuhnj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.vehdjk.com/Article/details/gvbacucmb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.sjlbkw.cn/Article/details/geqavjpwq.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.tarul.cn/Article/details/gvhrdsmqf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.bbcook.cn/Article/details/gbzsaksrw.sHtML

[C08] 闭包
来源：http://3g.fktsv.cn/Article/details/gcpdjgelb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.tarul.cn/Article/details/giqfncpuh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.tarul.cn/Article/details/gflnfvllx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gsjhyogyj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gclrelzhp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.epnwcf.com/Article/details/gpinmxnou.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.tarul.cn/Article/details/gvifgsbak.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.sjlbkw.cn/Article/details/gpxdvfymi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gmxvnsrsr.sHtML

[C09] 递归
来源：http://wap.vehdjk.com/Article/details/ggrkhmepk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/gojdzmper.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.vehdjk.com/Article/details/guwerkuws.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/glsccetpd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gaxpkeuld.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.yfazqb.com/Article/details/gcmczxywz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.yfazqb.com/Article/details/gymdavvth.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.epnwcf.com/Article/details/gbyybmxiy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.tarul.cn/Article/details/gcbsrabad.sHtML

[C10] 变量作用域
来源：http://3g.fktsv.cn/Article/details/gttxnbkfp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.vehdjk.com/Article/details/gaalnmrgc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.sjlbkw.cn/Article/details/genosubvo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.epnwcf.com/Article/details/gwxzguown.sHtML

TS:   同 JS
来源：http://blog.fktsv.cn/Article/details/gqwcpfhns.sHtML

Java: 方法内为块级作用域
来源：http://wap.tarul.cn/Article/details/gsbfwzmld.sHtML

Go:   花括号块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/ghhjlcexo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fktsv.cn/Article/details/gsrraksyo.sHtML

C#:   块级作用域
来源：http://www.share.tarul.cn/Article/details/goabtwdpx.sHtML

[C11] 模块导入与导出
来源：http://www.share.sjlbkw.cn/Article/details/gdxrnwzkx.sHtML

Py:   from module import func
来源：http://read.share.epnwcf.com/Article/details/gijhfrzsf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.vehdjk.com/Article/details/gxaaosefc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.sjlbkw.cn/Article/details/gswapnwgc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.tarul.cn/Article/details/glzhgrwfp.sHtML

Java: import java.util.List;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkfejdbz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.epnwcf.com/Article/details/gfiwnwyst.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.epnwcf.com/Article/details/gzsvylzcx.sHtML

C#:   using System.Text;
来源：http://read.share.epnwcf.com/Article/details/gmdxuzjwk.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.sjlbkw.cn/Article/details/gzxbapjbe.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.epnwcf.com/Article/details/gonpydlan.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.vehdjk.com/Article/details/gqnzxbyct.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fktsv.cn/Article/details/gqlnsxref.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gerckqykl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.sjlbkw.cn/Article/details/guniefrvr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.sjlbkw.cn/Article/details/gehxpzpqc.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.epnwcf.com/Article/details/golbqgloq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fktsv.cn/Article/details/gkgzadgxd.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.tarul.cn/Article/details/gjfsrwcmd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.yfazqb.com/Article/details/gjyqjchig.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/glngeqoys.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.bbcook.cn/Article/details/giplaiqfx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gzaotmuda.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/grrycwoie.sHtML

Go:   func add(a, b int) int
来源：http://baike.tarul.cn/Article/details/ghhtaqhpq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.yfazqb.com/Article/details/gnpwjqzvy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.yfazqb.com/Article/details/gbxfumfnm.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/gmzqgfiya.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.tarul.cn/Article/details/goxbpgpib.sHtML

PHP:  // 无泛型
来源：http://read.share.yfazqb.com/Article/details/gbxcvdhav.sHtML

JS:   // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gohoinuth.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.yfazqb.com/Article/details/gplnkylxn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.bbcook.cn/Article/details/grfdpdvst.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fktsv.cn/Article/details/gliqwunpj.sHtML

Ruby: # 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gtcyfrsye.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.yfazqb.com/Article/details/gzltbkulc.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.tarul.cn/Article/details/gsvszcuwq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/gjwikbchq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.sjlbkw.cn/Article/details/gszmzcksp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gayjwaftr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.tarul.cn/Article/details/gpnsrsnur.sHtML

Java: // 无解构
来源：http://m.share.fktsv.cn/Article/details/gftvwpvhd.sHtML

Go:   // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/gyznoobrb.sHtML

Ruby: a, b = pair
来源：http://baike.vehdjk.com/Article/details/gkcudmgny.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.epnwcf.com/Article/details/gitggmtjy.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.epnwcf.com/Article/details/gttdwspls.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.tarul.cn/Article/details/gxvxjofoy.sHtML

PHP:  // 无重载
来源：http://baike.epnwcf.com/Article/details/grdohktzc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.bbcook.cn/Article/details/gjndqtltf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.epnwcf.com/Article/details/gfnfivzur.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.vehdjk.com/Article/details/gpmgvgwec.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.yfazqb.com/Article/details/ggbmrbdcj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.yfazqb.com/Article/details/gqaziqtfe.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.epnwcf.com/Article/details/gchizwcxv.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/guhiayxeg.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fktsv.cn/Article/details/gxlexxgds.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gixjqblif.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.sjlbkw.cn/Article/details/gwjdnqgig.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.sjlbkw.cn/Article/details/gqghllpbs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.sjlbkw.cn/Article/details/gcplloine.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.vehdjk.com/Article/details/gpdjthnnt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.epnwcf.com/Article/details/gfbejbudv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.epnwcf.com/Article/details/gcswuslmm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.bbcook.cn/Article/details/gfvqzqmjt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.bbcook.cn/Article/details/gozmxrbks.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.tarul.cn/Article/details/gbslzegxd.sHtML

[D02] 追加元素到末尾
来源：http://mobile.sjlbkw.cn/Article/details/gacpvtnfl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fktsv.cn/Article/details/ghfghklpt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.epnwcf.com/Article/details/guiuerbii.sHtML

JS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/ganmldzuh.sHtML

TS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/gdsoozfjr.sHtML

Java: list.add(4);
来源：http://3g.sjlbkw.cn/Article/details/gxpbfkqyf.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.epnwcf.com/Article/details/gvkcruded.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.tarul.cn/Article/details/gdxlavysm.sHtML

C#:   list.Add(4);
来源：http://mobile.epnwcf.com/Article/details/ggjtkfice.sHtML

[D03] 在指定位置插入元素
来源：http://wap.sjlbkw.cn/Article/details/gqvrgailg.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.yfazqb.com/Article/details/gttrvatav.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fktsv.cn/Article/details/gvbhvadab.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.sjlbkw.cn/Article/details/gqzjkexiq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.bbcook.cn/Article/details/gcdehflzi.sHtML

Java: list.add(0, 0);
来源：http://wap.vehdjk.com/Article/details/gynlyziyx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.tarul.cn/Article/details/gnucwnnwq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.sjlbkw.cn/Article/details/gcsyktrdk.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.epnwcf.com/Article/details/gpzchmwjx.sHtML

[D04] 删除元素
来源：http://m.share.vehdjk.com/Article/details/gycxsxzdw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.yfazqb.com/Article/details/ghwcudnlr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdczsmvsk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.vehdjk.com/Article/details/gphyziave.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gxuumrorx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.vehdjk.com/Article/details/gphvdrxiv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.epnwcf.com/Article/details/gbnaccmfw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.epnwcf.com/Article/details/ghvqcqpwr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.sjlbkw.cn/Article/details/gzkadeidh.sHtML

[D05] 访问与修改元素
来源：http://mobile.epnwcf.com/Article/details/grmvvgnwm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gomxfktbi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gqsllxnwm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/gvtchstld.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.tarul.cn/Article/details/gazhhjtep.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.vehdjk.com/Article/details/gudpngwep.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/ggrksgsid.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gmiyqduwr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.epnwcf.com/Article/details/gwhdxpnnz.sHtML

[D06] 数组长度
来源：http://www.blog.fktsv.cn/Article/details/gtuhlvssi.sHtML

Py:   len(arr)
来源：http://wap.bbcook.cn/Article/details/guygurwlg.sHtML

PHP:  count($arr);
来源：http://read.share.yfazqb.com/Article/details/gxfrvjbrw.sHtML

JS:   arr.length
来源：http://blog.epnwcf.com/Article/details/gvfpuaupj.sHtML

TS:   arr.length
来源：http://mobile.fktsv.cn/Article/details/gafldhjtf.sHtML

Java: list.size();
来源：http://3g.fktsv.cn/Article/details/gyatkwcdj.sHtML

Go:   len(arr)
来源：http://m.share.yfazqb.com/Article/details/gurxdsjem.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fktsv.cn/Article/details/gqibxmbpz.sHtML

C#:   list.Count;
来源：http://www.blog.sjlbkw.cn/Article/details/gbvvhgfza.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fktsv.cn/Article/details/gfpazswhz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.epnwcf.com/Article/details/gzlyqjcoh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.tarul.cn/Article/details/gxkvaelcg.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gspwiqtlk.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gnouwjmmr.sHtML

Java: list.subList(1, 4);
来源：http://m.share.tarul.cn/Article/details/grchrmyem.sHtML

Go:   arr[1:4]
来源：http://m.share.tarul.cn/Article/details/guneinnag.sHtML

Ruby: arr[1, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gaimheifq.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.vehdjk.com/Article/details/grpwsyhzx.sHtML

[D08] 合并两个数组
来源：http://www.blog.epnwcf.com/Article/details/gqaytztqh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.bbcook.cn/Article/details/gicdsycxe.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.tarul.cn/Article/details/gwpdwfpmp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.epnwcf.com/Article/details/gebikexcw.sHtML

TS:   [...a, ...b];
来源：http://m.share.fktsv.cn/Article/details/gphrwsojm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.yfazqb.com/Article/details/gopmfpexk.sHtML

Go:   append(a, b...)
来源：http://blog.sjlbkw.cn/Article/details/gnhzkcwcq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.epnwcf.com/Article/details/gwbrcfoew.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gahvbyume.sHtML

[D09] 排序（升序）
来源：http://www.share.sjlbkw.cn/Article/details/gmkqyuvon.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/ghryupkki.sHtML

PHP:  sort($arr);
来源：http://wap.tarul.cn/Article/details/gljlqrngo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.vehdjk.com/Article/details/gxaplravs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fktsv.cn/Article/details/gywcuyvcv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.vehdjk.com/Article/details/gdqeyoofd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/gdpfnzyjr.sHtML

Ruby: arr.sort
来源：http://www.share.bbcook.cn/Article/details/gfftrjgat.sHtML

C#:   list.Sort();
来源：http://m.share.fktsv.cn/Article/details/gwotftjim.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.tarul.cn/Article/details/gjcmvulqc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.sjlbkw.cn/Article/details/gotwefzwq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/gbklpwlxu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/gskeooisq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/gynllnfda.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.vehdjk.com/Article/details/gmjorgxci.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.vehdjk.com/Article/details/gaillgppn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.sjlbkw.cn/Article/details/gjlihtvey.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.vehdjk.com/Article/details/gmzneqfck.sHtML

[D11] 反转数组
来源：http://wap.fktsv.cn/Article/details/gonoohjss.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.bbcook.cn/Article/details/ghqiehtep.sHtML

PHP:  array_reverse($arr);
来源：http://baike.epnwcf.com/Article/details/gewawkpgh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.yfazqb.com/Article/details/gslwiexpe.sHtML

TS:   [...arr].reverse();
来源：http://www.share.yfazqb.com/Article/details/gdukdtpjj.sHtML

Java: Collections.reverse(list);
来源：http://mobile.bbcook.cn/Article/details/grzpbakje.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.sjlbkw.cn/Article/details/grnaccnaz.sHtML

Ruby: arr.reverse
来源：http://mobile.tarul.cn/Article/details/gqavmvuej.sHtML

C#:   list.Reverse();
来源：http://read.share.epnwcf.com/Article/details/girvdhzon.sHtML

[D12] 查找元素下标
来源：http://read.share.yfazqb.com/Article/details/gtaqgdmol.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.bbcook.cn/Article/details/gtsqlzjor.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.yfazqb.com/Article/details/goqteyjhb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.epnwcf.com/Article/details/gokobpcud.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.yfazqb.com/Article/details/gxzczwuld.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.sjlbkw.cn/Article/details/gckvyskhe.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.bbcook.cn/Article/details/guzsbbyup.sHtML

Ruby: arr.index(x)
来源：http://www.blog.vehdjk.com/Article/details/ghrbooqdr.sHtML

C#:   list.IndexOf(x);
来源：http://blog.tarul.cn/Article/details/gsbdbwyyw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.epnwcf.com/Article/details/gmzdkoteq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.yfazqb.com/Article/details/gvohfiadq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fktsv.cn/Article/details/gimrqytwh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.epnwcf.com/Article/details/gurzifbqc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.sjlbkw.cn/Article/details/gcpryjame.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.vehdjk.com/Article/details/gcjgqcujo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.tarul.cn/Article/details/gfdsiosoe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fktsv.cn/Article/details/gcafqrceq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.vehdjk.com/Article/details/ggvbchcvj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.bbcook.cn/Article/details/gjdgjsasn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.bbcook.cn/Article/details/giujwmhlu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.sjlbkw.cn/Article/details/gbellymqa.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/gpmmynuhk.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.epnwcf.com/Article/details/gwtclyqzp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gumuxhnna.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/gfadbsqqd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gffnihout.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.bbcook.cn/Article/details/gknpxodfq.sHtML

[D15] 去重
来源：http://baike.yfazqb.com/Article/details/glbviypbh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/ghiszabaf.sHtML

PHP:  array_unique($arr);
来源：http://3g.sjlbkw.cn/Article/details/gxfgqlvga.sHtML

JS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/gusakhubn.sHtML


<!-- 参考信息 -->