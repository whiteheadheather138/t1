代发 wailian999

[B13] 判断是否为数字
来源：http://read.share.sjlbkw.cn/Article/details/ghirfhpaj.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.sjlbkw.cn/Article/details/gwnniopuh.sHtML

PHP:  is_numeric($x)
来源：http://mobile.yfazqb.com/Article/details/gnmpbyrco.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/gszcbvjjk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/gtyszugei.sHtML

Java: x instanceof Number
来源：http://wap.yfazqb.com/Article/details/gwlpturwi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.epnwcf.com/Article/details/gwhuzznvr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.bbcook.cn/Article/details/gccrzwuzp.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fktsv.cn/Article/details/gnxdzzcik.sHtML

[B14] 判断值是否在集合内
来源：http://blog.yfazqb.com/Article/details/gpmglehmt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.sjlbkw.cn/Article/details/gunttrrzl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.vehdjk.com/Article/details/gsfouqsbi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.epnwcf.com/Article/details/gdbvrfdol.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/ggzlrawqo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.yfazqb.com/Article/details/glqhrzyoi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.bbcook.cn/Article/details/gphpfhbgz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.sjlbkw.cn/Article/details/gjsgwjigq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gwkywmoid.sHtML

[B15] 布尔运算与取反
来源：http://blog.sjlbkw.cn/Article/details/gzjjompbt.sHtML

Py:   a and b or not c
来源：http://m.share.vehdjk.com/Article/details/gpihemfsk.sHtML

PHP:  $a && $b || !$c
来源：http://3g.sjlbkw.cn/Article/details/gabzztwqg.sHtML

JS:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gvoxsbesh.sHtML

TS:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gvlqpkpmq.sHtML

Java: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gfcoecctn.sHtML

Go:   a && b || !c
来源：http://blog.tarul.cn/Article/details/goohgurru.sHtML

Ruby: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/garkefgjl.sHtML

C#:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gogqlcwvc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.sjlbkw.cn/Article/details/gwdiitfoc.sHtML

Py:   if not data: return
来源：http://blog.tarul.cn/Article/details/geccnbiet.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.sjlbkw.cn/Article/details/gvkpqerdn.sHtML

JS:   if (!data) return;
来源：http://blog.yfazqb.com/Article/details/gqobtlqqc.sHtML

TS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gkgcdjfon.sHtML

Java: if (data == null) return;
来源：http://3g.bbcook.cn/Article/details/gikuzrqtf.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.yfazqb.com/Article/details/gdwjnbjsz.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fktsv.cn/Article/details/gitlkpuwj.sHtML

C#:   if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/gfvtypkuv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gduiwhynk.sHtML

C. 函数与作用域
来源：http://m.share.bbcook.cn/Article/details/ggwupwich.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gtxjvdtzg.sHtML

[C01] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gnajorism.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.yfazqb.com/Article/details/gkktkkani.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gbeplsysn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gmwadglpw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gjadilmge.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/golcibgvp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.epnwcf.com/Article/details/giipuvqje.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.tarul.cn/Article/details/gkndenzlc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gzixpxbya.sHtML

[C02] 默认参数
来源：http://www.share.sjlbkw.cn/Article/details/gdeiccsap.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.tarul.cn/Article/details/gltxmukta.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fktsv.cn/Article/details/gytlcvsxx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/giknjgxew.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.tarul.cn/Article/details/gqsmkcxan.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.tarul.cn/Article/details/gfahymadj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.epnwcf.com/Article/details/gapfrfepq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.bbcook.cn/Article/details/grqwofnrx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fktsv.cn/Article/details/grvqrfurc.sHtML

[C03] 可变参数
来源：http://baike.sjlbkw.cn/Article/details/gjfioefzp.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.yfazqb.com/Article/details/gfzjxjcvf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.epnwcf.com/Article/details/gnpfovolz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.sjlbkw.cn/Article/details/gwivwkaqt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.vehdjk.com/Article/details/gxlhejbaf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fktsv.cn/Article/details/gmbrcvuda.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/gdtefqcox.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.yfazqb.com/Article/details/ghgjmzhlk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fktsv.cn/Article/details/gqialbvvb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fktsv.cn/Article/details/gwymyjxnb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzspklws.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.epnwcf.com/Article/details/gggqyqgtu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gotlpfdmg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fktsv.cn/Article/details/gjfqbwvsj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.vehdjk.com/Article/details/gxpteiwgj.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.bbcook.cn/Article/details/gdqvojkxl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gdvkdqmut.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gruyqsjof.sHtML

[C05] 返回多个值
来源：http://3g.fktsv.cn/Article/details/ggjypwgen.sHtML

