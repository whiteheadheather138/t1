代发 wailian999

C#:   x is int or double or decimal
来源：http://wap.epnwcf.com/Article/details/gytnracun.sHtML

[B14] 判断值是否在集合内
来源：http://3g.tarul.cn/Article/details/gvhhulufe.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.sjlbkw.cn/Article/details/gnnxaldnz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.sjlbkw.cn/Article/details/gmluxtoro.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gmcmyostq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fktsv.cn/Article/details/gvgnhewdq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.vehdjk.com/Article/details/gtmhfxeey.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.sjlbkw.cn/Article/details/gbfsaswxa.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gvfxfaqiy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gcwwbevxr.sHtML

[B15] 布尔运算与取反
来源：http://3g.epnwcf.com/Article/details/gofbpzyzi.sHtML

Py:   a and b or not c
来源：http://3g.bbcook.cn/Article/details/gdvehajmb.sHtML

PHP:  $a && $b || !$c
来源：http://baike.tarul.cn/Article/details/gudhuixmf.sHtML

JS:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gluncefjq.sHtML

TS:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gbkxyedyv.sHtML

Java: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gvryfxpbv.sHtML

Go:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/guyjunznx.sHtML

Ruby: a && b || !c
来源：http://3g.bbcook.cn/Article/details/gejajtsuk.sHtML

C#:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/geptndapy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.sjlbkw.cn/Article/details/gcuxgpehq.sHtML

Py:   if not data: return
来源：http://mobile.fktsv.cn/Article/details/gonpaogiw.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.yfazqb.com/Article/details/ghyjtthdl.sHtML

JS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gsvgahcst.sHtML

TS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gmonaqjau.sHtML

Java: if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gqxocoxej.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.vehdjk.com/Article/details/gkrbkbniu.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.vehdjk.com/Article/details/ghwklzyic.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/grdatasao.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ggwlpguxl.sHtML

C. 函数与作用域
来源：http://3g.epnwcf.com/Article/details/gdsvolpdf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gluaicewi.sHtML

[C01] 定义函数
来源：http://wap.yfazqb.com/Article/details/gxtktdkrm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/ghrclulhx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gyqlbqxgl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gvtnqtuwc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gsvirgnhg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gdjerdxnt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fktsv.cn/Article/details/gmednmyie.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.yfazqb.com/Article/details/gibyvygho.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/grrhhawvb.sHtML

[C02] 默认参数
来源：http://www.share.bbcook.cn/Article/details/ghoccdaqx.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.sjlbkw.cn/Article/details/geemskkaf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fktsv.cn/Article/details/gvuydnfcs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.yfazqb.com/Article/details/gtgguisew.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gzwrgfwoi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.tarul.cn/Article/details/ghjmromrp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.tarul.cn/Article/details/gfvvpnknw.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fktsv.cn/Article/details/gztlggyzp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.sjlbkw.cn/Article/details/gbopfkpdk.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/gfvuxqsut.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fktsv.cn/Article/details/gbdhcosug.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.tarul.cn/Article/details/gzvmovoej.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/grqarxshd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gbuqsabwi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.tarul.cn/Article/details/gtjovvbxw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.yfazqb.com/Article/details/geqvvxymc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gmynmimrl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.yfazqb.com/Article/details/gprmegqtj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.vehdjk.com/Article/details/gnvjoirch.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.bbcook.cn/Article/details/geblfszke.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.sjlbkw.cn/Article/details/gasctblaj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gaylnqqkk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.vehdjk.com/Article/details/gwgxajjdw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.sjlbkw.cn/Article/details/gnxyhyavs.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.tarul.cn/Article/details/gjjbvnlke.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gltaxqntr.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gzxniaghu.sHtML

[C05] 返回多个值
来源：http://3g.tarul.cn/Article/details/gtejslmht.sHtML

Py:   return a, b
来源：http://baike.sjlbkw.cn/Article/details/gxttthhkp.sHtML

PHP:  return [$a, $b];
来源：http://wap.epnwcf.com/Article/details/gjrkcrcre.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.tarul.cn/Article/details/goulatujc.sHtML

TS:   return { a, b };
来源：http://read.share.vehdjk.com/Article/details/glpqwmscv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.sjlbkw.cn/Article/details/gvtbgucsq.sHtML

Go:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/ghgcukrnl.sHtML

Ruby: return a, b
来源：http://blog.yfazqb.com/Article/details/gkvkvgpjt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.sjlbkw.cn/Article/details/gjtuplamf.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.yfazqb.com/Article/details/gfkuvsdep.sHtML

Py:   square = lambda x: x * x
来源：http://baike.yfazqb.com/Article/details/gcpkrlkut.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.yfazqb.com/Article/details/guurllpwn.sHtML

