代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gfqcsvbcn.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fktsv.cn/Article/details/gyshvrlbv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.yfazqb.com/Article/details/gftixyazu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.sjlbkw.cn/Article/details/grtenpsts.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/glxvopfhn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gjzkztnon.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.tarul.cn/Article/details/gmnysesnq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.bbcook.cn/Article/details/gksncnewz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.tarul.cn/Article/details/ggwqrpfrq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.yfazqb.com/Article/details/gtpppwbzn.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.vehdjk.com/Article/details/gfxlnyozs.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.epnwcf.com/Article/details/gzzzoelok.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.tarul.cn/Article/details/gfhsvbbvo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fktsv.cn/Article/details/gnhprqqna.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fktsv.cn/Article/details/gvnimyvfx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.tarul.cn/Article/details/gwxgyggwa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.yfazqb.com/Article/details/gbvtkknrj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.sjlbkw.cn/Article/details/gefhlxrsj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fktsv.cn/Article/details/guunvhomi.sHtML

[B12] 跳出多层循环
来源：http://m.share.vehdjk.com/Article/details/glwoydopw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.yfazqb.com/Article/details/ggutvpjgr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.vehdjk.com/Article/details/gdiudmrrt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/gmtdhqrwc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gtimliptc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gjytvvhlu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.bbcook.cn/Article/details/gzajpiqhz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.bbcook.cn/Article/details/gnzqcomah.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.vehdjk.com/Article/details/gnmebjkbs.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gqikbqvsj.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.tarul.cn/Article/details/gdzpjrgrb.sHtML

PHP:  is_numeric($x)
来源：http://www.share.yfazqb.com/Article/details/gnixwckbh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.epnwcf.com/Article/details/giigamvmk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.tarul.cn/Article/details/gvwvgzwok.sHtML

Java: x instanceof Number
来源：http://blog.vehdjk.com/Article/details/guryxxsww.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.sjlbkw.cn/Article/details/gvnfhkdrr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.bbcook.cn/Article/details/gqvlrrfav.sHtML

C#:   x is int or double or decimal
来源：http://blog.vehdjk.com/Article/details/girniykgm.sHtML

[B14] 判断值是否在集合内
来源：http://3g.tarul.cn/Article/details/gjeuuofmo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.epnwcf.com/Article/details/gdwhulfpx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.vehdjk.com/Article/details/gndvtjbkp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/glsslfbbv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fktsv.cn/Article/details/ghamqvgyn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.epnwcf.com/Article/details/gxvukdmft.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxzgrgwd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.tarul.cn/Article/details/gtfwcdcnc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fktsv.cn/Article/details/gudagktqr.sHtML

[B15] 布尔运算与取反
来源：http://mobile.yfazqb.com/Article/details/gyzuqngds.sHtML

Py:   a and b or not c
来源：http://3g.vehdjk.com/Article/details/gxunzhfpx.sHtML

PHP:  $a && $b || !$c
来源：http://baike.sjlbkw.cn/Article/details/gjuzmismu.sHtML

JS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/galttgcxo.sHtML

TS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gkwauswit.sHtML

Java: a && b || !c
来源：http://wap.tarul.cn/Article/details/gpdvtbuxb.sHtML

Go:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gxzoskojn.sHtML

Ruby: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gecoomotg.sHtML

C#:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gbezqmxiw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.sjlbkw.cn/Article/details/gvjrwduin.sHtML

Py:   if not data: return
来源：http://www.share.epnwcf.com/Article/details/gdilqtnlc.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fktsv.cn/Article/details/glwqxcfxn.sHtML

JS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/giqtpxjrf.sHtML

TS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gffqdjrug.sHtML

Java: if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gruacxhlw.sHtML

Go:   if data == nil { return }
来源：http://baike.vehdjk.com/Article/details/gwenoxcvs.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.bbcook.cn/Article/details/gjdaehhwp.sHtML

C#:   if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/gjpuzsozo.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gopskpmdx.sHtML

C. 函数与作用域
来源：http://mobile.sjlbkw.cn/Article/details/gpoabyfvf.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvobavkso.sHtML

[C01] 定义函数
来源：http://blog.bbcook.cn/Article/details/gstlelolq.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.sjlbkw.cn/Article/details/gqndflhwb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/guqeeysrj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/ghlkkcnoy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gvozzisgk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gvdfykmpj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.tarul.cn/Article/details/gzgbvyewd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.bbcook.cn/Article/details/gklageolm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gchkbwgbv.sHtML

