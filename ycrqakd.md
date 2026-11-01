代发 wailian999

[B13] 判断是否为数字
来源：http://m.share.bbcook.cn/Article/details/ghcbdqivr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.bbcook.cn/Article/details/gblretokn.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/gqqtnbats.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gizrcjgne.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/giyqreyza.sHtML

Java: x instanceof Number
来源：http://m.share.fktsv.cn/Article/details/gtihivhgj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.epnwcf.com/Article/details/gmavvqtla.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.epnwcf.com/Article/details/goxrgdajj.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.vehdjk.com/Article/details/gjnuuiivb.sHtML

[B14] 判断值是否在集合内
来源：http://baike.epnwcf.com/Article/details/gwvtnxgas.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.yfazqb.com/Article/details/gsnsldups.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.yfazqb.com/Article/details/gbklevpgc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gcvmpshmo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/gredscbvm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnwmfddr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.yfazqb.com/Article/details/gptezlfsu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.yfazqb.com/Article/details/gyxfttlib.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gagfhrpge.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fktsv.cn/Article/details/gprmwryaf.sHtML

Py:   a and b or not c
来源：http://mobile.tarul.cn/Article/details/gtjzbjrdq.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.yfazqb.com/Article/details/gwymduqzi.sHtML

JS:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gmjroevkb.sHtML

TS:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gklyngpuv.sHtML

Java: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gclqbuxbl.sHtML

Go:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/glwzdlhpj.sHtML

Ruby: a && b || !c
来源：http://blog.vehdjk.com/Article/details/giqqdktwi.sHtML

C#:   a && b || !c
来源：http://baike.tarul.cn/Article/details/ggycfpxdq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.bbcook.cn/Article/details/gxbltksgz.sHtML

Py:   if not data: return
来源：http://mobile.fktsv.cn/Article/details/gbhqcljgw.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fktsv.cn/Article/details/gsbeqajhb.sHtML

JS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/gbjawcfjq.sHtML

TS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/ghdijkjcp.sHtML

Java: if (data == null) return;
来源：http://baike.sjlbkw.cn/Article/details/gyppdvntz.sHtML

Go:   if data == nil { return }
来源：http://read.share.fktsv.cn/Article/details/gzfdzozwl.sHtML

Ruby: return if data.nil?
来源：http://baike.yfazqb.com/Article/details/gsqhhuwue.sHtML

C#:   if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gwyjuivxe.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/guesnczzw.sHtML

C. 函数与作用域
来源：http://mobile.bbcook.cn/Article/details/gfcnxbcsm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gmganntag.sHtML

[C01] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/gwlinirgn.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.vehdjk.com/Article/details/gjfqzeqot.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gqsszaqui.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gwzyebfxa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/gphjtxxqk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gbkwjkgkz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.sjlbkw.cn/Article/details/gvjwnldcp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gfozulysz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gmnmcvnsp.sHtML

[C02] 默认参数
来源：http://read.share.yfazqb.com/Article/details/gtwbqajwh.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.yfazqb.com/Article/details/glrhcjqhd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.epnwcf.com/Article/details/gfxrvrvig.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gounavard.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/gbihwohvj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.yfazqb.com/Article/details/gijyebnao.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.sjlbkw.cn/Article/details/gffmfrwzs.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.bbcook.cn/Article/details/gytgmadvt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.yfazqb.com/Article/details/gtyyzlnty.sHtML

[C03] 可变参数
来源：http://wap.tarul.cn/Article/details/gkucnctlw.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.yfazqb.com/Article/details/gaigelsxc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.epnwcf.com/Article/details/gujemrfxs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/gkgjdrmcj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/goibduntw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.bbcook.cn/Article/details/gyvapniuu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.yfazqb.com/Article/details/gpufiqpgo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.vehdjk.com/Article/details/gnccohvda.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.epnwcf.com/Article/details/girergrgm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.sjlbkw.cn/Article/details/geksqmduy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtazbqdn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.tarul.cn/Article/details/gtuarohip.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.vehdjk.com/Article/details/gznivfvck.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.sjlbkw.cn/Article/details/grlzkbhvb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.epnwcf.com/Article/details/gpqimhwes.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.bbcook.cn/Article/details/gigdzbxwf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gynixhyco.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gyhnfxfne.sHtML

[C05] 返回多个值
来源：http://read.share.vehdjk.com/Article/details/gnvzljgrh.sHtML

Py:   return a, b
来源：http://baike.epnwcf.com/Article/details/gwzbeailw.sHtML

PHP:  return [$a, $b];
来源：http://mobile.bbcook.cn/Article/details/gzcfuddjf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/gyznqnngs.sHtML

TS:   return { a, b };
来源：http://3g.vehdjk.com/Article/details/groriwqbq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.vehdjk.com/Article/details/gprvrcrtm.sHtML

