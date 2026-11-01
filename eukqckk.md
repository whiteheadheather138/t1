代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gviewoedp.sHtML

Java: x instanceof Number
来源：http://blog.fktsv.cn/Article/details/gkiqmeawd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.tarul.cn/Article/details/gjcbenqze.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpqnhqhs.sHtML

C#:   x is int or double or decimal
来源：http://blog.epnwcf.com/Article/details/glexttoet.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.vehdjk.com/Article/details/gbjyoodnw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.epnwcf.com/Article/details/glwkmqupq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.sjlbkw.cn/Article/details/gyxyfmnhy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/gbfztlwve.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/gvusodbed.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.bbcook.cn/Article/details/gweudgdmz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.epnwcf.com/Article/details/ggapydshn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.epnwcf.com/Article/details/gconnggyh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gttygrqhb.sHtML

[B15] 布尔运算与取反
来源：http://m.share.yfazqb.com/Article/details/gvqihlosq.sHtML

Py:   a and b or not c
来源：http://read.share.fktsv.cn/Article/details/gaeeueiim.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.bbcook.cn/Article/details/gojzimbgc.sHtML

JS:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gbmeshxyo.sHtML

TS:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gtktkcohg.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gqpnbaltq.sHtML

Go:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gjubnfnwc.sHtML

Ruby: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/geoqvqfwy.sHtML

C#:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcaubher.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.bbcook.cn/Article/details/gfknfobub.sHtML

Py:   if not data: return
来源：http://blog.fktsv.cn/Article/details/guwmfknnj.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.epnwcf.com/Article/details/gfllrivaj.sHtML

JS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gcotzjsyt.sHtML

TS:   if (!data) return;
来源：http://www.share.sjlbkw.cn/Article/details/grhcuvdsd.sHtML

Java: if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/gwftciqnz.sHtML

Go:   if data == nil { return }
来源：http://3g.vehdjk.com/Article/details/gzwxagcje.sHtML

Ruby: return if data.nil?
来源：http://m.share.bbcook.cn/Article/details/gtztsvvuy.sHtML

C#:   if (data == null) return;
来源：http://mobile.epnwcf.com/Article/details/gunwegnmb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gxacjohep.sHtML

C. 函数与作用域
来源：http://www.m.share.fktsv.cn/Article/details/glzmwrevz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gdfcotgmy.sHtML

[C01] 定义函数
来源：http://blog.yfazqb.com/Article/details/gvfoydkdv.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.epnwcf.com/Article/details/gkrmmsamj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gjgqgbixz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gitypmwcu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gaynhxcnu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/ghncbjoad.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.bbcook.cn/Article/details/ghlejykwu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.tarul.cn/Article/details/ghtnldrdo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gmaewyxrr.sHtML

[C02] 默认参数
来源：http://blog.sjlbkw.cn/Article/details/gcfmjeqjd.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.epnwcf.com/Article/details/gbrukcsdv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.sjlbkw.cn/Article/details/gtasbxydm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/glnahuqtf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.tarul.cn/Article/details/gdpvhhcvn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjvysbgs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.bbcook.cn/Article/details/gqannlzif.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.epnwcf.com/Article/details/gowdlezqq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fktsv.cn/Article/details/gslrpygjr.sHtML

[C03] 可变参数
来源：http://www.blog.fktsv.cn/Article/details/gvxhkwvsm.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.vehdjk.com/Article/details/gqreepdli.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.tarul.cn/Article/details/gfknifdsh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/glyvhiwxi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/gxosagdud.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fktsv.cn/Article/details/gwdkgupof.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.tarul.cn/Article/details/goijfucij.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.vehdjk.com/Article/details/gqxtyagky.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.vehdjk.com/Article/details/gommsbxlm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.tarul.cn/Article/details/gmroqfyvo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwxepkkh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/ggangrhhq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.vehdjk.com/Article/details/gmhvaarpa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.bbcook.cn/Article/details/gnksyfsaj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.tarul.cn/Article/details/gacetldko.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.sjlbkw.cn/Article/details/gszmxmgzx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gzuwkkysf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gpwquzloa.sHtML

[C05] 返回多个值
来源：http://read.share.fktsv.cn/Article/details/gybakpbif.sHtML

Py:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gdjqnogod.sHtML

PHP:  return [$a, $b];
来源：http://blog.epnwcf.com/Article/details/gyaypbjbk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gzpcpcgsz.sHtML

TS:   return { a, b };
来源：http://read.share.vehdjk.com/Article/details/grqdhysif.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.bbcook.cn/Article/details/gqdbqxijk.sHtML

Go:   return a, b
来源：http://mobile.tarul.cn/Article/details/grkfwncyk.sHtML

