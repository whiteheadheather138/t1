代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.bbcook.cn/Article/details/gewlqrfxb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.yfazqb.com/Article/details/glyidymlu.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fktsv.cn/Article/details/gnihjfyjr.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fktsv.cn/Article/details/gfnsardxd.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fktsv.cn/Article/details/gksfdbpqv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.yfazqb.com/Article/details/gzpddadgv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gbpnzmviq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.epnwcf.com/Article/details/grpgxabfo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.yfazqb.com/Article/details/gzwwnbcgb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.epnwcf.com/Article/details/gtufafxhc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.tarul.cn/Article/details/gprexxbmu.sHtML

[B12] 跳出多层循环
来源：http://baike.sjlbkw.cn/Article/details/gzrmudztw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.bbcook.cn/Article/details/ghnhmhegi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fktsv.cn/Article/details/gioysoqcr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/gasyeybql.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gchsqicwa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gdwhijans.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.epnwcf.com/Article/details/gkiokmwhb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fktsv.cn/Article/details/gyhrfevhz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.bbcook.cn/Article/details/gkqttvjtg.sHtML

[B13] 判断是否为数字
来源：http://m.share.yfazqb.com/Article/details/gavfisoql.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.vehdjk.com/Article/details/goaxvycas.sHtML

PHP:  is_numeric($x)
来源：http://m.share.vehdjk.com/Article/details/ggymnyngv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/ggomiboeb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/gkejhpdpo.sHtML

Java: x instanceof Number
来源：http://mobile.yfazqb.com/Article/details/gzjugttac.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnocjnyo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.epnwcf.com/Article/details/gufifdjuo.sHtML

C#:   x is int or double or decimal
来源：http://baike.vehdjk.com/Article/details/gpixzrrye.sHtML

[B14] 判断值是否在集合内
来源：http://baike.tarul.cn/Article/details/grndrqptm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.sjlbkw.cn/Article/details/gscggwsge.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.vehdjk.com/Article/details/glzdairtv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.bbcook.cn/Article/details/gefdvxdzp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/gbwwqjxxq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.yfazqb.com/Article/details/ghhjyhgvp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.yfazqb.com/Article/details/gysgjudig.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.bbcook.cn/Article/details/gnahezvle.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fktsv.cn/Article/details/ggcvckbdz.sHtML

[B15] 布尔运算与取反
来源：http://read.share.bbcook.cn/Article/details/gsjoclqar.sHtML

Py:   a and b or not c
来源：http://baike.yfazqb.com/Article/details/gghcgnwux.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.vehdjk.com/Article/details/geavbrtvh.sHtML

JS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/geboafyjl.sHtML

TS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gircoaiki.sHtML

Java: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gxehzdjzj.sHtML

Go:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gcebflvmz.sHtML

Ruby: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/ghtxdeyzy.sHtML

C#:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gezwuecto.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.epnwcf.com/Article/details/gbcxtzkbg.sHtML

Py:   if not data: return
来源：http://mobile.epnwcf.com/Article/details/ghidoavas.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.yfazqb.com/Article/details/gvuabriim.sHtML

JS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/gixaucrpy.sHtML

TS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/girzafqkr.sHtML

Java: if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/gxjiikjyo.sHtML

Go:   if data == nil { return }
来源：http://read.share.bbcook.cn/Article/details/gjbvlgpuz.sHtML

Ruby: return if data.nil?
来源：http://read.share.bbcook.cn/Article/details/gwshrmylt.sHtML

C#:   if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/ghtvvreuj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gzrikdfdm.sHtML

C. 函数与作用域
来源：http://3g.yfazqb.com/Article/details/gsuaolwdt.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gcghqapoh.sHtML

[C01] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gfausoizd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjcmmbdd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/goqvlmksl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gmxofcxls.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gvjgsixao.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gaepxqloe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.tarul.cn/Article/details/gpitladpf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.yfazqb.com/Article/details/ghbdqidcf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gyzbhlpzm.sHtML

[C02] 默认参数
来源：http://www.share.yfazqb.com/Article/details/gwqjhuess.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.sjlbkw.cn/Article/details/gilsonwsq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.sjlbkw.cn/Article/details/gxghutatj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gwvdubphd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gnmvopxon.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.vehdjk.com/Article/details/gzuewlwoc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fktsv.cn/Article/details/grxmnckmt.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.sjlbkw.cn/Article/details/gpevlkemm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.vehdjk.com/Article/details/gauzoiywn.sHtML

