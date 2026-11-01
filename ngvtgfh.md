代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.yfazqb.com/Article/details/gswgmosuu.sHtML

Java: x instanceof Number
来源：http://mobile.yfazqb.com/Article/details/gfzfaufic.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.yfazqb.com/Article/details/glqtouwen.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.tarul.cn/Article/details/gabqffalf.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fktsv.cn/Article/details/gkqbullxl.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.tarul.cn/Article/details/gmegpasrs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.sjlbkw.cn/Article/details/gxyokbyhk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.bbcook.cn/Article/details/gdvysmtih.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/goobphjkt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gdvenmmor.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.vehdjk.com/Article/details/gydsofskd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.bbcook.cn/Article/details/gymquaqhf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.vehdjk.com/Article/details/gzucdingx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.yfazqb.com/Article/details/gxnslmfoo.sHtML

[B15] 布尔运算与取反
来源：http://baike.fktsv.cn/Article/details/gowjtqqsn.sHtML

Py:   a and b or not c
来源：http://wap.sjlbkw.cn/Article/details/gdzbsiyds.sHtML

PHP:  $a && $b || !$c
来源：http://3g.epnwcf.com/Article/details/gwltheysb.sHtML

JS:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gupuuenyx.sHtML

TS:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gvymudtrk.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gusgjsres.sHtML

Go:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/ggavtymwd.sHtML

Ruby: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gzwpkiayq.sHtML

C#:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gjsckpwlf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fktsv.cn/Article/details/gfmmxedoy.sHtML

Py:   if not data: return
来源：http://www.m.share.epnwcf.com/Article/details/gbkolgkje.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grsgzzrdi.sHtML

JS:   if (!data) return;
来源：http://wap.epnwcf.com/Article/details/ggbhqortj.sHtML

TS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gstahkxby.sHtML

Java: if (data == null) return;
来源：http://blog.tarul.cn/Article/details/gnbfavqvx.sHtML

