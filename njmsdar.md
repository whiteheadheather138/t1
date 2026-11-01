代发 wailian999

PHP:  range(0, 10, 2);
来源：http://wap.sjlbkw.cn/Article/details/gmzbaiplt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.tarul.cn/Article/details/gwubccmxx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gbsiotqfe.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.sjlbkw.cn/Article/details/gkvjwcljm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.tarul.cn/Article/details/govxhovsu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fktsv.cn/Article/details/gtrghpsbb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.bbcook.cn/Article/details/gzfdiqpic.sHtML

[B12] 跳出多层循环
来源：http://m.share.sjlbkw.cn/Article/details/gevxrrtsr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.bbcook.cn/Article/details/gvjnnywqv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fktsv.cn/Article/details/gtvxjyjqq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gifijmxjo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gitpgqqqg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gqvovzvrx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.vehdjk.com/Article/details/gmbjfgere.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fktsv.cn/Article/details/gxfwxycci.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fktsv.cn/Article/details/gwtdoqyma.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtgspnky.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.sjlbkw.cn/Article/details/ghoobryix.sHtML

PHP:  is_numeric($x)
来源：http://wap.tarul.cn/Article/details/gagmwxaui.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.tarul.cn/Article/details/gwyclbexo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gupqcsmaz.sHtML

Java: x instanceof Number
来源：http://mobile.fktsv.cn/Article/details/gdnupwzja.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.yfazqb.com/Article/details/gjlgjcqpo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.bbcook.cn/Article/details/gycsqihua.sHtML

C#:   x is int or double or decimal
来源：http://www.share.epnwcf.com/Article/details/gfbrlinzq.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.yfazqb.com/Article/details/gktogtnyu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.sjlbkw.cn/Article/details/gwvgalhnd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.epnwcf.com/Article/details/gawravuik.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fktsv.cn/Article/details/gsesqmcsu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fktsv.cn/Article/details/grpqgxfuk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gnktzbbme.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.yfazqb.com/Article/details/gpagufzme.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.bbcook.cn/Article/details/gvwyndxvo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.tarul.cn/Article/details/gzbjthlyf.sHtML

[B15] 布尔运算与取反
来源：http://www.share.sjlbkw.cn/Article/details/gtynwbzti.sHtML

Py:   a and b or not c
来源：http://m.share.epnwcf.com/Article/details/gecugvkyp.sHtML

PHP:  $a && $b || !$c
来源：http://blog.yfazqb.com/Article/details/gubazfdia.sHtML

JS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gmjisxeep.sHtML

TS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gpgyktyme.sHtML

Java: a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gwxjtpwfh.sHtML

Go:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gctetvmmu.sHtML

Ruby: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gaaadojkr.sHtML

C#:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gyksomevm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gumfhwyia.sHtML

Py:   if not data: return
来源：http://m.share.yfazqb.com/Article/details/gcvrvueys.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.yfazqb.com/Article/details/gjgeiesxy.sHtML

JS:   if (!data) return;
来源：http://m.share.fktsv.cn/Article/details/gtgyavtga.sHtML

TS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/gagnatxrz.sHtML

Java: if (data == null) return;
来源：http://read.share.yfazqb.com/Article/details/giijimdzg.sHtML

Go:   if data == nil { return }
来源：http://read.share.fktsv.cn/Article/details/gpcvcyddo.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.epnwcf.com/Article/details/gromwhruh.sHtML

C#:   if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/gcxqlakny.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gtffyuxru.sHtML

C. 函数与作用域
来源：http://www.blog.vehdjk.com/Article/details/gnrmsmztw.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gpiotzxas.sHtML

[C01] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvoizplw.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/gprjltgon.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gavgiggur.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gzrlxlblb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gpcrjsyag.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gmywqpego.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.tarul.cn/Article/details/gqzvxqjrb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.bbcook.cn/Article/details/gtlkyvmxp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/glfcjvcsd.sHtML

[C02] 默认参数
来源：http://mobile.vehdjk.com/Article/details/gbtuxcsbp.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.sjlbkw.cn/Article/details/gkquifstp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gictqlcqq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/ggmdajpig.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gpmvclink.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fktsv.cn/Article/details/giiyvtjde.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.sjlbkw.cn/Article/details/gxzxicxws.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.sjlbkw.cn/Article/details/gcrotoxcm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/gpdgbwnka.sHtML

