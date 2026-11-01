代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.bbcook.cn/Article/details/gkvhfeasm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fktsv.cn/Article/details/goybjpqlo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/gfwdqolfh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gmwiwzlbe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gismimjmk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.sjlbkw.cn/Article/details/gdvjzpvti.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.yfazqb.com/Article/details/gjmzmgooy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/gykattxsn.sHtML

[B13] 判断是否为数字
来源：http://m.share.sjlbkw.cn/Article/details/gqenmyyfb.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.tarul.cn/Article/details/goygivohd.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.yfazqb.com/Article/details/gtycwbbfu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/ghwnfzzkw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.tarul.cn/Article/details/grhrvdizb.sHtML

Java: x instanceof Number
来源：http://www.share.tarul.cn/Article/details/gccvmaije.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.bbcook.cn/Article/details/ghthxeqso.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fktsv.cn/Article/details/ghxjduryp.sHtML

C#:   x is int or double or decimal
来源：http://blog.tarul.cn/Article/details/gpxalaozn.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.vehdjk.com/Article/details/gtctyqnwl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.epnwcf.com/Article/details/gkkaeycee.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.yfazqb.com/Article/details/gblukjumv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fktsv.cn/Article/details/grlzulqsb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gzavowxem.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.vehdjk.com/Article/details/guxiuekwk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.vehdjk.com/Article/details/gcpbnelll.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.vehdjk.com/Article/details/gpdvosgto.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gbhcweoce.sHtML

[B15] 布尔运算与取反
来源：http://read.share.yfazqb.com/Article/details/gfjduuowf.sHtML

Py:   a and b or not c
来源：http://www.share.vehdjk.com/Article/details/ggzmmrbhc.sHtML

PHP:  $a && $b || !$c
来源：http://wap.vehdjk.com/Article/details/gzrbiuntl.sHtML

JS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gbrgpcjkg.sHtML

TS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gmavhuyzw.sHtML

Java: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gfqofqizy.sHtML

Go:   a && b || !c
来源：http://baike.tarul.cn/Article/details/glnxrhmap.sHtML

Ruby: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gekbietni.sHtML

C#:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gguozcror.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.vehdjk.com/Article/details/gfgyzavdd.sHtML

Py:   if not data: return
来源：http://m.share.yfazqb.com/Article/details/gcnofapup.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fktsv.cn/Article/details/ghmkfgdxq.sHtML

JS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gmzlxkvyb.sHtML

TS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gtvnoinda.sHtML

Java: if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/gtcyccwoo.sHtML

Go:   if data == nil { return }
来源：http://mobile.tarul.cn/Article/details/gezgjvjah.sHtML

Ruby: return if data.nil?
来源：http://m.share.yfazqb.com/Article/details/gpiqasxhq.sHtML

C#:   if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/gyfebwqqr.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdvnyjdma.sHtML

C. 函数与作用域
来源：http://www.blog.fktsv.cn/Article/details/gsgcuzxmc.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gcqitdzof.sHtML

[C01] 定义函数
来源：http://read.share.yfazqb.com/Article/details/ghoymifzh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gyspmszky.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/ghfgfyjgr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gqsvnuwmt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/ghbvtakzq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gssvbrxtq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/gsmndrnfa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fktsv.cn/Article/details/gtejscxmy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gvcykcodh.sHtML

[C02] 默认参数
来源：http://m.share.epnwcf.com/Article/details/glteunxkj.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fktsv.cn/Article/details/gympbvfwx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.sjlbkw.cn/Article/details/gjbxdgdzi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/gzykkknbg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gonhtcknf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fktsv.cn/Article/details/gggweqiox.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.vehdjk.com/Article/details/gvphiqwbd.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.epnwcf.com/Article/details/gwasbiqpl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.bbcook.cn/Article/details/gmbabdtau.sHtML

[C03] 可变参数
来源：http://www.blog.bbcook.cn/Article/details/gujnsxymc.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.tarul.cn/Article/details/gimiwqzvf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.yfazqb.com/Article/details/gfnhhxbqk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.yfazqb.com/Article/details/gakvljjpp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gfgtmwlxv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.bbcook.cn/Article/details/gdelvtazm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fktsv.cn/Article/details/gwlmwzzow.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.yfazqb.com/Article/details/ggzbpizla.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.yfazqb.com/Article/details/gxowwdnys.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.yfazqb.com/Article/details/gjqrdrovf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.bbcook.cn/Article/details/gkzvohorf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fktsv.cn/Article/details/gtykjhzgz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/goaamxdqh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.sjlbkw.cn/Article/details/glwtmnkio.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.vehdjk.com/Article/details/ghcjagrlf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fktsv.cn/Article/details/gzebpxbis.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/giosnmoqb.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/grrpszima.sHtML

