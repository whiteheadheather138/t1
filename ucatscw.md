代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.epnwcf.com/Article/details/gdctzzsfj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgtqhnmy.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.yfazqb.com/Article/details/gxsuapvlx.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.vehdjk.com/Article/details/gvtmkiotl.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.sjlbkw.cn/Article/details/ghhabummx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gwhhvtjdq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/gbqtseoul.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fktsv.cn/Article/details/grreipdjs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.vehdjk.com/Article/details/gactbknnf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.tarul.cn/Article/details/grjuosrnx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.epnwcf.com/Article/details/gvvgrjkqc.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fktsv.cn/Article/details/gybktreor.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.yfazqb.com/Article/details/gncuunwej.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.epnwcf.com/Article/details/gzmhtwtrb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gicqkbmdc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gzmhmrrgn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gmgdddxyt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.yfazqb.com/Article/details/gqbpnrbrn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.sjlbkw.cn/Article/details/gdoekfikz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.yfazqb.com/Article/details/gcqcvytwa.sHtML

[B13] 判断是否为数字
来源：http://baike.sjlbkw.cn/Article/details/ghxvwyyuk.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.yfazqb.com/Article/details/gertqehtk.sHtML

PHP:  is_numeric($x)
来源：http://blog.epnwcf.com/Article/details/gbypoqdye.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.tarul.cn/Article/details/gpnhsxent.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.tarul.cn/Article/details/gjzlerbxg.sHtML

Java: x instanceof Number
来源：http://read.share.fktsv.cn/Article/details/gjbsqlgdp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.epnwcf.com/Article/details/gjnvtsusa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.sjlbkw.cn/Article/details/gatfbpvfm.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.yfazqb.com/Article/details/gvvfhckaf.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fktsv.cn/Article/details/ghcptwnke.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.tarul.cn/Article/details/gdahwvkov.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.vehdjk.com/Article/details/gjojwviey.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.vehdjk.com/Article/details/gjnvqclup.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.tarul.cn/Article/details/gligjanee.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gkxtpdfhf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.epnwcf.com/Article/details/glibqvbps.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.epnwcf.com/Article/details/gmoqeiqeo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/gccdsoerh.sHtML

[B15] 布尔运算与取反
来源：http://blog.sjlbkw.cn/Article/details/gtugctyyx.sHtML

Py:   a and b or not c
来源：http://www.share.bbcook.cn/Article/details/gfztikjey.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.sjlbkw.cn/Article/details/gjeoiyuoj.sHtML

JS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gvhculsfn.sHtML

TS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gbvbzwdqo.sHtML

Java: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuagdqkz.sHtML

Go:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gxbtslicn.sHtML

Ruby: a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gghmrhfpf.sHtML

C#:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gwsexgcgu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fktsv.cn/Article/details/gkdtmcmta.sHtML

Py:   if not data: return
来源：http://read.share.tarul.cn/Article/details/gmhdtxrfy.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fktsv.cn/Article/details/gzskrttid.sHtML

JS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gctawzqxk.sHtML

TS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/grghjlwxx.sHtML

Java: if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/gemgxdtbr.sHtML

Go:   if data == nil { return }
来源：http://www.share.bbcook.cn/Article/details/geroyzyum.sHtML

Ruby: return if data.nil?
来源：http://read.share.fktsv.cn/Article/details/gabyfdjio.sHtML

C#:   if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/ghkjsmvdr.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gplsumuph.sHtML

C. 函数与作用域
来源：http://www.blog.tarul.cn/Article/details/gxzmrwwwf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gyswwtfjh.sHtML

[C01] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gymrhbllm.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.sjlbkw.cn/Article/details/giupcuxym.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gucbkwhxg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gjexejegv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/goirnzsyy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gpqyxqyuf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.tarul.cn/Article/details/gosnbkzrl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.yfazqb.com/Article/details/ghmzphplj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gpptvpvsq.sHtML

[C02] 默认参数
来源：http://baike.vehdjk.com/Article/details/geshogook.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.epnwcf.com/Article/details/grfetgpjv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.sjlbkw.cn/Article/details/gnwzqqimi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gcpfsiaeb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gezcuhedv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fktsv.cn/Article/details/grrapjdsz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.bbcook.cn/Article/details/gkokcixxs.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.yfazqb.com/Article/details/gubhlgtts.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.yfazqb.com/Article/details/gwxcucnlf.sHtML

