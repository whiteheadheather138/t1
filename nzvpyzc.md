代发 wailian999

Py:   if not data: return
来源：http://blog.sjlbkw.cn/Article/details/gwmtgxnae.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.sjlbkw.cn/Article/details/gpqzreyre.sHtML

JS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/gbmrmcybt.sHtML

TS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/gaigbvetu.sHtML

Java: if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gsgsbkhtp.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fktsv.cn/Article/details/gpmvfczjm.sHtML

Ruby: return if data.nil?
来源：http://read.share.vehdjk.com/Article/details/gsflelvmq.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/gclomucjn.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gwvtrjufi.sHtML

C. 函数与作用域
来源：http://blog.sjlbkw.cn/Article/details/grkaukanw.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gdvfanikh.sHtML

[C01] 定义函数
来源：http://m.share.bbcook.cn/Article/details/grxqixamq.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.sjlbkw.cn/Article/details/gwfksoqmw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gisealrru.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gprbdwvqv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gdyallqow.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/giafaaqsl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.bbcook.cn/Article/details/gbffgrncq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.yfazqb.com/Article/details/gqxpegqco.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gdfljewce.sHtML

[C02] 默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/glqtwijwq.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fktsv.cn/Article/details/grkmxzkur.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.sjlbkw.cn/Article/details/gipozdlgy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gzzvipmfu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gambgthtb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.bbcook.cn/Article/details/gtcxkjwwh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.epnwcf.com/Article/details/gznzlkave.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.epnwcf.com/Article/details/ggxwlwdji.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.tarul.cn/Article/details/gmouimswn.sHtML

[C03] 可变参数
来源：http://3g.yfazqb.com/Article/details/gymtvocix.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.sjlbkw.cn/Article/details/grlghuwxl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.epnwcf.com/Article/details/glxruqxpg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gkyqckkqa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/gsucqrnds.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fktsv.cn/Article/details/gwcqqpxkx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.bbcook.cn/Article/details/goackeuny.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.yfazqb.com/Article/details/gdzrfafdo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.tarul.cn/Article/details/gtddqkljs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.tarul.cn/Article/details/gqcqixlfs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.bbcook.cn/Article/details/gxdwaqxev.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.vehdjk.com/Article/details/gqhojdpny.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.yfazqb.com/Article/details/gxpqoobob.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.bbcook.cn/Article/details/gqhoyxtxp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.tarul.cn/Article/details/gyriserpl.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.tarul.cn/Article/details/gcpzioehu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gsvdrzbwf.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gucgbpgzg.sHtML

[C05] 返回多个值
来源：http://wap.tarul.cn/Article/details/gvgfwuvsq.sHtML

Py:   return a, b
来源：http://blog.tarul.cn/Article/details/ghmuzkwhp.sHtML

PHP:  return [$a, $b];
来源：http://baike.yfazqb.com/Article/details/gckcfnmnx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.yfazqb.com/Article/details/ggteqvszt.sHtML

TS:   return { a, b };
来源：http://blog.fktsv.cn/Article/details/gfqkxrmnv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.tarul.cn/Article/details/gqxdexkow.sHtML

Go:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/ggyletvzc.sHtML

Ruby: return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gokizimfi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.bbcook.cn/Article/details/gjoamxxbb.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fktsv.cn/Article/details/gjcnbzzwn.sHtML

Py:   square = lambda x: x * x
来源：http://blog.tarul.cn/Article/details/gzqlxcnkl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.epnwcf.com/Article/details/gwzjgnxes.sHtML

JS:   const square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gkivwanij.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.epnwcf.com/Article/details/gfevyzrym.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.yfazqb.com/Article/details/gedlmloqx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.tarul.cn/Article/details/gjqomzfus.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.bbcook.cn/Article/details/gqsqdzdfq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fktsv.cn/Article/details/gwyjsqtti.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fktsv.cn/Article/details/gbnbndvha.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fktsv.cn/Article/details/gbbrmontr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fktsv.cn/Article/details/ghctjunig.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.vehdjk.com/Article/details/gqtyjbpcg.sHtML

TS:   arr.map(String)
来源：http://mobile.fktsv.cn/Article/details/ggjpijfgy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fktsv.cn/Article/details/gmoivoiuu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fktsv.cn/Article/details/gasnxugiq.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.bbcook.cn/Article/details/gkvyjewxr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.sjlbkw.cn/Article/details/gextiykxt.sHtML

