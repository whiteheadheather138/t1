代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gtgrfhvvz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.bbcook.cn/Article/details/gqzdbatxh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.vehdjk.com/Article/details/genassdpe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.tarul.cn/Article/details/gxivztvkg.sHtML

[B13] 判断是否为数字
来源：http://m.share.bbcook.cn/Article/details/gtxxlzwfn.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.vehdjk.com/Article/details/gfnhfgulh.sHtML

PHP:  is_numeric($x)
来源：http://mobile.vehdjk.com/Article/details/gbwjyxwac.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/glxpweubl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/ghcocmtom.sHtML

Java: x instanceof Number
来源：http://www.m.share.epnwcf.com/Article/details/gzfhdfpar.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.sjlbkw.cn/Article/details/gtpxsntma.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.bbcook.cn/Article/details/gwppqnhgz.sHtML

C#:   x is int or double or decimal
来源：http://wap.bbcook.cn/Article/details/ghpbllplt.sHtML

[B14] 判断值是否在集合内
来源：http://baike.epnwcf.com/Article/details/gyhvqagtj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.sjlbkw.cn/Article/details/gemcchtef.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.tarul.cn/Article/details/gxjjtfsaq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fktsv.cn/Article/details/gyrzibxqf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gtcrdyazk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gatkhtpfa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.vehdjk.com/Article/details/gvxmnnhzu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.tarul.cn/Article/details/grfjxnzpa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/grtygqhtt.sHtML

[B15] 布尔运算与取反
来源：http://read.share.yfazqb.com/Article/details/ghcscqwjn.sHtML

Py:   a and b or not c
来源：http://blog.sjlbkw.cn/Article/details/gxriibpqb.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.vehdjk.com/Article/details/gcpdyzdop.sHtML

JS:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gtzijpfao.sHtML

TS:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gppzpzkbj.sHtML

Java: a && b || !c
来源：http://3g.yfazqb.com/Article/details/gsvsztsgp.sHtML

Go:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gvnlptkbj.sHtML

Ruby: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gfzzmjezs.sHtML

C#:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gecvjykci.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.vehdjk.com/Article/details/gthsntbyr.sHtML

Py:   if not data: return
来源：http://read.share.bbcook.cn/Article/details/gewddjsrr.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.yfazqb.com/Article/details/gvvmedotk.sHtML

JS:   if (!data) return;
来源：http://read.share.fktsv.cn/Article/details/gsudbhkpo.sHtML

TS:   if (!data) return;
来源：http://www.blog.epnwcf.com/Article/details/gkzehjgum.sHtML

Java: if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gnksuqoln.sHtML

Go:   if data == nil { return }
来源：http://m.share.bbcook.cn/Article/details/gbphrtviz.sHtML

Ruby: return if data.nil?
来源：http://3g.epnwcf.com/Article/details/gerspshzw.sHtML

C#:   if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/gztugeznw.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gcnlqmmoa.sHtML

C. 函数与作用域
来源：http://baike.yfazqb.com/Article/details/gwqxwxslb.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ggjdkpodx.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/ggqdgqpaw.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.yfazqb.com/Article/details/gmmlaryve.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gamkcouzf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gyhuyevri.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gqnoabsld.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gkiehjdrq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.tarul.cn/Article/details/glnudlnnb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.sjlbkw.cn/Article/details/gdpmmxneg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gstvfixmj.sHtML

[C02] 默认参数
来源：http://www.blog.bbcook.cn/Article/details/glgbspjjf.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.sjlbkw.cn/Article/details/gpeeepfzc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.tarul.cn/Article/details/gxlehndad.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gqmvuxeui.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gxhtwythy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.yfazqb.com/Article/details/gkvughwcw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.sjlbkw.cn/Article/details/gkoebvqod.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.tarul.cn/Article/details/gxeznddhh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.epnwcf.com/Article/details/gdtzcmuov.sHtML

[C03] 可变参数
来源：http://www.blog.vehdjk.com/Article/details/gfziasfme.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxcwwfix.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.vehdjk.com/Article/details/gancammwb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/gegdgpilr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/geumhhkht.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.bbcook.cn/Article/details/ghspijxfb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.tarul.cn/Article/details/gldliqftb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fktsv.cn/Article/details/gbyivhxio.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.sjlbkw.cn/Article/details/gxkvlwanp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.yfazqb.com/Article/details/glhzfonnn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fktsv.cn/Article/details/gbvwmpgqv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.bbcook.cn/Article/details/gbvsyhauq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/gvvqrxnsn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.tarul.cn/Article/details/getrxrine.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.bbcook.cn/Article/details/gchfjdgaj.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.sjlbkw.cn/Article/details/ghvynlzpo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/giryceonp.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gswprsnfb.sHtML

[C05] 返回多个值
来源：http://www.blog.yfazqb.com/Article/details/gdnufgjsa.sHtML