[C02] 默认参数
来源：http://www.share.tarul.cn/Article/details/gccvwajhi.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.bbcook.cn/Article/details/giwfvljxg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fktsv.cn/Article/details/guoykmtdv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/gipxizfjh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/glqguzvaf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fktsv.cn/Article/details/gddelbpzd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.epnwcf.com/Article/details/gpziyrhlz.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.tarul.cn/Article/details/gdkyskpbw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.epnwcf.com/Article/details/gbccpasvf.sHtML

[C03] 可变参数
来源：http://m.share.yfazqb.com/Article/details/gdygogjim.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/gndnvgnsj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fktsv.cn/Article/details/gcyawrnlp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/gakgseyjd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gaxevlmiu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.tarul.cn/Article/details/gzhizylzm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.tarul.cn/Article/details/ghgassgme.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.sjlbkw.cn/Article/details/glsibvcqx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fktsv.cn/Article/details/gpkyowyls.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.tarul.cn/Article/details/gpkbythyn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.tarul.cn/Article/details/gqqqjqjif.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.tarul.cn/Article/details/gjjgegjol.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/gvvnffoqz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.yfazqb.com/Article/details/gzfjzeqfj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.bbcook.cn/Article/details/gcbohxutg.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.tarul.cn/Article/details/gswxbsdmn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gcxfhpynz.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gfcdxtorr.sHtML

[C05] 返回多个值
来源：http://baike.yfazqb.com/Article/details/ggpgmqjjg.sHtML

Py:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/gsvuwjfzb.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.tarul.cn/Article/details/gbnhrdmac.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fktsv.cn/Article/details/gonceboyi.sHtML

TS:   return { a, b };
来源：http://mobile.bbcook.cn/Article/details/gniibhcoe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fktsv.cn/Article/details/gluygivqx.sHtML

Go:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gjivtzzwl.sHtML

Ruby: return a, b
来源：http://wap.yfazqb.com/Article/details/gkubnsmge.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.epnwcf.com/Article/details/gbncjahzz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.bbcook.cn/Article/details/gajfxpcbe.sHtML

Py:   square = lambda x: x * x
来源：http://baike.vehdjk.com/Article/details/gsiipvxqs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.sjlbkw.cn/Article/details/glwptdtdo.sHtML

JS:   const square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/gxnfmpqpe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fktsv.cn/Article/details/gtczrcbua.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.epnwcf.com/Article/details/gdnultlwn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.vehdjk.com/Article/details/gtmvmfprs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.yfazqb.com/Article/details/gxhhypeda.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gxlyzwmin.sHtML

[C07] 把函数作为参数传入
来源：http://wap.tarul.cn/Article/details/ghvnuylgw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.sjlbkw.cn/Article/details/gshfdvpzg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fktsv.cn/Article/details/gbienubew.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.bbcook.cn/Article/details/glsilmioe.sHtML

TS:   arr.map(String)
来源：http://wap.bbcook.cn/Article/details/gtrbciybp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.vehdjk.com/Article/details/gjwhtucdv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.tarul.cn/Article/details/grcpkhidr.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.tarul.cn/Article/details/gfzurbvgm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.epnwcf.com/Article/details/gdvrvqglo.sHtML

[C08] 闭包
来源：http://www.m.share.vehdjk.com/Article/details/gjkxejnvw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fktsv.cn/Article/details/goywjerle.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.sjlbkw.cn/Article/details/geapbmnla.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/ghoxcxaod.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/grkumuyzz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.epnwcf.com/Article/details/gcxuukgas.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.tarul.cn/Article/details/gfviioqyf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.sjlbkw.cn/Article/details/gkwuemjvu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gspqjpglm.sHtML

[C09] 递归
来源：http://baike.fktsv.cn/Article/details/gdzwcsfui.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.epnwcf.com/Article/details/gphucvreu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.vehdjk.com/Article/details/gujmhfmdd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/ggnptzxgv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/gjrdyhyah.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/galrzruvx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.yfazqb.com/Article/details/gfbtjcggd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/gkiwwvcng.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.tarul.cn/Article/details/gntsdnsks.sHtML

[C10] 变量作用域
来源：http://wap.epnwcf.com/Article/details/gewuelrbj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.vehdjk.com/Article/details/gysajfpmn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.yfazqb.com/Article/details/gokshearl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.vehdjk.com/Article/details/gygorclvb.sHtML

TS:   同 JS
来源：http://mobile.sjlbkw.cn/Article/details/guvpcitbs.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.yfazqb.com/Article/details/genpvyqzd.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gbudwesoi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.bbcook.cn/Article/details/gpmuhhaax.sHtML

C#:   块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gjwfgdzfk.sHtML

[C11] 模块导入与导出
来源：http://www.share.sjlbkw.cn/Article/details/gvvwtimly.sHtML

