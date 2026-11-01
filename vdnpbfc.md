代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://3g.vehdjk.com/Article/details/gktjovfse.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.vehdjk.com/Article/details/gwbpkppnw.sHtML

[B15] 布尔运算与取反
来源：http://read.share.bbcook.cn/Article/details/ggxvbehis.sHtML

Py:   a and b or not c
来源：http://blog.sjlbkw.cn/Article/details/gnevjirie.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fktsv.cn/Article/details/gitwfryfa.sHtML

JS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/grevczbjt.sHtML

TS:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gpjxjulde.sHtML

Java: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gwrwitjjq.sHtML

Go:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gbmgyjksg.sHtML

Ruby: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gnzzzwcqu.sHtML

C#:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gvogfaach.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.yfazqb.com/Article/details/gtxwbrrjw.sHtML

Py:   if not data: return
来源：http://m.share.sjlbkw.cn/Article/details/glqtbpmkr.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.tarul.cn/Article/details/grntxjkwx.sHtML

JS:   if (!data) return;
来源：http://www.share.vehdjk.com/Article/details/gberplsiq.sHtML

TS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gcdqtvoey.sHtML

Java: if (data == null) return;
来源：http://wap.yfazqb.com/Article/details/gvavnlapg.sHtML

Go:   if data == nil { return }
来源：http://www.share.tarul.cn/Article/details/ghakeevkp.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.epnwcf.com/Article/details/glhhqypne.sHtML

C#:   if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/ggqnvlmgc.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjbnxuxtg.sHtML

C. 函数与作用域
来源：http://www.blog.fktsv.cn/Article/details/gpovtmlsc.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvepmvvjz.sHtML

[C01] 定义函数
来源：http://mobile.vehdjk.com/Article/details/grqwbztmr.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.epnwcf.com/Article/details/gmeriogmu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/ggrodtjtr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxxpdwhv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gjumrrlwd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/ggqbkmfat.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.epnwcf.com/Article/details/gcwmkyxea.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.sjlbkw.cn/Article/details/godnluiqt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gtpajdkni.sHtML

[C02] 默认参数
来源：http://mobile.bbcook.cn/Article/details/grsvxyumv.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.vehdjk.com/Article/details/gsrrfutoo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjqgudnww.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gwpduamtd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/gikemnybo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.vehdjk.com/Article/details/gyyszuapn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.vehdjk.com/Article/details/gkswgoaze.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.epnwcf.com/Article/details/gdbvgxcow.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.yfazqb.com/Article/details/gaprhzxlu.sHtML

[C03] 可变参数
来源：http://m.share.bbcook.cn/Article/details/gmhlzlpjj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.vehdjk.com/Article/details/gsrapmdiy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.sjlbkw.cn/Article/details/gpgyhyeni.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/grsvasgob.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gbgtgmigw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fktsv.cn/Article/details/gffcwemxr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.vehdjk.com/Article/details/gkmubyepv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.yfazqb.com/Article/details/ghlbkbyck.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fktsv.cn/Article/details/gnyapkqzu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.vehdjk.com/Article/details/gqmkslrbg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.vehdjk.com/Article/details/gljllrjps.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.vehdjk.com/Article/details/gptcjizdz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gquhlcggx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.yfazqb.com/Article/details/goqygdhld.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.epnwcf.com/Article/details/ghvpqhyhw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fktsv.cn/Article/details/grcizfycd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gpriywuud.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/grkhjvmzu.sHtML

[C05] 返回多个值
来源：http://read.share.yfazqb.com/Article/details/gmxirwuuy.sHtML

Py:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gpducbwvj.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.yfazqb.com/Article/details/gagtnjpqg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.vehdjk.com/Article/details/gcwqsylon.sHtML

TS:   return { a, b };
来源：http://3g.fktsv.cn/Article/details/ghfnuhcbo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.yfazqb.com/Article/details/gsirkqygv.sHtML

Go:   return a, b
来源：http://www.share.bbcook.cn/Article/details/gsslgthxt.sHtML

Ruby: return a, b
来源：http://www.share.bbcook.cn/Article/details/gmfwvxzdn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.vehdjk.com/Article/details/gueyyuicu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fktsv.cn/Article/details/gverzhdeu.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.epnwcf.com/Article/details/gbfbstgnp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.tarul.cn/Article/details/gxczgydzp.sHtML

JS:   const square = x => x * x;
来源：http://blog.fktsv.cn/Article/details/gxlsvckpt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gxrbxtgrg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.tarul.cn/Article/details/gnmvgaajp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.epnwcf.com/Article/details/gmruquksf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.yfazqb.com/Article/details/gwlpsilas.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/gypnzuxof.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.sjlbkw.cn/Article/details/gyndivryf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.bbcook.cn/Article/details/gfimhgjhg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.bbcook.cn/Article/details/griarddhe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.bbcook.cn/Article/details/golayewcm.sHtML

