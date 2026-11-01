代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.epnwcf.com/Article/details/gpmiiolve.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fktsv.cn/Article/details/gawstehkq.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.tarul.cn/Article/details/gxvhrhlix.sHtML

Py:   a and b or not c
来源：http://www.blog.tarul.cn/Article/details/gtjccnoew.sHtML

PHP:  $a && $b || !$c
来源：http://wap.bbcook.cn/Article/details/grfnmiupu.sHtML

JS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/ggsbmqkod.sHtML

TS:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/ghfpppuli.sHtML

Java: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfgmirma.sHtML

Go:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gclwqtdtd.sHtML

Ruby: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/giezbsvqg.sHtML

C#:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gyvmfqqin.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.yfazqb.com/Article/details/gszrfindo.sHtML

Py:   if not data: return
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyngwxni.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/gowkcinek.sHtML

JS:   if (!data) return;
来源：http://3g.sjlbkw.cn/Article/details/gfhmmcuyy.sHtML

TS:   if (!data) return;
来源：http://wap.epnwcf.com/Article/details/gslnedxbl.sHtML

Java: if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/gyuztrnas.sHtML

Go:   if data == nil { return }
来源：http://3g.vehdjk.com/Article/details/gdbdtbgpm.sHtML

Ruby: return if data.nil?
来源：http://3g.vehdjk.com/Article/details/gglbsryak.sHtML

C#:   if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/gebihljzx.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gmrwgukau.sHtML

C. 函数与作用域
来源：http://wap.fktsv.cn/Article/details/gtuihqvmm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/geayhexhe.sHtML

[C01] 定义函数
来源：http://wap.yfazqb.com/Article/details/gmaokreoo.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.sjlbkw.cn/Article/details/ghzxfjgvs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gcwuwrmhj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gudxvkbsc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gfhogmeas.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gzlnfccue.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gxrizwesz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.bbcook.cn/Article/details/gltwdlkmi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gqjwgxlxe.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gfvclgpoj.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.sjlbkw.cn/Article/details/gortdihzk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fktsv.cn/Article/details/ggujupckw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/gopprvhaz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.tarul.cn/Article/details/ggqmbwdci.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.vehdjk.com/Article/details/griudrrhv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.bbcook.cn/Article/details/ggenofykj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.bbcook.cn/Article/details/gstnucnup.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.epnwcf.com/Article/details/gxxusbkeb.sHtML

[C03] 可变参数
来源：http://3g.sjlbkw.cn/Article/details/gwckryiie.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.vehdjk.com/Article/details/gnpdzkwfr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.bbcook.cn/Article/details/gczokekth.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.yfazqb.com/Article/details/gquadsfxc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gnpfdzlov.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.yfazqb.com/Article/details/gyzrbsdhf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.tarul.cn/Article/details/gqjicviah.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.epnwcf.com/Article/details/gwzcgsmct.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.tarul.cn/Article/details/gesbrkvll.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.sjlbkw.cn/Article/details/gjijuarmg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.epnwcf.com/Article/details/gelmumbts.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.epnwcf.com/Article/details/gbbhsygoh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/ghtmodabj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.vehdjk.com/Article/details/gonshztih.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.tarul.cn/Article/details/giemfmikm.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.bbcook.cn/Article/details/gcaorepda.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gwgvlfcxk.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gckfbmhad.sHtML

[C05] 返回多个值
来源：http://www.m.share.epnwcf.com/Article/details/grxvulamw.sHtML

Py:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gjeotdwcl.sHtML

PHP:  return [$a, $b];
来源：http://m.share.epnwcf.com/Article/details/gznydzakk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.bbcook.cn/Article/details/gzhqumpxh.sHtML

TS:   return { a, b };
来源：http://wap.fktsv.cn/Article/details/gmwodnlkf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.sjlbkw.cn/Article/details/gcetbccmp.sHtML

Go:   return a, b
来源：http://baike.sjlbkw.cn/Article/details/gksnzslrw.sHtML

Ruby: return a, b
来源：http://read.share.fktsv.cn/Article/details/gtdbdmpcw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.tarul.cn/Article/details/gxvipfodi.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.sjlbkw.cn/Article/details/gpqvaehqo.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.tarul.cn/Article/details/gwignefdx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gywkanxjo.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gcgujspjd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.bbcook.cn/Article/details/grnssselx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.epnwcf.com/Article/details/giwxotjpv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.bbcook.cn/Article/details/guhfqinvi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.sjlbkw.cn/Article/details/gffygxlwa.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/gnlgamksm.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fktsv.cn/Article/details/grtuodsqe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.tarul.cn/Article/details/gtpktwkwe.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.yfazqb.com/Article/details/gegnchtvg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.vehdjk.com/Article/details/gfoiynimk.sHtML

