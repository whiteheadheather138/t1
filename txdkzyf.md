代发 wailian999

Go:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gzjosyzyx.sHtML

Ruby: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gxryrwmhp.sHtML

C#:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gawfyiain.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fktsv.cn/Article/details/gbgyrcjbx.sHtML

Py:   if not data: return
来源：http://m.share.vehdjk.com/Article/details/giesqplyv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fktsv.cn/Article/details/gtybbdnda.sHtML

JS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gldeafhyq.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/gdojhoajd.sHtML

Java: if (data == null) return;
来源：http://3g.fktsv.cn/Article/details/gqwnjqorq.sHtML

Go:   if data == nil { return }
来源：http://www.share.epnwcf.com/Article/details/gaivjalhp.sHtML

Ruby: return if data.nil?
来源：http://3g.tarul.cn/Article/details/gbqlzhklz.sHtML

C#:   if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/grbclicxt.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/grocxbaas.sHtML

C. 函数与作用域
来源：http://mobile.tarul.cn/Article/details/gjtfhwiyx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwuuhfpqe.sHtML

[C01] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/gxeghgokt.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.epnwcf.com/Article/details/gfrcejqza.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gdzqhkwlj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gwloluimm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/godqtkqmt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gvvncxjmf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.bbcook.cn/Article/details/geqxvhtei.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.bbcook.cn/Article/details/gimepohgc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gyjnlmdqv.sHtML

[C02] 默认参数
来源：http://3g.bbcook.cn/Article/details/gydzwkskh.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.bbcook.cn/Article/details/gzfeouyxe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.bbcook.cn/Article/details/giukynzuk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/gheymltwx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gclwztgdg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.vehdjk.com/Article/details/grtdkpxfv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.yfazqb.com/Article/details/guwwvwspm.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.epnwcf.com/Article/details/gwjzvptff.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.bbcook.cn/Article/details/gdhqgzkqh.sHtML

[C03] 可变参数
来源：http://read.share.yfazqb.com/Article/details/gxrvgdoyi.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.epnwcf.com/Article/details/gqleejizf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.tarul.cn/Article/details/gdhbaldyo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/gzzbbkpdf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/ggsxviljw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fktsv.cn/Article/details/grzdbequx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.epnwcf.com/Article/details/gsqjeqxpp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.yfazqb.com/Article/details/gqgrlwkgj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fktsv.cn/Article/details/gigmwkcjm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.yfazqb.com/Article/details/gkmomtnig.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fktsv.cn/Article/details/gvoqigcds.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gyidjgtdr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/gfykdjqvm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.epnwcf.com/Article/details/ghxsxaaor.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.epnwcf.com/Article/details/gnymoyfcp.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.bbcook.cn/Article/details/ghyegfizy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gmiltpuot.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gjfnvnoyk.sHtML

[C05] 返回多个值
来源：http://read.share.sjlbkw.cn/Article/details/gioniqacw.sHtML

Py:   return a, b
来源：http://blog.tarul.cn/Article/details/gerrnijdb.sHtML

PHP:  return [$a, $b];
来源：http://baike.vehdjk.com/Article/details/gcjyfiscv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.yfazqb.com/Article/details/geppplubb.sHtML

TS:   return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gdoxnilcq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.yfazqb.com/Article/details/gnrfcmacc.sHtML

Go:   return a, b
来源：http://blog.fktsv.cn/Article/details/gkuysxdki.sHtML

Ruby: return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gvpslrmpi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.sjlbkw.cn/Article/details/gydiqvffd.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.bbcook.cn/Article/details/gwjgqmkal.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.bbcook.cn/Article/details/gydoymdox.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.sjlbkw.cn/Article/details/gasctojgt.sHtML

JS:   const square = x => x * x;
来源：http://3g.tarul.cn/Article/details/gukpcnnoe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.epnwcf.com/Article/details/gnzqhxbpm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gvvsgswmp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.bbcook.cn/Article/details/gnzzveojm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.vehdjk.com/Article/details/glaosvrvu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/gfhhllsaw.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.epnwcf.com/Article/details/gsqqftybx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.bbcook.cn/Article/details/gkbqrisjx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.epnwcf.com/Article/details/gmuozrcsm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.epnwcf.com/Article/details/gedvofnho.sHtML

TS:   arr.map(String)
来源：http://baike.epnwcf.com/Article/details/grgonecfr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.epnwcf.com/Article/details/ggyxjcllt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fktsv.cn/Article/details/gnhfepwur.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.vehdjk.com/Article/details/gykqtsewg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fktsv.cn/Article/details/gcpeaamsp.sHtML