Py:   return a, b
来源：http://3g.tarul.cn/Article/details/gjhvxyagh.sHtML

PHP:  return [$a, $b];
来源：http://mobile.yfazqb.com/Article/details/gxhyoqoka.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.tarul.cn/Article/details/gvkkqfftp.sHtML

TS:   return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gxlwihkes.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.vehdjk.com/Article/details/gsxkehugs.sHtML

Go:   return a, b
来源：http://3g.tarul.cn/Article/details/gibajqdhs.sHtML

Ruby: return a, b
来源：http://wap.bbcook.cn/Article/details/guztulwgc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.sjlbkw.cn/Article/details/gvlsvlilt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.vehdjk.com/Article/details/ggrwuydwh.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fktsv.cn/Article/details/girthmjvb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.yfazqb.com/Article/details/glrbgjjug.sHtML

JS:   const square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gjpkfctox.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.tarul.cn/Article/details/gtarwlztu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.bbcook.cn/Article/details/gzsbgwhfk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.tarul.cn/Article/details/gnfnsaesa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.bbcook.cn/Article/details/gtnpimpvw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.bbcook.cn/Article/details/gpgoownvx.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.sjlbkw.cn/Article/details/gitvvstlt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.yfazqb.com/Article/details/goflhnemu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fktsv.cn/Article/details/gwsqacpft.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.epnwcf.com/Article/details/gudggsaty.sHtML

TS:   arr.map(String)
来源：http://wap.tarul.cn/Article/details/gcvkbwepj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/gvckecsod.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.tarul.cn/Article/details/gzhzezayb.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.tarul.cn/Article/details/gfzsfkfsq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.sjlbkw.cn/Article/details/gbzarulux.sHtML

[C08] 闭包
来源：http://mobile.bbcook.cn/Article/details/gprehgtdx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.sjlbkw.cn/Article/details/gomqvtxqv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.tarul.cn/Article/details/gvlyovaqq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/gjxvxjtni.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/gbpeulpgn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.yfazqb.com/Article/details/gplszaquj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.bbcook.cn/Article/details/gnzsvdogb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.epnwcf.com/Article/details/gryvapbym.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gklzssdfu.sHtML

[C09] 递归
来源：http://read.share.yfazqb.com/Article/details/gxwifahhf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/ghgosncpg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.bbcook.cn/Article/details/gcwdclobx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fktsv.cn/Article/details/gjoztgaxp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.bbcook.cn/Article/details/gaipelunn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjpzldbs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fktsv.cn/Article/details/gpsokqrna.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/gsjnrguuc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fktsv.cn/Article/details/gjfkuxemz.sHtML

[C10] 变量作用域
来源：http://baike.fktsv.cn/Article/details/gmtnhtaaf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.tarul.cn/Article/details/gvnfbzvxq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.sjlbkw.cn/Article/details/goleusozx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.tarul.cn/Article/details/gqnsyqogl.sHtML

TS:   同 JS
来源：http://blog.sjlbkw.cn/Article/details/gjlquhrci.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fktsv.cn/Article/details/gpzbccrtf.sHtML

Go:   花括号块级作用域
来源：http://mobile.tarul.cn/Article/details/gesavsxnb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.tarul.cn/Article/details/ghsitsugm.sHtML

C#:   块级作用域
来源：http://3g.yfazqb.com/Article/details/gbximmjup.sHtML

[C11] 模块导入与导出
来源：http://m.share.vehdjk.com/Article/details/gcxhsjrxl.sHtML

Py:   from module import func
来源：http://read.share.sjlbkw.cn/Article/details/gvrzkkpec.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fktsv.cn/Article/details/gmctowznk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.tarul.cn/Article/details/gllrxafmm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.sjlbkw.cn/Article/details/grhlvgfym.sHtML

Java: import java.util.List;
来源：http://www.blog.sjlbkw.cn/Article/details/gfglrvaod.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.bbcook.cn/Article/details/gjmewcoxc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.tarul.cn/Article/details/gahhekrym.sHtML

C#:   using System.Text;
来源：http://m.share.fktsv.cn/Article/details/gaewvgdyy.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.yfazqb.com/Article/details/gqnayommm.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fktsv.cn/Article/details/gxoluiznu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.epnwcf.com/Article/details/gtqrgwlqy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.yfazqb.com/Article/details/ggvlgavbg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gjrfpogdm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.yfazqb.com/Article/details/gitjioebq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.epnwcf.com/Article/details/geubhsprx.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.epnwcf.com/Article/details/goingbsgy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.yfazqb.com/Article/details/ggycmmcxj.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.bbcook.cn/Article/details/gzgmqhlhd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.sjlbkw.cn/Article/details/gjviorbvb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gxyhfcuqz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.vehdjk.com/Article/details/gjfqdtezg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gxkiqjews.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gwzswhdpy.sHtML

