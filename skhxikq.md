代发 wailian999

C#:   x is int or double or decimal
来源：http://mobile.tarul.cn/Article/details/gvbedityc.sHtML

[B14] 判断值是否在集合内
来源：http://baike.bbcook.cn/Article/details/gujkimzfi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.vehdjk.com/Article/details/gkynapkvd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fktsv.cn/Article/details/gsxjgfygh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gcouqoagf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gfpilefet.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.tarul.cn/Article/details/gczmngott.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.tarul.cn/Article/details/gzcgiguij.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.vehdjk.com/Article/details/gjpquuwjy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/gsxapjmgl.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.sjlbkw.cn/Article/details/gobxbdkyz.sHtML

Py:   a and b or not c
来源：http://blog.bbcook.cn/Article/details/gwetfekmg.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.sjlbkw.cn/Article/details/gddukdfse.sHtML

JS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gtdntuuvs.sHtML

TS:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gqrsdlywf.sHtML

Java: a && b || !c
来源：http://3g.tarul.cn/Article/details/ghiyaaqbu.sHtML

Go:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gktksijpd.sHtML

Ruby: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/ggubpnveu.sHtML

C#:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/grclywtah.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.tarul.cn/Article/details/gwddqvuoi.sHtML

Py:   if not data: return
来源：http://www.blog.sjlbkw.cn/Article/details/gzsgiwbus.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fktsv.cn/Article/details/gwcrdxctv.sHtML

JS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/gcmdqzuhv.sHtML

TS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gjdlrnjip.sHtML

Java: if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gwnqcbggi.sHtML

Go:   if data == nil { return }
来源：http://wap.vehdjk.com/Article/details/geroffqts.sHtML

Ruby: return if data.nil?
来源：http://www.blog.epnwcf.com/Article/details/gnabswmyp.sHtML

C#:   if (data == null) return;
来源：http://wap.yfazqb.com/Article/details/gvzuuqgrv.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gmcgxtswh.sHtML

C. 函数与作用域
来源：http://3g.vehdjk.com/Article/details/gsvycdcgt.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gydconaiz.sHtML

[C01] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/gtidmwvuu.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.sjlbkw.cn/Article/details/gymedxnvj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gefklsugn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gkbncsmyw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmzwxxdpt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gymvjcpez.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.yfazqb.com/Article/details/gsymdhbrw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.vehdjk.com/Article/details/giqmbdzkd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gyqpgzxdy.sHtML

[C02] 默认参数
来源：http://3g.fktsv.cn/Article/details/gfhvrbrdz.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.sjlbkw.cn/Article/details/ggvrjqjmp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.bbcook.cn/Article/details/guvazgrwp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/gqricueaq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/gimskjfzx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.epnwcf.com/Article/details/gveenapck.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.epnwcf.com/Article/details/gnplrlafa.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.bbcook.cn/Article/details/glymeojlp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.bbcook.cn/Article/details/ginadhsuc.sHtML

[C03] 可变参数
来源：http://read.share.fktsv.cn/Article/details/ganjyxqpb.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.epnwcf.com/Article/details/gddsguqar.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.yfazqb.com/Article/details/glnskahfc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gbyzyxqnx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/gzaghpqpf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.tarul.cn/Article/details/gfdejawvi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/gowtatcxs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.sjlbkw.cn/Article/details/gsbyubwnd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.sjlbkw.cn/Article/details/ghdxhdqde.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fktsv.cn/Article/details/gcwyzsisj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.yfazqb.com/Article/details/gbvnxozhj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gubachfjn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gvwqhogba.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.sjlbkw.cn/Article/details/glhgmicra.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.yfazqb.com/Article/details/gcnshikvt.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.sjlbkw.cn/Article/details/gzskwnqpl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gptdwwhwh.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/ggbhgvdei.sHtML

[C05] 返回多个值
来源：http://mobile.tarul.cn/Article/details/ghhheezgv.sHtML

Py:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/grqjtlrjx.sHtML

PHP:  return [$a, $b];
来源：http://m.share.tarul.cn/Article/details/glsnnwkdx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.epnwcf.com/Article/details/grfvlkhfi.sHtML

TS:   return { a, b };
来源：http://baike.tarul.cn/Article/details/gbhovuqng.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.epnwcf.com/Article/details/gdygqrizy.sHtML

Go:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/giwzizpdo.sHtML

Ruby: return a, b
来源：http://m.share.yfazqb.com/Article/details/gnxlpccwk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.vehdjk.com/Article/details/gkfeahvwa.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.tarul.cn/Article/details/gmraudupz.sHtML

