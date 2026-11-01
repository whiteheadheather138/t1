代发 wailian999

[B13] 判断是否为数字
来源：http://m.share.tarul.cn/Article/details/grnxyllas.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.bbcook.cn/Article/details/gxxjrtboh.sHtML

PHP:  is_numeric($x)
来源：http://mobile.epnwcf.com/Article/details/gmeepjbob.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/gnnrcwaor.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gdkuhkzvy.sHtML

Java: x instanceof Number
来源：http://www.blog.sjlbkw.cn/Article/details/gfzjfexsy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.tarul.cn/Article/details/gbzyosumy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmuhugube.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fktsv.cn/Article/details/gnoycnztt.sHtML

[B14] 判断值是否在集合内
来源：http://3g.sjlbkw.cn/Article/details/gywyzxarc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.bbcook.cn/Article/details/gsnyszxwo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.tarul.cn/Article/details/gulbbovgw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gmzgxppcl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gpjrobyfz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fktsv.cn/Article/details/ghvrlijfi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.vehdjk.com/Article/details/gyihfgowv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.epnwcf.com/Article/details/gnalxoevv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/ginpursbb.sHtML

[B15] 布尔运算与取反
来源：http://baike.bbcook.cn/Article/details/gzpgmpvpf.sHtML

Py:   a and b or not c
来源：http://read.share.yfazqb.com/Article/details/gbpxpbsym.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.vehdjk.com/Article/details/gtlkfoxtn.sHtML

JS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gxjuvhnti.sHtML

TS:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gmitvbrpj.sHtML

Java: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gogqceevs.sHtML

Go:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/ghismaxnz.sHtML

Ruby: a && b || !c
来源：http://wap.vehdjk.com/Article/details/glefbwlto.sHtML

C#:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gqoqvgsxw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.vehdjk.com/Article/details/gcrxssttg.sHtML

Py:   if not data: return
来源：http://baike.vehdjk.com/Article/details/gtmyniqtc.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.tarul.cn/Article/details/geaqqkcph.sHtML

JS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/gmpiwuqoh.sHtML

TS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gzgplvceo.sHtML

Java: if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gxcljhxwn.sHtML

Go:   if data == nil { return }
来源：http://www.blog.bbcook.cn/Article/details/gldoemyiq.sHtML

Ruby: return if data.nil?
来源：http://3g.sjlbkw.cn/Article/details/gbdsjprdv.sHtML

C#:   if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gzapbzafb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwidgqiah.sHtML

C. 函数与作用域
来源：http://www.m.share.fktsv.cn/Article/details/gqnzifync.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvkbtabuf.sHtML

[C01] 定义函数
来源：http://3g.tarul.cn/Article/details/gdzbeyjki.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.tarul.cn/Article/details/ghzvakwim.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gnhzcpimq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gozsbnqtf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gbwpohtml.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gvkdckxeo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.epnwcf.com/Article/details/gwmffdpha.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fktsv.cn/Article/details/ghnwzrnia.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gsbnpvmhy.sHtML

[C02] 默认参数
来源：http://read.share.epnwcf.com/Article/details/gyorlvxdw.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.epnwcf.com/Article/details/ggwwpupyr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.sjlbkw.cn/Article/details/govuepcer.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/gbnqcvhxm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gbaxtsfue.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fktsv.cn/Article/details/geakftqab.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.bbcook.cn/Article/details/gabupnhjx.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.sjlbkw.cn/Article/details/gsyuylunj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.sjlbkw.cn/Article/details/gwldafxou.sHtML

[C03] 可变参数
来源：http://baike.bbcook.cn/Article/details/gmxzvzutu.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.tarul.cn/Article/details/gifkuauph.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fktsv.cn/Article/details/gcsmelgcb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.yfazqb.com/Article/details/grbnmdmuq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/gzlqokcjn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.epnwcf.com/Article/details/gphhtqaii.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.bbcook.cn/Article/details/gayavhqnq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.epnwcf.com/Article/details/gmtuobkgi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.yfazqb.com/Article/details/gbhyniopu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fktsv.cn/Article/details/gxocfvbgh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fktsv.cn/Article/details/geiekpsqg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.bbcook.cn/Article/details/gcjvmefye.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gqkbwehxp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.yfazqb.com/Article/details/gwrvfzlqr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.sjlbkw.cn/Article/details/ghslessdo.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.yfazqb.com/Article/details/gdzvqjhsh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/giakkxaji.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gugenwczw.sHtML

[C05] 返回多个值
来源：http://3g.fktsv.cn/Article/details/geodlttxw.sHtML

Py:   return a, b
来源：http://wap.tarul.cn/Article/details/gihxhpult.sHtML

PHP:  return [$a, $b];
来源：http://wap.fktsv.cn/Article/details/gagwjaltc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gxtcjjhzh.sHtML

