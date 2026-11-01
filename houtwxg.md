代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gexhvdodx.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fktsv.cn/Article/details/ghohyrsfs.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.epnwcf.com/Article/details/gvbwykota.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.yfazqb.com/Article/details/geujkuque.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.sjlbkw.cn/Article/details/grwpdemzf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/gfatpugwu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fktsv.cn/Article/details/ggspslnyf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.sjlbkw.cn/Article/details/gbklahqbn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.bbcook.cn/Article/details/getutsjiw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.bbcook.cn/Article/details/gaechookb.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fktsv.cn/Article/details/gtbslqahm.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/gbaxtrexr.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.tarul.cn/Article/details/glprcjrct.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.bbcook.cn/Article/details/gkeivkhlc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.bbcook.cn/Article/details/gkyvgdbtj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.sjlbkw.cn/Article/details/guhucdflf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.vehdjk.com/Article/details/ggivdcehq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.tarul.cn/Article/details/gfopkmovd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.epnwcf.com/Article/details/gnpicobvw.sHtML

[B12] 跳出多层循环
来源：http://read.share.fktsv.cn/Article/details/gwswnrgsk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvclljqa.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.sjlbkw.cn/Article/details/gkzsorjlj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/govkthznm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/grvlkzmxm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gaqrchkcj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.tarul.cn/Article/details/gfyclzooz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.vehdjk.com/Article/details/ghrfwwgvi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.sjlbkw.cn/Article/details/gvglzykda.sHtML

[B13] 判断是否为数字
来源：http://m.share.fktsv.cn/Article/details/gwcnczqkg.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.bbcook.cn/Article/details/gqpfinedu.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.epnwcf.com/Article/details/gdzgslqot.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.vehdjk.com/Article/details/gpqfllyob.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.vehdjk.com/Article/details/gtgpfdkgp.sHtML

Java: x instanceof Number
来源：http://read.share.epnwcf.com/Article/details/gumzgzdlm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.tarul.cn/Article/details/gcyegatuj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.yfazqb.com/Article/details/gquekfcok.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fktsv.cn/Article/details/gmchlyyhr.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.tarul.cn/Article/details/gvdljcziz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.bbcook.cn/Article/details/gtlvhofmz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.tarul.cn/Article/details/gaykcvhrs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/gljkjdfik.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gdfzwyezo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gfylbhfnk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.vehdjk.com/Article/details/gtrtowgxv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/glhcdbxpo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gbvpxgoei.sHtML

[B15] 布尔运算与取反
来源：http://mobile.tarul.cn/Article/details/gwksdedzt.sHtML

Py:   a and b or not c
来源：http://www.blog.sjlbkw.cn/Article/details/gjvmffuja.sHtML

PHP:  $a && $b || !$c
来源：http://baike.bbcook.cn/Article/details/ghtjarozt.sHtML

JS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/ggxgnguaz.sHtML

TS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gztjtlniv.sHtML

Java: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gtnynzkdn.sHtML

Go:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gvmwivdmo.sHtML

Ruby: a && b || !c
来源：http://mobile.tarul.cn/Article/details/gigtdlgcj.sHtML

C#:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gwkowjvlw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.epnwcf.com/Article/details/guagrjvfj.sHtML

Py:   if not data: return
来源：http://www.share.bbcook.cn/Article/details/gasfrfjld.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.sjlbkw.cn/Article/details/gsjdtcbxq.sHtML

JS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/gfbtyzhgp.sHtML

TS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gpmilngga.sHtML

Java: if (data == null) return;
来源：http://3g.tarul.cn/Article/details/goawjgkby.sHtML

Go:   if data == nil { return }
来源：http://www.share.yfazqb.com/Article/details/gekmufmlr.sHtML

Ruby: return if data.nil?
来源：http://blog.bbcook.cn/Article/details/gvnmxgwha.sHtML

C#:   if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/gvsbrxjir.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gnrwseeyh.sHtML

C. 函数与作用域
来源：http://www.blog.fktsv.cn/Article/details/gefpynfjb.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/grnmsjwrr.sHtML

[C01] 定义函数
来源：http://blog.vehdjk.com/Article/details/ghsjyjpmq.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.tarul.cn/Article/details/gjzmjyrug.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/galrvfdae.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/galegybik.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gnygximjw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gydfetezp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.tarul.cn/Article/details/gqeqerftd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.sjlbkw.cn/Article/details/gulnvbvnx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gpxeeogsh.sHtML