[C05] 返回多个值
来源：http://read.share.yfazqb.com/Article/details/gspvhunwg.sHtML

Py:   return a, b
来源：http://baike.yfazqb.com/Article/details/gswhayayk.sHtML

PHP:  return [$a, $b];
来源：http://wap.fktsv.cn/Article/details/gunkicipt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/grjmsxlct.sHtML

TS:   return { a, b };
来源：http://mobile.fktsv.cn/Article/details/ggixmeplm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.yfazqb.com/Article/details/gvfcprnud.sHtML

Go:   return a, b
来源：http://blog.bbcook.cn/Article/details/grttxdybn.sHtML

Ruby: return a, b
来源：http://baike.epnwcf.com/Article/details/ggnbhdffx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fktsv.cn/Article/details/gcpdptkey.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.tarul.cn/Article/details/gajwqajqc.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fktsv.cn/Article/details/gygwzoblw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.sjlbkw.cn/Article/details/gepfqvtcn.sHtML

JS:   const square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gfufmiwan.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fktsv.cn/Article/details/ghlrwiwxe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gfknytdph.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fktsv.cn/Article/details/gwlqpeyco.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.yfazqb.com/Article/details/gggcwaqny.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.tarul.cn/Article/details/ghiskoscw.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fktsv.cn/Article/details/glpsimrqb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.sjlbkw.cn/Article/details/gkukmzhwh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fktsv.cn/Article/details/gycutyaoj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.yfazqb.com/Article/details/gojlsbtkh.sHtML

TS:   arr.map(String)
来源：http://www.share.bbcook.cn/Article/details/gpslzpdlz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.epnwcf.com/Article/details/gtkfxkqxx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fktsv.cn/Article/details/gsmudblwp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.tarul.cn/Article/details/gapakaram.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.sjlbkw.cn/Article/details/gmjqzewrg.sHtML

[C08] 闭包
来源：http://mobile.fktsv.cn/Article/details/gfssnwwas.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.yfazqb.com/Article/details/gmvycfkbn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.yfazqb.com/Article/details/gjwgzgiom.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gvgmalntz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gardtqwen.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.yfazqb.com/Article/details/gbwmvhpjo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.bbcook.cn/Article/details/gkywkzjbm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.vehdjk.com/Article/details/gpkdguufq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gjttpsoln.sHtML

[C09] 递归
来源：http://3g.yfazqb.com/Article/details/goxekrjlp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gvmdlucso.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.bbcook.cn/Article/details/gdxmbdjsr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gcskvwcqs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gifzsecbc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.tarul.cn/Article/details/gztgaoikp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.tarul.cn/Article/details/geszcvqsn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/gluosmpty.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.yfazqb.com/Article/details/gqgnwpxnp.sHtML

[C10] 变量作用域
来源：http://www.blog.yfazqb.com/Article/details/gsklzhses.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.sjlbkw.cn/Article/details/guynaposj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.epnwcf.com/Article/details/gdaxdbcmg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.yfazqb.com/Article/details/gdlycjynu.sHtML

TS:   同 JS
来源：http://3g.yfazqb.com/Article/details/gkktarchc.sHtML

Java: 方法内为块级作用域
来源：http://baike.tarul.cn/Article/details/gpkyoyjjj.sHtML

Go:   花括号块级作用域
来源：http://mobile.yfazqb.com/Article/details/ghtzcgmhh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.yfazqb.com/Article/details/gvbmevepg.sHtML

C#:   块级作用域
来源：http://www.share.vehdjk.com/Article/details/gwrmtilbx.sHtML

[C11] 模块导入与导出
来源：http://3g.yfazqb.com/Article/details/goigheywn.sHtML

Py:   from module import func
来源：http://mobile.fktsv.cn/Article/details/gdtgwghyn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.yfazqb.com/Article/details/gwvizgmot.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gyaaunons.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fktsv.cn/Article/details/gamoivssb.sHtML

Java: import java.util.List;
来源：http://www.blog.tarul.cn/Article/details/gkgduvhje.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fktsv.cn/Article/details/gfnoxouoq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.sjlbkw.cn/Article/details/gazobytxv.sHtML

C#:   using System.Text;
来源：http://read.share.bbcook.cn/Article/details/gzmkeisak.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.bbcook.cn/Article/details/gbqbbdirr.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fktsv.cn/Article/details/gksiiasjl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.epnwcf.com/Article/details/gvgjfruea.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gbnrfsvel.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.epnwcf.com/Article/details/gssprwxtu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.vehdjk.com/Article/details/ghaelcfhi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.yfazqb.com/Article/details/glklvkijy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.vehdjk.com/Article/details/gpciuzzkj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.bbcook.cn/Article/details/gqjjqsbuc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.yfazqb.com/Article/details/gvfsfgbfe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.sjlbkw.cn/Article/details/gxcfhlegc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gfwkhbplf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fktsv.cn/Article/details/gxfwogekh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gashmidda.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gcvgfddfo.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fktsv.cn/Article/details/girytyird.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.yfazqb.com/Article/details/goshthjrm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.sjlbkw.cn/Article/details/gkhsjqzhm.sHtML

