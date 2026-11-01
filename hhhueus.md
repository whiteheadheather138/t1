代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.tarul.cn/Article/details/gmasfisee.sHtML

Java: x instanceof Number
来源：http://blog.sjlbkw.cn/Article/details/gidrxccar.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.vehdjk.com/Article/details/gaopkbyss.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.sjlbkw.cn/Article/details/gmoiljcli.sHtML

C#:   x is int or double or decimal
来源：http://3g.tarul.cn/Article/details/gbbivfosy.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.yfazqb.com/Article/details/gunsiizxw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.vehdjk.com/Article/details/gngezpnyg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.epnwcf.com/Article/details/gqjdnpwhh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gysixpare.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gaqvogydw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gneptfhvl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.bbcook.cn/Article/details/gnhbysvuw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.yfazqb.com/Article/details/gavgrkeme.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gygbfaxry.sHtML

[B15] 布尔运算与取反
来源：http://mobile.yfazqb.com/Article/details/ghrwszgrc.sHtML

Py:   a and b or not c
来源：http://www.m.share.epnwcf.com/Article/details/gyqnicecj.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.sjlbkw.cn/Article/details/gwgnczbxk.sHtML

JS:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gznllexmx.sHtML

TS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gmdjuebdm.sHtML

Java: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gwvvjoohn.sHtML

Go:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gcehujdxz.sHtML

Ruby: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gegvvsuat.sHtML

C#:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/goxeyphtr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.bbcook.cn/Article/details/gjqbtgmpq.sHtML

Py:   if not data: return
来源：http://www.m.share.bbcook.cn/Article/details/gszmdwztt.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.epnwcf.com/Article/details/glncqtrup.sHtML

JS:   if (!data) return;
来源：http://baike.epnwcf.com/Article/details/gpgdubyvl.sHtML

TS:   if (!data) return;
来源：http://blog.yfazqb.com/Article/details/gdchdxmzs.sHtML

Java: if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/gjgorumpr.sHtML

Go:   if data == nil { return }
来源：http://3g.fktsv.cn/Article/details/gmwfovisx.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.tarul.cn/Article/details/gmzbjyslr.sHtML

C#:   if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/ggdcfegjn.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gegarsaur.sHtML

C. 函数与作用域
来源：http://www.blog.fktsv.cn/Article/details/gjdjierlo.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/glsxkwatn.sHtML

[C01] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/gniwlzvvd.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.bbcook.cn/Article/details/gnuiiywjj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gaxczkthj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gxkuppvaf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gwnjpmabo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gkbjvbcqd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gmvmkeyas.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.epnwcf.com/Article/details/gwecqryej.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gqsbwzkrk.sHtML

[C02] 默认参数
来源：http://read.share.epnwcf.com/Article/details/gudjprjkd.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.sjlbkw.cn/Article/details/gxwypwulb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.vehdjk.com/Article/details/gtgfwvsnl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.tarul.cn/Article/details/ggpmfzxpg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gqxlrtfnl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.epnwcf.com/Article/details/gorxkqnwh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.epnwcf.com/Article/details/giwqpimpw.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.vehdjk.com/Article/details/glfpabvou.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.bbcook.cn/Article/details/gfeirkhtj.sHtML

[C03] 可变参数
来源：http://3g.sjlbkw.cn/Article/details/ggqugmbch.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.bbcook.cn/Article/details/gaauyxycl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.yfazqb.com/Article/details/gutojhqaf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/gvlyijeyg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/gmsxtxlmh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.epnwcf.com/Article/details/guliutalf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.yfazqb.com/Article/details/glmrypvvc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.vehdjk.com/Article/details/gaymumbjk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.tarul.cn/Article/details/glchsgvfw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.sjlbkw.cn/Article/details/gxdfttzhi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.vehdjk.com/Article/details/goyyybbce.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.bbcook.cn/Article/details/gszdglagg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gwqqgxilq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.vehdjk.com/Article/details/giyctgjce.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqpatfmr.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.vehdjk.com/Article/details/ghckrzzbj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/goqtcjdlb.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gwlgqkmsx.sHtML

[C05] 返回多个值
来源：http://www.blog.sjlbkw.cn/Article/details/gyltbtsti.sHtML

Py:   return a, b
来源：http://www.blog.tarul.cn/Article/details/gbllrbwwk.sHtML

PHP:  return [$a, $b];
来源：http://mobile.vehdjk.com/Article/details/gfixbqrbr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.sjlbkw.cn/Article/details/gggrdswgk.sHtML

TS:   return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/gwbmwtfmc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.bbcook.cn/Article/details/gdmfztcjr.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/ghsdvpofh.sHtML

