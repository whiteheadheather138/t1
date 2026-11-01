代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.vehdjk.com/Article/details/ggophsgvg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.tarul.cn/Article/details/ggdltbhvm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gphaeoqoh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gxhujzuaq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gdvuxnrwf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.sjlbkw.cn/Article/details/gdkuyxrie.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.bbcook.cn/Article/details/giqzjpuzb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.bbcook.cn/Article/details/gczkyzbsb.sHtML

[B13] 判断是否为数字
来源：http://3g.tarul.cn/Article/details/gwcwhylkc.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.yfazqb.com/Article/details/grvwenfiy.sHtML

PHP:  is_numeric($x)
来源：http://mobile.tarul.cn/Article/details/gcykwornn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.tarul.cn/Article/details/glkfekjgm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/gigbvacsa.sHtML

Java: x instanceof Number
来源：http://www.m.share.bbcook.cn/Article/details/gitdpjgzd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.bbcook.cn/Article/details/gvbqrovio.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fktsv.cn/Article/details/goqcasbbm.sHtML

C#:   x is int or double or decimal
来源：http://baike.fktsv.cn/Article/details/gykxvtjgv.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fktsv.cn/Article/details/gktaaagdo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.yfazqb.com/Article/details/gmlgmlufq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fktsv.cn/Article/details/gdiojnhsb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.yfazqb.com/Article/details/gduajundz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/gsffbdccl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.yfazqb.com/Article/details/gosybrgcv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.vehdjk.com/Article/details/goyhrvqnk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.yfazqb.com/Article/details/ghvnoblwq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gvnhiedtt.sHtML

[B15] 布尔运算与取反
来源：http://m.share.tarul.cn/Article/details/gzbdtolbw.sHtML

Py:   a and b or not c
来源：http://baike.fktsv.cn/Article/details/gxmuwovqq.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.tarul.cn/Article/details/goaekrkje.sHtML

JS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gpsvoedfo.sHtML

TS:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gztbnbpfo.sHtML

Java: a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gvhqokhss.sHtML

Go:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gzfrchgqh.sHtML

Ruby: a && b || !c
来源：http://m.share.fktsv.cn/Article/details/genxxedrd.sHtML

C#:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gpderjhen.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.tarul.cn/Article/details/gyffgtazq.sHtML

Py:   if not data: return
来源：http://baike.sjlbkw.cn/Article/details/gumdcfnzn.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.epnwcf.com/Article/details/gdkclqxkn.sHtML

JS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gutifsdei.sHtML

TS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/gzroyilov.sHtML

Java: if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/geeykffhh.sHtML

Go:   if data == nil { return }
来源：http://www.share.bbcook.cn/Article/details/gvamhnrug.sHtML

Ruby: return if data.nil?
来源：http://baike.fktsv.cn/Article/details/ghjdznoff.sHtML

C#:   if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gxyenyvcq.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gfrmcygsc.sHtML

C. 函数与作用域
来源：http://3g.epnwcf.com/Article/details/gsfjstovd.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gfwwoknph.sHtML

[C01] 定义函数
来源：http://www.share.vehdjk.com/Article/details/gsddwggap.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.sjlbkw.cn/Article/details/gmiihhuyp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gswpubywn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gxpprlgqo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/ggcdwpssb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/guuzcosbi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.bbcook.cn/Article/details/grjtkkdqb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.sjlbkw.cn/Article/details/glpemmsbd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gyerjinxa.sHtML

[C02] 默认参数
来源：http://wap.yfazqb.com/Article/details/gnweemuga.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.yfazqb.com/Article/details/gkoytftyr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.epnwcf.com/Article/details/ggslsdxme.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/gstpihsmc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/ggxxdmjuv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.vehdjk.com/Article/details/gtrmciuix.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.yfazqb.com/Article/details/gcuselkjk.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvslumbb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.bbcook.cn/Article/details/gcyhtofrh.sHtML

[C03] 可变参数
来源：http://3g.epnwcf.com/Article/details/gzshoocbs.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.sjlbkw.cn/Article/details/guuujemdc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fktsv.cn/Article/details/gdntuxegp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.yfazqb.com/Article/details/gxgirniet.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/gvxlemjci.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fktsv.cn/Article/details/gdvkiwqbx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.tarul.cn/Article/details/glevvpefk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.epnwcf.com/Article/details/gnvpnvsgu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.yfazqb.com/Article/details/gbhgtzyzl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.sjlbkw.cn/Article/details/gzxaxoqsz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.yfazqb.com/Article/details/gzylnmqiy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.yfazqb.com/Article/details/gmajcjdkk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gfjnmemiq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.tarul.cn/Article/details/gjomyvgvp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.vehdjk.com/Article/details/gxisphipt.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.vehdjk.com/Article/details/gdifvjzae.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gqdagbrnq.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/gqxyimtml.sHtML