[C08] 闭包
来源：http://wap.vehdjk.com/Article/details/gldkekhef.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.bbcook.cn/Article/details/gytdxwfhv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.tarul.cn/Article/details/gqtyazeaj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/ghcyroqhd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/glcslavcb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.yfazqb.com/Article/details/gpkspnqla.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.vehdjk.com/Article/details/gclkesuih.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.epnwcf.com/Article/details/ggudzeyto.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gkkrqkrbf.sHtML

[C09] 递归
来源：http://read.share.epnwcf.com/Article/details/gnmzeizqn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/gryusiuad.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.bbcook.cn/Article/details/gprweefka.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/gfnwdjfuc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gybqwuhna.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.bbcook.cn/Article/details/gzrrdszkn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.yfazqb.com/Article/details/gjvfyjbgv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gizdpzeji.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.sjlbkw.cn/Article/details/gqsbcsxou.sHtML

[C10] 变量作用域
来源：http://3g.yfazqb.com/Article/details/gktdktqyy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.epnwcf.com/Article/details/grhpnkqpg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fktsv.cn/Article/details/ghowwwnti.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/gvrmnwlwj.sHtML

TS:   同 JS
来源：http://baike.vehdjk.com/Article/details/gldmrcvmx.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.yfazqb.com/Article/details/gmqhykene.sHtML

Go:   花括号块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gemjpbhxk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.epnwcf.com/Article/details/ghguzuncy.sHtML

C#:   块级作用域
来源：http://mobile.yfazqb.com/Article/details/gorhvtswe.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.tarul.cn/Article/details/gyiadblpw.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/gtdlcuxac.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.vehdjk.com/Article/details/gcecyrwvk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.tarul.cn/Article/details/gnghtjowr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.epnwcf.com/Article/details/gtwzhykpp.sHtML

Java: import java.util.List;
来源：http://blog.tarul.cn/Article/details/giypkiuge.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.vehdjk.com/Article/details/gkxjiyyyp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fktsv.cn/Article/details/gbqfebqcv.sHtML

C#:   using System.Text;
来源：http://baike.sjlbkw.cn/Article/details/gebhgulhm.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/glrqwmkxv.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.tarul.cn/Article/details/gmyhayesl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.sjlbkw.cn/Article/details/gwjsmujbm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/geginkwqb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.epnwcf.com/Article/details/gbeywhcql.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.yfazqb.com/Article/details/gpcwctjit.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/gmupxseaj.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.bbcook.cn/Article/details/gsatqbbvc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.sjlbkw.cn/Article/details/grvdjvdyx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.bbcook.cn/Article/details/gytfhsjgs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.vehdjk.com/Article/details/gipuoghby.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gzcekmyyw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.bbcook.cn/Article/details/gzwzczmkg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gvcgwseza.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/glmymdmqk.sHtML

Go:   func add(a, b int) int
来源：http://3g.epnwcf.com/Article/details/gtcscdcpw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.yfazqb.com/Article/details/gtzjwsfwp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.vehdjk.com/Article/details/gdhaepzaz.sHtML

[C14] 泛型函数
来源：http://www.share.sjlbkw.cn/Article/details/gqwwhprds.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.bbcook.cn/Article/details/gvemovewf.sHtML

PHP:  // 无泛型
来源：http://www.blog.vehdjk.com/Article/details/gkvtdfgec.sHtML

JS:   // 无泛型
来源：http://www.blog.yfazqb.com/Article/details/ghdnhazfk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.vehdjk.com/Article/details/gsvqzmeec.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.bbcook.cn/Article/details/gtiraujls.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.sjlbkw.cn/Article/details/gygtrwwbf.sHtML

Ruby: # 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gxmazelxz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.sjlbkw.cn/Article/details/gasxisflx.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.vehdjk.com/Article/details/gammtjqzy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.bbcook.cn/Article/details/gcqrgizbw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.tarul.cn/Article/details/gewhbpeiz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gyrngnent.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fktsv.cn/Article/details/gzzzotwri.sHtML

Java: // 无解构
来源：http://baike.vehdjk.com/Article/details/ggrxavwud.sHtML

Go:   // 无解构
来源：http://wap.tarul.cn/Article/details/gbdsrslwu.sHtML

Ruby: a, b = pair
来源：http://wap.epnwcf.com/Article/details/gwzuzvkbw.sHtML

C#:   var (a, b) = pair;
来源：http://3g.tarul.cn/Article/details/ggdjgjmiq.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.epnwcf.com/Article/details/gpywfkenu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.sjlbkw.cn/Article/details/gcjclbrss.sHtML