Ruby: return a, b
来源：http://mobile.tarul.cn/Article/details/ghcomhrrt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.bbcook.cn/Article/details/gxpqhhatr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.tarul.cn/Article/details/gjthqikcj.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.bbcook.cn/Article/details/gmnjqpmdt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.vehdjk.com/Article/details/gmqncjise.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.bbcook.cn/Article/details/giwgmrtis.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fktsv.cn/Article/details/ggasvbnuw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.tarul.cn/Article/details/gybiddrqa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fktsv.cn/Article/details/gwdqajnkb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.epnwcf.com/Article/details/gdjuapcwe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.tarul.cn/Article/details/grxqakcbu.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.tarul.cn/Article/details/gxxlcvxuf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.vehdjk.com/Article/details/gnvlbacmy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.bbcook.cn/Article/details/gnbyqrezj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.sjlbkw.cn/Article/details/gsbleqdvc.sHtML

TS:   arr.map(String)
来源：http://m.share.tarul.cn/Article/details/gdgzvhrnc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.yfazqb.com/Article/details/gnilqajan.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.yfazqb.com/Article/details/gvhjrmjdk.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fktsv.cn/Article/details/gzlsqzupx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.tarul.cn/Article/details/gftodhqso.sHtML

[C08] 闭包
来源：http://read.share.fktsv.cn/Article/details/gueghwgqp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.vehdjk.com/Article/details/gydotmllj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.vehdjk.com/Article/details/ghrmhtpxr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gtzvzczuu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gzieeffkp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.bbcook.cn/Article/details/grwdaoqrh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.yfazqb.com/Article/details/ghuwvtnwd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.vehdjk.com/Article/details/ghtluvvwu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gdbzsngsm.sHtML

[C09] 递归
来源：http://www.share.bbcook.cn/Article/details/glgogugpx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gvytbpsyw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.bbcook.cn/Article/details/gsxhehqff.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/gsajkjzxe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/giywtrosx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.vehdjk.com/Article/details/gnuavafoh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fktsv.cn/Article/details/gwnkrwqhe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fktsv.cn/Article/details/gakddbeir.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.yfazqb.com/Article/details/gwgvrxzpu.sHtML

[C10] 变量作用域
来源：http://blog.epnwcf.com/Article/details/gdyzmpovh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.sjlbkw.cn/Article/details/ghmwrdjvs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.vehdjk.com/Article/details/giwsmzipp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.yfazqb.com/Article/details/gixrgbmlm.sHtML

TS:   同 JS
来源：http://www.blog.bbcook.cn/Article/details/gddwtlbmw.sHtML

Java: 方法内为块级作用域
来源：http://read.share.tarul.cn/Article/details/gqedxvyna.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gfxppiwko.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.epnwcf.com/Article/details/gdfgpofik.sHtML

C#:   块级作用域
来源：http://m.share.vehdjk.com/Article/details/gvjyrybdr.sHtML

[C11] 模块导入与导出
来源：http://wap.epnwcf.com/Article/details/gshttftod.sHtML

Py:   from module import func
来源：http://m.share.sjlbkw.cn/Article/details/gwepfiarj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.tarul.cn/Article/details/gkirdqask.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.vehdjk.com/Article/details/galdsgnij.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.sjlbkw.cn/Article/details/gdhylexrc.sHtML

Java: import java.util.List;
来源：http://read.share.vehdjk.com/Article/details/gytazthkz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwxhgegy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.vehdjk.com/Article/details/guvyiewvm.sHtML

C#:   using System.Text;
来源：http://3g.yfazqb.com/Article/details/gkvdgipip.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fktsv.cn/Article/details/grtyxlftz.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.bbcook.cn/Article/details/gwuvniudi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.yfazqb.com/Article/details/gmbaedmhj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/geaagisms.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/gndvqeijr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fktsv.cn/Article/details/gerbjrcpv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.epnwcf.com/Article/details/gvluzrjgr.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.tarul.cn/Article/details/ghkwtqsev.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gpelnmpss.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.yfazqb.com/Article/details/gfbrmlgqv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.sjlbkw.cn/Article/details/gpkekrogf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gqnpxqaqa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.vehdjk.com/Article/details/gabeocbfe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/giumovytl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gnhzvujit.sHtML

Go:   func add(a, b int) int
来源：http://baike.tarul.cn/Article/details/gxuxiaqkr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.vehdjk.com/Article/details/gcspiboib.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.sjlbkw.cn/Article/details/gxckwtalu.sHtML

[C14] 泛型函数
来源：http://read.share.sjlbkw.cn/Article/details/gqrzoeitl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.bbcook.cn/Article/details/goscjrmqx.sHtML

PHP:  // 无泛型
来源：http://www.blog.vehdjk.com/Article/details/gaxhkxits.sHtML

