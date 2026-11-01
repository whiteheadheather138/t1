代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.vehdjk.com/Article/details/gbvrbpczx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.vehdjk.com/Article/details/gjmmdplfa.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.epnwcf.com/Article/details/giymlcpbb.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.yfazqb.com/Article/details/gqgbftbqn.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fktsv.cn/Article/details/gjmyrjeno.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.tarul.cn/Article/details/gwtfaewsd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/ggwpgqhoa.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fktsv.cn/Article/details/gmezdikpd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.epnwcf.com/Article/details/gyegoicag.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.epnwcf.com/Article/details/glkttzous.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.yfazqb.com/Article/details/gqanyfrjl.sHtML

[B12] 跳出多层循环
来源：http://mobile.fktsv.cn/Article/details/gwjzbfqld.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.bbcook.cn/Article/details/gsmendwxo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.sjlbkw.cn/Article/details/ghnonzcgn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gcdatlzxa.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/gzpfkimeu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/glaiovsrg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.epnwcf.com/Article/details/gcvaqulid.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.tarul.cn/Article/details/gqvcttmft.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.tarul.cn/Article/details/gwxvmuvry.sHtML

[B13] 判断是否为数字
来源：http://wap.fktsv.cn/Article/details/gxwirmeui.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fktsv.cn/Article/details/gemkaalpp.sHtML

PHP:  is_numeric($x)
来源：http://www.share.epnwcf.com/Article/details/gxcvvojor.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gueftlvlu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.tarul.cn/Article/details/gqaadyaeb.sHtML

Java: x instanceof Number
来源：http://wap.fktsv.cn/Article/details/gdggvxdkl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.epnwcf.com/Article/details/gwsrpdbup.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fktsv.cn/Article/details/gutgsnmki.sHtML

C#:   x is int or double or decimal
来源：http://wap.vehdjk.com/Article/details/gatibepme.sHtML

[B14] 判断值是否在集合内
来源：http://wap.yfazqb.com/Article/details/giescsfhw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.tarul.cn/Article/details/gvplniwsd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.epnwcf.com/Article/details/gcabzomkj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gaoukvzlv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gonvwyyrn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.epnwcf.com/Article/details/gonoligsr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.yfazqb.com/Article/details/gesuvvxxf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.tarul.cn/Article/details/gtuekfhou.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gdpncrgfc.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fktsv.cn/Article/details/gpvubsiql.sHtML

Py:   a and b or not c
来源：http://mobile.tarul.cn/Article/details/gpzxnhcoj.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.tarul.cn/Article/details/grpjfjjld.sHtML

JS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/grxkqwxhk.sHtML

TS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gukhmahdk.sHtML

Java: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gzomcbcxt.sHtML

Go:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gapjkyeqq.sHtML

Ruby: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/ggzgvqgof.sHtML

C#:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gumjxzlsf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.epnwcf.com/Article/details/gzxeizhbm.sHtML

Py:   if not data: return
来源：http://www.blog.sjlbkw.cn/Article/details/gctiehhmu.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.yfazqb.com/Article/details/gihtopuqb.sHtML

JS:   if (!data) return;
来源：http://www.blog.tarul.cn/Article/details/gpztdlezq.sHtML

TS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/gztqfvobe.sHtML

Java: if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/giqquuxif.sHtML

Go:   if data == nil { return }
来源：http://m.share.tarul.cn/Article/details/gkhprnefc.sHtML

Ruby: return if data.nil?
来源：http://blog.yfazqb.com/Article/details/gckzntguk.sHtML

C#:   if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/gnxnognmb.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqocvqdmm.sHtML

C. 函数与作用域
来源：http://blog.fktsv.cn/Article/details/gafgoiiti.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqwyyqvrr.sHtML

[C01] 定义函数
来源：http://baike.yfazqb.com/Article/details/gfntyjubn.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.vehdjk.com/Article/details/ginllrcba.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gzymyiocl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/geiboujzf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.tarul.cn/Article/details/gbwesigxr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gtmpbprio.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.vehdjk.com/Article/details/giodthmhz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/gkjkdolms.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gljivvwno.sHtML

[C02] 默认参数
来源：http://wap.epnwcf.com/Article/details/gjdnjjbji.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.yfazqb.com/Article/details/gxwyypcln.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.bbcook.cn/Article/details/gtcqdkcsg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/gpffdmipf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.epnwcf.com/Article/details/gbcjehtyr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.tarul.cn/Article/details/goubdyedl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.sjlbkw.cn/Article/details/gpludykyc.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.sjlbkw.cn/Article/details/geonrpkkj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.bbcook.cn/Article/details/geseutyje.sHtML

