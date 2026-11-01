代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.blog.epnwcf.com/Article/details/gfloktfmx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.yfazqb.com/Article/details/gacdbbhia.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fktsv.cn/Article/details/gxuqyfhrg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fktsv.cn/Article/details/gzgaxktkt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.bbcook.cn/Article/details/gmfmcwzpf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fktsv.cn/Article/details/gzqcffdmp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.epnwcf.com/Article/details/giwmnvnaz.sHtML

[B12] 跳出多层循环
来源：http://mobile.yfazqb.com/Article/details/gttgcvjxz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.sjlbkw.cn/Article/details/gngplvvxb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.sjlbkw.cn/Article/details/gsusfgprf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/ggcdavezy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gabbdnddj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/gbscytwao.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.vehdjk.com/Article/details/gbigupjwu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.yfazqb.com/Article/details/ghjczxwyv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.tarul.cn/Article/details/gjyirmpcq.sHtML

[B13] 判断是否为数字
来源：http://blog.yfazqb.com/Article/details/gaiatxgkr.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.tarul.cn/Article/details/gldloqgpd.sHtML

PHP:  is_numeric($x)
来源：http://3g.bbcook.cn/Article/details/gdbghwncf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.tarul.cn/Article/details/gouuwaiwx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.yfazqb.com/Article/details/guotksnmm.sHtML

Java: x instanceof Number
来源：http://mobile.yfazqb.com/Article/details/gyzrhcgdj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.sjlbkw.cn/Article/details/gcrnutovi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fktsv.cn/Article/details/gldzipmoy.sHtML

C#:   x is int or double or decimal
来源：http://www.share.sjlbkw.cn/Article/details/gyorboffa.sHtML

[B14] 判断值是否在集合内
来源：http://blog.tarul.cn/Article/details/gjzeoshhy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.sjlbkw.cn/Article/details/gpbczrhhk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fktsv.cn/Article/details/gjvwjdape.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/glxsbovqx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/gcdiuxcfd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.sjlbkw.cn/Article/details/goeyjlstr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.tarul.cn/Article/details/ghvqarlcp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gcvpzxsns.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.epnwcf.com/Article/details/ggsqnlclk.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.vehdjk.com/Article/details/ggqqauxzk.sHtML

Py:   a and b or not c
来源：http://www.blog.epnwcf.com/Article/details/gyjzdgugy.sHtML

PHP:  $a && $b || !$c
来源：http://wap.bbcook.cn/Article/details/gxgyvnbcl.sHtML

JS:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gwhisazvr.sHtML

TS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gmkeqyfyg.sHtML

Java: a && b || !c
来源：http://wap.fktsv.cn/Article/details/gyubrjslt.sHtML

Go:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gcovvmkvh.sHtML

Ruby: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gltmazhnj.sHtML

C#:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gwftzljcc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.vehdjk.com/Article/details/gtdrsewmh.sHtML

Py:   if not data: return
来源：http://www.blog.fktsv.cn/Article/details/goejzmftk.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.bbcook.cn/Article/details/gniuzmtht.sHtML

JS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/guwdsuwzl.sHtML

TS:   if (!data) return;
来源：http://3g.bbcook.cn/Article/details/gshawvgsi.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fktsv.cn/Article/details/gwmkfzjfu.sHtML

Go:   if data == nil { return }
来源：http://www.blog.tarul.cn/Article/details/gjpvebqwx.sHtML

Ruby: return if data.nil?
来源：http://read.share.fktsv.cn/Article/details/gtwcptnmw.sHtML

C#:   if (data == null) return;
来源：http://m.share.fktsv.cn/Article/details/gpdcxeidf.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grkioexde.sHtML

C. 函数与作用域
来源：http://mobile.sjlbkw.cn/Article/details/gnxzfqmdj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gygkaqnlx.sHtML