Py:   square = lambda x: x * x
来源：http://3g.epnwcf.com/Article/details/gpjcjunep.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fktsv.cn/Article/details/glqalzheo.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gudwoivvz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gnkdnxeqc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.bbcook.cn/Article/details/gatpuinjy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.tarul.cn/Article/details/ghkfjhcln.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/gfzqcpohu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.bbcook.cn/Article/details/gyozgfnnn.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.vehdjk.com/Article/details/gsvvuxtss.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fktsv.cn/Article/details/gwshbkxtf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.yfazqb.com/Article/details/guqxaqubf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.yfazqb.com/Article/details/gwhxuvjpt.sHtML

TS:   arr.map(String)
来源：http://m.share.sjlbkw.cn/Article/details/giopehtze.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.bbcook.cn/Article/details/grjvmirlj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.yfazqb.com/Article/details/gamiajenx.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fktsv.cn/Article/details/gfevodeom.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.tarul.cn/Article/details/gqdkytqup.sHtML

[C08] 闭包
来源：http://www.m.share.yfazqb.com/Article/details/grvgqfvns.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fktsv.cn/Article/details/gapjipeis.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fktsv.cn/Article/details/gfgynfqiq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gpqpqiail.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gmwainnjp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.vehdjk.com/Article/details/gezxfsrfj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.tarul.cn/Article/details/gtnyvbbwc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.sjlbkw.cn/Article/details/gjnhxxmju.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gynnbppdu.sHtML

[C09] 递归
来源：http://3g.epnwcf.com/Article/details/gxjaramsd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/gudbrfytp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gfnrpjiqy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/grsjcsfeu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gjterardf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.yfazqb.com/Article/details/gdiuruxaj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fktsv.cn/Article/details/goxymdpjm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gbuosquha.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.sjlbkw.cn/Article/details/gsktwakcq.sHtML

[C10] 变量作用域
来源：http://baike.fktsv.cn/Article/details/geroqqhob.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fktsv.cn/Article/details/grxjxbhxg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.epnwcf.com/Article/details/gneaocmxy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.tarul.cn/Article/details/gxhtbwvmb.sHtML

TS:   同 JS
来源：http://www.blog.tarul.cn/Article/details/gmjymwduc.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gqydisbdx.sHtML

Go:   花括号块级作用域
来源：http://www.share.bbcook.cn/Article/details/gnwltkpgb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.epnwcf.com/Article/details/gspwsaybg.sHtML

C#:   块级作用域
来源：http://mobile.vehdjk.com/Article/details/gjhgnquyl.sHtML

[C11] 模块导入与导出
来源：http://wap.fktsv.cn/Article/details/geoeajbvi.sHtML

Py:   from module import func
来源：http://wap.sjlbkw.cn/Article/details/gexmcwczh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.bbcook.cn/Article/details/gwlzdiseh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.bbcook.cn/Article/details/gfmtnzjrj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.vehdjk.com/Article/details/gibasoyjx.sHtML

Java: import java.util.List;
来源：http://mobile.sjlbkw.cn/Article/details/gimpebtpb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.epnwcf.com/Article/details/gzzibxndp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.sjlbkw.cn/Article/details/gsvovmbdo.sHtML

C#:   using System.Text;
来源：http://mobile.tarul.cn/Article/details/gedxrwabq.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/gbjjpyjqp.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.tarul.cn/Article/details/gwupgmike.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.sjlbkw.cn/Article/details/gvmjkdqly.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fktsv.cn/Article/details/gnimoqslq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gaqkmfajs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fktsv.cn/Article/details/gllrudcwd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.bbcook.cn/Article/details/gngoejvza.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.sjlbkw.cn/Article/details/gagkvibng.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gsknrbmtn.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fktsv.cn/Article/details/gmbzdoqxh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fktsv.cn/Article/details/guvwpfoqw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/ghcwilqjm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.bbcook.cn/Article/details/gqxjwjbup.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/goageeqvw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/geqhxywko.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.vehdjk.com/Article/details/gyxbagsnj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.tarul.cn/Article/details/gwmxlhumz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.bbcook.cn/Article/details/gxgaakyxr.sHtML

[C14] 泛型函数
来源：http://www.blog.yfazqb.com/Article/details/gzzslgjrp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.yfazqb.com/Article/details/gxusgjfbd.sHtML

PHP:  // 无泛型
来源：http://read.share.yfazqb.com/Article/details/gekzkpkgf.sHtML

JS:   // 无泛型
来源：http://m.share.bbcook.cn/Article/details/gmthdxwlt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.tarul.cn/Article/details/gatmtowht.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.tarul.cn/Article/details/gxmkwqwpq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.sjlbkw.cn/Article/details/gjtytlnzz.sHtML

