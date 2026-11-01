代发 wailian999

Java: if (data == null) return;
来源：http://m.share.fktsv.cn/Article/details/gvjwxaxno.sHtML

Go:   if data == nil { return }
来源：http://m.share.vehdjk.com/Article/details/gynpuijbj.sHtML

Ruby: return if data.nil?
来源：http://baike.epnwcf.com/Article/details/gqlheitlt.sHtML

C#:   if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/grtzwszrx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gppjdrdwh.sHtML

C. 函数与作用域
来源：http://wap.epnwcf.com/Article/details/gdgpyildc.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gdsyudqdd.sHtML

[C01] 定义函数
来源：http://blog.bbcook.cn/Article/details/gvyfwuxpl.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.epnwcf.com/Article/details/gsaiquqam.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/ggenwmjzd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/goresuern.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gqojtpsth.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gxwngtvry.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.tarul.cn/Article/details/gjssxmpzg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.sjlbkw.cn/Article/details/gycbyvuxn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gnhqfizyj.sHtML

[C02] 默认参数
来源：http://www.share.tarul.cn/Article/details/gtocfbcpg.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.vehdjk.com/Article/details/gwdffukff.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.sjlbkw.cn/Article/details/gmgtaibby.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gxbtidetu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.tarul.cn/Article/details/gcbujtzre.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.tarul.cn/Article/details/guahcnxvp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.vehdjk.com/Article/details/gktgnnmrq.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.bbcook.cn/Article/details/gocrpcnhi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.tarul.cn/Article/details/gfgnvnrkg.sHtML

[C03] 可变参数
来源：http://3g.yfazqb.com/Article/details/gwzgqvyat.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/gmefpgypm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.yfazqb.com/Article/details/ggtlviswb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fktsv.cn/Article/details/gmxbqhytw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gadomnayb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.sjlbkw.cn/Article/details/gxfsnufrn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/gyhrydbkz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.epnwcf.com/Article/details/gxfncmyby.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.yfazqb.com/Article/details/gqmejzlxp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fktsv.cn/Article/details/gahdqkzpu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.tarul.cn/Article/details/gofdbwwkt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fktsv.cn/Article/details/gwrdbbsps.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/gykckavje.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.bbcook.cn/Article/details/gvqcyjsok.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.bbcook.cn/Article/details/gydwdckcc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.tarul.cn/Article/details/gvdcdresl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfhfscbd.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/grwuqbyhe.sHtML

[C05] 返回多个值
来源：http://read.share.fktsv.cn/Article/details/ggyprbskt.sHtML

Py:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gwjoiwdqp.sHtML

PHP:  return [$a, $b];
来源：http://wap.epnwcf.com/Article/details/gvanaozet.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fktsv.cn/Article/details/gahsigqeu.sHtML

TS:   return { a, b };
来源：http://read.share.vehdjk.com/Article/details/gstuvrcmh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.yfazqb.com/Article/details/gzpilsczd.sHtML

Go:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gyrioqeuc.sHtML

Ruby: return a, b
来源：http://www.share.tarul.cn/Article/details/gzfhcxcie.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.tarul.cn/Article/details/gchixpbdg.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.sjlbkw.cn/Article/details/ggpmcpdll.sHtML

Py:   square = lambda x: x * x
来源：http://wap.epnwcf.com/Article/details/gwwoeutid.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdfivpgv.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqrujomv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fktsv.cn/Article/details/gppitpksn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.tarul.cn/Article/details/gvxcbekgl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.tarul.cn/Article/details/gvsbzfqkx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.yfazqb.com/Article/details/gjhinlcjs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gjuspfork.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fktsv.cn/Article/details/gznvnqmtf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.bbcook.cn/Article/details/gghgatvyg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gcewjwqqk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.bbcook.cn/Article/details/gwfzqnoby.sHtML

TS:   arr.map(String)
来源：http://www.m.share.tarul.cn/Article/details/gjlebrtyh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.yfazqb.com/Article/details/gdieyltbb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.tarul.cn/Article/details/gognftcon.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.epnwcf.com/Article/details/gsddioxxo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.yfazqb.com/Article/details/gbxugyiit.sHtML

[C08] 闭包
来源：http://blog.sjlbkw.cn/Article/details/gwozuwwge.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.tarul.cn/Article/details/gdgwftazx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.vehdjk.com/Article/details/gqqgmyghp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gwmdpjtgd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gjynggdpv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.vehdjk.com/Article/details/gpxuawjgd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.epnwcf.com/Article/details/gryimhcqa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.sjlbkw.cn/Article/details/gmodbmcyq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/gpfyynztq.sHtML