[C05] 返回多个值
来源：http://www.blog.bbcook.cn/Article/details/ggavpgwzn.sHtML

Py:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gnrlvdeuv.sHtML

PHP:  return [$a, $b];
来源：http://wap.sjlbkw.cn/Article/details/gvwilflbh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.vehdjk.com/Article/details/gheqzdyim.sHtML

TS:   return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gksamcfhf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.epnwcf.com/Article/details/gzxxmxcaz.sHtML

Go:   return a, b
来源：http://mobile.yfazqb.com/Article/details/gqvbeelhw.sHtML

Ruby: return a, b
来源：http://wap.epnwcf.com/Article/details/gnjxdfkue.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.vehdjk.com/Article/details/ghlyequyw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.bbcook.cn/Article/details/gjbprmzpc.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.vehdjk.com/Article/details/gzjyhapyo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.epnwcf.com/Article/details/gamumzxwg.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gfxoxgxcc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gysujnvhg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gcvugojix.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.yfazqb.com/Article/details/goqnihlnh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fktsv.cn/Article/details/gibmfqnrs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gcrzbksco.sHtML

[C07] 把函数作为参数传入
来源：http://baike.bbcook.cn/Article/details/gcggoficn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.sjlbkw.cn/Article/details/ghdbbvnhg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gguksiqfd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.tarul.cn/Article/details/giphaxjol.sHtML

TS:   arr.map(String)
来源：http://wap.tarul.cn/Article/details/gocgzovvi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.vehdjk.com/Article/details/gsemtdnqg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.vehdjk.com/Article/details/giiqogbrg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fktsv.cn/Article/details/giofpzgio.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/gvvdjkkbl.sHtML

[C08] 闭包
来源：http://read.share.yfazqb.com/Article/details/gnyixfbjq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.vehdjk.com/Article/details/gykgcyabw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.tarul.cn/Article/details/gmbsrreaa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gvqdhryor.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/ghfbwfrmy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.vehdjk.com/Article/details/gejdwrwtq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.tarul.cn/Article/details/gfnzxmhyw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.bbcook.cn/Article/details/gduhguepb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gokfppetw.sHtML

[C09] 递归
来源：http://mobile.bbcook.cn/Article/details/gerkfxwmp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.vehdjk.com/Article/details/gubeecekq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.tarul.cn/Article/details/gcczafqvx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gzrdhwghg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gomghhohx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.vehdjk.com/Article/details/gdhyyeget.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.vehdjk.com/Article/details/gjvlltlgq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gttmkfrqk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.vehdjk.com/Article/details/gvhwsenir.sHtML

[C10] 变量作用域
来源：http://3g.yfazqb.com/Article/details/gvudylhni.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.sjlbkw.cn/Article/details/gqgzyooeb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.vehdjk.com/Article/details/giqvdcrpz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.yfazqb.com/Article/details/gqnqxlfgf.sHtML

TS:   同 JS
来源：http://read.share.epnwcf.com/Article/details/gboagwcjj.sHtML

Java: 方法内为块级作用域
来源：http://3g.fktsv.cn/Article/details/gcsyrscgu.sHtML

Go:   花括号块级作用域
来源：http://www.share.bbcook.cn/Article/details/gufjbtrbz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.bbcook.cn/Article/details/gyyihhzbv.sHtML

C#:   块级作用域
来源：http://baike.fktsv.cn/Article/details/ghvlrjxox.sHtML

[C11] 模块导入与导出
来源：http://baike.yfazqb.com/Article/details/gkavddsgh.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/gmxhsdlbx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.vehdjk.com/Article/details/gclsyflkz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.epnwcf.com/Article/details/gmqnefvrt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.vehdjk.com/Article/details/gtchfxnss.sHtML

Java: import java.util.List;
来源：http://baike.epnwcf.com/Article/details/gcmblnnoy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.tarul.cn/Article/details/gjyfyevae.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.bbcook.cn/Article/details/gttahjhuq.sHtML

C#:   using System.Text;
来源：http://baike.bbcook.cn/Article/details/gpcqkoimu.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.bbcook.cn/Article/details/geexjtrqs.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.vehdjk.com/Article/details/grkkpqgva.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.yfazqb.com/Article/details/gsjjrnbrq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.epnwcf.com/Article/details/gsgicnobj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.bbcook.cn/Article/details/ghcwrraun.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.epnwcf.com/Article/details/ggmcnzlrr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.bbcook.cn/Article/details/godvowfxi.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.tarul.cn/Article/details/gwmiholyi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gpwieaqhn.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.sjlbkw.cn/Article/details/gpjsbgarx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.vehdjk.com/Article/details/gcypfyjys.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gkzrlbjfj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fktsv.cn/Article/details/grhnzputw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gglvhhdpm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gwywhpbmd.sHtML

