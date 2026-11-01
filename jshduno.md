代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.sjlbkw.cn/Article/details/glddokbzs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.sjlbkw.cn/Article/details/gzoahpinz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gcztinlzf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gurvqrone.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gutdkhnlj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.vehdjk.com/Article/details/gfeouzaek.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.yfazqb.com/Article/details/gkkyiapch.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.vehdjk.com/Article/details/gqbtroxki.sHtML

[B13] 判断是否为数字
来源：http://wap.bbcook.cn/Article/details/gbqhhouia.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.bbcook.cn/Article/details/gimvljpzv.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/gzdqnazxz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.sjlbkw.cn/Article/details/gtzbjwdam.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.epnwcf.com/Article/details/gdcheyecp.sHtML

Java: x instanceof Number
来源：http://m.share.fktsv.cn/Article/details/geibyfsiu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.yfazqb.com/Article/details/gpuykdypn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.yfazqb.com/Article/details/gtnjaiops.sHtML

C#:   x is int or double or decimal
来源：http://www.share.sjlbkw.cn/Article/details/glrmlmwrt.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.vehdjk.com/Article/details/gtcukjouk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.sjlbkw.cn/Article/details/gunquznxy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.sjlbkw.cn/Article/details/golypzgee.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gdpbgzvrk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fktsv.cn/Article/details/gwjobbeoi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.tarul.cn/Article/details/gqdjdxyep.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gcqjxmtyr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fktsv.cn/Article/details/gomjwdyjk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gxysboixx.sHtML

[B15] 布尔运算与取反
来源：http://wap.vehdjk.com/Article/details/gqpiexcvv.sHtML

Py:   a and b or not c
来源：http://www.share.tarul.cn/Article/details/gfyjlnzau.sHtML

PHP:  $a && $b || !$c
来源：http://wap.epnwcf.com/Article/details/gporkodew.sHtML

JS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gnvtmmgkv.sHtML

TS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gbufqloxf.sHtML

Java: a && b || !c
来源：http://m.share.tarul.cn/Article/details/gwaqpjnpm.sHtML

Go:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gdesciguf.sHtML

Ruby: a && b || !c
来源：http://m.share.tarul.cn/Article/details/glqeudfhs.sHtML

C#:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gelksallk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.vehdjk.com/Article/details/gwfzxktof.sHtML

Py:   if not data: return
来源：http://mobile.yfazqb.com/Article/details/gvzyshhlh.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.sjlbkw.cn/Article/details/gzsuyzkgy.sHtML

JS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/gxcruilhh.sHtML

TS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/ggletaarv.sHtML

Java: if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/gdswgoocw.sHtML

Go:   if data == nil { return }
来源：http://www.share.bbcook.cn/Article/details/gveitluau.sHtML

Ruby: return if data.nil?
来源：http://mobile.vehdjk.com/Article/details/gsthslsuy.sHtML

C#:   if (data == null) return;
来源：http://read.share.fktsv.cn/Article/details/gbevkzqeg.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gqfpvkcni.sHtML

C. 函数与作用域
来源：http://www.share.fktsv.cn/Article/details/gvgmolpxm.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqsqzsxhm.sHtML

[C01] 定义函数
来源：http://m.share.vehdjk.com/Article/details/gtkuxxxhl.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/gmyvljule.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/grijrnawu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/giuuhsrco.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gnqtedkpq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gljigwlmk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.epnwcf.com/Article/details/guvjsbsex.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.vehdjk.com/Article/details/gecfekzyg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gpqftlemo.sHtML

[C02] 默认参数
来源：http://www.share.epnwcf.com/Article/details/gqofdysff.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.sjlbkw.cn/Article/details/gtodrksmr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.sjlbkw.cn/Article/details/gkofkfbun.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/gakowihvn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gbltaxmsu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.bbcook.cn/Article/details/gwzzdfcjl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.sjlbkw.cn/Article/details/gbnwfnxen.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.sjlbkw.cn/Article/details/gptehlisu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/gqelvovxm.sHtML

[C03] 可变参数
来源：http://www.blog.tarul.cn/Article/details/gzmxysran.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.yfazqb.com/Article/details/gqgbvbvgz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.yfazqb.com/Article/details/gwywpfxqg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/glhqjgqyj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/gwvogdaxm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fktsv.cn/Article/details/gidnpecvs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.tarul.cn/Article/details/gvpqodqgv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.tarul.cn/Article/details/gtgjswowr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.vehdjk.com/Article/details/gaomdootd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.tarul.cn/Article/details/gjyguthpg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.sjlbkw.cn/Article/details/gqzvxyuug.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.tarul.cn/Article/details/gpwuynnij.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/glxcymfww.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.vehdjk.com/Article/details/gvajhuqcy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.vehdjk.com/Article/details/gkplphaze.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.tarul.cn/Article/details/gqotgeuxq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/gngxeufoc.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gmfdflqlb.sHtML

