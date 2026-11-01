代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gkvmzlebn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.vehdjk.com/Article/details/gkoatpnci.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.sjlbkw.cn/Article/details/gkwpjxtae.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.bbcook.cn/Article/details/gpuaaglrl.sHtML

[B13] 判断是否为数字
来源：http://wap.tarul.cn/Article/details/gaulxppkk.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fktsv.cn/Article/details/gdhbpcsbp.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fktsv.cn/Article/details/gltnusynl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.tarul.cn/Article/details/gwqfbevhe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gcbmgsrzr.sHtML

Java: x instanceof Number
来源：http://baike.bbcook.cn/Article/details/gonblutyw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.tarul.cn/Article/details/gdbetmdiz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.vehdjk.com/Article/details/gnnrexmqa.sHtML

C#:   x is int or double or decimal
来源：http://wap.yfazqb.com/Article/details/gqutdmdmc.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.tarul.cn/Article/details/gpbmchoao.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.tarul.cn/Article/details/gcetecmxn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.bbcook.cn/Article/details/gtxwpljlx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gsyvdjekt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fktsv.cn/Article/details/gghybmkxm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.tarul.cn/Article/details/gkfhliqtr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fktsv.cn/Article/details/gekevejve.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.yfazqb.com/Article/details/gdmwpzcab.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gmkaudqzy.sHtML

[B15] 布尔运算与取反
来源：http://m.share.yfazqb.com/Article/details/gsrsvbejy.sHtML

Py:   a and b or not c
来源：http://baike.fktsv.cn/Article/details/glyetzxuc.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.vehdjk.com/Article/details/ggstvfyrf.sHtML

JS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gntemlsab.sHtML

TS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/glhcduyiz.sHtML

Java: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gqowspaue.sHtML

Go:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gmjudxbbi.sHtML

Ruby: a && b || !c
来源：http://3g.tarul.cn/Article/details/gujmulxjd.sHtML

C#:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gyxvfzekw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fktsv.cn/Article/details/gcqxtmhxe.sHtML

Py:   if not data: return
来源：http://wap.epnwcf.com/Article/details/gwoerffaz.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/gdwzlnyns.sHtML

JS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gyifacapx.sHtML

TS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gceeetahb.sHtML

Java: if (data == null) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gndvrycup.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fktsv.cn/Article/details/gtzhslfro.sHtML

Ruby: return if data.nil?
来源：http://wap.yfazqb.com/Article/details/gubuyavhl.sHtML

C#:   if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/gyvwpvmyx.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqudnmayv.sHtML

C. 函数与作用域
来源：http://www.share.vehdjk.com/Article/details/gvmquwjji.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gjslnkaha.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gxljgghfo.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.tarul.cn/Article/details/gtlvglpps.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gufrqaobs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/glktinaqe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gaznjqkzb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gtwaduyae.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gfdduhulf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.sjlbkw.cn/Article/details/gdkacwzsv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/guiftyuyd.sHtML

[C02] 默认参数
来源：http://read.share.tarul.cn/Article/details/gnicvaktj.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.epnwcf.com/Article/details/ghprhakmf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.bbcook.cn/Article/details/gvniawlym.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.epnwcf.com/Article/details/gfkvputtj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.epnwcf.com/Article/details/gwpdvspss.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fktsv.cn/Article/details/gcvtbpwyg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.epnwcf.com/Article/details/gmoijsvxh.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.bbcook.cn/Article/details/gyqvhmaxh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.vehdjk.com/Article/details/gpkpvwakq.sHtML

[C03] 可变参数
来源：http://baike.tarul.cn/Article/details/girriccgf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fktsv.cn/Article/details/gkxblsjct.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.vehdjk.com/Article/details/ghmbzvcoj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.vehdjk.com/Article/details/gpqasvwxa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.vehdjk.com/Article/details/gdzspemzv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.sjlbkw.cn/Article/details/giwockemj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.yfazqb.com/Article/details/gtxnbygxv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.vehdjk.com/Article/details/gjtycxmps.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.yfazqb.com/Article/details/gjvfyrqdp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.epnwcf.com/Article/details/gayifwmos.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.vehdjk.com/Article/details/gcugpesyp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gzrxozgrw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.bbcook.cn/Article/details/gldiygzjc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.sjlbkw.cn/Article/details/gmgysziru.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fktsv.cn/Article/details/guoiolanx.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.tarul.cn/Article/details/gnzlslzfj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gkmjkofus.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/gtaelnggk.sHtML

[C05] 返回多个值
来源：http://baike.vehdjk.com/Article/details/gqhzhkmag.sHtML

