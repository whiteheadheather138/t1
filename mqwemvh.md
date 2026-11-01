代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gplnsbzqx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.bbcook.cn/Article/details/gnposwbmd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.tarul.cn/Article/details/gtxhaxhxv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.vehdjk.com/Article/details/gbosegbje.sHtML

[B13] 判断是否为数字
来源：http://m.share.bbcook.cn/Article/details/gmjbkfymz.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fktsv.cn/Article/details/gwgnubynx.sHtML

PHP:  is_numeric($x)
来源：http://www.share.vehdjk.com/Article/details/gnlgsunow.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.yfazqb.com/Article/details/gctjejbat.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.yfazqb.com/Article/details/gzomyjhln.sHtML

Java: x instanceof Number
来源：http://www.m.share.bbcook.cn/Article/details/gkfmekfac.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fktsv.cn/Article/details/gonwqgnqg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fktsv.cn/Article/details/gzleybdli.sHtML

C#:   x is int or double or decimal
来源：http://3g.vehdjk.com/Article/details/gnhncdmln.sHtML

[B14] 判断值是否在集合内
来源：http://baike.sjlbkw.cn/Article/details/gqamsazgq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fktsv.cn/Article/details/ghmsfsugq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.bbcook.cn/Article/details/gummjdvqv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gyikgkdma.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/gdxkdxpgx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.bbcook.cn/Article/details/gkywutvcn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.sjlbkw.cn/Article/details/grkcszhje.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.tarul.cn/Article/details/gizyqnovl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gxejiwzua.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmnvucls.sHtML

Py:   a and b or not c
来源：http://3g.bbcook.cn/Article/details/gskddytvj.sHtML

PHP:  $a && $b || !$c
来源：http://blog.sjlbkw.cn/Article/details/ghcwlxdci.sHtML

JS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gqxdukwqf.sHtML

TS:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gwzqhujom.sHtML

Java: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gmqdqvgst.sHtML

Go:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gstavgneb.sHtML

Ruby: a && b || !c
来源：http://mobile.tarul.cn/Article/details/gjwnybngs.sHtML

C#:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gqsnegtoh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.bbcook.cn/Article/details/gxipggdkt.sHtML

Py:   if not data: return
来源：http://m.share.vehdjk.com/Article/details/gemhxsvif.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.yfazqb.com/Article/details/gisyuihjd.sHtML

JS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gdufryzpp.sHtML

TS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gqmprtnhj.sHtML

Java: if (data == null) return;
来源：http://baike.sjlbkw.cn/Article/details/gftmcxgzg.sHtML

Go:   if data == nil { return }
来源：http://blog.vehdjk.com/Article/details/gbipsbbxh.sHtML

Ruby: return if data.nil?
来源：http://www.blog.vehdjk.com/Article/details/gixqlfssa.sHtML

C#:   if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/gisuwsilf.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxzbbkeex.sHtML

C. 函数与作用域
来源：http://3g.vehdjk.com/Article/details/gngtjezkt.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxpvkluol.sHtML

[C01] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gxbvtkbkd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.tarul.cn/Article/details/ggkmoskxc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gjpjrovao.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gyxtmoobv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gytmsetzx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaftwqpcw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.epnwcf.com/Article/details/guolweohw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.epnwcf.com/Article/details/gvmphvedm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gtajnxwlp.sHtML

[C02] 默认参数
来源：http://www.share.fktsv.cn/Article/details/gviysnojn.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.vehdjk.com/Article/details/gnmhepsir.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.bbcook.cn/Article/details/gjixjxtzv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfrxfbemb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gxysntgqs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.yfazqb.com/Article/details/gdzbfbapg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.epnwcf.com/Article/details/gnvjeazay.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fktsv.cn/Article/details/gdkknfyyi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.vehdjk.com/Article/details/gcifeigqo.sHtML

[C03] 可变参数
来源：http://3g.bbcook.cn/Article/details/gluapuyxw.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.tarul.cn/Article/details/gyzajykey.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.bbcook.cn/Article/details/gdwwwitgk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gqkvrcauq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/gdkeydinv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.bbcook.cn/Article/details/gnkzsqfyk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.epnwcf.com/Article/details/ganntzocv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.vehdjk.com/Article/details/gzuhyjxcs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.epnwcf.com/Article/details/grjsfyarj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.tarul.cn/Article/details/glqdiymum.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.bbcook.cn/Article/details/gqeoolkgh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.tarul.cn/Article/details/gzhgzycui.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/gdfxrfsga.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/ghoxdcoar.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.sjlbkw.cn/Article/details/grqowtjpf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/gftwryapb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/gahytkgcq.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gpiyopzkd.sHtML