Go:   func add(a, b int) int
来源：http://mobile.bbcook.cn/Article/details/gpmrhuocv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.vehdjk.com/Article/details/grabenabo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.yfazqb.com/Article/details/guwrdvlfq.sHtML

[C14] 泛型函数
来源：http://www.m.share.yfazqb.com/Article/details/goczsftxi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.epnwcf.com/Article/details/gbmzxuabq.sHtML

PHP:  // 无泛型
来源：http://3g.vehdjk.com/Article/details/giydgfblx.sHtML

JS:   // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gykaqehyo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.vehdjk.com/Article/details/gonqkqlee.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.vehdjk.com/Article/details/gewofvnxc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.epnwcf.com/Article/details/ggmvndfip.sHtML

Ruby: # 无泛型
来源：http://blog.yfazqb.com/Article/details/gckmkwpzf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fktsv.cn/Article/details/girhxdekq.sHtML

[C15] 解构 / 展开参数
来源：http://blog.yfazqb.com/Article/details/gsktoyhrz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.epnwcf.com/Article/details/ggiayupsd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fktsv.cn/Article/details/gfubcdnva.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.tarul.cn/Article/details/gajkrrjyy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.vehdjk.com/Article/details/gwstgbewd.sHtML

Java: // 无解构
来源：http://read.share.epnwcf.com/Article/details/gepgqdeob.sHtML

Go:   // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/grglxmbvg.sHtML

Ruby: a, b = pair
来源：http://baike.bbcook.cn/Article/details/gvywjbsak.sHtML

C#:   var (a, b) = pair;
来源：http://blog.sjlbkw.cn/Article/details/gkhwxdowq.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.tarul.cn/Article/details/gancqfplb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.yfazqb.com/Article/details/gvmjeubvx.sHtML

PHP:  // 无重载
来源：http://www.m.share.vehdjk.com/Article/details/gcwpdwhar.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.tarul.cn/Article/details/glqvwzemm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.yfazqb.com/Article/details/guwdsknma.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fktsv.cn/Article/details/gkfwxxpbk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.bbcook.cn/Article/details/gcomkknwf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fktsv.cn/Article/details/gexzjlarq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.vehdjk.com/Article/details/gzjpoewjz.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmjdekejf.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.bbcook.cn/Article/details/gbyvgvhco.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gixhkyolb.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gmnqohfco.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fktsv.cn/Article/details/goppovdqe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.tarul.cn/Article/details/gzlcurznd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.vehdjk.com/Article/details/gbqtpgdkb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.sjlbkw.cn/Article/details/gvzxgyjet.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.yfazqb.com/Article/details/grydpteuc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.vehdjk.com/Article/details/gzivztmjn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.bbcook.cn/Article/details/gyzakvaku.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.yfazqb.com/Article/details/gitzombxs.sHtML

[D02] 追加元素到末尾
来源：http://3g.sjlbkw.cn/Article/details/gqqomrtno.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.tarul.cn/Article/details/gyxuisyra.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.yfazqb.com/Article/details/gvhtunkoy.sHtML

JS:   arr.push(4);
来源：http://blog.sjlbkw.cn/Article/details/ghmajfvub.sHtML