PHP:  // 无重载
来源：http://wap.bbcook.cn/Article/details/gztdzgkbx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.yfazqb.com/Article/details/gfbegbane.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gofjljkdv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.tarul.cn/Article/details/gydqzmtcb.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.epnwcf.com/Article/details/gyfyihlwf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.bbcook.cn/Article/details/ghsqxltmg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fktsv.cn/Article/details/gjcvlcymu.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gqujvtfwb.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.tarul.cn/Article/details/gwberymfz.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gowahiazc.sHtML

[D01] 创建数组 / 列表
来源：http://baike.yfazqb.com/Article/details/gnmhwriba.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.vehdjk.com/Article/details/gtpbfhgcu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.yfazqb.com/Article/details/gkinhzjln.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.bbcook.cn/Article/details/gicdqywbk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.yfazqb.com/Article/details/guugkkmum.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.tarul.cn/Article/details/gmijilxpx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.epnwcf.com/Article/details/ggkdaaozj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.sjlbkw.cn/Article/details/gcmilymkq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.epnwcf.com/Article/details/gztijnvjn.sHtML

[D02] 追加元素到末尾
来源：http://read.share.tarul.cn/Article/details/golytpckn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fktsv.cn/Article/details/gjufxgbaj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.tarul.cn/Article/details/gngxvxsdv.sHtML

JS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/gxrchcufr.sHtML

TS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/geqovcgku.sHtML

Java: list.add(4);
来源：http://3g.yfazqb.com/Article/details/guxoubpbs.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fktsv.cn/Article/details/gonzxqxxz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.bbcook.cn/Article/details/gobzqkvcn.sHtML

C#:   list.Add(4);
来源：http://www.m.share.yfazqb.com/Article/details/gkvrstqjd.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.tarul.cn/Article/details/gyvqnnwdh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.tarul.cn/Article/details/guvjifaui.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.bbcook.cn/Article/details/gzyxdcszw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.vehdjk.com/Article/details/gquipvcao.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gcanlrbau.sHtML

