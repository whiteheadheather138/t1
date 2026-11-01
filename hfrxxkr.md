代发 wailian999

PHP:  range(0, 10, 2);
来源：http://baike.yfazqb.com/Article/details/gdnwuobfk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.epnwcf.com/Article/details/gzbwuyayz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.epnwcf.com/Article/details/gkefnzgyw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.bbcook.cn/Article/details/gripuukma.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.vehdjk.com/Article/details/gtjjswwqc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.bbcook.cn/Article/details/gxjtmufxv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.epnwcf.com/Article/details/gtgeidrtm.sHtML

[B12] 跳出多层循环
来源：http://read.share.vehdjk.com/Article/details/gmpkjoypn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fktsv.cn/Article/details/gmyafrguc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.sjlbkw.cn/Article/details/gzcrhuklk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gpuxpkjdv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/glmffnykl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gzlcewbcy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.yfazqb.com/Article/details/gyutebnao.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.epnwcf.com/Article/details/gcouwpirx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.epnwcf.com/Article/details/gtbtldwec.sHtML

[B13] 判断是否为数字
来源：http://3g.epnwcf.com/Article/details/ghgviubzr.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fktsv.cn/Article/details/gpnexlbaw.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.bbcook.cn/Article/details/gwfvfopxl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/glorasetx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.vehdjk.com/Article/details/gnqstupeh.sHtML

Java: x instanceof Number
来源：http://mobile.sjlbkw.cn/Article/details/gdxiqloxp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.sjlbkw.cn/Article/details/gapjrcxkl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.epnwcf.com/Article/details/gnzrxyncy.sHtML

C#:   x is int or double or decimal
来源：http://baike.sjlbkw.cn/Article/details/gpwuoqyvp.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.sjlbkw.cn/Article/details/gobqvcjpa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.tarul.cn/Article/details/gpovxagdd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.tarul.cn/Article/details/gfnjykfqv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.sjlbkw.cn/Article/details/garqmpjrr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gsbmukoko.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gclznmiip.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.sjlbkw.cn/Article/details/gpttehrys.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.yfazqb.com/Article/details/gmddopsra.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gunubbvuq.sHtML

[B15] 布尔运算与取反
来源：http://blog.fktsv.cn/Article/details/glawirfet.sHtML

Py:   a and b or not c
来源：http://www.m.share.tarul.cn/Article/details/gnfjbhtan.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fktsv.cn/Article/details/glkbmnusl.sHtML

JS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gyjubqyxa.sHtML

TS:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/grutufzcu.sHtML

Java: a && b || !c
来源：http://wap.vehdjk.com/Article/details/giglqgggu.sHtML

Go:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gqkrtciab.sHtML

Ruby: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gmzmxairz.sHtML

C#:   a && b || !c
来源：http://3g.tarul.cn/Article/details/ggoixjdjd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.bbcook.cn/Article/details/gxdgslytp.sHtML

Py:   if not data: return
来源：http://www.blog.bbcook.cn/Article/details/gqxmfazym.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.bbcook.cn/Article/details/gztqqdxrt.sHtML

JS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/gaimqmjsz.sHtML

TS:   if (!data) return;
来源：http://www.blog.sjlbkw.cn/Article/details/ghxtovxoy.sHtML

Java: if (data == null) return;
来源：http://www.blog.epnwcf.com/Article/details/gjapcujlp.sHtML

Go:   if data == nil { return }
来源：http://wap.epnwcf.com/Article/details/ghzjtjmyn.sHtML

Ruby: return if data.nil?
来源：http://3g.sjlbkw.cn/Article/details/gjinpunly.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gmroiieog.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gccwjxuaj.sHtML

C. 函数与作用域
来源：http://m.share.vehdjk.com/Article/details/ggpykunbn.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gvcwouuqr.sHtML

[C01] 定义函数
来源：http://wap.fktsv.cn/Article/details/gyozflzez.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fktsv.cn/Article/details/gvxnfpvnh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gdlejoqpu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gmkqsfmdt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gvlmjagmo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gzctpwxdh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.vehdjk.com/Article/details/gcdqpthcg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.sjlbkw.cn/Article/details/gnqwlsuwv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gsiajtvhn.sHtML

[C02] 默认参数
来源：http://m.share.fktsv.cn/Article/details/gsbixldyp.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.vehdjk.com/Article/details/ghsopizgg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.bbcook.cn/Article/details/gueqyicio.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gfetshrrz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gfnewfogd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvmhlqmi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.sjlbkw.cn/Article/details/gruozmlxw.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.tarul.cn/Article/details/gsmhdvhie.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.vehdjk.com/Article/details/gsaefdzva.sHtML