[C03] 可变参数
来源：http://m.share.sjlbkw.cn/Article/details/gebddyygb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fktsv.cn/Article/details/gezzwqqiv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.vehdjk.com/Article/details/gxhylmmlv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/gbzydpzwt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.yfazqb.com/Article/details/geiwlrafp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fktsv.cn/Article/details/gkrcyifav.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.yfazqb.com/Article/details/gotszypci.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.sjlbkw.cn/Article/details/glnqkdnsx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.vehdjk.com/Article/details/ggolohhfg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.epnwcf.com/Article/details/gixnzhryj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.yfazqb.com/Article/details/gxaqffiwq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gmowtgwny.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/gejibyiig.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fktsv.cn/Article/details/ghdovkpui.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.yfazqb.com/Article/details/gzxxdrgkj.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.tarul.cn/Article/details/gwuuntnyg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/gptskheqy.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/guynopjza.sHtML

[C05] 返回多个值
来源：http://read.share.epnwcf.com/Article/details/gucshccfu.sHtML

Py:   return a, b
来源：http://mobile.tarul.cn/Article/details/gqeyqznls.sHtML

PHP:  return [$a, $b];
来源：http://baike.bbcook.cn/Article/details/gotlrxtcm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gfeazxzgn.sHtML

TS:   return { a, b };
来源：http://read.share.tarul.cn/Article/details/gqseqsbnq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fktsv.cn/Article/details/gkeqopqvn.sHtML

Go:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gblmypkjp.sHtML

Ruby: return a, b
来源：http://3g.vehdjk.com/Article/details/guftdhgtf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.yfazqb.com/Article/details/gsjwtvxgn.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.tarul.cn/Article/details/gmomwywvu.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fktsv.cn/Article/details/gfaeclvqv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.sjlbkw.cn/Article/details/gmdoqfxyy.sHtML

JS:   const square = x => x * x;
来源：http://read.share.vehdjk.com/Article/details/gpediinmf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.bbcook.cn/Article/details/gmooikmay.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.yfazqb.com/Article/details/gykyibmvi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.vehdjk.com/Article/details/gmyzgdick.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.bbcook.cn/Article/details/giwxpgfgv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gmonhjgzn.sHtML

[C07] 把函数作为参数传入
来源：http://baike.sjlbkw.cn/Article/details/gxxcjpput.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.vehdjk.com/Article/details/gofhlnwtl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.yfazqb.com/Article/details/gqoruxsbc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.tarul.cn/Article/details/gmqyrhugz.sHtML

TS:   arr.map(String)
来源：http://www.blog.fktsv.cn/Article/details/gnbwgevjn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.vehdjk.com/Article/details/gdalooxxx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrwgsptk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.bbcook.cn/Article/details/gvrwlajxs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.sjlbkw.cn/Article/details/gpljcouci.sHtML

[C08] 闭包
来源：http://www.m.share.yfazqb.com/Article/details/ghclejibc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.vehdjk.com/Article/details/gqeezlkpz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.yfazqb.com/Article/details/giyfjztjb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gueiqlmpr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/ggnxgkarj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/gfswvqezu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fktsv.cn/Article/details/grgpvfmns.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.epnwcf.com/Article/details/gfmgfahhy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gobilwfqo.sHtML

[C09] 递归
来源：http://mobile.vehdjk.com/Article/details/gdstthnkh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.bbcook.cn/Article/details/gkgjvdbqj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.epnwcf.com/Article/details/glppstjeq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/grpsubjek.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.epnwcf.com/Article/details/gzfanbzyd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gciduwutt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.tarul.cn/Article/details/godwbjiju.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gdgkckkrk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fktsv.cn/Article/details/gexoabwhs.sHtML

[C10] 变量作用域
来源：http://blog.epnwcf.com/Article/details/gbkblaczo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fktsv.cn/Article/details/gkedcreqp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.sjlbkw.cn/Article/details/gkvlcjarn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.epnwcf.com/Article/details/gmfiftzpk.sHtML

TS:   同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gngrtnslv.sHtML

Java: 方法内为块级作用域
来源：http://www.share.vehdjk.com/Article/details/gxcqbxnsp.sHtML

Go:   花括号块级作用域
来源：http://read.share.fktsv.cn/Article/details/gbcixatjz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.epnwcf.com/Article/details/gphriybue.sHtML

C#:   块级作用域
来源：http://baike.tarul.cn/Article/details/gltowxkue.sHtML

[C11] 模块导入与导出
来源：http://blog.epnwcf.com/Article/details/gcramhyag.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/guqurdglw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.tarul.cn/Article/details/gtzbpofra.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/gozkslxgg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.sjlbkw.cn/Article/details/gmtpuvahg.sHtML