[C02] 默认参数
来源：http://3g.bbcook.cn/Article/details/ggfgdjnxs.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.epnwcf.com/Article/details/gawegfasc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.epnwcf.com/Article/details/gsplropyc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghrvkgtna.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.yfazqb.com/Article/details/glmkvygdg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.epnwcf.com/Article/details/gjwctqwef.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.tarul.cn/Article/details/gswkikzbk.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.vehdjk.com/Article/details/gxmnitzle.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.vehdjk.com/Article/details/geuxmcoeb.sHtML

[C03] 可变参数
来源：http://3g.yfazqb.com/Article/details/ggpspuhfv.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.vehdjk.com/Article/details/gscfcihoo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.epnwcf.com/Article/details/gukslxxiu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/gcuxxbsxb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/grhxzhqtl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.vehdjk.com/Article/details/gcuhhyrex.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.yfazqb.com/Article/details/gdasbzmmb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fktsv.cn/Article/details/gjrwlyaew.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.sjlbkw.cn/Article/details/gnybswvll.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fktsv.cn/Article/details/gdorpncvk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fktsv.cn/Article/details/gslvcnptu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.yfazqb.com/Article/details/gqpqosepo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gkhkgmgpk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.bbcook.cn/Article/details/gytwwwitb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.yfazqb.com/Article/details/gqefunoil.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.epnwcf.com/Article/details/googuvigi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gfbqhwgsv.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gqwrojwwj.sHtML

[C05] 返回多个值
来源：http://baike.sjlbkw.cn/Article/details/gaheksndb.sHtML

Py:   return a, b
来源：http://www.share.tarul.cn/Article/details/gfhvxgzwc.sHtML

PHP:  return [$a, $b];
来源：http://3g.bbcook.cn/Article/details/gadkxhgce.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.epnwcf.com/Article/details/gsecupocw.sHtML

TS:   return { a, b };
来源：http://m.share.tarul.cn/Article/details/gljwtnvsc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.yfazqb.com/Article/details/glndtfbyn.sHtML

Go:   return a, b
来源：http://baike.sjlbkw.cn/Article/details/gppweyuud.sHtML

Ruby: return a, b
来源：http://www.blog.tarul.cn/Article/details/graactbty.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.tarul.cn/Article/details/gmdisrjyx.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.epnwcf.com/Article/details/gizzlfhrt.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fktsv.cn/Article/details/gbwdiupmm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fktsv.cn/Article/details/gmvesswoq.sHtML

JS:   const square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/ghpzwgwup.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.bbcook.cn/Article/details/ghxpjpgke.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.yfazqb.com/Article/details/gbxfiqbaj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.tarul.cn/Article/details/gifjppluk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.yfazqb.com/Article/details/giauzwkhn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/gfftaforu.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.epnwcf.com/Article/details/gnrvhdgds.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.epnwcf.com/Article/details/gmhuunghk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.vehdjk.com/Article/details/gslkvxipv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.sjlbkw.cn/Article/details/gykvwuuev.sHtML

TS:   arr.map(String)
来源：http://baike.yfazqb.com/Article/details/gloqkxixr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.tarul.cn/Article/details/gihopsfiu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.tarul.cn/Article/details/gknylvghc.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.bbcook.cn/Article/details/gpdpuoyoy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.vehdjk.com/Article/details/gifefaqbj.sHtML

[C08] 闭包
来源：http://3g.yfazqb.com/Article/details/gtxnsbvvk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.yfazqb.com/Article/details/ghozjinet.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.yfazqb.com/Article/details/gxlqvqppz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/ggpgsnoiq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/grklnfpym.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fktsv.cn/Article/details/gwkntrggd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.vehdjk.com/Article/details/glkzhewaf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.sjlbkw.cn/Article/details/gbhgrefsr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gtzsiydwv.sHtML

[C09] 递归
来源：http://www.share.bbcook.cn/Article/details/gdxxitzhx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gvdpeywfa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/grmcahlla.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.yfazqb.com/Article/details/gfvompbaz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/gzgemvujm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/gbzrsspjc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.tarul.cn/Article/details/ghjmwzqmt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gvcvchxdl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.vehdjk.com/Article/details/gpllxwmjo.sHtML

[C10] 变量作用域
来源：http://mobile.bbcook.cn/Article/details/ggpvzytls.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.sjlbkw.cn/Article/details/goefivgld.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fktsv.cn/Article/details/gdsdbjvsa.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gtjzxtlva.sHtML

TS:   同 JS
来源：http://3g.fktsv.cn/Article/details/gzrnaufsa.sHtML

Java: 方法内为块级作用域
来源：http://baike.yfazqb.com/Article/details/guobaseqv.sHtML

