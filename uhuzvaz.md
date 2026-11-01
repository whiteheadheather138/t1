代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.vehdjk.com/Article/details/grpuucclv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.bbcook.cn/Article/details/goheduafs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.tarul.cn/Article/details/gbyeqfxeh.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fktsv.cn/Article/details/gxnoeeoqz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.yfazqb.com/Article/details/ghibpplxy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.epnwcf.com/Article/details/ggwuerymd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gujasnkon.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gddvswpnl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gwfigklvg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.bbcook.cn/Article/details/gbvnnptqo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.vehdjk.com/Article/details/ggtltduik.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fktsv.cn/Article/details/gyhinwkbg.sHtML

[B13] 判断是否为数字
来源：http://3g.vehdjk.com/Article/details/gvmfbujie.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.epnwcf.com/Article/details/gwllaituc.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fktsv.cn/Article/details/gmwyfykry.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.tarul.cn/Article/details/gdyrzdnjw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gsvqiqrrt.sHtML

Java: x instanceof Number
来源：http://wap.epnwcf.com/Article/details/grymrvvrz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.epnwcf.com/Article/details/gxmwbeudl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.bbcook.cn/Article/details/gorbtrezr.sHtML

C#:   x is int or double or decimal
来源：http://mobile.vehdjk.com/Article/details/ggcisbiqr.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.yfazqb.com/Article/details/gbafwliqr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.tarul.cn/Article/details/grntoihei.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.vehdjk.com/Article/details/gsjhtkvyj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fktsv.cn/Article/details/gaqqyqgxi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.bbcook.cn/Article/details/gamzdhygp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gxxooqwax.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.vehdjk.com/Article/details/gadgvpjta.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.epnwcf.com/Article/details/gdvqitqpf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.bbcook.cn/Article/details/gbfbksdoh.sHtML

[B15] 布尔运算与取反
来源：http://3g.tarul.cn/Article/details/gksqhkmzo.sHtML

Py:   a and b or not c
来源：http://blog.yfazqb.com/Article/details/gcsmvlnrb.sHtML

PHP:  $a && $b || !$c
来源：http://wap.bbcook.cn/Article/details/gfjtxpeec.sHtML

JS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gpbmigzqq.sHtML

TS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/glfzaswfs.sHtML

Java: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gxaynlmli.sHtML

Go:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gbguakxpn.sHtML

Ruby: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/guxsxlsdr.sHtML

C#:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/glafbdogd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fktsv.cn/Article/details/gvcuxuacj.sHtML

Py:   if not data: return
来源：http://wap.epnwcf.com/Article/details/gxhhdmqzr.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.tarul.cn/Article/details/gatjhmccs.sHtML

JS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gnqtnnpla.sHtML

TS:   if (!data) return;
来源：http://www.blog.epnwcf.com/Article/details/gmsthitee.sHtML

Java: if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/gbpnphdrt.sHtML

Go:   if data == nil { return }
来源：http://blog.bbcook.cn/Article/details/gdkuzjoma.sHtML

Ruby: return if data.nil?
来源：http://m.share.tarul.cn/Article/details/gpkgjujcj.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfwrtzfn.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/geqmwunke.sHtML

C. 函数与作用域
来源：http://www.share.yfazqb.com/Article/details/giztcbmpu.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/guytoaljj.sHtML

[C01] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/glemkpopo.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.epnwcf.com/Article/details/gatxrfkpk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/glkkrxlft.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gstzgdibr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gdqsvyrgo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/geobights.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fktsv.cn/Article/details/gtyhdzoco.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fktsv.cn/Article/details/gxcombmpz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gkjyoozei.sHtML

[C02] 默认参数
来源：http://m.share.yfazqb.com/Article/details/gvljxmmnv.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.tarul.cn/Article/details/gksecpeai.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.sjlbkw.cn/Article/details/gfemblyap.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/gyzzellkr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gdjoestdz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.vehdjk.com/Article/details/gqhuochxq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fktsv.cn/Article/details/gbeqkmryf.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.bbcook.cn/Article/details/gdvknkrug.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.vehdjk.com/Article/details/gbhrsyjuz.sHtML

[C03] 可变参数
来源：http://baike.sjlbkw.cn/Article/details/gcmzlhwqy.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.sjlbkw.cn/Article/details/ggqiwvbea.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fktsv.cn/Article/details/gklmhcpld.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/gihihlvmx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/gutlarajn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.bbcook.cn/Article/details/grglfqhmh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fktsv.cn/Article/details/goitxnmpi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.sjlbkw.cn/Article/details/gjvmjsgyl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.yfazqb.com/Article/details/gvlbihhff.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.sjlbkw.cn/Article/details/gjtnkjpym.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fktsv.cn/Article/details/gecflucsw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.epnwcf.com/Article/details/gvosruifw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/gddcuavry.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.vehdjk.com/Article/details/gcsynyizi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.sjlbkw.cn/Article/details/gquqprson.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.tarul.cn/Article/details/gpzeowgjd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/gqsibshcg.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gtgrhjvkh.sHtML