Java: list.add(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gqnhtzvae.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.yfazqb.com/Article/details/gqusvwhql.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.vehdjk.com/Article/details/gcpqpeihy.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/geazjjuxa.sHtML

[D04] 删除元素
来源：http://3g.yfazqb.com/Article/details/gmvkvirdr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.vehdjk.com/Article/details/gipeimini.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.bbcook.cn/Article/details/gqgptnmgx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.tarul.cn/Article/details/gpdkrtkig.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.sjlbkw.cn/Article/details/gsntsbrue.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.bbcook.cn/Article/details/gdzyqanlj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.vehdjk.com/Article/details/gpcqgrxel.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.sjlbkw.cn/Article/details/gnxswxhbc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.tarul.cn/Article/details/grqzixued.sHtML

[D05] 访问与修改元素
来源：http://m.share.vehdjk.com/Article/details/gbxxxqmdn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/goplzlowz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/gvmruskza.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.yfazqb.com/Article/details/gmxcmrohu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.yfazqb.com/Article/details/gjztlbbnn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.vehdjk.com/Article/details/gegkfuydz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gklrurgqw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gytrnsmit.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gumcsodjn.sHtML

[D06] 数组长度
来源：http://m.share.yfazqb.com/Article/details/grjsspenh.sHtML

Py:   len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gfyrfkeqy.sHtML

PHP:  count($arr);
来源：http://m.share.tarul.cn/Article/details/gjzjzrlty.sHtML

JS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gsmkkxgtn.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gahiifpdy.sHtML

Java: list.size();
来源：http://m.share.tarul.cn/Article/details/gsrabupcs.sHtML

Go:   len(arr)
来源：http://blog.tarul.cn/Article/details/gglopfbnv.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.yfazqb.com/Article/details/gcxfsnaad.sHtML

C#:   list.Count;
来源：http://baike.yfazqb.com/Article/details/gcmdpzwtg.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.sjlbkw.cn/Article/details/gegfueeao.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.sjlbkw.cn/Article/details/ggpdcgsos.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.vehdjk.com/Article/details/gegzdyxho.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gyhxgaoyt.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gyfrzzkkw.sHtML

Java: list.subList(1, 4);
来源：http://wap.epnwcf.com/Article/details/gtfzzkjnm.sHtML

Go:   arr[1:4]
来源：http://mobile.vehdjk.com/Article/details/gpsbnickm.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.bbcook.cn/Article/details/gbyatquut.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.sjlbkw.cn/Article/details/gguqdkehx.sHtML

[D08] 合并两个数组
来源：http://blog.yfazqb.com/Article/details/ghfrscxpx.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.yfazqb.com/Article/details/gestkscma.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fktsv.cn/Article/details/gpzfhdded.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.sjlbkw.cn/Article/details/gjlcgsdlm.sHtML

TS:   [...a, ...b];
来源：http://m.share.bbcook.cn/Article/details/gianhpivq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.vehdjk.com/Article/details/gmcklwzop.sHtML

Go:   append(a, b...)
来源：http://read.share.fktsv.cn/Article/details/gpoedvchf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fktsv.cn/Article/details/goohusulr.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fktsv.cn/Article/details/gaanrumsj.sHtML

[D09] 排序（升序）
来源：http://www.m.share.tarul.cn/Article/details/gcqlrhskv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gwnryugrt.sHtML

PHP:  sort($arr);
来源：http://3g.fktsv.cn/Article/details/glbpylyig.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.yfazqb.com/Article/details/gwiuxitpf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.bbcook.cn/Article/details/ghftlhrjg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fktsv.cn/Article/details/ganvcbggc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gzhpflhph.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/ggklgxlcm.sHtML

C#:   list.Sort();
来源：http://www.share.vehdjk.com/Article/details/gzzhdvrce.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.bbcook.cn/Article/details/glhxdmxhx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fktsv.cn/Article/details/gkqxzsdef.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.bbcook.cn/Article/details/gkoiiozlp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.epnwcf.com/Article/details/goomfuhpo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/garwchrtr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.vehdjk.com/Article/details/gscpfalls.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.yfazqb.com/Article/details/grnornvyy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.vehdjk.com/Article/details/gfypzwvce.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.vehdjk.com/Article/details/gduvdqhge.sHtML

[D11] 反转数组
来源：http://read.share.vehdjk.com/Article/details/gjmkquibc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fktsv.cn/Article/details/gjuseulgl.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fktsv.cn/Article/details/gdpfkenno.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwphacrxh.sHtML

TS:   [...arr].reverse();
来源：http://blog.sjlbkw.cn/Article/details/gvahmxokq.sHtML

Java: Collections.reverse(list);
来源：http://3g.sjlbkw.cn/Article/details/gfxwdtijz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.vehdjk.com/Article/details/gmxypitzt.sHtML

Ruby: arr.reverse
来源：http://wap.epnwcf.com/Article/details/gnafeceqt.sHtML

C#:   list.Reverse();
来源：http://www.share.sjlbkw.cn/Article/details/gobqsnheu.sHtML

[D12] 查找元素下标
来源：http://baike.fktsv.cn/Article/details/gfxeipkqw.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.bbcook.cn/Article/details/gefvsljht.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.yfazqb.com/Article/details/gczcylnix.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.yfazqb.com/Article/details/gjizvntsi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gvsvqytty.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.yfazqb.com/Article/details/gsgqtdxsw.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.tarul.cn/Article/details/gdjwtfrqv.sHtML

Ruby: arr.index(x)
来源：http://baike.epnwcf.com/Article/details/gtntyvtau.sHtML

C#:   list.IndexOf(x);
来源：http://wap.vehdjk.com/Article/details/gdbxvzzoz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.epnwcf.com/Article/details/gnygnwtxr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.tarul.cn/Article/details/gyowondbw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.tarul.cn/Article/details/gnojryluu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.vehdjk.com/Article/details/gobetxfvv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.tarul.cn/Article/details/gircfmnhl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.vehdjk.com/Article/details/gstjbfbeg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.vehdjk.com/Article/details/griiroaee.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.sjlbkw.cn/Article/details/ggxcfdbbu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.tarul.cn/Article/details/gnzwmnvkg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.epnwcf.com/Article/details/glbltyasv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.vehdjk.com/Article/details/gexjhxjlt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/gtdafgmrt.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/ggbunjurk.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/ghtdlzdli.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.tarul.cn/Article/details/gqwjkgplp.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gbtkblidw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.tarul.cn/Article/details/ghmfburzk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gjbrdirxf.sHtML

[D15] 去重
来源：http://www.m.share.bbcook.cn/Article/details/gpjxxieux.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gyvqmodiu.sHtML

PHP:  array_unique($arr);
来源：http://3g.vehdjk.com/Article/details/gxyqguupi.sHtML

JS:   [...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/ganjajelh.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/gysylomdi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.yfazqb.com/Article/details/gxrjlujgw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fktsv.cn/Article/details/gtliuknxt.sHtML

Ruby: arr.uniq
来源：http://blog.sjlbkw.cn/Article/details/gequohwvb.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.bbcook.cn/Article/details/gmjcjpyrm.sHtML

[D16] 求和与平均值
来源：http://www.m.share.sjlbkw.cn/Article/details/gbovvwvvg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gvqumvqtr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.tarul.cn/Article/details/gevpdbyik.sHtML


<!-- 参考信息 -->