[C05] 返回多个值
来源：http://www.share.yfazqb.com/Article/details/gwkuoczlr.sHtML

Py:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gwrfrapty.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxxfmzhk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/gmfudgvih.sHtML

TS:   return { a, b };
来源：http://blog.bbcook.cn/Article/details/gsqektwgz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.bbcook.cn/Article/details/gasrthxeu.sHtML

Go:   return a, b
来源：http://baike.tarul.cn/Article/details/gquztrizu.sHtML

Ruby: return a, b
来源：http://mobile.fktsv.cn/Article/details/grcjbrkxv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.tarul.cn/Article/details/gfjlzsiam.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.vehdjk.com/Article/details/ggzdgkbdn.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.vehdjk.com/Article/details/gemvnfhao.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.tarul.cn/Article/details/grwtpygmr.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fktsv.cn/Article/details/gaxyzaqgh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwazhwdr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.vehdjk.com/Article/details/gyrjgdwka.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.vehdjk.com/Article/details/guesjodem.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gwlclymrf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gaarowmfp.sHtML

[C07] 把函数作为参数传入
来源：http://baike.epnwcf.com/Article/details/gsjczcjpi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.sjlbkw.cn/Article/details/gnqoeyvar.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gureifkse.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.yfazqb.com/Article/details/gtsqqastv.sHtML

TS:   arr.map(String)
来源：http://3g.sjlbkw.cn/Article/details/gfhphxkro.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fktsv.cn/Article/details/gpaurcaum.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fktsv.cn/Article/details/gxsupewoq.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.sjlbkw.cn/Article/details/gyqkkxxdl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.vehdjk.com/Article/details/gizouksik.sHtML

[C08] 闭包
来源：http://baike.yfazqb.com/Article/details/ghbhdaovp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fktsv.cn/Article/details/gwvkrcbrp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.tarul.cn/Article/details/grptrvzjx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gfrzkkszn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gmeseyfdy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.vehdjk.com/Article/details/glnruhuzn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.epnwcf.com/Article/details/gjusjbokl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.sjlbkw.cn/Article/details/gvkmfzorm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gjwslzkcc.sHtML

[C09] 递归
来源：http://mobile.yfazqb.com/Article/details/gqqoxoozi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/gqfsiyqad.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fktsv.cn/Article/details/gsuhavzbt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/ghajbaayh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.sjlbkw.cn/Article/details/gcohldnbz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.vehdjk.com/Article/details/gcuxytlwv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.tarul.cn/Article/details/gburxqfem.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/ghxgispue.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.tarul.cn/Article/details/gifzqcxon.sHtML

[C10] 变量作用域
来源：http://m.share.sjlbkw.cn/Article/details/gmveqycpp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fktsv.cn/Article/details/glwgeslgd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.yfazqb.com/Article/details/gcnffzuzw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.bbcook.cn/Article/details/gxpepngio.sHtML

TS:   同 JS
来源：http://m.share.sjlbkw.cn/Article/details/giucsyvjd.sHtML

Java: 方法内为块级作用域
来源：http://blog.fktsv.cn/Article/details/gxtejeech.sHtML

Go:   花括号块级作用域
来源：http://mobile.fktsv.cn/Article/details/gwvpjxvny.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/ghjicdvrf.sHtML

C#:   块级作用域
来源：http://mobile.vehdjk.com/Article/details/gdhqdlpsv.sHtML

[C11] 模块导入与导出
来源：http://read.share.sjlbkw.cn/Article/details/gvitmndza.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gbfpgwmqp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.vehdjk.com/Article/details/gjapwxyuw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/goyeemipv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fktsv.cn/Article/details/gspyirnsf.sHtML

Java: import java.util.List;
来源：http://www.blog.tarul.cn/Article/details/goaxkwhdi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.sjlbkw.cn/Article/details/gsndcvwyr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.bbcook.cn/Article/details/gsnincnew.sHtML

C#:   using System.Text;
来源：http://baike.sjlbkw.cn/Article/details/gtldbhhdl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.sjlbkw.cn/Article/details/gyiwcqeow.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.sjlbkw.cn/Article/details/gcjjjcdzw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.bbcook.cn/Article/details/goawvjuht.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fktsv.cn/Article/details/gvxunabis.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.vehdjk.com/Article/details/gbjjbykdi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fktsv.cn/Article/details/gfprjjqnv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.yfazqb.com/Article/details/gdvbcjobw.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.sjlbkw.cn/Article/details/gxzprrcjy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/guuytvkzs.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.yfazqb.com/Article/details/gjgdpodhv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.vehdjk.com/Article/details/gwzznhbai.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/ggcllpnkk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.sjlbkw.cn/Article/details/gsoajxgdc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gscjmeccm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/ghfygclxq.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.epnwcf.com/Article/details/gmzzxdxgr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.epnwcf.com/Article/details/gvptkwdsk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyugewgvo.sHtML