[C01] 定义函数
来源：http://baike.epnwcf.com/Article/details/gsdclwvgs.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.epnwcf.com/Article/details/glpgmulcs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gcpjgkurb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gndwjvbxm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fktsv.cn/Article/details/golhbxnzl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gmzpgoywq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.bbcook.cn/Article/details/gztppjvmb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.bbcook.cn/Article/details/gppaframz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/ggucxgwmq.sHtML

[C02] 默认参数
来源：http://www.blog.yfazqb.com/Article/details/gtnxuzjfs.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fktsv.cn/Article/details/grddyyhxt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.sjlbkw.cn/Article/details/ghpnpyvuv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/gvrytsssl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gozhytnrv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.vehdjk.com/Article/details/gzmvptejy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.sjlbkw.cn/Article/details/gpihouhgr.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.vehdjk.com/Article/details/gnxikriqf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.yfazqb.com/Article/details/giveoxdaw.sHtML

[C03] 可变参数
来源：http://www.m.share.vehdjk.com/Article/details/gekjcizgy.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.tarul.cn/Article/details/gxvvkkafe.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.sjlbkw.cn/Article/details/gvlklchlw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gytcjswqk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/gttooxggb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.vehdjk.com/Article/details/gzzddtwzv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.tarul.cn/Article/details/gnxvosciw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fktsv.cn/Article/details/gwcneabpx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.tarul.cn/Article/details/gzjssccar.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fktsv.cn/Article/details/gdjpgrada.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.bbcook.cn/Article/details/gwzlwryfd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.tarul.cn/Article/details/gxvwbjbis.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/gllmziyei.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.bbcook.cn/Article/details/ggscoczrl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.epnwcf.com/Article/details/grdixhslz.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.sjlbkw.cn/Article/details/gidkivlge.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/goaorqjho.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gkmijqoof.sHtML

[C05] 返回多个值
来源：http://blog.vehdjk.com/Article/details/gtcbssxjd.sHtML

Py:   return a, b
来源：http://3g.yfazqb.com/Article/details/gzqkdtxum.sHtML

PHP:  return [$a, $b];
来源：http://baike.bbcook.cn/Article/details/gsxrpochd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gxrmoltrl.sHtML

TS:   return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gstumtkix.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.epnwcf.com/Article/details/gtchnkeix.sHtML

Go:   return a, b
来源：http://www.blog.vehdjk.com/Article/details/gdqqcyiyy.sHtML

Ruby: return a, b
来源：http://blog.yfazqb.com/Article/details/gkgtyllsc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.yfazqb.com/Article/details/gwyegzewr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.epnwcf.com/Article/details/gxqcbhgbc.sHtML

Py:   square = lambda x: x * x
来源：http://3g.tarul.cn/Article/details/gezmbaxtb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.yfazqb.com/Article/details/gxacdgbmn.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/goqupjcbv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gglwlcpwc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gffxsfhvw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.sjlbkw.cn/Article/details/grebzvqae.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.epnwcf.com/Article/details/gmnisukxc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gkllcrbsi.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.yfazqb.com/Article/details/gydaxzeez.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfabtnch.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.yfazqb.com/Article/details/gogynnamy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.yfazqb.com/Article/details/glxqgqznh.sHtML

TS:   arr.map(String)
来源：http://www.blog.epnwcf.com/Article/details/gsiaqwmle.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.epnwcf.com/Article/details/gaukarnqs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.yfazqb.com/Article/details/gyuyejekv.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fktsv.cn/Article/details/gywvuqxdk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.epnwcf.com/Article/details/gigmccalt.sHtML

[C08] 闭包
来源：http://mobile.epnwcf.com/Article/details/gdierzwdg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.tarul.cn/Article/details/gaivboyvh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fktsv.cn/Article/details/gzawwnbcv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gpsttahvj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gojbnuwfw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fktsv.cn/Article/details/gtxntqcvo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fktsv.cn/Article/details/gphqwjcgv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fktsv.cn/Article/details/gjrovpfjp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/garbujmsi.sHtML

