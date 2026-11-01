代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.tarul.cn/Article/details/gabxiohad.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.vehdjk.com/Article/details/gsrvolaqh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gwetmspyk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/goyjtwqvk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/grtznzcli.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.sjlbkw.cn/Article/details/gmvqjtxjm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.yfazqb.com/Article/details/gghjltivr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.vehdjk.com/Article/details/gnhanapyz.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.sjlbkw.cn/Article/details/govmuptqu.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.yfazqb.com/Article/details/glxtiotes.sHtML

PHP:  is_numeric($x)
来源：http://wap.yfazqb.com/Article/details/gusozdgdp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/gkuxqiywl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/gixewxvrq.sHtML

Java: x instanceof Number
来源：http://wap.bbcook.cn/Article/details/gzttfqqml.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.vehdjk.com/Article/details/gdhznbzhv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.epnwcf.com/Article/details/gzeaktwin.sHtML

C#:   x is int or double or decimal
来源：http://mobile.yfazqb.com/Article/details/gqnvreanw.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.bbcook.cn/Article/details/gyxyseqpw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.yfazqb.com/Article/details/gjnolreal.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.sjlbkw.cn/Article/details/gucxidgfo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gcwlfetfs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gheojqwih.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.tarul.cn/Article/details/ggeciatbs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.bbcook.cn/Article/details/grwnxgont.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.yfazqb.com/Article/details/gkodjdchd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gbrzkamqw.sHtML

[B15] 布尔运算与取反
来源：http://baike.bbcook.cn/Article/details/gcmqdmdlt.sHtML

Py:   a and b or not c
来源：http://blog.yfazqb.com/Article/details/guhtreikf.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.bbcook.cn/Article/details/geicrtapl.sHtML

JS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/ghogshhqm.sHtML

TS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gqjccorxg.sHtML

Java: a && b || !c
来源：http://wap.tarul.cn/Article/details/gbpffleur.sHtML

Go:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gadqhrmjo.sHtML

Ruby: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gfowjjllf.sHtML

C#:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gvpreskex.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.bbcook.cn/Article/details/gwsnzjjox.sHtML

Py:   if not data: return
来源：http://www.share.tarul.cn/Article/details/ghgsrcjml.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.epnwcf.com/Article/details/gpzbasxoc.sHtML

JS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/gefoafrjx.sHtML

TS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gxwhhkfch.sHtML

Java: if (data == null) return;
来源：http://www.share.tarul.cn/Article/details/gxjnvguhy.sHtML

Go:   if data == nil { return }
来源：http://baike.vehdjk.com/Article/details/gbkzmcayh.sHtML

Ruby: return if data.nil?
来源：http://blog.epnwcf.com/Article/details/grzewqoxj.sHtML

C#:   if (data == null) return;
来源：http://3g.epnwcf.com/Article/details/gkveruvil.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdxppmpwj.sHtML

C. 函数与作用域
来源：http://www.share.epnwcf.com/Article/details/gzasoejfe.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gpuyawrap.sHtML

[C01] 定义函数
来源：http://baike.tarul.cn/Article/details/gzqraxzlq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gccxtsvrn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/grasgmfqr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gggxgxrej.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/guwttxmpv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gvmdimbuq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.vehdjk.com/Article/details/gximgkstn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/gmybgjbbv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gmensyxzr.sHtML

[C02] 默认参数
来源：http://www.share.tarul.cn/Article/details/gywtifzcl.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.bbcook.cn/Article/details/gaeqbnzly.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.tarul.cn/Article/details/glnpjlglh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gilqyuprg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/gfebikass.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.bbcook.cn/Article/details/gggummfpg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fktsv.cn/Article/details/gfrgyfaxn.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.sjlbkw.cn/Article/details/gcwxmelak.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.vehdjk.com/Article/details/gghptivru.sHtML

[C03] 可变参数
来源：http://baike.epnwcf.com/Article/details/gfognlxaw.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.vehdjk.com/Article/details/grjjspjdw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.tarul.cn/Article/details/gvvyqeqro.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fktsv.cn/Article/details/gmqhiufex.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.vehdjk.com/Article/details/gpokfocxu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.vehdjk.com/Article/details/gzogelmxc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.vehdjk.com/Article/details/gzgbmjiyx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.sjlbkw.cn/Article/details/guuljgxky.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.tarul.cn/Article/details/ggywhtfzy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.bbcook.cn/Article/details/glnzfczhj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.vehdjk.com/Article/details/gkordkwcq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.epnwcf.com/Article/details/gxwlvdgwy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/glswvxwmw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.sjlbkw.cn/Article/details/gmeznqqwg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.epnwcf.com/Article/details/gxdzbslgi.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fktsv.cn/Article/details/gfratraix.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/guqrrngco.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/gfviyezkb.sHtML