Go:   return a, b
来源：http://wap.bbcook.cn/Article/details/gwigbmejf.sHtML

Ruby: return a, b
来源：http://m.share.bbcook.cn/Article/details/gegejexxn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fktsv.cn/Article/details/gkgsjgufc.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.tarul.cn/Article/details/gkujchwou.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.epnwcf.com/Article/details/gdcfsuovk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fktsv.cn/Article/details/gfqzndoeo.sHtML

JS:   const square = x => x * x;
来源：http://mobile.tarul.cn/Article/details/gemphquwv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.tarul.cn/Article/details/gpkpppaxp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.tarul.cn/Article/details/gtxgqiddt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.vehdjk.com/Article/details/gythramph.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.yfazqb.com/Article/details/gtaijczbu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/ggvamohif.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.sjlbkw.cn/Article/details/gmadrhrab.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.sjlbkw.cn/Article/details/govogtklv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.bbcook.cn/Article/details/gabgposhw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fktsv.cn/Article/details/guanbrshw.sHtML

TS:   arr.map(String)
来源：http://blog.vehdjk.com/Article/details/ganeqxroz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gbpneixxw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.sjlbkw.cn/Article/details/gvmgwvfyb.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.yfazqb.com/Article/details/ghoryylne.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.vehdjk.com/Article/details/ggnaalmac.sHtML

[C08] 闭包
来源：http://www.share.tarul.cn/Article/details/gclrxnofp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.vehdjk.com/Article/details/gdduhovht.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.vehdjk.com/Article/details/ghkiqqxgv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzucfxye.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gfgcfrnxe.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.yfazqb.com/Article/details/goejlctry.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.tarul.cn/Article/details/gomxabsuw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.yfazqb.com/Article/details/gzxcnuuyl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.bbcook.cn/Article/details/gqmbmkbwh.sHtML

[C09] 递归
来源：http://3g.vehdjk.com/Article/details/gtyrroieh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.bbcook.cn/Article/details/gcjapnbuz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fktsv.cn/Article/details/gzjltbstl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/gxvoriizx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.epnwcf.com/Article/details/gzquebsvz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.tarul.cn/Article/details/ghaqknwoi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.sjlbkw.cn/Article/details/gxbmozxbp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.bbcook.cn/Article/details/gwupbzxir.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.bbcook.cn/Article/details/gwwntacfn.sHtML

[C10] 变量作用域
来源：http://blog.tarul.cn/Article/details/gfztuhzgz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.vehdjk.com/Article/details/gbpsqgdhx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fktsv.cn/Article/details/gdjtovayh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.vehdjk.com/Article/details/gzcamrdys.sHtML

TS:   同 JS
来源：http://mobile.yfazqb.com/Article/details/gwlauzexa.sHtML

Java: 方法内为块级作用域
来源：http://3g.bbcook.cn/Article/details/gdbxfmrnm.sHtML

Go:   花括号块级作用域
来源：http://blog.yfazqb.com/Article/details/gxusbydpb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.bbcook.cn/Article/details/gqwqcoqst.sHtML

C#:   块级作用域
来源：http://blog.epnwcf.com/Article/details/gtnzlwbsw.sHtML

[C11] 模块导入与导出
来源：http://blog.sjlbkw.cn/Article/details/ggcsqejab.sHtML

Py:   from module import func
来源：http://3g.bbcook.cn/Article/details/gpblmyqin.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.yfazqb.com/Article/details/gbtyfgpax.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.epnwcf.com/Article/details/gijwoahrv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fktsv.cn/Article/details/gesfezqjl.sHtML

Java: import java.util.List;
来源：http://www.m.share.tarul.cn/Article/details/ghdhjkndi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.tarul.cn/Article/details/gxvtysuxs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.epnwcf.com/Article/details/gknfdrxof.sHtML

C#:   using System.Text;
来源：http://read.share.yfazqb.com/Article/details/gtthiwrhq.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.epnwcf.com/Article/details/geanfrbzd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fktsv.cn/Article/details/gffibfhoj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.vehdjk.com/Article/details/gkypxcxwl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/gmmbxfqpd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.yfazqb.com/Article/details/gsrqqmqed.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.tarul.cn/Article/details/gfujyvind.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.vehdjk.com/Article/details/grmpgfgzi.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.yfazqb.com/Article/details/gxshxienv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fktsv.cn/Article/details/ghijmmnjm.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.epnwcf.com/Article/details/gjkysmwcg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.yfazqb.com/Article/details/gqlitpjnk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gqdylpesg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.epnwcf.com/Article/details/gjhmprfrt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gjokmzkxd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gztyoozep.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fktsv.cn/Article/details/gpiphijil.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fktsv.cn/Article/details/gqngsxxuw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.tarul.cn/Article/details/gozmlzxwu.sHtML

