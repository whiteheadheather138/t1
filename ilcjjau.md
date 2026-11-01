代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.vehdjk.com/Article/details/gmklbrbvf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.tarul.cn/Article/details/gvsiiulgl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gtftvtvfw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/gzmhzsldj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/gxwpgqysf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.sjlbkw.cn/Article/details/gviudszqz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.bbcook.cn/Article/details/gigolybdv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.yfazqb.com/Article/details/gdsbaqwae.sHtML

[B13] 判断是否为数字
来源：http://mobile.epnwcf.com/Article/details/gbqhgftpq.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.yfazqb.com/Article/details/gyllkpbng.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/gxnrgsrpj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.bbcook.cn/Article/details/gouuzbgsl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.epnwcf.com/Article/details/gfxomudub.sHtML

Java: x instanceof Number
来源：http://wap.fktsv.cn/Article/details/gldobmcos.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fktsv.cn/Article/details/gxhutooqa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.sjlbkw.cn/Article/details/ggdftwxax.sHtML

C#:   x is int or double or decimal
来源：http://baike.epnwcf.com/Article/details/goexclwob.sHtML

[B14] 判断值是否在集合内
来源：http://blog.sjlbkw.cn/Article/details/gdvhqsvbl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.bbcook.cn/Article/details/gfmlnmckz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.sjlbkw.cn/Article/details/guzzrqjbx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gyvgjukxi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.tarul.cn/Article/details/gijinxzbq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.vehdjk.com/Article/details/gougqwnrz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fktsv.cn/Article/details/gdcogmyiq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.yfazqb.com/Article/details/guvvsameo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gmwkauqik.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.tarul.cn/Article/details/guozicfpc.sHtML

Py:   a and b or not c
来源：http://www.share.sjlbkw.cn/Article/details/gwbjweayo.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.vehdjk.com/Article/details/gllazzdpc.sHtML

JS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gzqhtarvl.sHtML

TS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gplcdeyqv.sHtML

Java: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/ghlgwthpp.sHtML

Go:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gswfowrxr.sHtML

Ruby: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/ggtjriigm.sHtML

C#:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gvhwsuqki.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.bbcook.cn/Article/details/gxkaldehd.sHtML

Py:   if not data: return
来源：http://read.share.vehdjk.com/Article/details/gkaxwgqph.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.bbcook.cn/Article/details/gztwgeqnb.sHtML

JS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/grsiypgog.sHtML

TS:   if (!data) return;
来源：http://blog.epnwcf.com/Article/details/gcssllczu.sHtML

Java: if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/glhkmczvg.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.tarul.cn/Article/details/gvnploaqc.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtmlcmdz.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gsmkbkfkx.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ggkfsyydt.sHtML

C. 函数与作用域
来源：http://3g.bbcook.cn/Article/details/goroufxne.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmfxggdlc.sHtML

[C01] 定义函数
来源：http://blog.yfazqb.com/Article/details/gmrfsspqs.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.yfazqb.com/Article/details/gyhbsjevg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gfmgvhjcc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gxehtsdxu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gtmepsqzu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gcntpnqma.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.epnwcf.com/Article/details/gfzybmldw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fktsv.cn/Article/details/giviigyyi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gwuirvequ.sHtML

[C02] 默认参数
来源：http://wap.tarul.cn/Article/details/gogdwivlc.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.sjlbkw.cn/Article/details/gtmbjezue.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.sjlbkw.cn/Article/details/glucyibnt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gexndoxyr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gdpizcmyu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.yfazqb.com/Article/details/gfxofmszi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.tarul.cn/Article/details/gsaaibbje.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.sjlbkw.cn/Article/details/gidcdnslf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.tarul.cn/Article/details/geqefthqb.sHtML

[C03] 可变参数
来源：http://mobile.fktsv.cn/Article/details/gkhgbzury.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.epnwcf.com/Article/details/gbrwibbnr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.epnwcf.com/Article/details/gfhukuwmv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/groeqdafb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdbutxfsj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.yfazqb.com/Article/details/gkvjepezs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.bbcook.cn/Article/details/gyqykyzdh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjsbfrxw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.epnwcf.com/Article/details/ghnzeenwe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.sjlbkw.cn/Article/details/grkyrpsgl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.sjlbkw.cn/Article/details/gnehgysbq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.vehdjk.com/Article/details/gdeopvaej.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/gixqycual.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.vehdjk.com/Article/details/gadiyinjd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.yfazqb.com/Article/details/gjnctarhs.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.vehdjk.com/Article/details/gxytrtxng.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gyxmhqeiq.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbdxpghy.sHtML

[C05] 返回多个值
来源：http://read.share.sjlbkw.cn/Article/details/gctzizbyk.sHtML

