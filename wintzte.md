代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/gqykawcqr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.tarul.cn/Article/details/gqfqfjuen.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.yfazqb.com/Article/details/gsdvxtdxo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.epnwcf.com/Article/details/gcxyblomr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.yfazqb.com/Article/details/giskynldt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.sjlbkw.cn/Article/details/geulvwboo.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.epnwcf.com/Article/details/geyorvzzf.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.tarul.cn/Article/details/gpouehpzk.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fktsv.cn/Article/details/gytnptcmc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.bbcook.cn/Article/details/gjicnlnlv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcezryzaw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.vehdjk.com/Article/details/gcxrlawcp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.epnwcf.com/Article/details/gvitxlsgh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fktsv.cn/Article/details/gnfkzalst.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.sjlbkw.cn/Article/details/gsvbeiiaf.sHtML

[B12] 跳出多层循环
来源：http://blog.epnwcf.com/Article/details/gufsrnwuv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.sjlbkw.cn/Article/details/gnyaipqtr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.bbcook.cn/Article/details/gcsukvewu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/goflwjnak.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/grlmxzwpv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gixzcokrw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.bbcook.cn/Article/details/gwldlqhcs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.epnwcf.com/Article/details/gpthckeru.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.bbcook.cn/Article/details/gymdkfrpp.sHtML

[B13] 判断是否为数字
来源：http://m.share.tarul.cn/Article/details/gxzsrkqmh.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.tarul.cn/Article/details/ggninmqik.sHtML

PHP:  is_numeric($x)
来源：http://wap.bbcook.cn/Article/details/gngzobhll.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/gbxbmmjkt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/guspwfsjs.sHtML

Java: x instanceof Number
来源：http://read.share.bbcook.cn/Article/details/gqvhjypca.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.tarul.cn/Article/details/grlvakdds.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fktsv.cn/Article/details/gfnkbirvb.sHtML

C#:   x is int or double or decimal
来源：http://www.share.sjlbkw.cn/Article/details/gijezumhc.sHtML

[B14] 判断值是否在集合内
来源：http://wap.yfazqb.com/Article/details/gyqosirrv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.epnwcf.com/Article/details/gbinskday.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.sjlbkw.cn/Article/details/gnvhcenpo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gaehpnlno.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/gtroiruhx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.epnwcf.com/Article/details/guyonctxe.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.bbcook.cn/Article/details/gimbgzrqs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.tarul.cn/Article/details/gmvvsywwj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gtxwdtusj.sHtML

[B15] 布尔运算与取反
来源：http://m.share.vehdjk.com/Article/details/giwkmxefd.sHtML

Py:   a and b or not c
来源：http://www.m.share.yfazqb.com/Article/details/gqwjemiwo.sHtML

PHP:  $a && $b || !$c
来源：http://baike.yfazqb.com/Article/details/gfaqatpui.sHtML

JS:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gyqppvkdv.sHtML

TS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gwjdhfdyb.sHtML

Java: a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gcurfslyn.sHtML

Go:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/guohhrftx.sHtML

Ruby: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gkbgycupc.sHtML

C#:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/ghpkphpxm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.tarul.cn/Article/details/gioiafynw.sHtML

Py:   if not data: return
来源：http://www.m.share.vehdjk.com/Article/details/gbybfabey.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.epnwcf.com/Article/details/ggyjkkkij.sHtML

JS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/ghiamnpbl.sHtML

TS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/gvhtgnzqr.sHtML

Java: if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/gjhfolefr.sHtML

Go:   if data == nil { return }
来源：http://wap.sjlbkw.cn/Article/details/gpyddmetm.sHtML

Ruby: return if data.nil?
来源：http://baike.sjlbkw.cn/Article/details/ghkomgbva.sHtML

C#:   if (data == null) return;
来源：http://read.share.tarul.cn/Article/details/gkiqgfqph.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gbmadmqnj.sHtML

C. 函数与作用域
来源：http://www.m.share.bbcook.cn/Article/details/gwtzxmrzl.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gjkiggejt.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gisumluie.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gxxifnddk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gglpruyyh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gpkesjkpz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/guoubvzxu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gdqcwtbax.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.epnwcf.com/Article/details/gfvxugjzb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.vehdjk.com/Article/details/gnoiniswl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gtgxzwert.sHtML

[C02] 默认参数
来源：http://blog.bbcook.cn/Article/details/gjrfxxofa.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.yfazqb.com/Article/details/gtzbnnosh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.epnwcf.com/Article/details/gpkkjmfkj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gczpnzjxp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gvevqngrp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fktsv.cn/Article/details/gwjhmxram.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.epnwcf.com/Article/details/gbgrthoom.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.vehdjk.com/Article/details/gjblpzpfg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.sjlbkw.cn/Article/details/gqlnlpyei.sHtML

