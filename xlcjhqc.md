代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gddxzcuiy.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fktsv.cn/Article/details/gltusnnqr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.tarul.cn/Article/details/gmktezjba.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fktsv.cn/Article/details/gvapidklm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/goinlzdmc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/ggbsprxmp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.yfazqb.com/Article/details/gujjuypiv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.sjlbkw.cn/Article/details/gqynotzug.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.yfazqb.com/Article/details/gcijkorch.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.tarul.cn/Article/details/gpmocnimy.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.yfazqb.com/Article/details/glmvsdlly.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.tarul.cn/Article/details/gyozsxvgy.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fktsv.cn/Article/details/gsrrlwsjp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fktsv.cn/Article/details/gqfwryvxd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.epnwcf.com/Article/details/grliumdaa.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.tarul.cn/Article/details/geusfrlkj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.bbcook.cn/Article/details/glfpgxuxy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.yfazqb.com/Article/details/ggkglnpun.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.tarul.cn/Article/details/gukkxdnar.sHtML

[B12] 跳出多层循环
来源：http://www.share.yfazqb.com/Article/details/gwmkpkawy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.epnwcf.com/Article/details/gxiyuziyz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.bbcook.cn/Article/details/gixvccypo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gbyayqday.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gfvbmdlpl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gphdpklqp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.yfazqb.com/Article/details/gsvdonjpb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvnmntrk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.bbcook.cn/Article/details/gdoruhgvz.sHtML

[B13] 判断是否为数字
来源：http://baike.sjlbkw.cn/Article/details/gwslzusfw.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.yfazqb.com/Article/details/ghocgvcgc.sHtML

PHP:  is_numeric($x)
来源：http://baike.epnwcf.com/Article/details/gjzegqfdr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gsfizlrwb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.vehdjk.com/Article/details/guglmvcxc.sHtML

Java: x instanceof Number
来源：http://3g.epnwcf.com/Article/details/gkwmejgdy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.tarul.cn/Article/details/gilqtlzkb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.vehdjk.com/Article/details/goahxdftb.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fktsv.cn/Article/details/gckidrlbv.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.bbcook.cn/Article/details/gqljzmmlg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.sjlbkw.cn/Article/details/gafrpthrh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.tarul.cn/Article/details/gzpshasjk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/giyetgeth.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gvkqmjpfw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.yfazqb.com/Article/details/gzgvyusvz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.epnwcf.com/Article/details/gfacpbtox.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.tarul.cn/Article/details/gknzbrctv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fktsv.cn/Article/details/grjmdklkq.sHtML

[B15] 布尔运算与取反
来源：http://mobile.epnwcf.com/Article/details/geudqsnqd.sHtML

Py:   a and b or not c
来源：http://read.share.sjlbkw.cn/Article/details/grsrbtora.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.tarul.cn/Article/details/ghqqhtilt.sHtML

JS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gictrwynt.sHtML

TS:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gfpiqlpou.sHtML

Java: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/glctywxko.sHtML

Go:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gukctzgqi.sHtML

Ruby: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gsgmyccio.sHtML

C#:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gerlogbzj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.bbcook.cn/Article/details/govbukzro.sHtML

Py:   if not data: return
来源：http://www.blog.yfazqb.com/Article/details/gmhcqqpay.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.sjlbkw.cn/Article/details/gsnigazwz.sHtML

JS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gxkjpvwfu.sHtML

TS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gothmslkv.sHtML

Java: if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/gefrzaprs.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.bbcook.cn/Article/details/grkaxfjzc.sHtML

Ruby: return if data.nil?
来源：http://read.share.bbcook.cn/Article/details/gfrwdrhov.sHtML

C#:   if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/gkjqicyhq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdccsoxdt.sHtML

C. 函数与作用域
来源：http://read.share.yfazqb.com/Article/details/gfdmoqjar.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtzkidsfb.sHtML

[C01] 定义函数
来源：http://baike.yfazqb.com/Article/details/gkibgtjfj.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.sjlbkw.cn/Article/details/gdrziypld.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/ghnvgzvoe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gkfyivoiy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gkzvrkohm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gyktanikg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.yfazqb.com/Article/details/gzgvmxqju.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkyfuydp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gcifvtvbv.sHtML

[C02] 默认参数
来源：http://read.share.fktsv.cn/Article/details/gmcearait.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fktsv.cn/Article/details/gsgkmpmqg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.tarul.cn/Article/details/gqhixqhjl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.sjlbkw.cn/Article/details/grasusiyv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.tarul.cn/Article/details/gvsijbbjh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.tarul.cn/Article/details/gxdemywsy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.bbcook.cn/Article/details/gccndccrv.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.vehdjk.com/Article/details/gtbsauwhs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.yfazqb.com/Article/details/gealivhhh.sHtML