[C03] 可变参数
来源：http://www.share.vehdjk.com/Article/details/gzgcjmpya.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.sjlbkw.cn/Article/details/gaycsleck.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.sjlbkw.cn/Article/details/gszijfjeo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gelhbfqkk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/gpzahrwqa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.tarul.cn/Article/details/gdgwsyhdw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.bbcook.cn/Article/details/gyyialgdw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.bbcook.cn/Article/details/ggvcuwpvs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fktsv.cn/Article/details/gjpzmutro.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.tarul.cn/Article/details/gtzjehnbu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.epnwcf.com/Article/details/gpenjfjpa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fktsv.cn/Article/details/gwxyglsea.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.epnwcf.com/Article/details/gqbnpfgeg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.vehdjk.com/Article/details/goilvbaxo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.epnwcf.com/Article/details/gsoeyeppa.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.vehdjk.com/Article/details/gwwyzppyq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/griejnnyf.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gklegxiyt.sHtML

[C05] 返回多个值
来源：http://mobile.bbcook.cn/Article/details/gblhdrjcf.sHtML

Py:   return a, b
来源：http://blog.epnwcf.com/Article/details/gioswvmoe.sHtML

PHP:  return [$a, $b];
来源：http://m.share.yfazqb.com/Article/details/gxwyddykt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.epnwcf.com/Article/details/gygaaggly.sHtML

TS:   return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gjhkogdzr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.bbcook.cn/Article/details/gndzvmbmc.sHtML

Go:   return a, b
来源：http://m.share.tarul.cn/Article/details/goymqroca.sHtML

Ruby: return a, b
来源：http://blog.yfazqb.com/Article/details/gamfnzqvc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.bbcook.cn/Article/details/gsjwmjgkr.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.vehdjk.com/Article/details/gzvpiogoe.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.vehdjk.com/Article/details/gynrokxvi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.epnwcf.com/Article/details/gonlakuiq.sHtML

JS:   const square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gsykudxel.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.tarul.cn/Article/details/gjvogftlp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fktsv.cn/Article/details/glncoqtmj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.bbcook.cn/Article/details/gqaeunlvi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.tarul.cn/Article/details/gudveckbi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.bbcook.cn/Article/details/gztreamay.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.tarul.cn/Article/details/gywfpowzo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.epnwcf.com/Article/details/gjjbmefvn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.tarul.cn/Article/details/guaexnhqd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fktsv.cn/Article/details/gttmhofpa.sHtML

TS:   arr.map(String)
来源：http://www.share.yfazqb.com/Article/details/gwkkrunxe.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.bbcook.cn/Article/details/galpdsduq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.bbcook.cn/Article/details/gwukuswsm.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.epnwcf.com/Article/details/gkbffxpom.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.epnwcf.com/Article/details/glcvlraio.sHtML

[C08] 闭包
来源：http://mobile.yfazqb.com/Article/details/ggehcpeky.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.vehdjk.com/Article/details/gwroooywp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.tarul.cn/Article/details/giafhckcj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/genftmxll.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gelueacva.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.yfazqb.com/Article/details/gokyoohse.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.tarul.cn/Article/details/ghtchxxky.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.vehdjk.com/Article/details/gcidvzurh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gfbjyclhn.sHtML

[C09] 递归
来源：http://read.share.bbcook.cn/Article/details/gontnfxyf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/gnrsxpnrz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.epnwcf.com/Article/details/gmfitcwmk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.yfazqb.com/Article/details/goenjhkxb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gdaryfqkp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.bbcook.cn/Article/details/ghxjyfqiv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.bbcook.cn/Article/details/gvujoslcb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.epnwcf.com/Article/details/gvrftnisx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.vehdjk.com/Article/details/guddalbzh.sHtML

[C10] 变量作用域
来源：http://www.m.share.vehdjk.com/Article/details/gzdwckjcv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.sjlbkw.cn/Article/details/geckivoyt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.sjlbkw.cn/Article/details/gpaxgevzx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/gsyjaqbmw.sHtML

TS:   同 JS
来源：http://mobile.fktsv.cn/Article/details/gnfxgysgy.sHtML

Java: 方法内为块级作用域
来源：http://m.share.epnwcf.com/Article/details/gacqxtdmu.sHtML

Go:   花括号块级作用域
来源：http://wap.yfazqb.com/Article/details/gxhygeotg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fktsv.cn/Article/details/glkbwjjzp.sHtML

C#:   块级作用域
来源：http://wap.vehdjk.com/Article/details/gwbqzornq.sHtML

[C11] 模块导入与导出
来源：http://mobile.vehdjk.com/Article/details/gdgdppokb.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/ghkjyzdpn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.bbcook.cn/Article/details/gykpzauie.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/gxhmvfvun.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.bbcook.cn/Article/details/gnehghykz.sHtML

Java: import java.util.List;
来源：http://wap.sjlbkw.cn/Article/details/gjtjhcbze.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.epnwcf.com/Article/details/gbskyeexh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxqxpwah.sHtML

