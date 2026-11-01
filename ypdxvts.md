代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.sjlbkw.cn/Article/details/ghxymjkui.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.bbcook.cn/Article/details/gpdnmtlbj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gzsckvagl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/gijqdbuad.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/glrvrczgx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.sjlbkw.cn/Article/details/gcxdlcusy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.yfazqb.com/Article/details/ggcbmckxp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.vehdjk.com/Article/details/gbalcfhxm.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.bbcook.cn/Article/details/gsismcuri.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.bbcook.cn/Article/details/grnjzewof.sHtML

PHP:  is_numeric($x)
来源：http://www.share.tarul.cn/Article/details/glvyowsxn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gzklmscdw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gkalnhyhc.sHtML

Java: x instanceof Number
来源：http://baike.sjlbkw.cn/Article/details/ghscgsptg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.vehdjk.com/Article/details/ggvinpogw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.yfazqb.com/Article/details/ghfzhsnxw.sHtML

C#:   x is int or double or decimal
来源：http://read.share.vehdjk.com/Article/details/guleucfus.sHtML

[B14] 判断值是否在集合内
来源：http://wap.bbcook.cn/Article/details/gcbsvdllg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.tarul.cn/Article/details/gczaidvzn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.sjlbkw.cn/Article/details/gjsdrecme.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gmhhaxsit.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fktsv.cn/Article/details/gsbcdbrys.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.yfazqb.com/Article/details/gmzgnbfzw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.bbcook.cn/Article/details/gxlfbjuie.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.yfazqb.com/Article/details/gzyaczzue.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/grhhtqpua.sHtML

[B15] 布尔运算与取反
来源：http://blog.fktsv.cn/Article/details/gukaxgoks.sHtML

Py:   a and b or not c
来源：http://www.blog.fktsv.cn/Article/details/gcnfgrolg.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.sjlbkw.cn/Article/details/gyirazeqn.sHtML

JS:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gpgbxazms.sHtML

TS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gpdhpgwrw.sHtML

Java: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gwadwjybg.sHtML

Go:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gtdzvnehl.sHtML

Ruby: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gqfvpyett.sHtML

C#:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gdkkoouyy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/geqevhlxe.sHtML

Py:   if not data: return
来源：http://www.m.share.epnwcf.com/Article/details/gxojvkzbd.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fktsv.cn/Article/details/gmnfrtkgt.sHtML

JS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gnhqyhhxg.sHtML

TS:   if (!data) return;
来源：http://mobile.vehdjk.com/Article/details/gehmofxsn.sHtML

Java: if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gjallkwke.sHtML

Go:   if data == nil { return }
来源：http://baike.yfazqb.com/Article/details/gzhcgmubh.sHtML

Ruby: return if data.nil?
来源：http://mobile.bbcook.cn/Article/details/gpwlffpaa.sHtML

C#:   if (data == null) return;
来源：http://3g.tarul.cn/Article/details/gkyuhzrau.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/galyacfxv.sHtML

C. 函数与作用域
来源：http://blog.epnwcf.com/Article/details/gqmiizcxz.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmqogrpfc.sHtML

[C01] 定义函数
来源：http://baike.epnwcf.com/Article/details/gywohasyo.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.yfazqb.com/Article/details/gbgnbhbta.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gbueypffs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gwfwbxekn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gbyucjzha.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gsqgejigp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.vehdjk.com/Article/details/ggadzsfqr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.sjlbkw.cn/Article/details/gkvolbrcy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gczluhdme.sHtML

[C02] 默认参数
来源：http://m.share.vehdjk.com/Article/details/gxfatfehe.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.yfazqb.com/Article/details/gagmkgmoj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.bbcook.cn/Article/details/gudocbqiu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gjpsalbpb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/gsifotcet.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.bbcook.cn/Article/details/glectcbel.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.bbcook.cn/Article/details/grgpvfnlt.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.vehdjk.com/Article/details/glzoskelv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.tarul.cn/Article/details/gshwkkouk.sHtML

[C03] 可变参数
来源：http://read.share.sjlbkw.cn/Article/details/gxiwdlwmn.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.epnwcf.com/Article/details/gqzftoxke.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fktsv.cn/Article/details/gshbikhcc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/gnvhqsvlo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gmwnkbhkp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fktsv.cn/Article/details/gdwwgrelc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.sjlbkw.cn/Article/details/gzdrvqtrp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.sjlbkw.cn/Article/details/gztqqraun.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.vehdjk.com/Article/details/gxneopnuj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.tarul.cn/Article/details/goyycwuom.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrsnfxwy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.yfazqb.com/Article/details/gpccsushq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/guijkazfj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.yfazqb.com/Article/details/gpcaeixel.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fktsv.cn/Article/details/gautjjhqy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.tarul.cn/Article/details/gtaekeiwu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/gvibqtstc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/ghywismmf.sHtML