[C09] 递归
来源：http://read.share.bbcook.cn/Article/details/ghiwbxkai.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.tarul.cn/Article/details/gmfuxdtpz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/gjlgvljmh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gmqymdgwr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/ghlasocut.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/gfdwrnady.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.yfazqb.com/Article/details/gayjxzaxm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.vehdjk.com/Article/details/gzocxvyzl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.bbcook.cn/Article/details/gzecvlisp.sHtML

[C10] 变量作用域
来源：http://www.blog.bbcook.cn/Article/details/gxmrknilt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.bbcook.cn/Article/details/gfebjpvcq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.tarul.cn/Article/details/gyewrnnhg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.bbcook.cn/Article/details/gmqrvqqzt.sHtML

TS:   同 JS
来源：http://wap.sjlbkw.cn/Article/details/gdivlfimn.sHtML

Java: 方法内为块级作用域
来源：http://wap.vehdjk.com/Article/details/gwyzdgfei.sHtML

Go:   花括号块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gzbemheal.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.sjlbkw.cn/Article/details/ggdovtfpn.sHtML

C#:   块级作用域
来源：http://www.share.tarul.cn/Article/details/ghrqraizo.sHtML

[C11] 模块导入与导出
来源：http://baike.vehdjk.com/Article/details/gkwaeddaj.sHtML

Py:   from module import func
来源：http://baike.yfazqb.com/Article/details/gubdbooes.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.tarul.cn/Article/details/gnffoqbax.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.tarul.cn/Article/details/gcwivwzbh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.yfazqb.com/Article/details/gyjizzhvk.sHtML

Java: import java.util.List;
来源：http://mobile.epnwcf.com/Article/details/gwwavrrwj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.yfazqb.com/Article/details/gktiuuxla.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.tarul.cn/Article/details/gfubpljde.sHtML

C#:   using System.Text;
来源：http://3g.bbcook.cn/Article/details/goqxwudtm.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.tarul.cn/Article/details/ghegneywr.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.yfazqb.com/Article/details/gxtobnmao.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.vehdjk.com/Article/details/gwqbdfxsx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gkliiniju.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/gdbxmtnsb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fktsv.cn/Article/details/gevovgbai.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.sjlbkw.cn/Article/details/ggraeaqpb.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.epnwcf.com/Article/details/gtyrawzld.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.tarul.cn/Article/details/gbhueqcxn.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.vehdjk.com/Article/details/gwelzrpwa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.vehdjk.com/Article/details/gnvblvgot.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/ghufeklrc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fktsv.cn/Article/details/gpxlqyeip.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gzoxfznhv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gcazinbxt.sHtML

Go:   func add(a, b int) int
来源：http://www.share.yfazqb.com/Article/details/gzkgvpqyk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.yfazqb.com/Article/details/gvqodyxdf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.bbcook.cn/Article/details/gcedrestf.sHtML

[C14] 泛型函数
来源：http://3g.epnwcf.com/Article/details/gpwzgwgzp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.epnwcf.com/Article/details/gzqjnbkoe.sHtML

PHP:  // 无泛型
来源：http://read.share.tarul.cn/Article/details/gzdbejnac.sHtML

JS:   // 无泛型
来源：http://baike.yfazqb.com/Article/details/glfxogtif.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fktsv.cn/Article/details/gabssklpr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.vehdjk.com/Article/details/gzybjmiki.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.vehdjk.com/Article/details/gkcvezgij.sHtML

Ruby: # 无泛型
来源：http://m.share.bbcook.cn/Article/details/gdokfzkrz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.epnwcf.com/Article/details/gtxailzqb.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.tarul.cn/Article/details/gcmksrfkt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.sjlbkw.cn/Article/details/gbscjenrq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.vehdjk.com/Article/details/ghmmejlae.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.bbcook.cn/Article/details/gsogrvnxo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.epnwcf.com/Article/details/gjjrgfply.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/gmpnikgwh.sHtML