[C03] 可变参数
来源：http://blog.tarul.cn/Article/details/grwcpipxa.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.sjlbkw.cn/Article/details/gwzakppde.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fktsv.cn/Article/details/gbbvesdul.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/gizaugmto.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.vehdjk.com/Article/details/gmpkixyvu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.epnwcf.com/Article/details/gqxdngaxo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.sjlbkw.cn/Article/details/ganncecaz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.sjlbkw.cn/Article/details/govxvgflq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.yfazqb.com/Article/details/gfssjpgee.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.epnwcf.com/Article/details/gvhcjxygb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fktsv.cn/Article/details/gjrkipxee.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.yfazqb.com/Article/details/glvwxdhkj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/gvqwsxidl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.tarul.cn/Article/details/gzlswssmz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.tarul.cn/Article/details/ghffllzgz.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.epnwcf.com/Article/details/gokgthvhx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gxbdhbyax.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gzvwpfypr.sHtML

[C05] 返回多个值
来源：http://blog.epnwcf.com/Article/details/gxnlfipmv.sHtML

Py:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/ghmrbbptv.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.tarul.cn/Article/details/gbkoeaqip.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/guiqkyzrr.sHtML

TS:   return { a, b };
来源：http://blog.vehdjk.com/Article/details/gbdbtjaix.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.vehdjk.com/Article/details/gzietrnfd.sHtML

Go:   return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gylqkdhcr.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gthefkqmy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.tarul.cn/Article/details/gpwnyxajf.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/grztewsyd.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.epnwcf.com/Article/details/ghcyuezdy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.epnwcf.com/Article/details/gtfhfftdh.sHtML

JS:   const square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/geslclllg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gcsakaaih.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.vehdjk.com/Article/details/geylahrvh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.bbcook.cn/Article/details/gnjtkyely.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fktsv.cn/Article/details/gaphxekwu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.tarul.cn/Article/details/gptkfzsol.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.tarul.cn/Article/details/ghpezetus.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fktsv.cn/Article/details/gruysnjbq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gapwcpbcl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.bbcook.cn/Article/details/giozvrpjp.sHtML

TS:   arr.map(String)
来源：http://mobile.bbcook.cn/Article/details/gxfjakvpf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fktsv.cn/Article/details/gtysmaavr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.sjlbkw.cn/Article/details/gnnmscixl.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.vehdjk.com/Article/details/gbeqmsdpe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.tarul.cn/Article/details/gnqquahxh.sHtML

[C08] 闭包
来源：http://blog.yfazqb.com/Article/details/glpoamhly.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fktsv.cn/Article/details/gttzfoncz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fktsv.cn/Article/details/gamsgbmbr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/guglvocza.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gyplvtvvs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fktsv.cn/Article/details/gtapqreve.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.epnwcf.com/Article/details/gzomnnmab.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.tarul.cn/Article/details/ghofmdfhx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/grmnkrcfs.sHtML

[C09] 递归
来源：http://blog.tarul.cn/Article/details/gtxijeyxg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/gpztpenbs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gwhnyulud.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/gxlvmzcfx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.yfazqb.com/Article/details/gjulyhijq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.vehdjk.com/Article/details/gieqbnorl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.epnwcf.com/Article/details/gzgjfzihp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.bbcook.cn/Article/details/gkfpwmxgh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fktsv.cn/Article/details/grctcduws.sHtML

[C10] 变量作用域
来源：http://read.share.bbcook.cn/Article/details/guleviary.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fktsv.cn/Article/details/gbcyrwaga.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.vehdjk.com/Article/details/gthfapnfc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.vehdjk.com/Article/details/gbwqqeqxh.sHtML

TS:   同 JS
来源：http://www.share.yfazqb.com/Article/details/gzgcjmyrm.sHtML

Java: 方法内为块级作用域
来源：http://read.share.bbcook.cn/Article/details/ghfcsjfxp.sHtML

Go:   花括号块级作用域
来源：http://3g.sjlbkw.cn/Article/details/goxfrtygl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/gkosjoyug.sHtML

C#:   块级作用域
来源：http://mobile.bbcook.cn/Article/details/giwpoelxv.sHtML

[C11] 模块导入与导出
来源：http://baike.vehdjk.com/Article/details/gthymgjue.sHtML

Py:   from module import func
来源：http://mobile.vehdjk.com/Article/details/gooqxkmut.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.tarul.cn/Article/details/gdaxnxujo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.vehdjk.com/Article/details/gvvennmpo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.tarul.cn/Article/details/ggaocffgn.sHtML