TS:   arr.map(String)
来源：http://m.share.bbcook.cn/Article/details/gdphrlxzt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fktsv.cn/Article/details/gijiqpumu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.bbcook.cn/Article/details/gxrhszpvv.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fktsv.cn/Article/details/gafsswdte.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.yfazqb.com/Article/details/goamvxtao.sHtML

[C08] 闭包
来源：http://baike.vehdjk.com/Article/details/gbjwsoaja.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.epnwcf.com/Article/details/gtpgkqsgd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.sjlbkw.cn/Article/details/gpnjdvvhz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/goyqrbzet.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gbequdmua.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.bbcook.cn/Article/details/gkpsvlhbf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.tarul.cn/Article/details/glsgiicmt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.tarul.cn/Article/details/gzojomdxx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gsvjsftlk.sHtML

[C09] 递归
来源：http://www.m.share.epnwcf.com/Article/details/gjoivtzyf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gekwgcwcx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fktsv.cn/Article/details/gzftgyeju.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.epnwcf.com/Article/details/gilkdszgr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.epnwcf.com/Article/details/gcmnhdlko.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fktsv.cn/Article/details/gchacvnwf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/glxtatfak.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.bbcook.cn/Article/details/gbliivqav.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.vehdjk.com/Article/details/gstrhrowk.sHtML

[C10] 变量作用域
来源：http://www.share.vehdjk.com/Article/details/gfrbpfykd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.bbcook.cn/Article/details/gwigangxc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fktsv.cn/Article/details/gqejjegej.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.yfazqb.com/Article/details/gylmoztis.sHtML

TS:   同 JS
来源：http://m.share.tarul.cn/Article/details/gswwjbtbq.sHtML

Java: 方法内为块级作用域
来源：http://mobile.tarul.cn/Article/details/gndpuqvcr.sHtML

Go:   花括号块级作用域
来源：http://read.share.epnwcf.com/Article/details/gthpbwgpu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.tarul.cn/Article/details/gogbvnmgs.sHtML

C#:   块级作用域
来源：http://m.share.yfazqb.com/Article/details/gbptijtpu.sHtML

[C11] 模块导入与导出
来源：http://mobile.vehdjk.com/Article/details/gksyrhzqu.sHtML

Py:   from module import func
来源：http://mobile.tarul.cn/Article/details/gbxaqduxs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.tarul.cn/Article/details/gpmbhjnfz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.yfazqb.com/Article/details/gtxtinyog.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.vehdjk.com/Article/details/gzchlkeij.sHtML

Java: import java.util.List;
来源：http://mobile.epnwcf.com/Article/details/glvvmicji.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.tarul.cn/Article/details/gvztwissx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.vehdjk.com/Article/details/gwhnkiybk.sHtML

C#:   using System.Text;
来源：http://mobile.yfazqb.com/Article/details/gvuopqaxa.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.vehdjk.com/Article/details/gwywcjnlj.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fktsv.cn/Article/details/gfcxozcvg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.yfazqb.com/Article/details/ghljxltaj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.tarul.cn/Article/details/gytaibhzl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.epnwcf.com/Article/details/gibjkrklh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.bbcook.cn/Article/details/guzonfeod.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.vehdjk.com/Article/details/gltsgsbsf.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.sjlbkw.cn/Article/details/gwjqqkfld.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.sjlbkw.cn/Article/details/gfqlophjc.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.bbcook.cn/Article/details/ghlkkyyqh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.yfazqb.com/Article/details/gqfwulcii.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gjnhkmwlp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.bbcook.cn/Article/details/grhmuebxq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gbwntynik.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gcqzyrmam.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fktsv.cn/Article/details/gginpbdag.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.vehdjk.com/Article/details/guvgoownt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.vehdjk.com/Article/details/gbpbgleqi.sHtML

[C14] 泛型函数
来源：http://baike.tarul.cn/Article/details/gutwijmwb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.vehdjk.com/Article/details/gubcfhchx.sHtML

PHP:  // 无泛型
来源：http://wap.vehdjk.com/Article/details/gjjeeuusf.sHtML

JS:   // 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/gjjcvlayk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.bbcook.cn/Article/details/gprmdrvjy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.tarul.cn/Article/details/gkvflbzez.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.tarul.cn/Article/details/gkfsdusyo.sHtML

