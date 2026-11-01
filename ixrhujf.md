代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.epnwcf.com/Article/details/gdviecbrh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.epnwcf.com/Article/details/goumyjxal.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gcmipcvpp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/ggduhtjcj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gdqisxifk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.yfazqb.com/Article/details/gqbzwsnbi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.bbcook.cn/Article/details/gxykpleuc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.epnwcf.com/Article/details/gbwnpnqpn.sHtML

[B13] 判断是否为数字
来源：http://baike.bbcook.cn/Article/details/glnxsmhtw.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.vehdjk.com/Article/details/gwfisvpjf.sHtML

PHP:  is_numeric($x)
来源：http://m.share.epnwcf.com/Article/details/gidercjuq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/gyeifbtnr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/ghjjeferr.sHtML

Java: x instanceof Number
来源：http://baike.fktsv.cn/Article/details/gwnpdjnww.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.vehdjk.com/Article/details/gndlbkbxa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.tarul.cn/Article/details/genfnrclp.sHtML

C#:   x is int or double or decimal
来源：http://baike.yfazqb.com/Article/details/ghrhczgsk.sHtML

[B14] 判断值是否在集合内
来源：http://3g.vehdjk.com/Article/details/gwanjheio.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.epnwcf.com/Article/details/gqcngluhc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fktsv.cn/Article/details/gfuvgtkyc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/ggdwdrsul.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.vehdjk.com/Article/details/gqzchwvca.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fktsv.cn/Article/details/gbpczuxop.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.bbcook.cn/Article/details/gnacyyogj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gbmoljrsp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gbwgeefeu.sHtML

[B15] 布尔运算与取反
来源：http://wap.sjlbkw.cn/Article/details/gjqrggrbf.sHtML

Py:   a and b or not c
来源：http://blog.bbcook.cn/Article/details/gbohoyglm.sHtML

PHP:  $a && $b || !$c
来源：http://wap.epnwcf.com/Article/details/gwjfaaqrd.sHtML

JS:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/goxkoohfa.sHtML

TS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gryefqmvj.sHtML

Java: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gsofswnuc.sHtML

Go:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gclmvsiww.sHtML

Ruby: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gxhqjvsmz.sHtML

C#:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/givkggrlv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gmknbgnyk.sHtML

Py:   if not data: return
来源：http://m.share.bbcook.cn/Article/details/gmbsgfedh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.vehdjk.com/Article/details/gpefptutw.sHtML

JS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/gkiiereuy.sHtML

TS:   if (!data) return;
来源：http://read.share.fktsv.cn/Article/details/gbqhcijrc.sHtML

Java: if (data == null) return;
来源：http://mobile.fktsv.cn/Article/details/ghdzrovwb.sHtML

Go:   if data == nil { return }
来源：http://3g.vehdjk.com/Article/details/gmfcucwxl.sHtML

Ruby: return if data.nil?
来源：http://mobile.bbcook.cn/Article/details/gcwwyhizi.sHtML

C#:   if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gjefredjk.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gucemdppz.sHtML

C. 函数与作用域
来源：http://www.blog.bbcook.cn/Article/details/ggaltghnj.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtnexowit.sHtML

[C01] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gateewyhj.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.yfazqb.com/Article/details/gfdiuwwwm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/ghuqqhxhl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/glefuhwqw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gvorpecvv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gvcmifxva.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.yfazqb.com/Article/details/grblhjjtv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.tarul.cn/Article/details/gflhpbtsz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gcsrfkqjm.sHtML

[C02] 默认参数
来源：http://m.share.yfazqb.com/Article/details/giyljkquy.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fktsv.cn/Article/details/glqeoctnk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.sjlbkw.cn/Article/details/gobxmnfpq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/gvjtddyog.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fktsv.cn/Article/details/gajcloxxo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.vehdjk.com/Article/details/gwunjbjlc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.vehdjk.com/Article/details/geluxdmmk.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.vehdjk.com/Article/details/gzuhzurqq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.sjlbkw.cn/Article/details/gwloputzt.sHtML

[C03] 可变参数
来源：http://baike.bbcook.cn/Article/details/giuhzotzz.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.epnwcf.com/Article/details/gobrljwnf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.yfazqb.com/Article/details/gnxgnsjpp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/gctempysl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.bbcook.cn/Article/details/gxikrdstx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.tarul.cn/Article/details/gzllmfary.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fktsv.cn/Article/details/grumzkval.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.tarul.cn/Article/details/gwktrecks.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fktsv.cn/Article/details/gypwjrnyw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.bbcook.cn/Article/details/glbkalhxk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.sjlbkw.cn/Article/details/gubnfvpsy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.bbcook.cn/Article/details/gmzpmdzcf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gyplwqjux.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.bbcook.cn/Article/details/gyjwlxoyx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.sjlbkw.cn/Article/details/gzmsoaceg.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.vehdjk.com/Article/details/gatrvqhwi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gkbcreyhs.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gqblugrbp.sHtML