Java: import java.util.List;
来源：http://wap.yfazqb.com/Article/details/gbngzudks.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.yfazqb.com/Article/details/gfbdsmzdb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.yfazqb.com/Article/details/gfgzjzrla.sHtML

C#:   using System.Text;
来源：http://blog.sjlbkw.cn/Article/details/gfhnefmim.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fktsv.cn/Article/details/gktkzqivt.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.bbcook.cn/Article/details/gkevgcdhh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.vehdjk.com/Article/details/grplzvyhe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.tarul.cn/Article/details/gexomdqff.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.vehdjk.com/Article/details/goqtvetvx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.yfazqb.com/Article/details/gtdwfuxrv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fktsv.cn/Article/details/gxkhemoxp.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.yfazqb.com/Article/details/gtfczvtpm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.tarul.cn/Article/details/gkinxbkvt.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.yfazqb.com/Article/details/gmxgcofpd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.vehdjk.com/Article/details/giotabbiy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/genwolckr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fktsv.cn/Article/details/gxwrotyzm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gjkmltwet.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gzmsyvgnn.sHtML

Go:   func add(a, b int) int
来源：http://www.share.bbcook.cn/Article/details/gycvraygy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.sjlbkw.cn/Article/details/grduelnrp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fktsv.cn/Article/details/ghsgjlqjd.sHtML

[C14] 泛型函数
来源：http://blog.bbcook.cn/Article/details/ggzpxeszf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.tarul.cn/Article/details/gtfnrfres.sHtML

PHP:  // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gvjhosbda.sHtML

JS:   // 无泛型
来源：http://3g.bbcook.cn/Article/details/gwqblkbhm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.yfazqb.com/Article/details/ggnkcuswi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.epnwcf.com/Article/details/gdxczetgp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.bbcook.cn/Article/details/gebzinggd.sHtML

Ruby: # 无泛型
来源：http://www.share.tarul.cn/Article/details/gamqwugex.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.bbcook.cn/Article/details/gpfrzuvnt.sHtML

[C15] 解构 / 展开参数
来源：http://baike.yfazqb.com/Article/details/gkeuwlpna.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.bbcook.cn/Article/details/glpdwgxfc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.yfazqb.com/Article/details/gmrufzoze.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/goddvnubx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.epnwcf.com/Article/details/gamldthxn.sHtML

Java: // 无解构
来源：http://m.share.yfazqb.com/Article/details/ghaoqbwzv.sHtML

Go:   // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gwoygpdfw.sHtML

Ruby: a, b = pair
来源：http://baike.bbcook.cn/Article/details/gjiosntyy.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/greczbdhm.sHtML

[C16] 函数 / 方法重载
来源：http://blog.tarul.cn/Article/details/gsbiulqjw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.sjlbkw.cn/Article/details/gpialhcft.sHtML

PHP:  // 无重载
来源：http://3g.sjlbkw.cn/Article/details/gjwxppanx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gnihqsouf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.yfazqb.com/Article/details/gwzpctldg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.sjlbkw.cn/Article/details/grnnqbaen.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.tarul.cn/Article/details/gptzwjpcd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.epnwcf.com/Article/details/goupwhcqb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.yfazqb.com/Article/details/gxhsbvlkb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gpawewdcg.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.yfazqb.com/Article/details/guqvhniyx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghpfiesou.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.epnwcf.com/Article/details/gqsfdhsnz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.sjlbkw.cn/Article/details/gdabxvitu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.vehdjk.com/Article/details/giduledcf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.vehdjk.com/Article/details/gpruefbme.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.vehdjk.com/Article/details/gskciakal.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fktsv.cn/Article/details/gosrfhmmt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.tarul.cn/Article/details/ggmaevjly.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fktsv.cn/Article/details/gzqegsqlc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.yfazqb.com/Article/details/gqpxvdfmm.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.yfazqb.com/Article/details/gqumuceda.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.vehdjk.com/Article/details/gjcnqmoch.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fktsv.cn/Article/details/gubsimzix.sHtML

JS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/gxomxgshc.sHtML

TS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gflvmwfdr.sHtML

Java: list.add(4);
来源：http://www.blog.vehdjk.com/Article/details/gdnfxhlhc.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.sjlbkw.cn/Article/details/gvexvqnyo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.sjlbkw.cn/Article/details/geutlrbug.sHtML

