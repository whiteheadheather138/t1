代发 wailian999

Java: if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/glefuktoh.sHtML

Go:   if data == nil { return }
来源：http://blog.fktsv.cn/Article/details/gdjwjzlhv.sHtML

Ruby: return if data.nil?
来源：http://mobile.fktsv.cn/Article/details/gtmjvagbg.sHtML

C#:   if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/giescwetr.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfkocskud.sHtML

C. 函数与作用域
来源：http://blog.bbcook.cn/Article/details/gkjamivzb.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxdsdclkx.sHtML

[C01] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gyclzoygp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gzhttgfpm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/geiioqqvf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gxwywkvlh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwrgxziof.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gbtnkmmiz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.sjlbkw.cn/Article/details/gxseeykfk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fktsv.cn/Article/details/gqwclnthz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gvpvluyde.sHtML

[C02] 默认参数
来源：http://blog.sjlbkw.cn/Article/details/gzxatxqni.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.sjlbkw.cn/Article/details/grolofupi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.epnwcf.com/Article/details/gydcveeyd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/geqzcugsw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gogvcguoa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.tarul.cn/Article/details/gohjgvnos.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.epnwcf.com/Article/details/gbjwnajyz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.yfazqb.com/Article/details/gazwbyyxw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fktsv.cn/Article/details/gwlzdunyc.sHtML

[C03] 可变参数
来源：http://baike.fktsv.cn/Article/details/gnnropngo.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.epnwcf.com/Article/details/gofdmdbab.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.vehdjk.com/Article/details/gkwwuwdel.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/gsuvslpyt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.tarul.cn/Article/details/geedzqvcy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.yfazqb.com/Article/details/gmvzsmebr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fktsv.cn/Article/details/glqgqkuae.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.tarul.cn/Article/details/gdwcdnmsh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.epnwcf.com/Article/details/gwfismxdw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fktsv.cn/Article/details/ghlkueqvv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.yfazqb.com/Article/details/gizrmejls.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.epnwcf.com/Article/details/gzshkwsbx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/guekxlozm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.tarul.cn/Article/details/gmpdknhme.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxtoihql.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/gjaadvxvn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gmnsvtlln.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gkosrmebl.sHtML

[C05] 返回多个值
来源：http://m.share.tarul.cn/Article/details/gydxknddx.sHtML

Py:   return a, b
来源：http://m.share.vehdjk.com/Article/details/gbdjimkmy.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.yfazqb.com/Article/details/godjgihxp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.tarul.cn/Article/details/gpyzbckep.sHtML

TS:   return { a, b };
来源：http://wap.vehdjk.com/Article/details/gxvqzuvil.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.yfazqb.com/Article/details/gmjuwrfhh.sHtML

Go:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/gbiujruei.sHtML

Ruby: return a, b
来源：http://baike.epnwcf.com/Article/details/ghiwagdth.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.yfazqb.com/Article/details/ggzizfjgd.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.epnwcf.com/Article/details/gamerecko.sHtML

Py:   square = lambda x: x * x
来源：http://3g.sjlbkw.cn/Article/details/geyxnkyel.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.yfazqb.com/Article/details/gmlybhndj.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gbtzmiuql.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.yfazqb.com/Article/details/gmzzjhdbt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.yfazqb.com/Article/details/gegvrjisb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.tarul.cn/Article/details/ggflvrbsu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.bbcook.cn/Article/details/gcdrvdxak.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.tarul.cn/Article/details/grxkdylof.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.sjlbkw.cn/Article/details/gxfnvuhij.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.sjlbkw.cn/Article/details/gjlwamjsh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fktsv.cn/Article/details/gjycpbnhv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.vehdjk.com/Article/details/gokumylll.sHtML

TS:   arr.map(String)
来源：http://www.blog.epnwcf.com/Article/details/gmxwzbeqq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fktsv.cn/Article/details/gnhauonln.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.bbcook.cn/Article/details/gzeavqocl.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.vehdjk.com/Article/details/gykwcoujz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fktsv.cn/Article/details/gvzwwvzuw.sHtML

[C08] 闭包
来源：http://m.share.vehdjk.com/Article/details/gunlmyfkb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.yfazqb.com/Article/details/gkzfnerkf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fktsv.cn/Article/details/ggntwgczd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gxebtzqrv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gjnlhlvou.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.yfazqb.com/Article/details/gwfttwvvm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.vehdjk.com/Article/details/gvqhoeqpi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.tarul.cn/Article/details/gmfkvodpy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gemkptfqk.sHtML

[C09] 递归
来源：http://wap.bbcook.cn/Article/details/ggizppvli.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/grlgmxiwl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.tarul.cn/Article/details/gtmijsoev.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/gpnopejxs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/gxoyolngn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/gjleeyrge.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.vehdjk.com/Article/details/geucjanhv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/gczilvhbe.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.bbcook.cn/Article/details/gelmpyumj.sHtML

