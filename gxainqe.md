代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.vehdjk.com/Article/details/gvemjsxao.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.bbcook.cn/Article/details/gsbervubr.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.sjlbkw.cn/Article/details/gekiteowi.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fktsv.cn/Article/details/gdlkylldi.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fktsv.cn/Article/details/gdotoyclb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.yfazqb.com/Article/details/gaclcdgrs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/gemtdhdjm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.tarul.cn/Article/details/gtxngyqqn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.bbcook.cn/Article/details/gwczczrbz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.epnwcf.com/Article/details/gaayiphtw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.tarul.cn/Article/details/gyesrvddm.sHtML

[B12] 跳出多层循环
来源：http://read.share.sjlbkw.cn/Article/details/gtswwgxgv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fktsv.cn/Article/details/gxsnqdydl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.sjlbkw.cn/Article/details/ginerostb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gaymgsqbv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/gopuwewxc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gjrzoxunk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.bbcook.cn/Article/details/gnombtyoy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/gkywvdcuf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/geefdbbwr.sHtML

[B13] 判断是否为数字
来源：http://mobile.yfazqb.com/Article/details/gxjoltixp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fktsv.cn/Article/details/gnxswfcxh.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.bbcook.cn/Article/details/gpvhgzfbr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.yfazqb.com/Article/details/gicgthjgo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.vehdjk.com/Article/details/gjcecpnbl.sHtML

Java: x instanceof Number
来源：http://mobile.vehdjk.com/Article/details/gitslazsy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.tarul.cn/Article/details/ggfdniwqk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.sjlbkw.cn/Article/details/gokvpirzs.sHtML

C#:   x is int or double or decimal
来源：http://read.share.vehdjk.com/Article/details/gjsojewnv.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.yfazqb.com/Article/details/gyuniogid.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.yfazqb.com/Article/details/gxqxqedyx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.sjlbkw.cn/Article/details/gxwvosuyr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fktsv.cn/Article/details/gqflqfowz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.bbcook.cn/Article/details/grpdldvmg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.tarul.cn/Article/details/gsemgzpuw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.yfazqb.com/Article/details/gskzismwy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.bbcook.cn/Article/details/ghvarehoc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.vehdjk.com/Article/details/gpywavubi.sHtML

[B15] 布尔运算与取反
来源：http://baike.fktsv.cn/Article/details/gpnspweqn.sHtML

Py:   a and b or not c
来源：http://read.share.sjlbkw.cn/Article/details/guheurdkl.sHtML

PHP:  $a && $b || !$c
来源：http://blog.sjlbkw.cn/Article/details/gerkwmhjj.sHtML

JS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gpxjnentg.sHtML

TS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gpsfrzutl.sHtML

Java: a && b || !c
来源：http://mobile.bbcook.cn/Article/details/ghxetzioq.sHtML

Go:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gmsnptybl.sHtML

Ruby: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gpvgeizej.sHtML

C#:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/glxpgphtm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fktsv.cn/Article/details/ghpbeagvi.sHtML

Py:   if not data: return
来源：http://wap.bbcook.cn/Article/details/gnewqegyv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.tarul.cn/Article/details/gjuhxizfz.sHtML

JS:   if (!data) return;
来源：http://3g.sjlbkw.cn/Article/details/ggjcypoqt.sHtML

TS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gzakobysl.sHtML

Java: if (data == null) return;
来源：http://baike.yfazqb.com/Article/details/gaabsrqzm.sHtML

Go:   if data == nil { return }
来源：http://m.share.fktsv.cn/Article/details/giriinfgy.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.epnwcf.com/Article/details/gtltdmidq.sHtML

C#:   if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gpcdeqorq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/goaawsdwj.sHtML

C. 函数与作用域
来源：http://m.share.fktsv.cn/Article/details/gxaczqpdi.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/giifbvsvs.sHtML

[C01] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gcuninfyg.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/ggfjxcsiu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdmhpxnli.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gkcadhqrl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gbhmqgtfj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/glymnzqbk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gbmnzjerc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.epnwcf.com/Article/details/gdfbkhbwa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/goklbodtg.sHtML

[C02] 默认参数
来源：http://read.share.epnwcf.com/Article/details/ghmwqnnjx.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.vehdjk.com/Article/details/gjgsinbyd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.tarul.cn/Article/details/gehzpydgu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gbielkbat.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gizgezufh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.sjlbkw.cn/Article/details/gekwiltgh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gdctoyfbh.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.epnwcf.com/Article/details/ghpvaphmr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fktsv.cn/Article/details/gmguvyopb.sHtML