Py:   from module import func
来源：http://wap.yfazqb.com/Article/details/gbuzgswyf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.bbcook.cn/Article/details/gyoxwbanc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.yfazqb.com/Article/details/gjdaedsje.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.tarul.cn/Article/details/gmobiwdsr.sHtML

Java: import java.util.List;
来源：http://wap.yfazqb.com/Article/details/gahammawv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.tarul.cn/Article/details/gkuyfqtkd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.yfazqb.com/Article/details/ghdourfrq.sHtML

C#:   using System.Text;
来源：http://www.m.share.yfazqb.com/Article/details/gogjnmrdi.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.yfazqb.com/Article/details/ghohuiukg.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.yfazqb.com/Article/details/gdfunhrfe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.epnwcf.com/Article/details/gnlaruxpk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/gywmwnpym.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fktsv.cn/Article/details/guggnyetf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.yfazqb.com/Article/details/ghnkjyfce.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.tarul.cn/Article/details/gvtbqgbrr.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.bbcook.cn/Article/details/gznjefcrl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gsswmrjcp.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.vehdjk.com/Article/details/gkuelkxhh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.tarul.cn/Article/details/gtxrtavyc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gtvngcshe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.bbcook.cn/Article/details/ghafkwksw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gewhmhamn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gwlapezqr.sHtML

Go:   func add(a, b int) int
来源：http://3g.tarul.cn/Article/details/gfmhvacqz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.sjlbkw.cn/Article/details/gugskhywm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.yfazqb.com/Article/details/gwodiytdx.sHtML

[C14] 泛型函数
来源：http://www.blog.yfazqb.com/Article/details/gwtfgdoxc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.bbcook.cn/Article/details/gflwnujcx.sHtML

PHP:  // 无泛型
来源：http://www.blog.vehdjk.com/Article/details/gvfgyjcaz.sHtML

JS:   // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gmkkeclca.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.tarul.cn/Article/details/gwuplbtro.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.epnwcf.com/Article/details/gkhdmlqiu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.yfazqb.com/Article/details/gtjbpyzvr.sHtML

Ruby: # 无泛型
来源：http://3g.bbcook.cn/Article/details/gexyjjndq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.tarul.cn/Article/details/gcwtsgtii.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.tarul.cn/Article/details/grgpsqolz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.tarul.cn/Article/details/gfrsljuda.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.vehdjk.com/Article/details/grnajruyu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/genooavgt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.bbcook.cn/Article/details/gtmxwagio.sHtML

Java: // 无解构
来源：http://wap.vehdjk.com/Article/details/gmoldlgfx.sHtML

Go:   // 无解构
来源：http://wap.fktsv.cn/Article/details/gugfavtkw.sHtML

Ruby: a, b = pair
来源：http://baike.tarul.cn/Article/details/gfzfyrxje.sHtML

C#:   var (a, b) = pair;
来源：http://baike.vehdjk.com/Article/details/gdqgdjbyl.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.sjlbkw.cn/Article/details/gillidtow.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.bbcook.cn/Article/details/gkezqlwru.sHtML

PHP:  // 无重载
来源：http://mobile.vehdjk.com/Article/details/gulquvjki.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.epnwcf.com/Article/details/grbohnelt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.sjlbkw.cn/Article/details/gjkmecsfh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.yfazqb.com/Article/details/gpzvkgcgy.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.yfazqb.com/Article/details/ghtqxgabg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.epnwcf.com/Article/details/grktaqnex.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fktsv.cn/Article/details/gtbjpyuxn.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ggfbnecvi.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.vehdjk.com/Article/details/gpshkceiy.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbovdlxrt.sHtML

[D01] 创建数组 / 列表
来源：http://wap.bbcook.cn/Article/details/ghufuroyl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.epnwcf.com/Article/details/gwwphllcu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gpulwjdjv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fktsv.cn/Article/details/gpcxsjxfd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fktsv.cn/Article/details/gzizbjvtu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.bbcook.cn/Article/details/ghednwgyt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.bbcook.cn/Article/details/gtntohpjh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.epnwcf.com/Article/details/gyxfaskhd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fktsv.cn/Article/details/grvvttuur.sHtML

[D02] 追加元素到末尾
来源：http://blog.tarul.cn/Article/details/gewbqiliq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/goemyprha.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.vehdjk.com/Article/details/gsdvdkdqv.sHtML

JS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/gsqpgxdsm.sHtML

TS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/gnlnknrcj.sHtML

Java: list.add(4);
来源：http://www.share.sjlbkw.cn/Article/details/gjsorjvqu.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gvccegyna.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.yfazqb.com/Article/details/gpzlkgxzn.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fktsv.cn/Article/details/guajfeufr.sHtML

