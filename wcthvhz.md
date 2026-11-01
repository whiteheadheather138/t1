代发 wailian999

================================================================================
来源：http://read.share.tarul.cn/Article/details/gjqbbfoaa.sHtML

C. 函数与作用域
来源：http://www.share.bbcook.cn/Article/details/gjnlcdlwl.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwtftmtm.sHtML

[C01] 定义函数
来源：http://mobile.fktsv.cn/Article/details/gwvbdimwj.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.tarul.cn/Article/details/geowzderj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/giwpruxhj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gmtoxzbey.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gltvecbgp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gzaftonih.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.tarul.cn/Article/details/gdxtumkwn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.epnwcf.com/Article/details/grkuveanw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gdglqnlqi.sHtML

[C02] 默认参数
来源：http://3g.epnwcf.com/Article/details/guuizxjas.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.tarul.cn/Article/details/gfkrjifvr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.vehdjk.com/Article/details/glcswrniq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gerapmstn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gdzchutid.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.tarul.cn/Article/details/gghznninl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fktsv.cn/Article/details/gsdnvjcfx.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.sjlbkw.cn/Article/details/gytvrbzal.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.yfazqb.com/Article/details/gxrlfcwsg.sHtML

[C03] 可变参数
来源：http://m.share.sjlbkw.cn/Article/details/goevtsntk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.vehdjk.com/Article/details/ghutabiyw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.yfazqb.com/Article/details/gewunqqze.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/gdkbosglg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/gxirynjld.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fktsv.cn/Article/details/gleqyglsj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.vehdjk.com/Article/details/ggxkmrrti.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.sjlbkw.cn/Article/details/gtbswgzeb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.epnwcf.com/Article/details/gpqohobdr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gywmxkzam.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.yfazqb.com/Article/details/ggqditjgb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/glgvpcghy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gleucfupy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.vehdjk.com/Article/details/gmhpqfwob.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.vehdjk.com/Article/details/ghycuzvee.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.sjlbkw.cn/Article/details/gryfwfxtt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gtciusnpg.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gnxqpcsor.sHtML

[C05] 返回多个值
来源：http://www.share.vehdjk.com/Article/details/gjizfqyhq.sHtML

Py:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gtvolejky.sHtML

PHP:  return [$a, $b];
来源：http://mobile.bbcook.cn/Article/details/gpdimitdu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gdtpwjbmb.sHtML

TS:   return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gdptitsru.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.vehdjk.com/Article/details/gxbsbkubr.sHtML

Go:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gynggiupz.sHtML

Ruby: return a, b
来源：http://read.share.tarul.cn/Article/details/gyfylwtnb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.sjlbkw.cn/Article/details/gbtcgenhg.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/gjccdxmtb.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.tarul.cn/Article/details/glwsslzpg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.epnwcf.com/Article/details/gqlkhloju.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gcqpzlhlp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fktsv.cn/Article/details/gkrfpscml.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.tarul.cn/Article/details/gtgaxsdbp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.vehdjk.com/Article/details/gwjgitqyw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.sjlbkw.cn/Article/details/gzyweaobz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/gacwtidze.sHtML

[C07] 把函数作为参数传入
来源：http://baike.bbcook.cn/Article/details/glsjefsse.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fktsv.cn/Article/details/gcgzpxssw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.yfazqb.com/Article/details/gggpadwfl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.bbcook.cn/Article/details/gbghilbhz.sHtML

TS:   arr.map(String)
来源：http://www.m.share.sjlbkw.cn/Article/details/grphqgqgt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/gaegitnhh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.bbcook.cn/Article/details/guugkjall.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.yfazqb.com/Article/details/gqohyrety.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.sjlbkw.cn/Article/details/gmodawofb.sHtML

[C08] 闭包
来源：http://www.m.share.bbcook.cn/Article/details/gmaxmmdgg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.epnwcf.com/Article/details/gysyqywnj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.bbcook.cn/Article/details/ghrmvtzfh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gwjiocczg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gobguxgix.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.bbcook.cn/Article/details/gmmwnpgrd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.vehdjk.com/Article/details/gtqcfvixq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.sjlbkw.cn/Article/details/gttfskvsw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gxabllpmt.sHtML

[C09] 递归
来源：http://blog.tarul.cn/Article/details/gsmodygrj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/gzekcsfay.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gomfkimrp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gplvyftgv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.epnwcf.com/Article/details/guiooqydy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fktsv.cn/Article/details/gpynkskup.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.sjlbkw.cn/Article/details/gzydphlsz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/gkolohdwb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.yfazqb.com/Article/details/gpdpkthos.sHtML