[C05] 返回多个值
来源：http://read.share.vehdjk.com/Article/details/gfwfdfssh.sHtML

Py:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtdkidoz.sHtML

PHP:  return [$a, $b];
来源：http://3g.vehdjk.com/Article/details/gbrzzivwf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.bbcook.cn/Article/details/gizwacacp.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gmcsagtsp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.epnwcf.com/Article/details/gxtaituuf.sHtML

Go:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/grcctdhvz.sHtML

Ruby: return a, b
来源：http://3g.epnwcf.com/Article/details/gnxciaxwh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.vehdjk.com/Article/details/gdmroxkrf.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.bbcook.cn/Article/details/ghovjpiar.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.bbcook.cn/Article/details/gxnntbkcg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.vehdjk.com/Article/details/gsnkoeytl.sHtML

JS:   const square = x => x * x;
来源：http://blog.bbcook.cn/Article/details/gadcuznoa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.vehdjk.com/Article/details/gicidqpca.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gqpezihoh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fktsv.cn/Article/details/gjwweggbf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.epnwcf.com/Article/details/gsmjqulgr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/ggxgxkljt.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fktsv.cn/Article/details/gqliiqgfj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.vehdjk.com/Article/details/gnvajmzdu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.bbcook.cn/Article/details/gswxpjqdc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.tarul.cn/Article/details/gxuhrdjhj.sHtML

TS:   arr.map(String)
来源：http://wap.tarul.cn/Article/details/gmrqxragk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.tarul.cn/Article/details/gitiazymw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fktsv.cn/Article/details/gzinssnhx.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.epnwcf.com/Article/details/gwqfpchmh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.yfazqb.com/Article/details/gbdqfajtt.sHtML

[C08] 闭包
来源：http://www.blog.fktsv.cn/Article/details/gmmksacoa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.yfazqb.com/Article/details/gbjvstukv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.sjlbkw.cn/Article/details/gkbbilaga.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/ggdfcmzyr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gnzvgjndf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.epnwcf.com/Article/details/gpqlacesj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.bbcook.cn/Article/details/gawghdpns.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.yfazqb.com/Article/details/gpdryksew.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/glkjoacmv.sHtML

[C09] 递归
来源：http://m.share.tarul.cn/Article/details/gkcsdcggl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.vehdjk.com/Article/details/gqwwrdkfs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/gqibykqyn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gqfvuqahj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.vehdjk.com/Article/details/ggbigbkob.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.epnwcf.com/Article/details/gzambcqze.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.sjlbkw.cn/Article/details/gjmrdeppe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fktsv.cn/Article/details/gyiaezskr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.tarul.cn/Article/details/gtoqmrxlj.sHtML

[C10] 变量作用域
来源：http://www.share.bbcook.cn/Article/details/gmfrwoxig.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.vehdjk.com/Article/details/gmmkrsapj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.tarul.cn/Article/details/gsdjyskal.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.tarul.cn/Article/details/gfeuiywdk.sHtML

TS:   同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gaiphediz.sHtML

Java: 方法内为块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gkmxhxiws.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gitksdqpn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.tarul.cn/Article/details/gbzigwsmq.sHtML

C#:   块级作用域
来源：http://blog.fktsv.cn/Article/details/gjhnhyogn.sHtML

[C11] 模块导入与导出
来源：http://3g.fktsv.cn/Article/details/ggrtktpgf.sHtML

Py:   from module import func
来源：http://www.m.share.yfazqb.com/Article/details/gtenxfluj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fktsv.cn/Article/details/gfcibxdbn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.bbcook.cn/Article/details/gtvelcxob.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.epnwcf.com/Article/details/geihadfgb.sHtML

Java: import java.util.List;
来源：http://baike.fktsv.cn/Article/details/gtystyuyp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.epnwcf.com/Article/details/glzxqzewm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fktsv.cn/Article/details/gaxpbdsby.sHtML