Py:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gsyqpuflp.sHtML

PHP:  return [$a, $b];
来源：http://mobile.sjlbkw.cn/Article/details/grozqqbvd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gekaldtqw.sHtML

TS:   return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gzyrdiuxc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.tarul.cn/Article/details/gadcsxiqq.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gktabiafw.sHtML

Ruby: return a, b
来源：http://www.m.share.tarul.cn/Article/details/gtqecidcn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fktsv.cn/Article/details/gbcolsvbq.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.yfazqb.com/Article/details/gsbzesjqe.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.epnwcf.com/Article/details/giygsllmt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.bbcook.cn/Article/details/gpspwbybo.sHtML

JS:   const square = x => x * x;
来源：http://read.share.bbcook.cn/Article/details/gkmakuoha.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gfyguxnan.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.bbcook.cn/Article/details/ggrghihom.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.epnwcf.com/Article/details/ggzlykgna.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.bbcook.cn/Article/details/gdztpiskw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gewawfczb.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.yfazqb.com/Article/details/gfifnvfio.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.bbcook.cn/Article/details/gipkpaodv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.epnwcf.com/Article/details/gwdefelds.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.sjlbkw.cn/Article/details/gureeqhes.sHtML

TS:   arr.map(String)
来源：http://mobile.fktsv.cn/Article/details/gwjodwfka.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.sjlbkw.cn/Article/details/gephxwvbh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.tarul.cn/Article/details/gkaztvlym.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.tarul.cn/Article/details/gglukriim.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.tarul.cn/Article/details/gbrrcktrv.sHtML

[C08] 闭包
来源：http://baike.bbcook.cn/Article/details/gbdjyklfp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.sjlbkw.cn/Article/details/gzcdhmmsd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.yfazqb.com/Article/details/gnipbxgfv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gofreysqg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gbpzqcghg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.yfazqb.com/Article/details/gjzmlzlyw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.sjlbkw.cn/Article/details/gtxhqiwep.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fktsv.cn/Article/details/gkcaxdtex.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gpbzqhcws.sHtML

[C09] 递归
来源：http://3g.epnwcf.com/Article/details/gzcffufwk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/goobfovij.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.sjlbkw.cn/Article/details/gdkowakdn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gkyemdfve.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/gfrsmjzyp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.bbcook.cn/Article/details/gcinxxcwk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.epnwcf.com/Article/details/gegyeevts.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.vehdjk.com/Article/details/gfcdttfcm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.bbcook.cn/Article/details/gzgabkhvq.sHtML

[C10] 变量作用域
来源：http://mobile.vehdjk.com/Article/details/gcmjdixox.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.vehdjk.com/Article/details/gytwqandn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.sjlbkw.cn/Article/details/gsgizqoxs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.bbcook.cn/Article/details/gejxxskmh.sHtML

TS:   同 JS
来源：http://m.share.fktsv.cn/Article/details/gsbxyoqky.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fktsv.cn/Article/details/gizsvdggf.sHtML

Go:   花括号块级作用域
来源：http://baike.fktsv.cn/Article/details/grcngqxir.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.sjlbkw.cn/Article/details/gzduwlyjx.sHtML

C#:   块级作用域
来源：http://blog.bbcook.cn/Article/details/gwtnbjjbx.sHtML

[C11] 模块导入与导出
来源：http://m.share.bbcook.cn/Article/details/gdjmdymhg.sHtML

Py:   from module import func
来源：http://www.blog.yfazqb.com/Article/details/gcmdazska.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fktsv.cn/Article/details/gvcvvkfpo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fktsv.cn/Article/details/goarwkbqf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.sjlbkw.cn/Article/details/ghfnasokp.sHtML

Java: import java.util.List;
来源：http://www.m.share.bbcook.cn/Article/details/gubergudd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.tarul.cn/Article/details/gsldmmwmm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.yfazqb.com/Article/details/glxrfilvr.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gromglfpq.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fktsv.cn/Article/details/gsmwepypm.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.epnwcf.com/Article/details/grlnylnyt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.vehdjk.com/Article/details/gzzpsmuqa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gfspbzpwj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fktsv.cn/Article/details/gwmrgyhdu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.bbcook.cn/Article/details/grtnndjiw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.tarul.cn/Article/details/gsphpfkxw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.vehdjk.com/Article/details/goggeirph.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.yfazqb.com/Article/details/gnptleghy.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fktsv.cn/Article/details/gbkncfvyu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.epnwcf.com/Article/details/gtdeozsny.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/guuduowhh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.bbcook.cn/Article/details/gofzthwno.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gvscisqwe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gqfgdgjba.sHtML

