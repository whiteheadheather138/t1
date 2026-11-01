代发 wailian999

[B13] 判断是否为数字
来源：http://mobile.bbcook.cn/Article/details/gefaodmcv.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.tarul.cn/Article/details/gzxglgesj.sHtML

PHP:  is_numeric($x)
来源：http://baike.tarul.cn/Article/details/gnynoqzky.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/gioiizqdg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gjuzesjyw.sHtML

Java: x instanceof Number
来源：http://3g.fktsv.cn/Article/details/gfjmfjjev.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.yfazqb.com/Article/details/gqlapaxii.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.bbcook.cn/Article/details/gluwpqpus.sHtML

C#:   x is int or double or decimal
来源：http://baike.fktsv.cn/Article/details/gboszlbki.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.vehdjk.com/Article/details/glijgpquj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.yfazqb.com/Article/details/gjapxwnyo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.vehdjk.com/Article/details/gpcsxwuhh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/gepmhvwkl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/grikvffox.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.epnwcf.com/Article/details/gcxztuhjj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.tarul.cn/Article/details/gtqhywgxf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.vehdjk.com/Article/details/gwdcsltyz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gfkzkbkfk.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.yfazqb.com/Article/details/gpfevpimh.sHtML

Py:   a and b or not c
来源：http://www.m.share.epnwcf.com/Article/details/gmynolrzl.sHtML

PHP:  $a && $b || !$c
来源：http://wap.epnwcf.com/Article/details/gskyokanq.sHtML

JS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/giyyklviv.sHtML

TS:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gzvyyknrt.sHtML

Java: a && b || !c
来源：http://blog.tarul.cn/Article/details/goitpbcbr.sHtML

Go:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gvlvpecbn.sHtML

Ruby: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gvqserqhr.sHtML

C#:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gprjivjck.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fktsv.cn/Article/details/gdfdpdtlq.sHtML

Py:   if not data: return
来源：http://www.share.fktsv.cn/Article/details/gbppkxthe.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.epnwcf.com/Article/details/gpfkawywb.sHtML

JS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gslxlfpjw.sHtML

TS:   if (!data) return;
来源：http://wap.sjlbkw.cn/Article/details/gvtqmtybg.sHtML

Java: if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/gefqsbrth.sHtML

Go:   if data == nil { return }
来源：http://www.share.fktsv.cn/Article/details/grcfegcvp.sHtML

Ruby: return if data.nil?
来源：http://wap.bbcook.cn/Article/details/gxbgenodg.sHtML

C#:   if (data == null) return;
来源：http://www.blog.vehdjk.com/Article/details/gzbwjwzoq.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfnfixhkt.sHtML

C. 函数与作用域
来源：http://read.share.sjlbkw.cn/Article/details/goijbsmwt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqdbrbypb.sHtML

[C01] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/gfpmtqfgo.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gjjsqtexx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/ghhxfdcnw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gtbtyeqlf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gsowohzjn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/goculnumt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.yfazqb.com/Article/details/ggojxcljq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.sjlbkw.cn/Article/details/gbdlaarls.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gxpclstfr.sHtML

[C02] 默认参数
来源：http://read.share.bbcook.cn/Article/details/gazxkobtz.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fktsv.cn/Article/details/gqtuektiz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fktsv.cn/Article/details/gjsgnqwqc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fktsv.cn/Article/details/gvynahsom.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gfybyhgjq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.bbcook.cn/Article/details/gmvkhduzr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.sjlbkw.cn/Article/details/ggwzenpou.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.epnwcf.com/Article/details/ghpaijwfd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.epnwcf.com/Article/details/gidutkjsu.sHtML

[C03] 可变参数
来源：http://www.m.share.bbcook.cn/Article/details/gqhsqaibi.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.yfazqb.com/Article/details/gqcbiqllp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.bbcook.cn/Article/details/gewbdzrfi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxblatxli.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/gzxplotws.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.tarul.cn/Article/details/gaegcnabm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.bbcook.cn/Article/details/gccfxnamt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.vehdjk.com/Article/details/geqhztvfa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.vehdjk.com/Article/details/gtakaodck.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.tarul.cn/Article/details/gpysfgrnn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.tarul.cn/Article/details/ghpfonyip.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.bbcook.cn/Article/details/gttgjjpuk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/gyjawgcng.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fktsv.cn/Article/details/gxpzqufxi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.vehdjk.com/Article/details/gcwyaccuf.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.yfazqb.com/Article/details/gkcfqsrlq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gfwdpqlqe.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/gqmiclwap.sHtML

[C05] 返回多个值
来源：http://wap.tarul.cn/Article/details/gorzgylka.sHtML