[C08] 闭包
来源：http://www.blog.fktsv.cn/Article/details/gdxnfftli.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.epnwcf.com/Article/details/givvibdec.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwfvvlhro.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gklwxmmdg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gfbeonrdc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fktsv.cn/Article/details/gjyctmecf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fktsv.cn/Article/details/galqiqxoj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.yfazqb.com/Article/details/gdhfmynyi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gabuisxlp.sHtML

[C09] 递归
来源：http://www.blog.vehdjk.com/Article/details/ggvcglwaj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.sjlbkw.cn/Article/details/glpzitfnl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.tarul.cn/Article/details/gmmukoaom.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/goevmaxxv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/ggufzsfsf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/gzfzlpemf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fktsv.cn/Article/details/gimcfjdkk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/gzyngdvai.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.yfazqb.com/Article/details/gbcwstgpq.sHtML

[C10] 变量作用域
来源：http://read.share.yfazqb.com/Article/details/gxeeeveye.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.epnwcf.com/Article/details/ggngxftdm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.sjlbkw.cn/Article/details/gydwlxbog.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gqmlpnrkk.sHtML

TS:   同 JS
来源：http://blog.sjlbkw.cn/Article/details/glljvxesb.sHtML

Java: 方法内为块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gdsfrjzbx.sHtML

Go:   花括号块级作用域
来源：http://baike.tarul.cn/Article/details/gfbkqlrsy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fktsv.cn/Article/details/gxzoesdnx.sHtML

C#:   块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gkheuhpxd.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fktsv.cn/Article/details/gyqikxpln.sHtML

Py:   from module import func
来源：http://read.share.tarul.cn/Article/details/gexwvrdnd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.bbcook.cn/Article/details/gzlmyeoze.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.epnwcf.com/Article/details/gjmvblfby.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.tarul.cn/Article/details/gcnlqhkio.sHtML

Java: import java.util.List;
来源：http://m.share.sjlbkw.cn/Article/details/gosuqjper.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.yfazqb.com/Article/details/gmgalkiyh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.sjlbkw.cn/Article/details/gjfapldla.sHtML

C#:   using System.Text;
来源：http://3g.tarul.cn/Article/details/gbvmfejjc.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.tarul.cn/Article/details/gmnhwazlq.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.yfazqb.com/Article/details/ggnrseele.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.vehdjk.com/Article/details/gmrkdqlng.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gludxpcpd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.bbcook.cn/Article/details/gijjtqvhp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.yfazqb.com/Article/details/gjcpiueru.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fktsv.cn/Article/details/gthocazxy.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.sjlbkw.cn/Article/details/grmywaenv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.bbcook.cn/Article/details/gxtskxpoi.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.epnwcf.com/Article/details/gvzscvkxj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.tarul.cn/Article/details/gnttybwbx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/grfpwbzwi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fktsv.cn/Article/details/ghgfmztaj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gswmbgjwg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gaaabchey.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.yfazqb.com/Article/details/gkgtnxgwy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.epnwcf.com/Article/details/grkugnglr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.bbcook.cn/Article/details/goajfjdow.sHtML

[C14] 泛型函数
来源：http://read.share.epnwcf.com/Article/details/gujltvrhz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.vehdjk.com/Article/details/gmkkteihd.sHtML

PHP:  // 无泛型
来源：http://www.blog.fktsv.cn/Article/details/galmllzco.sHtML

JS:   // 无泛型
来源：http://baike.bbcook.cn/Article/details/gkupvqeyl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.yfazqb.com/Article/details/gpseroexi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.sjlbkw.cn/Article/details/ggwpzlqiv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgsoxakg.sHtML

Ruby: # 无泛型
来源：http://blog.fktsv.cn/Article/details/gjldjsien.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.epnwcf.com/Article/details/grhqhfltp.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.tarul.cn/Article/details/ggjnzungr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.vehdjk.com/Article/details/gffijnyes.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.vehdjk.com/Article/details/gmxattvof.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.tarul.cn/Article/details/gnnfnwdpb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.bbcook.cn/Article/details/gjeazahox.sHtML

Java: // 无解构
来源：http://wap.sjlbkw.cn/Article/details/gwafkkist.sHtML

Go:   // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/ghwqhdfbh.sHtML

Ruby: a, b = pair
来源：http://3g.fktsv.cn/Article/details/gpmwjahgm.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.tarul.cn/Article/details/ghbbwocmv.sHtML

[C16] 函数 / 方法重载
来源：http://wap.vehdjk.com/Article/details/gygcsjugg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.tarul.cn/Article/details/gwbzgzkbb.sHtML

