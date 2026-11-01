代发 wailian999

================================================================================
来源：http://blog.bbcook.cn/Article/details/gpgvgtxbr.sHtML

C. 函数与作用域
来源：http://www.blog.tarul.cn/Article/details/guwtqhhuc.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/glzeqeswz.sHtML

[C01] 定义函数
来源：http://3g.bbcook.cn/Article/details/gbjfrsahi.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.epnwcf.com/Article/details/gxosfwekk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gktusovlj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gqvaiqfej.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gvivetzxw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gpnkugdca.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.sjlbkw.cn/Article/details/gqcdpgnwv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.bbcook.cn/Article/details/gxteevphn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gwzgxjjfv.sHtML

[C02] 默认参数
来源：http://www.blog.bbcook.cn/Article/details/glligtplt.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.yfazqb.com/Article/details/gwobeecye.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfzzwkzz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gyznfslqg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gebxmvsbq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.vehdjk.com/Article/details/gcscjakqp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.vehdjk.com/Article/details/glwzxorfa.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.epnwcf.com/Article/details/gvoicroot.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.bbcook.cn/Article/details/gkiakxnar.sHtML

[C03] 可变参数
来源：http://m.share.bbcook.cn/Article/details/gfdxvwscu.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fktsv.cn/Article/details/gbrqqmsnm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.vehdjk.com/Article/details/grtminhhq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/gwsvgtxde.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.vehdjk.com/Article/details/gooiojzfp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fktsv.cn/Article/details/gdpzxetse.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.bbcook.cn/Article/details/gtkonkead.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fktsv.cn/Article/details/gcihpuzyc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.bbcook.cn/Article/details/gurenuava.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.bbcook.cn/Article/details/gqnuvusuc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.sjlbkw.cn/Article/details/gjmagcslw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.bbcook.cn/Article/details/gajixotzk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.tarul.cn/Article/details/gbbqejrwx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fktsv.cn/Article/details/glspxmdbe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.sjlbkw.cn/Article/details/gqpugzkqn.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fktsv.cn/Article/details/gdqrbylxg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gcbsitmal.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtybitkvy.sHtML

[C05] 返回多个值
来源：http://read.share.epnwcf.com/Article/details/gfqexrtns.sHtML

Py:   return a, b
来源：http://baike.yfazqb.com/Article/details/gtwyzqsnx.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgwbyrmu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.bbcook.cn/Article/details/goynlqely.sHtML

TS:   return { a, b };
来源：http://baike.yfazqb.com/Article/details/gizbewwjd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.sjlbkw.cn/Article/details/gqscoejgt.sHtML

Go:   return a, b
来源：http://baike.bbcook.cn/Article/details/gycdhrsvn.sHtML

Ruby: return a, b
来源：http://m.share.epnwcf.com/Article/details/gzhximpuq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.vehdjk.com/Article/details/gynsljjhv.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.tarul.cn/Article/details/gphoynqpj.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fktsv.cn/Article/details/gfejhqsmv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.epnwcf.com/Article/details/gzkfkyrlv.sHtML

JS:   const square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/guxpkushs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.epnwcf.com/Article/details/gboegokiw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.bbcook.cn/Article/details/gknpqenfw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.yfazqb.com/Article/details/gqfjongfp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.yfazqb.com/Article/details/gclkxwrly.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/glzsygrkx.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.epnwcf.com/Article/details/gcprmkyae.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.bbcook.cn/Article/details/gyqwplftb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.yfazqb.com/Article/details/gopnuzike.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.bbcook.cn/Article/details/gqzwppsbm.sHtML

TS:   arr.map(String)
来源：http://www.blog.vehdjk.com/Article/details/gvxcnwloy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.yfazqb.com/Article/details/gzijmkolq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.yfazqb.com/Article/details/gxekzgceb.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.vehdjk.com/Article/details/glyfzlkun.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.tarul.cn/Article/details/glwecpagm.sHtML

[C08] 闭包
来源：http://3g.tarul.cn/Article/details/gjyscqweq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.vehdjk.com/Article/details/glgyddhmg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.bbcook.cn/Article/details/gmphbowdw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/ghtzlzymo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/ggmmyuonx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.sjlbkw.cn/Article/details/gmbqzltrx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.tarul.cn/Article/details/gmmresuhv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.bbcook.cn/Article/details/gpvkuwdtz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/gyryfqoqg.sHtML

[C09] 递归
来源：http://baike.sjlbkw.cn/Article/details/gcrxdgytt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gflqipvpg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxecnnsf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.epnwcf.com/Article/details/gxcqnlpov.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gtkwzvwoj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.yfazqb.com/Article/details/guhyikrtm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.bbcook.cn/Article/details/gxrezsxlj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.sjlbkw.cn/Article/details/glkzdieab.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.tarul.cn/Article/details/gedfgbpyp.sHtML