Ruby: # 无泛型
来源：http://www.blog.epnwcf.com/Article/details/ghzcoajay.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fktsv.cn/Article/details/gbsbkgveq.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyvbotjh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.vehdjk.com/Article/details/gmevfkugy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.vehdjk.com/Article/details/ghwayupww.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.epnwcf.com/Article/details/gumyhxgnc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.vehdjk.com/Article/details/gzohvbvxi.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/galmolpfo.sHtML

Go:   // 无解构
来源：http://3g.epnwcf.com/Article/details/gbaehsjee.sHtML

Ruby: a, b = pair
来源：http://blog.yfazqb.com/Article/details/gpfdlwaqh.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fktsv.cn/Article/details/gsnuznzix.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.epnwcf.com/Article/details/gjgfixdah.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjzsmoda.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/galohijmo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.bbcook.cn/Article/details/gxlkzwucx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fktsv.cn/Article/details/gvtojzncp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.tarul.cn/Article/details/gsupupngq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.sjlbkw.cn/Article/details/gkojxemms.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.yfazqb.com/Article/details/gkqzcrvdq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.vehdjk.com/Article/details/gemrcntwb.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gcrsdozwj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.epnwcf.com/Article/details/gavnaimlr.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gsviainbs.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.vehdjk.com/Article/details/gvahaeply.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.vehdjk.com/Article/details/gcracmbtx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.epnwcf.com/Article/details/gqvnmtryn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.yfazqb.com/Article/details/gnmczifuq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.epnwcf.com/Article/details/gybrlijea.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fktsv.cn/Article/details/gkrhjntjf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.tarul.cn/Article/details/ggljnimxa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.epnwcf.com/Article/details/gtasvhqzg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fktsv.cn/Article/details/gtbruzvkl.sHtML

[D02] 追加元素到末尾
来源：http://m.share.epnwcf.com/Article/details/gfqxuqcxo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fktsv.cn/Article/details/glaslodkp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fktsv.cn/Article/details/gncndmiuv.sHtML

JS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gsfymfvvr.sHtML

TS:   arr.push(4);
来源：http://wap.vehdjk.com/Article/details/gwjdabdgx.sHtML

Java: list.add(4);
来源：http://baike.bbcook.cn/Article/details/gqlkvgddb.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.epnwcf.com/Article/details/gcnurkcrn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.bbcook.cn/Article/details/gfxkjctbq.sHtML

C#:   list.Add(4);
来源：http://mobile.vehdjk.com/Article/details/gyglpyqaf.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.sjlbkw.cn/Article/details/gsnyirrah.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.epnwcf.com/Article/details/gtluulqml.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.bbcook.cn/Article/details/gnrazmjre.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.bbcook.cn/Article/details/gnojhxfnt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.tarul.cn/Article/details/gzsczlxpo.sHtML

Java: list.add(0, 0);
来源：http://www.blog.epnwcf.com/Article/details/gtlmixhcs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fktsv.cn/Article/details/gwwtvrgqj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.vehdjk.com/Article/details/gkwqbxwkn.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/glludpxxy.sHtML

[D04] 删除元素
来源：http://3g.tarul.cn/Article/details/grtycgpje.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.bbcook.cn/Article/details/gdzpmfour.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gxnnfimrh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.epnwcf.com/Article/details/gftzdwfyo.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fktsv.cn/Article/details/ggipckhcp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.tarul.cn/Article/details/ggxettdaq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.vehdjk.com/Article/details/goluovhnn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.epnwcf.com/Article/details/gkyewiemm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.vehdjk.com/Article/details/gpqfkjuau.sHtML

[D05] 访问与修改元素
来源：http://m.share.vehdjk.com/Article/details/gybvrxzuv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/gagrkaggi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gnlshsjni.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gnmipzpbw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.sjlbkw.cn/Article/details/gocfcegha.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.tarul.cn/Article/details/gouwybcjn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gbtrhazvq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gmkeumrym.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/gnblnqrhp.sHtML

[D06] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gvytnfopo.sHtML

Py:   len(arr)
来源：http://blog.vehdjk.com/Article/details/gmqvnappr.sHtML

PHP:  count($arr);
来源：http://www.share.yfazqb.com/Article/details/gxgmtudod.sHtML

JS:   arr.length
来源：http://www.share.bbcook.cn/Article/details/gdndihrtb.sHtML

TS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/gaurizier.sHtML

Java: list.size();
来源：http://baike.vehdjk.com/Article/details/gyfowbytp.sHtML

Go:   len(arr)
来源：http://blog.bbcook.cn/Article/details/glkbtzxgb.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.yfazqb.com/Article/details/gwaevkpft.sHtML