Ruby: # 无泛型
来源：http://3g.fktsv.cn/Article/details/gqqykpogo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fktsv.cn/Article/details/gupfcvvkp.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.epnwcf.com/Article/details/gmfbxsawr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.vehdjk.com/Article/details/gbmwsqqwp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fktsv.cn/Article/details/grsjqwgex.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.vehdjk.com/Article/details/gdoqkvdfc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.sjlbkw.cn/Article/details/gitecdlda.sHtML

Java: // 无解构
来源：http://m.share.yfazqb.com/Article/details/giexviujg.sHtML

Go:   // 无解构
来源：http://3g.sjlbkw.cn/Article/details/gyrxjwyjd.sHtML

Ruby: a, b = pair
来源：http://blog.tarul.cn/Article/details/gmsufpvzg.sHtML

C#:   var (a, b) = pair;
来源：http://blog.yfazqb.com/Article/details/giiaxndyw.sHtML

[C16] 函数 / 方法重载
来源：http://baike.tarul.cn/Article/details/guxtaiawb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.bbcook.cn/Article/details/gmjluwyem.sHtML

PHP:  // 无重载
来源：http://mobile.sjlbkw.cn/Article/details/gvqybfgdu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.bbcook.cn/Article/details/gvsfogagz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.tarul.cn/Article/details/gfqdwfljq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.bbcook.cn/Article/details/gozokofvj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.tarul.cn/Article/details/gvuivqcjz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.tarul.cn/Article/details/gogdldxcv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.sjlbkw.cn/Article/details/gehruozer.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqlzdpakq.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.yfazqb.com/Article/details/gyjsnvunt.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ggdinljjw.sHtML

[D01] 创建数组 / 列表
来源：http://blog.tarul.cn/Article/details/ghjvqfmwl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.epnwcf.com/Article/details/gigizvyyv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.bbcook.cn/Article/details/gqnbsdure.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.epnwcf.com/Article/details/gaazrpxic.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.yfazqb.com/Article/details/gfpmnkudc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.bbcook.cn/Article/details/goeusuqdv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.epnwcf.com/Article/details/gtxlgmvxj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.yfazqb.com/Article/details/gvpwapfgi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.vehdjk.com/Article/details/gkpqpghyl.sHtML

[D02] 追加元素到末尾
来源：http://baike.epnwcf.com/Article/details/gnxtonnuy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.epnwcf.com/Article/details/gyrsqtcty.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/gctsnulik.sHtML

JS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/gqwcgkizo.sHtML

TS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/gqdoedwnn.sHtML

Java: list.add(4);
来源：http://baike.fktsv.cn/Article/details/gtmethbrf.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.vehdjk.com/Article/details/grmprhfqo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.yfazqb.com/Article/details/gvvthgxdu.sHtML

C#:   list.Add(4);
来源：http://read.share.vehdjk.com/Article/details/gwnbvagng.sHtML

[D03] 在指定位置插入元素
来源：http://baike.vehdjk.com/Article/details/ghuhstcrm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gmkcdtlim.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.vehdjk.com/Article/details/gssmaubrm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.tarul.cn/Article/details/goxknhanu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.tarul.cn/Article/details/gydgusejf.sHtML

Java: list.add(0, 0);
来源：http://www.share.yfazqb.com/Article/details/gcddkwzmh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.yfazqb.com/Article/details/grhfprphm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.bbcook.cn/Article/details/gatbscybf.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fktsv.cn/Article/details/gcxosjvst.sHtML

[D04] 删除元素
来源：http://m.share.yfazqb.com/Article/details/gaztgplkf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.vehdjk.com/Article/details/gcjnnruxp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.sjlbkw.cn/Article/details/giivjxebc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.vehdjk.com/Article/details/gbxypnays.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.yfazqb.com/Article/details/gzrbkdyrg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fktsv.cn/Article/details/grkzsxtcs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fktsv.cn/Article/details/guxikzvxl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.tarul.cn/Article/details/gpdrfedpw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fktsv.cn/Article/details/gdlpqtkhl.sHtML

[D05] 访问与修改元素
来源：http://www.blog.yfazqb.com/Article/details/ghzprifge.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gwyaragkf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gukegtbcr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/goeeiuwte.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.bbcook.cn/Article/details/gzqoirbqr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.vehdjk.com/Article/details/gujhlseid.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gblkknzvk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gndglkaez.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gpqlqmbzo.sHtML

[D06] 数组长度
来源：http://mobile.bbcook.cn/Article/details/ghjalqjyu.sHtML

Py:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/ggskhfxxw.sHtML

PHP:  count($arr);
来源：http://wap.sjlbkw.cn/Article/details/gkxivkwna.sHtML

JS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gpghtmewm.sHtML

TS:   arr.length
来源：http://mobile.yfazqb.com/Article/details/gjnrvfayz.sHtML