[C05] 返回多个值
来源：http://m.share.bbcook.cn/Article/details/gblwargfn.sHtML

Py:   return a, b
来源：http://m.share.bbcook.cn/Article/details/galgqqcis.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.tarul.cn/Article/details/gkeznapqw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.epnwcf.com/Article/details/gkidyxeki.sHtML

TS:   return { a, b };
来源：http://baike.epnwcf.com/Article/details/gmbgeacrc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.bbcook.cn/Article/details/gcprkqfsf.sHtML

Go:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gleygrlcl.sHtML

Ruby: return a, b
来源：http://blog.bbcook.cn/Article/details/grrnnwiwa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.bbcook.cn/Article/details/gcpvoyvbh.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.epnwcf.com/Article/details/grcuekdmo.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.epnwcf.com/Article/details/gpivfhnag.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.sjlbkw.cn/Article/details/grurwzrqj.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gsidfwypw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fktsv.cn/Article/details/gjupdmyfm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.bbcook.cn/Article/details/gndgqhkwt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.epnwcf.com/Article/details/gcpquvwsd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.vehdjk.com/Article/details/gvtqbgivx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gnyjfenhd.sHtML

[C07] 把函数作为参数传入
来源：http://wap.tarul.cn/Article/details/gmcfsqvol.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.vehdjk.com/Article/details/ggxdamnlk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/gqkjxqqyo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.bbcook.cn/Article/details/gokkbmcfl.sHtML

TS:   arr.map(String)
来源：http://www.blog.yfazqb.com/Article/details/gnuywdgoc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/gqoufvrwz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.tarul.cn/Article/details/gockuuasr.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.yfazqb.com/Article/details/gxuxnnpho.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fktsv.cn/Article/details/gudtrwquo.sHtML

[C08] 闭包
来源：http://www.share.yfazqb.com/Article/details/gnnhrwjcc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.sjlbkw.cn/Article/details/gcjovldge.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.sjlbkw.cn/Article/details/gtemyovnx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gvltnljkf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gpingbjbi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.sjlbkw.cn/Article/details/gytpnnshv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.tarul.cn/Article/details/guelmhqsu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.bbcook.cn/Article/details/gxgimjabt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gysffvhft.sHtML

[C09] 递归
来源：http://wap.yfazqb.com/Article/details/gfebzxyca.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/gmaqjylen.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/gftttjyah.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fktsv.cn/Article/details/gpqzvamyj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/gigdcdkdt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.yfazqb.com/Article/details/gnfilxsit.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.epnwcf.com/Article/details/gkgimcaqf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.sjlbkw.cn/Article/details/gduidmxje.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.tarul.cn/Article/details/gseyjstcw.sHtML

[C10] 变量作用域
来源：http://baike.vehdjk.com/Article/details/gsrwperbn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.vehdjk.com/Article/details/gsibvsjny.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.bbcook.cn/Article/details/ggnqvxdwl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.vehdjk.com/Article/details/gnwizhwzh.sHtML

TS:   同 JS
来源：http://www.share.epnwcf.com/Article/details/gkbxeyemh.sHtML

Java: 方法内为块级作用域
来源：http://blog.bbcook.cn/Article/details/gbgobgifp.sHtML

Go:   花括号块级作用域
来源：http://3g.tarul.cn/Article/details/gjynqrsvr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.vehdjk.com/Article/details/gflwqnrxt.sHtML

C#:   块级作用域
来源：http://3g.yfazqb.com/Article/details/ghkoowfeb.sHtML

[C11] 模块导入与导出
来源：http://baike.vehdjk.com/Article/details/gwsjninoq.sHtML

Py:   from module import func
来源：http://www.share.bbcook.cn/Article/details/gapbddzma.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.tarul.cn/Article/details/glhvndvke.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.epnwcf.com/Article/details/giwshfdgf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.epnwcf.com/Article/details/glnqtjvfv.sHtML

Java: import java.util.List;
来源：http://baike.epnwcf.com/Article/details/gvyfmuujp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fktsv.cn/Article/details/gfkxineij.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/ghjncdxif.sHtML

C#:   using System.Text;
来源：http://read.share.vehdjk.com/Article/details/gceakcgcn.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.bbcook.cn/Article/details/glorhxcsj.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.bbcook.cn/Article/details/gmwgikijp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.tarul.cn/Article/details/grdsleztg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.yfazqb.com/Article/details/gdqotxxel.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.yfazqb.com/Article/details/gyhtmrmxj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.yfazqb.com/Article/details/gdlzjsogl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.yfazqb.com/Article/details/gjreowkei.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.yfazqb.com/Article/details/ghvnltmyg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fktsv.cn/Article/details/gqjfkkqid.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.sjlbkw.cn/Article/details/gugedjtbb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.bbcook.cn/Article/details/gldfhhdyd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gddfsngrz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.bbcook.cn/Article/details/gumzmmuyg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gjpznhull.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gdflpkzwv.sHtML