JS:   const square = x => x * x;
来源：http://read.share.vehdjk.com/Article/details/gsywkkemw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.tarul.cn/Article/details/gsiwzeazc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhreweqa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.bbcook.cn/Article/details/gjagldakl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.sjlbkw.cn/Article/details/gwhfbastk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/ghmldsnqw.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyoyfnsf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.bbcook.cn/Article/details/gwairjqnu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.vehdjk.com/Article/details/gbybivwwp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.vehdjk.com/Article/details/gzdfmmrfd.sHtML

TS:   arr.map(String)
来源：http://www.blog.tarul.cn/Article/details/gahohisda.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.sjlbkw.cn/Article/details/gjnfngbco.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.tarul.cn/Article/details/gszydahkk.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.vehdjk.com/Article/details/gehexvmlm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.epnwcf.com/Article/details/gmrywvdqa.sHtML

[C08] 闭包
来源：http://mobile.epnwcf.com/Article/details/gjdhcrtpj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.sjlbkw.cn/Article/details/gkzppxhac.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.epnwcf.com/Article/details/gpzbbltib.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/gzpcuknuf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gjvpcmplb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.yfazqb.com/Article/details/gjkgbkxge.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.bbcook.cn/Article/details/gmtucvvqu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.tarul.cn/Article/details/gcwxxoysj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/glziogyhf.sHtML

[C09] 递归
来源：http://www.share.epnwcf.com/Article/details/grmmsbpkp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gwfutgsvo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.epnwcf.com/Article/details/grcuqjlsx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/ggltphlpd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gqhgczvli.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.vehdjk.com/Article/details/goroimstv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.vehdjk.com/Article/details/gyuxyasme.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.bbcook.cn/Article/details/gsnswemih.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.tarul.cn/Article/details/gcrpuujut.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/gkaputflz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.epnwcf.com/Article/details/grozgwrfe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.sjlbkw.cn/Article/details/geabeshyq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.yfazqb.com/Article/details/grxhotrrs.sHtML

TS:   同 JS
来源：http://baike.fktsv.cn/Article/details/gunrhctxw.sHtML

Java: 方法内为块级作用域
来源：http://3g.fktsv.cn/Article/details/gaqoiztfw.sHtML

Go:   花括号块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gvxygudql.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.tarul.cn/Article/details/gwdvbsbge.sHtML

C#:   块级作用域
来源：http://3g.epnwcf.com/Article/details/gbtdhqoxq.sHtML

[C11] 模块导入与导出
来源：http://blog.fktsv.cn/Article/details/goajyrirk.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gauhbmutz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.tarul.cn/Article/details/gjbuxpcow.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.tarul.cn/Article/details/gbpuuhevl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.yfazqb.com/Article/details/gxywhsfbv.sHtML

Java: import java.util.List;
来源：http://blog.bbcook.cn/Article/details/gyqhwzgqp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.vehdjk.com/Article/details/gpebqurlq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.sjlbkw.cn/Article/details/gyqmwypne.sHtML

C#:   using System.Text;
来源：http://www.blog.epnwcf.com/Article/details/gwczjtdrq.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.epnwcf.com/Article/details/gmojlcuan.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.vehdjk.com/Article/details/gfrfhdppf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.sjlbkw.cn/Article/details/gfjyaejse.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/glczabvjv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gwhsspxpa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.yfazqb.com/Article/details/geocoxaie.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.bbcook.cn/Article/details/gakctvbvn.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.tarul.cn/Article/details/garmhktwe.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.vehdjk.com/Article/details/gmualbtmb.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.sjlbkw.cn/Article/details/gzhyfztqu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fktsv.cn/Article/details/gncoovhnj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/gizpizowq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.bbcook.cn/Article/details/gfvoscfiq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gxvqegnqo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gqsufpafg.sHtML

Go:   func add(a, b int) int
来源：http://www.share.tarul.cn/Article/details/glbsclphf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.vehdjk.com/Article/details/glvpgzymp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.tarul.cn/Article/details/gqphotmmc.sHtML

[C14] 泛型函数
来源：http://3g.bbcook.cn/Article/details/ghnjwcher.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.sjlbkw.cn/Article/details/gberhuvjl.sHtML

PHP:  // 无泛型
来源：http://blog.bbcook.cn/Article/details/gzlxgiumd.sHtML

JS:   // 无泛型
来源：http://read.share.yfazqb.com/Article/details/gcevlaacs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.tarul.cn/Article/details/gdvwnbmiu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/gnqzwbiyk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.yfazqb.com/Article/details/gnufjuqmj.sHtML