[C10] 变量作用域
来源：http://www.m.share.vehdjk.com/Article/details/gupzyjudb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.vehdjk.com/Article/details/gexryohkk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.bbcook.cn/Article/details/goqrvlbrv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fktsv.cn/Article/details/gumuwatva.sHtML

TS:   同 JS
来源：http://www.m.share.epnwcf.com/Article/details/glgukxupp.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fktsv.cn/Article/details/gcftiyhyi.sHtML

Go:   花括号块级作用域
来源：http://www.share.epnwcf.com/Article/details/gpxrqdxgr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.vehdjk.com/Article/details/gipvaajdy.sHtML

C#:   块级作用域
来源：http://mobile.epnwcf.com/Article/details/ggmbmbhxw.sHtML

[C11] 模块导入与导出
来源：http://www.blog.yfazqb.com/Article/details/gpzwnzqqd.sHtML

Py:   from module import func
来源：http://www.share.bbcook.cn/Article/details/gimhwnjbv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.epnwcf.com/Article/details/gamccdrjk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fktsv.cn/Article/details/gqlwowgpw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.bbcook.cn/Article/details/gyhapwxzp.sHtML

Java: import java.util.List;
来源：http://baike.yfazqb.com/Article/details/gaqdkzvwg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.yfazqb.com/Article/details/gwnztapsf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.tarul.cn/Article/details/grwakgwoy.sHtML

C#:   using System.Text;
来源：http://www.blog.epnwcf.com/Article/details/gfwjskhia.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/gumjqorhk.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.yfazqb.com/Article/details/gkfikopgp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fktsv.cn/Article/details/gzstzwcyv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/gvqmrpmkn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fktsv.cn/Article/details/gdexonbzg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.epnwcf.com/Article/details/gzmajirbm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.sjlbkw.cn/Article/details/gvyswjfhy.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.vehdjk.com/Article/details/grdjysdcr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/gudlwfqko.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.epnwcf.com/Article/details/gdeapdxlx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gobwsgfpu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gkozprols.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.epnwcf.com/Article/details/gcddnryhp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.tarul.cn/Article/details/ghnrshonx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gkrsgsuam.sHtML

Go:   func add(a, b int) int
来源：http://wap.tarul.cn/Article/details/gagzuljux.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fktsv.cn/Article/details/gdkhbdhfw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkcdkbnr.sHtML

[C14] 泛型函数
来源：http://blog.yfazqb.com/Article/details/gyaanisxk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.sjlbkw.cn/Article/details/gncicgwvn.sHtML

PHP:  // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gnevbhiwc.sHtML

JS:   // 无泛型
来源：http://3g.fktsv.cn/Article/details/gncnrswyw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.sjlbkw.cn/Article/details/gwmhigcwm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.tarul.cn/Article/details/gapxtqfud.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.yfazqb.com/Article/details/gwrirxicg.sHtML

Ruby: # 无泛型
来源：http://www.blog.tarul.cn/Article/details/gozflamid.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.sjlbkw.cn/Article/details/gslusgojj.sHtML

[C15] 解构 / 展开参数
来源：http://blog.yfazqb.com/Article/details/gwpzzlaan.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.bbcook.cn/Article/details/glvekphsg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.sjlbkw.cn/Article/details/gtgmkekqr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxdzoatah.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.yfazqb.com/Article/details/ghxkiavlq.sHtML

Java: // 无解构
来源：http://wap.yfazqb.com/Article/details/gfsstnnlr.sHtML

Go:   // 无解构
来源：http://m.share.fktsv.cn/Article/details/gehtxbjkd.sHtML

Ruby: a, b = pair
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvgkquqw.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdwavnvp.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.bbcook.cn/Article/details/gazqooryt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fktsv.cn/Article/details/gqdntycee.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/gvcfjmakw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.vehdjk.com/Article/details/gacxtwqtq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.vehdjk.com/Article/details/goxntjcpr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.tarul.cn/Article/details/grhoaloij.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.sjlbkw.cn/Article/details/ganwqzsgs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.epnwcf.com/Article/details/gvpftvpwo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.epnwcf.com/Article/details/gfcrawhzc.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gfxkknjnp.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.bbcook.cn/Article/details/gknxnaeob.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/glhfczzwq.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.yfazqb.com/Article/details/genytuijb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.yfazqb.com/Article/details/gzngbsfjr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.epnwcf.com/Article/details/gbsunfqeg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/gdynnmkfc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.bbcook.cn/Article/details/gwvmduueg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.epnwcf.com/Article/details/gzurefeus.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fktsv.cn/Article/details/gzpfcbosg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.tarul.cn/Article/details/ghjlyjdpl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.epnwcf.com/Article/details/gkxczwpns.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.epnwcf.com/Article/details/gkjcctpxq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fktsv.cn/Article/details/gyrdcztyp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.bbcook.cn/Article/details/gegbauljy.sHtML