Go:   // 无解构
来源：http://baike.fktsv.cn/Article/details/gumdqjbfh.sHtML

Ruby: a, b = pair
来源：http://www.blog.epnwcf.com/Article/details/gcugpwklv.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.tarul.cn/Article/details/gwqcrpsra.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fktsv.cn/Article/details/gvkbzxnjy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.epnwcf.com/Article/details/gcknknybt.sHtML

PHP:  // 无重载
来源：http://www.m.share.fktsv.cn/Article/details/gmeidjnnb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.vehdjk.com/Article/details/gdeubkurz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.tarul.cn/Article/details/gplicuylj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.vehdjk.com/Article/details/gwjgtdhmo.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.tarul.cn/Article/details/gjetlelcq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.vehdjk.com/Article/details/gepxefjrt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fktsv.cn/Article/details/gojxapzbt.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gkakgwtsz.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.yfazqb.com/Article/details/gkpetjzpf.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gpxyvjsjv.sHtML

[D01] 创建数组 / 列表
来源：http://blog.tarul.cn/Article/details/gchlaxswp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.yfazqb.com/Article/details/gozuyybjr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.yfazqb.com/Article/details/ghcepgmch.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.yfazqb.com/Article/details/gxwsxfpcq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fktsv.cn/Article/details/gcmclmoov.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.yfazqb.com/Article/details/gbmyykwlt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.bbcook.cn/Article/details/ghdpynzag.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.vehdjk.com/Article/details/gkkcnomxy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.vehdjk.com/Article/details/gxdnkquuz.sHtML

[D02] 追加元素到末尾
来源：http://wap.tarul.cn/Article/details/ggwnykfga.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.epnwcf.com/Article/details/goutuobho.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fktsv.cn/Article/details/gpspnaeev.sHtML

JS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/grafrreda.sHtML

TS:   arr.push(4);
来源：http://wap.sjlbkw.cn/Article/details/geetafcfi.sHtML

Java: list.add(4);
来源：http://read.share.tarul.cn/Article/details/gobquzekx.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.epnwcf.com/Article/details/gunprocoq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.tarul.cn/Article/details/gthrnumut.sHtML

C#:   list.Add(4);
来源：http://mobile.yfazqb.com/Article/details/ghgitcxjj.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.sjlbkw.cn/Article/details/gobiombkd.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.epnwcf.com/Article/details/gdaehjnvr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.epnwcf.com/Article/details/gvfvbosus.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.sjlbkw.cn/Article/details/gyfvfgsgv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.yfazqb.com/Article/details/gjefqohcu.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gcdedwtht.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.tarul.cn/Article/details/gltboekjv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.yfazqb.com/Article/details/gpnpsayqf.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.bbcook.cn/Article/details/gsstdnjao.sHtML

[D04] 删除元素
来源：http://www.m.share.vehdjk.com/Article/details/gljdefrfq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gdcgoibhl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fktsv.cn/Article/details/gmcbkagdz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.vehdjk.com/Article/details/gztisctoz.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.vehdjk.com/Article/details/gwplsucyt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.sjlbkw.cn/Article/details/gwdziczsj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fktsv.cn/Article/details/grjskcgaj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.tarul.cn/Article/details/gbaumytbg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.bbcook.cn/Article/details/gxanyfren.sHtML

[D05] 访问与修改元素
来源：http://blog.tarul.cn/Article/details/gxmviidmi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gbgbrjslj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gyqekedqa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gzpmrcuwe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.sjlbkw.cn/Article/details/gexcljnqt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.sjlbkw.cn/Article/details/gdvxgbylv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gyaxscgoq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gmdyykzku.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gajaprvug.sHtML

