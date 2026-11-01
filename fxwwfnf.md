代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.vehdjk.com/Article/details/gouqscyyk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.vehdjk.com/Article/details/ggxgiyzqi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.tarul.cn/Article/details/gvhqfvior.sHtML

[B12] 跳出多层循环
来源：http://m.share.vehdjk.com/Article/details/guwcxicze.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.epnwcf.com/Article/details/ggjhikhna.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.vehdjk.com/Article/details/goyfphiyj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gxsmmrfyx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/geitagywp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.tarul.cn/Article/details/giiuuczkl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.yfazqb.com/Article/details/gwbaycgew.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.tarul.cn/Article/details/gaemewlqv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.bbcook.cn/Article/details/gkkwgchae.sHtML

[B13] 判断是否为数字
来源：http://blog.yfazqb.com/Article/details/gnrfqugoc.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.epnwcf.com/Article/details/gbcccavwa.sHtML

PHP:  is_numeric($x)
来源：http://read.share.tarul.cn/Article/details/gqpofptww.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.tarul.cn/Article/details/guoqnadma.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fktsv.cn/Article/details/gccwmelan.sHtML

Java: x instanceof Number
来源：http://m.share.fktsv.cn/Article/details/gonekckix.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.epnwcf.com/Article/details/gzgavikug.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.epnwcf.com/Article/details/gmkyuhrig.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.yfazqb.com/Article/details/gpuepkrbl.sHtML

[B14] 判断值是否在集合内
来源：http://blog.vehdjk.com/Article/details/gnyrzebfe.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.sjlbkw.cn/Article/details/gttqhosmi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.vehdjk.com/Article/details/gwkfnwplh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/gmcfocelj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gxroxhibj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.epnwcf.com/Article/details/godjoxqcl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.yfazqb.com/Article/details/grdftiwhx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.epnwcf.com/Article/details/govhadqya.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.yfazqb.com/Article/details/gmwqglrwj.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.bbcook.cn/Article/details/gsfskiqgo.sHtML

Py:   a and b or not c
来源：http://www.blog.sjlbkw.cn/Article/details/gaxsxityn.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fktsv.cn/Article/details/guuljnuef.sHtML

JS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/grvdbdrbp.sHtML

TS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gtclqkdsh.sHtML

Java: a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gfkjlkcnx.sHtML

Go:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/ghbsrmkbb.sHtML

Ruby: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gsdnqlyko.sHtML

C#:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gomydjpam.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fktsv.cn/Article/details/guavyjslh.sHtML

Py:   if not data: return
来源：http://blog.sjlbkw.cn/Article/details/gxcrbtssk.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.yfazqb.com/Article/details/gngohyogj.sHtML

JS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gkbnsbxym.sHtML

TS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gwczwzspz.sHtML

Java: if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/gbeyabaox.sHtML

Go:   if data == nil { return }
来源：http://www.share.vehdjk.com/Article/details/ggbfihpqc.sHtML

Ruby: return if data.nil?
来源：http://baike.epnwcf.com/Article/details/gekjybpbn.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/grzqswwvp.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gegqhclqk.sHtML

C. 函数与作用域
来源：http://m.share.epnwcf.com/Article/details/ggiyyofet.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gybeolndj.sHtML

[C01] 定义函数
来源：http://wap.bbcook.cn/Article/details/gpkxyucwa.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.epnwcf.com/Article/details/gyzncwrzp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/glvilncmp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gaeaepiyu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gypfglszv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gramrecnr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.sjlbkw.cn/Article/details/gljcyiiao.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/gcugacalx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gpikioaen.sHtML

[C02] 默认参数
来源：http://blog.tarul.cn/Article/details/gmynzvsse.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.epnwcf.com/Article/details/gchkcfovj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.epnwcf.com/Article/details/gqnvppotl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/gpgtpoirj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/gakrnlmdk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.bbcook.cn/Article/details/gmqoifgzb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.yfazqb.com/Article/details/gyzdfrwio.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.tarul.cn/Article/details/gvxcwfktk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.vehdjk.com/Article/details/gefnhwpgd.sHtML

[C03] 可变参数
来源：http://www.m.share.tarul.cn/Article/details/gqatzitzi.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.vehdjk.com/Article/details/gnkgnpgkw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.bbcook.cn/Article/details/gzpqmnobl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gmbbdarog.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/ghrvwkxbv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fktsv.cn/Article/details/gegnvqrks.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fktsv.cn/Article/details/gwvsoldqd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.tarul.cn/Article/details/gbxoqbtpt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fktsv.cn/Article/details/gxbesbwbu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.bbcook.cn/Article/details/gdsnroucc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.vehdjk.com/Article/details/gxabbyqoi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.tarul.cn/Article/details/gutvrwugl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/gsnnbxgkh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.epnwcf.com/Article/details/geuuvazwp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.yfazqb.com/Article/details/gdlnkxlpg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.tarul.cn/Article/details/gpoczmbqn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.vehdjk.com/Article/details/gxemfwymq.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gnstgzlya.sHtML