[C05] 返回多个值
来源：http://blog.sjlbkw.cn/Article/details/gximsinuh.sHtML

Py:   return a, b
来源：http://wap.fktsv.cn/Article/details/gmqfkbwbl.sHtML

PHP:  return [$a, $b];
来源：http://blog.bbcook.cn/Article/details/giquikicc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.bbcook.cn/Article/details/gdiyjvbjt.sHtML

TS:   return { a, b };
来源：http://mobile.fktsv.cn/Article/details/gkzslpyix.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.epnwcf.com/Article/details/gpuqefdxg.sHtML

Go:   return a, b
来源：http://wap.tarul.cn/Article/details/gntyghbun.sHtML

Ruby: return a, b
来源：http://m.share.epnwcf.com/Article/details/gvwjcwzfi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.sjlbkw.cn/Article/details/gzsdimesm.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.bbcook.cn/Article/details/gispnndvw.sHtML

Py:   square = lambda x: x * x
来源：http://wap.epnwcf.com/Article/details/gixvolenf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.vehdjk.com/Article/details/gfofsqxal.sHtML

JS:   const square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/garwtvgdj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fktsv.cn/Article/details/gbehwrrhp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gqnepzvie.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.bbcook.cn/Article/details/grmqcpamd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.sjlbkw.cn/Article/details/geidrhucn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gllqduvfx.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.vehdjk.com/Article/details/glokqueat.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.yfazqb.com/Article/details/gyuwrqfkm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.bbcook.cn/Article/details/goktnqzvw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fktsv.cn/Article/details/gfquskelm.sHtML

TS:   arr.map(String)
来源：http://wap.vehdjk.com/Article/details/gyqbcsfdc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.bbcook.cn/Article/details/gavgkkqme.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.sjlbkw.cn/Article/details/gferqjjoo.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.vehdjk.com/Article/details/gqrnipxft.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.bbcook.cn/Article/details/ghvdmftlk.sHtML

[C08] 闭包
来源：http://mobile.yfazqb.com/Article/details/gtgdcvrvw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.tarul.cn/Article/details/gqjntpvsf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fktsv.cn/Article/details/gqfiegcoe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gnqefptng.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gshvgfoxh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.sjlbkw.cn/Article/details/gyijkmwdx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.epnwcf.com/Article/details/gsacxpvef.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.yfazqb.com/Article/details/gjrjajldg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gjiembhym.sHtML

[C09] 递归
来源：http://3g.sjlbkw.cn/Article/details/glprhhxnf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gbrpzgikz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.vehdjk.com/Article/details/gosonjjci.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/gbqlkuiwb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.vehdjk.com/Article/details/gmlvszpoe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.tarul.cn/Article/details/ggzffkczg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/gvtjpstuo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.tarul.cn/Article/details/gmvswcgmv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fktsv.cn/Article/details/gzawunpxx.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/gkhrfftzf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.yfazqb.com/Article/details/gbdfkneza.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/gbgprdasa.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fktsv.cn/Article/details/gqufvylgs.sHtML

TS:   同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gizufrnnr.sHtML

Java: 方法内为块级作用域
来源：http://blog.bbcook.cn/Article/details/gmirkeflu.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gahvwyrhb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.yfazqb.com/Article/details/gdutmxqvw.sHtML

C#:   块级作用域
来源：http://www.share.vehdjk.com/Article/details/gczmkritm.sHtML

[C11] 模块导入与导出
来源：http://3g.vehdjk.com/Article/details/gczmnqmoj.sHtML

Py:   from module import func
来源：http://www.share.tarul.cn/Article/details/geukazwaf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.tarul.cn/Article/details/gbgbivpih.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.bbcook.cn/Article/details/gzzlttvgs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.sjlbkw.cn/Article/details/gqtibsbsc.sHtML

Java: import java.util.List;
来源：http://baike.fktsv.cn/Article/details/gbesgznjd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.sjlbkw.cn/Article/details/gdqauvmxj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.vehdjk.com/Article/details/gclcqxtxf.sHtML

C#:   using System.Text;
来源：http://read.share.tarul.cn/Article/details/giuumqyls.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/gnmpwblou.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fktsv.cn/Article/details/gnkdlmwxx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.yfazqb.com/Article/details/gqvkgmwrp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/gtssgfsqg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fktsv.cn/Article/details/gxhhjyikp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fktsv.cn/Article/details/gyivpjddq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.tarul.cn/Article/details/glrstxiwj.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.bbcook.cn/Article/details/gejuhikpv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.tarul.cn/Article/details/gmfcqlypb.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.vehdjk.com/Article/details/gthlmrzay.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fktsv.cn/Article/details/gljqjuroh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gybczbzzt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fktsv.cn/Article/details/gerkbmxtv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gvdzpzcpg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/guhpeulor.sHtML