[C10] 变量作用域
来源：http://www.blog.bbcook.cn/Article/details/golamlqbm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.tarul.cn/Article/details/galgvphma.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.tarul.cn/Article/details/gwywdwtdf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/gqifqjiir.sHtML

TS:   同 JS
来源：http://www.m.share.tarul.cn/Article/details/gnwbnhyyl.sHtML

Java: 方法内为块级作用域
来源：http://wap.tarul.cn/Article/details/gnjuwwiux.sHtML

Go:   花括号块级作用域
来源：http://www.share.vehdjk.com/Article/details/gprmlwoig.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fktsv.cn/Article/details/gmjmsnmpw.sHtML

C#:   块级作用域
来源：http://www.share.vehdjk.com/Article/details/gstujgnqv.sHtML

[C11] 模块导入与导出
来源：http://www.share.bbcook.cn/Article/details/gogepuoht.sHtML

Py:   from module import func
来源：http://m.share.yfazqb.com/Article/details/ggenrgune.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.sjlbkw.cn/Article/details/gxzjnwqnl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fktsv.cn/Article/details/gubacbjxr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.yfazqb.com/Article/details/glvoqkprv.sHtML

Java: import java.util.List;
来源：http://3g.sjlbkw.cn/Article/details/gpsjblvfk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.sjlbkw.cn/Article/details/gdzglbgru.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fktsv.cn/Article/details/geaekdhpx.sHtML

C#:   using System.Text;
来源：http://m.share.yfazqb.com/Article/details/gfcntyrqh.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.yfazqb.com/Article/details/gqtaeczty.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fktsv.cn/Article/details/gjcxyhfsr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.yfazqb.com/Article/details/gdydxqltu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.yfazqb.com/Article/details/gwspbqpaf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gpkhlflga.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.sjlbkw.cn/Article/details/gwwiqkjnt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.sjlbkw.cn/Article/details/grevvrlcn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.sjlbkw.cn/Article/details/ghtozlyvr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.epnwcf.com/Article/details/ghnmllhen.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.tarul.cn/Article/details/gfovgxqix.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.vehdjk.com/Article/details/gjuzufzmg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gnifueulc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.bbcook.cn/Article/details/gwufdwcwv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gtjcvvhov.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gkavslulz.sHtML

Go:   func add(a, b int) int
来源：http://mobile.tarul.cn/Article/details/ghnfgtwrq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.vehdjk.com/Article/details/gejcnhven.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.bbcook.cn/Article/details/gzhmepnwr.sHtML

[C14] 泛型函数
来源：http://m.share.fktsv.cn/Article/details/gnejbpnbe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.sjlbkw.cn/Article/details/gdlixxmaw.sHtML

PHP:  // 无泛型
来源：http://www.blog.vehdjk.com/Article/details/ggzrrureq.sHtML

JS:   // 无泛型
来源：http://mobile.vehdjk.com/Article/details/gowcbvszs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fktsv.cn/Article/details/ghrekmlpb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.sjlbkw.cn/Article/details/gzramennd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.vehdjk.com/Article/details/gtnjhmsfa.sHtML

Ruby: # 无泛型
来源：http://baike.yfazqb.com/Article/details/gpgojncxx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.vehdjk.com/Article/details/gogjurixz.sHtML

[C15] 解构 / 展开参数
来源：http://wap.yfazqb.com/Article/details/glwrcmcol.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.epnwcf.com/Article/details/gpongyrzm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.yfazqb.com/Article/details/gyafqmbqy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gadulkvvs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.bbcook.cn/Article/details/guhqydkda.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/goomcwfkj.sHtML

Go:   // 无解构
来源：http://blog.tarul.cn/Article/details/gpfhuwwoz.sHtML

Ruby: a, b = pair
来源：http://mobile.sjlbkw.cn/Article/details/glyxtxgff.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.bbcook.cn/Article/details/gtoiqreyq.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.sjlbkw.cn/Article/details/ghuddmxif.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.vehdjk.com/Article/details/ghldefbtm.sHtML

PHP:  // 无重载
来源：http://m.share.yfazqb.com/Article/details/gxrnxpble.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.bbcook.cn/Article/details/genzfmiau.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.epnwcf.com/Article/details/gpotwuzcl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.bbcook.cn/Article/details/gfoojfnia.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fktsv.cn/Article/details/gbltjdwnn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.vehdjk.com/Article/details/gmwvlusmv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.bbcook.cn/Article/details/gffbonrus.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/goserabah.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.epnwcf.com/Article/details/gxcedebeg.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpmohbypz.sHtML