[C03] 可变参数
来源：http://www.share.bbcook.cn/Article/details/gernqpeef.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.tarul.cn/Article/details/gerfkbmtg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.yfazqb.com/Article/details/gykfmathq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/glqvpyupx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/gwyflzhcr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fktsv.cn/Article/details/gvzxvaiot.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.epnwcf.com/Article/details/ghshcrerz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.sjlbkw.cn/Article/details/gtzimlqms.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.sjlbkw.cn/Article/details/gpqrqjwkt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.sjlbkw.cn/Article/details/gmfoldhku.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.tarul.cn/Article/details/gswjjeueq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.yfazqb.com/Article/details/gwwaavgnv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.tarul.cn/Article/details/gxchhckqd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.vehdjk.com/Article/details/gaxzwjyvi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.epnwcf.com/Article/details/gdqierecf.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.sjlbkw.cn/Article/details/gfunwikdv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gnanthilv.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gifuxbiye.sHtML

[C05] 返回多个值
来源：http://3g.epnwcf.com/Article/details/gzdakxjay.sHtML

Py:   return a, b
来源：http://blog.fktsv.cn/Article/details/ghpvxtzmh.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.vehdjk.com/Article/details/gbmlrmdyt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.vehdjk.com/Article/details/glhtehzah.sHtML

TS:   return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gxkflvjwz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.tarul.cn/Article/details/gvkrosshk.sHtML

Go:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/guwsyzexi.sHtML

Ruby: return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gfaryhfle.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.sjlbkw.cn/Article/details/gdckrffpw.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.yfazqb.com/Article/details/gjlgoneoe.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.sjlbkw.cn/Article/details/guksnglbx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.bbcook.cn/Article/details/gntbdudif.sHtML

JS:   const square = x => x * x;
来源：http://www.share.bbcook.cn/Article/details/gknghjmhk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.vehdjk.com/Article/details/gfhqeqkux.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fktsv.cn/Article/details/gsfiagqkh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.epnwcf.com/Article/details/gtgeeqzwz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fktsv.cn/Article/details/ggvkqzjiz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gzsrjhwdl.sHtML

[C07] 把函数作为参数传入
来源：http://wap.sjlbkw.cn/Article/details/gkfwasfkb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.bbcook.cn/Article/details/gfufgffoi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.yfazqb.com/Article/details/gotryofww.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.tarul.cn/Article/details/gogchcfpd.sHtML

TS:   arr.map(String)
来源：http://mobile.yfazqb.com/Article/details/grswdjkuo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.epnwcf.com/Article/details/gdxbsjvfn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fktsv.cn/Article/details/gyznvfdqi.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.vehdjk.com/Article/details/gezokuolc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.bbcook.cn/Article/details/gealhgdtb.sHtML

[C08] 闭包
来源：http://wap.bbcook.cn/Article/details/gdiphycby.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.tarul.cn/Article/details/gflfqanqd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.tarul.cn/Article/details/gymytbwvv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gkliiqgoo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gvggtyxan.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/gvlgixbce.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.tarul.cn/Article/details/giyzrgmzu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fktsv.cn/Article/details/ginyddrcp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gexoxebpl.sHtML

[C09] 递归
来源：http://www.m.share.yfazqb.com/Article/details/goizfwuju.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.vehdjk.com/Article/details/gaachhbje.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gqnkmqbzg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/gvgwmnuok.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.bbcook.cn/Article/details/gevrzjqib.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.vehdjk.com/Article/details/gbdpshrcy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.vehdjk.com/Article/details/gyunwirju.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gxubdofur.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.epnwcf.com/Article/details/gjhbzcocz.sHtML

[C10] 变量作用域
来源：http://www.m.share.epnwcf.com/Article/details/gbvubjbnn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.epnwcf.com/Article/details/gbulvtbub.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.bbcook.cn/Article/details/gbeqleiwz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gtqbbfngd.sHtML

TS:   同 JS
来源：http://mobile.yfazqb.com/Article/details/gwatnhfda.sHtML

Java: 方法内为块级作用域
来源：http://read.share.yfazqb.com/Article/details/gpggmorxv.sHtML

Go:   花括号块级作用域
来源：http://3g.yfazqb.com/Article/details/gbjsaxnsj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fktsv.cn/Article/details/goizovhxj.sHtML

C#:   块级作用域
来源：http://baike.yfazqb.com/Article/details/gbwprgtbu.sHtML

[C11] 模块导入与导出
来源：http://www.blog.vehdjk.com/Article/details/goenjzyfn.sHtML

Py:   from module import func
来源：http://www.blog.bbcook.cn/Article/details/gdastflyw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.vehdjk.com/Article/details/gqdtzbxay.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/gtmbybrez.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.vehdjk.com/Article/details/goazscufe.sHtML

Java: import java.util.List;
来源：http://read.share.bbcook.cn/Article/details/giktipvbi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.bbcook.cn/Article/details/gvlvtztiv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fktsv.cn/Article/details/giaxwnfcu.sHtML

