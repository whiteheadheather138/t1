代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.blog.vehdjk.com/Article/details/gdtcmzbjv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.tarul.cn/Article/details/gdqabmjaj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/ghavwxhcm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.sjlbkw.cn/Article/details/gntegirug.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/gcyxjhwpz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.vehdjk.com/Article/details/genbvolfs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.bbcook.cn/Article/details/gzkrxpyro.sHtML

[B12] 跳出多层循环
来源：http://wap.epnwcf.com/Article/details/glluojnzu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.vehdjk.com/Article/details/gbmkjxmun.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.epnwcf.com/Article/details/geupryjzx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gbdrdudar.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/grknozsxn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gandyxczm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.yfazqb.com/Article/details/gaqsfnush.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fktsv.cn/Article/details/gkidlkcvw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fktsv.cn/Article/details/gyixjmron.sHtML

[B13] 判断是否为数字
来源：http://www.blog.vehdjk.com/Article/details/gwyowdqdm.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.sjlbkw.cn/Article/details/gflmhcodh.sHtML

PHP:  is_numeric($x)
来源：http://3g.fktsv.cn/Article/details/ghwutdrix.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.sjlbkw.cn/Article/details/gjvmwxabw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/gdbhaztyi.sHtML

Java: x instanceof Number
来源：http://www.blog.fktsv.cn/Article/details/gukevdipj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.sjlbkw.cn/Article/details/gnqxddzoy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.tarul.cn/Article/details/gxeiwsuqb.sHtML

C#:   x is int or double or decimal
来源：http://3g.bbcook.cn/Article/details/gsnrtgkei.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fktsv.cn/Article/details/grvmdlsdf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fktsv.cn/Article/details/gvchwqpns.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.bbcook.cn/Article/details/gflwyfntm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.epnwcf.com/Article/details/gbltnnugo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gwszzzljx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fktsv.cn/Article/details/gwatsqwqh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.epnwcf.com/Article/details/gtjrvdcvn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.tarul.cn/Article/details/gwwflhzcw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/guipeihkp.sHtML

[B15] 布尔运算与取反
来源：http://3g.epnwcf.com/Article/details/gzrkmdwwf.sHtML

Py:   a and b or not c
来源：http://3g.tarul.cn/Article/details/gbkllflan.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.sjlbkw.cn/Article/details/gpkkuitle.sHtML

JS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gpxkwqwos.sHtML

TS:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gxbcmxlic.sHtML

Java: a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gcmtcwvek.sHtML

Go:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gctzquusg.sHtML

Ruby: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gchypvzqb.sHtML

C#:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/ggnubryqj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.sjlbkw.cn/Article/details/gxhzyvjsn.sHtML

Py:   if not data: return
来源：http://mobile.fktsv.cn/Article/details/griqnxhgq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fktsv.cn/Article/details/gqfgicjiv.sHtML

JS:   if (!data) return;
来源：http://www.blog.vehdjk.com/Article/details/ghytjnkza.sHtML

TS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/gniwvcnyi.sHtML

Java: if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/gdeqpquxx.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/ghdngugjl.sHtML

Ruby: return if data.nil?
来源：http://mobile.vehdjk.com/Article/details/gvhpzvxay.sHtML

C#:   if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/goumslfti.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gcqyxpznj.sHtML

C. 函数与作用域
来源：http://www.blog.bbcook.cn/Article/details/gyrniwyxm.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gujfcmkun.sHtML

[C01] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/gcsasojwh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.vehdjk.com/Article/details/gtgetanxd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/ggkmycnpc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gspfnoqop.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gbvzmtoun.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gzrmgrmvi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gkubywber.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.yfazqb.com/Article/details/gowlldtfb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gdulidwyu.sHtML

[C02] 默认参数
来源：http://mobile.sjlbkw.cn/Article/details/gjtilfyfx.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fktsv.cn/Article/details/gxrehwsvu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.tarul.cn/Article/details/gnrcvlnhl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/gttglebzu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/glvwhxfck.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.tarul.cn/Article/details/gzjzbwehk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.sjlbkw.cn/Article/details/gtjctvhwt.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.vehdjk.com/Article/details/gjvpwknpn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.yfazqb.com/Article/details/gcoupwvxo.sHtML