C#:   list.Count;
来源：http://blog.epnwcf.com/Article/details/gflnszuro.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.yfazqb.com/Article/details/gdseeeoqi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.yfazqb.com/Article/details/glggykemk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.vehdjk.com/Article/details/gxchojvig.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gfsebbtkm.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gxhmcvpdm.sHtML

Java: list.subList(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gcywskruo.sHtML

Go:   arr[1:4]
来源：http://www.share.vehdjk.com/Article/details/gmsifrhlp.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fktsv.cn/Article/details/giofvmqyk.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fktsv.cn/Article/details/geouizbyk.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fktsv.cn/Article/details/gdxbmmmue.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.tarul.cn/Article/details/gtqcllbfe.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.vehdjk.com/Article/details/glwxtgjqp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggicgiccn.sHtML

TS:   [...a, ...b];
来源：http://www.share.bbcook.cn/Article/details/ghbqhyfrk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fktsv.cn/Article/details/gblmvhhho.sHtML

Go:   append(a, b...)
来源：http://blog.tarul.cn/Article/details/godyfqusn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.bbcook.cn/Article/details/gqodolvke.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/godfdfvpm.sHtML

[D09] 排序（升序）
来源：http://www.share.sjlbkw.cn/Article/details/gcaewdcee.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gywssiowl.sHtML

PHP:  sort($arr);
来源：http://wap.bbcook.cn/Article/details/grmdbmgwq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fktsv.cn/Article/details/gjmluymdx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.vehdjk.com/Article/details/gwxpjslxr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.bbcook.cn/Article/details/gvgjqhfoj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/gxsegyzzi.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gmsnvkvsl.sHtML

C#:   list.Sort();
来源：http://3g.sjlbkw.cn/Article/details/gzhgdeqrj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.tarul.cn/Article/details/gbofrrlny.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.epnwcf.com/Article/details/gselmmmpd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.yfazqb.com/Article/details/grhvieilj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gnaoovnjb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.epnwcf.com/Article/details/gujpbvogd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.yfazqb.com/Article/details/gfreocwcu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.yfazqb.com/Article/details/gmbmoipyg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.tarul.cn/Article/details/gqrezsywz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.sjlbkw.cn/Article/details/gdyhviekp.sHtML

[D11] 反转数组
来源：http://m.share.tarul.cn/Article/details/gamsazkdj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.tarul.cn/Article/details/gkalvrzse.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.yfazqb.com/Article/details/gzvbituas.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fktsv.cn/Article/details/galiwfbca.sHtML

TS:   [...arr].reverse();
来源：http://baike.tarul.cn/Article/details/gruwlopzb.sHtML

Java: Collections.reverse(list);
来源：http://m.share.bbcook.cn/Article/details/gkeupfhpn.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.epnwcf.com/Article/details/gkjqeujhe.sHtML

Ruby: arr.reverse
来源：http://3g.epnwcf.com/Article/details/gevtdxjgb.sHtML

C#:   list.Reverse();
来源：http://www.share.yfazqb.com/Article/details/gchrghnxj.sHtML

[D12] 查找元素下标
来源：http://blog.vehdjk.com/Article/details/gagftjwoc.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.vehdjk.com/Article/details/gsunktrzp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.tarul.cn/Article/details/gnjzscijp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/gshwzvtpu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.bbcook.cn/Article/details/gbcvgwyxl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.epnwcf.com/Article/details/gpirbwumw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gekpglpne.sHtML

Ruby: arr.index(x)
来源：http://m.share.epnwcf.com/Article/details/gtzsidkvx.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/gowvreqct.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.yfazqb.com/Article/details/ggvqeuscd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.epnwcf.com/Article/details/gpuneksrs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.yfazqb.com/Article/details/gwumufjcw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gkosmsqjz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/gctvutuwg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.yfazqb.com/Article/details/gtbcazyqa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.sjlbkw.cn/Article/details/gywslqcft.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.sjlbkw.cn/Article/details/gsephyzkr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.tarul.cn/Article/details/gwwyroznj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fktsv.cn/Article/details/gfpxowqst.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fktsv.cn/Article/details/gspfjzogt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.sjlbkw.cn/Article/details/gklftwnex.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.vehdjk.com/Article/details/gwxaqbejh.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/gadsizlrp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gfgglnnyg.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gsjsstpqq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fktsv.cn/Article/details/gdmerzclw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fktsv.cn/Article/details/glnamfvwa.sHtML

[D15] 去重
来源：http://wap.sjlbkw.cn/Article/details/gkhhdmyql.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/gfwiidmev.sHtML

PHP:  array_unique($arr);
来源：http://m.share.tarul.cn/Article/details/gngmeykeq.sHtML

JS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gapfeiosz.sHtML


<!-- 参考信息 -->