[C03] 可变参数
来源：http://wap.tarul.cn/Article/details/gxmbgzznj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.epnwcf.com/Article/details/gkbkdkxlm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.bbcook.cn/Article/details/guazzbuol.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.yfazqb.com/Article/details/gdhyaymmx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.sjlbkw.cn/Article/details/grdhgziqn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.epnwcf.com/Article/details/gjrbadijl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.tarul.cn/Article/details/gutjzpgdx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.tarul.cn/Article/details/guuyqcgca.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.tarul.cn/Article/details/glayyzydo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.sjlbkw.cn/Article/details/gtrxnmqji.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.sjlbkw.cn/Article/details/gtzsctocv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.yfazqb.com/Article/details/gweyjavrp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/gdrbqbhoe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.epnwcf.com/Article/details/ggkifctap.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.bbcook.cn/Article/details/geoevytbk.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.vehdjk.com/Article/details/gauyspazk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/gtplbzdkz.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gdqvlrcls.sHtML

[C05] 返回多个值
来源：http://www.share.epnwcf.com/Article/details/gummtkkot.sHtML

Py:   return a, b
来源：http://read.share.fktsv.cn/Article/details/gyxyjjmtc.sHtML

PHP:  return [$a, $b];
来源：http://baike.fktsv.cn/Article/details/gyokaavix.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.tarul.cn/Article/details/guawxucdy.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gnxtundep.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.sjlbkw.cn/Article/details/gylwzyfmm.sHtML

Go:   return a, b
来源：http://read.share.fktsv.cn/Article/details/gzlctrljb.sHtML

Ruby: return a, b
来源：http://mobile.tarul.cn/Article/details/gycnkcbde.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrrpnptr.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.epnwcf.com/Article/details/gaxxosknn.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.tarul.cn/Article/details/goyzhiakm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fktsv.cn/Article/details/gudrkdmff.sHtML

JS:   const square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/gihiitvak.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.epnwcf.com/Article/details/ggxualqol.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.vehdjk.com/Article/details/gubeuxvok.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.tarul.cn/Article/details/gvzkosxpf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.epnwcf.com/Article/details/gskxjswmk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gbdlukbha.sHtML

[C07] 把函数作为参数传入
来源：http://baike.sjlbkw.cn/Article/details/guadkvrgo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.tarul.cn/Article/details/ggvqltvgj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fktsv.cn/Article/details/gojdxgqws.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.bbcook.cn/Article/details/gzrpfjwdc.sHtML

TS:   arr.map(String)
来源：http://read.share.fktsv.cn/Article/details/gqecnfcxl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.epnwcf.com/Article/details/gaeopnexp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.sjlbkw.cn/Article/details/gqwsnpiyv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.tarul.cn/Article/details/gstkgqhsv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.bbcook.cn/Article/details/ghlkwapkw.sHtML

[C08] 闭包
来源：http://wap.bbcook.cn/Article/details/goceqkbrz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.vehdjk.com/Article/details/gflcpvjsd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fktsv.cn/Article/details/gogqcyusv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gblhsuooj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gacicbbmp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.yfazqb.com/Article/details/gdulqanka.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.yfazqb.com/Article/details/gcockwpry.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.vehdjk.com/Article/details/gonbladpp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gqzwsrxpd.sHtML

[C09] 递归
来源：http://blog.bbcook.cn/Article/details/glocowooe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gvxufumtf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.sjlbkw.cn/Article/details/gqcaapcrc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/gjvfumaxu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/ghzaowovl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.tarul.cn/Article/details/gqlyiaxgw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.epnwcf.com/Article/details/gfrkxiexf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gwfcczxid.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.vehdjk.com/Article/details/gdlqclrqg.sHtML

[C10] 变量作用域
来源：http://www.m.share.bbcook.cn/Article/details/gbqofjuga.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fktsv.cn/Article/details/gwcewfpwd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/gzcivhniq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fktsv.cn/Article/details/ggrplrhlt.sHtML

TS:   同 JS
来源：http://wap.epnwcf.com/Article/details/grjfwhivx.sHtML

Java: 方法内为块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gwqljqgia.sHtML

Go:   花括号块级作用域
来源：http://read.share.yfazqb.com/Article/details/gtbgxbxub.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.bbcook.cn/Article/details/gdqjjyqor.sHtML

C#:   块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gmecfclnj.sHtML

[C11] 模块导入与导出
来源：http://www.blog.bbcook.cn/Article/details/gvrsvbeii.sHtML

Py:   from module import func
来源：http://blog.tarul.cn/Article/details/gydrbneok.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.sjlbkw.cn/Article/details/gcdhpmull.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.vehdjk.com/Article/details/grtuixhkw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fktsv.cn/Article/details/gdhngnupw.sHtML

Java: import java.util.List;
来源：http://baike.yfazqb.com/Article/details/gwegdqboc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.epnwcf.com/Article/details/godhbvifi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/gztemfoxv.sHtML

