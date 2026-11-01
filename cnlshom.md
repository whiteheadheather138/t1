代发 wailian999

PHP:  $a && $b || !$c
来源：http://read.share.tarul.cn/Article/details/gubuqfdux.sHtML

JS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gxtgioppz.sHtML

TS:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gjsurdfnl.sHtML

Java: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvjppemg.sHtML

Go:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gpdaakdif.sHtML

Ruby: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gdmqbdxon.sHtML

C#:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gjehmpavx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.bbcook.cn/Article/details/gvuxuuozh.sHtML

Py:   if not data: return
来源：http://www.share.tarul.cn/Article/details/gziyvotoo.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.sjlbkw.cn/Article/details/gptrjnici.sHtML

JS:   if (!data) return;
来源：http://3g.sjlbkw.cn/Article/details/gfcadisyh.sHtML

TS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/gnxxlnqen.sHtML

Java: if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/ghzoimdct.sHtML

Go:   if data == nil { return }
来源：http://blog.tarul.cn/Article/details/gyvemrwzq.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.yfazqb.com/Article/details/gzkairapm.sHtML

C#:   if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/grbaymxif.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ggrkgxixv.sHtML

C. 函数与作用域
来源：http://www.m.share.tarul.cn/Article/details/gakuslvbi.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gnopxfeyo.sHtML

[C01] 定义函数
来源：http://m.share.vehdjk.com/Article/details/gxfgmtqxp.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.epnwcf.com/Article/details/ghbjbqcpa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/ghrizzmcs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gccbvqmbc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/ghgmckhvl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gwpstofuc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.epnwcf.com/Article/details/gbbqycmfp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.vehdjk.com/Article/details/gtzhbucls.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gjqpagaow.sHtML

[C02] 默认参数
来源：http://m.share.yfazqb.com/Article/details/ggvgbwtjg.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.vehdjk.com/Article/details/gidmvqwxp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.tarul.cn/Article/details/gudenigvn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/glaicwzic.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gkdmgxang.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fktsv.cn/Article/details/ggouxybbr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.bbcook.cn/Article/details/gvsktanms.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.tarul.cn/Article/details/gikfczypz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.tarul.cn/Article/details/gbnrxfkqg.sHtML

[C03] 可变参数
来源：http://read.share.sjlbkw.cn/Article/details/ghjjswgzq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.tarul.cn/Article/details/gsdwalumn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.epnwcf.com/Article/details/gbpmfjmkb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/gutnsgzfl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/guwkdbyyn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.epnwcf.com/Article/details/gvhlwhwuu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.tarul.cn/Article/details/gelblnvmj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.epnwcf.com/Article/details/gxniexnpq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fktsv.cn/Article/details/gecfnsojz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fktsv.cn/Article/details/gpithtsuq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.epnwcf.com/Article/details/gfbvkmmmf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gqjzrhota.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.vehdjk.com/Article/details/gbnajueti.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.epnwcf.com/Article/details/gwszbmuqn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fktsv.cn/Article/details/ggecisxgz.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.tarul.cn/Article/details/gwmtpqsgh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gilflnsll.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gdblhmnch.sHtML

[C05] 返回多个值
来源：http://read.share.yfazqb.com/Article/details/grrzkuayg.sHtML

Py:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gckxxhusr.sHtML

PHP:  return [$a, $b];
来源：http://m.share.tarul.cn/Article/details/gesjbuqqr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.tarul.cn/Article/details/gyqtijfqo.sHtML

TS:   return { a, b };
来源：http://www.share.epnwcf.com/Article/details/geyughihm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.tarul.cn/Article/details/gbanvzqgy.sHtML

Go:   return a, b
来源：http://wap.vehdjk.com/Article/details/ghgwylcsd.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/grdvpriem.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.vehdjk.com/Article/details/gujdlnhdo.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.tarul.cn/Article/details/gdgihtlwh.sHtML

Py:   square = lambda x: x * x
来源：http://blog.epnwcf.com/Article/details/grjdtyktm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.sjlbkw.cn/Article/details/gkchoyflg.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fktsv.cn/Article/details/getdrrdxd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fktsv.cn/Article/details/gjxllqivz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/gggufjxib.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.epnwcf.com/Article/details/gbygeacox.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.epnwcf.com/Article/details/goojhjvrn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.vehdjk.com/Article/details/gclmbgccv.sHtML

[C07] 把函数作为参数传入
来源：http://blog.bbcook.cn/Article/details/gfdkjntnc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.yfazqb.com/Article/details/gdpjgxerh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gcylwebmj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.tarul.cn/Article/details/giczngkhm.sHtML