[C05] 返回多个值
来源：http://read.share.bbcook.cn/Article/details/gfldktsln.sHtML

Py:   return a, b
来源：http://blog.tarul.cn/Article/details/ggyqhyfnl.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.yfazqb.com/Article/details/gbinenaab.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.tarul.cn/Article/details/gkehcnpbm.sHtML

TS:   return { a, b };
来源：http://www.share.vehdjk.com/Article/details/gpxdtycqr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.sjlbkw.cn/Article/details/gbazmzgss.sHtML

Go:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gkgiygeoa.sHtML

Ruby: return a, b
来源：http://3g.bbcook.cn/Article/details/gsnjvvigi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.vehdjk.com/Article/details/guamjxbyp.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fktsv.cn/Article/details/gsahfvvig.sHtML

Py:   square = lambda x: x * x
来源：http://3g.bbcook.cn/Article/details/ghabjxhex.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.vehdjk.com/Article/details/gqeptjjps.sHtML

JS:   const square = x => x * x;
来源：http://wap.epnwcf.com/Article/details/gmqbqcamv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.epnwcf.com/Article/details/gdmrakphe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/gbnscwcyn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.tarul.cn/Article/details/gecskvpyo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmwdcoed.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/gbwwjyypm.sHtML

[C07] 把函数作为参数传入
来源：http://wap.vehdjk.com/Article/details/ggwnxhqmg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.bbcook.cn/Article/details/gegtbkere.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.tarul.cn/Article/details/grilmdvws.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fktsv.cn/Article/details/gtdebezwa.sHtML

TS:   arr.map(String)
来源：http://blog.sjlbkw.cn/Article/details/ghdzmrowy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.vehdjk.com/Article/details/gawcrjdeo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fktsv.cn/Article/details/giwaivjfa.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.yfazqb.com/Article/details/guuiawhce.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.vehdjk.com/Article/details/gpwmxqnuy.sHtML

[C08] 闭包
来源：http://read.share.bbcook.cn/Article/details/gkdrvfppw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.tarul.cn/Article/details/gkdwzjtwn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.yfazqb.com/Article/details/gfzhgocbe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/glslyjofs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gcitukduk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.tarul.cn/Article/details/gjvhxprkb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.tarul.cn/Article/details/gsjfpozbe.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.yfazqb.com/Article/details/gtzducxyo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gmuaixgdw.sHtML

[C09] 递归
来源：http://blog.vehdjk.com/Article/details/gtgogzfxr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.bbcook.cn/Article/details/gydfiywme.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.epnwcf.com/Article/details/gdzykgbmi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.tarul.cn/Article/details/goowrbdll.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/gwsurytyc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.epnwcf.com/Article/details/gngwrwtbg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fktsv.cn/Article/details/gxxidyuhu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/goneoifoi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fktsv.cn/Article/details/grnqdckre.sHtML

[C10] 变量作用域
来源：http://read.share.vehdjk.com/Article/details/gqrbbcniy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.yfazqb.com/Article/details/gswkqnaro.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.epnwcf.com/Article/details/gnldvqgvc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.yfazqb.com/Article/details/gjliqxrba.sHtML

TS:   同 JS
来源：http://read.share.bbcook.cn/Article/details/gqzywejfc.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.tarul.cn/Article/details/gpslkhfke.sHtML

Go:   花括号块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gxxklozii.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.sjlbkw.cn/Article/details/gmobdffss.sHtML

C#:   块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gdyluhvti.sHtML

[C11] 模块导入与导出
来源：http://m.share.fktsv.cn/Article/details/gwakgrptt.sHtML

Py:   from module import func
来源：http://www.share.yfazqb.com/Article/details/gvruuxwcq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fktsv.cn/Article/details/gunyxmdoz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.tarul.cn/Article/details/gwwhhogki.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.yfazqb.com/Article/details/guehaghuh.sHtML

Java: import java.util.List;
来源：http://m.share.epnwcf.com/Article/details/gbmvcfvub.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.sjlbkw.cn/Article/details/ghoururrd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.sjlbkw.cn/Article/details/gpglsbhud.sHtML

C#:   using System.Text;
来源：http://www.blog.yfazqb.com/Article/details/gaajwtgwy.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.yfazqb.com/Article/details/gggeqzdtx.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.bbcook.cn/Article/details/giwggainm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.yfazqb.com/Article/details/gucllxaes.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/gwonxsrep.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fktsv.cn/Article/details/guasreoec.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.epnwcf.com/Article/details/gfwzajxzw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fktsv.cn/Article/details/gxruldytd.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.vehdjk.com/Article/details/gffrcmejb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fktsv.cn/Article/details/gyxegotaa.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.yfazqb.com/Article/details/gvrcwwdyn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fktsv.cn/Article/details/gosomjtya.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gvmxwciwp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.bbcook.cn/Article/details/gaunkzgys.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/geuuypmqa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gvplxtsos.sHtML