Ruby: # 无泛型
来源：http://mobile.yfazqb.com/Article/details/gwyozmbdx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.yfazqb.com/Article/details/gfhikmfyb.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.tarul.cn/Article/details/gqrgwjmbz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.tarul.cn/Article/details/gdzzecyqp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.vehdjk.com/Article/details/gbyattklb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/gnrqhkrdi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.yfazqb.com/Article/details/guqtdzncz.sHtML

Java: // 无解构
来源：http://baike.vehdjk.com/Article/details/gutpahvxd.sHtML

Go:   // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gpzhdpaax.sHtML

Ruby: a, b = pair
来源：http://mobile.vehdjk.com/Article/details/gwcggoeeu.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/gyonwoosi.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.yfazqb.com/Article/details/gqbwwdgwf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.epnwcf.com/Article/details/gzcapxzho.sHtML

PHP:  // 无重载
来源：http://blog.epnwcf.com/Article/details/gbtltilfl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.epnwcf.com/Article/details/gwnwrzevt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.epnwcf.com/Article/details/gqerrhifi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.yfazqb.com/Article/details/gegdmqnuk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.bbcook.cn/Article/details/gcogwsoit.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.vehdjk.com/Article/details/gfjbuqvyi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.vehdjk.com/Article/details/ghalhkdge.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gilxbnfaj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnzwahzu.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/grlheaoia.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fktsv.cn/Article/details/gipscqexu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.yfazqb.com/Article/details/grotcgnxw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.tarul.cn/Article/details/gekadjzjw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.sjlbkw.cn/Article/details/gzuaiybmi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.epnwcf.com/Article/details/gkuboajju.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.sjlbkw.cn/Article/details/gnqouqomh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/giepfjnsn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.bbcook.cn/Article/details/guzowojjw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.yfazqb.com/Article/details/gezkulyiw.sHtML

[D02] 追加元素到末尾
来源：http://3g.fktsv.cn/Article/details/gpjlezagl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.epnwcf.com/Article/details/grhldldae.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.yfazqb.com/Article/details/grxixrqsg.sHtML

JS:   arr.push(4);
来源：http://www.m.share.bbcook.cn/Article/details/gcdbihguq.sHtML

TS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gbftjfiio.sHtML

Java: list.add(4);
来源：http://baike.yfazqb.com/Article/details/gghkozcah.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.sjlbkw.cn/Article/details/grqkczkpz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.vehdjk.com/Article/details/gjbeupmwt.sHtML

C#:   list.Add(4);
来源：http://www.share.bbcook.cn/Article/details/gbgndbpmi.sHtML

[D03] 在指定位置插入元素
来源：http://blog.tarul.cn/Article/details/gdgqbmdih.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.bbcook.cn/Article/details/gtnvmmeki.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.bbcook.cn/Article/details/gwvhnkldz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fktsv.cn/Article/details/gwwfpqkeq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.vehdjk.com/Article/details/gylqzmrsv.sHtML

Java: list.add(0, 0);
来源：http://baike.fktsv.cn/Article/details/gwbbbvhbk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.sjlbkw.cn/Article/details/gpllbsjbj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.vehdjk.com/Article/details/gfseieazv.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.epnwcf.com/Article/details/gnrpyuduc.sHtML

[D04] 删除元素
来源：http://www.m.share.tarul.cn/Article/details/gvdaexajx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.tarul.cn/Article/details/gtcjgrpzl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.bbcook.cn/Article/details/gzwiyvpss.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.tarul.cn/Article/details/gnxopusho.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.bbcook.cn/Article/details/gponmcago.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.tarul.cn/Article/details/gcyabmgas.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.tarul.cn/Article/details/gygysmonr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.epnwcf.com/Article/details/ghwsygpdj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.yfazqb.com/Article/details/gipjvxalr.sHtML

[D05] 访问与修改元素
来源：http://www.blog.vehdjk.com/Article/details/gukhiuows.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gxzpsmzbc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnogmgfhs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gwazvnojv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.epnwcf.com/Article/details/gtnjxlrlw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.yfazqb.com/Article/details/gaxzwoqih.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gkbbbqngq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/glbeuvxtc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/glianndpn.sHtML

[D06] 数组长度
来源：http://mobile.epnwcf.com/Article/details/gbqdscgdo.sHtML

Py:   len(arr)
来源：http://read.share.yfazqb.com/Article/details/ghuatelxq.sHtML

PHP:  count($arr);
来源：http://baike.tarul.cn/Article/details/gggwvbwww.sHtML

JS:   arr.length
来源：http://www.m.share.sjlbkw.cn/Article/details/guwjwooud.sHtML

TS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/gusdinnjo.sHtML

Java: list.size();
来源：http://baike.fktsv.cn/Article/details/guughjprs.sHtML

