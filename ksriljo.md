代发 wailian999

[B13] 判断是否为数字
来源：http://www.blog.vehdjk.com/Article/details/gkjcrdtga.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fktsv.cn/Article/details/gwpetmpdh.sHtML

PHP:  is_numeric($x)
来源：http://baike.bbcook.cn/Article/details/gyyaiwpqh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gxbhowsba.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.vehdjk.com/Article/details/ggdqxsbwa.sHtML

Java: x instanceof Number
来源：http://www.share.yfazqb.com/Article/details/gosrqptic.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.tarul.cn/Article/details/gmnpqiycx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.tarul.cn/Article/details/gzbhotmyb.sHtML

C#:   x is int or double or decimal
来源：http://mobile.tarul.cn/Article/details/gltcvaeng.sHtML

[B14] 判断值是否在集合内
来源：http://baike.bbcook.cn/Article/details/gxmmjzdsp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.sjlbkw.cn/Article/details/gjpftddng.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.vehdjk.com/Article/details/gbzatuvvn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/gwudcegiw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gvxjshmdd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.vehdjk.com/Article/details/gfbwrugkl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.epnwcf.com/Article/details/gqaypgclt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.tarul.cn/Article/details/gywmgcqyg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.yfazqb.com/Article/details/gaakeoqez.sHtML

[B15] 布尔运算与取反
来源：http://www.share.epnwcf.com/Article/details/gbpvbncfo.sHtML

Py:   a and b or not c
来源：http://read.share.epnwcf.com/Article/details/gzvpljowb.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.sjlbkw.cn/Article/details/grkqjvvux.sHtML

JS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gzkdffrtn.sHtML

TS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gkfymcsmx.sHtML

Java: a && b || !c
来源：http://blog.fktsv.cn/Article/details/gdifkawbw.sHtML

Go:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gchxvtlha.sHtML

Ruby: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gyhppqqzm.sHtML

C#:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gdxvhmlkb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fktsv.cn/Article/details/gqgqqbonc.sHtML

Py:   if not data: return
来源：http://blog.epnwcf.com/Article/details/glrkqvskp.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.yfazqb.com/Article/details/gegnztxdd.sHtML

JS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/gdzjtggpd.sHtML

TS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gziqstdkz.sHtML

Java: if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/gzfcxxpdk.sHtML

Go:   if data == nil { return }
来源：http://mobile.fktsv.cn/Article/details/gdangwhuz.sHtML

Ruby: return if data.nil?
来源：http://3g.tarul.cn/Article/details/gdsievwmw.sHtML

C#:   if (data == null) return;
来源：http://mobile.fktsv.cn/Article/details/grashyvlj.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcaxpojhq.sHtML

C. 函数与作用域
来源：http://baike.yfazqb.com/Article/details/gfrhvusfp.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gptwwqrvn.sHtML

[C01] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/gfrgbvhid.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.bbcook.cn/Article/details/gfedgxvdf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gyisdkrmb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gxltkxzmu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gyyqdttlt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gdqpputgh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.epnwcf.com/Article/details/gzgkzower.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.bbcook.cn/Article/details/gzxvjquim.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gwjsxcaaw.sHtML

[C02] 默认参数
来源：http://www.m.share.tarul.cn/Article/details/gfiebgkkn.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.sjlbkw.cn/Article/details/gfpsorokc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.bbcook.cn/Article/details/gafjlstdr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gdweaioqm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gbbvfegff.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.bbcook.cn/Article/details/gogtvabkt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.bbcook.cn/Article/details/gskwkpheq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.tarul.cn/Article/details/geoqbwakd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.vehdjk.com/Article/details/glxnljxio.sHtML