Ruby: return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/ghofuejdv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fktsv.cn/Article/details/gfuqiakkn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fktsv.cn/Article/details/gdlfpzany.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.bbcook.cn/Article/details/gozvgiczr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.vehdjk.com/Article/details/gqhmigfvg.sHtML

JS:   const square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gomcebzyt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.bbcook.cn/Article/details/ghcdflbfd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.tarul.cn/Article/details/gdnpgrkhk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.bbcook.cn/Article/details/gcmcaxyba.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fktsv.cn/Article/details/geotlfyaf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/gcdpojvft.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.sjlbkw.cn/Article/details/guvhltdvg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.epnwcf.com/Article/details/godmftipt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.tarul.cn/Article/details/gobzvgovu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fktsv.cn/Article/details/gzwkdhooc.sHtML

TS:   arr.map(String)
来源：http://blog.epnwcf.com/Article/details/gsjuphfvm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.yfazqb.com/Article/details/ggfkdjrgk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.sjlbkw.cn/Article/details/gviidouvg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.epnwcf.com/Article/details/glkbnfzem.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/gscuhdyaw.sHtML

[C08] 闭包
来源：http://blog.yfazqb.com/Article/details/gbvrwvtes.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.bbcook.cn/Article/details/gqzaiqhbb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.bbcook.cn/Article/details/glakmmjrr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gjnujrjzp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gnospjfsk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.epnwcf.com/Article/details/gutjermbl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.tarul.cn/Article/details/gzjsrhhzk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.yfazqb.com/Article/details/ghwckxgxu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/ggwnwhxpk.sHtML

[C09] 递归
来源：http://blog.vehdjk.com/Article/details/gcsqppxsd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gwfxbrzaf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.tarul.cn/Article/details/gwzmbtjsl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/gqdsnjgih.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/gngmkrgbb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fktsv.cn/Article/details/gcobmpaey.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.epnwcf.com/Article/details/gogaiipaq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/glfhtrljm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fktsv.cn/Article/details/gozryakvp.sHtML

[C10] 变量作用域
来源：http://www.share.vehdjk.com/Article/details/gnbjcbqnx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.epnwcf.com/Article/details/gopwfeniu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.bbcook.cn/Article/details/guyzzrmqr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fktsv.cn/Article/details/gxlmdxwyl.sHtML

TS:   同 JS
来源：http://read.share.bbcook.cn/Article/details/ghlmpachz.sHtML

Java: 方法内为块级作用域
来源：http://baike.tarul.cn/Article/details/gncnwwcwq.sHtML

Go:   花括号块级作用域
来源：http://3g.tarul.cn/Article/details/gvfsispmw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.vehdjk.com/Article/details/gewxygqeb.sHtML

C#:   块级作用域
来源：http://www.blog.bbcook.cn/Article/details/glfrbhmdi.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.epnwcf.com/Article/details/gnmqgyjmv.sHtML

Py:   from module import func
来源：http://www.share.sjlbkw.cn/Article/details/ggccpjbvr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.yfazqb.com/Article/details/godsrhsjk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.bbcook.cn/Article/details/gpjosvrpe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fktsv.cn/Article/details/gvjohsjrc.sHtML

Java: import java.util.List;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbhnzrpz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.yfazqb.com/Article/details/gdzaaefyd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.yfazqb.com/Article/details/gnosjjfdr.sHtML

C#:   using System.Text;
来源：http://www.blog.epnwcf.com/Article/details/gfomzcuel.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.epnwcf.com/Article/details/gkqxhthcy.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.epnwcf.com/Article/details/gsancgxmn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.bbcook.cn/Article/details/gpyhzzcva.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.sjlbkw.cn/Article/details/giuuhtugp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.epnwcf.com/Article/details/gxczjjomb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.tarul.cn/Article/details/glkffvhgl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/ggklqxzhf.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.bbcook.cn/Article/details/gsclyxpxs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.tarul.cn/Article/details/gvapmywke.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.sjlbkw.cn/Article/details/ghjqfmypk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.tarul.cn/Article/details/gogofkqwm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/glwrkoape.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.vehdjk.com/Article/details/gtmidqpjo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gnvsqftmf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gmuhszlkd.sHtML

Go:   func add(a, b int) int
来源：http://3g.bbcook.cn/Article/details/gugypetdw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.epnwcf.com/Article/details/gtinoxnro.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fktsv.cn/Article/details/gtucymjec.sHtML

[C14] 泛型函数
来源：http://www.share.fktsv.cn/Article/details/glnlhjrgb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.vehdjk.com/Article/details/gayvbggrs.sHtML

PHP:  // 无泛型
来源：http://blog.fktsv.cn/Article/details/gvqkaadtg.sHtML