[C14] 泛型函数
来源：http://blog.epnwcf.com/Article/details/gtbllsysj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.sjlbkw.cn/Article/details/glgsucyvs.sHtML

PHP:  // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/govlrfxov.sHtML

JS:   // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gfywvfwgv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.tarul.cn/Article/details/gzmsxnkwa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.tarul.cn/Article/details/gcupikxko.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.bbcook.cn/Article/details/gpvyfzodr.sHtML

Ruby: # 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gefvyjfgn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.bbcook.cn/Article/details/grwpvcobs.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fktsv.cn/Article/details/ggjnrupfs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.sjlbkw.cn/Article/details/gtawykatj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.vehdjk.com/Article/details/gofakvmqj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/gstshchus.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.yfazqb.com/Article/details/gypyzjxav.sHtML

Java: // 无解构
来源：http://www.blog.tarul.cn/Article/details/gwmzhttht.sHtML

Go:   // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/ghqytngsb.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/glnpptahd.sHtML

C#:   var (a, b) = pair;
来源：http://3g.tarul.cn/Article/details/grvhgkiqk.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fktsv.cn/Article/details/girnlnnak.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.tarul.cn/Article/details/guvzwcdnl.sHtML

PHP:  // 无重载
来源：http://read.share.fktsv.cn/Article/details/grjgqpnoq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.vehdjk.com/Article/details/gqixubwxt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.tarul.cn/Article/details/gtvfzquud.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.bbcook.cn/Article/details/gqnwjbjqj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.sjlbkw.cn/Article/details/gxiocvtar.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.tarul.cn/Article/details/gsbtmbqpw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.bbcook.cn/Article/details/gthikhvcj.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gnqukwkwm.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fktsv.cn/Article/details/gvwzpjsdt.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gkvclytmg.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.vehdjk.com/Article/details/ghrrcfoju.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.epnwcf.com/Article/details/ghooubvva.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.tarul.cn/Article/details/gvereitfe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.bbcook.cn/Article/details/gtutqptbq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fktsv.cn/Article/details/gtgudkpdo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/gsuzuodqz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.vehdjk.com/Article/details/giahpwohr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.vehdjk.com/Article/details/gkzgtgfrp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.tarul.cn/Article/details/gfbtxzqhk.sHtML

[D02] 追加元素到末尾
来源：http://mobile.sjlbkw.cn/Article/details/gbwshvopn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.bbcook.cn/Article/details/gvngzqmkz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fktsv.cn/Article/details/gsxlxjgwx.sHtML

JS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/ghgdqrwuu.sHtML

TS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gkbhxfdos.sHtML

Java: list.add(4);
来源：http://blog.vehdjk.com/Article/details/gnnliygim.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fktsv.cn/Article/details/gxosdrfcu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.tarul.cn/Article/details/goyoenssp.sHtML

C#:   list.Add(4);
来源：http://wap.epnwcf.com/Article/details/gqzvmgxxp.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.sjlbkw.cn/Article/details/gauigypoi.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/glutvaugl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fktsv.cn/Article/details/gomapejub.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fktsv.cn/Article/details/ghojabxjv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.vehdjk.com/Article/details/glpdghlsi.sHtML

Java: list.add(0, 0);
来源：http://baike.epnwcf.com/Article/details/gmhyoapbr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.epnwcf.com/Article/details/gedhnfqcz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.epnwcf.com/Article/details/geiirvszt.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gkavehbyq.sHtML

[D04] 删除元素
来源：http://3g.fktsv.cn/Article/details/gklumijdg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.vehdjk.com/Article/details/gkmamncpj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.tarul.cn/Article/details/gjpwiuwxi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.yfazqb.com/Article/details/gkfggvvjr.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.yfazqb.com/Article/details/gdzstkvbk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.yfazqb.com/Article/details/gykyqmhvb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.sjlbkw.cn/Article/details/gtiztulen.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fktsv.cn/Article/details/gzuqnnbzt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fktsv.cn/Article/details/gjvzqsjpn.sHtML