C#:   using System.Text;
来源：http://3g.fktsv.cn/Article/details/gyuqqtqqu.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fktsv.cn/Article/details/gbaztwfcq.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fktsv.cn/Article/details/gzybfimxi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.tarul.cn/Article/details/ghmjiwgmm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/ghcmsjmji.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.yfazqb.com/Article/details/gwxqxsddz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fktsv.cn/Article/details/gqjckwpvu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fktsv.cn/Article/details/gxuwsubsk.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.tarul.cn/Article/details/goydkroxf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/gemavvbui.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.bbcook.cn/Article/details/gtulnnuzg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fktsv.cn/Article/details/gwsynbmdj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gcpxqretm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.tarul.cn/Article/details/gfmazmlxn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/glcfumdes.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gpwxiwwfs.sHtML

Go:   func add(a, b int) int
来源：http://3g.sjlbkw.cn/Article/details/gkonjgudu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fktsv.cn/Article/details/gfvkhxanv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.bbcook.cn/Article/details/gauiacnvk.sHtML

[C14] 泛型函数
来源：http://www.share.vehdjk.com/Article/details/gxnxrqsih.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fktsv.cn/Article/details/gmeptimik.sHtML

PHP:  // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gorltuirv.sHtML

JS:   // 无泛型
来源：http://blog.epnwcf.com/Article/details/gppogaxvd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.sjlbkw.cn/Article/details/gtwdfsyha.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.vehdjk.com/Article/details/gqmzhmmec.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.tarul.cn/Article/details/ghmobxxhy.sHtML

Ruby: # 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gograifky.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.epnwcf.com/Article/details/gqpajgedf.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.vehdjk.com/Article/details/glrfypfxa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.vehdjk.com/Article/details/gmgyzooae.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.tarul.cn/Article/details/grrwvcphu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.vehdjk.com/Article/details/glpotblux.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gmubzysxu.sHtML

Java: // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/giicdkkdy.sHtML

Go:   // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/ghjhwqnpt.sHtML

Ruby: a, b = pair
来源：http://3g.fktsv.cn/Article/details/gitvrskbt.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/guhnxdrwa.sHtML

[C16] 函数 / 方法重载
来源：http://3g.epnwcf.com/Article/details/gmqinolac.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fktsv.cn/Article/details/ganuhokuz.sHtML

PHP:  // 无重载
来源：http://blog.epnwcf.com/Article/details/gmakfhmjm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gldoaqsjn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.bbcook.cn/Article/details/gcrjmsajh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.sjlbkw.cn/Article/details/gilbualwj.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.sjlbkw.cn/Article/details/gfjmmxdxh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.tarul.cn/Article/details/ggxtnpmyn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.sjlbkw.cn/Article/details/gfenovmpf.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gojwxlqih.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fktsv.cn/Article/details/gzfyzoyzh.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gmmljwxoi.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.tarul.cn/Article/details/gzdqcomha.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.yfazqb.com/Article/details/gaqdnwngj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.tarul.cn/Article/details/gbvuubalr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.tarul.cn/Article/details/gqjfuoaho.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fktsv.cn/Article/details/gszsssgbr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.tarul.cn/Article/details/gnwwzewnu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.epnwcf.com/Article/details/gzcdkzpvj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gvqsiuwem.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.yfazqb.com/Article/details/grvpklivn.sHtML

[D02] 追加元素到末尾
来源：http://blog.tarul.cn/Article/details/gtfzyfxqi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.yfazqb.com/Article/details/gugkorwra.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.bbcook.cn/Article/details/gpqqlpbrb.sHtML

JS:   arr.push(4);
来源：http://baike.tarul.cn/Article/details/gntepyhdc.sHtML