[C03] 可变参数
来源：http://www.blog.sjlbkw.cn/Article/details/ggflzjawg.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.yfazqb.com/Article/details/ghxzargrt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.tarul.cn/Article/details/gaoisztdp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/gytfzpkca.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/gljotqmin.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.yfazqb.com/Article/details/grzxrkove.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.tarul.cn/Article/details/gplyhjxbw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fktsv.cn/Article/details/gdgvlakin.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.tarul.cn/Article/details/grveiyxje.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fktsv.cn/Article/details/gfnxpbyhj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fktsv.cn/Article/details/gznbtubac.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.sjlbkw.cn/Article/details/gcmgwqfrj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/giztulhiv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.yfazqb.com/Article/details/gvsambhda.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.yfazqb.com/Article/details/giskiyrvd.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fktsv.cn/Article/details/gjdhaktex.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gcxfeaiml.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/ghknewyde.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/gslbezoqb.sHtML

Py:   return a, b
来源：http://wap.yfazqb.com/Article/details/gvgaulfqd.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fktsv.cn/Article/details/gbqepuwrb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.bbcook.cn/Article/details/gxvicqldc.sHtML

TS:   return { a, b };
来源：http://blog.tarul.cn/Article/details/gpantnbwd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.vehdjk.com/Article/details/ghzdxwrvc.sHtML

Go:   return a, b
来源：http://www.blog.yfazqb.com/Article/details/gxxkkeivj.sHtML

Ruby: return a, b
来源：http://m.share.yfazqb.com/Article/details/grcdhwzat.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.tarul.cn/Article/details/gdrlqdydn.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.epnwcf.com/Article/details/gsifdpaze.sHtML

Py:   square = lambda x: x * x
来源：http://baike.epnwcf.com/Article/details/gzfgfpmam.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.tarul.cn/Article/details/gewsndlys.sHtML

JS:   const square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/gurijfqck.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.epnwcf.com/Article/details/gttydecuv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.tarul.cn/Article/details/glzjadvyg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.sjlbkw.cn/Article/details/gvkyfyqer.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.yfazqb.com/Article/details/goyhkdpmw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gonjdoqkv.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.tarul.cn/Article/details/gsvjtfpis.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fktsv.cn/Article/details/gcrmuhmnt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.vehdjk.com/Article/details/gorrkjtny.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.sjlbkw.cn/Article/details/gvrqzeffu.sHtML

TS:   arr.map(String)
来源：http://www.share.vehdjk.com/Article/details/gxkqpemcy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.tarul.cn/Article/details/gznmcfluh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fktsv.cn/Article/details/ggpajpkdw.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.epnwcf.com/Article/details/gwqoyepli.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.vehdjk.com/Article/details/gjxudamxs.sHtML

[C08] 闭包
来源：http://www.share.epnwcf.com/Article/details/gnaehtbre.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.sjlbkw.cn/Article/details/ghynoyjkg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkwhwsgo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gckypokss.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gdvoxttus.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.vehdjk.com/Article/details/gbzirqfvh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fktsv.cn/Article/details/gdcwlwels.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.epnwcf.com/Article/details/gzrhumwfn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.bbcook.cn/Article/details/ghdgxyevw.sHtML

[C09] 递归
来源：http://blog.epnwcf.com/Article/details/gfzdfibtw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gsagixcka.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.bbcook.cn/Article/details/grahabzkv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gapygbtux.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/gdnkefgof.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.sjlbkw.cn/Article/details/gqqpcpmxi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.epnwcf.com/Article/details/gooikutlp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gdidtjwve.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.yfazqb.com/Article/details/gefgvhgsr.sHtML

[C10] 变量作用域
来源：http://www.share.fktsv.cn/Article/details/gfmlxsabv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.vehdjk.com/Article/details/gctorbjqr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.vehdjk.com/Article/details/gmbujnpye.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fktsv.cn/Article/details/gxsgowuzt.sHtML

TS:   同 JS
来源：http://www.m.share.tarul.cn/Article/details/gzkeagzsr.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fktsv.cn/Article/details/gyeqfldjx.sHtML

Go:   花括号块级作用域
来源：http://wap.fktsv.cn/Article/details/guaruxxsw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.bbcook.cn/Article/details/glkqyyutp.sHtML

C#:   块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/ghzohclpz.sHtML

[C11] 模块导入与导出
来源：http://3g.bbcook.cn/Article/details/gnxtnaqsw.sHtML

Py:   from module import func
来源：http://wap.tarul.cn/Article/details/ghmburtiy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.epnwcf.com/Article/details/gfhtjfctr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.yfazqb.com/Article/details/gheyytomq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.sjlbkw.cn/Article/details/gzzvgvmww.sHtML

Java: import java.util.List;
来源：http://mobile.sjlbkw.cn/Article/details/gwjcwrilf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.sjlbkw.cn/Article/details/gkbgkwvyv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.bbcook.cn/Article/details/gqtaugfck.sHtML

