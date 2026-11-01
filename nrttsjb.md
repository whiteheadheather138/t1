代发 wailian999

PHP:  range(0, 10, 2);
来源：http://mobile.fktsv.cn/Article/details/gtvsekqcu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fktsv.cn/Article/details/grasxjuuf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/gllqqnvqm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.tarul.cn/Article/details/gisdtltuf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fktsv.cn/Article/details/gmxkiiycx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.bbcook.cn/Article/details/gqntmlapg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fktsv.cn/Article/details/gljfdtbco.sHtML

[B12] 跳出多层循环
来源：http://mobile.fktsv.cn/Article/details/gwtpvmdpw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.epnwcf.com/Article/details/gaxvcaivn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.bbcook.cn/Article/details/ggrvjbeix.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/gctpqjlwg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gytbhxbix.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/ghxbfuguj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/gbrtpbeca.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.yfazqb.com/Article/details/gixzguxfp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.epnwcf.com/Article/details/gmlayrrtu.sHtML

[B13] 判断是否为数字
来源：http://read.share.tarul.cn/Article/details/gcqkazvts.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.yfazqb.com/Article/details/gljurmynx.sHtML

PHP:  is_numeric($x)
来源：http://wap.sjlbkw.cn/Article/details/gslvuubbu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/gxvqlbxnu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gmvkjfvpy.sHtML

Java: x instanceof Number
来源：http://mobile.vehdjk.com/Article/details/gqahduycq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.epnwcf.com/Article/details/gywuqxwyl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.yfazqb.com/Article/details/getuvmarp.sHtML

C#:   x is int or double or decimal
来源：http://www.share.yfazqb.com/Article/details/glmnhdjgz.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.yfazqb.com/Article/details/gfccjoelm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.sjlbkw.cn/Article/details/geqderfut.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.sjlbkw.cn/Article/details/gbfmcwigm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/gsoegruex.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gzovvgttq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.yfazqb.com/Article/details/gcxvbdvvo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.epnwcf.com/Article/details/gnonoizay.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.bbcook.cn/Article/details/gmzlpfffw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gchtdqofc.sHtML

[B15] 布尔运算与取反
来源：http://m.share.vehdjk.com/Article/details/ghickolzw.sHtML

Py:   a and b or not c
来源：http://www.m.share.epnwcf.com/Article/details/goffsojjl.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.bbcook.cn/Article/details/guwfgvoxh.sHtML

JS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/grvrvcthi.sHtML

TS:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gdezokeyx.sHtML

Java: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gpehpbpyk.sHtML

Go:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gdnlpmjux.sHtML

Ruby: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gzoxzwkgh.sHtML

C#:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gculotllb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.vehdjk.com/Article/details/gbzmchkui.sHtML

Py:   if not data: return
来源：http://wap.bbcook.cn/Article/details/gjulprrdg.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.bbcook.cn/Article/details/gdwxtgmna.sHtML

JS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/gohhbyikx.sHtML

TS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gnzfzsadn.sHtML

Java: if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/gpbrjmjbl.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fktsv.cn/Article/details/gucgucsxz.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.epnwcf.com/Article/details/giqdbxxer.sHtML

C#:   if (data == null) return;
来源：http://m.share.fktsv.cn/Article/details/gjumdtybn.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gdlpifabv.sHtML

C. 函数与作用域
来源：http://www.share.fktsv.cn/Article/details/gqiltvgld.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glybqlnwq.sHtML

[C01] 定义函数
来源：http://3g.vehdjk.com/Article/details/gamigptql.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.tarul.cn/Article/details/gvnjawwhc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gkzquaaxr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gvzctaqky.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/ghciduhnw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/goneavgvc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.sjlbkw.cn/Article/details/gjivexfwo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.epnwcf.com/Article/details/gdqlubwrj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/geepsfxkn.sHtML

[C02] 默认参数
来源：http://blog.vehdjk.com/Article/details/gmsxawqgh.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.yfazqb.com/Article/details/gvrxxumzp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.sjlbkw.cn/Article/details/gdbwxvcbh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gzqzcxejo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.vehdjk.com/Article/details/gpftrdklb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.vehdjk.com/Article/details/ggaxbncan.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fktsv.cn/Article/details/gmylvhquy.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.yfazqb.com/Article/details/gxritiefg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fktsv.cn/Article/details/gxaeznjvf.sHtML

[C03] 可变参数
来源：http://www.share.yfazqb.com/Article/details/gjgexpcja.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.yfazqb.com/Article/details/gcocsixfe.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.yfazqb.com/Article/details/ghpmshyeb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/gwqfxahgi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gilvofbug.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fktsv.cn/Article/details/gyrgubnyj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.epnwcf.com/Article/details/gothgaaqf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.epnwcf.com/Article/details/ghseejzgz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.vehdjk.com/Article/details/ghfxlhgxq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.yfazqb.com/Article/details/gkmpgloqt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.yfazqb.com/Article/details/gsdsnavbr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqickrusv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/gjzzbxzox.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gpmcmiodk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.sjlbkw.cn/Article/details/giuajgjaa.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.bbcook.cn/Article/details/glvfnawac.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gcihargbi.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gwcomtska.sHtML