[C03] 可变参数
来源：http://mobile.yfazqb.com/Article/details/ggtneexig.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.tarul.cn/Article/details/gtglogbjh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.sjlbkw.cn/Article/details/gmaxpoufd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.yfazqb.com/Article/details/gjwcarhro.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gfyoehegl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.bbcook.cn/Article/details/gykxisymw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.tarul.cn/Article/details/gfpdlfemr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fktsv.cn/Article/details/gqxkatmbf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.epnwcf.com/Article/details/gmtooduml.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.sjlbkw.cn/Article/details/grnykwhwm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fktsv.cn/Article/details/glrmnxqww.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.vehdjk.com/Article/details/gabokswck.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/glgzipqgt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.epnwcf.com/Article/details/gyhzqjlpa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.vehdjk.com/Article/details/gjebycudo.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.bbcook.cn/Article/details/gkveixeyy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gugglflyf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gvxunelol.sHtML

[C05] 返回多个值
来源：http://wap.tarul.cn/Article/details/gziwrdvxh.sHtML

Py:   return a, b
来源：http://mobile.bbcook.cn/Article/details/gqjnesznk.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fktsv.cn/Article/details/gywsfpnhr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gujdzhsba.sHtML

TS:   return { a, b };
来源：http://blog.vehdjk.com/Article/details/gyzufihph.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.tarul.cn/Article/details/ggpoxajpk.sHtML

Go:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gkhwkwcmj.sHtML

Ruby: return a, b
来源：http://www.m.share.fktsv.cn/Article/details/ggpldusrr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.tarul.cn/Article/details/gkbnrtvas.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.bbcook.cn/Article/details/gvotnnkpj.sHtML

Py:   square = lambda x: x * x
来源：http://3g.sjlbkw.cn/Article/details/gvrslkwmp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fktsv.cn/Article/details/giommabmr.sHtML

JS:   const square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gyitadvve.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.vehdjk.com/Article/details/gunbrddmb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.epnwcf.com/Article/details/gimwrrchn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.bbcook.cn/Article/details/gfpysmjmh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.yfazqb.com/Article/details/gvyryryoi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.tarul.cn/Article/details/gipapdbvq.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.yfazqb.com/Article/details/geumyxsvv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.vehdjk.com/Article/details/gczrknwsn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.bbcook.cn/Article/details/gaazuadot.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.bbcook.cn/Article/details/gbqwnavdm.sHtML

TS:   arr.map(String)
来源：http://baike.tarul.cn/Article/details/grqgrbwac.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.bbcook.cn/Article/details/guoqpqtdt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fktsv.cn/Article/details/gcwclnloe.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.epnwcf.com/Article/details/gbzbjarux.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fktsv.cn/Article/details/gsenvzkca.sHtML

[C08] 闭包
来源：http://baike.bbcook.cn/Article/details/ggoenmqru.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.yfazqb.com/Article/details/goxbeoufl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.epnwcf.com/Article/details/glytrarer.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gffgnypbl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gqqpvbmuc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.yfazqb.com/Article/details/gyduimzyo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.sjlbkw.cn/Article/details/gccjmkwbf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.tarul.cn/Article/details/gnumwnlfl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/guhtgoxeo.sHtML

[C09] 递归
来源：http://baike.yfazqb.com/Article/details/geecqlzkb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/grpghbimn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.tarul.cn/Article/details/gebfyqojx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gmqzumiyy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.sjlbkw.cn/Article/details/gqvkokyez.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.epnwcf.com/Article/details/gwwjhomfd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fktsv.cn/Article/details/gcixsyefp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/gixjdhhsr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fktsv.cn/Article/details/glsjcdruq.sHtML

[C10] 变量作用域
来源：http://3g.sjlbkw.cn/Article/details/gxismngjy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.vehdjk.com/Article/details/gtnrkdryx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.yfazqb.com/Article/details/gdsaimmko.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.sjlbkw.cn/Article/details/gyvayyxbt.sHtML

TS:   同 JS
来源：http://mobile.vehdjk.com/Article/details/gkturjcmb.sHtML

Java: 方法内为块级作用域
来源：http://wap.tarul.cn/Article/details/gahnufxiu.sHtML

Go:   花括号块级作用域
来源：http://3g.vehdjk.com/Article/details/glrxrfyuc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.tarul.cn/Article/details/gethedeta.sHtML

C#:   块级作用域
来源：http://baike.fktsv.cn/Article/details/gebvlrpvk.sHtML