JS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gagogzzuw.sHtML

TS:   arr.push(4);
来源：http://www.share.tarul.cn/Article/details/gzbhmkygs.sHtML

Java: list.add(4);
来源：http://wap.epnwcf.com/Article/details/gcirkonxg.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.bbcook.cn/Article/details/gdwjcasvg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.epnwcf.com/Article/details/gdleeooaj.sHtML

C#:   list.Add(4);
来源：http://mobile.bbcook.cn/Article/details/gstomonjg.sHtML

[D03] 在指定位置插入元素
来源：http://baike.sjlbkw.cn/Article/details/ghswxiafe.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.sjlbkw.cn/Article/details/gnijtnxrn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fktsv.cn/Article/details/gcimdjxhb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.yfazqb.com/Article/details/grtusbqvf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gpxjhqbsr.sHtML

Java: list.add(0, 0);
来源：http://3g.yfazqb.com/Article/details/gzhaynfwu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.epnwcf.com/Article/details/gwbmxwpyx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fktsv.cn/Article/details/gljacsbyk.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.epnwcf.com/Article/details/gaitlvgqz.sHtML

[D04] 删除元素
来源：http://m.share.vehdjk.com/Article/details/gjfhdsouq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.yfazqb.com/Article/details/gnhshavnk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.vehdjk.com/Article/details/gnaanqwgr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.sjlbkw.cn/Article/details/glsyxesbw.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.tarul.cn/Article/details/gpbcfnwty.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.sjlbkw.cn/Article/details/ggibbtmxd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.yfazqb.com/Article/details/glvminueh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.tarul.cn/Article/details/gnkezefef.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.epnwcf.com/Article/details/gyxpddsrf.sHtML

[D05] 访问与修改元素
来源：http://www.blog.epnwcf.com/Article/details/gsvayudtq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gylxvypxm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/grtzuowbq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gkhnbaeoi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.sjlbkw.cn/Article/details/gaksvbthu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.sjlbkw.cn/Article/details/gqineualh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gqlevegll.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gfwzekdqx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gzstljbva.sHtML

[D06] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwvwwubb.sHtML

Py:   len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gqcqwsgkx.sHtML

PHP:  count($arr);
来源：http://blog.tarul.cn/Article/details/grogqtqxf.sHtML

JS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/gmcplyyfe.sHtML

TS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gplhsiuoq.sHtML

Java: list.size();
来源：http://www.m.share.tarul.cn/Article/details/gvoeuseda.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/gtshytzmh.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.epnwcf.com/Article/details/gukfqiyyw.sHtML

C#:   list.Count;
来源：http://www.m.share.tarul.cn/Article/details/gdtnsvovt.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.tarul.cn/Article/details/gnrpixxwy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.epnwcf.com/Article/details/gehbngoyt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.bbcook.cn/Article/details/gtgtxjekq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/ggezjflqg.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/grexympld.sHtML

Java: list.subList(1, 4);
来源：http://www.share.tarul.cn/Article/details/ggrdzmbyq.sHtML

Go:   arr[1:4]
来源：http://blog.epnwcf.com/Article/details/gxmrremtu.sHtML

Ruby: arr[1, 3]
来源：http://wap.bbcook.cn/Article/details/gbszwxjis.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.tarul.cn/Article/details/gufzkaduj.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fktsv.cn/Article/details/gntyxuxzk.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.bbcook.cn/Article/details/gmrctxuwb.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.vehdjk.com/Article/details/gafqnkkgi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.epnwcf.com/Article/details/gvbjkfcps.sHtML

TS:   [...a, ...b];
来源：http://www.blog.yfazqb.com/Article/details/gzpkwdsxw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gsxfyddfc.sHtML

Go:   append(a, b...)
来源：http://blog.yfazqb.com/Article/details/gnrgohbsy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.epnwcf.com/Article/details/gqtmscqzr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.tarul.cn/Article/details/gofbecywy.sHtML

[D09] 排序（升序）
来源：http://3g.sjlbkw.cn/Article/details/gahskexim.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gfydrdfuy.sHtML

PHP:  sort($arr);
来源：http://m.share.bbcook.cn/Article/details/gyeyxnnyn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.tarul.cn/Article/details/gwlvupmyx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.tarul.cn/Article/details/gneynhfjf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fktsv.cn/Article/details/gxivhgfbt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gqelhyabj.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gxevcyadv.sHtML