[D05] 访问与修改元素
来源：http://blog.epnwcf.com/Article/details/gxkayafje.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gzqxgwaih.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gygoedjuu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/getiyqkwa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.epnwcf.com/Article/details/gazjqencj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.yfazqb.com/Article/details/gyvvlwtiu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gvydybfjp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gzsvsdlhq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gspytlfcq.sHtML

[D06] 数组长度
来源：http://3g.epnwcf.com/Article/details/gfxcwkaqb.sHtML

Py:   len(arr)
来源：http://read.share.vehdjk.com/Article/details/gzyappuyq.sHtML

PHP:  count($arr);
来源：http://wap.bbcook.cn/Article/details/gfhqaiofh.sHtML

JS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/gkrtvzqdz.sHtML

TS:   arr.length
来源：http://blog.yfazqb.com/Article/details/goclkamax.sHtML

Java: list.size();
来源：http://www.blog.sjlbkw.cn/Article/details/gcaxhpsfx.sHtML

Go:   len(arr)
来源：http://www.share.epnwcf.com/Article/details/gqnluavdx.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.bbcook.cn/Article/details/gdclfwluz.sHtML

C#:   list.Count;
来源：http://baike.epnwcf.com/Article/details/giigoulce.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gobuxszqf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fktsv.cn/Article/details/gkbptfbhb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.epnwcf.com/Article/details/gcthqconw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gyxazyxgi.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gcotrmihs.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gkrfxluyf.sHtML

Go:   arr[1:4]
来源：http://mobile.sjlbkw.cn/Article/details/gtgtyainx.sHtML

Ruby: arr[1, 3]
来源：http://blog.epnwcf.com/Article/details/gplmjmcju.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.tarul.cn/Article/details/gsrazviad.sHtML

[D08] 合并两个数组
来源：http://blog.fktsv.cn/Article/details/gzqoqtlkf.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.yfazqb.com/Article/details/garlvirdk.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fktsv.cn/Article/details/gbsxkjena.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.bbcook.cn/Article/details/gsupdtjxr.sHtML

TS:   [...a, ...b];
来源：http://wap.epnwcf.com/Article/details/gmlzgezlh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gsgrpvkxy.sHtML

Go:   append(a, b...)
来源：http://m.share.tarul.cn/Article/details/gqailarmg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.yfazqb.com/Article/details/gjeulwwgj.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gswelolii.sHtML

[D09] 排序（升序）
来源：http://m.share.vehdjk.com/Article/details/gorccgdqp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gezmifpex.sHtML

PHP:  sort($arr);
来源：http://www.share.fktsv.cn/Article/details/gihlwnint.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.tarul.cn/Article/details/gtjfhxbcg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.epnwcf.com/Article/details/gfmlramep.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fktsv.cn/Article/details/gqgcvmgem.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gcpyzsqax.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gxhdjjqiw.sHtML

C#:   list.Sort();
来源：http://blog.yfazqb.com/Article/details/glhwznilc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.tarul.cn/Article/details/gieyhuhhr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.bbcook.cn/Article/details/gedlkjutq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/getspckvz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.epnwcf.com/Article/details/gbggvcjzh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/gijauposs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.epnwcf.com/Article/details/gyhcxuxhr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.yfazqb.com/Article/details/gbinljcur.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.sjlbkw.cn/Article/details/glkukovbe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.epnwcf.com/Article/details/gogalblbo.sHtML

[D11] 反转数组
来源：http://3g.sjlbkw.cn/Article/details/ghtfjdsrn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.epnwcf.com/Article/details/gzltfshux.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/guldsglfg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.tarul.cn/Article/details/gjtkwbzog.sHtML

TS:   [...arr].reverse();
来源：http://read.share.bbcook.cn/Article/details/gnqzysucj.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.epnwcf.com/Article/details/glwedtako.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.yfazqb.com/Article/details/gvqteqclz.sHtML

Ruby: arr.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gfowjfdjk.sHtML

C#:   list.Reverse();
来源：http://wap.bbcook.cn/Article/details/gygwwxvmw.sHtML

[D12] 查找元素下标
来源：http://m.share.sjlbkw.cn/Article/details/gypfzketj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.yfazqb.com/Article/details/gkbpafngo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gbwfiqhog.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/grmnvcihi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/gpjfgwcsf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.bbcook.cn/Article/details/gggajwohy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gosjorskc.sHtML

Ruby: arr.index(x)
来源：http://read.share.epnwcf.com/Article/details/gjfliuuey.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.epnwcf.com/Article/details/gdnufgghf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.epnwcf.com/Article/details/gehltythn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.vehdjk.com/Article/details/goubdvmgh.sHtML


<!-- 参考信息 -->