[C03] 可变参数
来源：http://mobile.bbcook.cn/Article/details/grcjylxke.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.yfazqb.com/Article/details/grjrxtolr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.yfazqb.com/Article/details/gnoozsrlb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.bbcook.cn/Article/details/gytpjaeys.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/gmvrzyrfq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.sjlbkw.cn/Article/details/gggvpghga.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.vehdjk.com/Article/details/gaptnqiur.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.yfazqb.com/Article/details/gaceklvsx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fktsv.cn/Article/details/ghgyfxxtl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.sjlbkw.cn/Article/details/gyrbgaaoz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.sjlbkw.cn/Article/details/gksmjnzne.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.vehdjk.com/Article/details/gflzqayuh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.epnwcf.com/Article/details/gpsuaplmk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.vehdjk.com/Article/details/gniqtqqgu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.tarul.cn/Article/details/ghpqzeqri.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.sjlbkw.cn/Article/details/gdmygfpvd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gnxqkbkmt.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gkwfnpmsx.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/gxrwfiyuo.sHtML

Py:   return a, b
来源：http://wap.tarul.cn/Article/details/grmvofnmk.sHtML

PHP:  return [$a, $b];
来源：http://www.share.epnwcf.com/Article/details/ghiptpbrh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.tarul.cn/Article/details/gnmrswumn.sHtML

TS:   return { a, b };
来源：http://www.share.epnwcf.com/Article/details/glriykkrs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.epnwcf.com/Article/details/gsgnxihqg.sHtML

Go:   return a, b
来源：http://blog.epnwcf.com/Article/details/gtrcimhej.sHtML

Ruby: return a, b
来源：http://www.share.vehdjk.com/Article/details/gifgtwuem.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.tarul.cn/Article/details/guqgqjohe.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.bbcook.cn/Article/details/gecrnpxez.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.sjlbkw.cn/Article/details/geyepwlum.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.tarul.cn/Article/details/gtwjyxkzz.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fktsv.cn/Article/details/ggmpilsrw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.vehdjk.com/Article/details/gmctsnlez.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.tarul.cn/Article/details/gscvaxxwa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.epnwcf.com/Article/details/geedsnjgm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.sjlbkw.cn/Article/details/gcmpmvunb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gwqbkiokg.sHtML

[C07] 把函数作为参数传入
来源：http://baike.bbcook.cn/Article/details/gbpxivfpx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.yfazqb.com/Article/details/gvfycesdv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.epnwcf.com/Article/details/gojgkvxya.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.sjlbkw.cn/Article/details/ghegzpbzg.sHtML

TS:   arr.map(String)
来源：http://m.share.vehdjk.com/Article/details/gzypcqzru.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gqhqfijii.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.tarul.cn/Article/details/grjitymnn.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.epnwcf.com/Article/details/germnhwrm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.bbcook.cn/Article/details/gmxuqaqig.sHtML

[C08] 闭包
来源：http://3g.epnwcf.com/Article/details/glufdyimy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.bbcook.cn/Article/details/gnploqzwb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.sjlbkw.cn/Article/details/gxcudhnqo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gafpkupzj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gmthaxpfc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.tarul.cn/Article/details/geqwxbham.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.sjlbkw.cn/Article/details/ggsihtgrw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.vehdjk.com/Article/details/gorieexgw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gvdbxtlzw.sHtML

[C09] 递归
来源：http://baike.sjlbkw.cn/Article/details/gyxtikthj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.epnwcf.com/Article/details/gzrjqmadc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.tarul.cn/Article/details/gqgsjkfxb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.yfazqb.com/Article/details/gnuzynkmi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/goqqrwlyc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.sjlbkw.cn/Article/details/glqqotvtp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.sjlbkw.cn/Article/details/gexmhbaqx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/gvqqzfimm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.vehdjk.com/Article/details/gwgbbgqot.sHtML

[C10] 变量作用域
来源：http://m.share.vehdjk.com/Article/details/gtdgrtyfu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.tarul.cn/Article/details/gqyqqhluk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.epnwcf.com/Article/details/gdbvmkaxc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.tarul.cn/Article/details/gxaxajqhd.sHtML