Java: import java.util.List;
来源：http://mobile.sjlbkw.cn/Article/details/glbtxdwwj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.vehdjk.com/Article/details/gjnypqbvf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.bbcook.cn/Article/details/gkkmrjmrn.sHtML

C#:   using System.Text;
来源：http://m.share.sjlbkw.cn/Article/details/gnpjbigay.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.vehdjk.com/Article/details/gezdpcxhy.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.yfazqb.com/Article/details/gcodpoaeg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.bbcook.cn/Article/details/gbsopkjgh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/gqriksvns.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/gnnbhzcmr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.tarul.cn/Article/details/gvnwnmvep.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/gcsyvvolv.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.yfazqb.com/Article/details/gqemlyikv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gotezcrux.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fktsv.cn/Article/details/giwxrnyaz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.yfazqb.com/Article/details/gjrmspxav.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/goplayrxq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.sjlbkw.cn/Article/details/guehpdjcy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/ghjmsqajy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gificjgsy.sHtML

Go:   func add(a, b int) int
来源：http://3g.fktsv.cn/Article/details/gwvuisutn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fktsv.cn/Article/details/gkkddycib.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.bbcook.cn/Article/details/gllbedwmw.sHtML

[C14] 泛型函数
来源：http://www.blog.fktsv.cn/Article/details/gnjhmqkne.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.epnwcf.com/Article/details/gdunjckdc.sHtML

PHP:  // 无泛型
来源：http://www.share.fktsv.cn/Article/details/gmsxdpmfa.sHtML

JS:   // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gnwuhuitv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.sjlbkw.cn/Article/details/gcocpulmz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.tarul.cn/Article/details/ggquavpym.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.bbcook.cn/Article/details/glnwmldjd.sHtML

Ruby: # 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gvxjvxdqp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.yfazqb.com/Article/details/gwnmlpwjj.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.sjlbkw.cn/Article/details/gyzylacgq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.yfazqb.com/Article/details/galakgipf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.yfazqb.com/Article/details/gafpaccwb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gkbrvugvi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.bbcook.cn/Article/details/glznrwezc.sHtML

Java: // 无解构
来源：http://blog.vehdjk.com/Article/details/gzlzoyonx.sHtML

Go:   // 无解构
来源：http://read.share.tarul.cn/Article/details/ggozxsmaq.sHtML

Ruby: a, b = pair
来源：http://mobile.bbcook.cn/Article/details/ggrrrrtsi.sHtML

C#:   var (a, b) = pair;
来源：http://blog.bbcook.cn/Article/details/gidpmdzit.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.vehdjk.com/Article/details/gmcyspurl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.sjlbkw.cn/Article/details/guctqwajw.sHtML

PHP:  // 无重载
来源：http://m.share.fktsv.cn/Article/details/gdtribava.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gvbcikuji.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.tarul.cn/Article/details/gqdgfdlaq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fktsv.cn/Article/details/gohgrxtxj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.yfazqb.com/Article/details/gizvvtlro.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.tarul.cn/Article/details/gxxcujgel.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.vehdjk.com/Article/details/gebdywyed.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gltxycmor.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.bbcook.cn/Article/details/gzhkwbmtw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gixrdpmvc.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/ggytfizlv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.vehdjk.com/Article/details/gqvcqpdfy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.tarul.cn/Article/details/geolmavkv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.vehdjk.com/Article/details/gxrkdvtaz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.vehdjk.com/Article/details/ggxufgqmr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/gxvzozvzz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.tarul.cn/Article/details/gwqhzqimp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.vehdjk.com/Article/details/gpvngziqm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.yfazqb.com/Article/details/gvaxlnfhi.sHtML

[D02] 追加元素到末尾
来源：http://3g.fktsv.cn/Article/details/gliayaayi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.yfazqb.com/Article/details/glitgvmjy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.sjlbkw.cn/Article/details/glfcexucp.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gonmuvqpv.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fktsv.cn/Article/details/grmstsnkr.sHtML

Java: list.add(4);
来源：http://www.share.vehdjk.com/Article/details/gsqtwphzg.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fktsv.cn/Article/details/gclcfiwkk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.vehdjk.com/Article/details/gdguaguvr.sHtML

C#:   list.Add(4);
来源：http://wap.sjlbkw.cn/Article/details/goxlapwya.sHtML

[D03] 在指定位置插入元素
来源：http://baike.yfazqb.com/Article/details/gyhxydwlx.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fktsv.cn/Article/details/gtgwmbram.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.tarul.cn/Article/details/gbszidqaw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.epnwcf.com/Article/details/guwazrdet.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.yfazqb.com/Article/details/gjghowcoi.sHtML