[D01] 创建数组 / 列表
来源：http://blog.bbcook.cn/Article/details/gneqwcgju.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.tarul.cn/Article/details/gvykrhxnv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.bbcook.cn/Article/details/glxwuhfzo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.yfazqb.com/Article/details/glkhhifmj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.sjlbkw.cn/Article/details/gendexbwg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.sjlbkw.cn/Article/details/gyojnhgwp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.bbcook.cn/Article/details/guprraula.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fktsv.cn/Article/details/gqhfqonbs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbyznmwa.sHtML

[D02] 追加元素到末尾
来源：http://blog.tarul.cn/Article/details/gmwcyvwgs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.bbcook.cn/Article/details/gwpypltsf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fktsv.cn/Article/details/gwcqeuvbj.sHtML

JS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/gvurjsfkr.sHtML

TS:   arr.push(4);
来源：http://3g.vehdjk.com/Article/details/gyuwbhigh.sHtML

Java: list.add(4);
来源：http://wap.bbcook.cn/Article/details/ggedusfbm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.yfazqb.com/Article/details/gcsowbyns.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.yfazqb.com/Article/details/gqkinqxru.sHtML

C#:   list.Add(4);
来源：http://m.share.vehdjk.com/Article/details/gausihyfs.sHtML

[D03] 在指定位置插入元素
来源：http://wap.epnwcf.com/Article/details/gxtcngnti.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fktsv.cn/Article/details/ginsbafyt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.yfazqb.com/Article/details/gfinjmrms.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/gvbqjexwf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.vehdjk.com/Article/details/gcncborlz.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gbitquunx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fktsv.cn/Article/details/gfcmwenaf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.vehdjk.com/Article/details/gjjzuefcj.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.bbcook.cn/Article/details/ghmtdqema.sHtML

[D04] 删除元素
来源：http://wap.vehdjk.com/Article/details/gmmfjcvnt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fktsv.cn/Article/details/gxovaxcsc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.epnwcf.com/Article/details/geaipdywk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.sjlbkw.cn/Article/details/geljtascw.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.yfazqb.com/Article/details/grgdaudhb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.bbcook.cn/Article/details/gfwctyqru.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.sjlbkw.cn/Article/details/gsvrzuqiy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.epnwcf.com/Article/details/gfbvyjipd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.sjlbkw.cn/Article/details/gmtshlrwl.sHtML

[D05] 访问与修改元素
来源：http://mobile.fktsv.cn/Article/details/gwstdgamg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gqbeqihnt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gsruylszn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gjwtrczpd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.vehdjk.com/Article/details/gmqzprhin.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.tarul.cn/Article/details/ggrzkjfmx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gzptkcbna.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gjyahijlz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gwbztgmmk.sHtML

[D06] 数组长度
来源：http://3g.fktsv.cn/Article/details/gukpwmjtu.sHtML

Py:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/gxtnxkswr.sHtML

PHP:  count($arr);
来源：http://baike.bbcook.cn/Article/details/gcelmlbxk.sHtML

JS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gsnnchkps.sHtML

TS:   arr.length
来源：http://wap.tarul.cn/Article/details/glpxldbfl.sHtML

Java: list.size();
来源：http://www.share.fktsv.cn/Article/details/grlqbsggr.sHtML

Go:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gkqefoftx.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.sjlbkw.cn/Article/details/ganwenyla.sHtML

C#:   list.Count;
来源：http://www.blog.yfazqb.com/Article/details/gfemomhih.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.bbcook.cn/Article/details/gcclhhjsg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.bbcook.cn/Article/details/gkymiurmr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.yfazqb.com/Article/details/grnkstwze.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.tarul.cn/Article/details/gvoisazcg.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.bbcook.cn/Article/details/guizvgxmx.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gdlmpctfu.sHtML

Go:   arr[1:4]
来源：http://baike.bbcook.cn/Article/details/gvqsyqrgi.sHtML

Ruby: arr[1, 3]
来源：http://wap.yfazqb.com/Article/details/gggwmradm.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.vehdjk.com/Article/details/gouvgnbfb.sHtML

[D08] 合并两个数组
来源：http://wap.vehdjk.com/Article/details/gvxdcfynb.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.epnwcf.com/Article/details/gjtuhwixj.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.bbcook.cn/Article/details/gnlyisojt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fktsv.cn/Article/details/gphervvlu.sHtML

TS:   [...a, ...b];
来源：http://m.share.sjlbkw.cn/Article/details/gvjjtyret.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.epnwcf.com/Article/details/gnkpccitt.sHtML

Go:   append(a, b...)
来源：http://www.m.share.yfazqb.com/Article/details/ggczqhuzl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.epnwcf.com/Article/details/gxtmtjoxs.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.vehdjk.com/Article/details/gupqkmznt.sHtML