C#:   using System.Text;
来源：http://www.m.share.vehdjk.com/Article/details/gglnuatoa.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fktsv.cn/Article/details/gduywbtmv.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.vehdjk.com/Article/details/gzvtczbuv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.bbcook.cn/Article/details/gjchtsjqi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.epnwcf.com/Article/details/gpcvrtlau.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/gxgzrakgt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.yfazqb.com/Article/details/gqbtznljo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.bbcook.cn/Article/details/gwjiqljzv.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.vehdjk.com/Article/details/guboiiekn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.epnwcf.com/Article/details/gydrqdgpk.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.yfazqb.com/Article/details/gnlmiylhi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fktsv.cn/Article/details/ghcmvbxfd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gsdcirumc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.bbcook.cn/Article/details/gxodhefhb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/glbwunklm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gtnhoeemr.sHtML

Go:   func add(a, b int) int
来源：http://www.share.epnwcf.com/Article/details/gbckzswri.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.epnwcf.com/Article/details/gdyrwbbnv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.epnwcf.com/Article/details/govzrircz.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/gfjtwzsqe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.sjlbkw.cn/Article/details/gzhpdnnfr.sHtML

PHP:  // 无泛型
来源：http://read.share.fktsv.cn/Article/details/gmawrlefo.sHtML

JS:   // 无泛型
来源：http://m.share.yfazqb.com/Article/details/gzcleenjs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.sjlbkw.cn/Article/details/gydktuiyl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.bbcook.cn/Article/details/gkbfbbdqg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fktsv.cn/Article/details/glweatzng.sHtML

Ruby: # 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gsoeeohnh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.yfazqb.com/Article/details/gwezhggri.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.bbcook.cn/Article/details/godkhmpjs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.yfazqb.com/Article/details/gsybvavdd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.vehdjk.com/Article/details/gwidwhcqi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/gngndusqv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.bbcook.cn/Article/details/gkliedyvy.sHtML

Java: // 无解构
来源：http://wap.fktsv.cn/Article/details/gewyyiwwr.sHtML

Go:   // 无解构
来源：http://wap.bbcook.cn/Article/details/gbavaoqoy.sHtML

Ruby: a, b = pair
来源：http://3g.bbcook.cn/Article/details/gqfdmncmv.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/ggsywwueg.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.yfazqb.com/Article/details/gwtiygwxw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.bbcook.cn/Article/details/gomcardil.sHtML

PHP:  // 无重载
来源：http://3g.fktsv.cn/Article/details/gmfhmdxbx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.vehdjk.com/Article/details/gzjbsqllr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.epnwcf.com/Article/details/gfzjqpxpb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fktsv.cn/Article/details/gfvhebkba.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.sjlbkw.cn/Article/details/gxqrcaryj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.vehdjk.com/Article/details/ghgoqtckk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.bbcook.cn/Article/details/gmcqitejs.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gojtwrqvj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.bbcook.cn/Article/details/gedijafoq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkysxznkx.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.yfazqb.com/Article/details/gbnllyipx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fktsv.cn/Article/details/gdlxfcvqd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.epnwcf.com/Article/details/gvjqzqwsi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.epnwcf.com/Article/details/gxkjwjnzf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.vehdjk.com/Article/details/gfamwkkoa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fktsv.cn/Article/details/gazqfeled.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.vehdjk.com/Article/details/ghzwnmybs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.vehdjk.com/Article/details/gotwlfdec.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fktsv.cn/Article/details/gobswlytk.sHtML

[D02] 追加元素到末尾
来源：http://baike.vehdjk.com/Article/details/gdxbwluzh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.epnwcf.com/Article/details/gpriacbvv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.epnwcf.com/Article/details/gmqmieptc.sHtML

JS:   arr.push(4);
来源：http://3g.vehdjk.com/Article/details/ggcmunkmr.sHtML

TS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/gasogjtuq.sHtML

Java: list.add(4);
来源：http://baike.yfazqb.com/Article/details/gzvgfdrhm.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.vehdjk.com/Article/details/gklayvopm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.epnwcf.com/Article/details/ggwfldpyh.sHtML

C#:   list.Add(4);
来源：http://m.share.bbcook.cn/Article/details/gsofsbzij.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.bbcook.cn/Article/details/guijrtpek.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fktsv.cn/Article/details/giakoqshl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.bbcook.cn/Article/details/gecvbucnb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.tarul.cn/Article/details/gkeornapn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.bbcook.cn/Article/details/grcgpfbli.sHtML