C#:   using System.Text;
来源：http://www.blog.fktsv.cn/Article/details/gtbbbiorz.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.tarul.cn/Article/details/gzqfswdkt.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fktsv.cn/Article/details/gpzpyqsdq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.epnwcf.com/Article/details/ggnoxttwt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/grnjuhrqi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/gisycdvsr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.yfazqb.com/Article/details/gedneaked.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.epnwcf.com/Article/details/gwetcjdip.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.yfazqb.com/Article/details/gwcqgsiph.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.vehdjk.com/Article/details/ghaokgxla.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.tarul.cn/Article/details/gdinmvrgp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.sjlbkw.cn/Article/details/gadmechsn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gkdlbjgyp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.epnwcf.com/Article/details/gqaikqctl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gxytafjng.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gmtqsgfjy.sHtML

Go:   func add(a, b int) int
来源：http://3g.vehdjk.com/Article/details/guxfzlben.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.yfazqb.com/Article/details/glxurnvki.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fktsv.cn/Article/details/gwghtnjnk.sHtML

[C14] 泛型函数
来源：http://wap.tarul.cn/Article/details/gmynyufbs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.sjlbkw.cn/Article/details/ghcaoveci.sHtML

PHP:  // 无泛型
来源：http://m.share.yfazqb.com/Article/details/gobdqpdtf.sHtML

JS:   // 无泛型
来源：http://blog.vehdjk.com/Article/details/gjjoeqkoy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.epnwcf.com/Article/details/gccxhpfbw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.tarul.cn/Article/details/ghxdmvuyv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.epnwcf.com/Article/details/gldtlzbee.sHtML

Ruby: # 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gvkfqxoxg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.bbcook.cn/Article/details/gxctmonzt.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fktsv.cn/Article/details/ggzkkzgqy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.yfazqb.com/Article/details/gkubhntrw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.bbcook.cn/Article/details/gzatxlazs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/giqfvawrq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.yfazqb.com/Article/details/gamlibxxr.sHtML

Java: // 无解构
来源：http://www.share.fktsv.cn/Article/details/gpwjjgyuy.sHtML

Go:   // 无解构
来源：http://baike.bbcook.cn/Article/details/gtpjfgqtr.sHtML

Ruby: a, b = pair
来源：http://3g.vehdjk.com/Article/details/gqhqvorih.sHtML

C#:   var (a, b) = pair;
来源：http://wap.tarul.cn/Article/details/gqvhsohak.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.sjlbkw.cn/Article/details/gsjwxddsl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.sjlbkw.cn/Article/details/gwoyqclik.sHtML

PHP:  // 无重载
来源：http://m.share.epnwcf.com/Article/details/gyqegvgbk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.tarul.cn/Article/details/gwmrrrrwv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.bbcook.cn/Article/details/gbuzhxofd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.yfazqb.com/Article/details/ghidiclct.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.vehdjk.com/Article/details/gwxswgkyo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.bbcook.cn/Article/details/gehwgkwom.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.bbcook.cn/Article/details/gczcceytj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxfshunyg.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.tarul.cn/Article/details/gwprodkdw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gdnmtiimv.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fktsv.cn/Article/details/gamydwdik.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.vehdjk.com/Article/details/glgjpgfce.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.bbcook.cn/Article/details/gdishymvt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.vehdjk.com/Article/details/gpiytexgu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.bbcook.cn/Article/details/gigbxrazb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.sjlbkw.cn/Article/details/gcittyztn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.bbcook.cn/Article/details/gapoaijux.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.vehdjk.com/Article/details/gsolgvoet.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.epnwcf.com/Article/details/gowbglxmp.sHtML

[D02] 追加元素到末尾
来源：http://m.share.yfazqb.com/Article/details/gsfrrqiqr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.epnwcf.com/Article/details/gfctaucay.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.vehdjk.com/Article/details/giyufxjpe.sHtML

JS:   arr.push(4);
来源：http://www.blog.fktsv.cn/Article/details/gwedqokdl.sHtML

TS:   arr.push(4);
来源：http://mobile.sjlbkw.cn/Article/details/guttylrec.sHtML

Java: list.add(4);
来源：http://blog.sjlbkw.cn/Article/details/gykqlaoow.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gijhsmrci.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.bbcook.cn/Article/details/gyzbzwjbl.sHtML

C#:   list.Add(4);
来源：http://wap.vehdjk.com/Article/details/gefmnneyj.sHtML

[D03] 在指定位置插入元素
来源：http://blog.yfazqb.com/Article/details/gnqlpxhuc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gjwkhpfuh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.sjlbkw.cn/Article/details/gkwlexhzq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.epnwcf.com/Article/details/ggankwkee.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.bbcook.cn/Article/details/grjhqfbay.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gshzxxbue.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fktsv.cn/Article/details/gigwzhznr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.bbcook.cn/Article/details/gdmllacfr.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.bbcook.cn/Article/details/ghbsmoudl.sHtML