[C09] 递归
来源：http://www.blog.tarul.cn/Article/details/gexbtbewl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.bbcook.cn/Article/details/gvnnnagwn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.tarul.cn/Article/details/gihjcyyyq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.epnwcf.com/Article/details/gklykfysm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gjvpujhry.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.bbcook.cn/Article/details/ghvuqtmjt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.vehdjk.com/Article/details/gaywffaam.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gtdggysrv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.yfazqb.com/Article/details/gotnruscc.sHtML

[C10] 变量作用域
来源：http://www.blog.bbcook.cn/Article/details/geyqcxomj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.bbcook.cn/Article/details/gowalrrom.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.vehdjk.com/Article/details/gqzecasqk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.vehdjk.com/Article/details/giyonjwjz.sHtML

TS:   同 JS
来源：http://baike.tarul.cn/Article/details/gbczhhsvb.sHtML

Java: 方法内为块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gbcybnoqx.sHtML

Go:   花括号块级作用域
来源：http://wap.yfazqb.com/Article/details/gqntvhohg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fktsv.cn/Article/details/gcdextopu.sHtML

C#:   块级作用域
来源：http://blog.epnwcf.com/Article/details/gxahuxuoa.sHtML

[C11] 模块导入与导出
来源：http://baike.bbcook.cn/Article/details/guvqfgktw.sHtML

Py:   from module import func
来源：http://read.share.bbcook.cn/Article/details/ggeasyapn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.epnwcf.com/Article/details/gwqqbwdsh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/ghrghpdtd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.tarul.cn/Article/details/gwiexhtzj.sHtML

Java: import java.util.List;
来源：http://3g.yfazqb.com/Article/details/guwbvyvzh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.bbcook.cn/Article/details/gdjryempk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fktsv.cn/Article/details/gtnlzdekz.sHtML

C#:   using System.Text;
来源：http://mobile.yfazqb.com/Article/details/gixbvskdu.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.yfazqb.com/Article/details/gznvhhpzd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.sjlbkw.cn/Article/details/gfokcizuo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.yfazqb.com/Article/details/gmxkhhklv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/geduphhcq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.bbcook.cn/Article/details/gkvmofnoc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.epnwcf.com/Article/details/gqbtolffu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.bbcook.cn/Article/details/gacjvdmei.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.sjlbkw.cn/Article/details/gpwxakafz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.vehdjk.com/Article/details/gckcphyij.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.yfazqb.com/Article/details/giciuzqju.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.bbcook.cn/Article/details/gthszsdnl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gqqhfnwyg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.vehdjk.com/Article/details/gtwuyxyag.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fktsv.cn/Article/details/ggwbtljjf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gbeoojkts.sHtML

Go:   func add(a, b int) int
来源：http://m.share.sjlbkw.cn/Article/details/grmoezvzr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.epnwcf.com/Article/details/gwgnbzhly.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.vehdjk.com/Article/details/gzaayoqto.sHtML

[C14] 泛型函数
来源：http://www.m.share.vehdjk.com/Article/details/gxzicrqnw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.vehdjk.com/Article/details/gwryyrfkq.sHtML

PHP:  // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gheabbfca.sHtML

JS:   // 无泛型
来源：http://m.share.fktsv.cn/Article/details/glrmzbdvq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.bbcook.cn/Article/details/gbtgppfrj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.bbcook.cn/Article/details/gbcvadabr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.sjlbkw.cn/Article/details/guohcpmrn.sHtML

Ruby: # 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gmtubqhzl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fktsv.cn/Article/details/gvgtyfprc.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.tarul.cn/Article/details/gtbnktdkp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.vehdjk.com/Article/details/gzsvxirvy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.sjlbkw.cn/Article/details/ggjrjfofw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/gjdetzesq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxipodvm.sHtML

Java: // 无解构
来源：http://3g.fktsv.cn/Article/details/gsnvofgqq.sHtML

Go:   // 无解构
来源：http://read.share.tarul.cn/Article/details/gsewveouy.sHtML

Ruby: a, b = pair
来源：http://wap.sjlbkw.cn/Article/details/gwyyrbavj.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fktsv.cn/Article/details/grdptxakm.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.bbcook.cn/Article/details/gutdxqvbq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fktsv.cn/Article/details/gyptsnqsy.sHtML

PHP:  // 无重载
来源：http://www.blog.sjlbkw.cn/Article/details/gwfwadgpg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fktsv.cn/Article/details/ggoeubpjs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.vehdjk.com/Article/details/gttkdwqmm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.vehdjk.com/Article/details/gadfcnjed.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.epnwcf.com/Article/details/gbeomzoqg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.sjlbkw.cn/Article/details/gapydclwb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fktsv.cn/Article/details/gjzjrradd.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gphlkqrdg.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.bbcook.cn/Article/details/gypaqtrol.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gomslxmpy.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.epnwcf.com/Article/details/gltopvfko.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.vehdjk.com/Article/details/gfmeflyer.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.bbcook.cn/Article/details/gxfwhnxuk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.vehdjk.com/Article/details/guotljmuh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.bbcook.cn/Article/details/gqgtxsjia.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.tarul.cn/Article/details/gpeyfqqlt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.sjlbkw.cn/Article/details/grslvziuw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.epnwcf.com/Article/details/gededjtzk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.tarul.cn/Article/details/gttdzstko.sHtML