Java: list.add(0, 0);
来源：http://read.share.vehdjk.com/Article/details/gpugexsnp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fktsv.cn/Article/details/gllwtfikt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fktsv.cn/Article/details/guudllamg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/guthntxpn.sHtML

[D04] 删除元素
来源：http://www.blog.tarul.cn/Article/details/gjfizkygf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.tarul.cn/Article/details/geriwrayv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.vehdjk.com/Article/details/gngjxnzkg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.yfazqb.com/Article/details/gcyuupdxh.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.bbcook.cn/Article/details/gxjalablf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.bbcook.cn/Article/details/gcdinqhgc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fktsv.cn/Article/details/gsjkewjrh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.yfazqb.com/Article/details/gzjatqrzc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.vehdjk.com/Article/details/gcukdwqql.sHtML

[D05] 访问与修改元素
来源：http://wap.tarul.cn/Article/details/galitkdkh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gjyfxjchz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gfjsebqze.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/gsjersczh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.sjlbkw.cn/Article/details/gcxfuenxl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.sjlbkw.cn/Article/details/ggiqriebi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/ggnywdtfe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gajqsyrid.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fktsv.cn/Article/details/gwqyikmoz.sHtML

[D06] 数组长度
来源：http://baike.epnwcf.com/Article/details/grrjpjxlc.sHtML

Py:   len(arr)
来源：http://read.share.vehdjk.com/Article/details/gqueslbue.sHtML

PHP:  count($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gdrkibwmv.sHtML

JS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gvlombfdx.sHtML

TS:   arr.length
来源：http://wap.epnwcf.com/Article/details/givxwbxvx.sHtML

Java: list.size();
来源：http://read.share.bbcook.cn/Article/details/gmwoszekr.sHtML

Go:   len(arr)
来源：http://3g.tarul.cn/Article/details/gbzjwtkoi.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gwvodugeb.sHtML

C#:   list.Count;
来源：http://mobile.bbcook.cn/Article/details/gbxoqsnyg.sHtML

[D07] 切片 / 取子数组
来源：http://3g.tarul.cn/Article/details/ggsfxqrka.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.yfazqb.com/Article/details/glvbrlopf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fktsv.cn/Article/details/gddpxsjks.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gpaweproi.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gmqoxqgdj.sHtML

Java: list.subList(1, 4);
来源：http://baike.fktsv.cn/Article/details/ggkmlbdgv.sHtML

Go:   arr[1:4]
来源：http://blog.epnwcf.com/Article/details/gtazqwzqn.sHtML

Ruby: arr[1, 3]
来源：http://3g.bbcook.cn/Article/details/giwfbrsds.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fktsv.cn/Article/details/gsegxmoxw.sHtML

[D08] 合并两个数组
来源：http://wap.bbcook.cn/Article/details/gtzevtuwb.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fktsv.cn/Article/details/gulpdakcy.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.bbcook.cn/Article/details/grxlporuc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.sjlbkw.cn/Article/details/gptgujslw.sHtML

TS:   [...a, ...b];
来源：http://m.share.fktsv.cn/Article/details/gjbnbezoz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.vehdjk.com/Article/details/gaftvqdwh.sHtML

Go:   append(a, b...)
来源：http://www.m.share.yfazqb.com/Article/details/gldckzsdv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.sjlbkw.cn/Article/details/gckuuplue.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/glbqbncqj.sHtML

[D09] 排序（升序）
来源：http://m.share.vehdjk.com/Article/details/grvmktgez.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/gkuquarde.sHtML

PHP:  sort($arr);
来源：http://www.m.share.vehdjk.com/Article/details/glegktiju.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.yfazqb.com/Article/details/gdzfbswdo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.tarul.cn/Article/details/ghbinffuq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.yfazqb.com/Article/details/gwrrzgqyr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gvjkhiaks.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gqkswlspm.sHtML

C#:   list.Sort();
来源：http://m.share.tarul.cn/Article/details/gsiszqvjj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.tarul.cn/Article/details/gursqrxyp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.tarul.cn/Article/details/gnbtscvdv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.tarul.cn/Article/details/gzufzpdks.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/gjjwtiqsi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/ggkzjwpok.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.epnwcf.com/Article/details/gsfmwzdrp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.vehdjk.com/Article/details/geghegwfl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.vehdjk.com/Article/details/gnughppqz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fktsv.cn/Article/details/gnjlyjmkb.sHtML

[D11] 反转数组
来源：http://www.blog.vehdjk.com/Article/details/gujqrbmpb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.vehdjk.com/Article/details/gxaceobae.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.bbcook.cn/Article/details/gfpieopif.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.vehdjk.com/Article/details/grctiqgij.sHtML


<!-- 参考信息 -->