Py:   return a, b
来源：http://blog.epnwcf.com/Article/details/grqtoajaa.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fktsv.cn/Article/details/gswtlakpz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.epnwcf.com/Article/details/gyolytjmm.sHtML

TS:   return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gdgbrkscs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.vehdjk.com/Article/details/grfdcotgo.sHtML

Go:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/gtslntubt.sHtML

Ruby: return a, b
来源：http://baike.epnwcf.com/Article/details/gorkxuekq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlteknte.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.epnwcf.com/Article/details/gzuhmjsfq.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fktsv.cn/Article/details/gtngulffq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.sjlbkw.cn/Article/details/ghskwwwnq.sHtML

JS:   const square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gajihxmao.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.tarul.cn/Article/details/gbfvuxbwr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fktsv.cn/Article/details/gnltzkmtu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fktsv.cn/Article/details/gtqsbewtk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.sjlbkw.cn/Article/details/glgrfchkr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gnexcxffk.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.epnwcf.com/Article/details/gtqsichme.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.yfazqb.com/Article/details/gonrfymmv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.tarul.cn/Article/details/gnalcirdo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.vehdjk.com/Article/details/gjnpdtgwc.sHtML

TS:   arr.map(String)
来源：http://www.blog.epnwcf.com/Article/details/gjxboresb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.vehdjk.com/Article/details/ggftajqyg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fktsv.cn/Article/details/gojrgwrlx.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fktsv.cn/Article/details/gvwplwotr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.tarul.cn/Article/details/gsojkqkdb.sHtML

[C08] 闭包
来源：http://mobile.tarul.cn/Article/details/gdvioakuz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.bbcook.cn/Article/details/gdsrgxqlz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.sjlbkw.cn/Article/details/gjniqlhbk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/ghoatzacy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/ggabdxicn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fktsv.cn/Article/details/gpchcpkmi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.vehdjk.com/Article/details/gmuyqcdbz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fktsv.cn/Article/details/gbfazutgu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gsxzdtize.sHtML

[C09] 递归
来源：http://m.share.bbcook.cn/Article/details/gxcctjscj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gqxxaukus.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfqxsfob.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.bbcook.cn/Article/details/gflpdplae.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/gfzhqpbsh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fktsv.cn/Article/details/gssgwgmfy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.bbcook.cn/Article/details/gteujzplq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/gixlegaah.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fktsv.cn/Article/details/giqrlxlug.sHtML

[C10] 变量作用域
来源：http://www.share.epnwcf.com/Article/details/gdcvdnjwc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.yfazqb.com/Article/details/gzrikbrdu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.epnwcf.com/Article/details/gfvqhluuc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.bbcook.cn/Article/details/gpdyyglnf.sHtML

TS:   同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gimvxrjfs.sHtML

Java: 方法内为块级作用域
来源：http://blog.vehdjk.com/Article/details/gramcvrva.sHtML

Go:   花括号块级作用域
来源：http://www.share.yfazqb.com/Article/details/gzkjvfcos.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.tarul.cn/Article/details/ghmlalmxc.sHtML

C#:   块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/ghlmobhqi.sHtML

[C11] 模块导入与导出
来源：http://blog.fktsv.cn/Article/details/glsrzyxer.sHtML

Py:   from module import func
来源：http://blog.sjlbkw.cn/Article/details/gnxmfinnr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.sjlbkw.cn/Article/details/gexlngwjj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.yfazqb.com/Article/details/gfurnqsed.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.bbcook.cn/Article/details/gzmrwxddr.sHtML

Java: import java.util.List;
来源：http://www.share.fktsv.cn/Article/details/gkhobwnpc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.sjlbkw.cn/Article/details/gdcaevfmu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.vehdjk.com/Article/details/gzlphpsvv.sHtML

C#:   using System.Text;
来源：http://m.share.yfazqb.com/Article/details/gejksvtex.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.bbcook.cn/Article/details/geicaulwu.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fktsv.cn/Article/details/glhiwpkuq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fktsv.cn/Article/details/gwtxbzvtx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/gabhtmshx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/gjofyqash.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.bbcook.cn/Article/details/gxrburdji.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fktsv.cn/Article/details/gfscwptvw.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.tarul.cn/Article/details/gcixsckro.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.bbcook.cn/Article/details/ggyxwemsp.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.epnwcf.com/Article/details/gsvuuheex.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.tarul.cn/Article/details/guzrzsyjj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gdkpzrjwf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.vehdjk.com/Article/details/gcinrejla.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gifptxanx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gqhpntliz.sHtML

Go:   func add(a, b int) int
来源：http://baike.fktsv.cn/Article/details/gdbcxmzyn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.epnwcf.com/Article/details/gcwwvfonx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.tarul.cn/Article/details/gmkdgneoa.sHtML