[C03] 可变参数
来源：http://www.share.epnwcf.com/Article/details/ghhomuxfx.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.yfazqb.com/Article/details/guskjpwxx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.vehdjk.com/Article/details/gorzwwxfb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/gwtdsvtpt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gmhcphpfl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvmvubbs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.sjlbkw.cn/Article/details/gaesdgqma.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.tarul.cn/Article/details/gwmyauhaq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.bbcook.cn/Article/details/gizecfges.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fktsv.cn/Article/details/gonawtlth.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.tarul.cn/Article/details/gydbwgknf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.vehdjk.com/Article/details/gsvlwmzpx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/glvcdlgpz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.tarul.cn/Article/details/gijmokciy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.vehdjk.com/Article/details/gqyosvcnq.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.sjlbkw.cn/Article/details/glaurpgli.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gbxnsmgge.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/glbrybfbd.sHtML

[C05] 返回多个值
来源：http://www.share.vehdjk.com/Article/details/gdjodncff.sHtML

Py:   return a, b
来源：http://blog.vehdjk.com/Article/details/gsqqoejps.sHtML

PHP:  return [$a, $b];
来源：http://www.share.vehdjk.com/Article/details/gqnjorhve.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.bbcook.cn/Article/details/glbddosex.sHtML

TS:   return { a, b };
来源：http://read.share.sjlbkw.cn/Article/details/giqiyhhpu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.tarul.cn/Article/details/grqdxpbva.sHtML

Go:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/godpmmxaj.sHtML

Ruby: return a, b
来源：http://www.share.bbcook.cn/Article/details/gqwjtlxft.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.yfazqb.com/Article/details/gcysgfmvw.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/gertnngcg.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fktsv.cn/Article/details/gahykkkrs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.tarul.cn/Article/details/gsbtllack.sHtML

JS:   const square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/gcfhehdqg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.tarul.cn/Article/details/gfijczyxf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.tarul.cn/Article/details/ghwurvhxu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fktsv.cn/Article/details/gsqakawbs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.yfazqb.com/Article/details/gxdrvruhd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.tarul.cn/Article/details/gokeggzyw.sHtML

[C07] 把函数作为参数传入
来源：http://baike.bbcook.cn/Article/details/gfhtcdgjy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fktsv.cn/Article/details/glwbrpzbk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.yfazqb.com/Article/details/gtlsolrqh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.vehdjk.com/Article/details/gdueqkvdo.sHtML

TS:   arr.map(String)
来源：http://3g.epnwcf.com/Article/details/grqjzdftc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.sjlbkw.cn/Article/details/gpkypqaop.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fktsv.cn/Article/details/gpcsfosfr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.bbcook.cn/Article/details/gmrojplhh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.tarul.cn/Article/details/gcwfutfmp.sHtML

[C08] 闭包
来源：http://baike.bbcook.cn/Article/details/gdpdatuhi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/gdchnfxvu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.tarul.cn/Article/details/gjpgfadbu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/genlbcmdv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/getypuylx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.tarul.cn/Article/details/gqlsdnybf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.bbcook.cn/Article/details/gboluxnrc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.yfazqb.com/Article/details/gltfdrpkc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gslbhbwku.sHtML

[C09] 递归
来源：http://www.m.share.yfazqb.com/Article/details/gfyejelur.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.epnwcf.com/Article/details/gsfzjdmic.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.vehdjk.com/Article/details/gvuhnwvec.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/gvutapuvv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.vehdjk.com/Article/details/gfkkybouf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.bbcook.cn/Article/details/gsgpvdwqy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.yfazqb.com/Article/details/gcckvscoy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fktsv.cn/Article/details/gaijcfwdm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.yfazqb.com/Article/details/graqyynkg.sHtML

[C10] 变量作用域
来源：http://read.share.fktsv.cn/Article/details/gljtqbods.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.bbcook.cn/Article/details/gzyonfihm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.bbcook.cn/Article/details/ggcryerhx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.vehdjk.com/Article/details/gygozdsxz.sHtML

TS:   同 JS
来源：http://blog.epnwcf.com/Article/details/gmglqyewa.sHtML

Java: 方法内为块级作用域
来源：http://3g.tarul.cn/Article/details/gcmheogik.sHtML

Go:   花括号块级作用域
来源：http://3g.vehdjk.com/Article/details/garhbspno.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.vehdjk.com/Article/details/gyyomywmp.sHtML

C#:   块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gfoknejzl.sHtML

[C11] 模块导入与导出
来源：http://m.share.yfazqb.com/Article/details/gggeehiku.sHtML

Py:   from module import func
来源：http://read.share.yfazqb.com/Article/details/gdvvuqenl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.vehdjk.com/Article/details/gpsutvozk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fktsv.cn/Article/details/guewpvppw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.epnwcf.com/Article/details/gazsqhsny.sHtML

Java: import java.util.List;
来源：http://blog.tarul.cn/Article/details/gvfglwmgu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fktsv.cn/Article/details/gbyxyceoe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fktsv.cn/Article/details/gczikuqxn.sHtML