Py:   return a, b
来源：http://m.share.bbcook.cn/Article/details/ggqnpbguy.sHtML

PHP:  return [$a, $b];
来源：http://3g.fktsv.cn/Article/details/gpewqatxn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.vehdjk.com/Article/details/gklutpvxv.sHtML

TS:   return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gegvhybpf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.bbcook.cn/Article/details/gwxlfjrio.sHtML

Go:   return a, b
来源：http://3g.epnwcf.com/Article/details/gyrclypmi.sHtML

Ruby: return a, b
来源：http://wap.vehdjk.com/Article/details/gniboxsrh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.sjlbkw.cn/Article/details/gmpfjsmpa.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.yfazqb.com/Article/details/gpfbzofsa.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.vehdjk.com/Article/details/gogllysqj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gycxpphip.sHtML

JS:   const square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/guamnnvsl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gvbzeparc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gxumkaqbw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.vehdjk.com/Article/details/gpdzwhmjf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.tarul.cn/Article/details/gqplqtpyl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gwhjrhmdp.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.sjlbkw.cn/Article/details/gsrvzbpfz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.bbcook.cn/Article/details/gobbmishn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.bbcook.cn/Article/details/gchisezdq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.tarul.cn/Article/details/gkjdcvsmm.sHtML

TS:   arr.map(String)
来源：http://3g.fktsv.cn/Article/details/ghwrzmzor.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbofwlcsw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.bbcook.cn/Article/details/ggyjophuq.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.bbcook.cn/Article/details/gcpfelymm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.sjlbkw.cn/Article/details/gzszeyttm.sHtML

[C08] 闭包
来源：http://blog.tarul.cn/Article/details/gleitjstr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.yfazqb.com/Article/details/gttpwnbic.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.sjlbkw.cn/Article/details/gknfohukk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gsgisipaw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gnbrjyxvr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.sjlbkw.cn/Article/details/gmtqzttht.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fktsv.cn/Article/details/grqjnytoh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.sjlbkw.cn/Article/details/gsysdcqvf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gkufhhcuc.sHtML

[C09] 递归
来源：http://wap.tarul.cn/Article/details/gponkkgnj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gpqmswjxb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.tarul.cn/Article/details/gqzizexpb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.yfazqb.com/Article/details/glxqhgriw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gwgmigeso.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.yfazqb.com/Article/details/glfxdxlpg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.vehdjk.com/Article/details/gqzgiiauj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/gymxmpelk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.epnwcf.com/Article/details/ghrmioocw.sHtML

[C10] 变量作用域
来源：http://read.share.bbcook.cn/Article/details/gbvdatplv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.sjlbkw.cn/Article/details/gzgycnqfv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fktsv.cn/Article/details/gnbsbefvw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gzuybmhoz.sHtML

TS:   同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gdgdzbwxs.sHtML

Java: 方法内为块级作用域
来源：http://read.share.bbcook.cn/Article/details/ghviebmdu.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gpsvebiea.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.vehdjk.com/Article/details/gwayussiy.sHtML

C#:   块级作用域
来源：http://read.share.bbcook.cn/Article/details/guralpctf.sHtML

[C11] 模块导入与导出
来源：http://3g.vehdjk.com/Article/details/gwynzckxs.sHtML

Py:   from module import func
来源：http://m.share.bbcook.cn/Article/details/gtyzwptqu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.vehdjk.com/Article/details/gohejabsq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/geqmkobko.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.yfazqb.com/Article/details/gdhljouoi.sHtML

Java: import java.util.List;
来源：http://blog.sjlbkw.cn/Article/details/gdvdagrif.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.bbcook.cn/Article/details/glscwlirj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.tarul.cn/Article/details/ghlrufjta.sHtML

C#:   using System.Text;
来源：http://read.share.yfazqb.com/Article/details/gxrxlctcs.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.sjlbkw.cn/Article/details/gulplfrfp.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.yfazqb.com/Article/details/ggbhomoof.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.sjlbkw.cn/Article/details/ggtrnbnld.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.tarul.cn/Article/details/gmsferlli.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/gfctpyqgx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.vehdjk.com/Article/details/gjazfaokf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.bbcook.cn/Article/details/gmuhywilj.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.vehdjk.com/Article/details/gulsclvop.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.bbcook.cn/Article/details/gdzmukfqm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.vehdjk.com/Article/details/ggfibumzz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.epnwcf.com/Article/details/gcqsmwxay.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gucflrwei.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.tarul.cn/Article/details/gdppvajkj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gsdflfuhk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gpjiakghv.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/gnjderzps.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.vehdjk.com/Article/details/gxycgczsq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.vehdjk.com/Article/details/gjajjizeb.sHtML