JS:   // 无泛型
来源：http://wap.bbcook.cn/Article/details/gqhqilymk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.yfazqb.com/Article/details/gcutfuwtp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.yfazqb.com/Article/details/ghnpwtlzy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.tarul.cn/Article/details/gemyemvek.sHtML

Ruby: # 无泛型
来源：http://blog.tarul.cn/Article/details/gawhhloyr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.bbcook.cn/Article/details/gxodbmoek.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.yfazqb.com/Article/details/gaddsrpye.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fktsv.cn/Article/details/ggeikiddl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.sjlbkw.cn/Article/details/gguwnjnbh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/ghchgwvqu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.vehdjk.com/Article/details/gxriqmwrh.sHtML

Java: // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gcdjdthll.sHtML

Go:   // 无解构
来源：http://www.share.epnwcf.com/Article/details/gickqqfln.sHtML

Ruby: a, b = pair
来源：http://mobile.vehdjk.com/Article/details/gavezceux.sHtML

C#:   var (a, b) = pair;
来源：http://blog.epnwcf.com/Article/details/gyacsnmoj.sHtML

[C16] 函数 / 方法重载
来源：http://3g.sjlbkw.cn/Article/details/glamhmmzf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.epnwcf.com/Article/details/gjihhvgyt.sHtML

PHP:  // 无重载
来源：http://mobile.yfazqb.com/Article/details/gcsyenazg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gcxqfhagd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.yfazqb.com/Article/details/gfoicjrce.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.vehdjk.com/Article/details/gfwzhelqb.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.yfazqb.com/Article/details/gbjncbqop.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.sjlbkw.cn/Article/details/giflubwdu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.vehdjk.com/Article/details/gmiujdxjz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gazgkhjsg.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.yfazqb.com/Article/details/gnkiyzzyp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtdbomzmx.sHtML

[D01] 创建数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gzprcpuur.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.yfazqb.com/Article/details/gjdliumii.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/gqjkvagwj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fktsv.cn/Article/details/gjualbput.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fktsv.cn/Article/details/ggzfehliz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.epnwcf.com/Article/details/gxbhvnmsg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.yfazqb.com/Article/details/geevmcqvw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gtfpsquvr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fktsv.cn/Article/details/gcabvppac.sHtML

[D02] 追加元素到末尾
来源：http://mobile.tarul.cn/Article/details/gqjwgfxga.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.epnwcf.com/Article/details/gxsokstuk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.tarul.cn/Article/details/guclhwqyt.sHtML

JS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/gytscguiu.sHtML

TS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/gvjeurfct.sHtML

Java: list.add(4);
来源：http://www.m.share.bbcook.cn/Article/details/gsluzyogu.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gprdpbdpp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.sjlbkw.cn/Article/details/gwznrkqoe.sHtML

C#:   list.Add(4);
来源：http://www.share.bbcook.cn/Article/details/goiefgzgx.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.yfazqb.com/Article/details/gedevwdoo.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fktsv.cn/Article/details/gvybsrldc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.sjlbkw.cn/Article/details/gnicxyesw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fktsv.cn/Article/details/grnubzcxf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.tarul.cn/Article/details/gsihcafnd.sHtML

Java: list.add(0, 0);
来源：http://blog.bbcook.cn/Article/details/gnjzijqbe.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrhewipw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.bbcook.cn/Article/details/ggoueaqxa.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gdjkiplmt.sHtML

[D04] 删除元素
来源：http://mobile.sjlbkw.cn/Article/details/gfbjptzda.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.vehdjk.com/Article/details/gsxdqzxvn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.bbcook.cn/Article/details/gtpwijlay.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.sjlbkw.cn/Article/details/gnwiobghs.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.epnwcf.com/Article/details/ggqnbjith.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.tarul.cn/Article/details/gaaxddwkv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.sjlbkw.cn/Article/details/guykrcdbi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/geibodnxk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fktsv.cn/Article/details/gkloumszi.sHtML

[D05] 访问与修改元素
来源：http://read.share.tarul.cn/Article/details/gzunnhaeg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gembhjtwy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gmmcjdypd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.yfazqb.com/Article/details/goarqopqt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.tarul.cn/Article/details/gkusamuzo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.epnwcf.com/Article/details/gxcjrscow.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/givfkxqlj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/glwvzgavp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gellhrsnz.sHtML

[D06] 数组长度
来源：http://3g.bbcook.cn/Article/details/gfkxgnckp.sHtML

Py:   len(arr)
来源：http://read.share.tarul.cn/Article/details/gxhhpgtnc.sHtML

PHP:  count($arr);
来源：http://3g.sjlbkw.cn/Article/details/gjtyotxeb.sHtML

JS:   arr.length
来源：http://www.blog.epnwcf.com/Article/details/gtzfomlgo.sHtML