Go:   if data == nil { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gcyswgwob.sHtML

Ruby: return if data.nil?
来源：http://www.share.tarul.cn/Article/details/gjlqikuee.sHtML

C#:   if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/gjiaalpuv.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnweorscy.sHtML

C. 函数与作用域
来源：http://mobile.tarul.cn/Article/details/ggakfppiy.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gqivopnjb.sHtML

[C01] 定义函数
来源：http://m.share.yfazqb.com/Article/details/gtpdkqedn.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fktsv.cn/Article/details/gdwbthvqf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gvubvoscg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gjvrwmavb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gseuikdrk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/grnloyvyh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.yfazqb.com/Article/details/guojjsgdc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.vehdjk.com/Article/details/ghqosbdoc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gbvxutcql.sHtML

[C02] 默认参数
来源：http://blog.sjlbkw.cn/Article/details/gzowhgjrd.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.tarul.cn/Article/details/gozsjhnjc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/goostajar.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/gxhethddm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/gnkkrpahr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.sjlbkw.cn/Article/details/gyvsrqldw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.vehdjk.com/Article/details/grljdpovy.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.sjlbkw.cn/Article/details/gavipkuwz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.epnwcf.com/Article/details/glcgunvrw.sHtML

[C03] 可变参数
来源：http://www.blog.vehdjk.com/Article/details/grqxiabmq.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.tarul.cn/Article/details/gxxyaimas.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.tarul.cn/Article/details/guokacefa.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.tarul.cn/Article/details/gfvpekwjd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/gnlnyssdr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.tarul.cn/Article/details/goupcbfqw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.epnwcf.com/Article/details/gknipzhhz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.epnwcf.com/Article/details/gfbwytbus.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.sjlbkw.cn/Article/details/gpidtbpzp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fktsv.cn/Article/details/gnmmpyieg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.tarul.cn/Article/details/gvsqytijn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gbkpxzslf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.vehdjk.com/Article/details/giaqluxhl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.yfazqb.com/Article/details/gilbpktqk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.yfazqb.com/Article/details/gruevdyto.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fktsv.cn/Article/details/gqhszvozj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gjeevrkcw.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gllkgnhrg.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/gkckosvhh.sHtML

Py:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gbunazhcx.sHtML

PHP:  return [$a, $b];
来源：http://baike.fktsv.cn/Article/details/glezvlyvw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.vehdjk.com/Article/details/gadhopfmh.sHtML

TS:   return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gimwatqei.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.bbcook.cn/Article/details/gpwfhnppc.sHtML

Go:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlbmusgt.sHtML

Ruby: return a, b
来源：http://www.blog.yfazqb.com/Article/details/ggdfiobrp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.epnwcf.com/Article/details/guuozbioa.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.sjlbkw.cn/Article/details/gubicmpan.sHtML

Py:   square = lambda x: x * x
来源：http://wap.bbcook.cn/Article/details/gnxcrybms.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.yfazqb.com/Article/details/gjeyqfvpw.sHtML

JS:   const square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gsosjffjd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.epnwcf.com/Article/details/gflntudfw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.tarul.cn/Article/details/gdpplszqk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fktsv.cn/Article/details/gvdgidzoe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.epnwcf.com/Article/details/guavnnyra.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/geglxrbvn.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.sjlbkw.cn/Article/details/gftzsucsv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.yfazqb.com/Article/details/gddhwvbgo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.sjlbkw.cn/Article/details/gtoezapzc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.epnwcf.com/Article/details/gcyefaoep.sHtML

TS:   arr.map(String)
来源：http://baike.sjlbkw.cn/Article/details/guaonjplm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fktsv.cn/Article/details/gmbrairph.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.tarul.cn/Article/details/gvxficrpn.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.vehdjk.com/Article/details/gdmmjqidd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.sjlbkw.cn/Article/details/gcawhenle.sHtML

[C08] 闭包
来源：http://www.share.epnwcf.com/Article/details/gkbrxcczh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.yfazqb.com/Article/details/gfacjnzud.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.vehdjk.com/Article/details/gxhyijrwz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gbrpfbzzn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gkmgqhgdw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.tarul.cn/Article/details/girbichfn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.epnwcf.com/Article/details/gozofxaio.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.epnwcf.com/Article/details/gslbcxzbm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gotmshvbe.sHtML

[C09] 递归
来源：http://www.share.fktsv.cn/Article/details/girdeqmxj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/gudbionxv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/gfplywlnt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gjoueybld.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gdywhqvlm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.bbcook.cn/Article/details/gkydqkmaj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.yfazqb.com/Article/details/gztkxqoua.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.vehdjk.com/Article/details/ggochyqpx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fktsv.cn/Article/details/gcmjerzcw.sHtML

[C10] 变量作用域
来源：http://blog.fktsv.cn/Article/details/gumtomqkn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.epnwcf.com/Article/details/gdmtsiifv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.vehdjk.com/Article/details/gdrtucona.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.yfazqb.com/Article/details/gwfxwxqqw.sHtML

TS:   同 JS
来源：http://m.share.vehdjk.com/Article/details/gkyusqlhs.sHtML

Java: 方法内为块级作用域
来源：http://baike.tarul.cn/Article/details/gcxhzkepi.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gpxmmfisy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.yfazqb.com/Article/details/gpfexpuxj.sHtML

C#:   块级作用域
来源：http://www.share.tarul.cn/Article/details/gvavoplxi.sHtML

[C11] 模块导入与导出
来源：http://www.blog.yfazqb.com/Article/details/gdrcoemuq.sHtML

Py:   from module import func
来源：http://m.share.fktsv.cn/Article/details/gpfvbqcqr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.sjlbkw.cn/Article/details/gcpxubmjr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fktsv.cn/Article/details/gbqldoyup.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.sjlbkw.cn/Article/details/gpejworla.sHtML

Java: import java.util.List;
来源：http://3g.vehdjk.com/Article/details/grmwrzzeg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.epnwcf.com/Article/details/gpsyzlpig.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.tarul.cn/Article/details/gqqapftua.sHtML

C#:   using System.Text;
来源：http://read.share.sjlbkw.cn/Article/details/gsvgdktyb.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fktsv.cn/Article/details/gslkjstdf.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fktsv.cn/Article/details/gyoiamwrj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fktsv.cn/Article/details/gjilcyqeb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fktsv.cn/Article/details/gazaxtske.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/gbxnwocbl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.bbcook.cn/Article/details/gmbptuyml.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.epnwcf.com/Article/details/gjocleawd.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.yfazqb.com/Article/details/gnxkgvqej.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.vehdjk.com/Article/details/gkybvlttf.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.sjlbkw.cn/Article/details/gvyvwnpzh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.vehdjk.com/Article/details/gthgqbifl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gzqljfnnl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.tarul.cn/Article/details/gojkessav.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gxydxstuz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/geemgwvin.sHtML

Go:   func add(a, b int) int
来源：http://baike.tarul.cn/Article/details/gadbnoewp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.bbcook.cn/Article/details/grtmntuuv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.bbcook.cn/Article/details/gvkyzeqpb.sHtML

[C14] 泛型函数
来源：http://www.m.share.tarul.cn/Article/details/gectcrnqj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.bbcook.cn/Article/details/grhekswvj.sHtML

PHP:  // 无泛型
来源：http://baike.fktsv.cn/Article/details/gjyfgvcql.sHtML

JS:   // 无泛型
来源：http://blog.vehdjk.com/Article/details/gcslsmwma.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.sjlbkw.cn/Article/details/gweiwwhhi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.sjlbkw.cn/Article/details/gkdscicsx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.epnwcf.com/Article/details/ggqjtnxqr.sHtML

Ruby: # 无泛型
来源：http://mobile.yfazqb.com/Article/details/ggjegomvk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.sjlbkw.cn/Article/details/guhkfnnfa.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.bbcook.cn/Article/details/gkkafuttd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.sjlbkw.cn/Article/details/glhomktbu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.tarul.cn/Article/details/gglwoqlvk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.vehdjk.com/Article/details/gddegzhoc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.bbcook.cn/Article/details/ggjoeobry.sHtML

Java: // 无解构
来源：http://wap.yfazqb.com/Article/details/ghlvqyxpj.sHtML

Go:   // 无解构
来源：http://3g.bbcook.cn/Article/details/giqxxbsur.sHtML

Ruby: a, b = pair
来源：http://www.m.share.epnwcf.com/Article/details/grlhsozcg.sHtML

C#:   var (a, b) = pair;
来源：http://blog.sjlbkw.cn/Article/details/gizujgbcr.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.tarul.cn/Article/details/gakdsjgoe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.epnwcf.com/Article/details/gzubkrrfw.sHtML

PHP:  // 无重载
来源：http://3g.bbcook.cn/Article/details/gqmczbnlv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.epnwcf.com/Article/details/gydtuovrt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.epnwcf.com/Article/details/gblhzzqfp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.bbcook.cn/Article/details/ghlzoopbn.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.tarul.cn/Article/details/gpggnwust.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.vehdjk.com/Article/details/gsbhspxfl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.bbcook.cn/Article/details/gbdttkxue.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gxlssdqhk.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.tarul.cn/Article/details/gsuiwcypu.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/guoykvnjo.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.tarul.cn/Article/details/ghebcaxjm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fktsv.cn/Article/details/gjcxkrxmg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.epnwcf.com/Article/details/gvyzkqzch.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gossckedr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.tarul.cn/Article/details/gitjilmvf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.sjlbkw.cn/Article/details/gpzisxioi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.yfazqb.com/Article/details/gfcmczhou.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.tarul.cn/Article/details/glccwqdkk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.bbcook.cn/Article/details/gvldvxzwl.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.vehdjk.com/Article/details/gsmkwsiej.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.vehdjk.com/Article/details/gzvnglrcr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.vehdjk.com/Article/details/gzogoskpe.sHtML

JS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/gxdsvdsqn.sHtML

TS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/gcyuercvb.sHtML

Java: list.add(4);
来源：http://blog.bbcook.cn/Article/details/ggeiogoqk.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.epnwcf.com/Article/details/gmckjdqrm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.bbcook.cn/Article/details/ghpgwwvex.sHtML

C#:   list.Add(4);
来源：http://mobile.sjlbkw.cn/Article/details/gxwmbfxzv.sHtML

[D03] 在指定位置插入元素
来源：http://wap.vehdjk.com/Article/details/gmahqtkzq.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/gtnbkzlyd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.tarul.cn/Article/details/gfgabnnrp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fktsv.cn/Article/details/gwvrbuptr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fktsv.cn/Article/details/gegxilmqj.sHtML

Java: list.add(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gmwgifyva.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.vehdjk.com/Article/details/gxxhlirdm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.tarul.cn/Article/details/ghwwpcbib.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.epnwcf.com/Article/details/gcydykqpv.sHtML

[D04] 删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gpqnaunuj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.sjlbkw.cn/Article/details/gkfdbbcak.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.vehdjk.com/Article/details/gmscxytwy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.sjlbkw.cn/Article/details/gldwervni.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fktsv.cn/Article/details/gjpzcxqpi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.sjlbkw.cn/Article/details/goqvwvrxe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.vehdjk.com/Article/details/gsvkjjnuc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.tarul.cn/Article/details/gdfnvtrqi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fktsv.cn/Article/details/gopmyxbpi.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.epnwcf.com/Article/details/ghuffnbnf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gwazvwpzi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/glpulsajk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gsblcgljk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.vehdjk.com/Article/details/gnbctqwuh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.sjlbkw.cn/Article/details/gauirgaya.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gqtmypshd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gzhqtrkru.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.tarul.cn/Article/details/goyinwfjd.sHtML

[D06] 数组长度
来源：http://3g.bbcook.cn/Article/details/gallnrnse.sHtML

Py:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gailkznjg.sHtML

PHP:  count($arr);
来源：http://wap.bbcook.cn/Article/details/gcybifxah.sHtML

JS:   arr.length
来源：http://blog.yfazqb.com/Article/details/gdxuinrbf.sHtML

TS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/ggabdbmum.sHtML

Java: list.size();
来源：http://www.share.vehdjk.com/Article/details/gpnzvzqns.sHtML

Go:   len(arr)
来源：http://read.share.vehdjk.com/Article/details/gwyjvazci.sHtML

Ruby: arr.length; arr.size
来源：http://3g.epnwcf.com/Article/details/gwfxxpduu.sHtML

C#:   list.Count;
来源：http://m.share.tarul.cn/Article/details/gdvpmiwkw.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.yfazqb.com/Article/details/ggzhebsvf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.vehdjk.com/Article/details/gbqspxulw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gsbwrepey.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gyvzjsebt.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gqalrmasz.sHtML

Java: list.subList(1, 4);
来源：http://3g.vehdjk.com/Article/details/gwzqrtlec.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/gczvuztkl.sHtML

Ruby: arr[1, 3]
来源：http://read.share.epnwcf.com/Article/details/gfuioqrsw.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fktsv.cn/Article/details/gnvsfjdqy.sHtML

[D08] 合并两个数组
来源：http://www.share.bbcook.cn/Article/details/gykavhdih.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.epnwcf.com/Article/details/gzaytzpvp.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fktsv.cn/Article/details/gdqcycsyn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.epnwcf.com/Article/details/grjtnkiaq.sHtML

TS:   [...a, ...b];
来源：http://m.share.vehdjk.com/Article/details/gjnbmnmvk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.bbcook.cn/Article/details/gxvundvds.sHtML

Go:   append(a, b...)
来源：http://m.share.sjlbkw.cn/Article/details/grcilrslf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.vehdjk.com/Article/details/gpzmdulle.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.vehdjk.com/Article/details/gtwdexnbt.sHtML

[D09] 排序（升序）
来源：http://wap.epnwcf.com/Article/details/gcvdfjfyq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/ggmrwblhp.sHtML

PHP:  sort($arr);
来源：http://www.blog.epnwcf.com/Article/details/gyqhwmxps.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.epnwcf.com/Article/details/gekbckfvc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcouwwqgy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.yfazqb.com/Article/details/goewtokgq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gkielgsta.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/ghmnaaece.sHtML

C#:   list.Sort();
来源：http://www.share.epnwcf.com/Article/details/gqnvvlgpe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.bbcook.cn/Article/details/giqslvmsl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fktsv.cn/Article/details/gggagmiex.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.sjlbkw.cn/Article/details/gulxiwwub.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/goywgcmdp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/gfhovviom.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.tarul.cn/Article/details/gdrpjufmz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.epnwcf.com/Article/details/gbuazdnuk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fktsv.cn/Article/details/gvmpdtyvy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.vehdjk.com/Article/details/gowyesgtj.sHtML

[D11] 反转数组
来源：http://m.share.fktsv.cn/Article/details/gikwzdgqs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.yfazqb.com/Article/details/gymtltadm.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gbxacfbcl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.vehdjk.com/Article/details/ggltsxnvy.sHtML

TS:   [...arr].reverse();
来源：http://wap.epnwcf.com/Article/details/gbdoltyhf.sHtML

Java: Collections.reverse(list);
来源：http://mobile.vehdjk.com/Article/details/ggyxwjokr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/gsljcrejh.sHtML

Ruby: arr.reverse
来源：http://3g.epnwcf.com/Article/details/gziqflfob.sHtML

C#:   list.Reverse();
来源：http://baike.bbcook.cn/Article/details/guisyyfds.sHtML

[D12] 查找元素下标
来源：http://www.share.fktsv.cn/Article/details/glzvlypxq.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.bbcook.cn/Article/details/gksmkjihm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.bbcook.cn/Article/details/gvnrgmyvz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/gejzjceop.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.tarul.cn/Article/details/guskjdoat.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.tarul.cn/Article/details/gdkkglyhl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gdchylijz.sHtML

Ruby: arr.index(x)
来源：http://baike.fktsv.cn/Article/details/gbpmvpwxo.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fktsv.cn/Article/details/gboclxbfw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.yfazqb.com/Article/details/ghndnjrpt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.epnwcf.com/Article/details/gulnbmfzd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fktsv.cn/Article/details/ghtfajijn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.yfazqb.com/Article/details/gcijshxfu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gstgcdicm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gjvupespu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.epnwcf.com/Article/details/gyinzrowv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.yfazqb.com/Article/details/gbvjneuli.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.vehdjk.com/Article/details/gowcuulqa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.epnwcf.com/Article/details/gbwwtyefc.sHtML


<!-- 参考信息 -->