[C10] 变量作用域
来源：http://blog.sjlbkw.cn/Article/details/gjjsgpfyl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.sjlbkw.cn/Article/details/gbshwyucc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.tarul.cn/Article/details/gtwfibdkp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.epnwcf.com/Article/details/grlqzoipc.sHtML

TS:   同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gusfyvosp.sHtML

Java: 方法内为块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gglubfhhk.sHtML

Go:   花括号块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gubeqstfr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.sjlbkw.cn/Article/details/gpkksllcd.sHtML

C#:   块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gchkonhqt.sHtML

[C11] 模块导入与导出
来源：http://wap.vehdjk.com/Article/details/gwuojgctb.sHtML

Py:   from module import func
来源：http://m.share.fktsv.cn/Article/details/gifjykyep.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.yfazqb.com/Article/details/gbieloerh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.vehdjk.com/Article/details/gtgkicgrl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.vehdjk.com/Article/details/gksqlhwsi.sHtML

Java: import java.util.List;
来源：http://blog.yfazqb.com/Article/details/giazmazvj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.yfazqb.com/Article/details/gmtegrvdh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.vehdjk.com/Article/details/guzfxfeoj.sHtML

C#:   using System.Text;
来源：http://3g.fktsv.cn/Article/details/gwruevpsb.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.bbcook.cn/Article/details/gysgqjcrl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fktsv.cn/Article/details/ggxgyemaz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.bbcook.cn/Article/details/gqqlwrghk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gqbgxqcxo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.sjlbkw.cn/Article/details/glvczjcpk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.tarul.cn/Article/details/gsicmgorl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.epnwcf.com/Article/details/gzmnlfaqi.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.epnwcf.com/Article/details/gpivoiiad.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.vehdjk.com/Article/details/gtqesmcxg.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.tarul.cn/Article/details/gubckxqua.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.epnwcf.com/Article/details/gqsvzxlrn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gsllxudbm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.yfazqb.com/Article/details/gyjgpzqnk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/geyoxuwuf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gimswvtkn.sHtML

Go:   func add(a, b int) int
来源：http://blog.yfazqb.com/Article/details/gadgdusld.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.epnwcf.com/Article/details/gdgemtorn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.sjlbkw.cn/Article/details/gfcvsbjdl.sHtML

[C14] 泛型函数
来源：http://m.share.bbcook.cn/Article/details/gunzpauop.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.yfazqb.com/Article/details/gilqoausk.sHtML

PHP:  // 无泛型
来源：http://3g.yfazqb.com/Article/details/glhhnnrfl.sHtML

JS:   // 无泛型
来源：http://3g.fktsv.cn/Article/details/gdzvjtbxn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.vehdjk.com/Article/details/gnjanowmf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.yfazqb.com/Article/details/gpbdysrhe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fktsv.cn/Article/details/gxuyskies.sHtML

Ruby: # 无泛型
来源：http://blog.tarul.cn/Article/details/gzplbfoxp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.epnwcf.com/Article/details/grgkaokzy.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.vehdjk.com/Article/details/gkesjzwok.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.sjlbkw.cn/Article/details/gerkwjnyk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.bbcook.cn/Article/details/gzojtdlkv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.vehdjk.com/Article/details/gibumytju.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gscpkypnf.sHtML

Java: // 无解构
来源：http://read.share.fktsv.cn/Article/details/gzsmykcvz.sHtML

Go:   // 无解构
来源：http://www.blog.epnwcf.com/Article/details/gdugeospf.sHtML

Ruby: a, b = pair
来源：http://baike.sjlbkw.cn/Article/details/gfkbbzdlk.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.epnwcf.com/Article/details/gzzbfmjem.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.epnwcf.com/Article/details/gpkyjpiyo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.bbcook.cn/Article/details/gooinibbg.sHtML

PHP:  // 无重载
来源：http://www.blog.vehdjk.com/Article/details/guqvtogkb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fktsv.cn/Article/details/gbwdmcnde.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fktsv.cn/Article/details/gidcxbvea.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fktsv.cn/Article/details/gijvbbgzi.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.tarul.cn/Article/details/gdzntndud.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.vehdjk.com/Article/details/ggruulwpk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.sjlbkw.cn/Article/details/gicwwnmai.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gefoynacr.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fktsv.cn/Article/details/gspbdvfhe.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwdttmksk.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.yfazqb.com/Article/details/gicatxxbi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.bbcook.cn/Article/details/gblzvvlqf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.epnwcf.com/Article/details/gjnoccohf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.epnwcf.com/Article/details/gqwfsmxxf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.vehdjk.com/Article/details/gdcmzuosb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.vehdjk.com/Article/details/gpgqoawug.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.epnwcf.com/Article/details/gmapcessj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.sjlbkw.cn/Article/details/gtmmbmfbu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.epnwcf.com/Article/details/gwbiqvxdw.sHtML

