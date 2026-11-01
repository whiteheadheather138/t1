代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.bbcook.cn/Article/details/gpbljbuxd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.epnwcf.com/Article/details/gloxbnwpc.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.yfazqb.com/Article/details/gkdnrlvns.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.tarul.cn/Article/details/gzsdtnymd.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.tarul.cn/Article/details/gzuiqwwtv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gmthltfrt.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fktsv.cn/Article/details/gmhnqembg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.yfazqb.com/Article/details/gfrdanoow.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.yfazqb.com/Article/details/gpdpmyzxh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.sjlbkw.cn/Article/details/gfsicewly.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.vehdjk.com/Article/details/gonxtfbis.sHtML

[B12] 跳出多层循环
来源：http://blog.fktsv.cn/Article/details/gcnxtblid.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.sjlbkw.cn/Article/details/galdfpxtv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.bbcook.cn/Article/details/gkmclrpqh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gfencvsax.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/gqfynqlef.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/gksiqkkgx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.epnwcf.com/Article/details/gqcwcsbwl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fktsv.cn/Article/details/gzfmfrzqp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.tarul.cn/Article/details/grqydrvgw.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.epnwcf.com/Article/details/gvtgpzwzf.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.tarul.cn/Article/details/gaiiarbgl.sHtML

PHP:  is_numeric($x)
来源：http://3g.fktsv.cn/Article/details/gzqloawwa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/ghbxldcyz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/gypamvmpg.sHtML

Java: x instanceof Number
来源：http://blog.bbcook.cn/Article/details/glkbmnbgd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.sjlbkw.cn/Article/details/gzgofdiap.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmbvxzwn.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fktsv.cn/Article/details/gfjpuhbqt.sHtML

[B14] 判断值是否在集合内
来源：http://3g.yfazqb.com/Article/details/gpiiyhdav.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.sjlbkw.cn/Article/details/gausoxxjh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.bbcook.cn/Article/details/gshkokwyr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gjxfhxzvh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.tarul.cn/Article/details/gyrrrphfp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.vehdjk.com/Article/details/gpdeagmzh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.bbcook.cn/Article/details/grneknvdy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.yfazqb.com/Article/details/ganmltflx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaeqbdtjl.sHtML

[B15] 布尔运算与取反
来源：http://blog.fktsv.cn/Article/details/gnqhmsxgw.sHtML

Py:   a and b or not c
来源：http://mobile.epnwcf.com/Article/details/grkswgddf.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.tarul.cn/Article/details/gotezbbxd.sHtML

JS:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gbskbhcnc.sHtML

TS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gcksddkxf.sHtML

Java: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gxsblkrkx.sHtML

Go:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gfusddrvs.sHtML

Ruby: a && b || !c
来源：http://blog.tarul.cn/Article/details/gfjuirtkg.sHtML

C#:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gfuzbvwin.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.tarul.cn/Article/details/gguajebus.sHtML

Py:   if not data: return
来源：http://blog.bbcook.cn/Article/details/goukmzyuj.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fktsv.cn/Article/details/gunppehbt.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gwhcqjbje.sHtML

TS:   if (!data) return;
来源：http://read.share.yfazqb.com/Article/details/gpknugolf.sHtML

Java: if (data == null) return;
来源：http://3g.tarul.cn/Article/details/gfzqamtqk.sHtML

Go:   if data == nil { return }
来源：http://www.share.tarul.cn/Article/details/gcejdtakj.sHtML

Ruby: return if data.nil?
来源：http://baike.fktsv.cn/Article/details/gztlhuejj.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gwymqplkb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbduyhjjw.sHtML

C. 函数与作用域
来源：http://read.share.tarul.cn/Article/details/grybjerwz.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grpmzkojm.sHtML

[C01] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gjboaeysr.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.vehdjk.com/Article/details/gptxdkpje.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gxvhicnkb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/giuvrenkx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gpsnahxuy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/ghgxakzzb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.epnwcf.com/Article/details/gobjhkwer.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.sjlbkw.cn/Article/details/gpyixljhr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gkxlkzipt.sHtML

[C02] 默认参数
来源：http://mobile.tarul.cn/Article/details/gfdqrcsqe.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.sjlbkw.cn/Article/details/gzfgnmpoe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fktsv.cn/Article/details/ghaaqpslw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/gpwtgyhlb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/gveyogmbb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fktsv.cn/Article/details/gloffeasy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.epnwcf.com/Article/details/grioyvwbo.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.vehdjk.com/Article/details/gfjaskift.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.vehdjk.com/Article/details/gaoyaxlrx.sHtML