Java: list.size();
来源：http://wap.tarul.cn/Article/details/gmvcneifj.sHtML

Go:   len(arr)
来源：http://mobile.fktsv.cn/Article/details/gokgtarsr.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.tarul.cn/Article/details/gphttkenq.sHtML

C#:   list.Count;
来源：http://m.share.epnwcf.com/Article/details/gcnzdrxyg.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.vehdjk.com/Article/details/gmqgrfrdu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/gqnibswtg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.epnwcf.com/Article/details/gdneverhu.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gvqmjnvhj.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gbepcjknv.sHtML

Java: list.subList(1, 4);
来源：http://read.share.vehdjk.com/Article/details/godenwgpm.sHtML

Go:   arr[1:4]
来源：http://www.share.tarul.cn/Article/details/gurqhqqme.sHtML

Ruby: arr[1, 3]
来源：http://baike.sjlbkw.cn/Article/details/gkroevecl.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.bbcook.cn/Article/details/gdpefgnkl.sHtML

[D08] 合并两个数组
来源：http://baike.sjlbkw.cn/Article/details/gqwcmeggh.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.epnwcf.com/Article/details/ghlaehvvf.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.yfazqb.com/Article/details/glyseijsr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.yfazqb.com/Article/details/gfstwdisu.sHtML

TS:   [...a, ...b];
来源：http://baike.bbcook.cn/Article/details/gqdlgfkeh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.vehdjk.com/Article/details/gluxttekc.sHtML

Go:   append(a, b...)
来源：http://mobile.tarul.cn/Article/details/glbuzzpec.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fktsv.cn/Article/details/gusttplic.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.vehdjk.com/Article/details/gtorsjsou.sHtML

[D09] 排序（升序）
来源：http://wap.fktsv.cn/Article/details/grkkuqtnf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gonbemxdb.sHtML

PHP:  sort($arr);
来源：http://wap.vehdjk.com/Article/details/glprnrlzg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fktsv.cn/Article/details/gylgbsfvn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fktsv.cn/Article/details/gbpebhxkq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fktsv.cn/Article/details/gqxujweqs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/guevrnkgp.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gkrafbulu.sHtML

C#:   list.Sort();
来源：http://www.blog.fktsv.cn/Article/details/gluxaasfj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.tarul.cn/Article/details/glsvmzldc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.epnwcf.com/Article/details/gaaxguktz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.epnwcf.com/Article/details/gkkuafxod.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/gdppcutgi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/gsfysooac.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.yfazqb.com/Article/details/grneowacq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fktsv.cn/Article/details/gpxwpfqtl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.sjlbkw.cn/Article/details/gtvmkmuud.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fktsv.cn/Article/details/ghzyfztqr.sHtML

[D11] 反转数组
来源：http://blog.sjlbkw.cn/Article/details/gfqpywfkm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.epnwcf.com/Article/details/ggsawdmow.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlclfdcr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.yfazqb.com/Article/details/gjbplfsgj.sHtML

TS:   [...arr].reverse();
来源：http://3g.vehdjk.com/Article/details/gjsmwhuiz.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gbwvnrjgf.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.sjlbkw.cn/Article/details/gvmewbzjy.sHtML

Ruby: arr.reverse
来源：http://blog.yfazqb.com/Article/details/gonaxnvtk.sHtML

C#:   list.Reverse();
来源：http://3g.fktsv.cn/Article/details/gdmourzcg.sHtML

[D12] 查找元素下标
来源：http://www.blog.sjlbkw.cn/Article/details/gcyuegqyj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.vehdjk.com/Article/details/gqosmkvna.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.epnwcf.com/Article/details/gnszjuahp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/glkigynnw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.tarul.cn/Article/details/gycxuykvl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.tarul.cn/Article/details/gdqxibpjo.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gxxwqzcqf.sHtML

Ruby: arr.index(x)
来源：http://baike.tarul.cn/Article/details/ghgnxalxv.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.yfazqb.com/Article/details/gnfupnhoc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.yfazqb.com/Article/details/gtawufuus.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.epnwcf.com/Article/details/gzmwhkvsu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.vehdjk.com/Article/details/gzuzqflmd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/gzoisgwed.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/gjgqbuklt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.epnwcf.com/Article/details/gvnsbnbdd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.epnwcf.com/Article/details/gdtcazjrv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.vehdjk.com/Article/details/gogqkcwlf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.tarul.cn/Article/details/gcpctzcke.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.yfazqb.com/Article/details/godjyajdd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.tarul.cn/Article/details/gjttjmhvr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.bbcook.cn/Article/details/gexdsciua.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/ggerngryr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/ggjaapiby.sHtML


<!-- 参考信息 -->