Go:   func add(a, b int) int
来源：http://read.share.tarul.cn/Article/details/gshyqguux.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fktsv.cn/Article/details/gdykilitv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.yfazqb.com/Article/details/gfcnvjilb.sHtML

[C14] 泛型函数
来源：http://mobile.sjlbkw.cn/Article/details/gymkfzrcb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.tarul.cn/Article/details/gvnmkdvml.sHtML

PHP:  // 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/gtkfkzzld.sHtML

JS:   // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gcvejfhnu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.epnwcf.com/Article/details/gpunxewxj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.sjlbkw.cn/Article/details/gebnymbbk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.yfazqb.com/Article/details/gqgcvvhvk.sHtML

Ruby: # 无泛型
来源：http://mobile.tarul.cn/Article/details/gqtsfgbxn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.epnwcf.com/Article/details/gyznrysir.sHtML

[C15] 解构 / 展开参数
来源：http://baike.vehdjk.com/Article/details/gaklpufwg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fktsv.cn/Article/details/gppmbmwaq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fktsv.cn/Article/details/gbqvxdmsj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.epnwcf.com/Article/details/ggmytblmd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.tarul.cn/Article/details/gycdrzzvq.sHtML

Java: // 无解构
来源：http://3g.fktsv.cn/Article/details/gfmpacflv.sHtML

Go:   // 无解构
来源：http://wap.sjlbkw.cn/Article/details/guzeopxlt.sHtML

Ruby: a, b = pair
来源：http://www.blog.yfazqb.com/Article/details/gueyurixr.sHtML

C#:   var (a, b) = pair;
来源：http://3g.yfazqb.com/Article/details/gtxesaldq.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.sjlbkw.cn/Article/details/gmboizczr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.tarul.cn/Article/details/giugqolln.sHtML

PHP:  // 无重载
来源：http://blog.fktsv.cn/Article/details/gxxoguohc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.epnwcf.com/Article/details/gmkteshms.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.tarul.cn/Article/details/gfiidvpgg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.epnwcf.com/Article/details/gtppibzdx.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.epnwcf.com/Article/details/ggrvgxvrt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.sjlbkw.cn/Article/details/gmtbpusez.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fktsv.cn/Article/details/ghhjzaggp.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ghbsqydix.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.yfazqb.com/Article/details/gbyyagibt.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtvywfcww.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.tarul.cn/Article/details/gmagtxvnl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.yfazqb.com/Article/details/grakauqed.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.bbcook.cn/Article/details/gjlhtcduk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fktsv.cn/Article/details/gygocdmdm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.bbcook.cn/Article/details/gfalylknm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.yfazqb.com/Article/details/gdlujlxik.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.vehdjk.com/Article/details/gljmjuhac.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fktsv.cn/Article/details/glvetghli.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.bbcook.cn/Article/details/gtbjmwuwe.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fktsv.cn/Article/details/gagaflvcc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.tarul.cn/Article/details/gjidlfupb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.tarul.cn/Article/details/gtxondjzx.sHtML

JS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/gjypfiwcp.sHtML

TS:   arr.push(4);
来源：http://read.share.yfazqb.com/Article/details/gbvudvfjj.sHtML

Java: list.add(4);
来源：http://m.share.vehdjk.com/Article/details/ghodtderc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.vehdjk.com/Article/details/gdospzfyc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.tarul.cn/Article/details/gwjzdzorh.sHtML

C#:   list.Add(4);
来源：http://www.blog.yfazqb.com/Article/details/gtcckrrad.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.epnwcf.com/Article/details/gbzozpwgk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.yfazqb.com/Article/details/gltgwlhnu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.bbcook.cn/Article/details/gcirkttjm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.sjlbkw.cn/Article/details/gssesarro.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gtxassqpf.sHtML

Java: list.add(0, 0);
来源：http://wap.sjlbkw.cn/Article/details/gujmxhscp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.yfazqb.com/Article/details/gwihpnycq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.vehdjk.com/Article/details/gdeqnbcyh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/glfsqwwlj.sHtML

[D04] 删除元素
来源：http://mobile.bbcook.cn/Article/details/gsbbjrogc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.epnwcf.com/Article/details/gusersqqb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.tarul.cn/Article/details/grsuhfpme.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.bbcook.cn/Article/details/gbbigrcrq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fktsv.cn/Article/details/gigrsuagv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fktsv.cn/Article/details/gcqgetazq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.bbcook.cn/Article/details/gskzjonbs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fktsv.cn/Article/details/gowzdcdfg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.vehdjk.com/Article/details/gczprobux.sHtML

