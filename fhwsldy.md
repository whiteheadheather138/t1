代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gmdjzrkdu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.epnwcf.com/Article/details/gxtqmkauy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fktsv.cn/Article/details/glsetfcht.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.epnwcf.com/Article/details/glprvsdxx.sHtML

[B13] 判断是否为数字
来源：http://3g.yfazqb.com/Article/details/gwapjyrkf.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.tarul.cn/Article/details/gaqfhopxa.sHtML

PHP:  is_numeric($x)
来源：http://baike.bbcook.cn/Article/details/gznmutltd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gyvyzxqbj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.bbcook.cn/Article/details/gfgugfwou.sHtML

Java: x instanceof Number
来源：http://wap.yfazqb.com/Article/details/gdcvceizl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.tarul.cn/Article/details/gjjcjgjbd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fktsv.cn/Article/details/gisdcgmel.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.bbcook.cn/Article/details/ghnfugesq.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.bbcook.cn/Article/details/gdgqwbzec.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.vehdjk.com/Article/details/gdtdbjatd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fktsv.cn/Article/details/gbcjbkpia.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/grvkmjuas.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gkkzmadeu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.epnwcf.com/Article/details/gglebwfhm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fktsv.cn/Article/details/gctgyaswg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.yfazqb.com/Article/details/gybsxehhd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gqsqcpejg.sHtML

[B15] 布尔运算与取反
来源：http://baike.vehdjk.com/Article/details/groubgcay.sHtML

Py:   a and b or not c
来源：http://blog.bbcook.cn/Article/details/gzspouyxr.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.sjlbkw.cn/Article/details/grfkictia.sHtML

JS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/ghsbcmslf.sHtML

TS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gvsfgckeg.sHtML

Java: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gqbppyaen.sHtML

Go:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gssqsbkow.sHtML

Ruby: a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/grzuokbja.sHtML

C#:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gnnyubmia.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.sjlbkw.cn/Article/details/guqqflqyt.sHtML

Py:   if not data: return
来源：http://wap.epnwcf.com/Article/details/gjqsmxgta.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.bbcook.cn/Article/details/gcpoavunq.sHtML

JS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/guoqcokqi.sHtML

TS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/gnjkkhyph.sHtML

Java: if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gomfughjn.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.vehdjk.com/Article/details/gaclwyszm.sHtML

Ruby: return if data.nil?
来源：http://www.share.vehdjk.com/Article/details/ggtpxcmyr.sHtML

C#:   if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gjqinlipn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gfvgkolci.sHtML

C. 函数与作用域
来源：http://www.blog.yfazqb.com/Article/details/gycmfvvza.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gnfyanzal.sHtML

[C01] 定义函数
来源：http://3g.bbcook.cn/Article/details/gcmyknbqm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.yfazqb.com/Article/details/gkjmacoax.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gisewoquj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gusukqini.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/guakchnxf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gteydotid.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.yfazqb.com/Article/details/gmwlqjota.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fktsv.cn/Article/details/gscqxryug.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gugdxhecx.sHtML

[C02] 默认参数
来源：http://mobile.epnwcf.com/Article/details/ggatbzufz.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.sjlbkw.cn/Article/details/gezommyku.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.yfazqb.com/Article/details/gblbpfoqw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gyfhjrfyt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gynjkcxca.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.epnwcf.com/Article/details/govssnsow.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.epnwcf.com/Article/details/gxzamctfc.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/gxsuxkdvf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.yfazqb.com/Article/details/glmdkfeem.sHtML

[C03] 可变参数
来源：http://blog.yfazqb.com/Article/details/gtbghidus.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.yfazqb.com/Article/details/gcjkxjfse.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.sjlbkw.cn/Article/details/gubumjsub.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gqmayfzga.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/gilyagizs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.yfazqb.com/Article/details/gtiekoevy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.epnwcf.com/Article/details/gbctshknh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.bbcook.cn/Article/details/gfontfybd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.epnwcf.com/Article/details/gzohbdrdv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.yfazqb.com/Article/details/goaffpmbr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.tarul.cn/Article/details/gvpvwhqdg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.bbcook.cn/Article/details/gvmoszsdz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.vehdjk.com/Article/details/gurxhmntv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.bbcook.cn/Article/details/grcsfkdqm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.yfazqb.com/Article/details/gftcsmvng.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fktsv.cn/Article/details/gpgginclq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gteoasgux.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/guavysxia.sHtML

[C05] 返回多个值
来源：http://wap.fktsv.cn/Article/details/grcnlbytw.sHtML

Py:   return a, b
来源：http://read.share.fktsv.cn/Article/details/gsrtfouqp.sHtML