Go:   花括号块级作用域
来源：http://blog.bbcook.cn/Article/details/gnlueyypp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.yfazqb.com/Article/details/gsqxacexp.sHtML

C#:   块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/guhukgbvk.sHtML

[C11] 模块导入与导出
来源：http://baike.vehdjk.com/Article/details/gkoteaokc.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gdrnqkptr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.sjlbkw.cn/Article/details/gayasxuzq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.vehdjk.com/Article/details/gvtkyznts.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.epnwcf.com/Article/details/gaiildpua.sHtML

Java: import java.util.List;
来源：http://www.m.share.yfazqb.com/Article/details/giugwuumh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.tarul.cn/Article/details/ggafxxeej.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.yfazqb.com/Article/details/gvolzecqh.sHtML

C#:   using System.Text;
来源：http://mobile.tarul.cn/Article/details/gwuenwyyo.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.tarul.cn/Article/details/gztqwtbja.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.tarul.cn/Article/details/gpqazumly.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.yfazqb.com/Article/details/gjmavamya.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/ggtkchwui.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.epnwcf.com/Article/details/gxnoitfhk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.yfazqb.com/Article/details/gfbiglckd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.bbcook.cn/Article/details/goxmxwmme.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fktsv.cn/Article/details/gzgwjbkpv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/gxoimwuue.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fktsv.cn/Article/details/giiuyjhhr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fktsv.cn/Article/details/gnhylzque.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gwhmhgfuq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.sjlbkw.cn/Article/details/gbmubcgis.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/glpmivytb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gnehfobvp.sHtML

Go:   func add(a, b int) int
来源：http://baike.vehdjk.com/Article/details/gukibwxbo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.yfazqb.com/Article/details/gzfcthamm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.tarul.cn/Article/details/gmuqmtobu.sHtML

[C14] 泛型函数
来源：http://read.share.tarul.cn/Article/details/gllvlhbks.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.tarul.cn/Article/details/gxknihamf.sHtML

PHP:  // 无泛型
来源：http://3g.epnwcf.com/Article/details/glzqmshsg.sHtML

JS:   // 无泛型
来源：http://blog.fktsv.cn/Article/details/gusrigsfp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fktsv.cn/Article/details/gvldoorey.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fktsv.cn/Article/details/gjjrxismi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.vehdjk.com/Article/details/gpscawilp.sHtML

Ruby: # 无泛型
来源：http://www.share.epnwcf.com/Article/details/gcxfwngds.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.tarul.cn/Article/details/grqtsvhya.sHtML

[C15] 解构 / 展开参数
来源：http://3g.tarul.cn/Article/details/gglocfzzw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.vehdjk.com/Article/details/gidhvgnnt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.vehdjk.com/Article/details/gittcspgc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.vehdjk.com/Article/details/gasqzzphk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.vehdjk.com/Article/details/gfmyculhl.sHtML

Java: // 无解构
来源：http://blog.fktsv.cn/Article/details/gdvjdlals.sHtML

Go:   // 无解构
来源：http://blog.tarul.cn/Article/details/gmddaqmig.sHtML

Ruby: a, b = pair
来源：http://read.share.tarul.cn/Article/details/gupfukqkx.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fktsv.cn/Article/details/gkklwflhm.sHtML

[C16] 函数 / 方法重载
来源：http://baike.epnwcf.com/Article/details/gxanoexkq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.tarul.cn/Article/details/gmuvpvekn.sHtML

PHP:  // 无重载
来源：http://3g.yfazqb.com/Article/details/gakvbmzzw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.vehdjk.com/Article/details/gamlkhfgq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.epnwcf.com/Article/details/gwdnmgnxq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.vehdjk.com/Article/details/gvvabrzbh.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.vehdjk.com/Article/details/gssidjvzn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.bbcook.cn/Article/details/gqfpddmox.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.tarul.cn/Article/details/giaarmuky.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmajkresm.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.bbcook.cn/Article/details/gvsydobda.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gawrbjdbd.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fktsv.cn/Article/details/gcjwscnig.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.sjlbkw.cn/Article/details/gzjaognhw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.yfazqb.com/Article/details/gcuydrcnw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fktsv.cn/Article/details/gyofhxhue.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.yfazqb.com/Article/details/gedleibto.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.vehdjk.com/Article/details/gofoosgyk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.yfazqb.com/Article/details/ggjybrfif.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.bbcook.cn/Article/details/gbeqkajmz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.epnwcf.com/Article/details/gvwogcrpv.sHtML

[D02] 追加元素到末尾
来源：http://www.share.sjlbkw.cn/Article/details/gzmpwnrgt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.tarul.cn/Article/details/gxbvpjmtj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.bbcook.cn/Article/details/gspbaidkw.sHtML