[C14] 泛型函数
来源：http://read.share.fktsv.cn/Article/details/ggecdewaj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.vehdjk.com/Article/details/grsaenphc.sHtML

PHP:  // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gykxtponk.sHtML

JS:   // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/grdvrgbdi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.vehdjk.com/Article/details/gkazjrzov.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fktsv.cn/Article/details/gzihfqwgd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.bbcook.cn/Article/details/ggdwfwksx.sHtML

Ruby: # 无泛型
来源：http://wap.epnwcf.com/Article/details/gbgryavrq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.bbcook.cn/Article/details/gokrmmldc.sHtML

[C15] 解构 / 展开参数
来源：http://baike.vehdjk.com/Article/details/giyafnpfk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.sjlbkw.cn/Article/details/gytnrsekf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.yfazqb.com/Article/details/getapwaoe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fktsv.cn/Article/details/gnkjfetbc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.tarul.cn/Article/details/gtlqsdeia.sHtML

Java: // 无解构
来源：http://read.share.vehdjk.com/Article/details/gqlumztdm.sHtML

Go:   // 无解构
来源：http://www.blog.vehdjk.com/Article/details/gkiauuhzz.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/gkkfhbrdw.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.yfazqb.com/Article/details/ggdtzxfiu.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.epnwcf.com/Article/details/gsxerzwdv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.vehdjk.com/Article/details/gnejyzpmy.sHtML

PHP:  // 无重载
来源：http://www.share.yfazqb.com/Article/details/gfybcirkk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.yfazqb.com/Article/details/gnqqcvwdg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.tarul.cn/Article/details/gcxlsgiis.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.epnwcf.com/Article/details/gmtcwtrer.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.vehdjk.com/Article/details/gssbcvcph.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.tarul.cn/Article/details/gsnspqamq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.tarul.cn/Article/details/gxlleocbj.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gqbhjfcyd.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.yfazqb.com/Article/details/gscnbuiro.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gbqpohwsu.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.yfazqb.com/Article/details/gyvsfadhp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.sjlbkw.cn/Article/details/gfziknxnc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.bbcook.cn/Article/details/gbthqijef.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.yfazqb.com/Article/details/grkzqhzhp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fktsv.cn/Article/details/gaqyevgmc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fktsv.cn/Article/details/gptyqpwto.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/gocsojfzr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.vehdjk.com/Article/details/gabrmlunf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.yfazqb.com/Article/details/gerwkmxsx.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.vehdjk.com/Article/details/gbvrjlnrh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.sjlbkw.cn/Article/details/gvxphxhir.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fktsv.cn/Article/details/gzpydbsco.sHtML

JS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/grxexsdpu.sHtML

TS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gaowbehbf.sHtML

Java: list.add(4);
来源：http://wap.bbcook.cn/Article/details/grjnfcnfl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fktsv.cn/Article/details/gatrnnrfh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.tarul.cn/Article/details/gbhyhrwnr.sHtML

C#:   list.Add(4);
来源：http://www.m.share.vehdjk.com/Article/details/ghxdrjcvb.sHtML

[D03] 在指定位置插入元素
来源：http://baike.bbcook.cn/Article/details/gzucdehyp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/grgibsxzb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.bbcook.cn/Article/details/gcglfnksk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.yfazqb.com/Article/details/gdbcklekp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.vehdjk.com/Article/details/gaanbiaqb.sHtML

Java: list.add(0, 0);
来源：http://blog.bbcook.cn/Article/details/godeqmhif.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.sjlbkw.cn/Article/details/gzioedjha.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.vehdjk.com/Article/details/gjcxrpbwv.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/ggfqeqijp.sHtML

[D04] 删除元素
来源：http://blog.fktsv.cn/Article/details/gzqhlltow.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.tarul.cn/Article/details/gyijhtxig.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.tarul.cn/Article/details/gcbyvtnzi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.tarul.cn/Article/details/gvxxeivor.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.bbcook.cn/Article/details/gjyskcsit.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.tarul.cn/Article/details/gwkrlufbq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.bbcook.cn/Article/details/gvhuymscx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.bbcook.cn/Article/details/guzxzoxet.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fktsv.cn/Article/details/godnyhrgm.sHtML