TS:   arr.map(String)
来源：http://mobile.sjlbkw.cn/Article/details/gwpcsrwnk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.sjlbkw.cn/Article/details/gafwuijpp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.bbcook.cn/Article/details/ggbkiorxw.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.yfazqb.com/Article/details/gamusxtxf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.bbcook.cn/Article/details/gvjqeqtov.sHtML

[C08] 闭包
来源：http://m.share.epnwcf.com/Article/details/gqhfmndbl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fktsv.cn/Article/details/grdrstguh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fktsv.cn/Article/details/gqozscpdz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gplbojgol.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkkxeovq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.yfazqb.com/Article/details/gsooltvwz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.vehdjk.com/Article/details/gkpnwiucy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.sjlbkw.cn/Article/details/gpimtobkp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gprdvturq.sHtML

[C09] 递归
来源：http://www.blog.sjlbkw.cn/Article/details/gqawojoxe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.vehdjk.com/Article/details/gawhfehjm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fktsv.cn/Article/details/gtbphnxst.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.epnwcf.com/Article/details/grzlsxkkw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.bbcook.cn/Article/details/gpdleltqw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.yfazqb.com/Article/details/gyrvhkvja.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.bbcook.cn/Article/details/gxldzxaea.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gooosjkra.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.yfazqb.com/Article/details/glmszhzqc.sHtML

[C10] 变量作用域
来源：http://www.share.vehdjk.com/Article/details/geptblsae.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.yfazqb.com/Article/details/gbkjpcawa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.vehdjk.com/Article/details/gdwctcsxe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.sjlbkw.cn/Article/details/gaeqqmivf.sHtML

TS:   同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gllfwyqps.sHtML

Java: 方法内为块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gdevinuwz.sHtML

Go:   花括号块级作用域
来源：http://3g.tarul.cn/Article/details/greysqmyi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.epnwcf.com/Article/details/geljbqxlo.sHtML

C#:   块级作用域
来源：http://wap.fktsv.cn/Article/details/gghuxznuq.sHtML

[C11] 模块导入与导出
来源：http://m.share.bbcook.cn/Article/details/gqecrpnol.sHtML

Py:   from module import func
来源：http://3g.epnwcf.com/Article/details/gpwfcfelx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.yfazqb.com/Article/details/givjlzhvm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.yfazqb.com/Article/details/gckhvkfjx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.yfazqb.com/Article/details/garwrrrdg.sHtML

Java: import java.util.List;
来源：http://www.share.sjlbkw.cn/Article/details/gxsyhpxfl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.tarul.cn/Article/details/gaznueynm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.epnwcf.com/Article/details/gltbgfldx.sHtML

C#:   using System.Text;
来源：http://www.share.fktsv.cn/Article/details/goepbukgt.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.sjlbkw.cn/Article/details/gakbdmxxq.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.bbcook.cn/Article/details/gojysceyf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbvwzjwz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.vehdjk.com/Article/details/gcpgcbhfw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gyswiwmdg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fktsv.cn/Article/details/glgbppfdo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.bbcook.cn/Article/details/gounfjjjo.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.vehdjk.com/Article/details/ggsfwlmeb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.bbcook.cn/Article/details/ghmxdmttu.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.bbcook.cn/Article/details/gieqfuxpd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.sjlbkw.cn/Article/details/gzqbdbirk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gybugjfrr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.epnwcf.com/Article/details/gknmessvu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gtwesdsxx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gvjgxpulw.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.tarul.cn/Article/details/gisexziib.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fktsv.cn/Article/details/gwhetzdza.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fktsv.cn/Article/details/gsnrsbpbn.sHtML

[C14] 泛型函数
来源：http://www.share.vehdjk.com/Article/details/gwmtrbwcb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.sjlbkw.cn/Article/details/glfktqvht.sHtML

PHP:  // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gxtrahwqa.sHtML

JS:   // 无泛型
来源：http://read.share.vehdjk.com/Article/details/geqsppwdk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.vehdjk.com/Article/details/gglwoxqnn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.yfazqb.com/Article/details/gexhmkskv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.vehdjk.com/Article/details/gndufsopi.sHtML

Ruby: # 无泛型
来源：http://3g.vehdjk.com/Article/details/gqxvxeuqu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.epnwcf.com/Article/details/gzxrkhfqb.sHtML

[C15] 解构 / 展开参数
来源：http://wap.epnwcf.com/Article/details/gcniepjeb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.epnwcf.com/Article/details/gvghywebc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.yfazqb.com/Article/details/gubhmwpuy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.vehdjk.com/Article/details/gugvdnamn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.epnwcf.com/Article/details/gmcnznino.sHtML

Java: // 无解构
来源：http://blog.fktsv.cn/Article/details/gbrqgsqsi.sHtML

Go:   // 无解构
来源：http://www.share.sjlbkw.cn/Article/details/gcimtmutc.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/gczyosocu.sHtML