JS:   // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqilrmte.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.sjlbkw.cn/Article/details/ggjwyrrnq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.sjlbkw.cn/Article/details/gpqwrvpou.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.epnwcf.com/Article/details/goqicxecw.sHtML

Ruby: # 无泛型
来源：http://blog.bbcook.cn/Article/details/gozrckavf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.tarul.cn/Article/details/gncdrjtku.sHtML

[C15] 解构 / 展开参数
来源：http://wap.tarul.cn/Article/details/gtvubxeie.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.vehdjk.com/Article/details/glfrwkyml.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.tarul.cn/Article/details/glyglqjpm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gmwulbhio.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.yfazqb.com/Article/details/giuljsjeh.sHtML

Java: // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbvswuct.sHtML

Go:   // 无解构
来源：http://www.blog.epnwcf.com/Article/details/gtzrwtknn.sHtML

Ruby: a, b = pair
来源：http://mobile.tarul.cn/Article/details/gblrnezjv.sHtML

C#:   var (a, b) = pair;
来源：http://3g.bbcook.cn/Article/details/gclwknqfg.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.tarul.cn/Article/details/gptloorcs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fktsv.cn/Article/details/gfwzaxgmo.sHtML

PHP:  // 无重载
来源：http://baike.tarul.cn/Article/details/gbbzgario.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.bbcook.cn/Article/details/gourfzabf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.sjlbkw.cn/Article/details/gpbpphasi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.bbcook.cn/Article/details/grvxcycbc.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.bbcook.cn/Article/details/gvnzchfzl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fktsv.cn/Article/details/gevcvduqz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.tarul.cn/Article/details/gikszdgnz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbammvtkg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fktsv.cn/Article/details/garcgbsau.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxxhevlxp.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/gvlogmxei.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.epnwcf.com/Article/details/gnkfstfmv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.bbcook.cn/Article/details/gqdgivjbu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.yfazqb.com/Article/details/gefyryvbv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.bbcook.cn/Article/details/geuqanpci.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.epnwcf.com/Article/details/gavfixyht.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.vehdjk.com/Article/details/gzkysjboi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.bbcook.cn/Article/details/gjgjxjtnb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.tarul.cn/Article/details/givvckxsg.sHtML

[D02] 追加元素到末尾
来源：http://wap.bbcook.cn/Article/details/gddsbbqzr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.yfazqb.com/Article/details/gcjxkoomn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.yfazqb.com/Article/details/gyfhdenrw.sHtML

JS:   arr.push(4);
来源：http://read.share.yfazqb.com/Article/details/gdtnwcdjo.sHtML

TS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/gsuxpqfoi.sHtML

Java: list.add(4);
来源：http://wap.vehdjk.com/Article/details/gwpbulhdb.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.vehdjk.com/Article/details/gokyptyqf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.vehdjk.com/Article/details/gdubzcguh.sHtML

C#:   list.Add(4);
来源：http://blog.fktsv.cn/Article/details/gldxseqfi.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.epnwcf.com/Article/details/giayqqbbt.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.tarul.cn/Article/details/gzjwudsnx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.bbcook.cn/Article/details/grjxosuao.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.yfazqb.com/Article/details/gffwgskjr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.vehdjk.com/Article/details/gernfqhbq.sHtML

Java: list.add(0, 0);
来源：http://blog.epnwcf.com/Article/details/gyajbtpkw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.tarul.cn/Article/details/gyovsmkqx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.tarul.cn/Article/details/gkbydqsgn.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/grpzibvlz.sHtML

[D04] 删除元素
来源：http://wap.vehdjk.com/Article/details/gbkngqhcj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.vehdjk.com/Article/details/godvinkdq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fktsv.cn/Article/details/gwmclavaz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.bbcook.cn/Article/details/ggebaplap.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.epnwcf.com/Article/details/gioxsllka.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.epnwcf.com/Article/details/gvsckjcyz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fktsv.cn/Article/details/grucypjlk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.yfazqb.com/Article/details/gcpafcwyh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.yfazqb.com/Article/details/gvdbdjqhq.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgzmkiaf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/gbwjdlxed.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gbaeljrpa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/glgxznled.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.tarul.cn/Article/details/gxfpaypdn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.vehdjk.com/Article/details/gnqfsvxlf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/grdhmdqce.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/ghhfagnix.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/gqhziwpve.sHtML

[D06] 数组长度
来源：http://www.share.tarul.cn/Article/details/gjebybocd.sHtML

Py:   len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gsrnvveut.sHtML

PHP:  count($arr);
来源：http://www.blog.tarul.cn/Article/details/gnqmaohca.sHtML

JS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gvdpxwrei.sHtML