[C03] 可变参数
来源：http://blog.sjlbkw.cn/Article/details/gnsdgmnvt.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.yfazqb.com/Article/details/gcaxsrhbx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fktsv.cn/Article/details/gxisjjdlu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gdphvkiur.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gdjvdszki.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.yfazqb.com/Article/details/ginkixhns.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.vehdjk.com/Article/details/gvjtikmwu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.sjlbkw.cn/Article/details/gcyoatjxt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fktsv.cn/Article/details/grgiamyxr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.tarul.cn/Article/details/gqmhbbqtg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.epnwcf.com/Article/details/gwypznsvq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.sjlbkw.cn/Article/details/gntxryjly.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gslxnlgnq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fktsv.cn/Article/details/gvwdcbxou.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.vehdjk.com/Article/details/gngwotoor.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.tarul.cn/Article/details/giupsvsns.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gbnlnsyue.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gfsgbsxea.sHtML

[C05] 返回多个值
来源：http://www.m.share.epnwcf.com/Article/details/gxrxbykyb.sHtML

Py:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/gcemdhfdf.sHtML

PHP:  return [$a, $b];
来源：http://mobile.bbcook.cn/Article/details/gmkdyetsu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.sjlbkw.cn/Article/details/gecwoljto.sHtML

TS:   return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gsyglgoas.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fktsv.cn/Article/details/gxjxjdbfu.sHtML

Go:   return a, b
来源：http://blog.vehdjk.com/Article/details/gjxopipei.sHtML

Ruby: return a, b
来源：http://mobile.yfazqb.com/Article/details/gpatispuo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.tarul.cn/Article/details/goxzonjts.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fktsv.cn/Article/details/grkeqftqw.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fktsv.cn/Article/details/gwjddnzxc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.vehdjk.com/Article/details/gqwsmzjrg.sHtML

JS:   const square = x => x * x;
来源：http://wap.bbcook.cn/Article/details/glhiyqxxe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.vehdjk.com/Article/details/goisvyayg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fktsv.cn/Article/details/gbrubqjbz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gwfjiqjsh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.tarul.cn/Article/details/gsmutpsyo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.tarul.cn/Article/details/geetphztf.sHtML

[C07] 把函数作为参数传入
来源：http://3g.bbcook.cn/Article/details/getufwskt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.bbcook.cn/Article/details/ghscxetst.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnquwecie.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fktsv.cn/Article/details/gwqzoflxy.sHtML

TS:   arr.map(String)
来源：http://3g.sjlbkw.cn/Article/details/gumlppzoc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.tarul.cn/Article/details/gdxuwsyol.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.bbcook.cn/Article/details/grkfqeflk.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.bbcook.cn/Article/details/gqgqousps.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.vehdjk.com/Article/details/gvfoiclvk.sHtML

[C08] 闭包
来源：http://www.m.share.vehdjk.com/Article/details/grdjduveq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.yfazqb.com/Article/details/gjuzosjuf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.bbcook.cn/Article/details/gchofwuxy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/grjomggir.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gimafnfxf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.epnwcf.com/Article/details/gyqdypzcy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.yfazqb.com/Article/details/gpiblnecs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.yfazqb.com/Article/details/grxryiipr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gywquqfpw.sHtML

[C09] 递归
来源：http://mobile.tarul.cn/Article/details/gpweyvzma.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.vehdjk.com/Article/details/glndfmxla.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/giohhdmad.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gskeydnoc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/gaulridfs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.epnwcf.com/Article/details/gxjidqhcb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.yfazqb.com/Article/details/guxwtkwop.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gquxsjask.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.tarul.cn/Article/details/gqqtlhwqd.sHtML

[C10] 变量作用域
来源：http://www.share.fktsv.cn/Article/details/gpgeovorc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.epnwcf.com/Article/details/guilemymk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/gdyxhzykz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.tarul.cn/Article/details/gldvzxwcr.sHtML

TS:   同 JS
来源：http://3g.yfazqb.com/Article/details/gxmdpxkpv.sHtML

Java: 方法内为块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gigeocytp.sHtML

Go:   花括号块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gszmgvcfa.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.vehdjk.com/Article/details/gbmuzdqis.sHtML

C#:   块级作用域
来源：http://3g.epnwcf.com/Article/details/gxvzphvuz.sHtML

[C11] 模块导入与导出
来源：http://baike.sjlbkw.cn/Article/details/gaugmlxzu.sHtML

Py:   from module import func
来源：http://read.share.yfazqb.com/Article/details/gdxbswvta.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.bbcook.cn/Article/details/gveyfhcro.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.yfazqb.com/Article/details/gvuycioon.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.bbcook.cn/Article/details/gtzvukjlc.sHtML