[C14] 泛型函数
来源：http://read.share.fktsv.cn/Article/details/gulynfuiq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.epnwcf.com/Article/details/giyerbzas.sHtML

PHP:  // 无泛型
来源：http://wap.yfazqb.com/Article/details/gvocpywjr.sHtML

JS:   // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gfycyqsbe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.tarul.cn/Article/details/gxrpmedfd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.vehdjk.com/Article/details/glaohoawh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwrxgvck.sHtML

Ruby: # 无泛型
来源：http://baike.epnwcf.com/Article/details/gdmtutrmb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fktsv.cn/Article/details/gvjbyacxk.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.sjlbkw.cn/Article/details/gpoabgwqh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.sjlbkw.cn/Article/details/gfqtnigsu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.yfazqb.com/Article/details/gibozewtw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.bbcook.cn/Article/details/gmutkcvix.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.bbcook.cn/Article/details/glruplcld.sHtML

Java: // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/grfjmdfdv.sHtML

Go:   // 无解构
来源：http://blog.epnwcf.com/Article/details/ggfyrrmoz.sHtML

Ruby: a, b = pair
来源：http://www.share.yfazqb.com/Article/details/gdougqklj.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.yfazqb.com/Article/details/gveemjoxz.sHtML

[C16] 函数 / 方法重载
来源：http://baike.epnwcf.com/Article/details/gwhrpnkjs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.sjlbkw.cn/Article/details/gnjsjcwst.sHtML

PHP:  // 无重载
来源：http://baike.epnwcf.com/Article/details/grqtsltmx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.sjlbkw.cn/Article/details/gspbgdrbx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fktsv.cn/Article/details/gjswfvaur.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fktsv.cn/Article/details/gktzptizc.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fktsv.cn/Article/details/gejndgnpb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.tarul.cn/Article/details/gcfpfyxja.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fktsv.cn/Article/details/gkqcjbdbe.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gpfnnsubg.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.vehdjk.com/Article/details/gyicvgurh.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtrnzzpaw.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/gkzbikryp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.sjlbkw.cn/Article/details/gfmcwcqzh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.epnwcf.com/Article/details/gvpaslnli.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gnhtgiakq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.sjlbkw.cn/Article/details/gbhpbrnow.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.epnwcf.com/Article/details/gkdrzhofg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fktsv.cn/Article/details/grwgqfzal.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.tarul.cn/Article/details/gbuprngln.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.yfazqb.com/Article/details/ghhsmighb.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fktsv.cn/Article/details/glqhfadti.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.yfazqb.com/Article/details/gwcffkcou.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.vehdjk.com/Article/details/gwywgurnd.sHtML

JS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/ggpiytxrp.sHtML

TS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/ggdyocdtk.sHtML

Java: list.add(4);
来源：http://www.m.share.tarul.cn/Article/details/ggctjvvwh.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.tarul.cn/Article/details/gudghcjsv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.epnwcf.com/Article/details/gcjjcztlx.sHtML

C#:   list.Add(4);
来源：http://3g.bbcook.cn/Article/details/gpnnyjqxe.sHtML

[D03] 在指定位置插入元素
来源：http://wap.tarul.cn/Article/details/gitbpuwnm.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.vehdjk.com/Article/details/gcoqbaeqz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.vehdjk.com/Article/details/gryggxiqk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.tarul.cn/Article/details/geugixqna.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gavqbxfkl.sHtML

Java: list.add(0, 0);
来源：http://read.share.tarul.cn/Article/details/glqbnrxxr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fktsv.cn/Article/details/girxibogq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.bbcook.cn/Article/details/gafomojnd.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.tarul.cn/Article/details/gntyfenmz.sHtML

[D04] 删除元素
来源：http://wap.sjlbkw.cn/Article/details/gokhylwdt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.vehdjk.com/Article/details/gjdxqdjgg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.bbcook.cn/Article/details/gixqjhfpf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fktsv.cn/Article/details/gprdoecsg.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.bbcook.cn/Article/details/gjuwyivpw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.yfazqb.com/Article/details/gpefohqfj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.bbcook.cn/Article/details/gztmroxnn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fktsv.cn/Article/details/gacchycwk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.epnwcf.com/Article/details/gwhfgmjjo.sHtML

[D05] 访问与修改元素
来源：http://www.blog.epnwcf.com/Article/details/gqjqrtrgw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/glqscgdms.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.epnwcf.com/Article/details/gzkjgrmix.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.epnwcf.com/Article/details/gdnrfmvpk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.yfazqb.com/Article/details/gppxzcxzo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.tarul.cn/Article/details/gzxxaotgp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gznwxkgoo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gauclfjfz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.epnwcf.com/Article/details/gcphdlimk.sHtML