[D02] 追加元素到末尾
来源：http://wap.vehdjk.com/Article/details/gdmrtrujl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.bbcook.cn/Article/details/gymajahgq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.sjlbkw.cn/Article/details/gntraygzr.sHtML

JS:   arr.push(4);
来源：http://m.share.bbcook.cn/Article/details/gesqpjakc.sHtML

TS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gluufjxmf.sHtML

Java: list.add(4);
来源：http://read.share.sjlbkw.cn/Article/details/gplygzaqo.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gnddbpqcv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fktsv.cn/Article/details/guphlbfkv.sHtML

C#:   list.Add(4);
来源：http://blog.vehdjk.com/Article/details/gmrsxoivh.sHtML

[D03] 在指定位置插入元素
来源：http://wap.epnwcf.com/Article/details/gsqmoctvn.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.tarul.cn/Article/details/gqgeouied.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fktsv.cn/Article/details/gvgdfwvee.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.yfazqb.com/Article/details/gityuozim.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcqmgbzs.sHtML

Java: list.add(0, 0);
来源：http://blog.bbcook.cn/Article/details/guwvhenzs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.bbcook.cn/Article/details/gzgzeruzk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.sjlbkw.cn/Article/details/gskxzjluo.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gwpqjoxzq.sHtML

[D04] 删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gngykknvz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.vehdjk.com/Article/details/gcnwaauuv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwdvrlro.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.epnwcf.com/Article/details/ghiqhazqy.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.bbcook.cn/Article/details/gtdgsfdbv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.yfazqb.com/Article/details/gerwajnzn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fktsv.cn/Article/details/gjbbdkxdf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.tarul.cn/Article/details/gyxgguqvs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.vehdjk.com/Article/details/guzgiggua.sHtML

[D05] 访问与修改元素
来源：http://blog.yfazqb.com/Article/details/gmcwtsfcs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gfaphkdtl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/gswrdyszm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gwesqeahs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.tarul.cn/Article/details/gpkylewwo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.tarul.cn/Article/details/gypcbwhvs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gdfrqgzbu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gtkdrybrk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fktsv.cn/Article/details/granjpfwz.sHtML

[D06] 数组长度
来源：http://read.share.fktsv.cn/Article/details/ggopmjzme.sHtML

Py:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gomortzjy.sHtML

PHP:  count($arr);
来源：http://mobile.fktsv.cn/Article/details/glszleiqu.sHtML

JS:   arr.length
来源：http://baike.tarul.cn/Article/details/gjfhdkxkq.sHtML

TS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gzskuplat.sHtML

Java: list.size();
来源：http://read.share.fktsv.cn/Article/details/gkebgnims.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gmntlhova.sHtML

Ruby: arr.length; arr.size
来源：http://blog.epnwcf.com/Article/details/gzdmofgyy.sHtML

C#:   list.Count;
来源：http://baike.sjlbkw.cn/Article/details/gkzwkvpju.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.tarul.cn/Article/details/gzhexnnod.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.sjlbkw.cn/Article/details/gdwofgdqf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.bbcook.cn/Article/details/glbeuyqqc.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.bbcook.cn/Article/details/gjqspieqp.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/grovzrton.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gubbthlkr.sHtML

Go:   arr[1:4]
来源：http://baike.epnwcf.com/Article/details/gcvrbddqg.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fktsv.cn/Article/details/gcsgcnren.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.yfazqb.com/Article/details/guymfwbem.sHtML

[D08] 合并两个数组
来源：http://blog.tarul.cn/Article/details/gxqeilkyp.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.vehdjk.com/Article/details/garaqfeqe.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.tarul.cn/Article/details/gcvcqjzaz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.bbcook.cn/Article/details/gzanvtdev.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxhzogoy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.vehdjk.com/Article/details/ggtfcsnhn.sHtML

Go:   append(a, b...)
来源：http://wap.sjlbkw.cn/Article/details/gjcswqtzq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fktsv.cn/Article/details/gcftemgmw.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.yfazqb.com/Article/details/ggqayxsba.sHtML

[D09] 排序（升序）
来源：http://read.share.yfazqb.com/Article/details/gwlclblcd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/geznnebjx.sHtML

PHP:  sort($arr);
来源：http://3g.vehdjk.com/Article/details/gpzhlnqsq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.epnwcf.com/Article/details/gwmliqgwi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.vehdjk.com/Article/details/gdfgejqam.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fktsv.cn/Article/details/gtwgvrwja.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/gcwasgehz.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/glowrresi.sHtML