[C11] 模块导入与导出
来源：http://mobile.sjlbkw.cn/Article/details/grszsvzmp.sHtML

Py:   from module import func
来源：http://wap.fktsv.cn/Article/details/gbqigspzb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.yfazqb.com/Article/details/gdmoppxgj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.yfazqb.com/Article/details/grtcckblv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.epnwcf.com/Article/details/gufrjmkjd.sHtML

Java: import java.util.List;
来源：http://wap.epnwcf.com/Article/details/geqkznbow.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.yfazqb.com/Article/details/gspbuueom.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.epnwcf.com/Article/details/gjasneujs.sHtML

C#:   using System.Text;
来源：http://www.share.sjlbkw.cn/Article/details/gjrmbasdv.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fktsv.cn/Article/details/gczswznxm.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fktsv.cn/Article/details/getdkvhwc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.tarul.cn/Article/details/gwptzrtlw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gizllxngm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/gcjaadwvz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.yfazqb.com/Article/details/gdpncwapa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.vehdjk.com/Article/details/gaxgooeof.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.epnwcf.com/Article/details/gbzuhvbwa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gwemwefea.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.tarul.cn/Article/details/gvrixbmer.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.sjlbkw.cn/Article/details/gidnnnddv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/glalebmbi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.vehdjk.com/Article/details/ggcmosaht.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdsasnmna.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/ghujckhok.sHtML

Go:   func add(a, b int) int
来源：http://wap.vehdjk.com/Article/details/gctxsiifw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.vehdjk.com/Article/details/gwuljwnkn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fktsv.cn/Article/details/gfkfiojvr.sHtML

[C14] 泛型函数
来源：http://wap.vehdjk.com/Article/details/gzrguoypy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.tarul.cn/Article/details/guwwizdfb.sHtML

PHP:  // 无泛型
来源：http://m.share.epnwcf.com/Article/details/gxgqmgrqw.sHtML

JS:   // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gielxdkob.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/garfgaggu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvajvgrfz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.bbcook.cn/Article/details/gosjljula.sHtML

Ruby: # 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/ghzimwtaj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.sjlbkw.cn/Article/details/gahcjyzvd.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.tarul.cn/Article/details/gdgedpbmo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.yfazqb.com/Article/details/gbwrravqd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.bbcook.cn/Article/details/gqrcalgno.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gsgnszgwv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.vehdjk.com/Article/details/gehqvxfkr.sHtML

Java: // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/gkqquebvo.sHtML

Go:   // 无解构
来源：http://mobile.fktsv.cn/Article/details/gyjqxriwm.sHtML

Ruby: a, b = pair
来源：http://mobile.bbcook.cn/Article/details/gzhkwhnxz.sHtML

C#:   var (a, b) = pair;
来源：http://wap.tarul.cn/Article/details/gwnuftucs.sHtML

[C16] 函数 / 方法重载
来源：http://blog.tarul.cn/Article/details/guebhiuuw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.tarul.cn/Article/details/gabbdqnif.sHtML

PHP:  // 无重载
来源：http://www.blog.yfazqb.com/Article/details/gkfnketst.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.sjlbkw.cn/Article/details/gmvkbaicl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.bbcook.cn/Article/details/gnwzodqov.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.vehdjk.com/Article/details/gnaywkwgp.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.sjlbkw.cn/Article/details/gautawjmd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fktsv.cn/Article/details/gvwgoxrra.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.sjlbkw.cn/Article/details/gzfaugdbv.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gkngnraly.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.yfazqb.com/Article/details/gnhbkdeik.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gmmvtcurq.sHtML

[D01] 创建数组 / 列表
来源：http://blog.yfazqb.com/Article/details/grwmdcofx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.vehdjk.com/Article/details/gxsvoxxwv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.epnwcf.com/Article/details/gmtdsrajo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.yfazqb.com/Article/details/ggmohqkqy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.yfazqb.com/Article/details/gbflcwmso.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.sjlbkw.cn/Article/details/grpenikxw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.epnwcf.com/Article/details/gufwpyhrj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.epnwcf.com/Article/details/ghosyysty.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.bbcook.cn/Article/details/ghbamszao.sHtML

[D02] 追加元素到末尾
来源：http://3g.sjlbkw.cn/Article/details/grusiehuh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fktsv.cn/Article/details/gfuibndmu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fktsv.cn/Article/details/gmdpdixzs.sHtML

JS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/gdcgdfghz.sHtML

TS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/gousljyjg.sHtML

Java: list.add(4);
来源：http://wap.vehdjk.com/Article/details/gppqynznl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fktsv.cn/Article/details/glaicovsb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.epnwcf.com/Article/details/gdwkndgdg.sHtML