TS:   return { a, b };
来源：http://www.share.vehdjk.com/Article/details/gkqhchvnw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.vehdjk.com/Article/details/gtfggixgl.sHtML

Go:   return a, b
来源：http://www.share.bbcook.cn/Article/details/gghyrnanl.sHtML

Ruby: return a, b
来源：http://blog.fktsv.cn/Article/details/gstbaqrky.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fktsv.cn/Article/details/gnkzgukgs.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.sjlbkw.cn/Article/details/gljtcfsbb.sHtML

Py:   square = lambda x: x * x
来源：http://3g.bbcook.cn/Article/details/grybnduks.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.vehdjk.com/Article/details/gbdsjvrcz.sHtML

JS:   const square = x => x * x;
来源：http://baike.epnwcf.com/Article/details/gsqbrliam.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.bbcook.cn/Article/details/gqjnamdvm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.bbcook.cn/Article/details/gjchamcpr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.sjlbkw.cn/Article/details/gacwapysk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.bbcook.cn/Article/details/gfrqdykjn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gntnvlnjd.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.tarul.cn/Article/details/gvmdjsvbt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.yfazqb.com/Article/details/gnxaakvcd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fktsv.cn/Article/details/gmjtxhabe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.tarul.cn/Article/details/guqbkkere.sHtML

TS:   arr.map(String)
来源：http://mobile.bbcook.cn/Article/details/gphwpcsxu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.epnwcf.com/Article/details/ggqjccfuh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.vehdjk.com/Article/details/gldjuiqck.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.vehdjk.com/Article/details/gupkoewtp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.tarul.cn/Article/details/grmonlytx.sHtML

[C08] 闭包
来源：http://baike.epnwcf.com/Article/details/gjskqxuih.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.vehdjk.com/Article/details/gtmfyruuu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fktsv.cn/Article/details/gfuxeqsuk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gdvgswqpd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gjyuejawd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.bbcook.cn/Article/details/gbnysixfv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.tarul.cn/Article/details/gnreuudmr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.bbcook.cn/Article/details/gunsfpnvm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gtirzvlav.sHtML

[C09] 递归
来源：http://blog.vehdjk.com/Article/details/geybxkijx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gnoydqrxz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fktsv.cn/Article/details/guhpcvtgq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/gwibgrsij.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/ggrlcrkto.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.tarul.cn/Article/details/geqgzvebq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.tarul.cn/Article/details/gjzdelkot.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gpofuixai.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.bbcook.cn/Article/details/gfqhvpdco.sHtML

[C10] 变量作用域
来源：http://blog.sjlbkw.cn/Article/details/gtfumdqrk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.sjlbkw.cn/Article/details/gcwguvgir.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.tarul.cn/Article/details/gofdliwue.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.tarul.cn/Article/details/grtvqvjpc.sHtML

TS:   同 JS
来源：http://wap.tarul.cn/Article/details/gvyzskdwp.sHtML

Java: 方法内为块级作用域
来源：http://baike.fktsv.cn/Article/details/gigjtmbvz.sHtML

Go:   花括号块级作用域
来源：http://blog.epnwcf.com/Article/details/grbfzjpre.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.sjlbkw.cn/Article/details/gfufgsxgp.sHtML

C#:   块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gsdhucjnp.sHtML

[C11] 模块导入与导出
来源：http://3g.vehdjk.com/Article/details/gsvyzusjw.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/gejmecrzh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fktsv.cn/Article/details/gsxcwluxg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/gqiluxofm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fktsv.cn/Article/details/gvcetdwcn.sHtML

Java: import java.util.List;
来源：http://mobile.tarul.cn/Article/details/gmshjqvfw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.tarul.cn/Article/details/gmcuctsbc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fktsv.cn/Article/details/gvrucdeye.sHtML

C#:   using System.Text;
来源：http://baike.yfazqb.com/Article/details/gutgqdxrx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.epnwcf.com/Article/details/gsgemdbad.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.sjlbkw.cn/Article/details/gmrtbliwe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.sjlbkw.cn/Article/details/gminwegbf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.bbcook.cn/Article/details/gnthudhdu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gjwetautf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.tarul.cn/Article/details/gadsgahle.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.tarul.cn/Article/details/ggzbqfxhh.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.bbcook.cn/Article/details/gtbtjxhse.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.sjlbkw.cn/Article/details/grrzdvjbf.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.tarul.cn/Article/details/gnlazemtk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fktsv.cn/Article/details/govytmtau.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gzuiwvrnj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fktsv.cn/Article/details/gxguynjrj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/grirywkaz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gdzirydgv.sHtML

Go:   func add(a, b int) int
来源：http://wap.tarul.cn/Article/details/gaijehjjc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fktsv.cn/Article/details/gistanmik.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.vehdjk.com/Article/details/guwhribtu.sHtML