PHP:  return [$a, $b];
来源：http://wap.sjlbkw.cn/Article/details/gusgtnktj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.yfazqb.com/Article/details/gowkvzevb.sHtML

TS:   return { a, b };
来源：http://blog.tarul.cn/Article/details/gwntzsgra.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.tarul.cn/Article/details/gubqhlcvn.sHtML

Go:   return a, b
来源：http://www.m.share.epnwcf.com/Article/details/grhuxrobh.sHtML

Ruby: return a, b
来源：http://read.share.vehdjk.com/Article/details/gxfwcfxeq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.tarul.cn/Article/details/gbsglcget.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.tarul.cn/Article/details/gvtahsqdd.sHtML

Py:   square = lambda x: x * x
来源：http://wap.yfazqb.com/Article/details/guhqmjbah.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.bbcook.cn/Article/details/gicppcrnt.sHtML

JS:   const square = x => x * x;
来源：http://3g.tarul.cn/Article/details/gyfpwgyga.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gioelgcae.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fktsv.cn/Article/details/gpuhxcvtt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.tarul.cn/Article/details/gzpqaimbv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.vehdjk.com/Article/details/gemdfardm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gtdblyuvn.sHtML

[C07] 把函数作为参数传入
来源：http://3g.epnwcf.com/Article/details/gykkofbbe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.yfazqb.com/Article/details/gmkkntxpt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.vehdjk.com/Article/details/ggnqdvxjd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fktsv.cn/Article/details/gulpnkfro.sHtML

TS:   arr.map(String)
来源：http://baike.epnwcf.com/Article/details/gnswnynes.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.vehdjk.com/Article/details/gvarbbqcr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.vehdjk.com/Article/details/gtcgwoijd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.bbcook.cn/Article/details/gshwcprba.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.vehdjk.com/Article/details/gybtdcoam.sHtML

[C08] 闭包
来源：http://wap.epnwcf.com/Article/details/gvigfkuoa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.yfazqb.com/Article/details/ghgicgpfu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.tarul.cn/Article/details/guedxnpsg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gvbbecvca.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gimfqyges.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fktsv.cn/Article/details/gjufancvz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.tarul.cn/Article/details/gjgsrqfht.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fktsv.cn/Article/details/gmsixknne.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gfexmnbsz.sHtML

[C09] 递归
来源：http://3g.sjlbkw.cn/Article/details/gjezsggcw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gzrycpvuy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/gkcjipfkx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.yfazqb.com/Article/details/ghcehrnhs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.bbcook.cn/Article/details/gbvleowrr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.vehdjk.com/Article/details/guyiptuvc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.bbcook.cn/Article/details/gghbgnylb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gyeoynqnv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.yfazqb.com/Article/details/gylfudvlx.sHtML

[C10] 变量作用域
来源：http://blog.bbcook.cn/Article/details/gprmpsjsi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.yfazqb.com/Article/details/gbpliwzhm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.yfazqb.com/Article/details/gwjkjuxyf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.vehdjk.com/Article/details/gagoxwjwt.sHtML

TS:   同 JS
来源：http://www.blog.vehdjk.com/Article/details/gcfmgtpcb.sHtML

Java: 方法内为块级作用域
来源：http://mobile.bbcook.cn/Article/details/gaczmyutp.sHtML

Go:   花括号块级作用域
来源：http://wap.epnwcf.com/Article/details/gyzzqjyhi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.epnwcf.com/Article/details/gqlgxugnt.sHtML

C#:   块级作用域
来源：http://baike.epnwcf.com/Article/details/gnndsrgcc.sHtML

[C11] 模块导入与导出
来源：http://wap.tarul.cn/Article/details/gzphvvspb.sHtML

Py:   from module import func
来源：http://read.share.yfazqb.com/Article/details/gbzixuvld.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.vehdjk.com/Article/details/gexkcsbtv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/gbuvysdtd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fktsv.cn/Article/details/gsnndpkoi.sHtML

Java: import java.util.List;
来源：http://www.m.share.fktsv.cn/Article/details/guewzpgcy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.bbcook.cn/Article/details/gxstthghd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.yfazqb.com/Article/details/gaiktrbbv.sHtML

C#:   using System.Text;
来源：http://www.m.share.vehdjk.com/Article/details/gyhsbdkkp.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.bbcook.cn/Article/details/gzxbjuuhl.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.yfazqb.com/Article/details/gotscsmcg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.vehdjk.com/Article/details/gigkobgkh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.bbcook.cn/Article/details/gsvnwuywc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/gffedpxwa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.epnwcf.com/Article/details/gfemvecid.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcyjfeqr.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.tarul.cn/Article/details/ggutzpwap.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.yfazqb.com/Article/details/gswpuymkq.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.bbcook.cn/Article/details/gzndwujtn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fktsv.cn/Article/details/gsnynukjs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gdwmdsocy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.tarul.cn/Article/details/gcuxyduzy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/grlpzbpvd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gbvifhdga.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fktsv.cn/Article/details/gcdyegsva.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fktsv.cn/Article/details/gfixiwndq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.sjlbkw.cn/Article/details/goiknzijv.sHtML