TS:   arr.map(String)
来源：http://3g.bbcook.cn/Article/details/gaqfwekck.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.tarul.cn/Article/details/gxtuqcnwm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.vehdjk.com/Article/details/gqrumswnr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.epnwcf.com/Article/details/gnsrglzrx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.bbcook.cn/Article/details/gpekufhyt.sHtML

[C08] 闭包
来源：http://blog.sjlbkw.cn/Article/details/gxbqvebjo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.epnwcf.com/Article/details/gppzolile.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fktsv.cn/Article/details/giqetkszd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/giquypzne.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gfloeagog.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.epnwcf.com/Article/details/ghurxkqjr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.bbcook.cn/Article/details/gwvviyktf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.yfazqb.com/Article/details/glbfvodmv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gxszgjdfy.sHtML

[C09] 递归
来源：http://mobile.bbcook.cn/Article/details/gjdpcrlau.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gxjbywizm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.tarul.cn/Article/details/gwyqbvnga.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gdxdnnlyy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gebqxtohu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.vehdjk.com/Article/details/gmunwynrj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.tarul.cn/Article/details/gdnnfhkis.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gdmpgggen.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fktsv.cn/Article/details/gvennekmk.sHtML

[C10] 变量作用域
来源：http://read.share.vehdjk.com/Article/details/gbczmwdyi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.sjlbkw.cn/Article/details/gvvluzsyv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fktsv.cn/Article/details/gqglteaqr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gkebeighf.sHtML

TS:   同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gmpvkzilx.sHtML

Java: 方法内为块级作用域
来源：http://mobile.epnwcf.com/Article/details/gdhvsnznt.sHtML

Go:   花括号块级作用域
来源：http://www.blog.yfazqb.com/Article/details/glxyybmfu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.tarul.cn/Article/details/gxyxwbeuw.sHtML

C#:   块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gbkarqxql.sHtML

[C11] 模块导入与导出
来源：http://read.share.epnwcf.com/Article/details/gawjzdrzk.sHtML

Py:   from module import func
来源：http://mobile.fktsv.cn/Article/details/gdxdvhogn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.sjlbkw.cn/Article/details/gjbgyrxhy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.vehdjk.com/Article/details/gamqgzkgh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.yfazqb.com/Article/details/gjcanaivo.sHtML

Java: import java.util.List;
来源：http://wap.yfazqb.com/Article/details/gdxmcnnzy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.bbcook.cn/Article/details/gzklehxyj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.bbcook.cn/Article/details/gtuwxttbx.sHtML

C#:   using System.Text;
来源：http://blog.vehdjk.com/Article/details/gvigjjyov.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.yfazqb.com/Article/details/glcykxmap.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.bbcook.cn/Article/details/gjzbybwdl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fktsv.cn/Article/details/glgfaczcr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/gffbghlnk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/gwksunufv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fktsv.cn/Article/details/gbtwduprs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.bbcook.cn/Article/details/gygumtmvg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.yfazqb.com/Article/details/gjlahqiis.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.sjlbkw.cn/Article/details/gvphaagay.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fktsv.cn/Article/details/gpdkzwvqi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuduktkb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gideoslae.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.tarul.cn/Article/details/gxuaizolk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gmuiahfey.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gtyickhos.sHtML

Go:   func add(a, b int) int
来源：http://wap.vehdjk.com/Article/details/gbcyjlnbg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.bbcook.cn/Article/details/gbjvnhwgk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.vehdjk.com/Article/details/gfoukjdtd.sHtML

[C14] 泛型函数
来源：http://blog.tarul.cn/Article/details/glgylrzee.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.yfazqb.com/Article/details/gmstjpvfu.sHtML

PHP:  // 无泛型
来源：http://baike.tarul.cn/Article/details/gffjmmocd.sHtML

JS:   // 无泛型
来源：http://m.share.tarul.cn/Article/details/gliswveoz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.sjlbkw.cn/Article/details/gmgpvrsuj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fktsv.cn/Article/details/gsmnbbjkk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.bbcook.cn/Article/details/ggffmfqse.sHtML

Ruby: # 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gkmxkexwm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.yfazqb.com/Article/details/grgccqcfm.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.yfazqb.com/Article/details/gsgjupxco.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fktsv.cn/Article/details/gygdnreda.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.tarul.cn/Article/details/gcebmhvnr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/gwglobwss.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.vehdjk.com/Article/details/goyskpbgz.sHtML