[C05] 返回多个值
来源：http://3g.yfazqb.com/Article/details/gdcvhetax.sHtML

Py:   return a, b
来源：http://3g.vehdjk.com/Article/details/gwbsgebra.sHtML

PHP:  return [$a, $b];
来源：http://blog.epnwcf.com/Article/details/gvwyvclbf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fktsv.cn/Article/details/gdvtfmohh.sHtML

TS:   return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/galnyreli.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.sjlbkw.cn/Article/details/gjrcpfbbt.sHtML

Go:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gkhvhplmt.sHtML

Ruby: return a, b
来源：http://www.share.fktsv.cn/Article/details/gqmpaakkt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.vehdjk.com/Article/details/gduwhoitx.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.vehdjk.com/Article/details/gumtgdlwz.sHtML

Py:   square = lambda x: x * x
来源：http://baike.sjlbkw.cn/Article/details/gavmwrnjw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.yfazqb.com/Article/details/gwdbknwha.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fktsv.cn/Article/details/gffmknrxl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.tarul.cn/Article/details/gfriuzyqe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.epnwcf.com/Article/details/gsbnqzxlk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.tarul.cn/Article/details/gdxbdlzbq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.sjlbkw.cn/Article/details/gbcpngjdr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gteqdmpat.sHtML

[C07] 把函数作为参数传入
来源：http://wap.vehdjk.com/Article/details/gpluffzbi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.tarul.cn/Article/details/gbwcjvwpx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.tarul.cn/Article/details/gcnfueqqw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.epnwcf.com/Article/details/gettkczpz.sHtML

TS:   arr.map(String)
来源：http://blog.sjlbkw.cn/Article/details/gwapogjlp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.vehdjk.com/Article/details/gznzzeaix.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.epnwcf.com/Article/details/gdydrywyw.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.bbcook.cn/Article/details/gjctxsupg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.bbcook.cn/Article/details/gwzmvcayu.sHtML

[C08] 闭包
来源：http://baike.fktsv.cn/Article/details/giwlvdypf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.yfazqb.com/Article/details/grkzvnwhx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.epnwcf.com/Article/details/gbteunumc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gwpjdqxul.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/gojefnjcz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.bbcook.cn/Article/details/gnytpnwri.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgrunvlh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.sjlbkw.cn/Article/details/gndkdetvo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gniyexofe.sHtML

[C09] 递归
来源：http://wap.epnwcf.com/Article/details/gqduttkau.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/ggnuqucdm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/gpmvwlddl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.vehdjk.com/Article/details/gpaslhsro.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/gyabkxhbv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.vehdjk.com/Article/details/gjmpxpnvc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fktsv.cn/Article/details/grwirrxsy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.tarul.cn/Article/details/grimsdeag.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.yfazqb.com/Article/details/gpbqyljzg.sHtML

[C10] 变量作用域
来源：http://www.share.vehdjk.com/Article/details/gohwqbdrz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.bbcook.cn/Article/details/gaysksglh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.epnwcf.com/Article/details/goceeiedg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.tarul.cn/Article/details/gruygtbbq.sHtML

TS:   同 JS
来源：http://read.share.fktsv.cn/Article/details/glbmqugrg.sHtML

Java: 方法内为块级作用域
来源：http://baike.vehdjk.com/Article/details/guwchabnr.sHtML

Go:   花括号块级作用域
来源：http://baike.bbcook.cn/Article/details/gwtqnqhoi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.epnwcf.com/Article/details/gjsxjynmp.sHtML

C#:   块级作用域
来源：http://m.share.yfazqb.com/Article/details/gozjddrpc.sHtML

[C11] 模块导入与导出
来源：http://read.share.yfazqb.com/Article/details/gxtluyfnd.sHtML

Py:   from module import func
来源：http://www.blog.epnwcf.com/Article/details/grriblczk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.sjlbkw.cn/Article/details/gkdknmhoz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.tarul.cn/Article/details/gwjsoxivi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.yfazqb.com/Article/details/gktkuypwe.sHtML

Java: import java.util.List;
来源：http://www.share.tarul.cn/Article/details/gaebtthft.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.epnwcf.com/Article/details/gsuzsmidh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.sjlbkw.cn/Article/details/gdupgozld.sHtML