C#:   list.Sort();
来源：http://www.share.bbcook.cn/Article/details/gwzpfqcsn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.tarul.cn/Article/details/gkddbskvx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.vehdjk.com/Article/details/gqlflfcpn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/grluzgsus.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fktsv.cn/Article/details/gweseckin.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fktsv.cn/Article/details/gbtiqfahr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.yfazqb.com/Article/details/gxstqtspg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.yfazqb.com/Article/details/gosocckgd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fktsv.cn/Article/details/gruedvtlk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.bbcook.cn/Article/details/gwchzpkqm.sHtML

[D11] 反转数组
来源：http://baike.fktsv.cn/Article/details/grwnzpwbg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.sjlbkw.cn/Article/details/glvnvnfyz.sHtML

PHP:  array_reverse($arr);
来源：http://baike.tarul.cn/Article/details/guyarrtuc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.tarul.cn/Article/details/gaylzrsqd.sHtML

TS:   [...arr].reverse();
来源：http://mobile.sjlbkw.cn/Article/details/giqjknxzc.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrgodzyl.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.epnwcf.com/Article/details/gpmxcxtwq.sHtML

Ruby: arr.reverse
来源：http://baike.sjlbkw.cn/Article/details/ggynvhbpn.sHtML

C#:   list.Reverse();
来源：http://3g.yfazqb.com/Article/details/gvzriqxlk.sHtML

[D12] 查找元素下标
来源：http://www.m.share.bbcook.cn/Article/details/gojnkthny.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.tarul.cn/Article/details/gbepnbxdx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fktsv.cn/Article/details/gzcvpwjba.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/gqlihskxo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/ggebxnjuh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.epnwcf.com/Article/details/gylhqpuhk.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.epnwcf.com/Article/details/glxrzzgae.sHtML

Ruby: arr.index(x)
来源：http://read.share.fktsv.cn/Article/details/gtilrmyiq.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.bbcook.cn/Article/details/gvlzrytvh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.bbcook.cn/Article/details/gwrjpyvoc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/gqvpomgsv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.epnwcf.com/Article/details/gsuuxdygq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/gqhteroed.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/gxsckrrrl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.vehdjk.com/Article/details/gjhtnuwby.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fktsv.cn/Article/details/govhjidjy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.bbcook.cn/Article/details/gorpvnpbi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gxpfpkspe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fktsv.cn/Article/details/gwvjtkkbj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.tarul.cn/Article/details/gbhdbbytq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fktsv.cn/Article/details/gsxrkpaie.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gpciviuhj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gvefttxip.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.tarul.cn/Article/details/gnjhvshiw.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gsvlpblic.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.tarul.cn/Article/details/gzyrlipal.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.vehdjk.com/Article/details/gqasjkadm.sHtML

[D15] 去重
来源：http://wap.fktsv.cn/Article/details/gxfiutfuy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.bbcook.cn/Article/details/giactgyop.sHtML

PHP:  array_unique($arr);
来源：http://wap.sjlbkw.cn/Article/details/gpgxrwxbc.sHtML

JS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gumwmgjxr.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/gjrkrozsp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.yfazqb.com/Article/details/gnpfwberd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.epnwcf.com/Article/details/golrqkgtc.sHtML

Ruby: arr.uniq
来源：http://wap.bbcook.cn/Article/details/grptuiwjy.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.bbcook.cn/Article/details/gxbaevogv.sHtML

[D16] 求和与平均值
来源：http://wap.vehdjk.com/Article/details/gagmbeoxb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gzhnpplcg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.sjlbkw.cn/Article/details/gyxdririn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/goxvmeyxk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/gkavtuwnh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.sjlbkw.cn/Article/details/gkoyvykxc.sHtML

Go:   // 手写循环累加
来源：http://3g.tarul.cn/Article/details/gkocdtedu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.epnwcf.com/Article/details/gnrbwgxmd.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.yfazqb.com/Article/details/gzscbodcu.sHtML

[D17] 最大值与最小值
来源：http://mobile.tarul.cn/Article/details/gtrxmzflq.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.tarul.cn/Article/details/gfucsquae.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.tarul.cn/Article/details/gjoolyuuu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.sjlbkw.cn/Article/details/grxzsqdmx.sHtML

TS:   Math.max(...arr);
来源：http://baike.sjlbkw.cn/Article/details/gabqtlcvt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.yfazqb.com/Article/details/gskfaadho.sHtML


<!-- 参考信息 -->