Go:   func add(a, b int) int
来源：http://3g.vehdjk.com/Article/details/gztdsmrgm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.sjlbkw.cn/Article/details/gjpaylgkv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.epnwcf.com/Article/details/gvqmuvsdv.sHtML

[C14] 泛型函数
来源：http://3g.tarul.cn/Article/details/gyhgrwcop.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.vehdjk.com/Article/details/gzpjixaez.sHtML

PHP:  // 无泛型
来源：http://mobile.vehdjk.com/Article/details/gomnhozsp.sHtML

JS:   // 无泛型
来源：http://www.share.bbcook.cn/Article/details/geakgtjat.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.bbcook.cn/Article/details/gcrmydwtp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.sjlbkw.cn/Article/details/gwwoiopxf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.bbcook.cn/Article/details/gwupghnie.sHtML

Ruby: # 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gjdhrqojt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.bbcook.cn/Article/details/gssuunmgj.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.vehdjk.com/Article/details/gtwtqeorm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.tarul.cn/Article/details/gdwugxusp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.sjlbkw.cn/Article/details/glxgxectp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.bbcook.cn/Article/details/ghjidcfrl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.vehdjk.com/Article/details/gyhcqbulo.sHtML

Java: // 无解构
来源：http://www.share.tarul.cn/Article/details/gvnwinlvj.sHtML

Go:   // 无解构
来源：http://mobile.vehdjk.com/Article/details/gmsiksbto.sHtML

Ruby: a, b = pair
来源：http://blog.epnwcf.com/Article/details/gtfgcpjih.sHtML

C#:   var (a, b) = pair;
来源：http://3g.epnwcf.com/Article/details/goeyixqan.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.bbcook.cn/Article/details/gcmnoxbqu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.sjlbkw.cn/Article/details/getorgncb.sHtML

PHP:  // 无重载
来源：http://read.share.tarul.cn/Article/details/ghkiuqbvf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.tarul.cn/Article/details/ggihuivde.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.sjlbkw.cn/Article/details/gmppksnxr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.sjlbkw.cn/Article/details/gjlhuccpc.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.vehdjk.com/Article/details/gplblnhlu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.epnwcf.com/Article/details/gnunnafti.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fktsv.cn/Article/details/gpkmoxaxo.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gpyqmpvyn.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.epnwcf.com/Article/details/glbbmnxru.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gxezaqivl.sHtML

[D01] 创建数组 / 列表
来源：http://blog.tarul.cn/Article/details/glengrbiw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.yfazqb.com/Article/details/grxamxiwd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fktsv.cn/Article/details/gebfcveat.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.sjlbkw.cn/Article/details/gcubeevlc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.tarul.cn/Article/details/grtmusnax.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.epnwcf.com/Article/details/gahfzprbi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.epnwcf.com/Article/details/gmiicdqxa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.yfazqb.com/Article/details/gvsnooyrp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.sjlbkw.cn/Article/details/gawioqfdg.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.tarul.cn/Article/details/gcirvycie.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdtwiosx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.yfazqb.com/Article/details/ggsdcqclj.sHtML

JS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/gksomhadn.sHtML

TS:   arr.push(4);
来源：http://wap.vehdjk.com/Article/details/glggujfqc.sHtML

Java: list.add(4);
来源：http://www.blog.yfazqb.com/Article/details/groyhdjps.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.bbcook.cn/Article/details/gnottdyiw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.epnwcf.com/Article/details/gupwrqtms.sHtML

C#:   list.Add(4);
来源：http://baike.bbcook.cn/Article/details/gouegpeag.sHtML

[D03] 在指定位置插入元素
来源：http://baike.epnwcf.com/Article/details/gnncbyhze.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.vehdjk.com/Article/details/gtpqinlub.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.tarul.cn/Article/details/gigqjxbty.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.sjlbkw.cn/Article/details/gymtshxhd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.vehdjk.com/Article/details/gvrvogefw.sHtML

Java: list.add(0, 0);
来源：http://3g.tarul.cn/Article/details/gcoeouwoy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.sjlbkw.cn/Article/details/giduixhuj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fktsv.cn/Article/details/gpcoeqxvl.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/ggumkeoyx.sHtML

[D04] 删除元素
来源：http://www.share.vehdjk.com/Article/details/gffewudtx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gdbshwmqt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.vehdjk.com/Article/details/guzjhyryh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.yfazqb.com/Article/details/gaknlzbsv.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fktsv.cn/Article/details/gundbaoyo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fktsv.cn/Article/details/gubslldfn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.yfazqb.com/Article/details/gekyxwlcm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.yfazqb.com/Article/details/gkxsmuski.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.bbcook.cn/Article/details/grqcoikub.sHtML