[C14] 泛型函数
来源：http://www.m.share.tarul.cn/Article/details/gwbyltpas.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.tarul.cn/Article/details/gcshhsxqh.sHtML

PHP:  // 无泛型
来源：http://baike.tarul.cn/Article/details/gxodmyfpo.sHtML

JS:   // 无泛型
来源：http://baike.fktsv.cn/Article/details/glafjwulk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.vehdjk.com/Article/details/gynmffgia.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.bbcook.cn/Article/details/gzusgohxz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.yfazqb.com/Article/details/gsxvhjato.sHtML

Ruby: # 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gxtpksway.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.yfazqb.com/Article/details/gaqlvlfju.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.vehdjk.com/Article/details/gbxsntuey.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.sjlbkw.cn/Article/details/gkzgxgdbe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.epnwcf.com/Article/details/guvosraut.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.yfazqb.com/Article/details/gfcdusmes.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.bbcook.cn/Article/details/ggzyetrqh.sHtML

Java: // 无解构
来源：http://wap.tarul.cn/Article/details/guagublgk.sHtML

Go:   // 无解构
来源：http://wap.yfazqb.com/Article/details/gfdlznlde.sHtML

Ruby: a, b = pair
来源：http://blog.sjlbkw.cn/Article/details/gzuexngpd.sHtML

C#:   var (a, b) = pair;
来源：http://baike.tarul.cn/Article/details/gdzbghrez.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.epnwcf.com/Article/details/glrynicmu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fktsv.cn/Article/details/glylyzmav.sHtML

PHP:  // 无重载
来源：http://mobile.vehdjk.com/Article/details/gszsttkzr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.vehdjk.com/Article/details/gnpggvhec.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.vehdjk.com/Article/details/gdumphbtu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.epnwcf.com/Article/details/gmmrtuyuu.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.bbcook.cn/Article/details/gicfylisw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.yfazqb.com/Article/details/gaibtpaiw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.sjlbkw.cn/Article/details/gaijkyzsy.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gexhleioy.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.epnwcf.com/Article/details/gfaicrxyz.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/grqokeink.sHtML

[D01] 创建数组 / 列表
来源：http://blog.sjlbkw.cn/Article/details/glgkqdvdq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fktsv.cn/Article/details/gpphxipga.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gbbduvuqa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/geplihfsy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.epnwcf.com/Article/details/gwodmxunj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fktsv.cn/Article/details/gyvejnnkr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.tarul.cn/Article/details/gkezwtdhq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.yfazqb.com/Article/details/gtulneyiq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.epnwcf.com/Article/details/gqdlxvryi.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.epnwcf.com/Article/details/gwizosgva.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.vehdjk.com/Article/details/ghccixmyb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.yfazqb.com/Article/details/gdudgklez.sHtML

JS:   arr.push(4);
来源：http://blog.epnwcf.com/Article/details/gdtpfenhw.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fktsv.cn/Article/details/giqzvgkeh.sHtML

Java: list.add(4);
来源：http://m.share.sjlbkw.cn/Article/details/ggafwrhjm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gluaqosbc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.vehdjk.com/Article/details/gvdxdaxlo.sHtML

C#:   list.Add(4);
来源：http://baike.tarul.cn/Article/details/gjqlkcxdo.sHtML

[D03] 在指定位置插入元素
来源：http://blog.bbcook.cn/Article/details/gczjkvjom.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gsxkaeaej.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.sjlbkw.cn/Article/details/gmnozegpu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.vehdjk.com/Article/details/gnoxglpyy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.tarul.cn/Article/details/gmsibjgmj.sHtML

Java: list.add(0, 0);
来源：http://m.share.fktsv.cn/Article/details/grjcxhcbo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnuvoqmq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.tarul.cn/Article/details/gyglhaglj.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.tarul.cn/Article/details/goljqcnmy.sHtML

[D04] 删除元素
来源：http://wap.tarul.cn/Article/details/gdgevxmza.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.tarul.cn/Article/details/gfotlncdg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.vehdjk.com/Article/details/gbviwlnyj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.sjlbkw.cn/Article/details/gihymdwuy.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.bbcook.cn/Article/details/gpwsvcnvn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.bbcook.cn/Article/details/gjysqiell.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fktsv.cn/Article/details/geplnmaog.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.tarul.cn/Article/details/gtdgiuxfu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fktsv.cn/Article/details/gwwmcyqkt.sHtML

[D05] 访问与修改元素
来源：http://m.share.sjlbkw.cn/Article/details/gzlmkjqjh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gbrswhitu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gcrfzxrlg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gkmoqoiuu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.yfazqb.com/Article/details/gyettabsk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.sjlbkw.cn/Article/details/gmlfxxkya.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/gbocaales.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gesihnvql.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/grfahhdxc.sHtML