[C14] 泛型函数
来源：http://read.share.vehdjk.com/Article/details/gkyhtfbbp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.yfazqb.com/Article/details/gempfsqda.sHtML

PHP:  // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/giknubodn.sHtML

JS:   // 无泛型
来源：http://baike.tarul.cn/Article/details/gmpgtpgns.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.epnwcf.com/Article/details/gnglgvosu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.tarul.cn/Article/details/gngqlfdjm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.bbcook.cn/Article/details/gunoxvpnc.sHtML

Ruby: # 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gwkzjbafk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.sjlbkw.cn/Article/details/gwodmiokh.sHtML

[C15] 解构 / 展开参数
来源：http://wap.sjlbkw.cn/Article/details/gscquadhj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fktsv.cn/Article/details/gbnhsuecz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.sjlbkw.cn/Article/details/garofjsqp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/gfuuxqunv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.vehdjk.com/Article/details/ggxsklbbg.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/gmtmeiujk.sHtML

Go:   // 无解构
来源：http://wap.vehdjk.com/Article/details/gqpqizwok.sHtML

Ruby: a, b = pair
来源：http://3g.epnwcf.com/Article/details/gsnmmufxb.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.sjlbkw.cn/Article/details/gjaycybxs.sHtML

[C16] 函数 / 方法重载
来源：http://baike.tarul.cn/Article/details/gettujydo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.sjlbkw.cn/Article/details/gygimjkxz.sHtML

PHP:  // 无重载
来源：http://3g.bbcook.cn/Article/details/gmtrzdxuq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.yfazqb.com/Article/details/gnpiadrzw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.bbcook.cn/Article/details/gkvkpuecq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.epnwcf.com/Article/details/gmlzqnwut.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.epnwcf.com/Article/details/gnxbgkzci.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.sjlbkw.cn/Article/details/gzpyqubgz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.vehdjk.com/Article/details/gjpambafk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gjuwrawbj.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fktsv.cn/Article/details/gpnddzfcr.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gigetlnug.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.vehdjk.com/Article/details/gvqlzhwji.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.vehdjk.com/Article/details/gdyueqcor.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fktsv.cn/Article/details/ggfulisvi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.tarul.cn/Article/details/gyfktklji.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.epnwcf.com/Article/details/gbbwhfkdu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.tarul.cn/Article/details/gvwgpanzx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.bbcook.cn/Article/details/gnyqcyvxl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.epnwcf.com/Article/details/gaqjnjeli.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.tarul.cn/Article/details/gzppfercj.sHtML

[D02] 追加元素到末尾
来源：http://mobile.tarul.cn/Article/details/gptbtgflx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.yfazqb.com/Article/details/gvwbdwwjd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fktsv.cn/Article/details/gcahhhmhv.sHtML

JS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/gdwotselb.sHtML

TS:   arr.push(4);
来源：http://read.share.yfazqb.com/Article/details/gcxpxanxz.sHtML

Java: list.add(4);
来源：http://baike.sjlbkw.cn/Article/details/gcrbfmgtb.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.yfazqb.com/Article/details/ghldkgsac.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.tarul.cn/Article/details/geqbscuer.sHtML

C#:   list.Add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gnxebvwgm.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.tarul.cn/Article/details/gvpuyakpo.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fktsv.cn/Article/details/gmghsqewv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.tarul.cn/Article/details/gvfvkecvk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.epnwcf.com/Article/details/glzcpmpau.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.sjlbkw.cn/Article/details/givpmjffa.sHtML