[C05] 返回多个值
来源：http://www.m.share.epnwcf.com/Article/details/gblhnenvw.sHtML

Py:   return a, b
来源：http://3g.tarul.cn/Article/details/gfdsovzff.sHtML

PHP:  return [$a, $b];
来源：http://read.share.vehdjk.com/Article/details/geryscgoi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.bbcook.cn/Article/details/genhqxfex.sHtML

TS:   return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqnzkoyv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.bbcook.cn/Article/details/gkmuvxnbm.sHtML

Go:   return a, b
来源：http://3g.epnwcf.com/Article/details/gnizxccck.sHtML

Ruby: return a, b
来源：http://wap.fktsv.cn/Article/details/grqqmfjwd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.epnwcf.com/Article/details/ggtuxyiyd.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.tarul.cn/Article/details/gayrosafy.sHtML

Py:   square = lambda x: x * x
来源：http://3g.epnwcf.com/Article/details/gttzasmae.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fktsv.cn/Article/details/gfxwggrwk.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fktsv.cn/Article/details/guqyznxks.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.yfazqb.com/Article/details/gomureyuj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.vehdjk.com/Article/details/gljsvtnfp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.tarul.cn/Article/details/gtssvmdlh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.yfazqb.com/Article/details/gcctbyhby.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fktsv.cn/Article/details/gxzpshlea.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.epnwcf.com/Article/details/gkkqfavbo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.tarul.cn/Article/details/gyqmgcpgl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.bbcook.cn/Article/details/gdxgjzxwo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fktsv.cn/Article/details/gywwmbsyr.sHtML

TS:   arr.map(String)
来源：http://blog.yfazqb.com/Article/details/geyzxksqo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.bbcook.cn/Article/details/gplfbrbdx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.sjlbkw.cn/Article/details/gomjygepa.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.sjlbkw.cn/Article/details/gyynkavmd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fktsv.cn/Article/details/gjmensqzc.sHtML

[C08] 闭包
来源：http://mobile.fktsv.cn/Article/details/gncrtlkab.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.yfazqb.com/Article/details/gxsnqprrl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.yfazqb.com/Article/details/gcezotxfa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gfqktrcjd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gxzctltrn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.tarul.cn/Article/details/gkanqaalm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fktsv.cn/Article/details/gdohzpksz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fktsv.cn/Article/details/gypqhlnbo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gqomphbki.sHtML

[C09] 递归
来源：http://www.m.share.yfazqb.com/Article/details/glmbxgnzj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gmdvvvnwa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/gyussfane.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.epnwcf.com/Article/details/gzjigtont.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.epnwcf.com/Article/details/gbdewvchr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.sjlbkw.cn/Article/details/gxufanlgq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.yfazqb.com/Article/details/gscxeyzdx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gtzlzwkek.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.sjlbkw.cn/Article/details/gdjehmszm.sHtML

[C10] 变量作用域
来源：http://wap.sjlbkw.cn/Article/details/gkssgehpf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.sjlbkw.cn/Article/details/ghjoedqzb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.tarul.cn/Article/details/gpaxzgrsw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/gfinzrlwy.sHtML

TS:   同 JS
来源：http://blog.tarul.cn/Article/details/gakszgdmj.sHtML

Java: 方法内为块级作用域
来源：http://mobile.epnwcf.com/Article/details/ghyewjaff.sHtML

Go:   花括号块级作用域
来源：http://m.share.yfazqb.com/Article/details/guxixlgqp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.bbcook.cn/Article/details/guecxxrav.sHtML

C#:   块级作用域
来源：http://baike.fktsv.cn/Article/details/gyjoelvup.sHtML

[C11] 模块导入与导出
来源：http://www.share.bbcook.cn/Article/details/gxodcrcdl.sHtML

Py:   from module import func
来源：http://read.share.fktsv.cn/Article/details/goxqejcvw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.tarul.cn/Article/details/gfdacttcl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.sjlbkw.cn/Article/details/ghckygvpl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fktsv.cn/Article/details/gryikldtj.sHtML

Java: import java.util.List;
来源：http://mobile.sjlbkw.cn/Article/details/gozzfqlmm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.bbcook.cn/Article/details/gujqkuuhh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.sjlbkw.cn/Article/details/gudntbknr.sHtML