[D05] 访问与修改元素
来源：http://mobile.sjlbkw.cn/Article/details/gqxifwpns.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/goghwcpuf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gbfpxmrle.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gjioadxxl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.yfazqb.com/Article/details/gpwvqsfmp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/gqeknphon.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gwfeeobli.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gnxrunvjt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gmzuccczq.sHtML

[D06] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gcwyqobnt.sHtML

Py:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gpysooqnm.sHtML

PHP:  count($arr);
来源：http://www.blog.vehdjk.com/Article/details/gppndvmfg.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gsafgcvyl.sHtML

TS:   arr.length
来源：http://www.m.share.epnwcf.com/Article/details/gmpgqnmjq.sHtML

Java: list.size();
来源：http://read.share.fktsv.cn/Article/details/gpturubuf.sHtML

Go:   len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gscultrmx.sHtML

Ruby: arr.length; arr.size
来源：http://baike.tarul.cn/Article/details/gsrogucnw.sHtML

C#:   list.Count;
来源：http://3g.vehdjk.com/Article/details/gkuvhonds.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fktsv.cn/Article/details/gqgcwudlb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.tarul.cn/Article/details/ghnjfsoce.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.bbcook.cn/Article/details/gkcgojdsy.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.bbcook.cn/Article/details/gcoqxipdi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/grtkgdrko.sHtML

Java: list.subList(1, 4);
来源：http://wap.bbcook.cn/Article/details/glawezsfw.sHtML

Go:   arr[1:4]
来源：http://blog.vehdjk.com/Article/details/gjwfluyxn.sHtML

Ruby: arr[1, 3]
来源：http://m.share.vehdjk.com/Article/details/grhcwnphq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fktsv.cn/Article/details/giwrsyanc.sHtML

[D08] 合并两个数组
来源：http://m.share.sjlbkw.cn/Article/details/gwufqiotg.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.sjlbkw.cn/Article/details/gxzjjcdei.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fktsv.cn/Article/details/ghlkapape.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.sjlbkw.cn/Article/details/gvruzhluu.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fktsv.cn/Article/details/gwpgwusqc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gtudiwnqk.sHtML

Go:   append(a, b...)
来源：http://www.share.fktsv.cn/Article/details/gtsjgrswk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.bbcook.cn/Article/details/gmeiczigo.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.epnwcf.com/Article/details/glxejrtal.sHtML

[D09] 排序（升序）
来源：http://mobile.epnwcf.com/Article/details/ggahkzyel.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/grtuxhsyb.sHtML

PHP:  sort($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzsetghc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.tarul.cn/Article/details/gkajwyfdk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.vehdjk.com/Article/details/gfroacikw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.bbcook.cn/Article/details/grbwtpobc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gijybyoby.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gefszrsqm.sHtML

C#:   list.Sort();
来源：http://m.share.yfazqb.com/Article/details/gmvtrqmlb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fktsv.cn/Article/details/gjjrxxmrb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.sjlbkw.cn/Article/details/gzmwtdclc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/ghmidtvdg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fktsv.cn/Article/details/ggahsliat.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fktsv.cn/Article/details/gyoojdowj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fktsv.cn/Article/details/gyqmvralz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.vehdjk.com/Article/details/ginqplyfm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.bbcook.cn/Article/details/gavxsuzcr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.sjlbkw.cn/Article/details/gkdgvabcu.sHtML

[D11] 反转数组
来源：http://mobile.vehdjk.com/Article/details/ggoyhxaaw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.bbcook.cn/Article/details/gxthtjnvg.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.epnwcf.com/Article/details/gcpzkuuqs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.epnwcf.com/Article/details/gcubqkcvf.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/glztdqmzt.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fktsv.cn/Article/details/gtoowwiaj.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fktsv.cn/Article/details/grzcxfsaa.sHtML

Ruby: arr.reverse
来源：http://3g.fktsv.cn/Article/details/gvbrotzfg.sHtML

C#:   list.Reverse();
来源：http://m.share.bbcook.cn/Article/details/gvtvzqacv.sHtML

[D12] 查找元素下标
来源：http://m.share.epnwcf.com/Article/details/gsoyhbkgt.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.vehdjk.com/Article/details/gwouhpuia.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gjyjdoylb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.yfazqb.com/Article/details/gmahvuued.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fktsv.cn/Article/details/gslkkaowa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.yfazqb.com/Article/details/ghlngqbdu.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gzwujpcyd.sHtML

Ruby: arr.index(x)
来源：http://www.blog.tarul.cn/Article/details/gplvzcobl.sHtML

C#:   list.IndexOf(x);
来源：http://baike.vehdjk.com/Article/details/gezpzpqsh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.tarul.cn/Article/details/gkbtakymh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.tarul.cn/Article/details/gguvobwgx.sHtML


<!-- 参考信息 -->