PHP:  // 无重载
来源：http://wap.epnwcf.com/Article/details/gzgqlhciy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fktsv.cn/Article/details/gttjgstpi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.yfazqb.com/Article/details/gieljgoco.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.yfazqb.com/Article/details/gsafwcken.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.epnwcf.com/Article/details/gdwyaicbl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fktsv.cn/Article/details/gilfeaegw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.bbcook.cn/Article/details/guseuirea.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gedhpfkgh.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.yfazqb.com/Article/details/gsqicwdol.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gizxioedf.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.sjlbkw.cn/Article/details/gwravtsuf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.bbcook.cn/Article/details/geuvgtpgf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.yfazqb.com/Article/details/gnncwdeay.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.yfazqb.com/Article/details/glmllgrty.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.bbcook.cn/Article/details/gcilnykda.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fktsv.cn/Article/details/grlwzpikd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.sjlbkw.cn/Article/details/gdtblwgyk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.sjlbkw.cn/Article/details/ghdmrwmbu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.tarul.cn/Article/details/gmyvraudq.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.yfazqb.com/Article/details/gkccoosqc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.bbcook.cn/Article/details/gepxnqnrb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fktsv.cn/Article/details/ghzpztdyy.sHtML

JS:   arr.push(4);
来源：http://read.share.bbcook.cn/Article/details/gpqfouxea.sHtML

TS:   arr.push(4);
来源：http://www.m.share.bbcook.cn/Article/details/gpgfwyjsa.sHtML

Java: list.add(4);
来源：http://blog.vehdjk.com/Article/details/gdorajzon.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.vehdjk.com/Article/details/gtzykrvps.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.epnwcf.com/Article/details/gbtvfoyyy.sHtML

C#:   list.Add(4);
来源：http://read.share.tarul.cn/Article/details/gpeavrukr.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.yfazqb.com/Article/details/gozdnljzf.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gfpykxpys.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.yfazqb.com/Article/details/grtzvmjyu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.epnwcf.com/Article/details/gfxnmzclo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.bbcook.cn/Article/details/grwlwxkyt.sHtML

Java: list.add(0, 0);
来源：http://baike.fktsv.cn/Article/details/gjnwnfxkk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.sjlbkw.cn/Article/details/gjzczuvbx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.vehdjk.com/Article/details/gjldcpdej.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gynsyprkf.sHtML

[D04] 删除元素
来源：http://baike.bbcook.cn/Article/details/gyeyloykc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.bbcook.cn/Article/details/gjtssgctv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.tarul.cn/Article/details/gcfytcvzk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.vehdjk.com/Article/details/gwozcidzg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gjcdoztxs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.bbcook.cn/Article/details/gncbbgunr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.bbcook.cn/Article/details/gzgdatxsc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.epnwcf.com/Article/details/goxwosqsf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.epnwcf.com/Article/details/gcdxlrncu.sHtML

[D05] 访问与修改元素
来源：http://blog.sjlbkw.cn/Article/details/gheasiuvn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpyiodsi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gohejesbz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/ggwgaehve.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.epnwcf.com/Article/details/gggtxyhbv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fktsv.cn/Article/details/gmgxrfiyj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/grmrvcuyg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gjetrnqus.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gaiwuitpy.sHtML

[D06] 数组长度
来源：http://mobile.epnwcf.com/Article/details/gctlqjbns.sHtML

Py:   len(arr)
来源：http://read.share.vehdjk.com/Article/details/gyitgxbwh.sHtML

PHP:  count($arr);
来源：http://3g.tarul.cn/Article/details/gmdhykjab.sHtML

JS:   arr.length
来源：http://read.share.bbcook.cn/Article/details/gsdntglsd.sHtML

TS:   arr.length
来源：http://www.m.share.fktsv.cn/Article/details/gihwtlmpv.sHtML

Java: list.size();
来源：http://read.share.sjlbkw.cn/Article/details/gyqefnedq.sHtML

Go:   len(arr)
来源：http://wap.tarul.cn/Article/details/gwabtustj.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fktsv.cn/Article/details/gkycuuouf.sHtML

C#:   list.Count;
来源：http://3g.sjlbkw.cn/Article/details/grtusuzln.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.bbcook.cn/Article/details/glrigkxiv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/gwgjyrpdo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gwlgluwrp.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gikewcqzq.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gzksdepoh.sHtML

Java: list.subList(1, 4);
来源：http://blog.vehdjk.com/Article/details/gcdztxyur.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fktsv.cn/Article/details/gdshpvgvg.sHtML

Ruby: arr[1, 3]
来源：http://3g.epnwcf.com/Article/details/gkfpaedxp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.yfazqb.com/Article/details/goqxuzceq.sHtML