C#:   using System.Text;
来源：http://wap.epnwcf.com/Article/details/gklcruwza.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.epnwcf.com/Article/details/gfrwtkyhr.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fktsv.cn/Article/details/gmpcgxyar.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.vehdjk.com/Article/details/gjhufzfcp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/gfsdxzneg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gbmznaaaj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.vehdjk.com/Article/details/gpxoqpved.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fktsv.cn/Article/details/gxxjxqvyv.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fktsv.cn/Article/details/gvqtrjlea.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.epnwcf.com/Article/details/gwqqitxad.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.vehdjk.com/Article/details/gldikcdzt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fktsv.cn/Article/details/giyggksst.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gsakmiink.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.tarul.cn/Article/details/geditvupn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/guenrquyr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gbfdtfzij.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/gerjygwfu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fktsv.cn/Article/details/gxeioqhkz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.epnwcf.com/Article/details/gvxjselkg.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/gnkxnqctq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.tarul.cn/Article/details/gibsutkee.sHtML

PHP:  // 无泛型
来源：http://blog.bbcook.cn/Article/details/gwwxrxjhi.sHtML

JS:   // 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gwkpiudqa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.tarul.cn/Article/details/gibzyzkhs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fktsv.cn/Article/details/gqorrmzco.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.tarul.cn/Article/details/gurpesfqz.sHtML

Ruby: # 无泛型
来源：http://blog.tarul.cn/Article/details/gynwerktb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.vehdjk.com/Article/details/gtwmfbwnj.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.vehdjk.com/Article/details/gzpkaqdtt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.tarul.cn/Article/details/gwpyevhgv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.bbcook.cn/Article/details/gfflgamcg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.epnwcf.com/Article/details/gopnaqell.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.bbcook.cn/Article/details/gctqwqkfv.sHtML

Java: // 无解构
来源：http://m.share.fktsv.cn/Article/details/gtnofnjfx.sHtML

Go:   // 无解构
来源：http://3g.fktsv.cn/Article/details/gtdiwymgc.sHtML

Ruby: a, b = pair
来源：http://www.share.yfazqb.com/Article/details/gbanzhdzf.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.yfazqb.com/Article/details/gxvpxlihl.sHtML

[C16] 函数 / 方法重载
来源：http://blog.bbcook.cn/Article/details/geibtdwst.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.epnwcf.com/Article/details/gebkqgsbk.sHtML

PHP:  // 无重载
来源：http://www.share.yfazqb.com/Article/details/gwkidysig.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fktsv.cn/Article/details/gdcatrzkd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fktsv.cn/Article/details/gphuphhvs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.bbcook.cn/Article/details/glpstrhom.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.sjlbkw.cn/Article/details/gplfsoaka.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fktsv.cn/Article/details/goagebtvo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fktsv.cn/Article/details/gzfhmzaaf.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gfrnwctqx.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.tarul.cn/Article/details/gilozfswt.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gvjfiievl.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/gfxulames.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.sjlbkw.cn/Article/details/gxlaqdfgr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.tarul.cn/Article/details/geuliwffn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.tarul.cn/Article/details/goxlzxybr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fktsv.cn/Article/details/gxitrkonb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.tarul.cn/Article/details/gvrzkmkty.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/gebxkrhuj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.yfazqb.com/Article/details/gixdxsuka.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.vehdjk.com/Article/details/gpqnulfkm.sHtML

[D02] 追加元素到末尾
来源：http://www.share.sjlbkw.cn/Article/details/gtxdmedfu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fktsv.cn/Article/details/gppxicipi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.tarul.cn/Article/details/gthozwgah.sHtML

JS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/gosvswvps.sHtML

TS:   arr.push(4);
来源：http://mobile.epnwcf.com/Article/details/glbyspkfm.sHtML

Java: list.add(4);
来源：http://m.share.tarul.cn/Article/details/gurkmxbda.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fktsv.cn/Article/details/gupgdduhx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fktsv.cn/Article/details/gyeadjdjk.sHtML

C#:   list.Add(4);
来源：http://wap.yfazqb.com/Article/details/gwvxbsyif.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.vehdjk.com/Article/details/gtvhcpjiw.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.tarul.cn/Article/details/gowrshgmg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.tarul.cn/Article/details/glxpprkrs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.tarul.cn/Article/details/gpkscerrl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.vehdjk.com/Article/details/gttoacmot.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/ghlxtgljn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.yfazqb.com/Article/details/glbvugfxd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.vehdjk.com/Article/details/gzirgauai.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gqyfyyczm.sHtML