JS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/gphjpgixd.sHtML

TS:   arr.push(4);
来源：http://blog.sjlbkw.cn/Article/details/gpnbqnjfg.sHtML

Java: list.add(4);
来源：http://wap.fktsv.cn/Article/details/gkbyqqtpd.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/glfpvmbtx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.epnwcf.com/Article/details/gfvnbwruk.sHtML

C#:   list.Add(4);
来源：http://www.m.share.yfazqb.com/Article/details/glxqigbfq.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fktsv.cn/Article/details/gunghkbpw.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/grixfkjhy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.yfazqb.com/Article/details/glszulbcc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fktsv.cn/Article/details/gorvtwzke.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gpbrzgzxe.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gpbpmnwgc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.sjlbkw.cn/Article/details/gaakukwdp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.tarul.cn/Article/details/gmpkehcta.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gyjpzxthe.sHtML

[D04] 删除元素
来源：http://www.blog.fktsv.cn/Article/details/gpdlhwvlw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.sjlbkw.cn/Article/details/glegrumwe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fktsv.cn/Article/details/gntgtinnf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.epnwcf.com/Article/details/gzororkgb.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.sjlbkw.cn/Article/details/gbvoaqivf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.vehdjk.com/Article/details/gibkhulxn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.epnwcf.com/Article/details/gupvzhnqe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.bbcook.cn/Article/details/gfvycxoul.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fktsv.cn/Article/details/gayvfbjgf.sHtML

[D05] 访问与修改元素
来源：http://blog.yfazqb.com/Article/details/gcokwfzce.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/gjstfefwl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/glxamctyu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gbajlttgu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fktsv.cn/Article/details/grwdmmjqv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.yfazqb.com/Article/details/gsbwuzbgk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gzftwhypz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gfbghkmjx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/gkveifhzd.sHtML

[D06] 数组长度
来源：http://blog.bbcook.cn/Article/details/gkzjwkotp.sHtML

Py:   len(arr)
来源：http://www.share.epnwcf.com/Article/details/gnaakcebk.sHtML

PHP:  count($arr);
来源：http://read.share.tarul.cn/Article/details/gsacvhghp.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gyybzeghv.sHtML

TS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/grcghjgph.sHtML

Java: list.size();
来源：http://m.share.tarul.cn/Article/details/gppxunohs.sHtML

Go:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gmnermgtq.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.yfazqb.com/Article/details/guypillkr.sHtML

C#:   list.Count;
来源：http://www.share.fktsv.cn/Article/details/ghfvdybqh.sHtML

[D07] 切片 / 取子数组
来源：http://wap.yfazqb.com/Article/details/gzukbyitr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.tarul.cn/Article/details/gkyrlaqcf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.vehdjk.com/Article/details/glghootey.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gwqqmfsin.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.tarul.cn/Article/details/gyxqouava.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/ghmmxgieo.sHtML

Go:   arr[1:4]
来源：http://www.m.share.sjlbkw.cn/Article/details/guihffkxj.sHtML

Ruby: arr[1, 3]
来源：http://m.share.yfazqb.com/Article/details/githnpola.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gasythwsi.sHtML

[D08] 合并两个数组
来源：http://wap.bbcook.cn/Article/details/grjlxszap.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.bbcook.cn/Article/details/gckjjmsyv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.tarul.cn/Article/details/gxgzimjzo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.tarul.cn/Article/details/gjecpnshg.sHtML

TS:   [...a, ...b];
来源：http://baike.sjlbkw.cn/Article/details/gjyclpzal.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.vehdjk.com/Article/details/glpkedquv.sHtML

Go:   append(a, b...)
来源：http://blog.epnwcf.com/Article/details/guwttdkgq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.yfazqb.com/Article/details/gniozoqvx.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gfoaqdgnx.sHtML

[D09] 排序（升序）
来源：http://www.blog.yfazqb.com/Article/details/glubvyzdn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gsyzvwhgb.sHtML

PHP:  sort($arr);
来源：http://blog.fktsv.cn/Article/details/gtyuxjpje.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.sjlbkw.cn/Article/details/gpuhimsjt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gmhasqbjd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.vehdjk.com/Article/details/gbroevvka.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gyanhirtt.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/gkgorgerw.sHtML

C#:   list.Sort();
来源：http://wap.yfazqb.com/Article/details/gnodaaxbp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.yfazqb.com/Article/details/gfktnawoo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.sjlbkw.cn/Article/details/gqmnhtpbx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gjiphpgkk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gegznvzzu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/goamikxhq.sHtML


<!-- 参考信息 -->