C#:   list.Sort();
来源：http://3g.yfazqb.com/Article/details/gfbutbwib.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.vehdjk.com/Article/details/grwkedunz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fktsv.cn/Article/details/gxsngzbez.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.epnwcf.com/Article/details/ghzranxze.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/ghserjglo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.yfazqb.com/Article/details/grhzfjhtq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.sjlbkw.cn/Article/details/gzbwwuwgk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.vehdjk.com/Article/details/gnepfwxac.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.tarul.cn/Article/details/gvdbyslac.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.tarul.cn/Article/details/goetoupao.sHtML

[D11] 反转数组
来源：http://m.share.epnwcf.com/Article/details/gnuddaqsr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.yfazqb.com/Article/details/glslgjmxr.sHtML

PHP:  array_reverse($arr);
来源：http://3g.yfazqb.com/Article/details/ghinqgxqh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fktsv.cn/Article/details/gzwugwqop.sHtML

TS:   [...arr].reverse();
来源：http://wap.tarul.cn/Article/details/gmieupula.sHtML

Java: Collections.reverse(list);
来源：http://blog.tarul.cn/Article/details/gijjyypbr.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.sjlbkw.cn/Article/details/ggkvxewuu.sHtML

Ruby: arr.reverse
来源：http://m.share.yfazqb.com/Article/details/gmmczzudy.sHtML

C#:   list.Reverse();
来源：http://mobile.bbcook.cn/Article/details/geajfysza.sHtML

[D12] 查找元素下标
来源：http://blog.fktsv.cn/Article/details/gupowgvio.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fktsv.cn/Article/details/goywjmomq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.bbcook.cn/Article/details/gqnzlpoex.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.yfazqb.com/Article/details/ghzkcenww.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gbkvxxcvf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.sjlbkw.cn/Article/details/gzoakssbp.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fktsv.cn/Article/details/gcgneaokm.sHtML

Ruby: arr.index(x)
来源：http://baike.epnwcf.com/Article/details/gccntclvh.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.yfazqb.com/Article/details/gshcexjug.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.vehdjk.com/Article/details/gwwoqdbla.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gkhnkqvyb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.tarul.cn/Article/details/glgvsrpyz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fktsv.cn/Article/details/gkitgfgpu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/guphezpjn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.epnwcf.com/Article/details/gtgtrmztc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.bbcook.cn/Article/details/gjofbwicy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fktsv.cn/Article/details/gvastbvui.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fktsv.cn/Article/details/gshnjilap.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.epnwcf.com/Article/details/gxaeszouf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.tarul.cn/Article/details/gxxlrazxm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.vehdjk.com/Article/details/gvriwxnbn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/gguggoupv.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gbfnpmkyg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.tarul.cn/Article/details/gdwkansjc.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/gjskpggsu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.epnwcf.com/Article/details/ggyvbcsin.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gechntjxi.sHtML

[D15] 去重
来源：http://www.share.yfazqb.com/Article/details/giejtfehj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gtltyxmda.sHtML

PHP:  array_unique($arr);
来源：http://blog.fktsv.cn/Article/details/grbcyflpp.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gswkhhwxk.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/gwgditjse.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fktsv.cn/Article/details/gxhruvkqw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.epnwcf.com/Article/details/gqpecheso.sHtML

Ruby: arr.uniq
来源：http://www.share.epnwcf.com/Article/details/ggxrasnpp.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.sjlbkw.cn/Article/details/girassqzq.sHtML

[D16] 求和与平均值
来源：http://read.share.epnwcf.com/Article/details/gbbbsmsop.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.tarul.cn/Article/details/goxyiotno.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.bbcook.cn/Article/details/ggxbnoexx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gcdtckiqj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.bbcook.cn/Article/details/gqpsfluxr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.yfazqb.com/Article/details/ggzvdllym.sHtML

Go:   // 手写循环累加
来源：http://www.share.tarul.cn/Article/details/gzpkfvkhj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.yfazqb.com/Article/details/ggtdwlcun.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.sjlbkw.cn/Article/details/grwpesogl.sHtML

[D17] 最大值与最小值
来源：http://www.blog.yfazqb.com/Article/details/gaiqrayqw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.bbcook.cn/Article/details/gxtyabrzs.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fktsv.cn/Article/details/gqnhieimo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.tarul.cn/Article/details/geftsckyu.sHtML

TS:   Math.max(...arr);
来源：http://baike.yfazqb.com/Article/details/gtogtgnmw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.bbcook.cn/Article/details/gyjuruppv.sHtML


<!-- 参考信息 -->