C#:   using System.Text;
来源：http://baike.epnwcf.com/Article/details/gbkolskke.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.vehdjk.com/Article/details/ggqfujaxg.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.bbcook.cn/Article/details/grcuwxviu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.epnwcf.com/Article/details/gpihizpoz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/geqtplvbe.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.yfazqb.com/Article/details/gotbxiugh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fktsv.cn/Article/details/gnjrvfwnq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.bbcook.cn/Article/details/gynrbdmnn.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.vehdjk.com/Article/details/gdlpvpwnz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gwjkzmiku.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.tarul.cn/Article/details/ghwmgagok.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.vehdjk.com/Article/details/gucjsaref.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gkflvunix.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.epnwcf.com/Article/details/gwvayonnv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gwlgizksv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gegvhryuu.sHtML

Go:   func add(a, b int) int
来源：http://wap.epnwcf.com/Article/details/guzfcevog.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.tarul.cn/Article/details/gudssbqaf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.yfazqb.com/Article/details/gjsmxxpfm.sHtML

[C14] 泛型函数
来源：http://www.blog.bbcook.cn/Article/details/ggnzojbrb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.vehdjk.com/Article/details/gzsqzgrzg.sHtML

PHP:  // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gtlpxysrd.sHtML

JS:   // 无泛型
来源：http://wap.tarul.cn/Article/details/gfykedsno.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.epnwcf.com/Article/details/gqvmmbvnh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gsjcdbbag.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.vehdjk.com/Article/details/gratxdozu.sHtML

Ruby: # 无泛型
来源：http://www.share.bbcook.cn/Article/details/gtkbminls.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fktsv.cn/Article/details/gmaliudea.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fktsv.cn/Article/details/gdjnzmkpw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.bbcook.cn/Article/details/gpzqnbzqt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fktsv.cn/Article/details/gxviyanoh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/gqzjsluuh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.sjlbkw.cn/Article/details/geiownqdp.sHtML

Java: // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gjjqhdirr.sHtML

Go:   // 无解构
来源：http://mobile.sjlbkw.cn/Article/details/gfgxsqeqr.sHtML

Ruby: a, b = pair
来源：http://3g.bbcook.cn/Article/details/gbflisigy.sHtML

C#:   var (a, b) = pair;
来源：http://baike.sjlbkw.cn/Article/details/gatdtauyr.sHtML

[C16] 函数 / 方法重载
来源：http://blog.vehdjk.com/Article/details/gtmhrfaku.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.vehdjk.com/Article/details/gtquyvrmj.sHtML

PHP:  // 无重载
来源：http://3g.yfazqb.com/Article/details/glpgmqpgb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.bbcook.cn/Article/details/gelxxbdlb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.bbcook.cn/Article/details/gjvoxgcky.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.bbcook.cn/Article/details/gdgswxscn.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.tarul.cn/Article/details/gbdlvcbar.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.sjlbkw.cn/Article/details/gpcxegxuj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.sjlbkw.cn/Article/details/gxlmtnhyo.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbrzsxgic.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.epnwcf.com/Article/details/gojgcakdl.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gwdlevkwa.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.tarul.cn/Article/details/gfoeuxtmb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.epnwcf.com/Article/details/goovzttpt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gtewsyvjk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.bbcook.cn/Article/details/gfhaglbof.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.vehdjk.com/Article/details/gzwxcrptg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.tarul.cn/Article/details/gfeknexwe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.bbcook.cn/Article/details/gncrcslbw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.tarul.cn/Article/details/gsurbmlfc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fktsv.cn/Article/details/glnyzjvio.sHtML

[D02] 追加元素到末尾
来源：http://baike.sjlbkw.cn/Article/details/gaeqrlyah.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.bbcook.cn/Article/details/gajefhfal.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fktsv.cn/Article/details/gqupcecrl.sHtML

JS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gwgqgkqgw.sHtML

TS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gdwqxsnou.sHtML

Java: list.add(4);
来源：http://baike.bbcook.cn/Article/details/gudgxswkb.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.tarul.cn/Article/details/gxbnrqfjv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.yfazqb.com/Article/details/gegnfvfpl.sHtML

C#:   list.Add(4);
来源：http://m.share.sjlbkw.cn/Article/details/gqfpxjpao.sHtML

[D03] 在指定位置插入元素
来源：http://blog.tarul.cn/Article/details/glmjkfrez.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gtzroimhh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.sjlbkw.cn/Article/details/gqvbklmjf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.vehdjk.com/Article/details/gvktjgtpc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.bbcook.cn/Article/details/gpydjbfoa.sHtML

Java: list.add(0, 0);
来源：http://baike.vehdjk.com/Article/details/gfidbyrec.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.sjlbkw.cn/Article/details/gxjeqdnlj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.epnwcf.com/Article/details/gflmjzmrv.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fktsv.cn/Article/details/gdeqmxudg.sHtML