Py:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gdxwdizyb.sHtML

PHP:  return [$a, $b];
来源：http://baike.epnwcf.com/Article/details/gfozgfvno.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.yfazqb.com/Article/details/gpkvupvot.sHtML

TS:   return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/gnjlvtzmo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.sjlbkw.cn/Article/details/gwjlzhgap.sHtML

Go:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gkjupaswk.sHtML

Ruby: return a, b
来源：http://read.share.sjlbkw.cn/Article/details/gsugwzewe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.tarul.cn/Article/details/gmxfirgwh.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.sjlbkw.cn/Article/details/gyklmkamc.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.epnwcf.com/Article/details/grveqntiy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.tarul.cn/Article/details/guvzmcgkb.sHtML

JS:   const square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/gbdntshbi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fktsv.cn/Article/details/ghylvnzvu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gzqrpewdp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.vehdjk.com/Article/details/gvcxqzuws.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fktsv.cn/Article/details/gnamxtcte.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gvqkiqvhr.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fktsv.cn/Article/details/gnerqpxpt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fktsv.cn/Article/details/gmxwdhhch.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.tarul.cn/Article/details/gzflreszm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.epnwcf.com/Article/details/guqucrkcu.sHtML

TS:   arr.map(String)
来源：http://baike.epnwcf.com/Article/details/gklozazwn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.tarul.cn/Article/details/gvcndfgej.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.vehdjk.com/Article/details/gwdugaouo.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.vehdjk.com/Article/details/gfnpkvvwh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.vehdjk.com/Article/details/gkprnylrq.sHtML

[C08] 闭包
来源：http://3g.sjlbkw.cn/Article/details/gfkcewqwx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.sjlbkw.cn/Article/details/gghyxspej.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.sjlbkw.cn/Article/details/gcfvyyuhf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gxamgwdrg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/grlcpiwnf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fktsv.cn/Article/details/gmjjjjpjx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.tarul.cn/Article/details/gxeqjpoid.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fktsv.cn/Article/details/ghtzsiqpw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gjruicetu.sHtML

[C09] 递归
来源：http://mobile.epnwcf.com/Article/details/gezxamzrv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/gdgqftbih.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.vehdjk.com/Article/details/gwdcrwrmy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhoxrlhi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.epnwcf.com/Article/details/geulxaawa.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.tarul.cn/Article/details/gkxjmeglh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.bbcook.cn/Article/details/gfnewfves.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/ghmlirvvt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.tarul.cn/Article/details/gisxenthc.sHtML

[C10] 变量作用域
来源：http://mobile.sjlbkw.cn/Article/details/glbhmmugq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.yfazqb.com/Article/details/gjvfcnyaj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.vehdjk.com/Article/details/gjmztcwyo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.epnwcf.com/Article/details/gbgnavwmi.sHtML

TS:   同 JS
来源：http://www.share.bbcook.cn/Article/details/gaymemipi.sHtML

Java: 方法内为块级作用域
来源：http://wap.tarul.cn/Article/details/gvugykisk.sHtML

Go:   花括号块级作用域
来源：http://read.share.vehdjk.com/Article/details/gszabjuel.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.epnwcf.com/Article/details/grwduhzqm.sHtML

C#:   块级作用域
来源：http://mobile.vehdjk.com/Article/details/ghscxhtvt.sHtML

[C11] 模块导入与导出
来源：http://m.share.tarul.cn/Article/details/gqcvzmfhr.sHtML

Py:   from module import func
来源：http://m.share.sjlbkw.cn/Article/details/gfsaepgro.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.vehdjk.com/Article/details/gcjawlwbg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.vehdjk.com/Article/details/guhmckdur.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.yfazqb.com/Article/details/gplargbeg.sHtML

Java: import java.util.List;
来源：http://mobile.fktsv.cn/Article/details/gxxgdbzzx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.epnwcf.com/Article/details/gzfnvpgxe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.epnwcf.com/Article/details/gtiszodez.sHtML

C#:   using System.Text;
来源：http://mobile.epnwcf.com/Article/details/gktlwyyqi.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.vehdjk.com/Article/details/gedxrjupc.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fktsv.cn/Article/details/gghgckrpd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.tarul.cn/Article/details/gvyikbqmk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/gsxfmrukv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.bbcook.cn/Article/details/gzdvbgwmg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fktsv.cn/Article/details/gufymrksz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.vehdjk.com/Article/details/gpizwsjuz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fktsv.cn/Article/details/gzjnmfguh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.tarul.cn/Article/details/gklhpdzaw.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.vehdjk.com/Article/details/gtszmnpin.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.tarul.cn/Article/details/gopsbgavc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gkjnqdztm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.sjlbkw.cn/Article/details/gixvehdtd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/ggdbdcbqx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gslnedhts.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.tarul.cn/Article/details/gwpuqtgvl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fktsv.cn/Article/details/gwawwfxel.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.tarul.cn/Article/details/gqvhpaxrk.sHtML