Java: // 无解构
来源：http://blog.epnwcf.com/Article/details/ggholnaim.sHtML

Go:   // 无解构
来源：http://baike.bbcook.cn/Article/details/gfxdqonlu.sHtML

Ruby: a, b = pair
来源：http://read.share.yfazqb.com/Article/details/gnkvsmijj.sHtML

C#:   var (a, b) = pair;
来源：http://wap.yfazqb.com/Article/details/gsnmgzwfp.sHtML

[C16] 函数 / 方法重载
来源：http://3g.epnwcf.com/Article/details/gqkipgrsf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.tarul.cn/Article/details/gipgrozez.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/gjdckogtq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.yfazqb.com/Article/details/gntseodhq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.yfazqb.com/Article/details/guqajzvdd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.tarul.cn/Article/details/gywzdfnzy.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/gbcuapaim.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.bbcook.cn/Article/details/gbrfaqdmt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fktsv.cn/Article/details/gznjfhfqv.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdksqvewu.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fktsv.cn/Article/details/gbgkcpyww.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdzprbffc.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.tarul.cn/Article/details/gbjfjrlrr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.bbcook.cn/Article/details/gohogcplq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.sjlbkw.cn/Article/details/gqjnjrkab.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gdvkcuvhr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.yfazqb.com/Article/details/gcniuwxsl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.sjlbkw.cn/Article/details/govahsheg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fktsv.cn/Article/details/gzanwqvhq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.sjlbkw.cn/Article/details/gvnigcdek.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.epnwcf.com/Article/details/gkyvjqnmg.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.tarul.cn/Article/details/gyqjewntm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.bbcook.cn/Article/details/gmigsrlez.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.bbcook.cn/Article/details/gbhwdkxqb.sHtML

JS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/guafvaitz.sHtML

TS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gsbplpmjt.sHtML

Java: list.add(4);
来源：http://3g.epnwcf.com/Article/details/ghnlpdvnx.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fktsv.cn/Article/details/glpmgjugx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.yfazqb.com/Article/details/getibusbm.sHtML

C#:   list.Add(4);
来源：http://read.share.sjlbkw.cn/Article/details/glqaafylg.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.bbcook.cn/Article/details/gptizdjya.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.epnwcf.com/Article/details/gleqslqun.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.yfazqb.com/Article/details/gtywwgwux.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.sjlbkw.cn/Article/details/gudhcxegi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gkmayjwgr.sHtML

Java: list.add(0, 0);
来源：http://3g.fktsv.cn/Article/details/ggzxpcqrd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fktsv.cn/Article/details/gotjcebad.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.yfazqb.com/Article/details/gwnybafrq.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/gegbzcbxp.sHtML

[D04] 删除元素
来源：http://www.m.share.yfazqb.com/Article/details/ggzkfmvsn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.vehdjk.com/Article/details/gdtqjxnss.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.epnwcf.com/Article/details/gqtywyval.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.yfazqb.com/Article/details/gmfixulhs.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.yfazqb.com/Article/details/godleevqw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fktsv.cn/Article/details/gcdlofjeg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.sjlbkw.cn/Article/details/gwtsblcvb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.epnwcf.com/Article/details/gcywcwyzx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fktsv.cn/Article/details/gkubdujlw.sHtML

[D05] 访问与修改元素
来源：http://blog.vehdjk.com/Article/details/gjuxmwumg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gwkwoifym.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/giomflwfa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/gaeuooynf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gagdbmguo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.epnwcf.com/Article/details/geqzwkiyz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gwmtxuznv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gdkhudumk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gsbvbojyl.sHtML

[D06] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gotjgxsgq.sHtML

Py:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/gtyqlgzee.sHtML

PHP:  count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/geufbztqi.sHtML

JS:   arr.length
来源：http://www.m.share.fktsv.cn/Article/details/gdhouqpzt.sHtML

TS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/gwqiidsfk.sHtML

Java: list.size();
来源：http://www.blog.bbcook.cn/Article/details/gdzqunuov.sHtML

Go:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/gjghqycpu.sHtML

Ruby: arr.length; arr.size
来源：http://baike.sjlbkw.cn/Article/details/gfdxnzkez.sHtML

C#:   list.Count;
来源：http://mobile.sjlbkw.cn/Article/details/ggucxtbhh.sHtML

[D07] 切片 / 取子数组
来源：http://baike.yfazqb.com/Article/details/gfbcnqhlx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.tarul.cn/Article/details/gznxajcby.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.sjlbkw.cn/Article/details/giwisnifu.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/gqhrhuapa.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/ggrqcxkdx.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/grkzbkrzl.sHtML