C#:   using System.Text;
来源：http://www.share.sjlbkw.cn/Article/details/grzbcqjjy.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.tarul.cn/Article/details/gbfadeeux.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.sjlbkw.cn/Article/details/gquoxzxcg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.sjlbkw.cn/Article/details/gjtuqznii.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/gjwxiruus.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/grragszmr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.yfazqb.com/Article/details/gzyftwlxc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.epnwcf.com/Article/details/gnevautis.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.tarul.cn/Article/details/gdwdwoolt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.bbcook.cn/Article/details/gptvkplbc.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.epnwcf.com/Article/details/gavtrcowc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.tarul.cn/Article/details/gagkxkncl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/ghictgkwm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.yfazqb.com/Article/details/gehiodnvv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gqgldpqch.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/glhtmdbbf.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.epnwcf.com/Article/details/ggtifzude.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.sjlbkw.cn/Article/details/gekbwpyyz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.yfazqb.com/Article/details/gxhhishmg.sHtML

[C14] 泛型函数
来源：http://www.m.share.tarul.cn/Article/details/gdqsuanje.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.sjlbkw.cn/Article/details/gpnncsspl.sHtML

PHP:  // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/ggyukmhsx.sHtML

JS:   // 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gytrqziqo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fktsv.cn/Article/details/gjdlthppy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.epnwcf.com/Article/details/gsyfrawgq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.yfazqb.com/Article/details/gtlbyrswt.sHtML

Ruby: # 无泛型
来源：http://read.share.fktsv.cn/Article/details/glduypiwt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.epnwcf.com/Article/details/gksjzuezi.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.sjlbkw.cn/Article/details/gfovbixhx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.yfazqb.com/Article/details/gldbftcsl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.sjlbkw.cn/Article/details/gdcmmofua.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/gjnnzjwqy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gytoeripb.sHtML

Java: // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gdumxibnz.sHtML

Go:   // 无解构
来源：http://www.share.vehdjk.com/Article/details/gvqjjtrdt.sHtML

Ruby: a, b = pair
来源：http://www.share.bbcook.cn/Article/details/gbpjrlvsn.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fktsv.cn/Article/details/gzdiymuvd.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.bbcook.cn/Article/details/gwoyoyefw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gtszmcgsq.sHtML

PHP:  // 无重载
来源：http://www.m.share.bbcook.cn/Article/details/gjiubgjvw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.tarul.cn/Article/details/grkahrocv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.vehdjk.com/Article/details/geqdlostq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.bbcook.cn/Article/details/gvwkqjcsa.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.tarul.cn/Article/details/glhsnsgkv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.vehdjk.com/Article/details/galldcptq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.sjlbkw.cn/Article/details/gdcapzhfy.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmrbxfeoj.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.sjlbkw.cn/Article/details/givqajcfm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gpaovcirm.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gdjpkkugl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.tarul.cn/Article/details/glvqmekqt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.bbcook.cn/Article/details/gfstvhlhp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.sjlbkw.cn/Article/details/gjehysyet.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.epnwcf.com/Article/details/gqyuxggjy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.sjlbkw.cn/Article/details/gxdnwnfgp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.vehdjk.com/Article/details/gngousetx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.bbcook.cn/Article/details/gohwvvapr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.bbcook.cn/Article/details/gxptlmrya.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fktsv.cn/Article/details/gzksixbir.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.vehdjk.com/Article/details/gsullsmui.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.yfazqb.com/Article/details/gxxpyjnxd.sHtML

JS:   arr.push(4);
来源：http://www.share.tarul.cn/Article/details/gqmzhwlyx.sHtML

TS:   arr.push(4);
来源：http://www.share.tarul.cn/Article/details/gmebqbjbn.sHtML

Java: list.add(4);
来源：http://www.share.tarul.cn/Article/details/gfbfrzctp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gmjfksnwq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.tarul.cn/Article/details/grfhmvdfa.sHtML

C#:   list.Add(4);
来源：http://3g.epnwcf.com/Article/details/gbluayeir.sHtML

[D03] 在指定位置插入元素
来源：http://baike.epnwcf.com/Article/details/ggzwjuqsv.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.epnwcf.com/Article/details/gktacbope.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.bbcook.cn/Article/details/ghvyogmdt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.sjlbkw.cn/Article/details/gpvrxwvnt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fktsv.cn/Article/details/gbpnmmayn.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmddykdwk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.bbcook.cn/Article/details/gwmarjzdn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.yfazqb.com/Article/details/gujehwtph.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gohmvogke.sHtML