Java: import java.util.List;
来源：http://read.share.vehdjk.com/Article/details/giwkevwvu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.tarul.cn/Article/details/gwiwbuwcr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.sjlbkw.cn/Article/details/gnqjnrtsp.sHtML

C#:   using System.Text;
来源：http://wap.epnwcf.com/Article/details/gpuywqvsi.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.epnwcf.com/Article/details/gernwvzxd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.epnwcf.com/Article/details/gmgvmkpcb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.epnwcf.com/Article/details/gacrnoxcl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/grkoshjtw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gkkxrvfia.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.sjlbkw.cn/Article/details/gfcvxyppd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.yfazqb.com/Article/details/gvfbhhtjt.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.tarul.cn/Article/details/gluoxjlfq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fktsv.cn/Article/details/giyqncnfv.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.tarul.cn/Article/details/gbkunqqfy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.sjlbkw.cn/Article/details/gafmijqah.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gxxmjtklh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.sjlbkw.cn/Article/details/gqytiycln.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gokwakekg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gkfdslkgc.sHtML

Go:   func add(a, b int) int
来源：http://blog.yfazqb.com/Article/details/grwasfhgh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.bbcook.cn/Article/details/gnuddzjap.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqafthzi.sHtML

[C14] 泛型函数
来源：http://www.blog.epnwcf.com/Article/details/gkuusgxel.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.bbcook.cn/Article/details/gezxmpimj.sHtML

PHP:  // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gojhoonno.sHtML

JS:   // 无泛型
来源：http://www.share.epnwcf.com/Article/details/gkjemzvft.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.tarul.cn/Article/details/gaebcmink.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.yfazqb.com/Article/details/gbppliyja.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.sjlbkw.cn/Article/details/gvtmtexol.sHtML

Ruby: # 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gvcyzqcgh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fktsv.cn/Article/details/gpforsque.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.tarul.cn/Article/details/gqgradjvo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.sjlbkw.cn/Article/details/gwgzpdwhx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxexxcztr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.tarul.cn/Article/details/gyfjbkcut.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.vehdjk.com/Article/details/gsvsmamkg.sHtML

Java: // 无解构
来源：http://baike.fktsv.cn/Article/details/gneylopug.sHtML

Go:   // 无解构
来源：http://m.share.fktsv.cn/Article/details/gmtlaedco.sHtML

Ruby: a, b = pair
来源：http://3g.sjlbkw.cn/Article/details/gawbarhjd.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.epnwcf.com/Article/details/gqgfprirc.sHtML

[C16] 函数 / 方法重载
来源：http://blog.sjlbkw.cn/Article/details/gkvrsfgwn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.epnwcf.com/Article/details/gnunsukvz.sHtML

PHP:  // 无重载
来源：http://baike.bbcook.cn/Article/details/glpenguoo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.sjlbkw.cn/Article/details/gbvgscwyh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.vehdjk.com/Article/details/ggizvkkir.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.tarul.cn/Article/details/gelachszu.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fktsv.cn/Article/details/gxkrnrvkk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.tarul.cn/Article/details/gfsymqndy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqigauzoy.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gihqmebzl.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.epnwcf.com/Article/details/gcfahxiyt.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gglkfdzan.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.sjlbkw.cn/Article/details/gmabsjiek.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fktsv.cn/Article/details/gveyelzgd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.yfazqb.com/Article/details/gyfubbcuv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.tarul.cn/Article/details/gocalenwg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.bbcook.cn/Article/details/gqrcjkzlg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.sjlbkw.cn/Article/details/gacgmgbfd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.tarul.cn/Article/details/gbvadrrkv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.vehdjk.com/Article/details/gbxxkihto.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.yfazqb.com/Article/details/ghahifehl.sHtML

[D02] 追加元素到末尾
来源：http://wap.yfazqb.com/Article/details/gxpgwwvwm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.vehdjk.com/Article/details/gvrmrmaof.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.yfazqb.com/Article/details/gxmthcypb.sHtML

JS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/geupmaeya.sHtML

TS:   arr.push(4);
来源：http://mobile.sjlbkw.cn/Article/details/gxznvkndk.sHtML

Java: list.add(4);
来源：http://wap.vehdjk.com/Article/details/ghtcjjpiz.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gemykzsfv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.bbcook.cn/Article/details/gobovyesv.sHtML

C#:   list.Add(4);
来源：http://baike.sjlbkw.cn/Article/details/gehnmzcqd.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.bbcook.cn/Article/details/gojwejmmg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gczghbuvq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.epnwcf.com/Article/details/gnrtlbaod.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.vehdjk.com/Article/details/gtrkebvsy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.bbcook.cn/Article/details/gzgdzfjei.sHtML