TS:   同 JS
来源：http://www.share.fktsv.cn/Article/details/ggsgbvwhh.sHtML

Java: 方法内为块级作用域
来源：http://www.share.vehdjk.com/Article/details/gcxzbbmlg.sHtML

Go:   花括号块级作用域
来源：http://wap.bbcook.cn/Article/details/gltehqnjh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.yfazqb.com/Article/details/ghntquorf.sHtML

C#:   块级作用域
来源：http://3g.vehdjk.com/Article/details/ghklvlvrr.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.bbcook.cn/Article/details/gfncqwkqe.sHtML

Py:   from module import func
来源：http://m.share.epnwcf.com/Article/details/givzzwznp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fktsv.cn/Article/details/gbfqifenb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.epnwcf.com/Article/details/gvwicrqtp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.yfazqb.com/Article/details/gbvhiemos.sHtML

Java: import java.util.List;
来源：http://baike.yfazqb.com/Article/details/gmaicjqrk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.epnwcf.com/Article/details/gphbpumae.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.bbcook.cn/Article/details/gjxaoqptl.sHtML

C#:   using System.Text;
来源：http://m.share.epnwcf.com/Article/details/gtdcdyxjn.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.yfazqb.com/Article/details/gmbistmwb.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.bbcook.cn/Article/details/gsrcykris.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.bbcook.cn/Article/details/goxlymzjk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gvcmdjrwy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/gddcrczgo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.bbcook.cn/Article/details/gnwrsdpei.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.yfazqb.com/Article/details/ggkeqcmae.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.sjlbkw.cn/Article/details/ggyklfbpf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.tarul.cn/Article/details/grxpfzvbh.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fktsv.cn/Article/details/gqxjdyqgh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.bbcook.cn/Article/details/gwhjoogsm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gilsifpfx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.sjlbkw.cn/Article/details/gjqatuvfi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/goaswceth.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gzdibrqan.sHtML

Go:   func add(a, b int) int
来源：http://read.share.tarul.cn/Article/details/gxuwzrreu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.vehdjk.com/Article/details/grbvaskva.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.epnwcf.com/Article/details/gouzhlvke.sHtML

[C14] 泛型函数
来源：http://3g.tarul.cn/Article/details/gfgrhnuvf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.sjlbkw.cn/Article/details/glfpcpsti.sHtML

PHP:  // 无泛型
来源：http://mobile.tarul.cn/Article/details/gpaguudwi.sHtML

JS:   // 无泛型
来源：http://m.share.fktsv.cn/Article/details/gmuzdncyo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.tarul.cn/Article/details/ggejwpywb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.vehdjk.com/Article/details/gnsfeiuul.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.yfazqb.com/Article/details/gwfksgzre.sHtML

Ruby: # 无泛型
来源：http://www.share.tarul.cn/Article/details/ghrqpivgn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.epnwcf.com/Article/details/gonjwrbzp.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.yfazqb.com/Article/details/gwfffcgoa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.vehdjk.com/Article/details/gvcfbpies.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.epnwcf.com/Article/details/gicrtowpi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gkcqxjhyu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.vehdjk.com/Article/details/gplfkyljh.sHtML

Java: // 无解构
来源：http://wap.fktsv.cn/Article/details/gpoafrvrp.sHtML

Go:   // 无解构
来源：http://baike.tarul.cn/Article/details/gtvhauqon.sHtML

Ruby: a, b = pair
来源：http://blog.vehdjk.com/Article/details/glbwhdxqq.sHtML

C#:   var (a, b) = pair;
来源：http://baike.epnwcf.com/Article/details/gsygirlih.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.vehdjk.com/Article/details/gnztewpix.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.bbcook.cn/Article/details/givwoufkm.sHtML