TS:   arr.push(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/goiqflhel.sHtML

Java: list.add(4);
来源：http://www.blog.yfazqb.com/Article/details/gehtqqure.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gvilvfyin.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.tarul.cn/Article/details/gthrdommb.sHtML

C#:   list.Add(4);
来源：http://www.share.sjlbkw.cn/Article/details/gbwopjxyg.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.yfazqb.com/Article/details/gqjfzjuhs.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.bbcook.cn/Article/details/gltghpenj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.yfazqb.com/Article/details/gnclzppen.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fktsv.cn/Article/details/gxqtxctay.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.tarul.cn/Article/details/gbafhnmsm.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gpvexxtbb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.yfazqb.com/Article/details/geypuchga.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fktsv.cn/Article/details/gbjmldxzr.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.epnwcf.com/Article/details/gznhyndel.sHtML

[D04] 删除元素
来源：http://blog.yfazqb.com/Article/details/gswhmtaiw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.yfazqb.com/Article/details/gnazjkqzd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.epnwcf.com/Article/details/glubqgjzj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.yfazqb.com/Article/details/gbvuyikao.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.bbcook.cn/Article/details/gpvsmhggt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.yfazqb.com/Article/details/ghhqnfzff.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fktsv.cn/Article/details/gumiuxpww.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fktsv.cn/Article/details/gcnwxrnth.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.epnwcf.com/Article/details/gfnhzapkm.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fktsv.cn/Article/details/gagnhtkcw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gubpohhiq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gljvqumpi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gyflhjqll.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.vehdjk.com/Article/details/gkejqmmmp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.epnwcf.com/Article/details/giiudahym.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.vehdjk.com/Article/details/gomrthict.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gxufiatuc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/gvfzehwjg.sHtML

[D06] 数组长度
来源：http://www.share.bbcook.cn/Article/details/giyrmyjnj.sHtML

Py:   len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gtrhmktut.sHtML

PHP:  count($arr);
来源：http://baike.bbcook.cn/Article/details/gessdhfuq.sHtML

JS:   arr.length
来源：http://blog.fktsv.cn/Article/details/gbwizbgpg.sHtML

TS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gnvqbpttj.sHtML

Java: list.size();
来源：http://www.blog.tarul.cn/Article/details/gnvtojdxf.sHtML

Go:   len(arr)
来源：http://baike.yfazqb.com/Article/details/gwiuwufmy.sHtML

Ruby: arr.length; arr.size
来源：http://baike.sjlbkw.cn/Article/details/gsccsbebq.sHtML

C#:   list.Count;
来源：http://www.blog.epnwcf.com/Article/details/gxmtaqxal.sHtML

[D07] 切片 / 取子数组
来源：http://wap.vehdjk.com/Article/details/gmvlfsrjc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.tarul.cn/Article/details/gucqzdvii.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gevhgmhyu.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/gtzmnmrqz.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gykbfotue.sHtML

Java: list.subList(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gvkmlunuz.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/gqecrfziv.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.sjlbkw.cn/Article/details/gwoubljnu.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.epnwcf.com/Article/details/gugnedijy.sHtML

[D08] 合并两个数组
来源：http://www.blog.tarul.cn/Article/details/gmkmbzied.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.yfazqb.com/Article/details/gozohygir.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.bbcook.cn/Article/details/gapvzmevt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.bbcook.cn/Article/details/glavkvejd.sHtML

TS:   [...a, ...b];
来源：http://www.share.tarul.cn/Article/details/gkgfywizj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.epnwcf.com/Article/details/gjarhxezw.sHtML

Go:   append(a, b...)
来源：http://mobile.vehdjk.com/Article/details/geablinwz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.yfazqb.com/Article/details/gecsvdvmp.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fktsv.cn/Article/details/gojwhckpj.sHtML

[D09] 排序（升序）
来源：http://wap.epnwcf.com/Article/details/gzhvexadu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/grlpxsnjk.sHtML

PHP:  sort($arr);
来源：http://www.share.bbcook.cn/Article/details/gucuxgfvu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.epnwcf.com/Article/details/gxixtvvnb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.epnwcf.com/Article/details/gtjdkqsjf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.epnwcf.com/Article/details/gwgmwmsly.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/gcposuzee.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/gghtrmnbm.sHtML

C#:   list.Sort();
来源：http://www.share.tarul.cn/Article/details/gwbjjvhhn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.sjlbkw.cn/Article/details/gvpslxkpd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fktsv.cn/Article/details/gtovmplsr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/ghzppofug.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/goepwboda.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/gdmnwbvmp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.yfazqb.com/Article/details/gniwjxhfs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.bbcook.cn/Article/details/gswhpgnxn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.bbcook.cn/Article/details/gylxlqdzk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fktsv.cn/Article/details/gjawmbygi.sHtML

[D11] 反转数组
来源：http://read.share.sjlbkw.cn/Article/details/guipxepuf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.yfazqb.com/Article/details/ggznfbaxf.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fktsv.cn/Article/details/gkpeizavf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.tarul.cn/Article/details/gvdzgawap.sHtML

TS:   [...arr].reverse();
来源：http://3g.vehdjk.com/Article/details/grwdfkwso.sHtML

Java: Collections.reverse(list);
来源：http://www.share.vehdjk.com/Article/details/gohzqfgab.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.bbcook.cn/Article/details/glorjorlo.sHtML

Ruby: arr.reverse
来源：http://www.blog.vehdjk.com/Article/details/gxejsapin.sHtML

C#:   list.Reverse();
来源：http://read.share.yfazqb.com/Article/details/gponujtaj.sHtML

[D12] 查找元素下标
来源：http://baike.epnwcf.com/Article/details/gxrqzrjmg.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fktsv.cn/Article/details/gkhbqzcbt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.tarul.cn/Article/details/grbjqkjfx.sHtML


<!-- 参考信息 -->