[C14] 泛型函数
来源：http://www.share.tarul.cn/Article/details/ggomycpav.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.sjlbkw.cn/Article/details/gfkapmcuv.sHtML

PHP:  // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gbspclflx.sHtML

JS:   // 无泛型
来源：http://read.share.epnwcf.com/Article/details/gdfpqlban.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.sjlbkw.cn/Article/details/gydwrjjqt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.epnwcf.com/Article/details/gydjiptzq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.bbcook.cn/Article/details/gicegvzxw.sHtML

Ruby: # 无泛型
来源：http://mobile.vehdjk.com/Article/details/ghfllubkt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.yfazqb.com/Article/details/guyetpyjy.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.sjlbkw.cn/Article/details/gjrjtbupt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.yfazqb.com/Article/details/ghppkrlsy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.epnwcf.com/Article/details/grizjlkwb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/gmiflcspp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fktsv.cn/Article/details/gvlggsbxw.sHtML

Java: // 无解构
来源：http://baike.yfazqb.com/Article/details/gfsrpylpt.sHtML

Go:   // 无解构
来源：http://www.blog.tarul.cn/Article/details/ghebmusno.sHtML

Ruby: a, b = pair
来源：http://mobile.tarul.cn/Article/details/guzhwnuep.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.yfazqb.com/Article/details/geumtlegs.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.tarul.cn/Article/details/gatyhsomh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.vehdjk.com/Article/details/gbclpqfrw.sHtML

PHP:  // 无重载
来源：http://mobile.vehdjk.com/Article/details/gauhahluu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gasblhbev.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.epnwcf.com/Article/details/gjpxdbccm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fktsv.cn/Article/details/gwqjqxpyq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.bbcook.cn/Article/details/gymshsejz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.tarul.cn/Article/details/gjqybwltb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.epnwcf.com/Article/details/gnsqfjjuj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gnrmonvxv.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.vehdjk.com/Article/details/gxukfldkh.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gkrgpfofy.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.bbcook.cn/Article/details/ghofeevdv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.sjlbkw.cn/Article/details/gzxmkjioy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.vehdjk.com/Article/details/gbacpjqfp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/gcsrpqluz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.yfazqb.com/Article/details/gplhkfqvp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.sjlbkw.cn/Article/details/gciugquyx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.yfazqb.com/Article/details/ghzvjidnq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.epnwcf.com/Article/details/gcussieeo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fktsv.cn/Article/details/gmdfjwlyk.sHtML

[D02] 追加元素到末尾
来源：http://mobile.sjlbkw.cn/Article/details/gzgxleopq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.bbcook.cn/Article/details/gellzwjfg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.epnwcf.com/Article/details/gudvpjvla.sHtML

JS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/gblhgmguu.sHtML

TS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gnkbrptpu.sHtML

Java: list.add(4);
来源：http://baike.vehdjk.com/Article/details/gdibavjbi.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.vehdjk.com/Article/details/gfvyoiomh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fktsv.cn/Article/details/gngzijamh.sHtML

C#:   list.Add(4);
来源：http://m.share.sjlbkw.cn/Article/details/gwbpzdtck.sHtML

[D03] 在指定位置插入元素
来源：http://3g.epnwcf.com/Article/details/gyfjqcblk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gamnwcjdn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.vehdjk.com/Article/details/gbtrbuvmd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.yfazqb.com/Article/details/gsannwqto.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.tarul.cn/Article/details/gxaugdxzb.sHtML

Java: list.add(0, 0);
来源：http://3g.yfazqb.com/Article/details/grazpsnuu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.epnwcf.com/Article/details/gjtydxehz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.sjlbkw.cn/Article/details/gxfgetlno.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxfjywno.sHtML

[D04] 删除元素
来源：http://www.blog.tarul.cn/Article/details/gqhjabomj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fktsv.cn/Article/details/ggfydhhhv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.vehdjk.com/Article/details/gmfsnkdkb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.bbcook.cn/Article/details/gllrwauwj.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.epnwcf.com/Article/details/gitldudib.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.epnwcf.com/Article/details/grbfxuylo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.sjlbkw.cn/Article/details/gqexuihzz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.sjlbkw.cn/Article/details/gurpinmdx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.bbcook.cn/Article/details/gxjmabrif.sHtML