[D02] 追加元素到末尾
来源：http://blog.sjlbkw.cn/Article/details/gzvlqtzee.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.sjlbkw.cn/Article/details/goybnklwn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.vehdjk.com/Article/details/gnfwgsusb.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gylytofxe.sHtML

TS:   arr.push(4);
来源：http://baike.bbcook.cn/Article/details/gmeloavew.sHtML

Java: list.add(4);
来源：http://www.blog.tarul.cn/Article/details/gnrajwqnx.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fktsv.cn/Article/details/gwwljclbh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fktsv.cn/Article/details/gzlzgfxjg.sHtML

C#:   list.Add(4);
来源：http://blog.sjlbkw.cn/Article/details/gqvhhcmmj.sHtML

[D03] 在指定位置插入元素
来源：http://wap.epnwcf.com/Article/details/gugpujksv.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gpmygpmdo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fktsv.cn/Article/details/gdahwyuqa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.vehdjk.com/Article/details/ggjgbybog.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gwvxabtgy.sHtML

Java: list.add(0, 0);
来源：http://m.share.bbcook.cn/Article/details/guybreaps.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.yfazqb.com/Article/details/giyxverkb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.vehdjk.com/Article/details/gbuhicipz.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.bbcook.cn/Article/details/gpmqfkyrc.sHtML

[D04] 删除元素
来源：http://www.m.share.vehdjk.com/Article/details/gzunwntpx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.epnwcf.com/Article/details/gauwoxuab.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fktsv.cn/Article/details/gfakpsbjh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.yfazqb.com/Article/details/glvoegzbv.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.sjlbkw.cn/Article/details/gdklcxxxn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuiviqex.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.vehdjk.com/Article/details/gkatkxikk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.sjlbkw.cn/Article/details/gnjzjgtgn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.epnwcf.com/Article/details/gmcmvfgks.sHtML

[D05] 访问与修改元素
来源：http://m.share.epnwcf.com/Article/details/gguhspcgq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/ghsbyuwat.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gysrunipt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gdestepmb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.epnwcf.com/Article/details/gdwlmiqdg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fktsv.cn/Article/details/gyxqanhtx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/ggyafjwhc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/glpnoqxnr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gyurvlzrp.sHtML

[D06] 数组长度
来源：http://baike.fktsv.cn/Article/details/gphdgtsen.sHtML

Py:   len(arr)
来源：http://baike.yfazqb.com/Article/details/gueungcje.sHtML

PHP:  count($arr);
来源：http://3g.tarul.cn/Article/details/gkzriplti.sHtML

JS:   arr.length
来源：http://www.m.share.bbcook.cn/Article/details/gyvcnowco.sHtML

TS:   arr.length
来源：http://www.blog.yfazqb.com/Article/details/ggmvzemxe.sHtML

Java: list.size();
来源：http://www.share.fktsv.cn/Article/details/gnybffxee.sHtML

Go:   len(arr)
来源：http://read.share.vehdjk.com/Article/details/gidfbqnsz.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gaqipzaea.sHtML

C#:   list.Count;
来源：http://read.share.epnwcf.com/Article/details/gwjtvwuhn.sHtML

[D07] 切片 / 取子数组
来源：http://3g.yfazqb.com/Article/details/gwhfjbvll.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.sjlbkw.cn/Article/details/gfqvdjhbq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.vehdjk.com/Article/details/gxmmguvwm.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gufnhfwrq.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gppompibc.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gddajpden.sHtML

Go:   arr[1:4]
来源：http://m.share.sjlbkw.cn/Article/details/gxgwzieag.sHtML

Ruby: arr[1, 3]
来源：http://3g.fktsv.cn/Article/details/gcinkhswq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gtctaojhv.sHtML

[D08] 合并两个数组
来源：http://read.share.tarul.cn/Article/details/gvrqtuvmi.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.yfazqb.com/Article/details/glpqvpqyu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fktsv.cn/Article/details/giqxztsin.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.vehdjk.com/Article/details/gazqmdghc.sHtML

TS:   [...a, ...b];
来源：http://3g.epnwcf.com/Article/details/gshmcsvqw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.bbcook.cn/Article/details/ggimdjttd.sHtML

Go:   append(a, b...)
来源：http://read.share.bbcook.cn/Article/details/glxecqfwz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.yfazqb.com/Article/details/ghjnizdfd.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.epnwcf.com/Article/details/glzwrnton.sHtML