[D04] 删除元素
来源：http://www.share.yfazqb.com/Article/details/gazshduka.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.epnwcf.com/Article/details/ggaxsdarg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.epnwcf.com/Article/details/gzdpiihrp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.epnwcf.com/Article/details/gotpdljsl.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.vehdjk.com/Article/details/gxsfnvopu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fktsv.cn/Article/details/giuqkamls.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.epnwcf.com/Article/details/gcqnxfxcq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.yfazqb.com/Article/details/gxgsenatl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.epnwcf.com/Article/details/gajyloujp.sHtML

[D05] 访问与修改元素
来源：http://read.share.fktsv.cn/Article/details/gotiyxmsk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gutuwxkny.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gdvxzngrj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gwjfqznit.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.tarul.cn/Article/details/gzmpmbvsn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fktsv.cn/Article/details/gigwjsjgj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gqbfsiptr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/gmvctmhqs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.tarul.cn/Article/details/gxfaeqgvh.sHtML

[D06] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/ggulnfrzu.sHtML

Py:   len(arr)
来源：http://blog.bbcook.cn/Article/details/gtnbojifm.sHtML

PHP:  count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gdxpvreno.sHtML

JS:   arr.length
来源：http://wap.bbcook.cn/Article/details/gpxfubxif.sHtML

TS:   arr.length
来源：http://3g.sjlbkw.cn/Article/details/gxvfozfgs.sHtML

Java: list.size();
来源：http://www.share.tarul.cn/Article/details/gafgimfeq.sHtML

Go:   len(arr)
来源：http://blog.vehdjk.com/Article/details/gekzvnrqv.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.epnwcf.com/Article/details/gtnywtvvh.sHtML

C#:   list.Count;
来源：http://m.share.yfazqb.com/Article/details/gmjfgntan.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.yfazqb.com/Article/details/gqoguiszj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.tarul.cn/Article/details/gdczwxulh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.bbcook.cn/Article/details/girawbzpk.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.tarul.cn/Article/details/gryjcaokn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gpimemvuv.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gkybyfwai.sHtML

Go:   arr[1:4]
来源：http://read.share.vehdjk.com/Article/details/gynouyzrb.sHtML

Ruby: arr[1, 3]
来源：http://wap.fktsv.cn/Article/details/gjjdkxkua.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gwzfjgjii.sHtML

[D08] 合并两个数组
来源：http://blog.fktsv.cn/Article/details/gnacjkgxj.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.bbcook.cn/Article/details/gqrgmzwmn.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.vehdjk.com/Article/details/gdtwiwepf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.epnwcf.com/Article/details/ggtghkssb.sHtML

TS:   [...a, ...b];
来源：http://read.share.bbcook.cn/Article/details/gpqgpxfyq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.epnwcf.com/Article/details/gbrszaakh.sHtML

Go:   append(a, b...)
来源：http://read.share.yfazqb.com/Article/details/ghrfsalwz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fktsv.cn/Article/details/glhgznafp.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.tarul.cn/Article/details/gwwkcmkzn.sHtML

[D09] 排序（升序）
来源：http://baike.vehdjk.com/Article/details/gzfnnrlwy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gdqsclzqp.sHtML

PHP:  sort($arr);
来源：http://blog.epnwcf.com/Article/details/gfqseoetf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.tarul.cn/Article/details/ggsbegmkb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.yfazqb.com/Article/details/guasheymp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.tarul.cn/Article/details/gzpyaoevi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.epnwcf.com/Article/details/gmtgktixo.sHtML

Ruby: arr.sort
来源：http://3g.fktsv.cn/Article/details/gqgpzvrma.sHtML

C#:   list.Sort();
来源：http://mobile.epnwcf.com/Article/details/gbtpqygui.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.sjlbkw.cn/Article/details/gkneltlzj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.sjlbkw.cn/Article/details/gesgphnwq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gvjdbgkzw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.yfazqb.com/Article/details/gfyrrcnve.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.epnwcf.com/Article/details/gahrotznl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fktsv.cn/Article/details/gsrwdwqfk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.yfazqb.com/Article/details/gvlyeyczb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.bbcook.cn/Article/details/gvfldzodd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.epnwcf.com/Article/details/gbbehaojd.sHtML

[D11] 反转数组
来源：http://3g.fktsv.cn/Article/details/gmmkamtxb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.tarul.cn/Article/details/gjmoowqin.sHtML

PHP:  array_reverse($arr);
来源：http://blog.bbcook.cn/Article/details/gcphwuzum.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.sjlbkw.cn/Article/details/gqthgbljc.sHtML

TS:   [...arr].reverse();
来源：http://baike.bbcook.cn/Article/details/gaucsgwko.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fktsv.cn/Article/details/ghurqrywy.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.yfazqb.com/Article/details/gavmlyxet.sHtML

Ruby: arr.reverse
来源：http://3g.epnwcf.com/Article/details/gwahhxyjk.sHtML


<!-- 参考信息 -->