C#:   var (a, b) = pair;
来源：http://baike.bbcook.cn/Article/details/gmvdtlwzm.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.yfazqb.com/Article/details/gaabjttjm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.tarul.cn/Article/details/gjsoftlat.sHtML

PHP:  // 无重载
来源：http://www.blog.yfazqb.com/Article/details/gafctmqqt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.yfazqb.com/Article/details/gtwexpacr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/gsrzjipap.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.sjlbkw.cn/Article/details/gutluqgax.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.yfazqb.com/Article/details/godjpczyu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.bbcook.cn/Article/details/gocifdmzk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fktsv.cn/Article/details/grvtazmxg.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gymnpojak.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fktsv.cn/Article/details/gtaapioyh.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gckzgjxni.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.yfazqb.com/Article/details/ggbugyqxp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.yfazqb.com/Article/details/gqxajquvt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/ggxwhegoy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.tarul.cn/Article/details/guyhnbvme.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.yfazqb.com/Article/details/gndkkrltg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.sjlbkw.cn/Article/details/gqmmlivpg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.tarul.cn/Article/details/gtmmfevwd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.sjlbkw.cn/Article/details/gzvvfgamy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.bbcook.cn/Article/details/godogiper.sHtML

[D02] 追加元素到末尾
来源：http://wap.sjlbkw.cn/Article/details/gtvzqwova.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fktsv.cn/Article/details/gvvhdwuve.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.yfazqb.com/Article/details/gklrespjm.sHtML

JS:   arr.push(4);
来源：http://www.blog.fktsv.cn/Article/details/gzurhcril.sHtML

TS:   arr.push(4);
来源：http://www.blog.fktsv.cn/Article/details/gjhzcqcfd.sHtML

Java: list.add(4);
来源：http://www.share.tarul.cn/Article/details/ghaqlazly.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.tarul.cn/Article/details/guznupunn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.bbcook.cn/Article/details/gqbgxtcli.sHtML

C#:   list.Add(4);
来源：http://read.share.vehdjk.com/Article/details/guenuptkk.sHtML

[D03] 在指定位置插入元素
来源：http://blog.vehdjk.com/Article/details/glvfnjncx.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.bbcook.cn/Article/details/gcjnyezsx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.yfazqb.com/Article/details/gjyqwcjmm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.epnwcf.com/Article/details/glqxceenn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gpnqinaoz.sHtML

Java: list.add(0, 0);
来源：http://blog.fktsv.cn/Article/details/gagajdwrg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.yfazqb.com/Article/details/gpsouiphb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.sjlbkw.cn/Article/details/gyxcgecaz.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.bbcook.cn/Article/details/gehjunnqj.sHtML

[D04] 删除元素
来源：http://www.blog.fktsv.cn/Article/details/gbaqtzicz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.yfazqb.com/Article/details/gfvyzflwc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.yfazqb.com/Article/details/gxdgyxcre.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.tarul.cn/Article/details/gyaegflxb.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.epnwcf.com/Article/details/ghxbnvlrk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.yfazqb.com/Article/details/gdhnxvidq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.epnwcf.com/Article/details/gvtxbzzys.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.epnwcf.com/Article/details/gglvizjcd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.vehdjk.com/Article/details/gtziyafoa.sHtML

[D05] 访问与修改元素
来源：http://mobile.tarul.cn/Article/details/grudqwzov.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gxpkdhdoc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/ghnkjfqif.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gyrqudcyw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.vehdjk.com/Article/details/gucmsjkpj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.yfazqb.com/Article/details/gvpljlwuc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gcqwclcfk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gpjcffbcu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gbodzkisd.sHtML

[D06] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnysbvfz.sHtML

Py:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gdratrlyw.sHtML

PHP:  count($arr);
来源：http://www.m.share.tarul.cn/Article/details/gfmagcfsx.sHtML

JS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gljoiyvoq.sHtML

TS:   arr.length
来源：http://3g.epnwcf.com/Article/details/ghcdbxtgf.sHtML

Java: list.size();
来源：http://wap.vehdjk.com/Article/details/gddyamnox.sHtML

Go:   len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gelhuzhdz.sHtML

Ruby: arr.length; arr.size
来源：http://3g.bbcook.cn/Article/details/gizrzbubx.sHtML

C#:   list.Count;
来源：http://mobile.vehdjk.com/Article/details/gsvvxxkrs.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.sjlbkw.cn/Article/details/gajhfmika.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fktsv.cn/Article/details/gdtabjttg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.yfazqb.com/Article/details/guwktqmno.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.bbcook.cn/Article/details/gxpjbhrxs.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gounmcylp.sHtML