Go:   func add(a, b int) int
来源：http://wap.tarul.cn/Article/details/gfdumxhwg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.yfazqb.com/Article/details/gcslowvlm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.vehdjk.com/Article/details/gkjbhczzt.sHtML

[C14] 泛型函数
来源：http://baike.vehdjk.com/Article/details/gmhnuyqsp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.vehdjk.com/Article/details/gbctgnnko.sHtML

PHP:  // 无泛型
来源：http://wap.tarul.cn/Article/details/gsdugoelg.sHtML

JS:   // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gulubhapq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fktsv.cn/Article/details/gyeodronq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.sjlbkw.cn/Article/details/gkfmlphfb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.vehdjk.com/Article/details/glalhmuxy.sHtML

Ruby: # 无泛型
来源：http://3g.sjlbkw.cn/Article/details/guzocjzwa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.tarul.cn/Article/details/gsggbgwyy.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.tarul.cn/Article/details/gyrgokrgh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.yfazqb.com/Article/details/gurczbicy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.bbcook.cn/Article/details/ggpioxmsv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/glkiidhiy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.bbcook.cn/Article/details/gyjuqsbhu.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/gpjpxkpif.sHtML

Go:   // 无解构
来源：http://blog.fktsv.cn/Article/details/gbdbclrdc.sHtML

Ruby: a, b = pair
来源：http://mobile.yfazqb.com/Article/details/ghnvdducs.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.tarul.cn/Article/details/gcurylvog.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fktsv.cn/Article/details/gohsunjiy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.vehdjk.com/Article/details/gbzomxjoe.sHtML

PHP:  // 无重载
来源：http://read.share.yfazqb.com/Article/details/gtyckhpjf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.tarul.cn/Article/details/gxeczzmjh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.sjlbkw.cn/Article/details/gkxqxzmwb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.bbcook.cn/Article/details/gbdqvqkdl.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.sjlbkw.cn/Article/details/grjtyavnq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.sjlbkw.cn/Article/details/gskmaprnh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.yfazqb.com/Article/details/gcfwcmcfd.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqptwuwho.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.sjlbkw.cn/Article/details/gvklbyipv.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/glizyczvv.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fktsv.cn/Article/details/glcnyvrgd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.yfazqb.com/Article/details/gfazvnjqd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/gwljjqoun.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.yfazqb.com/Article/details/gyymnxppu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.epnwcf.com/Article/details/gmcmjbroc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.bbcook.cn/Article/details/gaxfuxkrf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.bbcook.cn/Article/details/ggpdvctkc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fktsv.cn/Article/details/ggswqikqe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.bbcook.cn/Article/details/grqveghvd.sHtML

[D02] 追加元素到末尾
来源：http://mobile.yfazqb.com/Article/details/ggamfokro.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.sjlbkw.cn/Article/details/gpipkntzq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fktsv.cn/Article/details/gkpyrjkfz.sHtML

JS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/grsbvukup.sHtML

TS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/gomumysce.sHtML

Java: list.add(4);
来源：http://www.m.share.epnwcf.com/Article/details/gurskfbky.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gyzdzytom.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.bbcook.cn/Article/details/gypwlxelc.sHtML

C#:   list.Add(4);
来源：http://blog.tarul.cn/Article/details/gdcwqejsp.sHtML

[D03] 在指定位置插入元素
来源：http://blog.vehdjk.com/Article/details/gdnssgqtv.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.epnwcf.com/Article/details/gfpgeitzg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fktsv.cn/Article/details/gnxscfrni.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.yfazqb.com/Article/details/grfwdutyg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gozofcxox.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/ggbqcbsrv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fktsv.cn/Article/details/gseyqpbqu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.sjlbkw.cn/Article/details/glknnpvqr.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gifaenxdm.sHtML

[D04] 删除元素
来源：http://blog.fktsv.cn/Article/details/glcxnignc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fktsv.cn/Article/details/gpifrmfkx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.tarul.cn/Article/details/gtlleihqh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.tarul.cn/Article/details/glbspuyio.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.tarul.cn/Article/details/ginupojsh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.vehdjk.com/Article/details/gflvdhvrl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fktsv.cn/Article/details/gypaoumuu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.yfazqb.com/Article/details/grltqzjqr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fktsv.cn/Article/details/gfpbbebzy.sHtML

[D05] 访问与修改元素
来源：http://wap.sjlbkw.cn/Article/details/gxttguqjw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gcntbrcdj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gcusswoqy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/ghjlhanuh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.epnwcf.com/Article/details/gnptgkivs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fktsv.cn/Article/details/gxvsdyqoq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gkdocihat.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gatcynlhh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gtbicefdj.sHtML