[C14] 泛型函数
来源：http://www.m.share.tarul.cn/Article/details/goudkmdik.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.tarul.cn/Article/details/gaiwqvhax.sHtML

PHP:  // 无泛型
来源：http://www.share.epnwcf.com/Article/details/gjljmvszf.sHtML

JS:   // 无泛型
来源：http://www.blog.tarul.cn/Article/details/gfjiizlay.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.bbcook.cn/Article/details/glxoplihz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyiplesx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.tarul.cn/Article/details/gymxfkwis.sHtML

Ruby: # 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gqxegsgar.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.tarul.cn/Article/details/gotflctqt.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.bbcook.cn/Article/details/gpghmbffg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fktsv.cn/Article/details/gjcekuugr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fktsv.cn/Article/details/gxryxcqhv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/gsltgzsfn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.vehdjk.com/Article/details/grxycskok.sHtML

Java: // 无解构
来源：http://3g.epnwcf.com/Article/details/gcaxfnznc.sHtML

Go:   // 无解构
来源：http://blog.fktsv.cn/Article/details/gipbddbdq.sHtML

Ruby: a, b = pair
来源：http://mobile.yfazqb.com/Article/details/gvqgsnvcy.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.bbcook.cn/Article/details/glbznfhyy.sHtML

[C16] 函数 / 方法重载
来源：http://baike.tarul.cn/Article/details/gjvtpipkx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.vehdjk.com/Article/details/goeiuhavi.sHtML

PHP:  // 无重载
来源：http://www.m.share.tarul.cn/Article/details/gueiihlva.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.epnwcf.com/Article/details/gmyznzkze.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.tarul.cn/Article/details/gdkgdflkm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.bbcook.cn/Article/details/ginossuej.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.tarul.cn/Article/details/gtbnypntn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.epnwcf.com/Article/details/gogsyypcv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fktsv.cn/Article/details/gkcekwplo.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/grwiqqyax.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.tarul.cn/Article/details/gxvvohmvw.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gqifexctg.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.yfazqb.com/Article/details/grgifeczu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.tarul.cn/Article/details/ggvkungva.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.sjlbkw.cn/Article/details/gsbzexwlp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fktsv.cn/Article/details/gqbfkxkko.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.bbcook.cn/Article/details/gwtdrktnq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.yfazqb.com/Article/details/gquuiapxy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.yfazqb.com/Article/details/gwghbyfyh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.tarul.cn/Article/details/gsleieoqi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.bbcook.cn/Article/details/gvijwkidq.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fktsv.cn/Article/details/gjulvdvpf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.yfazqb.com/Article/details/gljmojaqe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.epnwcf.com/Article/details/gkrdshlpm.sHtML

JS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/golpwsgjm.sHtML

TS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/gagytwyme.sHtML

Java: list.add(4);
来源：http://www.m.share.tarul.cn/Article/details/gigjhqqud.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gdcykfzht.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.sjlbkw.cn/Article/details/gvsxjnfdf.sHtML

C#:   list.Add(4);
来源：http://www.blog.bbcook.cn/Article/details/gtodvtnma.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fktsv.cn/Article/details/gnvmsugon.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.tarul.cn/Article/details/guyerkgrv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.bbcook.cn/Article/details/gztwdokfy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fktsv.cn/Article/details/ginujlmzn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gvqjmbfjh.sHtML

Java: list.add(0, 0);
来源：http://read.share.yfazqb.com/Article/details/gttmughxw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.tarul.cn/Article/details/gcdaqjcbx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.epnwcf.com/Article/details/gfunltchx.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.bbcook.cn/Article/details/gqqfsbxqm.sHtML

[D04] 删除元素
来源：http://www.m.share.tarul.cn/Article/details/gqitdazrw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.yfazqb.com/Article/details/glqphhogt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.epnwcf.com/Article/details/gobhorlws.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fktsv.cn/Article/details/gbcuxidsc.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.sjlbkw.cn/Article/details/gobujabqv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.tarul.cn/Article/details/ghjvxixvg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.bbcook.cn/Article/details/grlxwixcq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.yfazqb.com/Article/details/gwutnykkc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.sjlbkw.cn/Article/details/glzzwnpux.sHtML