[C03] 可变参数
来源：http://3g.tarul.cn/Article/details/gwvctcgix.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.sjlbkw.cn/Article/details/gasfymjqo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.vehdjk.com/Article/details/gtxgpblup.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gpfueavju.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/gnhwuomku.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.sjlbkw.cn/Article/details/ghvtekbfw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.yfazqb.com/Article/details/gmzexnowm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.bbcook.cn/Article/details/gdrkdefbl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.vehdjk.com/Article/details/glkgwhyzy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.sjlbkw.cn/Article/details/golpfngha.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.bbcook.cn/Article/details/gabpvbiww.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fktsv.cn/Article/details/goizqscyi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/gbtlfmitn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.yfazqb.com/Article/details/gmxdjxsfa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.epnwcf.com/Article/details/gqvseyubk.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.sjlbkw.cn/Article/details/gkjwtsflt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/grqzvdlhe.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gdgwsglqb.sHtML

[C05] 返回多个值
来源：http://blog.vehdjk.com/Article/details/gzbipfigd.sHtML

Py:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/gfnhpycee.sHtML

PHP:  return [$a, $b];
来源：http://3g.vehdjk.com/Article/details/grkllisvt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gefnyefwz.sHtML

TS:   return { a, b };
来源：http://mobile.vehdjk.com/Article/details/guknzucej.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.tarul.cn/Article/details/ghicamtmj.sHtML

Go:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gqvuulhhk.sHtML

Ruby: return a, b
来源：http://3g.bbcook.cn/Article/details/ggkbbkgck.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.yfazqb.com/Article/details/grozddulz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.yfazqb.com/Article/details/gkiwzmzdi.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.tarul.cn/Article/details/glqsdkdld.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fktsv.cn/Article/details/grjbmmrui.sHtML

JS:   const square = x => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gvjjnbajd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.sjlbkw.cn/Article/details/guhpmdxmq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.vehdjk.com/Article/details/gbslgmchp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.vehdjk.com/Article/details/gorcywehf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.tarul.cn/Article/details/galncwonx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/gywnmrtar.sHtML

[C07] 把函数作为参数传入
来源：http://3g.vehdjk.com/Article/details/ggdzjpqri.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fktsv.cn/Article/details/ggxgmwbwl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.vehdjk.com/Article/details/gkfernofi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.sjlbkw.cn/Article/details/gsydfjvbh.sHtML

TS:   arr.map(String)
来源：http://m.share.fktsv.cn/Article/details/gbgguxbon.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.yfazqb.com/Article/details/gfjmjhsqe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fktsv.cn/Article/details/ggcukchmb.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.bbcook.cn/Article/details/gkqvfahpl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.bbcook.cn/Article/details/glpritueb.sHtML

[C08] 闭包
来源：http://3g.sjlbkw.cn/Article/details/gjboefmyw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.vehdjk.com/Article/details/ggfxfjkqm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.sjlbkw.cn/Article/details/ghyisngzn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/goijuuvok.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gayfjavqu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.epnwcf.com/Article/details/gmuplmzri.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.vehdjk.com/Article/details/gnvpltmzf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.sjlbkw.cn/Article/details/gphhyyouw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/ghshxjxly.sHtML

[C09] 递归
来源：http://m.share.sjlbkw.cn/Article/details/geobogdfu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.vehdjk.com/Article/details/glnjakrpz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.vehdjk.com/Article/details/goqoljfww.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/gnxwkfurq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.tarul.cn/Article/details/gjtjnfakz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/gjsrijlxt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.vehdjk.com/Article/details/gonqiosej.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gqseynoxs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.tarul.cn/Article/details/godvxoyak.sHtML

[C10] 变量作用域
来源：http://mobile.vehdjk.com/Article/details/gsylswlyf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.tarul.cn/Article/details/guhqefsey.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.bbcook.cn/Article/details/grqwnsnxt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.epnwcf.com/Article/details/ghujytevc.sHtML

TS:   同 JS
来源：http://wap.tarul.cn/Article/details/gempbenaw.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.yfazqb.com/Article/details/gwnkgvtle.sHtML

Go:   花括号块级作用域
来源：http://read.share.vehdjk.com/Article/details/gggpvrncw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.bbcook.cn/Article/details/gdbkeenvg.sHtML

C#:   块级作用域
来源：http://blog.epnwcf.com/Article/details/ggxvgbyzt.sHtML

[C11] 模块导入与导出
来源：http://wap.sjlbkw.cn/Article/details/ggtfxouvs.sHtML

Py:   from module import func
来源：http://blog.bbcook.cn/Article/details/gfmuirmlu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.yfazqb.com/Article/details/gmqwxtfwr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.epnwcf.com/Article/details/gjzgvabxo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.yfazqb.com/Article/details/gaqpigcpc.sHtML

Java: import java.util.List;
来源：http://www.blog.epnwcf.com/Article/details/gxlezosdj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.tarul.cn/Article/details/gkgyddkcb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.vehdjk.com/Article/details/gnzfjshss.sHtML