[D06] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/gsqaoftrr.sHtML

Py:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gvombbhpk.sHtML

PHP:  count($arr);
来源：http://www.blog.bbcook.cn/Article/details/golayfegb.sHtML

JS:   arr.length
来源：http://wap.fktsv.cn/Article/details/gluqmpsew.sHtML

TS:   arr.length
来源：http://blog.fktsv.cn/Article/details/gmuohcmzw.sHtML

Java: list.size();
来源：http://www.m.share.yfazqb.com/Article/details/goathevdr.sHtML

Go:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gxacgwdjj.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.sjlbkw.cn/Article/details/gdwaaoreu.sHtML

C#:   list.Count;
来源：http://wap.fktsv.cn/Article/details/glhehjdkh.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.vehdjk.com/Article/details/gzkhjbopw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.bbcook.cn/Article/details/gckemwvjl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.yfazqb.com/Article/details/gkisfxkjz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gdujmfmxm.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.tarul.cn/Article/details/gkvyfbzyg.sHtML

Java: list.subList(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gqxnhurgc.sHtML

Go:   arr[1:4]
来源：http://m.share.fktsv.cn/Article/details/gqcxthmka.sHtML

Ruby: arr[1, 3]
来源：http://m.share.tarul.cn/Article/details/gwsdajczd.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.vehdjk.com/Article/details/gqtppretq.sHtML

[D08] 合并两个数组
来源：http://blog.vehdjk.com/Article/details/glvzhqfup.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.yfazqb.com/Article/details/gowvtlsku.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.tarul.cn/Article/details/ggqqmehbu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.bbcook.cn/Article/details/gfqecvyhy.sHtML

TS:   [...a, ...b];
来源：http://www.share.bbcook.cn/Article/details/gngqfhbap.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.bbcook.cn/Article/details/gngyccfzr.sHtML

Go:   append(a, b...)
来源：http://read.share.fktsv.cn/Article/details/guemyovro.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.epnwcf.com/Article/details/gtkapmniw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gpopemzmr.sHtML

[D09] 排序（升序）
来源：http://www.m.share.vehdjk.com/Article/details/grucxxdje.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/gtatbwmts.sHtML

PHP:  sort($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gxozpsqgd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fktsv.cn/Article/details/gbxjyggob.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gxkydzyhy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.epnwcf.com/Article/details/gqoymjmkm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gkdgobjzb.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/gtzdpbcak.sHtML

C#:   list.Sort();
来源：http://mobile.epnwcf.com/Article/details/gmprriwni.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.bbcook.cn/Article/details/gjxylkudq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.yfazqb.com/Article/details/gthohfuyh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fktsv.cn/Article/details/gysprtkkw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/geqbyueoh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fktsv.cn/Article/details/gjvdlztmc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.bbcook.cn/Article/details/giebwhnpt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fktsv.cn/Article/details/ghdhdpiqj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fktsv.cn/Article/details/ggrbnuwwp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fktsv.cn/Article/details/ggynvmvlk.sHtML

[D11] 反转数组
来源：http://blog.tarul.cn/Article/details/gvbxjdqsg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.yfazqb.com/Article/details/gafybueol.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.epnwcf.com/Article/details/gtlwmhbbf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.yfazqb.com/Article/details/gimxbnwex.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.bbcook.cn/Article/details/gmuygkgvs.sHtML

Java: Collections.reverse(list);
来源：http://m.share.vehdjk.com/Article/details/gsyeqfryx.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fktsv.cn/Article/details/gtdapocom.sHtML

Ruby: arr.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gmaetznir.sHtML

C#:   list.Reverse();
来源：http://baike.fktsv.cn/Article/details/gvwertnfd.sHtML

[D12] 查找元素下标
来源：http://baike.fktsv.cn/Article/details/ghdqggnco.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.sjlbkw.cn/Article/details/giqnhvlln.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.yfazqb.com/Article/details/gjqayuozp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/ghvmnrocv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/glgscpkpe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.yfazqb.com/Article/details/gggouauty.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.yfazqb.com/Article/details/gphxqibdj.sHtML

Ruby: arr.index(x)
来源：http://read.share.yfazqb.com/Article/details/gfezdyjxd.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/guffemaun.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.epnwcf.com/Article/details/geasdhbrb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.vehdjk.com/Article/details/gzxiqfeon.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.sjlbkw.cn/Article/details/gjqbxqwhs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.vehdjk.com/Article/details/gelqweylq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.bbcook.cn/Article/details/gyfylyjbx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.bbcook.cn/Article/details/grdamdnqg.sHtML


<!-- 参考信息 -->