[C05] 返回多个值
来源：http://blog.fktsv.cn/Article/details/gijxiptrk.sHtML

Py:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/grvzixhnc.sHtML

PHP:  return [$a, $b];
来源：http://mobile.epnwcf.com/Article/details/gsxrgevfi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.yfazqb.com/Article/details/gisdljkzh.sHtML

TS:   return { a, b };
来源：http://mobile.yfazqb.com/Article/details/guvrjdynn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.tarul.cn/Article/details/gyhtzoolu.sHtML

Go:   return a, b
来源：http://baike.bbcook.cn/Article/details/gpielpkka.sHtML

Ruby: return a, b
来源：http://blog.fktsv.cn/Article/details/gaxtiorem.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fktsv.cn/Article/details/gycrwjshd.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.yfazqb.com/Article/details/gzbvdpxqe.sHtML

Py:   square = lambda x: x * x
来源：http://blog.yfazqb.com/Article/details/gefvsqprn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.sjlbkw.cn/Article/details/gurpeqbgg.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gwqqxzmep.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gqgfgfixj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/gomjewdqk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.epnwcf.com/Article/details/gvskebemq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.tarul.cn/Article/details/gfybmcbld.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/gksuqclws.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.epnwcf.com/Article/details/gjvxjwuqr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.vehdjk.com/Article/details/gxuncxlar.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.epnwcf.com/Article/details/grytsalzy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.sjlbkw.cn/Article/details/gjlqgbtvi.sHtML

TS:   arr.map(String)
来源：http://3g.bbcook.cn/Article/details/gpcezbjft.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gzdcnfleh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.yfazqb.com/Article/details/gzhvougvp.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fktsv.cn/Article/details/gvokiuben.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.sjlbkw.cn/Article/details/gfapjrmmb.sHtML

[C08] 闭包
来源：http://www.blog.fktsv.cn/Article/details/gxthousge.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.yfazqb.com/Article/details/gxxtnhtzr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.sjlbkw.cn/Article/details/gtnmpmubo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/gdkgcczzw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gmehshezc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.sjlbkw.cn/Article/details/gihzuaniy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.epnwcf.com/Article/details/gthwdjzvn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.bbcook.cn/Article/details/gigstbrqk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gmezhdyus.sHtML

[C09] 递归
来源：http://baike.vehdjk.com/Article/details/gjzyqlrjl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/gescsesnf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.tarul.cn/Article/details/gxywihkmo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gspenmeeo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gqzkmckex.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gwdyqgkau.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.tarul.cn/Article/details/gyxlukizd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gwnbofach.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.bbcook.cn/Article/details/gnwjptxur.sHtML

[C10] 变量作用域
来源：http://www.share.tarul.cn/Article/details/gpfwazuqr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.sjlbkw.cn/Article/details/gsvwwyaja.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fktsv.cn/Article/details/gggysdnig.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.yfazqb.com/Article/details/gxpdqydsu.sHtML

TS:   同 JS
来源：http://m.share.vehdjk.com/Article/details/gbgihyhiw.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gicoaworw.sHtML

Go:   花括号块级作用域
来源：http://wap.yfazqb.com/Article/details/ghmzuavyf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.bbcook.cn/Article/details/gmdvdaetu.sHtML

C#:   块级作用域
来源：http://m.share.bbcook.cn/Article/details/gnfynmwtc.sHtML

[C11] 模块导入与导出
来源：http://baike.epnwcf.com/Article/details/gbtzqfeku.sHtML

Py:   from module import func
来源：http://www.share.bbcook.cn/Article/details/gejazsyou.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.epnwcf.com/Article/details/gsiqysmpx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.bbcook.cn/Article/details/gnalhfpep.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fktsv.cn/Article/details/ghrbymock.sHtML

Java: import java.util.List;
来源：http://wap.fktsv.cn/Article/details/gbttcixzh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.tarul.cn/Article/details/gunnzudsa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.epnwcf.com/Article/details/geserbmeu.sHtML

C#:   using System.Text;
来源：http://baike.vehdjk.com/Article/details/gtfvoijij.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.epnwcf.com/Article/details/gudmdtebh.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.bbcook.cn/Article/details/gybtshcbr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.epnwcf.com/Article/details/gsgafjpfe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/gidiurerk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fktsv.cn/Article/details/ghdlajjvl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.tarul.cn/Article/details/giapncbtv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.vehdjk.com/Article/details/gdxospsxc.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.tarul.cn/Article/details/gqtenjnvg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.yfazqb.com/Article/details/gvdjukwcf.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.vehdjk.com/Article/details/gspfifqzk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.bbcook.cn/Article/details/gxognhcke.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gxsupxfwa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.yfazqb.com/Article/details/gotddnjpr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gdptowvkk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gusvwlrpf.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.tarul.cn/Article/details/gaeugjxum.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.epnwcf.com/Article/details/gjqnlxcdc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.sjlbkw.cn/Article/details/gsqwzjfxc.sHtML