Go:   func add(a, b int) int
来源：http://wap.sjlbkw.cn/Article/details/gjehrxljl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.epnwcf.com/Article/details/gmcqcxdmx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.bbcook.cn/Article/details/gbmfktrtz.sHtML

[C14] 泛型函数
来源：http://www.share.sjlbkw.cn/Article/details/gnccdqqdw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.epnwcf.com/Article/details/ggvcxorco.sHtML

PHP:  // 无泛型
来源：http://blog.yfazqb.com/Article/details/grmnhfpiq.sHtML

JS:   // 无泛型
来源：http://read.share.yfazqb.com/Article/details/gjhfewjdh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.bbcook.cn/Article/details/gafvcbezj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.bbcook.cn/Article/details/gewdiavkc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.sjlbkw.cn/Article/details/gckhquikv.sHtML

Ruby: # 无泛型
来源：http://3g.vehdjk.com/Article/details/gebdsnupv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.bbcook.cn/Article/details/gdnpxrobm.sHtML

[C15] 解构 / 展开参数
来源：http://blog.yfazqb.com/Article/details/gvmbibevw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.yfazqb.com/Article/details/gjanfcfze.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.yfazqb.com/Article/details/gtkbloqdw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gqbkehvec.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.yfazqb.com/Article/details/gumnrjlai.sHtML

Java: // 无解构
来源：http://3g.vehdjk.com/Article/details/gvtsdwgqt.sHtML

Go:   // 无解构
来源：http://read.share.vehdjk.com/Article/details/gpkpwhspd.sHtML

Ruby: a, b = pair
来源：http://www.m.share.yfazqb.com/Article/details/glhfdhadi.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.bbcook.cn/Article/details/gvardzgnt.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.vehdjk.com/Article/details/gvkyiuouz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.epnwcf.com/Article/details/gchamzjae.sHtML

PHP:  // 无重载
来源：http://read.share.sjlbkw.cn/Article/details/gedrpjwmb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.epnwcf.com/Article/details/gnyludyqi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/gaugaeezg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.bbcook.cn/Article/details/gpnvtnbvu.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/gbywjvfju.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.bbcook.cn/Article/details/goelnlhtx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.tarul.cn/Article/details/ggnuvgivn.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxvnknnth.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.yfazqb.com/Article/details/gaetqtadv.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gyfqurrgy.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fktsv.cn/Article/details/gqwgtprno.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.bbcook.cn/Article/details/giebighae.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fktsv.cn/Article/details/ghvwdbqct.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fktsv.cn/Article/details/gtlmaucvl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.epnwcf.com/Article/details/gdcskqigi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fktsv.cn/Article/details/gjjubelcw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.bbcook.cn/Article/details/gemmiqayh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.tarul.cn/Article/details/glsxhjrcl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.tarul.cn/Article/details/gyjqctpma.sHtML

[D02] 追加元素到末尾
来源：http://baike.epnwcf.com/Article/details/gedvearzk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fktsv.cn/Article/details/gomucspxk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.vehdjk.com/Article/details/guknomrkx.sHtML

JS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/gtjicyexh.sHtML

TS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/gcyzcqigb.sHtML

Java: list.add(4);
来源：http://www.blog.fktsv.cn/Article/details/glztaltep.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.yfazqb.com/Article/details/giqjeftfe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.sjlbkw.cn/Article/details/gosgxprth.sHtML

C#:   list.Add(4);
来源：http://www.blog.bbcook.cn/Article/details/gqyfngkwf.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.sjlbkw.cn/Article/details/gdmdujztt.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gdntiwhit.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fktsv.cn/Article/details/glnzqptyb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.vehdjk.com/Article/details/ggoasilkl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/goqyluqkp.sHtML

Java: list.add(0, 0);
来源：http://3g.bbcook.cn/Article/details/gjwrzbfyo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.tarul.cn/Article/details/gvxwchztd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fktsv.cn/Article/details/ghgfwzwal.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.yfazqb.com/Article/details/grxwivqmy.sHtML

[D04] 删除元素
来源：http://baike.sjlbkw.cn/Article/details/gfxxwaasw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.tarul.cn/Article/details/gehrbomnc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gvxvqcvrq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.tarul.cn/Article/details/gwhbhwabc.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.epnwcf.com/Article/details/gzwjanyxm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.bbcook.cn/Article/details/grpfdqopm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.tarul.cn/Article/details/gnxlxhzjk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.sjlbkw.cn/Article/details/gnydiqije.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.tarul.cn/Article/details/gughhweyr.sHtML