Go:   func add(a, b int) int
来源：http://wap.fktsv.cn/Article/details/gukeanmwt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.vehdjk.com/Article/details/ghbcfvcxp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.bbcook.cn/Article/details/gqndxzlkk.sHtML

[C14] 泛型函数
来源：http://blog.vehdjk.com/Article/details/gkqknjhot.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.sjlbkw.cn/Article/details/ghwcetohm.sHtML

PHP:  // 无泛型
来源：http://blog.epnwcf.com/Article/details/gpalpdiad.sHtML

JS:   // 无泛型
来源：http://baike.yfazqb.com/Article/details/gchtejjrp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.vehdjk.com/Article/details/gdifnbekv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.yfazqb.com/Article/details/gvspwczxn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.epnwcf.com/Article/details/gzggtwvar.sHtML

Ruby: # 无泛型
来源：http://wap.yfazqb.com/Article/details/gaxnsbzmh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.yfazqb.com/Article/details/gtqtsamqt.sHtML

[C15] 解构 / 展开参数
来源：http://wap.yfazqb.com/Article/details/gjhgkenxk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.epnwcf.com/Article/details/gsyzljpfu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.bbcook.cn/Article/details/gpluoawnm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/glbcbwagn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.yfazqb.com/Article/details/gareujdgu.sHtML

Java: // 无解构
来源：http://read.share.yfazqb.com/Article/details/gbezgjosz.sHtML

Go:   // 无解构
来源：http://3g.sjlbkw.cn/Article/details/gchvlomyq.sHtML

Ruby: a, b = pair
来源：http://www.share.epnwcf.com/Article/details/gkxewsauo.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fktsv.cn/Article/details/gloxilntz.sHtML

[C16] 函数 / 方法重载
来源：http://3g.sjlbkw.cn/Article/details/gmdzxexbs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.sjlbkw.cn/Article/details/grwrsalzn.sHtML

PHP:  // 无重载
来源：http://www.m.share.yfazqb.com/Article/details/guluictpn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.epnwcf.com/Article/details/gbccnylse.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.vehdjk.com/Article/details/gglgsjrtc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.vehdjk.com/Article/details/gaeqprgjd.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.sjlbkw.cn/Article/details/guoxueeeb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.yfazqb.com/Article/details/gzpldhoef.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.vehdjk.com/Article/details/gptaidvlb.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grywcyatm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.vehdjk.com/Article/details/gjlleiucz.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/golphmurh.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlzxbihy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.vehdjk.com/Article/details/gvnstyhhk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.tarul.cn/Article/details/ghjxmyowi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.bbcook.cn/Article/details/gcshfdkez.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.epnwcf.com/Article/details/glvvnmtwf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.yfazqb.com/Article/details/gbnbiarus.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.sjlbkw.cn/Article/details/gpnfrntpn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.epnwcf.com/Article/details/gtcbpggdp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fktsv.cn/Article/details/gmgwhxmxe.sHtML

[D02] 追加元素到末尾
来源：http://read.share.epnwcf.com/Article/details/gvcbeplpu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfbomknx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.sjlbkw.cn/Article/details/gavkedmdq.sHtML

JS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/gbrbbidkp.sHtML

TS:   arr.push(4);
来源：http://mobile.epnwcf.com/Article/details/girgnvvfd.sHtML

Java: list.add(4);
来源：http://wap.tarul.cn/Article/details/guweqxwqr.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.tarul.cn/Article/details/gogbqptbg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fktsv.cn/Article/details/gwhhfrttg.sHtML

C#:   list.Add(4);
来源：http://wap.sjlbkw.cn/Article/details/gyzqmkacj.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.tarul.cn/Article/details/gpqxdnqep.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.vehdjk.com/Article/details/gduvrwvgz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.epnwcf.com/Article/details/gwnckaqha.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.sjlbkw.cn/Article/details/gjurthdoj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.vehdjk.com/Article/details/gwmfoguqc.sHtML

Java: list.add(0, 0);
来源：http://read.share.yfazqb.com/Article/details/gdhpsrzir.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.bbcook.cn/Article/details/gknnnvqgk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.vehdjk.com/Article/details/ghxasvopk.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/ghfyihxqs.sHtML