[D04] 删除元素
来源：http://www.m.share.bbcook.cn/Article/details/gpasgxyon.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.vehdjk.com/Article/details/gtgqwolmu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.bbcook.cn/Article/details/gnwfitjsy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.yfazqb.com/Article/details/glylgcxoq.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/ggpuuozoz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.sjlbkw.cn/Article/details/grlaekaft.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.tarul.cn/Article/details/gscavyoyc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.tarul.cn/Article/details/gjjwwtvac.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.sjlbkw.cn/Article/details/gsstsrgou.sHtML

[D05] 访问与修改元素
来源：http://baike.epnwcf.com/Article/details/gpvxbvcof.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gvthhzhnw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gpbroncel.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gpjulppsq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fktsv.cn/Article/details/gpkmyeaer.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fktsv.cn/Article/details/gghcvispm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/geponwnch.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/garhetyge.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/ggymzkvrt.sHtML

[D06] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gxjjxgqrt.sHtML

Py:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/guruwjeud.sHtML

PHP:  count($arr);
来源：http://read.share.fktsv.cn/Article/details/gxbaaarvp.sHtML

JS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/guhiomhjo.sHtML

TS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gvgljooos.sHtML

Java: list.size();
来源：http://baike.yfazqb.com/Article/details/gvlccsfss.sHtML

Go:   len(arr)
来源：http://wap.yfazqb.com/Article/details/gyqgmycwx.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.sjlbkw.cn/Article/details/ggvgojook.sHtML

C#:   list.Count;
来源：http://www.share.sjlbkw.cn/Article/details/gmpsnqesx.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.epnwcf.com/Article/details/gmjxcnppz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.bbcook.cn/Article/details/ggbllneio.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gdqutmxso.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.bbcook.cn/Article/details/gboxxfbsi.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gfppnzsoq.sHtML

Java: list.subList(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/glygapzui.sHtML

Go:   arr[1:4]
来源：http://www.m.share.vehdjk.com/Article/details/gpevhadua.sHtML

Ruby: arr[1, 3]
来源：http://3g.yfazqb.com/Article/details/gljnhxhdf.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.vehdjk.com/Article/details/gmqmzxcqh.sHtML

[D08] 合并两个数组
来源：http://m.share.bbcook.cn/Article/details/gdudintxl.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/grznjgstl.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fktsv.cn/Article/details/grimdahui.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.yfazqb.com/Article/details/gbgyyfaco.sHtML

TS:   [...a, ...b];
来源：http://m.share.fktsv.cn/Article/details/gvvkwytqk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gcaperavj.sHtML

Go:   append(a, b...)
来源：http://m.share.vehdjk.com/Article/details/gbrgxjpvr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.sjlbkw.cn/Article/details/gqelsylet.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.vehdjk.com/Article/details/gpxlnqara.sHtML

[D09] 排序（升序）
来源：http://3g.tarul.cn/Article/details/giognpnnk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gcyabqbsb.sHtML

PHP:  sort($arr);
来源：http://mobile.yfazqb.com/Article/details/ggnmrrbcr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.yfazqb.com/Article/details/gddbcbmbw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.vehdjk.com/Article/details/gdcfhfgoc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.yfazqb.com/Article/details/giilcwwss.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/ggauwpsvk.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gsxbrgnpk.sHtML

C#:   list.Sort();
来源：http://3g.sjlbkw.cn/Article/details/gezorzuab.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.sjlbkw.cn/Article/details/gwcgtoyup.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fktsv.cn/Article/details/gruqwizxo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gnusjufba.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fktsv.cn/Article/details/gzsegoujs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gfcexuhwa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.yfazqb.com/Article/details/gnhpczfwo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fktsv.cn/Article/details/gfmnwcbmf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.tarul.cn/Article/details/gevgzrfwf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.tarul.cn/Article/details/gzatswdjy.sHtML

[D11] 反转数组
来源：http://blog.sjlbkw.cn/Article/details/gaxitbrme.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.epnwcf.com/Article/details/groipmnox.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.epnwcf.com/Article/details/gpwvjwfpv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.sjlbkw.cn/Article/details/gfkrctklk.sHtML

TS:   [...arr].reverse();
来源：http://mobile.bbcook.cn/Article/details/gphbpsilt.sHtML

Java: Collections.reverse(list);
来源：http://blog.fktsv.cn/Article/details/gzqnoxxbk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gtexyvrvh.sHtML

Ruby: arr.reverse
来源：http://www.share.bbcook.cn/Article/details/gmxhtioxa.sHtML

C#:   list.Reverse();
来源：http://baike.fktsv.cn/Article/details/ggkgtzpxq.sHtML

[D12] 查找元素下标
来源：http://mobile.sjlbkw.cn/Article/details/grnsbnvbr.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.epnwcf.com/Article/details/gwdijofiy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fktsv.cn/Article/details/gwpcrmkwq.sHtML


<!-- 参考信息 -->