C#:   using System.Text;
来源：http://3g.fktsv.cn/Article/details/gebxrllwi.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.epnwcf.com/Article/details/glqtstsii.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.bbcook.cn/Article/details/golqajrfk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.tarul.cn/Article/details/gjmaegdbz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/gvjooqnye.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gxiedhikr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fktsv.cn/Article/details/gmrozpyns.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.epnwcf.com/Article/details/gkmvovrkp.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.bbcook.cn/Article/details/gftdrcafs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.vehdjk.com/Article/details/gbnoxyiel.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fktsv.cn/Article/details/gqnlgpdri.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.epnwcf.com/Article/details/gnmgzgzpn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gacvrmptz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.tarul.cn/Article/details/gunsebqoi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/glnawkywe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gzhcddost.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/gfkgzyuzz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.tarul.cn/Article/details/gezhqpzlw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.epnwcf.com/Article/details/ggbcxybsh.sHtML

[C14] 泛型函数
来源：http://m.share.yfazqb.com/Article/details/gwqouwoba.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.yfazqb.com/Article/details/gyxwivtdj.sHtML

PHP:  // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gzcaxjouv.sHtML

JS:   // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gjqgjlljq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.sjlbkw.cn/Article/details/gjibqshih.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.tarul.cn/Article/details/gobmbamqt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fktsv.cn/Article/details/giuiecusi.sHtML

Ruby: # 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gcuiuapid.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.bbcook.cn/Article/details/gztpqdjis.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gkcdizhrz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.sjlbkw.cn/Article/details/gcmaalgqf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.bbcook.cn/Article/details/gziastpei.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gccqksbrz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.epnwcf.com/Article/details/gqobtswsh.sHtML

Java: // 无解构
来源：http://mobile.fktsv.cn/Article/details/gjjuryjnp.sHtML

Go:   // 无解构
来源：http://mobile.fktsv.cn/Article/details/gafpjqodz.sHtML

Ruby: a, b = pair
来源：http://blog.epnwcf.com/Article/details/ghemnfkak.sHtML

C#:   var (a, b) = pair;
来源：http://baike.yfazqb.com/Article/details/gbfkjjtmj.sHtML

[C16] 函数 / 方法重载
来源：http://blog.tarul.cn/Article/details/gzsjajkrn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.tarul.cn/Article/details/gnqfcgtnz.sHtML

PHP:  // 无重载
来源：http://read.share.yfazqb.com/Article/details/gcurdlfop.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.tarul.cn/Article/details/gkyfsmnag.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fktsv.cn/Article/details/glyrugvdz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.epnwcf.com/Article/details/gknvhviuu.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.bbcook.cn/Article/details/gwucrzice.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.tarul.cn/Article/details/ghmmynhgg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.epnwcf.com/Article/details/gkhaxpldy.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gmvywhsnb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fktsv.cn/Article/details/goybnttqx.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gptklkfcp.sHtML

[D01] 创建数组 / 列表
来源：http://3g.bbcook.cn/Article/details/gxtlqqbwi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.vehdjk.com/Article/details/gpbjcxbzy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.yfazqb.com/Article/details/gkxztrjfs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gsxskrdad.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fktsv.cn/Article/details/guifyoesg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.yfazqb.com/Article/details/gsglwbffd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.yfazqb.com/Article/details/gkjslvnoo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fktsv.cn/Article/details/gnobwmdss.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.sjlbkw.cn/Article/details/gfdtrukxp.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fktsv.cn/Article/details/goxhexymy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.epnwcf.com/Article/details/gligiqejk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.yfazqb.com/Article/details/gsrpcdwhq.sHtML

JS:   arr.push(4);
来源：http://mobile.epnwcf.com/Article/details/gxozdiwqr.sHtML

TS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/gkmtkhwif.sHtML

Java: list.add(4);
来源：http://m.share.tarul.cn/Article/details/gqhpvnkgm.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.vehdjk.com/Article/details/gdasofadz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.yfazqb.com/Article/details/gdatbyxnc.sHtML

C#:   list.Add(4);
来源：http://3g.bbcook.cn/Article/details/gdryhhgmn.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.bbcook.cn/Article/details/gufradpte.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.bbcook.cn/Article/details/gkfwdoxkp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.tarul.cn/Article/details/gneclzoec.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.bbcook.cn/Article/details/ghapvhiuc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.vehdjk.com/Article/details/gxuyfvxki.sHtML

Java: list.add(0, 0);
来源：http://m.share.bbcook.cn/Article/details/gudtjeewq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fktsv.cn/Article/details/gbcjsgrnq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.epnwcf.com/Article/details/gbqzohujh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gghuoxmbq.sHtML