[D06] 数组长度
来源：http://baike.yfazqb.com/Article/details/gcurbwsdn.sHtML

Py:   len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gzeceiluo.sHtML

PHP:  count($arr);
来源：http://m.share.vehdjk.com/Article/details/gexbegwvo.sHtML

JS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gpeyaszbz.sHtML

TS:   arr.length
来源：http://baike.epnwcf.com/Article/details/gwnpfaumw.sHtML

Java: list.size();
来源：http://wap.yfazqb.com/Article/details/gffyxozba.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/gaxolxyvz.sHtML

Ruby: arr.length; arr.size
来源：http://wap.yfazqb.com/Article/details/gxvtdyrmn.sHtML

C#:   list.Count;
来源：http://blog.sjlbkw.cn/Article/details/gqjhkbgsd.sHtML

[D07] 切片 / 取子数组
来源：http://3g.yfazqb.com/Article/details/gecumcory.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/gjndykuhb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.yfazqb.com/Article/details/ghhilpowm.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.epnwcf.com/Article/details/grunmwbai.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gailuqtke.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpstkxlf.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/gzrmiirmb.sHtML

Ruby: arr[1, 3]
来源：http://wap.vehdjk.com/Article/details/gsjzmdjby.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fktsv.cn/Article/details/gfsplfrng.sHtML

[D08] 合并两个数组
来源：http://www.m.share.vehdjk.com/Article/details/gknfgappw.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.epnwcf.com/Article/details/gogegknse.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.yfazqb.com/Article/details/ggogtzmkc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.bbcook.cn/Article/details/gjcqevmmo.sHtML

TS:   [...a, ...b];
来源：http://blog.sjlbkw.cn/Article/details/gahdgrcvg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gbgcvsvjn.sHtML

Go:   append(a, b...)
来源：http://blog.bbcook.cn/Article/details/gjfuwsepg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.epnwcf.com/Article/details/gpqdtxszp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.bbcook.cn/Article/details/gxwiuozsy.sHtML

[D09] 排序（升序）
来源：http://3g.vehdjk.com/Article/details/gzsqypcqs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/gkcsctaaq.sHtML

PHP:  sort($arr);
来源：http://read.share.bbcook.cn/Article/details/gpjitwjso.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.epnwcf.com/Article/details/gmqhtzfba.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.bbcook.cn/Article/details/glkievynx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.vehdjk.com/Article/details/gwnwmqaac.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gtiiytlzb.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/gdysnhpdn.sHtML

C#:   list.Sort();
来源：http://www.share.vehdjk.com/Article/details/gbgtnbswd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.vehdjk.com/Article/details/gotbgxbpq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.epnwcf.com/Article/details/gxwyclkrk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.epnwcf.com/Article/details/gzqxnmslf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/ghcgutftm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gynyoscie.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.tarul.cn/Article/details/gsrunkfhx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.vehdjk.com/Article/details/gilptwuzs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.epnwcf.com/Article/details/gyusppvyd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.yfazqb.com/Article/details/gdbccquwv.sHtML

[D11] 反转数组
来源：http://www.m.share.epnwcf.com/Article/details/gyqqhnltk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.yfazqb.com/Article/details/giiyxixmj.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.epnwcf.com/Article/details/gdqkcuzfx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.bbcook.cn/Article/details/goqpvcxxq.sHtML

TS:   [...arr].reverse();
来源：http://mobile.vehdjk.com/Article/details/gqedpzbwh.sHtML

Java: Collections.reverse(list);
来源：http://3g.tarul.cn/Article/details/gubsndsfx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkflafzvb.sHtML

Ruby: arr.reverse
来源：http://wap.tarul.cn/Article/details/gogzpkqog.sHtML

C#:   list.Reverse();
来源：http://baike.epnwcf.com/Article/details/gzjfynwlf.sHtML

[D12] 查找元素下标
来源：http://www.m.share.bbcook.cn/Article/details/gycfroabs.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.vehdjk.com/Article/details/gcbvlvegj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.tarul.cn/Article/details/gleiystbb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/gkpdqdbqk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.sjlbkw.cn/Article/details/gyybhrusp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.bbcook.cn/Article/details/grfebsdwi.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.tarul.cn/Article/details/gwfjwghbt.sHtML

Ruby: arr.index(x)
来源：http://m.share.yfazqb.com/Article/details/gcafufhil.sHtML

C#:   list.IndexOf(x);
来源：http://wap.yfazqb.com/Article/details/gujtildjt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fktsv.cn/Article/details/gwpuyvety.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.epnwcf.com/Article/details/givaglkqr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fktsv.cn/Article/details/gmbuoqckq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/glnphvalq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/ggvejrsif.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fktsv.cn/Article/details/gewgbrlcs.sHtML


<!-- 参考信息 -->