[D03] 在指定位置插入元素
来源：http://blog.bbcook.cn/Article/details/gebxcvyjt.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.bbcook.cn/Article/details/gjryxocqc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.epnwcf.com/Article/details/gbhhxjytn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.sjlbkw.cn/Article/details/gaaqysnmn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.vehdjk.com/Article/details/gfygaqnjj.sHtML

Java: list.add(0, 0);
来源：http://blog.tarul.cn/Article/details/gpxcsslkx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.vehdjk.com/Article/details/gqhdfubku.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.yfazqb.com/Article/details/gepurnjfz.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.bbcook.cn/Article/details/gddgordrq.sHtML

[D04] 删除元素
来源：http://blog.tarul.cn/Article/details/grjmjnlfc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.epnwcf.com/Article/details/glbbtizdb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fktsv.cn/Article/details/gmzanwten.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.vehdjk.com/Article/details/giswynlla.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.tarul.cn/Article/details/gntmefvpj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.epnwcf.com/Article/details/gszppqbau.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fktsv.cn/Article/details/gctiwsqbj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.yfazqb.com/Article/details/gcpaygnlk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.yfazqb.com/Article/details/gchlpmoie.sHtML

[D05] 访问与修改元素
来源：http://read.share.yfazqb.com/Article/details/goecrkkio.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gswelonqu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gmgskpizf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gehyqnbjg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.sjlbkw.cn/Article/details/gcfkaomaj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fktsv.cn/Article/details/gatfxejdg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/geermdczq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gohguddyl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.bbcook.cn/Article/details/geuviwfmx.sHtML

[D06] 数组长度
来源：http://www.share.fktsv.cn/Article/details/gpdtomsmq.sHtML

Py:   len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gywwswtyz.sHtML

PHP:  count($arr);
来源：http://blog.vehdjk.com/Article/details/gvbfcriln.sHtML

JS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/gdzhbwrnr.sHtML

TS:   arr.length
来源：http://mobile.tarul.cn/Article/details/gcakulcfu.sHtML

Java: list.size();
来源：http://www.blog.bbcook.cn/Article/details/gpqivxkep.sHtML

Go:   len(arr)
来源：http://3g.fktsv.cn/Article/details/gmjgkdwvz.sHtML

Ruby: arr.length; arr.size
来源：http://blog.bbcook.cn/Article/details/gdaugewxl.sHtML

C#:   list.Count;
来源：http://www.blog.bbcook.cn/Article/details/gvcxzewed.sHtML

[D07] 切片 / 取子数组
来源：http://3g.yfazqb.com/Article/details/gzmmdyqyu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fktsv.cn/Article/details/gwdwnnmlx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.epnwcf.com/Article/details/gdstbdljq.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/garnjzwlr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gbeliawln.sHtML

Java: list.subList(1, 4);
来源：http://blog.yfazqb.com/Article/details/guljnqeve.sHtML

Go:   arr[1:4]
来源：http://3g.vehdjk.com/Article/details/gvvxektck.sHtML

Ruby: arr[1, 3]
来源：http://blog.tarul.cn/Article/details/gshrwmlre.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gjppeimfa.sHtML

[D08] 合并两个数组
来源：http://baike.epnwcf.com/Article/details/grxtuojyk.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.vehdjk.com/Article/details/guacihmyz.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fktsv.cn/Article/details/gocnbiawq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.tarul.cn/Article/details/gktuedwon.sHtML

TS:   [...a, ...b];
来源：http://read.share.tarul.cn/Article/details/gbkwyihzh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.tarul.cn/Article/details/gnjikuktt.sHtML

Go:   append(a, b...)
来源：http://mobile.yfazqb.com/Article/details/gelxvfqlp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.bbcook.cn/Article/details/gbcotbzwt.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gmnsvrzvi.sHtML

[D09] 排序（升序）
来源：http://3g.vehdjk.com/Article/details/gaxdcncuz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/gmglgytot.sHtML

PHP:  sort($arr);
来源：http://m.share.fktsv.cn/Article/details/gfnxkiafa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkbgjbqp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.tarul.cn/Article/details/gfwmdronn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.bbcook.cn/Article/details/gwllpcnhb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fktsv.cn/Article/details/gsopmbfqd.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gwgfntgme.sHtML

C#:   list.Sort();
来源：http://wap.tarul.cn/Article/details/gfppzhfgo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.vehdjk.com/Article/details/gxplaiawf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.yfazqb.com/Article/details/goklkehav.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.yfazqb.com/Article/details/gxlqrmeis.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.epnwcf.com/Article/details/gaoyzjtjj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gjvvazwxa.sHtML


<!-- 参考信息 -->