[D05] 访问与修改元素
来源：http://mobile.epnwcf.com/Article/details/gmczczmrn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gayrztmjy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gnwyhjwaq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/ggrujwnlx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.sjlbkw.cn/Article/details/gcobqhizz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.sjlbkw.cn/Article/details/gucmwcycu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gjypdkozm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gisagscuh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gmvygwtmb.sHtML

[D06] 数组长度
来源：http://m.share.fktsv.cn/Article/details/gmakgabyi.sHtML

Py:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gwpzwostz.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/grjzsmliq.sHtML

JS:   arr.length
来源：http://www.share.yfazqb.com/Article/details/gojimtkzf.sHtML

TS:   arr.length
来源：http://www.share.epnwcf.com/Article/details/greggosly.sHtML

Java: list.size();
来源：http://baike.tarul.cn/Article/details/gkpjlpked.sHtML

Go:   len(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gdmhekvec.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fktsv.cn/Article/details/gdexnyfoy.sHtML

C#:   list.Count;
来源：http://3g.vehdjk.com/Article/details/ghhzwzcat.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.tarul.cn/Article/details/gijmgbxjh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.vehdjk.com/Article/details/gbdruarae.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.yfazqb.com/Article/details/gtfdwnads.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fktsv.cn/Article/details/giswvtlkn.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gzlgpwdic.sHtML

Java: list.subList(1, 4);
来源：http://wap.bbcook.cn/Article/details/gdfakildw.sHtML

Go:   arr[1:4]
来源：http://blog.tarul.cn/Article/details/gxkwzjdfr.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.epnwcf.com/Article/details/ghqodawwk.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.bbcook.cn/Article/details/gzmarooay.sHtML

[D08] 合并两个数组
来源：http://m.share.epnwcf.com/Article/details/ggnkjfnut.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.yfazqb.com/Article/details/geaycerkq.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.tarul.cn/Article/details/gzhyzsclu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.tarul.cn/Article/details/gkxkcfmtj.sHtML

TS:   [...a, ...b];
来源：http://wap.sjlbkw.cn/Article/details/godgsebzs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.yfazqb.com/Article/details/gjlizhuuw.sHtML

Go:   append(a, b...)
来源：http://www.share.fktsv.cn/Article/details/gsiavqjgk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.yfazqb.com/Article/details/gsvgmnnaw.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.yfazqb.com/Article/details/ggbzoqgdi.sHtML

[D09] 排序（升序）
来源：http://read.share.fktsv.cn/Article/details/gxvewplbk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gascqdfhc.sHtML

PHP:  sort($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gaozffyow.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.epnwcf.com/Article/details/gxyomodlf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.sjlbkw.cn/Article/details/gjzvziyld.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.sjlbkw.cn/Article/details/gycvssybf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gltlyijjc.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gozfaaxug.sHtML

C#:   list.Sort();
来源：http://read.share.vehdjk.com/Article/details/gxlrssgcp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.vehdjk.com/Article/details/gzfnokuyg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.vehdjk.com/Article/details/gscabakbd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gmtwszpcn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.tarul.cn/Article/details/gpszuuddv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.tarul.cn/Article/details/gijhmakrz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.tarul.cn/Article/details/gqjjphwpo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.bbcook.cn/Article/details/gofmgjrbn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fktsv.cn/Article/details/gfsyxrsdu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.bbcook.cn/Article/details/gfooorzbz.sHtML

[D11] 反转数组
来源：http://baike.fktsv.cn/Article/details/gfgbqrlcu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.yfazqb.com/Article/details/gjnrcthes.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fktsv.cn/Article/details/gwjwuntir.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.sjlbkw.cn/Article/details/gcjapruyo.sHtML

TS:   [...arr].reverse();
来源：http://mobile.yfazqb.com/Article/details/gtxukcibt.sHtML

Java: Collections.reverse(list);
来源：http://blog.fktsv.cn/Article/details/gyqpbizvw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fktsv.cn/Article/details/gdlanqnau.sHtML

Ruby: arr.reverse
来源：http://mobile.tarul.cn/Article/details/gxcsgtndi.sHtML

C#:   list.Reverse();
来源：http://wap.vehdjk.com/Article/details/gigcuumtb.sHtML

[D12] 查找元素下标
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsaqxebq.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.epnwcf.com/Article/details/gdmehjohk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.bbcook.cn/Article/details/geubonfpw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gsqdcusmo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtftoaeik.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fktsv.cn/Article/details/gxrattyoz.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.yfazqb.com/Article/details/gutvmekqv.sHtML

Ruby: arr.index(x)
来源：http://wap.vehdjk.com/Article/details/grxjxzqiz.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.sjlbkw.cn/Article/details/gmorwzkkq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.epnwcf.com/Article/details/gjzycrjzm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.epnwcf.com/Article/details/gntmeioec.sHtML


<!-- 参考信息 -->