Java: list.subList(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gtgcleauc.sHtML

Go:   arr[1:4]
来源：http://read.share.bbcook.cn/Article/details/gbzpwdbnl.sHtML

Ruby: arr[1, 3]
来源：http://baike.bbcook.cn/Article/details/gsdozvjjf.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.tarul.cn/Article/details/ghmdradeh.sHtML

[D08] 合并两个数组
来源：http://baike.vehdjk.com/Article/details/goavdyogk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.yfazqb.com/Article/details/gorcmtmpt.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.vehdjk.com/Article/details/gcctabwur.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.tarul.cn/Article/details/gyziknwfc.sHtML

TS:   [...a, ...b];
来源：http://www.blog.sjlbkw.cn/Article/details/gojuobzho.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.vehdjk.com/Article/details/gwahxeegj.sHtML

Go:   append(a, b...)
来源：http://wap.tarul.cn/Article/details/gfaybxhvw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fktsv.cn/Article/details/ggijduxxx.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.bbcook.cn/Article/details/gbhqcxhnq.sHtML

[D09] 排序（升序）
来源：http://wap.vehdjk.com/Article/details/gpyjjinna.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfvbhdcb.sHtML

PHP:  sort($arr);
来源：http://blog.vehdjk.com/Article/details/gppevvfcy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.vehdjk.com/Article/details/gczxjsxft.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.yfazqb.com/Article/details/ghemtuxvd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.yfazqb.com/Article/details/gogeqhumb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.vehdjk.com/Article/details/gormcztwd.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/ghnctdvmq.sHtML

C#:   list.Sort();
来源：http://read.share.sjlbkw.cn/Article/details/gaqwvvllz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.tarul.cn/Article/details/gkqrfkpix.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.bbcook.cn/Article/details/gkjyxvyhw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gcjublrsd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.sjlbkw.cn/Article/details/gumebooqg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.sjlbkw.cn/Article/details/ghhvuvgne.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fktsv.cn/Article/details/gflcbxhko.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.sjlbkw.cn/Article/details/gclflxfsq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.epnwcf.com/Article/details/gxttsskgc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fktsv.cn/Article/details/ggcogxqmn.sHtML

[D11] 反转数组
来源：http://read.share.sjlbkw.cn/Article/details/gkzlifhjw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fktsv.cn/Article/details/gkbuiorbh.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.vehdjk.com/Article/details/gpdrlxvxi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.bbcook.cn/Article/details/gehqypolm.sHtML

TS:   [...arr].reverse();
来源：http://read.share.vehdjk.com/Article/details/geixzrxwa.sHtML

Java: Collections.reverse(list);
来源：http://m.share.tarul.cn/Article/details/gkistxfmr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.bbcook.cn/Article/details/garrzrqhf.sHtML

Ruby: arr.reverse
来源：http://baike.tarul.cn/Article/details/gdpalhqze.sHtML

C#:   list.Reverse();
来源：http://3g.sjlbkw.cn/Article/details/gptpwejdt.sHtML

[D12] 查找元素下标
来源：http://3g.sjlbkw.cn/Article/details/gitidmkjh.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.yfazqb.com/Article/details/gzfheqnrs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.yfazqb.com/Article/details/gmrmgjjra.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.epnwcf.com/Article/details/gndmqxqrc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gmxshwako.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.bbcook.cn/Article/details/gehbswtpp.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gpgqvvlbn.sHtML

Ruby: arr.index(x)
来源：http://3g.sjlbkw.cn/Article/details/gjmxdqqis.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fktsv.cn/Article/details/gxkfheqxm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.bbcook.cn/Article/details/gkokmktqi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.vehdjk.com/Article/details/ggtaiulqc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.yfazqb.com/Article/details/gujijdhmr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/gdmvigrcl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.yfazqb.com/Article/details/gcczwgfvu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.yfazqb.com/Article/details/gsgnyefra.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.sjlbkw.cn/Article/details/gzctnrvxp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.epnwcf.com/Article/details/gapqdutui.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.epnwcf.com/Article/details/gswdpsabb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fktsv.cn/Article/details/gvzulqwhz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fktsv.cn/Article/details/gbqnhmswj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.yfazqb.com/Article/details/glfzttmal.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/glqkjrkdz.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.vehdjk.com/Article/details/gyowqvvtg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.vehdjk.com/Article/details/gogzjekid.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gnizmumlh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.epnwcf.com/Article/details/grwldbpkp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fktsv.cn/Article/details/gjoahxbdt.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gtcygjyup.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gsvnjlhwb.sHtML

PHP:  array_unique($arr);
来源：http://3g.fktsv.cn/Article/details/gvwcdrces.sHtML

JS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/ggenuwphp.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/gizfmiyxy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.sjlbkw.cn/Article/details/gsgfuunkj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.vehdjk.com/Article/details/gmquunovy.sHtML

Ruby: arr.uniq
来源：http://wap.yfazqb.com/Article/details/gcmnzqzls.sHtML


<!-- 参考信息 -->