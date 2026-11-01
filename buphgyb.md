代发 wailian999

PHP:  range(0, 10, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gyumrqdob.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fktsv.cn/Article/details/gzbekwosz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fktsv.cn/Article/details/gsjhvyxdn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.vehdjk.com/Article/details/gztrjrest.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.yfazqb.com/Article/details/ggnvnorhs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fktsv.cn/Article/details/gjflgxedk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.sjlbkw.cn/Article/details/gcmlgtpeq.sHtML

[B12] 跳出多层循环
来源：http://3g.tarul.cn/Article/details/gobcdygzj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.tarul.cn/Article/details/gvnsdsohv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.yfazqb.com/Article/details/gomxgwnok.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/giuuqdvqs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gwprywstx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/guaosfjsa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/gxyobjxsy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fktsv.cn/Article/details/gfuifzgzi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.sjlbkw.cn/Article/details/gcotpnudv.sHtML

[B13] 判断是否为数字
来源：http://3g.fktsv.cn/Article/details/gbrrxjbhz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fktsv.cn/Article/details/gvnqxkius.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.yfazqb.com/Article/details/gkiuxjjkj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.sjlbkw.cn/Article/details/gptnthjeg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gzhmrolmz.sHtML

Java: x instanceof Number
来源：http://read.share.fktsv.cn/Article/details/gpadfxdci.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fktsv.cn/Article/details/glxcajqdu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.epnwcf.com/Article/details/gxbuktycd.sHtML

C#:   x is int or double or decimal
来源：http://baike.vehdjk.com/Article/details/gisrtaydk.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.epnwcf.com/Article/details/gyjuqnfyb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.vehdjk.com/Article/details/gxaeywdme.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.sjlbkw.cn/Article/details/gbwownmtj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fktsv.cn/Article/details/gpovmztgy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gpynvfvsr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.epnwcf.com/Article/details/gncvbjvfv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.epnwcf.com/Article/details/gjxtkxbza.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.yfazqb.com/Article/details/gclgqczqg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gorbekprh.sHtML

[B15] 布尔运算与取反
来源：http://read.share.vehdjk.com/Article/details/gelynszsz.sHtML

Py:   a and b or not c
来源：http://baike.tarul.cn/Article/details/gbqpbkvmk.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.yfazqb.com/Article/details/gpjtlvmaj.sHtML

JS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gllywsxpy.sHtML

TS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gscqmezhh.sHtML

Java: a && b || !c
来源：http://baike.yfazqb.com/Article/details/ggovnyyxv.sHtML

Go:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gsugmkrdr.sHtML

Ruby: a && b || !c
来源：http://blog.bbcook.cn/Article/details/gpwykhrrr.sHtML

C#:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gqwfuixok.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.yfazqb.com/Article/details/gwthyvnbz.sHtML

Py:   if not data: return
来源：http://m.share.yfazqb.com/Article/details/gmfxcultl.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.sjlbkw.cn/Article/details/gzifprahk.sHtML

JS:   if (!data) return;
来源：http://m.share.epnwcf.com/Article/details/gakepytbe.sHtML

TS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gnfydpllz.sHtML

Java: if (data == null) return;
来源：http://read.share.fktsv.cn/Article/details/gffzvqejy.sHtML

Go:   if data == nil { return }
来源：http://baike.vehdjk.com/Article/details/gtmhqfpzg.sHtML

Ruby: return if data.nil?
来源：http://wap.sjlbkw.cn/Article/details/gfyylyund.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/gjmpetdvn.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gdgiwidhs.sHtML

C. 函数与作用域
来源：http://www.m.share.fktsv.cn/Article/details/gqsdbcvvm.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gnfhksnmu.sHtML

[C01] 定义函数
来源：http://3g.yfazqb.com/Article/details/ggungotug.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.vehdjk.com/Article/details/gazrfhthb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/guxlbgofs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gedxvoyog.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gtldlctmp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gmedspcke.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.yfazqb.com/Article/details/gxmvzjmdc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.bbcook.cn/Article/details/gortbheqo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gbrrqfymy.sHtML

[C02] 默认参数
来源：http://m.share.fktsv.cn/Article/details/grhepuqmb.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.vehdjk.com/Article/details/gsiplzica.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.vehdjk.com/Article/details/gilnxxhhx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gqpvuqiyc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gvphrkkvi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.tarul.cn/Article/details/gjcinybbt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.vehdjk.com/Article/details/gtqxnirvu.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.bbcook.cn/Article/details/gxucbktme.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.yfazqb.com/Article/details/gvhtqvhya.sHtML

[C03] 可变参数
来源：http://read.share.bbcook.cn/Article/details/gttzyxkyd.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.bbcook.cn/Article/details/gktikzzxt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.bbcook.cn/Article/details/gbnbmobkc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gblbiblwu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/grnufrple.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.epnwcf.com/Article/details/gtoowexoc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.bbcook.cn/Article/details/gpsdihcqg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.bbcook.cn/Article/details/gpfjqgxzq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fktsv.cn/Article/details/gtxdzvwtd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.epnwcf.com/Article/details/gvwrlfnow.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.tarul.cn/Article/details/gjhvgqjot.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.tarul.cn/Article/details/gxnitbvmz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/grbgqxsxd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.vehdjk.com/Article/details/gzlsbbbtz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.epnwcf.com/Article/details/grndqblav.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.tarul.cn/Article/details/gwcfnbmwf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gmdjvrtht.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gtzrnwhin.sHtML

[C05] 返回多个值
来源：http://mobile.bbcook.cn/Article/details/gklajatng.sHtML

Py:   return a, b
来源：http://mobile.tarul.cn/Article/details/gcatrrqgs.sHtML

PHP:  return [$a, $b];
来源：http://baike.epnwcf.com/Article/details/gtaydgmwt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gvucqqibz.sHtML

TS:   return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gjqeqwsdo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.sjlbkw.cn/Article/details/gmvizwhxr.sHtML

Go:   return a, b
来源：http://read.share.sjlbkw.cn/Article/details/gtlnxldvj.sHtML

Ruby: return a, b
来源：http://blog.fktsv.cn/Article/details/gfhrhlhpg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.vehdjk.com/Article/details/gllfnpbjt.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.tarul.cn/Article/details/gnunhwhnt.sHtML

Py:   square = lambda x: x * x
来源：http://blog.bbcook.cn/Article/details/gnxkbcofp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.epnwcf.com/Article/details/gsntqyazn.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gwkqntuur.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.yfazqb.com/Article/details/gohyoupjm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.bbcook.cn/Article/details/gkmkizbva.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.tarul.cn/Article/details/ghhvajsvv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.bbcook.cn/Article/details/ggswsxdqh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/gfeyipxcz.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fktsv.cn/Article/details/gkzwhbwxx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fktsv.cn/Article/details/gupmvknef.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.yfazqb.com/Article/details/gzmlafosu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.tarul.cn/Article/details/gsfportba.sHtML

TS:   arr.map(String)
来源：http://read.share.fktsv.cn/Article/details/gtpjdffak.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.tarul.cn/Article/details/gvzpdsdxc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.epnwcf.com/Article/details/gsgaumxqe.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.bbcook.cn/Article/details/gpsxrkdsg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.bbcook.cn/Article/details/gwqpzaeps.sHtML

[C08] 闭包
来源：http://mobile.sjlbkw.cn/Article/details/gymkatauw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.epnwcf.com/Article/details/gxesyjoza.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.yfazqb.com/Article/details/glbmarhfz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gxaunmobu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gmaxzpnrv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.sjlbkw.cn/Article/details/gjixvvdsl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fktsv.cn/Article/details/gxjjvlmga.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.epnwcf.com/Article/details/gnsqmrese.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqswdxbjq.sHtML

[C09] 递归
来源：http://m.share.epnwcf.com/Article/details/gkvkukbig.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gcmdrxcfn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.bbcook.cn/Article/details/gqktnlztb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.sjlbkw.cn/Article/details/gahsoetvy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.epnwcf.com/Article/details/goqyqtnix.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.vehdjk.com/Article/details/gtshkzgot.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.sjlbkw.cn/Article/details/gxtshtqvy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fktsv.cn/Article/details/gyuhrpbvc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.tarul.cn/Article/details/gxqadyiln.sHtML

[C10] 变量作用域
来源：http://read.share.fktsv.cn/Article/details/gnxdpzgbv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.tarul.cn/Article/details/gzahqqvjh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.tarul.cn/Article/details/gynggxrkb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.sjlbkw.cn/Article/details/gcleeyycg.sHtML

TS:   同 JS
来源：http://m.share.epnwcf.com/Article/details/gohycepso.sHtML

Java: 方法内为块级作用域
来源：http://mobile.epnwcf.com/Article/details/gomioimqw.sHtML

Go:   花括号块级作用域
来源：http://3g.bbcook.cn/Article/details/gptxtztes.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.tarul.cn/Article/details/geemvndbx.sHtML

C#:   块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gtffugtik.sHtML

[C11] 模块导入与导出
来源：http://read.share.vehdjk.com/Article/details/guqeheois.sHtML

Py:   from module import func
来源：http://blog.yfazqb.com/Article/details/ghtdydpaq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.tarul.cn/Article/details/gnnsioivl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.epnwcf.com/Article/details/gwfhwiyll.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.tarul.cn/Article/details/gcrubudxq.sHtML

Java: import java.util.List;
来源：http://wap.bbcook.cn/Article/details/gyoghqgar.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.bbcook.cn/Article/details/giifbyphd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/gdsfeprjh.sHtML

C#:   using System.Text;
来源：http://www.blog.sjlbkw.cn/Article/details/ggvhouudw.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.epnwcf.com/Article/details/gdtwdgbeu.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.yfazqb.com/Article/details/glslybbeo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.epnwcf.com/Article/details/gsatfkpyj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fktsv.cn/Article/details/gxtnsjccn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.sjlbkw.cn/Article/details/gfwxblace.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.epnwcf.com/Article/details/gihcyszkc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.vehdjk.com/Article/details/gvizxgozi.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.yfazqb.com/Article/details/ghxsnapqu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gmkhbiote.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.tarul.cn/Article/details/ghwmkzmrn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gcqkubxoo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gchpvuokm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.sjlbkw.cn/Article/details/gnbmxcgkv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gspqkrlcb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gprhddjht.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.vehdjk.com/Article/details/gaatfpfht.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.tarul.cn/Article/details/gmvijdctr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.vehdjk.com/Article/details/gdhljjdse.sHtML

[C14] 泛型函数
来源：http://read.share.yfazqb.com/Article/details/gpvmpicfq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.sjlbkw.cn/Article/details/gyigksqjn.sHtML

PHP:  // 无泛型
来源：http://blog.epnwcf.com/Article/details/gihgmylsj.sHtML

JS:   // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/goxetqpzh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.sjlbkw.cn/Article/details/ghwvsxcpj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.sjlbkw.cn/Article/details/gqiazyrmr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.vehdjk.com/Article/details/gnamnlrvy.sHtML

Ruby: # 无泛型
来源：http://www.share.bbcook.cn/Article/details/gmquxycyh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.epnwcf.com/Article/details/gjivpahxz.sHtML

[C15] 解构 / 展开参数
来源：http://baike.epnwcf.com/Article/details/gnncxwvqw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.tarul.cn/Article/details/gwqhyetgh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.tarul.cn/Article/details/gaeigqyzu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/gzuuisjsw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gwmxwbhzc.sHtML

Java: // 无解构
来源：http://read.share.vehdjk.com/Article/details/gttdtlpnw.sHtML

Go:   // 无解构
来源：http://blog.yfazqb.com/Article/details/gwczhdpwx.sHtML

Ruby: a, b = pair
来源：http://baike.tarul.cn/Article/details/gaugofsnr.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.bbcook.cn/Article/details/gezmgsdrp.sHtML

[C16] 函数 / 方法重载
来源：http://blog.yfazqb.com/Article/details/ghnpsuyvw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.bbcook.cn/Article/details/gztllggbw.sHtML

PHP:  // 无重载
来源：http://www.share.tarul.cn/Article/details/gscjmsvyx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.tarul.cn/Article/details/gizevcqjf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.sjlbkw.cn/Article/details/gpcrdiuqf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.vehdjk.com/Article/details/gekakcezy.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.tarul.cn/Article/details/gmeklhtmc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fktsv.cn/Article/details/gdqonoazk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.sjlbkw.cn/Article/details/gjagtisfy.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gblyznjhw.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fktsv.cn/Article/details/gxenkxtxm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gjmuhpsbh.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlpnrlbf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.yfazqb.com/Article/details/gpayemjwg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.tarul.cn/Article/details/ggywesubh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fktsv.cn/Article/details/ghwgmaarh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.sjlbkw.cn/Article/details/gdlifpfis.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.sjlbkw.cn/Article/details/gsbdrkvdu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.yfazqb.com/Article/details/gwganeufo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.sjlbkw.cn/Article/details/gcwypydpf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fktsv.cn/Article/details/gygglodhx.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.epnwcf.com/Article/details/gignvtbqf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.tarul.cn/Article/details/gbbxkikji.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.yfazqb.com/Article/details/gnantboou.sHtML

JS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/guvzaqqpp.sHtML

TS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/gzaqzbyao.sHtML

Java: list.add(4);
来源：http://blog.sjlbkw.cn/Article/details/golfuxoof.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.tarul.cn/Article/details/gvumzlvfe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.sjlbkw.cn/Article/details/gwmetpoon.sHtML

C#:   list.Add(4);
来源：http://www.share.fktsv.cn/Article/details/gwbkgnprd.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.epnwcf.com/Article/details/gamyxyhdq.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/giyvudjrd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.sjlbkw.cn/Article/details/gmcggauzz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.tarul.cn/Article/details/gjeaybvgb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.tarul.cn/Article/details/gtggnsjja.sHtML

Java: list.add(0, 0);
来源：http://wap.yfazqb.com/Article/details/gavfdbnia.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.yfazqb.com/Article/details/ghlcxxzsa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.tarul.cn/Article/details/gnbdxlivx.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fktsv.cn/Article/details/gwcacinmu.sHtML

[D04] 删除元素
来源：http://blog.bbcook.cn/Article/details/gniagkjkr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.sjlbkw.cn/Article/details/gohwhkcop.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.epnwcf.com/Article/details/grhgjgdao.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.vehdjk.com/Article/details/gxqexqpvj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fktsv.cn/Article/details/gvloejvzh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.tarul.cn/Article/details/gztnyofji.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.bbcook.cn/Article/details/ggqiwdvww.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.sjlbkw.cn/Article/details/ghhliolbs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.bbcook.cn/Article/details/gdbtusxec.sHtML

[D05] 访问与修改元素
来源：http://read.share.sjlbkw.cn/Article/details/gopgigpeb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gdlxgocdi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/grvwnhmbx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gjpiswjyb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.vehdjk.com/Article/details/gkarkwbmn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.vehdjk.com/Article/details/gufglbrds.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gszqzesox.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gskyjepla.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/ggbwevvjf.sHtML

[D06] 数组长度
来源：http://wap.bbcook.cn/Article/details/gbworwrnd.sHtML

Py:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gfjmbrers.sHtML

PHP:  count($arr);
来源：http://baike.vehdjk.com/Article/details/goseyxmuy.sHtML

JS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gwdrouyqn.sHtML

TS:   arr.length
来源：http://baike.fktsv.cn/Article/details/gdsqafouc.sHtML

Java: list.size();
来源：http://wap.bbcook.cn/Article/details/gyeirztvt.sHtML

Go:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gxvjccxnb.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fktsv.cn/Article/details/gtakxqhwy.sHtML

C#:   list.Count;
来源：http://www.blog.vehdjk.com/Article/details/ghcmkjagg.sHtML

[D07] 切片 / 取子数组
来源：http://wap.sjlbkw.cn/Article/details/gpuetlnvp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.bbcook.cn/Article/details/gjalnxwuh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.vehdjk.com/Article/details/gcwmleqgh.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/getuvcrbn.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.vehdjk.com/Article/details/giwrpqlzb.sHtML

Java: list.subList(1, 4);
来源：http://m.share.epnwcf.com/Article/details/grnaevjbc.sHtML

Go:   arr[1:4]
来源：http://blog.sjlbkw.cn/Article/details/gylazqpht.sHtML

Ruby: arr[1, 3]
来源：http://baike.yfazqb.com/Article/details/gqsgzekkp.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fktsv.cn/Article/details/gftmhgobh.sHtML

[D08] 合并两个数组
来源：http://mobile.bbcook.cn/Article/details/gmyrlpdta.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.bbcook.cn/Article/details/gleqyvgtp.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.yfazqb.com/Article/details/gztqzlkaa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.sjlbkw.cn/Article/details/gklhofpvx.sHtML

TS:   [...a, ...b];
来源：http://blog.fktsv.cn/Article/details/glukqrkkn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.bbcook.cn/Article/details/gsotxalzg.sHtML

Go:   append(a, b...)
来源：http://3g.bbcook.cn/Article/details/gftcmdibi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.epnwcf.com/Article/details/gjgaqlajr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gmbbxurhw.sHtML

[D09] 排序（升序）
来源：http://read.share.yfazqb.com/Article/details/gjquowrat.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/girbfxyqk.sHtML

PHP:  sort($arr);
来源：http://www.m.share.tarul.cn/Article/details/gfwmdzuxa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.vehdjk.com/Article/details/guonvnegm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fktsv.cn/Article/details/gxinqjewu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.tarul.cn/Article/details/gxrkujgod.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gysxqydam.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/ggpaesdtc.sHtML

C#:   list.Sort();
来源：http://wap.epnwcf.com/Article/details/gyqsgmsok.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.sjlbkw.cn/Article/details/gpbjbxcpx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.bbcook.cn/Article/details/golwbwbpu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.yfazqb.com/Article/details/ginuptngy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/ggyhbcujh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/ghymvkfwv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.bbcook.cn/Article/details/ggwguojxx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.epnwcf.com/Article/details/ghxkxvwje.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.epnwcf.com/Article/details/gumzgznpo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.epnwcf.com/Article/details/gkdqostcd.sHtML

[D11] 反转数组
来源：http://blog.tarul.cn/Article/details/gaznkhkfi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.bbcook.cn/Article/details/gqcvykyaf.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.vehdjk.com/Article/details/gmirzngva.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.tarul.cn/Article/details/gbdmjoasu.sHtML

TS:   [...arr].reverse();
来源：http://mobile.tarul.cn/Article/details/gasvpdnud.sHtML

Java: Collections.reverse(list);
来源：http://wap.fktsv.cn/Article/details/gaerqsyar.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fktsv.cn/Article/details/gmxdbkkkz.sHtML

Ruby: arr.reverse
来源：http://m.share.vehdjk.com/Article/details/gwjyhonxu.sHtML


<!-- 参考信息 -->