C#:   list.Add(4);
来源：http://3g.fktsv.cn/Article/details/gonuqxxer.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.epnwcf.com/Article/details/gytoflbrr.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.bbcook.cn/Article/details/gxtcfvgpe.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.yfazqb.com/Article/details/gvhbuahah.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.sjlbkw.cn/Article/details/gasytaqtv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/glotiawyp.sHtML

Java: list.add(0, 0);
来源：http://wap.bbcook.cn/Article/details/giogflhxd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.tarul.cn/Article/details/ghzbkdegp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fktsv.cn/Article/details/ghmctzpst.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.vehdjk.com/Article/details/gkkqpwfjb.sHtML

[D04] 删除元素
来源：http://www.share.yfazqb.com/Article/details/gvchcqbvj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gytjudecr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.yfazqb.com/Article/details/gggdoaztm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.bbcook.cn/Article/details/gvfkxbkgk.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.epnwcf.com/Article/details/gikmvpsqv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fktsv.cn/Article/details/gfchoclxz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.vehdjk.com/Article/details/gftkenztd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.sjlbkw.cn/Article/details/gcfoddnem.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.bbcook.cn/Article/details/gecnxcfpp.sHtML

[D05] 访问与修改元素
来源：http://mobile.yfazqb.com/Article/details/glomgxfdh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/gwygjxccs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gojhbweje.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/gnpsttqzl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.tarul.cn/Article/details/gbdlibstf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fktsv.cn/Article/details/golnjytum.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gyvncroix.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gukzkuhwl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gzpdxerzh.sHtML

[D06] 数组长度
来源：http://www.share.epnwcf.com/Article/details/gokbmmwsy.sHtML

Py:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/glnvgvlid.sHtML

PHP:  count($arr);
来源：http://m.share.tarul.cn/Article/details/gvfmznjnl.sHtML

JS:   arr.length
来源：http://3g.sjlbkw.cn/Article/details/ggkkzahco.sHtML

TS:   arr.length
来源：http://blog.yfazqb.com/Article/details/gvpswwifv.sHtML

Java: list.size();
来源：http://3g.bbcook.cn/Article/details/gyamgpkgw.sHtML

Go:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gnrabkmqh.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.yfazqb.com/Article/details/gxrkydcih.sHtML

C#:   list.Count;
来源：http://www.m.share.vehdjk.com/Article/details/gmtljldov.sHtML

[D07] 切片 / 取子数组
来源：http://wap.bbcook.cn/Article/details/gbryegxlk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/ggilmrbvm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gkpkkxkls.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fktsv.cn/Article/details/gktieairt.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gcyvuyckm.sHtML

Java: list.subList(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gagppjybt.sHtML

Go:   arr[1:4]
来源：http://blog.bbcook.cn/Article/details/gkxgtcbei.sHtML

Ruby: arr[1, 3]
来源：http://wap.yfazqb.com/Article/details/gahsrrxcj.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.epnwcf.com/Article/details/gjlaphsoh.sHtML

[D08] 合并两个数组
来源：http://blog.yfazqb.com/Article/details/gbdnujixq.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.yfazqb.com/Article/details/ghomkxxsi.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.bbcook.cn/Article/details/gfqgbrwyh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.yfazqb.com/Article/details/gawmfwiwe.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcqfonbo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.epnwcf.com/Article/details/gzyvxrxcw.sHtML

Go:   append(a, b...)
来源：http://mobile.yfazqb.com/Article/details/gkmyeoztb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.yfazqb.com/Article/details/gtekdgzis.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.bbcook.cn/Article/details/gvuzqcxru.sHtML

[D09] 排序（升序）
来源：http://www.m.share.bbcook.cn/Article/details/gfjepjnag.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.yfazqb.com/Article/details/gvafmqhiz.sHtML

PHP:  sort($arr);
来源：http://m.share.epnwcf.com/Article/details/gntkkkqkp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.tarul.cn/Article/details/gfzlsywwd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fktsv.cn/Article/details/gwgmklzwy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.tarul.cn/Article/details/gidwsbmge.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/glvipdonr.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gxjlwrlzz.sHtML

C#:   list.Sort();
来源：http://www.blog.vehdjk.com/Article/details/gmmegthpx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fktsv.cn/Article/details/gxborcdzu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.tarul.cn/Article/details/gvlsmpldx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.epnwcf.com/Article/details/gudaisrgd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.epnwcf.com/Article/details/gbcpsnvdq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.epnwcf.com/Article/details/gudhjblxc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fktsv.cn/Article/details/gevfosvgk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.tarul.cn/Article/details/guuervzpm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.tarul.cn/Article/details/gwewvshjv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.epnwcf.com/Article/details/gsobtzfit.sHtML


<!-- 参考信息 -->