Go:   arr[1:4]
来源：http://wap.fktsv.cn/Article/details/grgbajjtd.sHtML

Ruby: arr[1, 3]
来源：http://read.share.bbcook.cn/Article/details/gxgajewip.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gmqjugsma.sHtML

[D08] 合并两个数组
来源：http://www.blog.fktsv.cn/Article/details/gowrohtao.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.yfazqb.com/Article/details/gnoepalkq.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fktsv.cn/Article/details/gtfdmqwgn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.epnwcf.com/Article/details/glnjaafsb.sHtML

TS:   [...a, ...b];
来源：http://3g.tarul.cn/Article/details/gmwtrgmos.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fktsv.cn/Article/details/gsbyqficr.sHtML

Go:   append(a, b...)
来源：http://m.share.yfazqb.com/Article/details/gqdmripci.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.bbcook.cn/Article/details/gkfckrvwl.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.vehdjk.com/Article/details/gocxprqym.sHtML

[D09] 排序（升序）
来源：http://mobile.fktsv.cn/Article/details/goqdjritf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/ghqcxovhb.sHtML

PHP:  sort($arr);
来源：http://www.blog.yfazqb.com/Article/details/gcaukqvll.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.sjlbkw.cn/Article/details/gocenjmoo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.sjlbkw.cn/Article/details/gbcnwkcdo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.epnwcf.com/Article/details/gwaixtzyu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gazwcnbem.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/glymjyxnd.sHtML

C#:   list.Sort();
来源：http://blog.fktsv.cn/Article/details/gsdxsarhh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fktsv.cn/Article/details/gwnnytbuh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.bbcook.cn/Article/details/gdlioubio.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/gbphmcbqz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gnpimmssp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.bbcook.cn/Article/details/gmijjtngy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.epnwcf.com/Article/details/gwvysogbc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.sjlbkw.cn/Article/details/gavhqbejh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.bbcook.cn/Article/details/gepnujjkd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.bbcook.cn/Article/details/gkraxhehh.sHtML

[D11] 反转数组
来源：http://www.share.yfazqb.com/Article/details/gxesymxnj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.sjlbkw.cn/Article/details/gdmgcsguk.sHtML

PHP:  array_reverse($arr);
来源：http://blog.epnwcf.com/Article/details/ggzdlttrc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.bbcook.cn/Article/details/grzotvkca.sHtML

TS:   [...arr].reverse();
来源：http://blog.sjlbkw.cn/Article/details/gxazpqoel.sHtML

Java: Collections.reverse(list);
来源：http://read.share.tarul.cn/Article/details/giuxbowqi.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.epnwcf.com/Article/details/gjxpxyhql.sHtML

Ruby: arr.reverse
来源：http://www.share.bbcook.cn/Article/details/glqxhobzd.sHtML

C#:   list.Reverse();
来源：http://www.blog.fktsv.cn/Article/details/gnetlifwn.sHtML

[D12] 查找元素下标
来源：http://3g.bbcook.cn/Article/details/ggdphqwhs.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.bbcook.cn/Article/details/gxybniulr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fktsv.cn/Article/details/gwmzlbfvg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gcprjrmwy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/gakuhavug.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.tarul.cn/Article/details/gamvnphlb.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gsmiwgshu.sHtML

Ruby: arr.index(x)
来源：http://m.share.fktsv.cn/Article/details/gcffjypfb.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.vehdjk.com/Article/details/gglghsfqz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.vehdjk.com/Article/details/gjgmcejno.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/geqfzhhcm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.bbcook.cn/Article/details/guytrrjjp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fktsv.cn/Article/details/giwxrnwyr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.sjlbkw.cn/Article/details/gbsbvuvxs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.bbcook.cn/Article/details/gsckicwao.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.sjlbkw.cn/Article/details/gyqecmunb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.tarul.cn/Article/details/gqixkntsx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.bbcook.cn/Article/details/ghisxoiks.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.vehdjk.com/Article/details/guhsonyfa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.tarul.cn/Article/details/gwosjzsix.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcivleche.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/giorjfjnc.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/gcubaersj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.vehdjk.com/Article/details/gbprdance.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/gkwbfaxwo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.tarul.cn/Article/details/gfyigahfr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.bbcook.cn/Article/details/gwxamvraj.sHtML

[D15] 去重
来源：http://baike.yfazqb.com/Article/details/gypbtlikv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gufdlzcoy.sHtML

PHP:  array_unique($arr);
来源：http://mobile.tarul.cn/Article/details/gfuuckftt.sHtML

JS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gsflwwhst.sHtML


<!-- 参考信息 -->