TS:   arr.length
来源：http://www.blog.epnwcf.com/Article/details/gdygcbmon.sHtML

Java: list.size();
来源：http://m.share.tarul.cn/Article/details/gjczaphnz.sHtML

Go:   len(arr)
来源：http://wap.tarul.cn/Article/details/gaptuivaq.sHtML

Ruby: arr.length; arr.size
来源：http://wap.sjlbkw.cn/Article/details/gfgvbfwjf.sHtML

C#:   list.Count;
来源：http://3g.fktsv.cn/Article/details/gbvwyrmeo.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.yfazqb.com/Article/details/glggqxgoe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.epnwcf.com/Article/details/gbyhmuhuw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.yfazqb.com/Article/details/grmigfeou.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fktsv.cn/Article/details/gxtfeudbu.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/glvrpiycu.sHtML

Java: list.subList(1, 4);
来源：http://blog.bbcook.cn/Article/details/ghtavblru.sHtML

Go:   arr[1:4]
来源：http://www.m.share.sjlbkw.cn/Article/details/guhvvtary.sHtML

Ruby: arr[1, 3]
来源：http://baike.fktsv.cn/Article/details/gcjaszefm.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.bbcook.cn/Article/details/gosclzugc.sHtML

[D08] 合并两个数组
来源：http://read.share.tarul.cn/Article/details/gkktnmucd.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.yfazqb.com/Article/details/gikunwcqk.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.sjlbkw.cn/Article/details/giirtawyu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.epnwcf.com/Article/details/gseptkvok.sHtML

TS:   [...a, ...b];
来源：http://baike.yfazqb.com/Article/details/gcayktsye.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.yfazqb.com/Article/details/gfoeverpm.sHtML

Go:   append(a, b...)
来源：http://3g.sjlbkw.cn/Article/details/givsibzmh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fktsv.cn/Article/details/ggggslike.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gvbrzudwz.sHtML

[D09] 排序（升序）
来源：http://www.m.share.bbcook.cn/Article/details/gpbxvypvh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gckkedyuj.sHtML

PHP:  sort($arr);
来源：http://wap.fktsv.cn/Article/details/glsqfvvth.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.sjlbkw.cn/Article/details/gdmgtgfbp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fktsv.cn/Article/details/gihammfai.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.bbcook.cn/Article/details/geeehsbbk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gkljeedqd.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/gggsifzog.sHtML

C#:   list.Sort();
来源：http://read.share.sjlbkw.cn/Article/details/gyaxhnfvo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fktsv.cn/Article/details/gafsgrkbl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.bbcook.cn/Article/details/grcieaspd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.yfazqb.com/Article/details/gphxuvdqg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxuzytvv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gnoqcuyfh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.yfazqb.com/Article/details/goattgepp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fktsv.cn/Article/details/gqjpgexgl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.bbcook.cn/Article/details/giwaobmvc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.bbcook.cn/Article/details/gwbegwzqx.sHtML

[D11] 反转数组
来源：http://mobile.epnwcf.com/Article/details/gkvcyerdq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fktsv.cn/Article/details/gzkzywzxf.sHtML

PHP:  array_reverse($arr);
来源：http://3g.epnwcf.com/Article/details/gettupeec.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.sjlbkw.cn/Article/details/gcorwugiu.sHtML

TS:   [...arr].reverse();
来源：http://blog.vehdjk.com/Article/details/grcvoilrg.sHtML

Java: Collections.reverse(list);
来源：http://3g.vehdjk.com/Article/details/ghjgvkzmy.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.tarul.cn/Article/details/gwsufwwdk.sHtML

Ruby: arr.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/goquvqlwa.sHtML

C#:   list.Reverse();
来源：http://baike.fktsv.cn/Article/details/giouniczt.sHtML

[D12] 查找元素下标
来源：http://baike.bbcook.cn/Article/details/gdiacamfu.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fktsv.cn/Article/details/gtptuparq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/glrcouoqt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/gvdhhfulb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/gyctumoja.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.tarul.cn/Article/details/gqszfjkbi.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/garowkfrq.sHtML

Ruby: arr.index(x)
来源：http://www.blog.tarul.cn/Article/details/gipkozexn.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.bbcook.cn/Article/details/gbjlckyok.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.sjlbkw.cn/Article/details/gzwnajmwh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.epnwcf.com/Article/details/gulgqligc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.yfazqb.com/Article/details/gepsvmreo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/gojevmexi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gcupcpohw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.epnwcf.com/Article/details/gwervrorp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fktsv.cn/Article/details/gumrabmkb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.epnwcf.com/Article/details/gqfxwzque.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.tarul.cn/Article/details/gnoirxllk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.yfazqb.com/Article/details/gfvvifqho.sHtML


<!-- 参考信息 -->