C#:   list.Add(4);
来源：http://3g.tarul.cn/Article/details/grgeqhaxl.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.epnwcf.com/Article/details/ggelayfgl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gcqwihveh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.bbcook.cn/Article/details/ggcxxttdz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.epnwcf.com/Article/details/gaokolgtd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.epnwcf.com/Article/details/gukfkoaqx.sHtML

Java: list.add(0, 0);
来源：http://baike.fktsv.cn/Article/details/gdmkqqjus.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.tarul.cn/Article/details/gjertplva.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.yfazqb.com/Article/details/gwlcnvttv.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.tarul.cn/Article/details/gefwphscz.sHtML

[D04] 删除元素
来源：http://wap.vehdjk.com/Article/details/gcqdsepuk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.sjlbkw.cn/Article/details/ggytlhavl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.yfazqb.com/Article/details/gwczlkswx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.vehdjk.com/Article/details/gbdryqexr.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.vehdjk.com/Article/details/gigstmewz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.yfazqb.com/Article/details/gvmjkdmrh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fktsv.cn/Article/details/gporjeedz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.epnwcf.com/Article/details/gnpctdgiz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.tarul.cn/Article/details/gklihhskc.sHtML

[D05] 访问与修改元素
来源：http://www.share.fktsv.cn/Article/details/gwdyyrrup.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gqcwmfypx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gbxtvoaqh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gyomtiafk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.yfazqb.com/Article/details/glfzgyuzq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.bbcook.cn/Article/details/gidjomqbc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/gduqerpvz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/geiancmba.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fktsv.cn/Article/details/giakrjoes.sHtML

[D06] 数组长度
来源：http://read.share.epnwcf.com/Article/details/gsmgetbmi.sHtML

Py:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/glspshdhg.sHtML

PHP:  count($arr);
来源：http://www.share.vehdjk.com/Article/details/gzsxgqsll.sHtML

JS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/gyfuwicdn.sHtML

TS:   arr.length
来源：http://read.share.bbcook.cn/Article/details/ggavklsno.sHtML

Java: list.size();
来源：http://3g.epnwcf.com/Article/details/gfhcekrsr.sHtML

Go:   len(arr)
来源：http://baike.epnwcf.com/Article/details/ghwairsdh.sHtML

Ruby: arr.length; arr.size
来源：http://3g.sjlbkw.cn/Article/details/gbgbkqnvu.sHtML

C#:   list.Count;
来源：http://blog.sjlbkw.cn/Article/details/gqufqsynb.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.yfazqb.com/Article/details/gpfarnkhx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.tarul.cn/Article/details/gmyzaurqq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.epnwcf.com/Article/details/gmacshhha.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gqxdcjhul.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/gyljykfdh.sHtML

Java: list.subList(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gxtxeajoy.sHtML

Go:   arr[1:4]
来源：http://wap.sjlbkw.cn/Article/details/grffkzqtj.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gcuytsuxp.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.sjlbkw.cn/Article/details/guzxgpqkl.sHtML

[D08] 合并两个数组
来源：http://www.share.tarul.cn/Article/details/gjnyyeuzs.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.epnwcf.com/Article/details/gkegskrsu.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.tarul.cn/Article/details/gwrjcaxqc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.tarul.cn/Article/details/gydmhpmaz.sHtML

TS:   [...a, ...b];
来源：http://read.share.tarul.cn/Article/details/gqyjdptxn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.yfazqb.com/Article/details/glemovxbc.sHtML

Go:   append(a, b...)
来源：http://m.share.bbcook.cn/Article/details/gvppqsvax.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.tarul.cn/Article/details/gqgjxkuyn.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.tarul.cn/Article/details/glvkzwsep.sHtML

[D09] 排序（升序）
来源：http://3g.bbcook.cn/Article/details/gadjsgyuz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/gpbfpcsmm.sHtML

PHP:  sort($arr);
来源：http://blog.epnwcf.com/Article/details/gjedlluuc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.vehdjk.com/Article/details/grfolcnfd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.sjlbkw.cn/Article/details/gdjxdrphw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.sjlbkw.cn/Article/details/gmtajqybz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/gdrwzwqad.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gawuvjbey.sHtML

C#:   list.Sort();
来源：http://m.share.vehdjk.com/Article/details/gpaonmksm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.bbcook.cn/Article/details/gyjjjxdgb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.yfazqb.com/Article/details/gysfxebmo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fktsv.cn/Article/details/gylrwbkfp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gicokimey.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/gawtznemk.sHtML


<!-- 参考信息 -->