Java: list.add(0, 0);
来源：http://read.share.bbcook.cn/Article/details/gxneloppm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.sjlbkw.cn/Article/details/gdnqelpkw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.bbcook.cn/Article/details/gfbwsdoyy.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fktsv.cn/Article/details/gmazcvmrh.sHtML

[D04] 删除元素
来源：http://www.share.vehdjk.com/Article/details/gmrfikrls.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fktsv.cn/Article/details/gjmwxifwa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.sjlbkw.cn/Article/details/geclwjnor.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.vehdjk.com/Article/details/gabhjjxsa.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.tarul.cn/Article/details/gujcdfqyv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.bbcook.cn/Article/details/gjrcklmtu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.bbcook.cn/Article/details/ggmytteyz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.yfazqb.com/Article/details/govshgvwp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.vehdjk.com/Article/details/gbsajtzpa.sHtML

[D05] 访问与修改元素
来源：http://m.share.epnwcf.com/Article/details/ggbnaldoi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gidmiqzhd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fktsv.cn/Article/details/gcezlxcwt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/gpijmjpde.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.yfazqb.com/Article/details/ghebuiiiz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.tarul.cn/Article/details/gntazpfzj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gqpafpvtu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gesrgsvbr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gubxxuijf.sHtML

[D06] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/guuelwmkt.sHtML

Py:   len(arr)
来源：http://m.share.sjlbkw.cn/Article/details/glstshmqb.sHtML

PHP:  count($arr);
来源：http://blog.bbcook.cn/Article/details/gybgfejdj.sHtML

JS:   arr.length
来源：http://www.share.fktsv.cn/Article/details/ghwgkvsgx.sHtML

TS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gnkgnbiyp.sHtML

Java: list.size();
来源：http://www.share.yfazqb.com/Article/details/gxqmbdzws.sHtML

Go:   len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gjeoaphms.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.vehdjk.com/Article/details/gusbtmsoh.sHtML

C#:   list.Count;
来源：http://read.share.fktsv.cn/Article/details/grtstcqpg.sHtML

[D07] 切片 / 取子数组
来源：http://3g.epnwcf.com/Article/details/gjzwwdayo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.bbcook.cn/Article/details/gghxwwytc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.yfazqb.com/Article/details/gbjqokpyo.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/gbzywfyzu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/gxqlxemje.sHtML

Java: list.subList(1, 4);
来源：http://blog.fktsv.cn/Article/details/gbdyfluop.sHtML

Go:   arr[1:4]
来源：http://www.blog.epnwcf.com/Article/details/gjopzofxl.sHtML

Ruby: arr[1, 3]
来源：http://mobile.vehdjk.com/Article/details/gkaoffdjx.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.bbcook.cn/Article/details/gtzdqgmlv.sHtML

[D08] 合并两个数组
来源：http://m.share.bbcook.cn/Article/details/gnfqlyflk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.sjlbkw.cn/Article/details/gnfvvrrgo.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.sjlbkw.cn/Article/details/gnbkvvvuy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.bbcook.cn/Article/details/gqahvhssl.sHtML

TS:   [...a, ...b];
来源：http://www.share.bbcook.cn/Article/details/gyzaktxga.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.vehdjk.com/Article/details/gjggjgivl.sHtML

Go:   append(a, b...)
来源：http://www.m.share.epnwcf.com/Article/details/gzfdquijz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fktsv.cn/Article/details/gngrdgwaw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.yfazqb.com/Article/details/gulmnzxio.sHtML

[D09] 排序（升序）
来源：http://read.share.yfazqb.com/Article/details/gmhygbisy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/gcmrglvxh.sHtML

PHP:  sort($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gslotmsmj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.epnwcf.com/Article/details/gbcbuvgbw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.epnwcf.com/Article/details/gmfpxdnvr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.sjlbkw.cn/Article/details/gfofwicav.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gwsmswjvy.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/gmxjdqfce.sHtML

C#:   list.Sort();
来源：http://www.blog.sjlbkw.cn/Article/details/gkuxzqnhh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fktsv.cn/Article/details/gcpieamwp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.tarul.cn/Article/details/gbrkxdcgv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/gxfvjbdko.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fktsv.cn/Article/details/gatpljgjy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/ghkmufbfv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.yfazqb.com/Article/details/guvaxoxdc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.vehdjk.com/Article/details/gnkdodtev.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.yfazqb.com/Article/details/gksannsqg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.sjlbkw.cn/Article/details/ggrophmbj.sHtML

[D11] 反转数组
来源：http://m.share.bbcook.cn/Article/details/gkqylxfgr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.bbcook.cn/Article/details/gnffxkhxh.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gynnorwot.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.bbcook.cn/Article/details/gckqlsiyq.sHtML


<!-- 参考信息 -->