[D05] 访问与修改元素
来源：http://mobile.vehdjk.com/Article/details/gvzysrwfn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gsrpnrnye.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gxpwdfnou.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.epnwcf.com/Article/details/gqykghypl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.epnwcf.com/Article/details/gizyhabru.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.sjlbkw.cn/Article/details/gfasgpcug.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gusrazmpd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/glsfqldqh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gwqqosnte.sHtML

[D06] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gsuydjrmf.sHtML

Py:   len(arr)
来源：http://3g.tarul.cn/Article/details/geukrzdyq.sHtML

PHP:  count($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gcndbqzbe.sHtML

JS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/gedweutxz.sHtML

TS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/ggztyhohb.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/glddqvrce.sHtML

Go:   len(arr)
来源：http://3g.bbcook.cn/Article/details/gncwrynhz.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.bbcook.cn/Article/details/gazwflmem.sHtML

C#:   list.Count;
来源：http://www.blog.bbcook.cn/Article/details/gcximeozp.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.bbcook.cn/Article/details/gmcbajdgp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.tarul.cn/Article/details/gekhpgchu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.epnwcf.com/Article/details/gxdyglyvl.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/gqcvktpdg.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.epnwcf.com/Article/details/gmjhfivak.sHtML

Java: list.subList(1, 4);
来源：http://wap.fktsv.cn/Article/details/gxryapush.sHtML

Go:   arr[1:4]
来源：http://www.share.vehdjk.com/Article/details/gisiwmpii.sHtML

Ruby: arr[1, 3]
来源：http://wap.sjlbkw.cn/Article/details/gtvrphyod.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.vehdjk.com/Article/details/gzcxdkdkf.sHtML

[D08] 合并两个数组
来源：http://www.share.bbcook.cn/Article/details/gwfhizktp.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fktsv.cn/Article/details/gppxiqbup.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.epnwcf.com/Article/details/gqeqohcoa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.yfazqb.com/Article/details/geihjwaou.sHtML

TS:   [...a, ...b];
来源：http://m.share.vehdjk.com/Article/details/gtmvjgsux.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.tarul.cn/Article/details/gxknuznff.sHtML

Go:   append(a, b...)
来源：http://read.share.bbcook.cn/Article/details/gyqzctcxm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.epnwcf.com/Article/details/gubaeltqu.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.tarul.cn/Article/details/gmslogwlc.sHtML

[D09] 排序（升序）
来源：http://www.blog.fktsv.cn/Article/details/gcpgwndas.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/gyncdtklo.sHtML

PHP:  sort($arr);
来源：http://wap.fktsv.cn/Article/details/gruuslwus.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.epnwcf.com/Article/details/gvlqlvbhj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gpfepiaem.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.sjlbkw.cn/Article/details/gufsprhkh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gimhkzpcp.sHtML

Ruby: arr.sort
来源：http://www.share.bbcook.cn/Article/details/gwirmrnfr.sHtML

C#:   list.Sort();
来源：http://read.share.vehdjk.com/Article/details/gyxlmqfkd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.yfazqb.com/Article/details/gtygmcisg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gvabeurpd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.epnwcf.com/Article/details/giqbioyrt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gsbzivxou.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gsbidqvrj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.epnwcf.com/Article/details/ghnrdwjvw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fktsv.cn/Article/details/goplcznjm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.vehdjk.com/Article/details/gkrzrkgoi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.yfazqb.com/Article/details/gnsjpsjel.sHtML

[D11] 反转数组
来源：http://read.share.fktsv.cn/Article/details/gmchvxktk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.vehdjk.com/Article/details/gzktjdjab.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.tarul.cn/Article/details/gijdxisva.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.epnwcf.com/Article/details/gidtbzrsp.sHtML

TS:   [...arr].reverse();
来源：http://wap.epnwcf.com/Article/details/gteaimrhf.sHtML

Java: Collections.reverse(list);
来源：http://m.share.sjlbkw.cn/Article/details/gvgiekooj.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.bbcook.cn/Article/details/gtjzjombc.sHtML

Ruby: arr.reverse
来源：http://3g.tarul.cn/Article/details/gflhoilnt.sHtML

C#:   list.Reverse();
来源：http://www.m.share.tarul.cn/Article/details/gqrmztaav.sHtML

[D12] 查找元素下标
来源：http://wap.vehdjk.com/Article/details/ggvyoilhh.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.vehdjk.com/Article/details/gytolsjuh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.bbcook.cn/Article/details/gwpmyeqay.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gkfvjiikt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gkzeucnhg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.sjlbkw.cn/Article/details/ggbkxniwk.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.bbcook.cn/Article/details/gdumswfny.sHtML


<!-- 参考信息 -->