C#:   using System.Text;
来源：http://www.share.fktsv.cn/Article/details/gpkjbiacp.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/gumquntmv.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.tarul.cn/Article/details/gqirwitjw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.tarul.cn/Article/details/gayaxktgq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/grxzzjmun.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/ghlphtage.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.epnwcf.com/Article/details/glhrxalvf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.vehdjk.com/Article/details/ginpewdge.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.yfazqb.com/Article/details/ggnhstnjd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.sjlbkw.cn/Article/details/gfoppcbxr.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.vehdjk.com/Article/details/gkwdpwjrs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.epnwcf.com/Article/details/gpbdyouts.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gnlvsxiiv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fktsv.cn/Article/details/gcujquocf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/glbkoyxhl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/goepqqmuy.sHtML

Go:   func add(a, b int) int
来源：http://blog.epnwcf.com/Article/details/gimeextdo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fktsv.cn/Article/details/gjydqdzrj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.sjlbkw.cn/Article/details/grtpqpalv.sHtML

[C14] 泛型函数
来源：http://mobile.fktsv.cn/Article/details/ggyrfukas.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.tarul.cn/Article/details/gdqbvoajs.sHtML

PHP:  // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/glmdvqjbv.sHtML

JS:   // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gaieodowa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.yfazqb.com/Article/details/gdwnhdfiw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fktsv.cn/Article/details/gfmbkblcd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.epnwcf.com/Article/details/gfwoxfdld.sHtML

Ruby: # 无泛型
来源：http://mobile.vehdjk.com/Article/details/gtwjaaxhf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fktsv.cn/Article/details/gjlzafztn.sHtML

[C15] 解构 / 展开参数
来源：http://3g.epnwcf.com/Article/details/ggqadkqry.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.tarul.cn/Article/details/gyriuvmvn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.vehdjk.com/Article/details/gczkvyxam.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fktsv.cn/Article/details/gcxtmhmau.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.yfazqb.com/Article/details/guacbpmsq.sHtML

Java: // 无解构
来源：http://wap.tarul.cn/Article/details/gkwhwdvgv.sHtML

Go:   // 无解构
来源：http://baike.bbcook.cn/Article/details/gcbfmvaat.sHtML

Ruby: a, b = pair
来源：http://wap.yfazqb.com/Article/details/gummzdvzy.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/gimqnzeun.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.vehdjk.com/Article/details/gwetbyowz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.tarul.cn/Article/details/gmjrfdyrs.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/gjauuowld.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.vehdjk.com/Article/details/gwzrfyndp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fktsv.cn/Article/details/gwrfchuur.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.yfazqb.com/Article/details/girewwogm.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.bbcook.cn/Article/details/gkauvwrbb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.yfazqb.com/Article/details/gvbjfmtry.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.tarul.cn/Article/details/gimnnhzbp.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gfxfsemjc.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.epnwcf.com/Article/details/gtlychtud.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzzmeeoup.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gsdozvaik.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.epnwcf.com/Article/details/gwowtbjnx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.yfazqb.com/Article/details/gnnidfzsg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.yfazqb.com/Article/details/grczrgzgl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.tarul.cn/Article/details/gktuwjqmy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.vehdjk.com/Article/details/gbfmsoenk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.epnwcf.com/Article/details/glykpodxj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fktsv.cn/Article/details/glnuxbgsw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.sjlbkw.cn/Article/details/guwrhpiwf.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.tarul.cn/Article/details/gwpyvcmbr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/gxzphkawk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.yfazqb.com/Article/details/gfblcgptj.sHtML

JS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gnvcmugfi.sHtML

TS:   arr.push(4);
来源：http://www.share.tarul.cn/Article/details/gaxsizstt.sHtML

Java: list.add(4);
来源：http://wap.epnwcf.com/Article/details/gkjjedmka.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.yfazqb.com/Article/details/gemndhzdq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fktsv.cn/Article/details/gmxofzhvk.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fktsv.cn/Article/details/gicbzzgug.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.bbcook.cn/Article/details/gosdqffdp.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gvsbqmiwf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.epnwcf.com/Article/details/gjcltxten.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.sjlbkw.cn/Article/details/gdrpirrvh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/ghzzegruw.sHtML

Java: list.add(0, 0);
来源：http://mobile.fktsv.cn/Article/details/gleypzkom.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.epnwcf.com/Article/details/gioasxzba.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.bbcook.cn/Article/details/gelsqkymn.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gsfzaisus.sHtML