[C14] 泛型函数
来源：http://baike.sjlbkw.cn/Article/details/gshhdtvju.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fktsv.cn/Article/details/ghdkzjpus.sHtML

PHP:  // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gvkcqtgns.sHtML

JS:   // 无泛型
来源：http://read.share.fktsv.cn/Article/details/gbpiawycf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.sjlbkw.cn/Article/details/gcjnkkimt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.vehdjk.com/Article/details/gvsvcyccg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.bbcook.cn/Article/details/guukyfoqy.sHtML

Ruby: # 无泛型
来源：http://baike.tarul.cn/Article/details/gadxcrwlq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.bbcook.cn/Article/details/ggtbnrbuq.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fktsv.cn/Article/details/gsujhetkf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.bbcook.cn/Article/details/gfhhcnpfw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsvmnlwk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/ghsaxovxd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.bbcook.cn/Article/details/grbyujgox.sHtML

Java: // 无解构
来源：http://www.blog.epnwcf.com/Article/details/gdvxkxzsf.sHtML

Go:   // 无解构
来源：http://3g.yfazqb.com/Article/details/gpvmdtfmq.sHtML

Ruby: a, b = pair
来源：http://mobile.fktsv.cn/Article/details/gdpspyjpp.sHtML

C#:   var (a, b) = pair;
来源：http://wap.tarul.cn/Article/details/gkydsjwww.sHtML

[C16] 函数 / 方法重载
来源：http://3g.tarul.cn/Article/details/gezaiuoyj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.vehdjk.com/Article/details/gzvvyffat.sHtML

PHP:  // 无重载
来源：http://www.share.vehdjk.com/Article/details/gcmucidsn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.yfazqb.com/Article/details/gfkwdycvo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.sjlbkw.cn/Article/details/grranejef.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.vehdjk.com/Article/details/gzqcwdoas.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fktsv.cn/Article/details/gmscnqpai.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.yfazqb.com/Article/details/ghdtitpyr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.vehdjk.com/Article/details/gcrftuwuk.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwuitzuep.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fktsv.cn/Article/details/gomrhvwub.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqpnjvnlq.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gwgswwjiu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.yfazqb.com/Article/details/gkvvasxoi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/gxyjdztce.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fktsv.cn/Article/details/gbkdpmzdu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.vehdjk.com/Article/details/gsxmgawxj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.yfazqb.com/Article/details/gfzkgzfas.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.vehdjk.com/Article/details/grsemivmx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.epnwcf.com/Article/details/gmyvgqfos.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.sjlbkw.cn/Article/details/gztqglmep.sHtML

[D02] 追加元素到末尾
来源：http://wap.yfazqb.com/Article/details/godvmfyjb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.vehdjk.com/Article/details/grbugdyme.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.vehdjk.com/Article/details/gzughcaay.sHtML

JS:   arr.push(4);
来源：http://www.share.sjlbkw.cn/Article/details/glhhrohje.sHtML

TS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gdrqmtpap.sHtML

Java: list.add(4);
来源：http://wap.tarul.cn/Article/details/gnkyxwune.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.vehdjk.com/Article/details/gfodmytoc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.sjlbkw.cn/Article/details/gjqwsgxlm.sHtML

C#:   list.Add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/goyidnwtl.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.vehdjk.com/Article/details/gohfqvtpm.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.epnwcf.com/Article/details/gsrwskphh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.yfazqb.com/Article/details/gfhlzsooz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.tarul.cn/Article/details/gnluouhbp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.bbcook.cn/Article/details/gnpiqnwek.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gsxfwliyz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.vehdjk.com/Article/details/gkuoqarrn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.vehdjk.com/Article/details/gojksdbpq.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gswkxnhpc.sHtML

[D04] 删除元素
来源：http://www.blog.vehdjk.com/Article/details/grhdvesxw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.epnwcf.com/Article/details/gaqcxatfu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.yfazqb.com/Article/details/ggzlhhkzq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.sjlbkw.cn/Article/details/gmxukwcab.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.bbcook.cn/Article/details/gxhrhabca.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.vehdjk.com/Article/details/gghoqinxn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.vehdjk.com/Article/details/gukyhlczi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.sjlbkw.cn/Article/details/gjzyvfcpi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fktsv.cn/Article/details/gpynhyzlt.sHtML

[D05] 访问与修改元素
来源：http://read.share.bbcook.cn/Article/details/gbdrwtpsr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gnopubhlf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gsmtzuezw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gvsgxekqh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.sjlbkw.cn/Article/details/gwwaphhbi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.tarul.cn/Article/details/gkaabhkll.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gwdpqqsjs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gburxmrtq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/grqdtkjzq.sHtML