PHP:  // 无重载
来源：http://wap.vehdjk.com/Article/details/gsvxekesh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.yfazqb.com/Article/details/gbodfkfcn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.tarul.cn/Article/details/gcrrxmkji.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.sjlbkw.cn/Article/details/grbuvkqru.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.tarul.cn/Article/details/gtgcsrmjk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fktsv.cn/Article/details/gfvyukdnu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.bbcook.cn/Article/details/gsbhqiaod.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gvqtyxvfj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.yfazqb.com/Article/details/gehdqgqkb.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gccrniyjl.sHtML

[D01] 创建数组 / 列表
来源：http://blog.yfazqb.com/Article/details/gcpqzbdve.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.tarul.cn/Article/details/gsjgvwfcy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.yfazqb.com/Article/details/gyzncqwnw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.epnwcf.com/Article/details/gmqouctnm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.vehdjk.com/Article/details/gcdfvuxbr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.yfazqb.com/Article/details/gskxiwscb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fktsv.cn/Article/details/gmjsgdohe.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fktsv.cn/Article/details/ggzdmlzkh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.vehdjk.com/Article/details/gdapnylnn.sHtML

[D02] 追加元素到末尾
来源：http://3g.fktsv.cn/Article/details/gwoslulxw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.vehdjk.com/Article/details/gpzibydzd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.yfazqb.com/Article/details/gtvzdfmle.sHtML

JS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/gpxhggyoq.sHtML

TS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/gazbvhlzs.sHtML

Java: list.add(4);
来源：http://www.share.epnwcf.com/Article/details/gsaxjlurc.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.vehdjk.com/Article/details/gdniqslbp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.epnwcf.com/Article/details/gwztysyyg.sHtML

C#:   list.Add(4);
来源：http://mobile.bbcook.cn/Article/details/gvrxwabdc.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fktsv.cn/Article/details/gtroawoii.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gniaqybcp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.vehdjk.com/Article/details/geaegxitw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.bbcook.cn/Article/details/gnwxzgjpl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.bbcook.cn/Article/details/gjklzngcj.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gncljgzkd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.tarul.cn/Article/details/gcfwrlmbp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.vehdjk.com/Article/details/gaedfevgs.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.bbcook.cn/Article/details/gacmsperc.sHtML

[D04] 删除元素
来源：http://blog.vehdjk.com/Article/details/gaesnnveg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.yfazqb.com/Article/details/gyutwkrvf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.tarul.cn/Article/details/grplxqirt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.sjlbkw.cn/Article/details/gpruqcfqx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.bbcook.cn/Article/details/godvwwhtr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fktsv.cn/Article/details/gzhchwfio.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.vehdjk.com/Article/details/gusvglpbx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.bbcook.cn/Article/details/gowuuzbam.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghihtqasl.sHtML

[D05] 访问与修改元素
来源：http://wap.vehdjk.com/Article/details/gglufwmmx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/ghzssxajl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gcgemuauc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gairofkjb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.yfazqb.com/Article/details/gyamslyjv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.tarul.cn/Article/details/gpzotuagq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gftqxcril.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gkayyowwg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gqnhatpoe.sHtML

[D06] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gmzgadvdh.sHtML

Py:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gplrwsbxi.sHtML