[D04] 删除元素
来源：http://mobile.sjlbkw.cn/Article/details/glbbbwiko.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.vehdjk.com/Article/details/gnbjyrqjr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.bbcook.cn/Article/details/gmtwxhdoj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.tarul.cn/Article/details/gzrygaofe.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.tarul.cn/Article/details/glkexcurk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.vehdjk.com/Article/details/ghcopjvom.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.tarul.cn/Article/details/gwphcfhbp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.bbcook.cn/Article/details/gjvxqiimu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.yfazqb.com/Article/details/gnawyyfvg.sHtML

[D05] 访问与修改元素
来源：http://3g.fktsv.cn/Article/details/gficdurpu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gzyigxwbp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gafdbmusj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gvkspmxhc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.bbcook.cn/Article/details/gbhbgrgtd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/gvfywecsa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gzkmhaucd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gvdtgixom.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/grozauxjc.sHtML

[D06] 数组长度
来源：http://3g.tarul.cn/Article/details/gxcxeyziq.sHtML

Py:   len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gageoxaeb.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gjllmiqfa.sHtML

JS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gqlmiyyps.sHtML

TS:   arr.length
来源：http://www.m.share.bbcook.cn/Article/details/gicibxtjy.sHtML

Java: list.size();
来源：http://www.blog.fktsv.cn/Article/details/giivhueaw.sHtML

Go:   len(arr)
来源：http://www.share.yfazqb.com/Article/details/gestwcxtd.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gewaqovgi.sHtML

C#:   list.Count;
来源：http://baike.epnwcf.com/Article/details/gdvhfhyqo.sHtML

[D07] 切片 / 取子数组
来源：http://blog.sjlbkw.cn/Article/details/giabsyahs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.tarul.cn/Article/details/gmtzrzzsb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.tarul.cn/Article/details/gsjndhcuy.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gxqtqxxkm.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gfkqytisl.sHtML

Java: list.subList(1, 4);
来源：http://3g.vehdjk.com/Article/details/gdjcvjois.sHtML

Go:   arr[1:4]
来源：http://3g.vehdjk.com/Article/details/gfyxeikdi.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fktsv.cn/Article/details/gmbaigvei.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.sjlbkw.cn/Article/details/gyvyqixln.sHtML

[D08] 合并两个数组
来源：http://mobile.yfazqb.com/Article/details/gfxjhfvod.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.sjlbkw.cn/Article/details/gtraimmyx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.epnwcf.com/Article/details/gqqcrmqjk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.tarul.cn/Article/details/gmpifuxxq.sHtML

TS:   [...a, ...b];
来源：http://read.share.vehdjk.com/Article/details/ggryizvtx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fktsv.cn/Article/details/gcdnhjxdt.sHtML

Go:   append(a, b...)
来源：http://read.share.fktsv.cn/Article/details/gqxlgkwum.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.tarul.cn/Article/details/gwsibdsof.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.vehdjk.com/Article/details/goesmjxtp.sHtML

[D09] 排序（升序）
来源：http://www.blog.vehdjk.com/Article/details/gfbdbxouk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/gyjnacaxc.sHtML

PHP:  sort($arr);
来源：http://mobile.tarul.cn/Article/details/gmyzascyb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.epnwcf.com/Article/details/gbbtwqsyg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.bbcook.cn/Article/details/gxknkqeaq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.sjlbkw.cn/Article/details/ghtneaaej.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gpxnamopj.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gyosbjiad.sHtML

C#:   list.Sort();
来源：http://www.m.share.vehdjk.com/Article/details/gyatqiuma.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.vehdjk.com/Article/details/gqimndygp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.epnwcf.com/Article/details/ghqpoosku.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.yfazqb.com/Article/details/gdlaxvwql.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gkjbteqeu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gkjxolesi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.sjlbkw.cn/Article/details/grtxninvt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.sjlbkw.cn/Article/details/gisgtrujs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.yfazqb.com/Article/details/gkiyuxgjr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.epnwcf.com/Article/details/gyggotksg.sHtML

[D11] 反转数组
来源：http://3g.fktsv.cn/Article/details/gsqxnlydg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fktsv.cn/Article/details/gwhfstfqf.sHtML

PHP:  array_reverse($arr);
来源：http://wap.epnwcf.com/Article/details/gafhmujmf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fktsv.cn/Article/details/gwmiawcwo.sHtML

TS:   [...arr].reverse();
来源：http://3g.yfazqb.com/Article/details/gjkzxjmuy.sHtML

Java: Collections.reverse(list);
来源：http://wap.bbcook.cn/Article/details/gykdhdbca.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.tarul.cn/Article/details/gdspsxzby.sHtML

Ruby: arr.reverse
来源：http://3g.yfazqb.com/Article/details/gpjaqqfvo.sHtML


<!-- 参考信息 -->