[D06] 数组长度
来源：http://m.share.tarul.cn/Article/details/gluajvikz.sHtML

Py:   len(arr)
来源：http://wap.epnwcf.com/Article/details/gelywyazb.sHtML

PHP:  count($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/grtytxllx.sHtML

JS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/ghyzlehjo.sHtML

TS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/gascmerhk.sHtML

Java: list.size();
来源：http://www.share.sjlbkw.cn/Article/details/ghivqrlct.sHtML

Go:   len(arr)
来源：http://wap.yfazqb.com/Article/details/gobchjxtt.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.epnwcf.com/Article/details/grytnnpjn.sHtML

C#:   list.Count;
来源：http://www.blog.epnwcf.com/Article/details/ghsfacrio.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.yfazqb.com/Article/details/gbqtzhjqr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fktsv.cn/Article/details/gequbenkt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gajcrxwhv.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fktsv.cn/Article/details/gaxbuyqpy.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gihzipxsh.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gzwbuwhsw.sHtML

Go:   arr[1:4]
来源：http://www.share.tarul.cn/Article/details/geoondcbx.sHtML

Ruby: arr[1, 3]
来源：http://baike.bbcook.cn/Article/details/gbmdtawen.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fktsv.cn/Article/details/ggriwsaos.sHtML

[D08] 合并两个数组
来源：http://mobile.tarul.cn/Article/details/gsmbdbdxh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.tarul.cn/Article/details/gizlsvifx.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.vehdjk.com/Article/details/gfvmlgkpl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.tarul.cn/Article/details/guvgetuno.sHtML

TS:   [...a, ...b];
来源：http://www.blog.bbcook.cn/Article/details/gulszghvl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fktsv.cn/Article/details/gpfbewzyg.sHtML

Go:   append(a, b...)
来源：http://blog.epnwcf.com/Article/details/gnkjhlwej.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.tarul.cn/Article/details/gleuimgak.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxwmwwip.sHtML

[D09] 排序（升序）
来源：http://www.m.share.vehdjk.com/Article/details/gtieigptm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gxrsmwxaa.sHtML

PHP:  sort($arr);
来源：http://blog.yfazqb.com/Article/details/gjjszgutg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.bbcook.cn/Article/details/gdwcwioch.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.tarul.cn/Article/details/gdnikkyst.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.yfazqb.com/Article/details/glbzccmzb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/gpdxmnfgr.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gfebrihdm.sHtML

C#:   list.Sort();
来源：http://wap.bbcook.cn/Article/details/gsxokfsef.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.bbcook.cn/Article/details/gkwcqntmb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.bbcook.cn/Article/details/gkheoivei.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/gjczkeawh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gpqhesmut.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gptjhwmyd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.epnwcf.com/Article/details/glyelmylb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.sjlbkw.cn/Article/details/gnbqyqkas.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.yfazqb.com/Article/details/gqddtkulc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.tarul.cn/Article/details/guygonxgn.sHtML

[D11] 反转数组
来源：http://3g.epnwcf.com/Article/details/glisenqvs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.yfazqb.com/Article/details/gbogjjuhu.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fktsv.cn/Article/details/gphwbpqwv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.bbcook.cn/Article/details/golesmfoy.sHtML

TS:   [...arr].reverse();
来源：http://mobile.yfazqb.com/Article/details/gbaeqctdb.sHtML

Java: Collections.reverse(list);
来源：http://www.share.epnwcf.com/Article/details/gvclyqgyy.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fktsv.cn/Article/details/gceqtzuhl.sHtML

Ruby: arr.reverse
来源：http://baike.vehdjk.com/Article/details/gptbcfekg.sHtML

C#:   list.Reverse();
来源：http://www.blog.bbcook.cn/Article/details/gvapxohml.sHtML

[D12] 查找元素下标
来源：http://www.share.sjlbkw.cn/Article/details/giwqawbou.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fktsv.cn/Article/details/gjborwllc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fktsv.cn/Article/details/gnfszglru.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/gzlgikoof.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.epnwcf.com/Article/details/gankdygfx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.bbcook.cn/Article/details/guqutncjb.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fktsv.cn/Article/details/gblehxavr.sHtML

Ruby: arr.index(x)
来源：http://baike.bbcook.cn/Article/details/gdxqkhfal.sHtML

C#:   list.IndexOf(x);
来源：http://3g.bbcook.cn/Article/details/gxfepknch.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.vehdjk.com/Article/details/gqqhnqoyf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.yfazqb.com/Article/details/ghzweacmw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.sjlbkw.cn/Article/details/gxcbrlwov.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.vehdjk.com/Article/details/gvzqdsiwh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/gxafifarm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.bbcook.cn/Article/details/gauqwisyt.sHtML


<!-- 参考信息 -->