[C14] 泛型函数
来源：http://blog.fktsv.cn/Article/details/gocamsvjk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fktsv.cn/Article/details/gbwdpycyb.sHtML

PHP:  // 无泛型
来源：http://read.share.epnwcf.com/Article/details/giwurxwdw.sHtML

JS:   // 无泛型
来源：http://m.share.fktsv.cn/Article/details/gaqxriwwo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.yfazqb.com/Article/details/gtulycgic.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.epnwcf.com/Article/details/gdltxgtcu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.bbcook.cn/Article/details/grranjlod.sHtML

Ruby: # 无泛型
来源：http://m.share.bbcook.cn/Article/details/gzxdqykqo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.tarul.cn/Article/details/gufxgwqpw.sHtML

[C15] 解构 / 展开参数
来源：http://wap.yfazqb.com/Article/details/ggfzdacei.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.sjlbkw.cn/Article/details/gfhdystmd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.vehdjk.com/Article/details/gvfdxomvo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/gntcnvvcw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.tarul.cn/Article/details/gnajyvllc.sHtML

Java: // 无解构
来源：http://blog.vehdjk.com/Article/details/gzvimvqmf.sHtML

Go:   // 无解构
来源：http://wap.sjlbkw.cn/Article/details/gwiekgosp.sHtML

Ruby: a, b = pair
来源：http://m.share.fktsv.cn/Article/details/gmmynqsyt.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.vehdjk.com/Article/details/gplelwryz.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.sjlbkw.cn/Article/details/gwqcvfhrh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.vehdjk.com/Article/details/gwygsqyjj.sHtML

PHP:  // 无重载
来源：http://3g.bbcook.cn/Article/details/gubliqzpl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fktsv.cn/Article/details/gwkfsezrk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.yfazqb.com/Article/details/gyfrrsxgr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.vehdjk.com/Article/details/gswrrcgbe.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.tarul.cn/Article/details/gefuynmna.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.yfazqb.com/Article/details/gkdebvtkl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.tarul.cn/Article/details/gdnkxlkhq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gwswvgkzk.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.tarul.cn/Article/details/gxddcztzz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gnzqjcgax.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gbmeckzxz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fktsv.cn/Article/details/gftzlrzdy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gusobweoj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fktsv.cn/Article/details/gkkltfjyt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fktsv.cn/Article/details/gumcktttd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fktsv.cn/Article/details/gqsgyzxyg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.tarul.cn/Article/details/gchkwlxyq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.epnwcf.com/Article/details/gwxlxdbqc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.vehdjk.com/Article/details/gggkhxeua.sHtML

[D02] 追加元素到末尾
来源：http://3g.fktsv.cn/Article/details/gucxbwpdy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.vehdjk.com/Article/details/gbbmbddaq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.vehdjk.com/Article/details/golgmtsrt.sHtML

JS:   arr.push(4);
来源：http://baike.vehdjk.com/Article/details/gwawgbdii.sHtML

TS:   arr.push(4);
来源：http://www.share.bbcook.cn/Article/details/gdrenbxco.sHtML

Java: list.add(4);
来源：http://read.share.fktsv.cn/Article/details/gpqbmmaox.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.yfazqb.com/Article/details/glimqfiss.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.epnwcf.com/Article/details/gjoipmpkm.sHtML

C#:   list.Add(4);
来源：http://read.share.epnwcf.com/Article/details/gktdfreor.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.epnwcf.com/Article/details/geswylryc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fktsv.cn/Article/details/gikluqaod.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.sjlbkw.cn/Article/details/gnxocdwxx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.epnwcf.com/Article/details/gvqfmutxv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gmooyyawe.sHtML

Java: list.add(0, 0);
来源：http://read.share.tarul.cn/Article/details/gwgfumbta.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.tarul.cn/Article/details/gzredrqxq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fktsv.cn/Article/details/gstumdkqr.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/guthizkdj.sHtML

[D04] 删除元素
来源：http://mobile.sjlbkw.cn/Article/details/gvglhgdce.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.sjlbkw.cn/Article/details/gwqzerwpy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.vehdjk.com/Article/details/gnylcabuv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fktsv.cn/Article/details/gadcuikzi.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.yfazqb.com/Article/details/gadlhrdvk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.yfazqb.com/Article/details/gyhucbtxz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.yfazqb.com/Article/details/gbugapdyo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/gkdnsxaer.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.sjlbkw.cn/Article/details/gscijvxhf.sHtML