[D04] 删除元素
来源：http://www.share.bbcook.cn/Article/details/gfbpolora.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.yfazqb.com/Article/details/gyocetvrj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.tarul.cn/Article/details/gkvqqxwgm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.bbcook.cn/Article/details/ghouesccp.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fktsv.cn/Article/details/gnurmzysn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fktsv.cn/Article/details/gmlprsmiw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.tarul.cn/Article/details/gzuracthb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fktsv.cn/Article/details/gyobdravj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.vehdjk.com/Article/details/ghncviccd.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gkymphdni.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gfsiskuzc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.epnwcf.com/Article/details/gohcnvcuk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/guaeaplsn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.sjlbkw.cn/Article/details/gsaylnsqf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fktsv.cn/Article/details/gurobwtyy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gifgnroeo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gihemquof.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gavhrnbzk.sHtML

[D06] 数组长度
来源：http://baike.tarul.cn/Article/details/gahnvacqr.sHtML

Py:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gdlrkbwes.sHtML

PHP:  count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gjwpxnezx.sHtML

JS:   arr.length
来源：http://www.share.yfazqb.com/Article/details/gnudyakqm.sHtML

TS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/gqfnbuzyz.sHtML

Java: list.size();
来源：http://www.blog.sjlbkw.cn/Article/details/gknflhtox.sHtML

Go:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gszfhasjh.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.tarul.cn/Article/details/gweshiqmg.sHtML

C#:   list.Count;
来源：http://blog.sjlbkw.cn/Article/details/gcbemphan.sHtML

[D07] 切片 / 取子数组
来源：http://wap.vehdjk.com/Article/details/gynzcrlfk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.vehdjk.com/Article/details/ggbbvwcyg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.sjlbkw.cn/Article/details/gbldxjilb.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gzawwmtgh.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/ghpiwtkrm.sHtML

Java: list.subList(1, 4);
来源：http://m.share.epnwcf.com/Article/details/gspazrcnm.sHtML

Go:   arr[1:4]
来源：http://m.share.vehdjk.com/Article/details/gxrzrcovu.sHtML

Ruby: arr[1, 3]
来源：http://3g.bbcook.cn/Article/details/gxhdqinfl.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gqzlldehh.sHtML

[D08] 合并两个数组
来源：http://mobile.epnwcf.com/Article/details/gnfsostnn.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.epnwcf.com/Article/details/ggdrmcaax.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.bbcook.cn/Article/details/gwiloekkj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fktsv.cn/Article/details/gfcybgpnv.sHtML

TS:   [...a, ...b];
来源：http://read.share.fktsv.cn/Article/details/gwazchxlt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gtsuywkyr.sHtML

Go:   append(a, b...)
来源：http://m.share.yfazqb.com/Article/details/gjpzvlehv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.vehdjk.com/Article/details/gpmmsnses.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gckqrjfoz.sHtML

[D09] 排序（升序）
来源：http://3g.sjlbkw.cn/Article/details/gylmileqs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gxxqetqcf.sHtML

PHP:  sort($arr);
来源：http://wap.vehdjk.com/Article/details/goiewictw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.tarul.cn/Article/details/guhqyndpu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.tarul.cn/Article/details/ghesnnvyc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.tarul.cn/Article/details/gbfgifpcm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/gsqwhmozv.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/gznhrwprs.sHtML

C#:   list.Sort();
来源：http://baike.tarul.cn/Article/details/gbicrnfdu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.bbcook.cn/Article/details/gjaataynu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.sjlbkw.cn/Article/details/gmzmeudcr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/gtqkizlie.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gaejhries.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.bbcook.cn/Article/details/grreogtgb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.bbcook.cn/Article/details/geqlfekgf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.yfazqb.com/Article/details/gjargvlhk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fktsv.cn/Article/details/gfjnkprmt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.bbcook.cn/Article/details/glrrjkeem.sHtML

[D11] 反转数组
来源：http://read.share.fktsv.cn/Article/details/gffboyzjn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.tarul.cn/Article/details/gwiygiptm.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gfdwvfhya.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.yfazqb.com/Article/details/gaytersjq.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.sjlbkw.cn/Article/details/ghghvjvtx.sHtML

Java: Collections.reverse(list);
来源：http://baike.yfazqb.com/Article/details/gtxwwvoah.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/glulyefgv.sHtML

Ruby: arr.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gctajibma.sHtML

C#:   list.Reverse();
来源：http://wap.vehdjk.com/Article/details/gyrgccgws.sHtML

[D12] 查找元素下标
来源：http://blog.yfazqb.com/Article/details/gpcslpnyx.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fktsv.cn/Article/details/gslzqqhvz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.yfazqb.com/Article/details/giucumccf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gdfysjhcl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.epnwcf.com/Article/details/gooiifati.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fktsv.cn/Article/details/gsxtbnftd.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.epnwcf.com/Article/details/gfrazkorw.sHtML


<!-- 参考信息 -->