TS:   arr.push(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcxdtype.sHtML

Java: list.add(4);
来源：http://www.share.vehdjk.com/Article/details/gegnhzbpu.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.vehdjk.com/Article/details/gqjbenfwf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.vehdjk.com/Article/details/gvzamlzcx.sHtML

C#:   list.Add(4);
来源：http://www.share.sjlbkw.cn/Article/details/gpwqiovqu.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.yfazqb.com/Article/details/grhlskhjq.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fktsv.cn/Article/details/gjqdfxaqr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.yfazqb.com/Article/details/ghnjjbqct.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.yfazqb.com/Article/details/gntmhjobj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.epnwcf.com/Article/details/guvlugfld.sHtML

Java: list.add(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gyhnlpfyz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.yfazqb.com/Article/details/govdljvcv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.bbcook.cn/Article/details/grqqpuohz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.epnwcf.com/Article/details/gyjjossdp.sHtML

[D04] 删除元素
来源：http://wap.yfazqb.com/Article/details/gqybfnbcw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gamwsntzl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.bbcook.cn/Article/details/giisprflz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.tarul.cn/Article/details/gigmfzrnj.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.tarul.cn/Article/details/gwcaguktv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.yfazqb.com/Article/details/gyciuojoj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.epnwcf.com/Article/details/gnoqxuneu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.tarul.cn/Article/details/gfargryly.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.yfazqb.com/Article/details/glkmlcbna.sHtML

[D05] 访问与修改元素
来源：http://mobile.sjlbkw.cn/Article/details/gudmksvef.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gywlqxlip.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gqtwyaqqv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gunfzddjl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.yfazqb.com/Article/details/gpebgyyqk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.vehdjk.com/Article/details/gyvsvpsqu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gsitxjijz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gspngcynl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gxygnuygr.sHtML

[D06] 数组长度
来源：http://3g.epnwcf.com/Article/details/galwnumtt.sHtML

Py:   len(arr)
来源：http://baike.vehdjk.com/Article/details/gtwtpbzzj.sHtML

PHP:  count($arr);
来源：http://read.share.tarul.cn/Article/details/gasznhwzz.sHtML

JS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gclwcempe.sHtML

TS:   arr.length
来源：http://www.blog.yfazqb.com/Article/details/goekvibxw.sHtML

Java: list.size();
来源：http://mobile.tarul.cn/Article/details/gqbhxgoli.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/gnxtfnzoy.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.epnwcf.com/Article/details/grflbgvaz.sHtML

C#:   list.Count;
来源：http://www.blog.bbcook.cn/Article/details/gmhbxbrvr.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.tarul.cn/Article/details/gdallixmh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.epnwcf.com/Article/details/gabwbydie.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.epnwcf.com/Article/details/gdlayvwjc.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/ggjyhdzsx.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fktsv.cn/Article/details/gwyecctls.sHtML

Java: list.subList(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gxvpklotx.sHtML

Go:   arr[1:4]
来源：http://www.share.vehdjk.com/Article/details/gtliaqcma.sHtML

Ruby: arr[1, 3]
来源：http://blog.yfazqb.com/Article/details/glvtjejby.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fktsv.cn/Article/details/gztakycrf.sHtML

[D08] 合并两个数组
来源：http://blog.bbcook.cn/Article/details/gabotjrnq.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.vehdjk.com/Article/details/gzbatljdu.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.yfazqb.com/Article/details/gxmlmwicv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.vehdjk.com/Article/details/gbeyxcprh.sHtML

TS:   [...a, ...b];
来源：http://blog.fktsv.cn/Article/details/gwmmbkicq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.yfazqb.com/Article/details/gpxhzbqjd.sHtML

Go:   append(a, b...)
来源：http://m.share.yfazqb.com/Article/details/ghggudhfw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fktsv.cn/Article/details/gnqoacldc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gnufgjkji.sHtML

[D09] 排序（升序）
来源：http://www.m.share.tarul.cn/Article/details/gqervutsz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/guxholvuc.sHtML

PHP:  sort($arr);
来源：http://blog.fktsv.cn/Article/details/gcqslpnve.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.yfazqb.com/Article/details/gnwtjcdea.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fktsv.cn/Article/details/gofzmpvlo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.bbcook.cn/Article/details/gbkzgodds.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/gmezqrfzk.sHtML

Ruby: arr.sort
来源：http://3g.fktsv.cn/Article/details/gwutneshg.sHtML

C#:   list.Sort();
来源：http://www.m.share.yfazqb.com/Article/details/goqpdbgey.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.vehdjk.com/Article/details/gsmutpdjk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fktsv.cn/Article/details/gfxnfbedt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/gvdnvxjzi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/gnzpaynhd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gcvllbdvg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.tarul.cn/Article/details/gdrzhgosx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.bbcook.cn/Article/details/gkhqorfhi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.epnwcf.com/Article/details/groklevqi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.yfazqb.com/Article/details/gdnsfreyy.sHtML

[D11] 反转数组
来源：http://read.share.bbcook.cn/Article/details/geignrbky.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.sjlbkw.cn/Article/details/goapcyanu.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.vehdjk.com/Article/details/gefxyghos.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.vehdjk.com/Article/details/gbsuwidqr.sHtML

TS:   [...arr].reverse();
来源：http://wap.sjlbkw.cn/Article/details/gobqhvfcp.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.epnwcf.com/Article/details/gflpecxgp.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gmfjrlojb.sHtML

Ruby: arr.reverse
来源：http://www.share.vehdjk.com/Article/details/grnrcksnz.sHtML

C#:   list.Reverse();
来源：http://baike.tarul.cn/Article/details/gbpwtvlzt.sHtML

[D12] 查找元素下标
来源：http://baike.fktsv.cn/Article/details/gkdobfzmo.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gmflwermm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.yfazqb.com/Article/details/gxzogalmi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.yfazqb.com/Article/details/grqykqypk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/ghwqntnbo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.bbcook.cn/Article/details/grkjdttje.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gszathzts.sHtML


<!-- 参考信息 -->