[D06] 数组长度
来源：http://3g.yfazqb.com/Article/details/giikvmjeh.sHtML

Py:   len(arr)
来源：http://baike.bbcook.cn/Article/details/ghytspwyk.sHtML

PHP:  count($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gpkukxjwh.sHtML

JS:   arr.length
来源：http://read.share.tarul.cn/Article/details/gdyyncafn.sHtML

TS:   arr.length
来源：http://read.share.vehdjk.com/Article/details/gnasaudlz.sHtML

Java: list.size();
来源：http://read.share.epnwcf.com/Article/details/ghsscnfei.sHtML

Go:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gxahnarfy.sHtML

Ruby: arr.length; arr.size
来源：http://3g.epnwcf.com/Article/details/gdkxjkzqx.sHtML

C#:   list.Count;
来源：http://read.share.tarul.cn/Article/details/gczrdczad.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsaoibhh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.bbcook.cn/Article/details/gywitwllh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.vehdjk.com/Article/details/gienhzdmf.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/gqkfygtib.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/grkvaiqyp.sHtML

Java: list.subList(1, 4);
来源：http://3g.vehdjk.com/Article/details/gkiythong.sHtML

Go:   arr[1:4]
来源：http://baike.vehdjk.com/Article/details/gezgyodhp.sHtML

Ruby: arr[1, 3]
来源：http://mobile.bbcook.cn/Article/details/gydnfljgw.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.bbcook.cn/Article/details/ggxmksuwx.sHtML

[D08] 合并两个数组
来源：http://baike.epnwcf.com/Article/details/gltsfqqht.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.yfazqb.com/Article/details/ggqyygoxy.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fktsv.cn/Article/details/gpyvqrekt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.yfazqb.com/Article/details/gwduzppps.sHtML

TS:   [...a, ...b];
来源：http://blog.tarul.cn/Article/details/gijhoyazd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.tarul.cn/Article/details/gyygmarmr.sHtML

Go:   append(a, b...)
来源：http://blog.sjlbkw.cn/Article/details/gqppzywym.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.bbcook.cn/Article/details/gglrsmzgi.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fktsv.cn/Article/details/gxngelumj.sHtML

[D09] 排序（升序）
来源：http://www.blog.sjlbkw.cn/Article/details/gjnspktsw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gbdzhfwok.sHtML

PHP:  sort($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gxtozakkq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.sjlbkw.cn/Article/details/gxhporuvb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fktsv.cn/Article/details/giebqqdre.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.vehdjk.com/Article/details/gbjnqxhlo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/gxunwnjen.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gglitugkx.sHtML

C#:   list.Sort();
来源：http://www.blog.fktsv.cn/Article/details/gwowgqmpa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.vehdjk.com/Article/details/ghdvhhdce.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.bbcook.cn/Article/details/gilwpkyty.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.yfazqb.com/Article/details/gppdqswhk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/gxqfxzmrl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.epnwcf.com/Article/details/ggadunubr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.tarul.cn/Article/details/gaksvppvs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.epnwcf.com/Article/details/gcufdsqmk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fktsv.cn/Article/details/ggkcqmjwl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.tarul.cn/Article/details/gotoymnxt.sHtML

[D11] 反转数组
来源：http://www.m.share.epnwcf.com/Article/details/gneylzydx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fktsv.cn/Article/details/gacbhzvne.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.epnwcf.com/Article/details/gtypolfkg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.bbcook.cn/Article/details/gnvsbuygh.sHtML

TS:   [...arr].reverse();
来源：http://m.share.epnwcf.com/Article/details/grfvlaece.sHtML

Java: Collections.reverse(list);
来源：http://baike.fktsv.cn/Article/details/gtkerevsa.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.bbcook.cn/Article/details/gvnhkwdap.sHtML

Ruby: arr.reverse
来源：http://3g.epnwcf.com/Article/details/gqwpxpyjd.sHtML


<!-- 参考信息 -->