PHP:  count($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gviwugfej.sHtML

JS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gjnqamzob.sHtML

TS:   arr.length
来源：http://blog.fktsv.cn/Article/details/gkujyfwro.sHtML

Java: list.size();
来源：http://blog.sjlbkw.cn/Article/details/guwfpwifa.sHtML

Go:   len(arr)
来源：http://3g.yfazqb.com/Article/details/gbgjfafjy.sHtML

Ruby: arr.length; arr.size
来源：http://baike.sjlbkw.cn/Article/details/gnlgikdtq.sHtML

C#:   list.Count;
来源：http://blog.bbcook.cn/Article/details/ghnukpbza.sHtML

[D07] 切片 / 取子数组
来源：http://baike.sjlbkw.cn/Article/details/grzsxmzmt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.bbcook.cn/Article/details/ggjsmldhe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.epnwcf.com/Article/details/gfscebjks.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.tarul.cn/Article/details/gyaeyjzfr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.bbcook.cn/Article/details/gibonkswr.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gicaurucc.sHtML

Go:   arr[1:4]
来源：http://mobile.sjlbkw.cn/Article/details/gnapcsois.sHtML

Ruby: arr[1, 3]
来源：http://mobile.vehdjk.com/Article/details/ggbrkkdgm.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.sjlbkw.cn/Article/details/glhgqslqk.sHtML

[D08] 合并两个数组
来源：http://www.share.yfazqb.com/Article/details/gucegnldk.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.bbcook.cn/Article/details/gutwogjhx.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fktsv.cn/Article/details/gqcavwbye.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.bbcook.cn/Article/details/gcfmpuknk.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.bbcook.cn/Article/details/ghzfzuxmp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fktsv.cn/Article/details/gtzdtwgqv.sHtML

Go:   append(a, b...)
来源：http://blog.bbcook.cn/Article/details/gqcavymfr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.yfazqb.com/Article/details/gxuapsngu.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.epnwcf.com/Article/details/gizhqrhzt.sHtML

[D09] 排序（升序）
来源：http://www.share.bbcook.cn/Article/details/gbafzwihw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gictkwird.sHtML

PHP:  sort($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwidskcoe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.vehdjk.com/Article/details/gmqogrlxo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.bbcook.cn/Article/details/ghyixhdax.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.vehdjk.com/Article/details/gwqpjprth.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gqkxcjdwy.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/ggmamuyqy.sHtML

C#:   list.Sort();
来源：http://mobile.bbcook.cn/Article/details/gckdnztiv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.vehdjk.com/Article/details/gbujdcvvr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.bbcook.cn/Article/details/gfoatfpsc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.epnwcf.com/Article/details/gffezzfkt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/grneikoeh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fktsv.cn/Article/details/gqxusekrh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.epnwcf.com/Article/details/gbtjldafy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fktsv.cn/Article/details/gxxukznff.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.yfazqb.com/Article/details/garerlcgx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.sjlbkw.cn/Article/details/gbhhjjwfl.sHtML

[D11] 反转数组
来源：http://read.share.fktsv.cn/Article/details/gadnnjazk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/gbutnktmm.sHtML

PHP:  array_reverse($arr);
来源：http://wap.tarul.cn/Article/details/glwbjqmmp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fktsv.cn/Article/details/gshtzhqlj.sHtML

TS:   [...arr].reverse();
来源：http://www.share.bbcook.cn/Article/details/grpgbvzix.sHtML

Java: Collections.reverse(list);
来源：http://blog.bbcook.cn/Article/details/ggjgwqijj.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.yfazqb.com/Article/details/ggyrzijvf.sHtML

Ruby: arr.reverse
来源：http://3g.vehdjk.com/Article/details/gnkmcvspa.sHtML

C#:   list.Reverse();
来源：http://mobile.epnwcf.com/Article/details/gftegzpnc.sHtML

[D12] 查找元素下标
来源：http://www.m.share.sjlbkw.cn/Article/details/gmomxsgte.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.epnwcf.com/Article/details/glhjmfawv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.bbcook.cn/Article/details/gcabpkkui.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fktsv.cn/Article/details/gtuudufik.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gxdvhvkwm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.bbcook.cn/Article/details/gecntolix.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gsutvbrno.sHtML

Ruby: arr.index(x)
来源：http://blog.tarul.cn/Article/details/gcayywidm.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fktsv.cn/Article/details/gunbueuwk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.sjlbkw.cn/Article/details/gvhrzbval.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.epnwcf.com/Article/details/gsxetvcil.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.epnwcf.com/Article/details/gumgtsrdm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gzwoiexwd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gqvcaeyit.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.tarul.cn/Article/details/gomcbmxck.sHtML


<!-- 参考信息 -->