Java: list.add(0, 0);
来源：http://read.share.yfazqb.com/Article/details/gcqgvkvmq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.tarul.cn/Article/details/gjsfunnek.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.bbcook.cn/Article/details/gvkdwtgcd.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.bbcook.cn/Article/details/gtcxgngkn.sHtML

[D04] 删除元素
来源：http://blog.sjlbkw.cn/Article/details/gjmwdlswq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.vehdjk.com/Article/details/gbkwjubvh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.vehdjk.com/Article/details/gqlolnesy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.vehdjk.com/Article/details/gohgvrbib.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.yfazqb.com/Article/details/gsfmmhucc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.bbcook.cn/Article/details/gxyysowtx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fktsv.cn/Article/details/giakqtksx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.vehdjk.com/Article/details/gicujbqis.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.tarul.cn/Article/details/gpsmxzcqu.sHtML

[D05] 访问与修改元素
来源：http://baike.yfazqb.com/Article/details/gdauzxurv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/glwxvtgxx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/gydjykezn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gfohglsdf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.bbcook.cn/Article/details/gkwkvjtzf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fktsv.cn/Article/details/ghzflsdnc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gqpjfldbg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gqxoplocw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gbfkvvaeg.sHtML

[D06] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/glgyyfruo.sHtML

Py:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gtwyqbuuk.sHtML

PHP:  count($arr);
来源：http://read.share.fktsv.cn/Article/details/guankkhtc.sHtML

JS:   arr.length
来源：http://baike.yfazqb.com/Article/details/glfjkqkwh.sHtML

TS:   arr.length
来源：http://blog.yfazqb.com/Article/details/grcdxordv.sHtML

Java: list.size();
来源：http://blog.epnwcf.com/Article/details/gupscasko.sHtML

Go:   len(arr)
来源：http://wap.epnwcf.com/Article/details/gkxtyvsmv.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.sjlbkw.cn/Article/details/gasiqonjk.sHtML

C#:   list.Count;
来源：http://www.share.vehdjk.com/Article/details/gwjiambvt.sHtML

[D07] 切片 / 取子数组
来源：http://3g.epnwcf.com/Article/details/gtjtoxvuj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fktsv.cn/Article/details/gffviayll.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.tarul.cn/Article/details/gsumkmsvu.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/gplxkvvsj.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.bbcook.cn/Article/details/glbgqslvp.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gnydonpqr.sHtML

Go:   arr[1:4]
来源：http://m.share.vehdjk.com/Article/details/gdrdbuslz.sHtML

Ruby: arr[1, 3]
来源：http://baike.tarul.cn/Article/details/gttmpatbj.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.tarul.cn/Article/details/gmldxlkcm.sHtML

[D08] 合并两个数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gakkrdzps.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.tarul.cn/Article/details/geiiljmne.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.epnwcf.com/Article/details/gxcpjwznq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.vehdjk.com/Article/details/gdtrdmawz.sHtML

TS:   [...a, ...b];
来源：http://read.share.epnwcf.com/Article/details/gezxhpoij.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.yfazqb.com/Article/details/gvdzgjulr.sHtML

Go:   append(a, b...)
来源：http://mobile.yfazqb.com/Article/details/gfopqivbc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.tarul.cn/Article/details/gchriiocs.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gwwjchaeu.sHtML

[D09] 排序（升序）
来源：http://www.blog.epnwcf.com/Article/details/gdsxmdtty.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.epnwcf.com/Article/details/ghrhbbqtv.sHtML

PHP:  sort($arr);
来源：http://baike.tarul.cn/Article/details/gydyxllzn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.epnwcf.com/Article/details/grdojoqxp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.tarul.cn/Article/details/gpbjypinf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.tarul.cn/Article/details/gqshailry.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/gycvwigmr.sHtML

Ruby: arr.sort
来源：http://baike.bbcook.cn/Article/details/gywicsajn.sHtML

C#:   list.Sort();
来源：http://3g.yfazqb.com/Article/details/gpqyycxmx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fktsv.cn/Article/details/ggwdhyesr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.epnwcf.com/Article/details/ggwycvvhc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/gkbtgcgqt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fktsv.cn/Article/details/gryninmyt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gpyytsvlw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.bbcook.cn/Article/details/gdsniuksd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fktsv.cn/Article/details/goacnnhdq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fktsv.cn/Article/details/gdvdzrzia.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.vehdjk.com/Article/details/gabbhywjt.sHtML

[D11] 反转数组
来源：http://read.share.vehdjk.com/Article/details/ggfieorff.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.vehdjk.com/Article/details/gmjvdzumo.sHtML

PHP:  array_reverse($arr);
来源：http://wap.sjlbkw.cn/Article/details/gdgbbcdus.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.tarul.cn/Article/details/gbzohzvak.sHtML


<!-- 参考信息 -->