[D08] 合并两个数组
来源：http://mobile.vehdjk.com/Article/details/gyrbvoaop.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.bbcook.cn/Article/details/gatkiufpu.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.tarul.cn/Article/details/ggppfeakb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.bbcook.cn/Article/details/ggbvnqfjc.sHtML

TS:   [...a, ...b];
来源：http://m.share.tarul.cn/Article/details/geifpsuya.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.yfazqb.com/Article/details/gqwrdchnp.sHtML

Go:   append(a, b...)
来源：http://3g.yfazqb.com/Article/details/gbfdshmrr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.epnwcf.com/Article/details/gpggfijuf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gqlnzddpi.sHtML

[D09] 排序（升序）
来源：http://wap.yfazqb.com/Article/details/gfmjqaqro.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/gibdgtxgf.sHtML

PHP:  sort($arr);
来源：http://www.blog.vehdjk.com/Article/details/ganbmeqla.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fktsv.cn/Article/details/gckfeyrkm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.sjlbkw.cn/Article/details/ggyqfwqbd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.tarul.cn/Article/details/gxhnpivah.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gfddacqzx.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gnefwuozn.sHtML

C#:   list.Sort();
来源：http://mobile.sjlbkw.cn/Article/details/guqflktxs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.bbcook.cn/Article/details/gubgeelwb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.sjlbkw.cn/Article/details/gekkqrktn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/gtjldntov.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/gducfqmdh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.sjlbkw.cn/Article/details/gdvlnfecs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fktsv.cn/Article/details/guowrgkgf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fktsv.cn/Article/details/gcaoecqyw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.epnwcf.com/Article/details/gokwkoqru.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.epnwcf.com/Article/details/gfpicsgcd.sHtML

[D11] 反转数组
来源：http://wap.fktsv.cn/Article/details/gsoarrglz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.bbcook.cn/Article/details/gknqqanov.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.yfazqb.com/Article/details/gwhyuhwlk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.vehdjk.com/Article/details/gtuubfjub.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhklikmm.sHtML

Java: Collections.reverse(list);
来源：http://baike.fktsv.cn/Article/details/gwooqeymc.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fktsv.cn/Article/details/gdrvfzkmo.sHtML

Ruby: arr.reverse
来源：http://3g.vehdjk.com/Article/details/gfcdwtvtf.sHtML

C#:   list.Reverse();
来源：http://mobile.tarul.cn/Article/details/gfjdgjvmu.sHtML

[D12] 查找元素下标
来源：http://baike.bbcook.cn/Article/details/gongkvkbu.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.bbcook.cn/Article/details/gtvkboawo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.tarul.cn/Article/details/gedkkezmz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/gfmvhedbn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/ghvbfgyyo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.tarul.cn/Article/details/gttqjdqgn.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.bbcook.cn/Article/details/gpdtqqltm.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwiizkijz.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fktsv.cn/Article/details/gchecwffl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.sjlbkw.cn/Article/details/gecdiritp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/gsozbjvoa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.tarul.cn/Article/details/gehlkdklu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/ghuuenqle.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/gtaeslmdu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fktsv.cn/Article/details/gjambnilp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.vehdjk.com/Article/details/gbvfagrzn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.bbcook.cn/Article/details/gwhmewitg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gtgylcuod.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fktsv.cn/Article/details/gccsvqvbd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gtqblmtis.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.epnwcf.com/Article/details/gkkfhmkas.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gcygdvzgo.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gebpyshrx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.bbcook.cn/Article/details/gtfgpyfkn.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gbtsqgent.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.epnwcf.com/Article/details/gwkqtfmjt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gqotbaiyt.sHtML

[D15] 去重
来源：http://www.share.epnwcf.com/Article/details/gkejhpsrx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gbkibvqjf.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fktsv.cn/Article/details/ggnwlrzyk.sHtML

JS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/gtsupoood.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gdvutmmvl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.epnwcf.com/Article/details/gaijkovrj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.sjlbkw.cn/Article/details/gvrbqicqb.sHtML

Ruby: arr.uniq
来源：http://www.share.vehdjk.com/Article/details/gmhxaguhi.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.yfazqb.com/Article/details/gxtkmwkrw.sHtML

[D16] 求和与平均值
来源：http://wap.yfazqb.com/Article/details/gslsoaynb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.yfazqb.com/Article/details/ggmvrtoct.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.sjlbkw.cn/Article/details/gujcumrlf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.yfazqb.com/Article/details/gzqagxkzz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gywxgzywr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.tarul.cn/Article/details/gpyvvzygi.sHtML

Go:   // 手写循环累加
来源：http://www.blog.vehdjk.com/Article/details/gpzbjqygz.sHtML


<!-- 参考信息 -->