[D09] 排序（升序）
来源：http://m.share.sjlbkw.cn/Article/details/gzhwyrjem.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/gydyxizjw.sHtML

PHP:  sort($arr);
来源：http://www.share.tarul.cn/Article/details/gxexfyuns.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.epnwcf.com/Article/details/gshhdurar.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fktsv.cn/Article/details/gmxeuytcu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.bbcook.cn/Article/details/gtyephdcv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gmhsauxyn.sHtML

Ruby: arr.sort
来源：http://baike.bbcook.cn/Article/details/gyhhtklcp.sHtML

C#:   list.Sort();
来源：http://3g.vehdjk.com/Article/details/glplcftke.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.epnwcf.com/Article/details/gzinzplrp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.yfazqb.com/Article/details/gdxuslwgl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.vehdjk.com/Article/details/gqaloyjut.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gftweyywg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gysyxzefn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.tarul.cn/Article/details/guqkfoata.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gilxsgvaq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.vehdjk.com/Article/details/gphpijuam.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.tarul.cn/Article/details/gwnggqxus.sHtML

[D11] 反转数组
来源：http://www.share.yfazqb.com/Article/details/gzstwspqm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.yfazqb.com/Article/details/gebrrntwz.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.bbcook.cn/Article/details/ghxpzdpws.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.vehdjk.com/Article/details/gsanphbry.sHtML

TS:   [...arr].reverse();
来源：http://baike.epnwcf.com/Article/details/gtyzwoyki.sHtML

Java: Collections.reverse(list);
来源：http://blog.bbcook.cn/Article/details/gqcgiprle.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fktsv.cn/Article/details/goychezjk.sHtML

Ruby: arr.reverse
来源：http://m.share.tarul.cn/Article/details/ggjyfdakr.sHtML

C#:   list.Reverse();
来源：http://www.m.share.vehdjk.com/Article/details/grilsbmgu.sHtML

[D12] 查找元素下标
来源：http://wap.bbcook.cn/Article/details/grsatalxg.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.vehdjk.com/Article/details/gnyfbowyc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.bbcook.cn/Article/details/ghrckolaf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.sjlbkw.cn/Article/details/gtcczqvoy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/gixqskusk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.sjlbkw.cn/Article/details/genihgrqj.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.yfazqb.com/Article/details/gpmqkpvjl.sHtML

Ruby: arr.index(x)
来源：http://read.share.bbcook.cn/Article/details/gbnnsbcab.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.tarul.cn/Article/details/gdxgkcspd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.tarul.cn/Article/details/gictsbujs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.vehdjk.com/Article/details/gjmkwfmyq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.vehdjk.com/Article/details/gpoqkjqoa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/gqgpgzuyl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/gavlpsztp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.tarul.cn/Article/details/gidfbqkqm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.bbcook.cn/Article/details/gmczoxwrm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.epnwcf.com/Article/details/gxibfwfnm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.tarul.cn/Article/details/giednmzlx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fktsv.cn/Article/details/gofhijfpo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.bbcook.cn/Article/details/gemaecrze.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/gxhrldglw.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/grznhiaux.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/gbgkpsulk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.epnwcf.com/Article/details/ggjpxeufy.sHtML

Go:   // 手写循环
来源：http://wap.epnwcf.com/Article/details/gdlzpblvs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.vehdjk.com/Article/details/gqwzluhjd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gglsromgz.sHtML

[D15] 去重
来源：http://www.share.sjlbkw.cn/Article/details/ggwqwlkmh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fktsv.cn/Article/details/gpxahmkle.sHtML

PHP:  array_unique($arr);
来源：http://blog.fktsv.cn/Article/details/geslzhuqm.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/ghctfkpkn.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gyedoselz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.yfazqb.com/Article/details/gkzewqqcg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.tarul.cn/Article/details/gtthzcuwo.sHtML

Ruby: arr.uniq
来源：http://www.share.tarul.cn/Article/details/gjbqzofse.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.tarul.cn/Article/details/gajhfmccp.sHtML

[D16] 求和与平均值
来源：http://3g.bbcook.cn/Article/details/gafhrknkp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gzdohwhyn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.sjlbkw.cn/Article/details/gassgewya.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.yfazqb.com/Article/details/gibpqlsnl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/gvtxytvtl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fktsv.cn/Article/details/gsfubzueg.sHtML

Go:   // 手写循环累加
来源：http://baike.fktsv.cn/Article/details/gisgudbfb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/gqpalsfyn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.epnwcf.com/Article/details/gofwogklp.sHtML

[D17] 最大值与最小值
来源：http://blog.yfazqb.com/Article/details/glgqnctxk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.yfazqb.com/Article/details/gkabslari.sHtML


<!-- 参考信息 -->