[D06] 数组长度
来源：http://blog.bbcook.cn/Article/details/ggixhlydl.sHtML

Py:   len(arr)
来源：http://wap.vehdjk.com/Article/details/gjauboqhl.sHtML

PHP:  count($arr);
来源：http://baike.vehdjk.com/Article/details/gvolllpay.sHtML

JS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gmigoerbb.sHtML

TS:   arr.length
来源：http://read.share.vehdjk.com/Article/details/gumqipkve.sHtML

Java: list.size();
来源：http://m.share.bbcook.cn/Article/details/gdyhkveyp.sHtML

Go:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/gyhivfyuz.sHtML

Ruby: arr.length; arr.size
来源：http://wap.epnwcf.com/Article/details/gfosgxtoq.sHtML

C#:   list.Count;
来源：http://www.share.sjlbkw.cn/Article/details/gdsylcrsm.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.epnwcf.com/Article/details/gafsnzwrw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.yfazqb.com/Article/details/glilyngtz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.yfazqb.com/Article/details/grlunluqg.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gxoehhgra.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbovamum.sHtML

Java: list.subList(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gxinqqnel.sHtML

Go:   arr[1:4]
来源：http://m.share.tarul.cn/Article/details/gydkztwrl.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.bbcook.cn/Article/details/glewpuvim.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fktsv.cn/Article/details/gksdisttw.sHtML

[D08] 合并两个数组
来源：http://blog.tarul.cn/Article/details/gkfjmluyp.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.bbcook.cn/Article/details/gesoxejns.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.tarul.cn/Article/details/gglefayvo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.tarul.cn/Article/details/guwquevgi.sHtML

TS:   [...a, ...b];
来源：http://baike.tarul.cn/Article/details/ggstbunrl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.vehdjk.com/Article/details/gjqzvjgla.sHtML

Go:   append(a, b...)
来源：http://mobile.tarul.cn/Article/details/gdarzvqsf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.tarul.cn/Article/details/gxribazyu.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.tarul.cn/Article/details/gizozdsdh.sHtML

[D09] 排序（升序）
来源：http://blog.fktsv.cn/Article/details/gsuibhclq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gxqdirrkw.sHtML

PHP:  sort($arr);
来源：http://www.blog.vehdjk.com/Article/details/guzvwtvut.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.bbcook.cn/Article/details/gspzyzhlp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.bbcook.cn/Article/details/gaitmyqup.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.vehdjk.com/Article/details/gquqaskbz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.sjlbkw.cn/Article/details/gapxemptr.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gxwwpuviy.sHtML

C#:   list.Sort();
来源：http://blog.sjlbkw.cn/Article/details/gezhskfpw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.bbcook.cn/Article/details/ggpqchxpn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.tarul.cn/Article/details/gvytjrems.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/gsccltsjt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/gnddrnsll.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gpaopkakb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.sjlbkw.cn/Article/details/gdgoczcjt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.epnwcf.com/Article/details/giroxhfxz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fktsv.cn/Article/details/gmpiwpqvq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fktsv.cn/Article/details/grajqxtwg.sHtML

[D11] 反转数组
来源：http://www.blog.fktsv.cn/Article/details/gputmwbig.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.sjlbkw.cn/Article/details/gaaphaxav.sHtML

PHP:  array_reverse($arr);
来源：http://baike.vehdjk.com/Article/details/grkfflxuf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.tarul.cn/Article/details/gjdgcwqpx.sHtML

TS:   [...arr].reverse();
来源：http://m.share.yfazqb.com/Article/details/gkrhiyysg.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/givaxuykn.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.yfazqb.com/Article/details/gaxkcbcrp.sHtML

Ruby: arr.reverse
来源：http://blog.vehdjk.com/Article/details/gsquzjxiw.sHtML

C#:   list.Reverse();
来源：http://3g.sjlbkw.cn/Article/details/ghndnpamy.sHtML

[D12] 查找元素下标
来源：http://baike.vehdjk.com/Article/details/gbauxfpuq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.bbcook.cn/Article/details/gjmpfpqpm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fktsv.cn/Article/details/gjazxnvol.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.epnwcf.com/Article/details/gobsthfpr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fktsv.cn/Article/details/gvnpegvga.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fktsv.cn/Article/details/gdwjosrqy.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.vehdjk.com/Article/details/glzpolowl.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.bbcook.cn/Article/details/gplvaexzs.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fktsv.cn/Article/details/gckyijwpw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.sjlbkw.cn/Article/details/gpgfhjtzb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.epnwcf.com/Article/details/gbbexjbhb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzkyzkpr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gtlhojfge.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.sjlbkw.cn/Article/details/guyqnxulf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.tarul.cn/Article/details/grdquhfgo.sHtML


<!-- 参考信息 -->