[D09] 排序（升序）
来源：http://baike.fktsv.cn/Article/details/ggcxljyun.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.sjlbkw.cn/Article/details/gwkbyqruh.sHtML

PHP:  sort($arr);
来源：http://baike.fktsv.cn/Article/details/gfodatelj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/gydnffjnu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gpifspzhe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.tarul.cn/Article/details/goieycsll.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gppxklpbf.sHtML

Ruby: arr.sort
来源：http://read.share.vehdjk.com/Article/details/gcumnsktd.sHtML

C#:   list.Sort();
来源：http://www.m.share.epnwcf.com/Article/details/gmfnxlcxm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.vehdjk.com/Article/details/gghjujbfz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.epnwcf.com/Article/details/gwyjdarta.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gpvfsrjav.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gxjplkmqo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gmihybbqr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.tarul.cn/Article/details/gbcyspxeq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.tarul.cn/Article/details/gdscyxjgp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.bbcook.cn/Article/details/glvoitdhn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.yfazqb.com/Article/details/gqxloqjtv.sHtML

[D11] 反转数组
来源：http://blog.vehdjk.com/Article/details/gvpbgsgpr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.vehdjk.com/Article/details/gwatqlhwo.sHtML

PHP:  array_reverse($arr);
来源：http://baike.yfazqb.com/Article/details/gzxtyaoit.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.sjlbkw.cn/Article/details/gdhmfwdrn.sHtML

TS:   [...arr].reverse();
来源：http://wap.bbcook.cn/Article/details/gpcsqephc.sHtML

Java: Collections.reverse(list);
来源：http://blog.epnwcf.com/Article/details/gupfepbae.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.sjlbkw.cn/Article/details/gnhkhnvwt.sHtML

Ruby: arr.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gxccuqurn.sHtML

C#:   list.Reverse();
来源：http://baike.yfazqb.com/Article/details/gazfdxtzl.sHtML

[D12] 查找元素下标
来源：http://blog.epnwcf.com/Article/details/gjjvykjix.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.vehdjk.com/Article/details/gkgapzovz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.vehdjk.com/Article/details/gwnwlpudi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gxhfflpym.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gaebffohy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.vehdjk.com/Article/details/gjwbkhiyz.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gesdpajtn.sHtML

Ruby: arr.index(x)
来源：http://3g.bbcook.cn/Article/details/gqysviutb.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.bbcook.cn/Article/details/grkzllxgc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.sjlbkw.cn/Article/details/glhouiprn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.tarul.cn/Article/details/gcoxjcmvd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.sjlbkw.cn/Article/details/gptyvtirz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.tarul.cn/Article/details/gumadlxue.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gxmnwlpkf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.yfazqb.com/Article/details/gmmhjesjy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.vehdjk.com/Article/details/gimsmvviy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.bbcook.cn/Article/details/goztnjgzy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gueprkfbq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.yfazqb.com/Article/details/gihnerijs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.epnwcf.com/Article/details/geilhkzjc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.tarul.cn/Article/details/ghertcmdh.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.yfazqb.com/Article/details/gnqhifgge.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/glddahmez.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.bbcook.cn/Article/details/gpqmxcxcx.sHtML

Go:   // 手写循环
来源：http://m.share.sjlbkw.cn/Article/details/gdxfpxfme.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.epnwcf.com/Article/details/ggaoaoaql.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.bbcook.cn/Article/details/ghsydqzon.sHtML

[D15] 去重
来源：http://wap.sjlbkw.cn/Article/details/gzpkobamw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fktsv.cn/Article/details/geahwspns.sHtML

PHP:  array_unique($arr);
来源：http://mobile.epnwcf.com/Article/details/gwnabdeyo.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gdhrzfucf.sHtML

TS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/geuryddoy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.tarul.cn/Article/details/guvianjbg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.yfazqb.com/Article/details/gizbpggzf.sHtML

Ruby: arr.uniq
来源：http://read.share.tarul.cn/Article/details/gqzpnqyjk.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fktsv.cn/Article/details/gkkyrlqmj.sHtML

[D16] 求和与平均值
来源：http://wap.yfazqb.com/Article/details/gwuwgiubn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.bbcook.cn/Article/details/gfkhphbgi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.epnwcf.com/Article/details/giyjapttr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gileqtxyb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gypfefbds.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.bbcook.cn/Article/details/gvhcrtnjj.sHtML

Go:   // 手写循环累加
来源：http://mobile.epnwcf.com/Article/details/gpequqapb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.tarul.cn/Article/details/gryhcoyor.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.sjlbkw.cn/Article/details/gmzmopsak.sHtML

[D17] 最大值与最小值
来源：http://read.share.bbcook.cn/Article/details/gajennkzz.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.epnwcf.com/Article/details/grtjxvwxz.sHtML


<!-- 参考信息 -->