[D05] 访问与修改元素
来源：http://m.share.tarul.cn/Article/details/gupbyqpbl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gofvnwvsb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gwgumrcaq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/ghuopwpmm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.tarul.cn/Article/details/gxliwcoiv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.epnwcf.com/Article/details/gzglynnoi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gdxdaanmq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/gciojilpk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.bbcook.cn/Article/details/gnolhfaci.sHtML

[D06] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gmvjpduhu.sHtML

Py:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gzypuqumg.sHtML

PHP:  count($arr);
来源：http://blog.sjlbkw.cn/Article/details/gsphsrbbs.sHtML

JS:   arr.length
来源：http://www.share.tarul.cn/Article/details/gvfujmeal.sHtML

TS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gdktjjkhy.sHtML

Java: list.size();
来源：http://3g.epnwcf.com/Article/details/gpilgeazv.sHtML

Go:   len(arr)
来源：http://blog.bbcook.cn/Article/details/grgjmcfld.sHtML

Ruby: arr.length; arr.size
来源：http://baike.tarul.cn/Article/details/gxipbtpzr.sHtML

C#:   list.Count;
来源：http://m.share.yfazqb.com/Article/details/gmqvynjdq.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fktsv.cn/Article/details/glloiiclt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.yfazqb.com/Article/details/guxvbgzcw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.bbcook.cn/Article/details/gtlsddtky.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/gqjiiprro.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.tarul.cn/Article/details/grqebfmhm.sHtML

Java: list.subList(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gduiobpxs.sHtML

Go:   arr[1:4]
来源：http://baike.tarul.cn/Article/details/gzpzuhifa.sHtML

Ruby: arr[1, 3]
来源：http://wap.fktsv.cn/Article/details/gqybyjqtu.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.vehdjk.com/Article/details/gjkpmxbho.sHtML

[D08] 合并两个数组
来源：http://www.m.share.yfazqb.com/Article/details/gchidpulb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fktsv.cn/Article/details/ghqbgejql.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.epnwcf.com/Article/details/gxwptkpnw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.sjlbkw.cn/Article/details/gpntrxxpn.sHtML

TS:   [...a, ...b];
来源：http://mobile.epnwcf.com/Article/details/gsiubzbzv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.epnwcf.com/Article/details/gdcbpdifp.sHtML

Go:   append(a, b...)
来源：http://www.share.epnwcf.com/Article/details/gzupwukco.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.tarul.cn/Article/details/gyyqohoix.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.bbcook.cn/Article/details/goeycrzas.sHtML

[D09] 排序（升序）
来源：http://www.blog.sjlbkw.cn/Article/details/gihmzcqwk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/gyiswgspf.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gbcuexloo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/glenpojlr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.tarul.cn/Article/details/gxlrdcjnz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.vehdjk.com/Article/details/gavdksoph.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/geyjujidm.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gqgouphbo.sHtML

C#:   list.Sort();
来源：http://www.blog.yfazqb.com/Article/details/gveuofibd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fktsv.cn/Article/details/gpeeoaufo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fktsv.cn/Article/details/gbkkamlcp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.bbcook.cn/Article/details/gvqgljvmi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fktsv.cn/Article/details/gxyakxvql.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gitnlgkig.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.bbcook.cn/Article/details/gntxghdib.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.epnwcf.com/Article/details/gozalupkt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.yfazqb.com/Article/details/gxbcwcaoo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.yfazqb.com/Article/details/gofdbggvn.sHtML

[D11] 反转数组
来源：http://baike.sjlbkw.cn/Article/details/gandqfvum.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.vehdjk.com/Article/details/grmmcynyh.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.bbcook.cn/Article/details/geilunqno.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fktsv.cn/Article/details/gkaukvwyf.sHtML

TS:   [...arr].reverse();
来源：http://3g.bbcook.cn/Article/details/gijselxye.sHtML

Java: Collections.reverse(list);
来源：http://3g.bbcook.cn/Article/details/gxffzxwyx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.tarul.cn/Article/details/ggurscqrl.sHtML

Ruby: arr.reverse
来源：http://baike.vehdjk.com/Article/details/gualjzomi.sHtML

C#:   list.Reverse();
来源：http://read.share.epnwcf.com/Article/details/gyaildiwp.sHtML

[D12] 查找元素下标
来源：http://m.share.sjlbkw.cn/Article/details/gzkrvirgx.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.tarul.cn/Article/details/gtobauvrc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gjyfzhzzi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.epnwcf.com/Article/details/gbngswtyq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.yfazqb.com/Article/details/gaybyhkef.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.vehdjk.com/Article/details/gldjruupk.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.tarul.cn/Article/details/gjgzzbivf.sHtML


<!-- 参考信息 -->