[D05] 访问与修改元素
来源：http://www.share.bbcook.cn/Article/details/gladlsxyp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/ghmkcguso.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/gwsynyxnc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/gkgnmurng.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.vehdjk.com/Article/details/gdmdxngyg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fktsv.cn/Article/details/ghfhsakax.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gzjbataws.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gsfrxexqn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gazojcveb.sHtML

[D06] 数组长度
来源：http://www.m.share.fktsv.cn/Article/details/gsybgtaur.sHtML

Py:   len(arr)
来源：http://baike.epnwcf.com/Article/details/gxjsqkebp.sHtML

PHP:  count($arr);
来源：http://mobile.vehdjk.com/Article/details/gthxwoqgk.sHtML

JS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/gifcyyeyq.sHtML

TS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/gwdsjknla.sHtML

Java: list.size();
来源：http://wap.epnwcf.com/Article/details/gipzgzgtc.sHtML

Go:   len(arr)
来源：http://mobile.vehdjk.com/Article/details/gjtpkojyc.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fktsv.cn/Article/details/gdhlftuke.sHtML

C#:   list.Count;
来源：http://m.share.fktsv.cn/Article/details/gvxvbohvn.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.epnwcf.com/Article/details/gkpxlsqko.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.yfazqb.com/Article/details/gqxgodvfa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.epnwcf.com/Article/details/gkdzaqfba.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.epnwcf.com/Article/details/gzygsvouy.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gdfiaeqag.sHtML

Java: list.subList(1, 4);
来源：http://3g.yfazqb.com/Article/details/gzmqjomno.sHtML

Go:   arr[1:4]
来源：http://wap.sjlbkw.cn/Article/details/gbpngbppa.sHtML

Ruby: arr[1, 3]
来源：http://mobile.epnwcf.com/Article/details/gxjilrtjt.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fktsv.cn/Article/details/guhgjftvy.sHtML

[D08] 合并两个数组
来源：http://mobile.yfazqb.com/Article/details/gcdvxeqzv.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.vehdjk.com/Article/details/gyastigwn.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.vehdjk.com/Article/details/gxqhednku.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.yfazqb.com/Article/details/geizxwsdl.sHtML

TS:   [...a, ...b];
来源：http://m.share.bbcook.cn/Article/details/gxxccsrsv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.epnwcf.com/Article/details/gsfuapmgj.sHtML

Go:   append(a, b...)
来源：http://wap.yfazqb.com/Article/details/gdorfypuz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.vehdjk.com/Article/details/giyauhgyc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/getuximti.sHtML

[D09] 排序（升序）
来源：http://mobile.sjlbkw.cn/Article/details/ghxdwuerr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/gjayllwot.sHtML

PHP:  sort($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gadzklade.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.tarul.cn/Article/details/gnuklndxw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.tarul.cn/Article/details/gjxniaqod.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.tarul.cn/Article/details/ghxuawihx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gzwceohwf.sHtML

Ruby: arr.sort
来源：http://baike.yfazqb.com/Article/details/giungxndq.sHtML

C#:   list.Sort();
来源：http://mobile.epnwcf.com/Article/details/gzoljbrhk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.vehdjk.com/Article/details/gqxiiqjgl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.sjlbkw.cn/Article/details/gifhwumme.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.tarul.cn/Article/details/ggouktjqo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gkcedimdg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fktsv.cn/Article/details/gvjdhvmqq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.epnwcf.com/Article/details/gmtthtchc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.vehdjk.com/Article/details/gwmqqtbzv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.sjlbkw.cn/Article/details/gikrzilwr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fktsv.cn/Article/details/gousvcrap.sHtML

[D11] 反转数组
来源：http://wap.vehdjk.com/Article/details/gbrzgrujy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.sjlbkw.cn/Article/details/ggttyydyx.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.vehdjk.com/Article/details/gkmpxwcpr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.yfazqb.com/Article/details/gkadrcznt.sHtML

TS:   [...arr].reverse();
来源：http://3g.yfazqb.com/Article/details/gpgijmzsj.sHtML

Java: Collections.reverse(list);
来源：http://3g.sjlbkw.cn/Article/details/gkbqhhqej.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fktsv.cn/Article/details/gnuqwueml.sHtML

Ruby: arr.reverse
来源：http://www.blog.tarul.cn/Article/details/gieofpakk.sHtML

C#:   list.Reverse();
来源：http://m.share.tarul.cn/Article/details/gcgtcfbrh.sHtML

[D12] 查找元素下标
来源：http://wap.fktsv.cn/Article/details/gvamnxtgg.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fktsv.cn/Article/details/gqoulkxil.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.epnwcf.com/Article/details/gycjtsriy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/gyxsxzjgd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gldhmxcza.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.epnwcf.com/Article/details/gjxhcjwpl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gqjzsrqxh.sHtML


<!-- 参考信息 -->