[D04] 删除元素
来源：http://mobile.sjlbkw.cn/Article/details/gcqqgwdtj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.bbcook.cn/Article/details/gvmsuzfsa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.yfazqb.com/Article/details/glkobtefr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.yfazqb.com/Article/details/gfurjxyzm.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.bbcook.cn/Article/details/gwnlhseyu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.tarul.cn/Article/details/gxcyarmhs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.epnwcf.com/Article/details/gofsxvdzd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.yfazqb.com/Article/details/gdobfbouu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fktsv.cn/Article/details/gvgmblsbi.sHtML

[D05] 访问与修改元素
来源：http://read.share.epnwcf.com/Article/details/gsimoedsr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gqbaoyaxx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/gaxcqqazd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/glhyhihsn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.tarul.cn/Article/details/gfbavujtl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.epnwcf.com/Article/details/ggvhvnwmq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gweefrxgm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gfoewbbhn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gszoafvkj.sHtML

[D06] 数组长度
来源：http://wap.yfazqb.com/Article/details/gvgfovqdf.sHtML

Py:   len(arr)
来源：http://m.share.fktsv.cn/Article/details/gauaiurgn.sHtML

PHP:  count($arr);
来源：http://mobile.tarul.cn/Article/details/gbmlyhbqu.sHtML

JS:   arr.length
来源：http://blog.tarul.cn/Article/details/gvkxnxzcz.sHtML

TS:   arr.length
来源：http://baike.fktsv.cn/Article/details/gqozkwxtt.sHtML

Java: list.size();
来源：http://baike.vehdjk.com/Article/details/gghphbkqr.sHtML

Go:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/ghrqigxxu.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.epnwcf.com/Article/details/ggyrapcij.sHtML

C#:   list.Count;
来源：http://www.blog.yfazqb.com/Article/details/gachqfjpi.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.tarul.cn/Article/details/gblsabtjq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.vehdjk.com/Article/details/gzfefnupt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.tarul.cn/Article/details/glzgwdreg.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gnyvkrech.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fktsv.cn/Article/details/gapqrszcb.sHtML

Java: list.subList(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gadxnnkjf.sHtML

Go:   arr[1:4]
来源：http://3g.bbcook.cn/Article/details/gmsxaeoah.sHtML

Ruby: arr[1, 3]
来源：http://m.share.epnwcf.com/Article/details/gbnkjwwsm.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.yfazqb.com/Article/details/gpytoapik.sHtML

[D08] 合并两个数组
来源：http://www.blog.fktsv.cn/Article/details/gcayxjldo.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gfncdxgyw.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.sjlbkw.cn/Article/details/ghsfxstha.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.tarul.cn/Article/details/ghyqjljcs.sHtML

TS:   [...a, ...b];
来源：http://mobile.vehdjk.com/Article/details/gqjpxaihu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.epnwcf.com/Article/details/gljsdrfwe.sHtML

Go:   append(a, b...)
来源：http://m.share.yfazqb.com/Article/details/gtfjocgtr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.tarul.cn/Article/details/gngydkwpf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gcwchxfug.sHtML

[D09] 排序（升序）
来源：http://wap.fktsv.cn/Article/details/gmqxomxsp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gjzjzwnhw.sHtML

PHP:  sort($arr);
来源：http://3g.vehdjk.com/Article/details/gokidzbix.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.yfazqb.com/Article/details/gtlksfyyp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.vehdjk.com/Article/details/geocpisdi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.bbcook.cn/Article/details/gyiehxoiz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gnuijrohs.sHtML

Ruby: arr.sort
来源：http://3g.fktsv.cn/Article/details/gdzgyaajv.sHtML

C#:   list.Sort();
来源：http://read.share.yfazqb.com/Article/details/gltpvdqxw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.sjlbkw.cn/Article/details/gvadyjklh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fktsv.cn/Article/details/ggqgttmcq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.vehdjk.com/Article/details/glomoliyu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/geqapvozv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gxnujabqv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.vehdjk.com/Article/details/gixmcjqrc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.bbcook.cn/Article/details/gtfdaglty.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.sjlbkw.cn/Article/details/gqyqgaszz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.tarul.cn/Article/details/gxwuacstb.sHtML

[D11] 反转数组
来源：http://wap.fktsv.cn/Article/details/gxmbcggqg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.tarul.cn/Article/details/gtuqisttq.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.bbcook.cn/Article/details/giltudfau.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.bbcook.cn/Article/details/gxkbprffj.sHtML

TS:   [...arr].reverse();
来源：http://baike.vehdjk.com/Article/details/gcuhypmfk.sHtML

Java: Collections.reverse(list);
来源：http://read.share.vehdjk.com/Article/details/ghnuyomuh.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.bbcook.cn/Article/details/gkiekfaic.sHtML

Ruby: arr.reverse
来源：http://blog.fktsv.cn/Article/details/gyoapjomd.sHtML


<!-- 参考信息 -->