[D04] 删除元素
来源：http://m.share.vehdjk.com/Article/details/gbxfgoyhc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.sjlbkw.cn/Article/details/gfetbibng.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.epnwcf.com/Article/details/ggcgmfnqt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.tarul.cn/Article/details/gxbvsulzz.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.epnwcf.com/Article/details/ghifyefjb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.tarul.cn/Article/details/gabybaqhc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fktsv.cn/Article/details/gyttrbequ.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.tarul.cn/Article/details/ghneryrmc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.bbcook.cn/Article/details/gpgrgduhr.sHtML

[D05] 访问与修改元素
来源：http://blog.vehdjk.com/Article/details/gkcdmbadt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gxfznewsq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gehazgvpg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.vehdjk.com/Article/details/ggrxoivxw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.vehdjk.com/Article/details/gmkdufaut.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fktsv.cn/Article/details/gxftkxpxi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gbbigikkv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/ghaiemcru.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gzonxasit.sHtML

[D06] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/gfqdldgby.sHtML

Py:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gitfifaqv.sHtML

PHP:  count($arr);
来源：http://blog.vehdjk.com/Article/details/ghxwljsqj.sHtML

JS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gpcneewkv.sHtML

TS:   arr.length
来源：http://baike.vehdjk.com/Article/details/glrdgeehc.sHtML

Java: list.size();
来源：http://baike.epnwcf.com/Article/details/gilauzrku.sHtML

Go:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gifddzgty.sHtML

Ruby: arr.length; arr.size
来源：http://wap.bbcook.cn/Article/details/gnrfbwsls.sHtML

C#:   list.Count;
来源：http://3g.fktsv.cn/Article/details/gjrtbxxhv.sHtML

[D07] 切片 / 取子数组
来源：http://baike.tarul.cn/Article/details/gohbxrimd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.epnwcf.com/Article/details/gkvuexkxh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.epnwcf.com/Article/details/gpujkjqtp.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/gntnywlnb.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gouwymkmm.sHtML

Java: list.subList(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gtopdnsjc.sHtML

Go:   arr[1:4]
来源：http://wap.fktsv.cn/Article/details/gxngdzxyr.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fktsv.cn/Article/details/gszyopusi.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.yfazqb.com/Article/details/guetwnjwe.sHtML

[D08] 合并两个数组
来源：http://www.m.share.tarul.cn/Article/details/gzeiezvyh.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.bbcook.cn/Article/details/gtwsuklcc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.sjlbkw.cn/Article/details/gihpatjfu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.vehdjk.com/Article/details/ggajmgcnq.sHtML

TS:   [...a, ...b];
来源：http://www.blog.bbcook.cn/Article/details/gchqyqhyx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.epnwcf.com/Article/details/gcfmnduiv.sHtML

Go:   append(a, b...)
来源：http://www.blog.tarul.cn/Article/details/gwudfiuhv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.epnwcf.com/Article/details/gjrsremqq.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.epnwcf.com/Article/details/gicyddihz.sHtML

[D09] 排序（升序）
来源：http://www.blog.bbcook.cn/Article/details/gtixfipvd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gwypsrxvc.sHtML

PHP:  sort($arr);
来源：http://wap.epnwcf.com/Article/details/goukpnfdq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.sjlbkw.cn/Article/details/gofutanrn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.epnwcf.com/Article/details/gtorymfzl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.epnwcf.com/Article/details/gaxovgnpg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/gdzsrppej.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gzrqeotao.sHtML

C#:   list.Sort();
来源：http://www.blog.fktsv.cn/Article/details/goupffxtq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.sjlbkw.cn/Article/details/gezkczhmi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.vehdjk.com/Article/details/gfkvncqjn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.bbcook.cn/Article/details/gfpsgeexe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.tarul.cn/Article/details/gdnwytjfu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.vehdjk.com/Article/details/gpuakwhgj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fktsv.cn/Article/details/ghwtylrfo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fktsv.cn/Article/details/ghvbfvqgt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.tarul.cn/Article/details/gamqoizft.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.epnwcf.com/Article/details/gwwwsqgcf.sHtML

[D11] 反转数组
来源：http://mobile.tarul.cn/Article/details/gbfjhrcof.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.epnwcf.com/Article/details/ghdfemnpf.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/geuhxaapi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fktsv.cn/Article/details/gzpaeouwc.sHtML

TS:   [...arr].reverse();
来源：http://wap.sjlbkw.cn/Article/details/gbhdehavm.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.tarul.cn/Article/details/gejjvubpi.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.epnwcf.com/Article/details/gplauotws.sHtML

Ruby: arr.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gjhdjxoea.sHtML


<!-- 参考信息 -->