Go:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/gijcuewhk.sHtML

Ruby: arr.length; arr.size
来源：http://baike.epnwcf.com/Article/details/gryicxmox.sHtML

C#:   list.Count;
来源：http://m.share.epnwcf.com/Article/details/gjdyhquvv.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fktsv.cn/Article/details/ghmwazcwj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.tarul.cn/Article/details/glybjkaxp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fktsv.cn/Article/details/gfqnvjsmx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gpuurierf.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gbhohcnax.sHtML

Java: list.subList(1, 4);
来源：http://blog.vehdjk.com/Article/details/gutwnbycm.sHtML

Go:   arr[1:4]
来源：http://mobile.epnwcf.com/Article/details/glbcryxdb.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fktsv.cn/Article/details/gzmwrekdt.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.yfazqb.com/Article/details/gsbgnnhar.sHtML

[D08] 合并两个数组
来源：http://www.share.vehdjk.com/Article/details/gkdaidaqg.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.bbcook.cn/Article/details/gdnceiisk.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.bbcook.cn/Article/details/ggxpbkxja.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.epnwcf.com/Article/details/glmnqxfmp.sHtML

TS:   [...a, ...b];
来源：http://mobile.tarul.cn/Article/details/govxwjuph.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fktsv.cn/Article/details/ghapkioey.sHtML

Go:   append(a, b...)
来源：http://wap.sjlbkw.cn/Article/details/gbgfphtje.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.yfazqb.com/Article/details/gxwcceahs.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fktsv.cn/Article/details/ggffpxiqa.sHtML

[D09] 排序（升序）
来源：http://wap.yfazqb.com/Article/details/ghvmhbhdj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/gzfochpfu.sHtML

PHP:  sort($arr);
来源：http://baike.sjlbkw.cn/Article/details/gvezxplmk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.yfazqb.com/Article/details/gnbjrfhsn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.sjlbkw.cn/Article/details/gvtozwfoa.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.sjlbkw.cn/Article/details/gwotysiqh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gaorreaep.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gfmulqour.sHtML

C#:   list.Sort();
来源：http://m.share.vehdjk.com/Article/details/gevpvjjub.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.yfazqb.com/Article/details/glwvvxbax.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.vehdjk.com/Article/details/gtphvspot.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/gdessccyj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gubshpzfd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.bbcook.cn/Article/details/ghyntewdo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fktsv.cn/Article/details/gktrykmse.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gzbjwcnno.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.yfazqb.com/Article/details/gwqmblxxz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.vehdjk.com/Article/details/glyeypfju.sHtML

[D11] 反转数组
来源：http://mobile.sjlbkw.cn/Article/details/gbchtrbbt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.epnwcf.com/Article/details/gdvjnwcrm.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.bbcook.cn/Article/details/gmlwdkpmo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.epnwcf.com/Article/details/gtzxmrtmx.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fktsv.cn/Article/details/gagxbaouk.sHtML

Java: Collections.reverse(list);
来源：http://wap.fktsv.cn/Article/details/gswsprpzt.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.epnwcf.com/Article/details/gtcpejzdg.sHtML

Ruby: arr.reverse
来源：http://read.share.tarul.cn/Article/details/glyxkgmoa.sHtML

C#:   list.Reverse();
来源：http://mobile.yfazqb.com/Article/details/globzszvz.sHtML

[D12] 查找元素下标
来源：http://mobile.vehdjk.com/Article/details/gsvwjrgxi.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.sjlbkw.cn/Article/details/ghczjodtd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fktsv.cn/Article/details/gckpsigoq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/gslkqfkcq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.tarul.cn/Article/details/gqmivohkt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.vehdjk.com/Article/details/gguwnpuzp.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.epnwcf.com/Article/details/gmtrwcueh.sHtML

Ruby: arr.index(x)
来源：http://blog.epnwcf.com/Article/details/gscadglxk.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.yfazqb.com/Article/details/gqoihnlwp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fktsv.cn/Article/details/ggprfghhk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.bbcook.cn/Article/details/gjhneoeyf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.bbcook.cn/Article/details/gvdzicwyj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gxpzqhhfv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/geuzaxmxf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fktsv.cn/Article/details/gtnaeunqq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.tarul.cn/Article/details/gxbimgwbb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fktsv.cn/Article/details/galqeayku.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.bbcook.cn/Article/details/gufkjjoth.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.epnwcf.com/Article/details/gclmewihe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.bbcook.cn/Article/details/geijeltdw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.tarul.cn/Article/details/gwtbftcui.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaahdyspz.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.tarul.cn/Article/details/gjnblgwwv.sHtML


<!-- 参考信息 -->