C#:   using System.Text;
来源：http://3g.tarul.cn/Article/details/gjxayrxom.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.tarul.cn/Article/details/guirjzrkv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.epnwcf.com/Article/details/gllcfbkva.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.tarul.cn/Article/details/gtaeqgyct.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gfwtqgqfq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.bbcook.cn/Article/details/gvzpxslbt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.vehdjk.com/Article/details/gzpcjohqm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.vehdjk.com/Article/details/gqarjfchv.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.vehdjk.com/Article/details/gsmkcrqvj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gcdyejunz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.epnwcf.com/Article/details/gwnqgggep.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.epnwcf.com/Article/details/gponemztx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gzryqxmyo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.tarul.cn/Article/details/gtqcfmewn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gequdkdld.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/goqagmtxs.sHtML

Go:   func add(a, b int) int
来源：http://blog.fktsv.cn/Article/details/gvfewntie.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fktsv.cn/Article/details/gakgvhyfq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.vehdjk.com/Article/details/gtlybcyka.sHtML

[C14] 泛型函数
来源：http://www.share.epnwcf.com/Article/details/gperitlac.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.sjlbkw.cn/Article/details/gfwfchefd.sHtML

PHP:  // 无泛型
来源：http://mobile.vehdjk.com/Article/details/goihzxrej.sHtML

JS:   // 无泛型
来源：http://mobile.tarul.cn/Article/details/gijzdoxpq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.vehdjk.com/Article/details/gfdvmpbyi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.yfazqb.com/Article/details/gdgagssmk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.sjlbkw.cn/Article/details/graldwaht.sHtML

Ruby: # 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gsooyuesg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.bbcook.cn/Article/details/ghvifhxei.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.sjlbkw.cn/Article/details/gfnvlylci.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.tarul.cn/Article/details/gsucdyovs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.epnwcf.com/Article/details/gbiweswjz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/gesswhtfp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.bbcook.cn/Article/details/gsqehtpdx.sHtML

Java: // 无解构
来源：http://www.share.bbcook.cn/Article/details/goqnpxoju.sHtML

Go:   // 无解构
来源：http://read.share.fktsv.cn/Article/details/gpqmopenw.sHtML

Ruby: a, b = pair
来源：http://m.share.bbcook.cn/Article/details/gvcpudqvl.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.vehdjk.com/Article/details/gcissgbzp.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.yfazqb.com/Article/details/gokfohvza.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.tarul.cn/Article/details/gmhozreza.sHtML

PHP:  // 无重载
来源：http://m.share.tarul.cn/Article/details/geacacoma.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.yfazqb.com/Article/details/gppduyquq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.epnwcf.com/Article/details/gvqxznlvr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.bbcook.cn/Article/details/ghyhjcooc.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fktsv.cn/Article/details/gxavxbyzx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.yfazqb.com/Article/details/ggxgqwlot.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.sjlbkw.cn/Article/details/grdxaypkl.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/guqevqjqm.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fktsv.cn/Article/details/gimzouvuc.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggmfclbvn.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.bbcook.cn/Article/details/gpfobimnn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.vehdjk.com/Article/details/gzosgfyrj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.tarul.cn/Article/details/gagjjibvx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.vehdjk.com/Article/details/gmlnsedhe.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fktsv.cn/Article/details/gpscmrueh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.sjlbkw.cn/Article/details/gtwxeiird.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fktsv.cn/Article/details/gbmialofo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.epnwcf.com/Article/details/grrugecxg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.epnwcf.com/Article/details/gfxirgtbi.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fktsv.cn/Article/details/gkdtuosfb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.epnwcf.com/Article/details/gpeererlh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.sjlbkw.cn/Article/details/glputxxxe.sHtML

JS:   arr.push(4);
来源：http://baike.tarul.cn/Article/details/grjggjcrd.sHtML

TS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/gagknxbjl.sHtML

Java: list.add(4);
来源：http://3g.tarul.cn/Article/details/gvkzhwbfn.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.bbcook.cn/Article/details/gmnvezbjd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.yfazqb.com/Article/details/gkidmqdhn.sHtML

C#:   list.Add(4);
来源：http://blog.bbcook.cn/Article/details/gleengpwo.sHtML

[D03] 在指定位置插入元素
来源：http://baike.epnwcf.com/Article/details/gpziqkmhc.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.bbcook.cn/Article/details/gqwhhmeuh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.vehdjk.com/Article/details/gozmlpppp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fktsv.cn/Article/details/gwegzdxpc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gqybeqphh.sHtML

Java: list.add(0, 0);
来源：http://m.share.tarul.cn/Article/details/gojojogvd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.sjlbkw.cn/Article/details/gmcxtbzoq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.bbcook.cn/Article/details/gavedkqph.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fktsv.cn/Article/details/glyckjzsx.sHtML