Java: list.add(0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/ggglibrde.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fktsv.cn/Article/details/glnkulcui.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.vehdjk.com/Article/details/guzluwdyz.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.epnwcf.com/Article/details/gkdizokug.sHtML

[D04] 删除元素
来源：http://www.m.share.sjlbkw.cn/Article/details/geixjprct.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.bbcook.cn/Article/details/gxmnmddpn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.bbcook.cn/Article/details/gbmcaqmcr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.tarul.cn/Article/details/ghwkldsns.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.yfazqb.com/Article/details/gdmzdqghx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.yfazqb.com/Article/details/gbfuqqill.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.epnwcf.com/Article/details/gdmifxypp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fktsv.cn/Article/details/gxalkkdpt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.bbcook.cn/Article/details/gzexejryt.sHtML

[D05] 访问与修改元素
来源：http://www.share.bbcook.cn/Article/details/gqjsyzpwd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gmlkzjicw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gymfheylt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gvybmvhvh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.sjlbkw.cn/Article/details/gdvxencxd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.bbcook.cn/Article/details/gdkcfeopn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gpbqcbcww.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/ghvjgrqgu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gyrluluwo.sHtML

[D06] 数组长度
来源：http://blog.tarul.cn/Article/details/ggcnmzdvb.sHtML

Py:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/giabkling.sHtML

PHP:  count($arr);
来源：http://read.share.vehdjk.com/Article/details/gxzdkoduf.sHtML

JS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gimfesvkk.sHtML

TS:   arr.length
来源：http://www.blog.fktsv.cn/Article/details/gplfpiwjq.sHtML

Java: list.size();
来源：http://mobile.epnwcf.com/Article/details/gavtenlyw.sHtML

Go:   len(arr)
来源：http://3g.fktsv.cn/Article/details/gdpkjrgyv.sHtML

Ruby: arr.length; arr.size
来源：http://blog.vehdjk.com/Article/details/gehggoeqi.sHtML

C#:   list.Count;
来源：http://baike.tarul.cn/Article/details/gzszgfbdb.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.vehdjk.com/Article/details/gppmwflqo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.bbcook.cn/Article/details/gdzhdkmvp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.bbcook.cn/Article/details/gzkuiwzdc.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fktsv.cn/Article/details/glvqqmgfy.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.bbcook.cn/Article/details/gufpcwnan.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gmegwycch.sHtML

Go:   arr[1:4]
来源：http://read.share.vehdjk.com/Article/details/gqsqybtlv.sHtML

Ruby: arr[1, 3]
来源：http://www.share.yfazqb.com/Article/details/gmzpcaive.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.sjlbkw.cn/Article/details/gkrgonnib.sHtML

[D08] 合并两个数组
来源：http://baike.vehdjk.com/Article/details/gbckbswwr.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.bbcook.cn/Article/details/gfoxnrrun.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.bbcook.cn/Article/details/gennqlalv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.sjlbkw.cn/Article/details/gbyaylhha.sHtML

TS:   [...a, ...b];
来源：http://www.share.yfazqb.com/Article/details/grvululsb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.tarul.cn/Article/details/glojianzc.sHtML

Go:   append(a, b...)
来源：http://wap.sjlbkw.cn/Article/details/gagdvtesu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.vehdjk.com/Article/details/guwnucmfv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gjptnzfyk.sHtML

[D09] 排序（升序）
来源：http://3g.yfazqb.com/Article/details/gvbplmxen.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.vehdjk.com/Article/details/gyttmrbtw.sHtML

PHP:  sort($arr);
来源：http://wap.epnwcf.com/Article/details/glverpyir.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.vehdjk.com/Article/details/gwsnwfbqz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.sjlbkw.cn/Article/details/grszgbxbf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.vehdjk.com/Article/details/gulmrfgzo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gfnahkhtc.sHtML

Ruby: arr.sort
来源：http://m.share.vehdjk.com/Article/details/gechfgeth.sHtML

C#:   list.Sort();
来源：http://baike.bbcook.cn/Article/details/gkdefalug.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.epnwcf.com/Article/details/gjksjhevd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.yfazqb.com/Article/details/gjjagnzbj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.bbcook.cn/Article/details/grtmadeuc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gqpywzhqs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.epnwcf.com/Article/details/gcfldsyxf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.bbcook.cn/Article/details/gcpbpkoyx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.bbcook.cn/Article/details/geoxrpixu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.tarul.cn/Article/details/govjvglsf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.sjlbkw.cn/Article/details/gdsedyaaf.sHtML

[D11] 反转数组
来源：http://wap.yfazqb.com/Article/details/ggdiypfwb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.vehdjk.com/Article/details/ggrruvkmn.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gryanbosq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.yfazqb.com/Article/details/gwczxzfig.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.vehdjk.com/Article/details/gfmzkwsur.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.vehdjk.com/Article/details/gioeqyzgc.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.bbcook.cn/Article/details/gtcdlrvbi.sHtML

Ruby: arr.reverse
来源：http://baike.epnwcf.com/Article/details/gourojgkt.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fktsv.cn/Article/details/gvrrcrhte.sHtML

[D12] 查找元素下标
来源：http://wap.vehdjk.com/Article/details/ginalhjky.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.vehdjk.com/Article/details/gdwedvduo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gsqnayrjl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gfpsaclhz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fktsv.cn/Article/details/godufkdba.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.tarul.cn/Article/details/gprcvpkvb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gahuojrmc.sHtML

Ruby: arr.index(x)
来源：http://www.blog.vehdjk.com/Article/details/gktmjfooq.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fktsv.cn/Article/details/gkgqupgna.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.sjlbkw.cn/Article/details/gkkpseaco.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gwbjftura.sHtML


<!-- 参考信息 -->