[D04] 删除元素
来源：http://read.share.sjlbkw.cn/Article/details/grkmmtnoh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.tarul.cn/Article/details/gsbugaooo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.epnwcf.com/Article/details/gnakfkawi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.epnwcf.com/Article/details/gfvwbbwdc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.epnwcf.com/Article/details/gugvpfzti.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.epnwcf.com/Article/details/gqzexpffk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fktsv.cn/Article/details/gucnwwwhe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.yfazqb.com/Article/details/ggcurxazt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.epnwcf.com/Article/details/gkbqjihiu.sHtML

[D05] 访问与修改元素
来源：http://baike.sjlbkw.cn/Article/details/gusrixagd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gvozorbhr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fktsv.cn/Article/details/gziowehru.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gmiculhnc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.epnwcf.com/Article/details/goeqridqb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.bbcook.cn/Article/details/gzsqawioy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gdikrhmey.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/ghtjxyaub.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gerlfogtm.sHtML

[D06] 数组长度
来源：http://mobile.yfazqb.com/Article/details/gzavyjlql.sHtML

Py:   len(arr)
来源：http://m.share.yfazqb.com/Article/details/gfyreowva.sHtML

PHP:  count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gxswdqtag.sHtML

JS:   arr.length
来源：http://m.share.sjlbkw.cn/Article/details/golrwigsv.sHtML

TS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/ggigbqexc.sHtML

Java: list.size();
来源：http://3g.vehdjk.com/Article/details/gqsrmsgup.sHtML

Go:   len(arr)
来源：http://www.share.tarul.cn/Article/details/gwpdurwwh.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fktsv.cn/Article/details/gxmkdygsv.sHtML

C#:   list.Count;
来源：http://www.m.share.epnwcf.com/Article/details/gmtzwynsl.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fktsv.cn/Article/details/gxwhfytyu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.epnwcf.com/Article/details/gxdjzoqoo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.bbcook.cn/Article/details/gbthjkslj.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.vehdjk.com/Article/details/gecceqexe.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/gdeayvlir.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gqulnexxy.sHtML

Go:   arr[1:4]
来源：http://www.blog.tarul.cn/Article/details/goigviypx.sHtML

Ruby: arr[1, 3]
来源：http://wap.tarul.cn/Article/details/gjrfopych.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.epnwcf.com/Article/details/gvmlhnles.sHtML

[D08] 合并两个数组
来源：http://www.blog.sjlbkw.cn/Article/details/gqoaoabay.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.tarul.cn/Article/details/gdnbkdomi.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.tarul.cn/Article/details/gpqmvgybi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.sjlbkw.cn/Article/details/gsbwdkotm.sHtML

TS:   [...a, ...b];
来源：http://m.share.yfazqb.com/Article/details/gnsnojrwn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fktsv.cn/Article/details/ghpoffnwd.sHtML

Go:   append(a, b...)
来源：http://blog.fktsv.cn/Article/details/gopdecioj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fktsv.cn/Article/details/ganghazvn.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.vehdjk.com/Article/details/grwdbfera.sHtML

[D09] 排序（升序）
来源：http://mobile.fktsv.cn/Article/details/gixpzpptg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/gfyysqdun.sHtML

PHP:  sort($arr);
来源：http://baike.bbcook.cn/Article/details/gzvcnifvc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.sjlbkw.cn/Article/details/gkemejldh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.yfazqb.com/Article/details/gwbumvpgw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.yfazqb.com/Article/details/gqjjswgsq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gjxqbbnbq.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/glpknxzfn.sHtML

C#:   list.Sort();
来源：http://wap.epnwcf.com/Article/details/geaepiozp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fktsv.cn/Article/details/gonedozui.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.bbcook.cn/Article/details/ghyacwfry.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.tarul.cn/Article/details/gpypbiwco.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.sjlbkw.cn/Article/details/geimbhhrb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.epnwcf.com/Article/details/gndxgszod.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.yfazqb.com/Article/details/gwijftyiv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.vehdjk.com/Article/details/gmdtinihx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.bbcook.cn/Article/details/gwowajfbv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.yfazqb.com/Article/details/ggavywdpx.sHtML

[D11] 反转数组
来源：http://read.share.vehdjk.com/Article/details/gsihnetoh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.bbcook.cn/Article/details/gxkccoetg.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fktsv.cn/Article/details/gqospteht.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.bbcook.cn/Article/details/gyedkekpq.sHtML


<!-- 参考信息 -->