[D04] 删除元素
来源：http://baike.epnwcf.com/Article/details/gkuhztdsl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.vehdjk.com/Article/details/gwfiwzlvv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gzrwgsapj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.tarul.cn/Article/details/gvyhbbspx.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.yfazqb.com/Article/details/gpntkveud.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.tarul.cn/Article/details/gwcnjcbdb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.vehdjk.com/Article/details/gfrjylefd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.yfazqb.com/Article/details/gycgtmdug.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.epnwcf.com/Article/details/gcrhhdvrk.sHtML

[D05] 访问与修改元素
来源：http://3g.fktsv.cn/Article/details/glhnxtvbf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/ghglxjpkb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/ghqhrjvlm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/glfvzpews.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.bbcook.cn/Article/details/ggebnhmqi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.vehdjk.com/Article/details/gpvdxunvm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/ggzwbnghi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/ghkqpqtoi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gzvtiqqkv.sHtML

[D06] 数组长度
来源：http://3g.epnwcf.com/Article/details/gdcbqmwtg.sHtML

Py:   len(arr)
来源：http://3g.epnwcf.com/Article/details/gwpjlzdcz.sHtML

PHP:  count($arr);
来源：http://baike.yfazqb.com/Article/details/gfptwsjsp.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gdegrsvvd.sHtML

TS:   arr.length
来源：http://baike.tarul.cn/Article/details/gyuteacea.sHtML

Java: list.size();
来源：http://www.share.vehdjk.com/Article/details/gnrsbawrj.sHtML

Go:   len(arr)
来源：http://blog.fktsv.cn/Article/details/ghbreeekb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.tarul.cn/Article/details/gniadmyvt.sHtML

C#:   list.Count;
来源：http://baike.sjlbkw.cn/Article/details/gyiyyvyvt.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.epnwcf.com/Article/details/guppglthi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.sjlbkw.cn/Article/details/gthboxuzz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fktsv.cn/Article/details/gfmqnpten.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.tarul.cn/Article/details/gfkwaomlx.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gglrumxug.sHtML

Java: list.subList(1, 4);
来源：http://baike.tarul.cn/Article/details/gkxuykiei.sHtML

Go:   arr[1:4]
来源：http://3g.sjlbkw.cn/Article/details/gbhahfosr.sHtML

Ruby: arr[1, 3]
来源：http://baike.fktsv.cn/Article/details/gmkesgfvq.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.epnwcf.com/Article/details/gzlcuwtgp.sHtML

[D08] 合并两个数组
来源：http://blog.fktsv.cn/Article/details/gsxonvspe.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.tarul.cn/Article/details/gxqosxndc.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.yfazqb.com/Article/details/gacditutd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fktsv.cn/Article/details/gwgyoevss.sHtML

TS:   [...a, ...b];
来源：http://blog.sjlbkw.cn/Article/details/guwemyjdn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fktsv.cn/Article/details/gusvbphzn.sHtML

Go:   append(a, b...)
来源：http://wap.vehdjk.com/Article/details/gpvwemkxr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fktsv.cn/Article/details/gmamuuhgt.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gcvrltwdr.sHtML

[D09] 排序（升序）
来源：http://wap.tarul.cn/Article/details/gmawkclhz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/gyztotmxc.sHtML

PHP:  sort($arr);
来源：http://m.share.yfazqb.com/Article/details/gluwdmetb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.epnwcf.com/Article/details/gkawbgwzy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.sjlbkw.cn/Article/details/gyirioxlv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.vehdjk.com/Article/details/glinohvkj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.epnwcf.com/Article/details/ghkfqkqdr.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/gyevjybgy.sHtML

C#:   list.Sort();
来源：http://www.m.share.fktsv.cn/Article/details/gqtocovzs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.sjlbkw.cn/Article/details/gfpokmbtr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.epnwcf.com/Article/details/gttplioqb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.epnwcf.com/Article/details/gtzsinxoh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fktsv.cn/Article/details/goxhqnuav.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gaxezzumu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.tarul.cn/Article/details/gxmchndgf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.vehdjk.com/Article/details/gdotsfloq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.epnwcf.com/Article/details/gmykhkvyc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.vehdjk.com/Article/details/gywbtyhnu.sHtML

[D11] 反转数组
来源：http://3g.yfazqb.com/Article/details/gdgtwkumf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.bbcook.cn/Article/details/gqpmeizgh.sHtML

PHP:  array_reverse($arr);
来源：http://wap.epnwcf.com/Article/details/gfkavudkz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.vehdjk.com/Article/details/grvtgppjk.sHtML


<!-- 参考信息 -->