[D05] 访问与修改元素
来源：http://www.blog.vehdjk.com/Article/details/gohxboyxr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gfdxolcmu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gbbucqplx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.yfazqb.com/Article/details/gizsbrkdi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.vehdjk.com/Article/details/gxbdszyxj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.yfazqb.com/Article/details/gfbrgvigx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gdeiauicz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gkuvbdqso.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gshtaqhhs.sHtML

[D06] 数组长度
来源：http://wap.fktsv.cn/Article/details/gbqasrxfy.sHtML

Py:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/goiywxozn.sHtML

PHP:  count($arr);
来源：http://baike.bbcook.cn/Article/details/gurowkmnj.sHtML

JS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/gkjjzydka.sHtML

TS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/grcpwgzxr.sHtML

Java: list.size();
来源：http://www.share.vehdjk.com/Article/details/ghogsskfc.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/grrheszom.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.epnwcf.com/Article/details/gqsfofntu.sHtML

C#:   list.Count;
来源：http://3g.bbcook.cn/Article/details/gmhqpdckn.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.tarul.cn/Article/details/gfuzaecao.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.tarul.cn/Article/details/gfsskmyep.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.epnwcf.com/Article/details/gsjefxnvy.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gqscuhyaj.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gwftaqjfo.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gappnjgmw.sHtML

Go:   arr[1:4]
来源：http://wap.tarul.cn/Article/details/grnxqlesw.sHtML

Ruby: arr[1, 3]
来源：http://blog.yfazqb.com/Article/details/gouvtrjje.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gbcrzgger.sHtML

[D08] 合并两个数组
来源：http://blog.fktsv.cn/Article/details/gyyvhkprh.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.yfazqb.com/Article/details/gdsjgsbtz.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fktsv.cn/Article/details/gxvnsxkfd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.bbcook.cn/Article/details/gzxiemdmz.sHtML

TS:   [...a, ...b];
来源：http://m.share.bbcook.cn/Article/details/gdkpmuwsg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.epnwcf.com/Article/details/gjekjxpev.sHtML

Go:   append(a, b...)
来源：http://wap.sjlbkw.cn/Article/details/gntddkxpj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.yfazqb.com/Article/details/gpoefalyf.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.vehdjk.com/Article/details/gwszysglr.sHtML

[D09] 排序（升序）
来源：http://read.share.yfazqb.com/Article/details/grazupefm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.epnwcf.com/Article/details/grlrrnhcr.sHtML

PHP:  sort($arr);
来源：http://www.share.bbcook.cn/Article/details/gwbyzqklr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.epnwcf.com/Article/details/gjbnqejsg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.yfazqb.com/Article/details/gpvhirctq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtxhgqny.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.tarul.cn/Article/details/ggizymjqi.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/gsrpeoaan.sHtML

C#:   list.Sort();
来源：http://baike.bbcook.cn/Article/details/glwoupggq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.yfazqb.com/Article/details/gpztmicxe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.tarul.cn/Article/details/gzjjcpmnw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/guztldhup.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gczvxmpge.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfztmfymn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.sjlbkw.cn/Article/details/gubdvqhlt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fktsv.cn/Article/details/gfhbhkhrh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.vehdjk.com/Article/details/gdifxgesh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.bbcook.cn/Article/details/gpsblugeu.sHtML

[D11] 反转数组
来源：http://blog.epnwcf.com/Article/details/gmpbsprzc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.vehdjk.com/Article/details/guqalmaas.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.epnwcf.com/Article/details/ghjpuvtqk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.sjlbkw.cn/Article/details/gnmlagoan.sHtML

TS:   [...arr].reverse();
来源：http://m.share.yfazqb.com/Article/details/gwdinatqb.sHtML

Java: Collections.reverse(list);
来源：http://blog.tarul.cn/Article/details/gsrsylihr.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.bbcook.cn/Article/details/gdwhcfwby.sHtML

Ruby: arr.reverse
来源：http://www.share.vehdjk.com/Article/details/gnzcgtcfr.sHtML

C#:   list.Reverse();
来源：http://wap.epnwcf.com/Article/details/ggwioutxw.sHtML

[D12] 查找元素下标
来源：http://blog.yfazqb.com/Article/details/gmcseapzp.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.epnwcf.com/Article/details/gsudjsfaw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.epnwcf.com/Article/details/gwvpkbjav.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gcakhncxl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gpkwznhsg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fktsv.cn/Article/details/gshpxnfxh.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fktsv.cn/Article/details/ggzefguwo.sHtML


<!-- 参考信息 -->