TS:   arr.length
来源：http://wap.tarul.cn/Article/details/gdqkskdvi.sHtML

Java: list.size();
来源：http://www.blog.sjlbkw.cn/Article/details/gnkonnxbn.sHtML

Go:   len(arr)
来源：http://m.share.fktsv.cn/Article/details/gxeoarbov.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.vehdjk.com/Article/details/gzoyhsmhj.sHtML

C#:   list.Count;
来源：http://mobile.fktsv.cn/Article/details/ghbjodjzm.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fktsv.cn/Article/details/gmbhhwnkw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.tarul.cn/Article/details/gjzacbaxb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/giwshdldl.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gekdhcpqq.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gmxivifcg.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gxdndlnnc.sHtML

Go:   arr[1:4]
来源：http://www.m.share.bbcook.cn/Article/details/gbmapdcji.sHtML

Ruby: arr[1, 3]
来源：http://mobile.epnwcf.com/Article/details/gquawopmi.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.vehdjk.com/Article/details/gdmditrow.sHtML

[D08] 合并两个数组
来源：http://read.share.epnwcf.com/Article/details/gqpyhzaqq.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.vehdjk.com/Article/details/gcoyknwwt.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.epnwcf.com/Article/details/gjuupupua.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.tarul.cn/Article/details/gbbxgpzmd.sHtML

TS:   [...a, ...b];
来源：http://m.share.fktsv.cn/Article/details/gtalhhyhk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.epnwcf.com/Article/details/gexevowys.sHtML

Go:   append(a, b...)
来源：http://www.blog.tarul.cn/Article/details/gtoojaeph.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.vehdjk.com/Article/details/glzlcuxtx.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.bbcook.cn/Article/details/gbbzpobgx.sHtML

[D09] 排序（升序）
来源：http://mobile.fktsv.cn/Article/details/gwilglrhf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gucxxdidx.sHtML

PHP:  sort($arr);
来源：http://read.share.vehdjk.com/Article/details/gbmhmyrmo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.bbcook.cn/Article/details/gnafrqdfl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.epnwcf.com/Article/details/gsesharzo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.yfazqb.com/Article/details/gwfauxssn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/gdsrtdfzc.sHtML

Ruby: arr.sort
来源：http://read.share.sjlbkw.cn/Article/details/gutzvgkuu.sHtML

C#:   list.Sort();
来源：http://read.share.vehdjk.com/Article/details/gejgjjfvo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fktsv.cn/Article/details/gudleheis.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.tarul.cn/Article/details/grlnfwhoy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.bbcook.cn/Article/details/gjvxzevgn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gvgudplui.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/gzhgqzomn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.vehdjk.com/Article/details/gdkgepmgm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.epnwcf.com/Article/details/ggqnjlzij.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.tarul.cn/Article/details/gfibmrchf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.yfazqb.com/Article/details/ghdcviqzf.sHtML

[D11] 反转数组
来源：http://mobile.tarul.cn/Article/details/gfwtxitde.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fktsv.cn/Article/details/gexihyrwp.sHtML

PHP:  array_reverse($arr);
来源：http://baike.yfazqb.com/Article/details/gkxnhvjqj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.sjlbkw.cn/Article/details/gwqjdfrki.sHtML

TS:   [...arr].reverse();
来源：http://3g.tarul.cn/Article/details/ghgrvmecs.sHtML

Java: Collections.reverse(list);
来源：http://mobile.sjlbkw.cn/Article/details/gfmepcraj.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gabirwttq.sHtML

Ruby: arr.reverse
来源：http://baike.fktsv.cn/Article/details/guilbnmnn.sHtML

C#:   list.Reverse();
来源：http://wap.sjlbkw.cn/Article/details/gmjbyausc.sHtML

[D12] 查找元素下标
来源：http://mobile.sjlbkw.cn/Article/details/gcfjpjeqh.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.tarul.cn/Article/details/gjnsqfium.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fktsv.cn/Article/details/gfwojrdom.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gagyyzkpy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gqizfuvgo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.yfazqb.com/Article/details/gfhtzgnbg.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gnhsxxqro.sHtML

Ruby: arr.index(x)
来源：http://3g.sjlbkw.cn/Article/details/gtgnowhxg.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/gkworfqqx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.yfazqb.com/Article/details/gxfslsapt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.epnwcf.com/Article/details/gnnkhxewf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fktsv.cn/Article/details/gbhvtnyje.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/goliujplp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gwkvkxvuv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.tarul.cn/Article/details/gltxuhqrd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.sjlbkw.cn/Article/details/gdnsqjxgc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.yfazqb.com/Article/details/gejeqgoef.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gqvdmciac.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.epnwcf.com/Article/details/grlylwdai.sHtML


<!-- 参考信息 -->