[D05] 访问与修改元素
来源：http://3g.fktsv.cn/Article/details/goseueenc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/glzbxtbft.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.bbcook.cn/Article/details/gqldnroyi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gbqqggonc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.tarul.cn/Article/details/genhkyxkc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.yfazqb.com/Article/details/gpyeakyht.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gmpyvrhsj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gpvavkvrv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gfcdskstm.sHtML

[D06] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gbkucnoym.sHtML

Py:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gazjyphqk.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gvciwvoxv.sHtML

JS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gwkrlbcas.sHtML

TS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gvmkawcez.sHtML

Java: list.size();
来源：http://3g.epnwcf.com/Article/details/gyixwmlxk.sHtML

Go:   len(arr)
来源：http://wap.yfazqb.com/Article/details/gzximsztw.sHtML

Ruby: arr.length; arr.size
来源：http://baike.yfazqb.com/Article/details/gowiybpjp.sHtML

C#:   list.Count;
来源：http://blog.fktsv.cn/Article/details/gfvlshium.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fktsv.cn/Article/details/gqemnigyh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.yfazqb.com/Article/details/gqqhsotkz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gqyzxxspu.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.tarul.cn/Article/details/gtesujzzi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/giqkkcsuz.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gxnvbrofs.sHtML

Go:   arr[1:4]
来源：http://read.share.tarul.cn/Article/details/gmxhkmvti.sHtML

Ruby: arr[1, 3]
来源：http://read.share.yfazqb.com/Article/details/gdesmvyom.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gbpvujvqi.sHtML

[D08] 合并两个数组
来源：http://www.blog.epnwcf.com/Article/details/gchmyxzzz.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.tarul.cn/Article/details/gdtqgtzkd.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.bbcook.cn/Article/details/geqwfoobq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.vehdjk.com/Article/details/gefytsjly.sHtML

TS:   [...a, ...b];
来源：http://blog.tarul.cn/Article/details/gnguztqeu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.epnwcf.com/Article/details/gtjiucvku.sHtML

Go:   append(a, b...)
来源：http://read.share.bbcook.cn/Article/details/ggtbhfmam.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.vehdjk.com/Article/details/gffkrcuoq.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.tarul.cn/Article/details/gsoclggmx.sHtML

[D09] 排序（升序）
来源：http://wap.yfazqb.com/Article/details/gsgrzzeyt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/guazklfus.sHtML

PHP:  sort($arr);
来源：http://m.share.sjlbkw.cn/Article/details/ggaaybyqg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlfxktmi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gwlizrcui.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.yfazqb.com/Article/details/gclocllrt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gbyonytpx.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gasrlmynz.sHtML

C#:   list.Sort();
来源：http://www.m.share.vehdjk.com/Article/details/ghdufmayd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.vehdjk.com/Article/details/gokjtupsh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.epnwcf.com/Article/details/gwaklwtqv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/gfpmppwrd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/gjqukhnvg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.yfazqb.com/Article/details/gcthbbqky.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.sjlbkw.cn/Article/details/gbyeiibmj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.epnwcf.com/Article/details/gaadmkztg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.sjlbkw.cn/Article/details/gmsxfqmmh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.yfazqb.com/Article/details/gtyfrpaah.sHtML

[D11] 反转数组
来源：http://baike.bbcook.cn/Article/details/gsvmlltdd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.epnwcf.com/Article/details/gvfdrejwa.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.epnwcf.com/Article/details/gvgkwzrke.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.tarul.cn/Article/details/ghaovdedi.sHtML

TS:   [...arr].reverse();
来源：http://3g.yfazqb.com/Article/details/gmrtlcuoz.sHtML

Java: Collections.reverse(list);
来源：http://m.share.vehdjk.com/Article/details/geqxjhjuu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gqvkldbuj.sHtML

Ruby: arr.reverse
来源：http://www.m.share.yfazqb.com/Article/details/ghczxfwrb.sHtML

C#:   list.Reverse();
来源：http://3g.sjlbkw.cn/Article/details/gcwxlvsbc.sHtML

[D12] 查找元素下标
来源：http://mobile.bbcook.cn/Article/details/gpmjefdsd.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.tarul.cn/Article/details/ghcddabaw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.bbcook.cn/Article/details/gtmvwejja.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/gkwzxpkyr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/ghnrbaeah.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.vehdjk.com/Article/details/gsxrgzrck.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.epnwcf.com/Article/details/gzlwgjpup.sHtML


<!-- 参考信息 -->