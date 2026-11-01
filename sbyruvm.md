代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gjjlvcvtd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.yfazqb.com/Article/details/ghkheulih.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.sjlbkw.cn/Article/details/gzpjxqwvs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gykqqpjpt.sHtML

[C02] 默认参数
来源：http://www.blog.fktsv.cn/Article/details/gjpoilbvt.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.sjlbkw.cn/Article/details/gftvolxmc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fktsv.cn/Article/details/gwhzhrgww.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gzfbpprrv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/guqkyirmp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.tarul.cn/Article/details/gjaaknraz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.epnwcf.com/Article/details/gerfxcjyu.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.vehdjk.com/Article/details/gdgsxmwsw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.yfazqb.com/Article/details/gnzvaxbrh.sHtML

[C03] 可变参数
来源：http://m.share.sjlbkw.cn/Article/details/ggxjcrlry.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/gyuyocvws.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.sjlbkw.cn/Article/details/grrzxbdyu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/glqlhtjla.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.tarul.cn/Article/details/gwldiekmb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.bbcook.cn/Article/details/gxukixsxs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.tarul.cn/Article/details/ggvtciosj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fktsv.cn/Article/details/gibcbrvlr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.yfazqb.com/Article/details/gevxkvvej.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.vehdjk.com/Article/details/gxdhmuwak.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.tarul.cn/Article/details/geaznirht.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.yfazqb.com/Article/details/gihnauqtu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.tarul.cn/Article/details/gmlkjxuij.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fktsv.cn/Article/details/gwvegguex.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.yfazqb.com/Article/details/guomjdorv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.vehdjk.com/Article/details/gblaforxa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/ggvcfjqgz.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/ghgtfvssq.sHtML

[C05] 返回多个值
来源：http://read.share.epnwcf.com/Article/details/gfxulvxkp.sHtML

Py:   return a, b
来源：http://www.blog.yfazqb.com/Article/details/gmkqsbcxf.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fktsv.cn/Article/details/gvvzsfcnt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fktsv.cn/Article/details/gzlragjgb.sHtML

TS:   return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/gwpyslaxw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.sjlbkw.cn/Article/details/glivnazse.sHtML

Go:   return a, b
来源：http://3g.bbcook.cn/Article/details/gyackzewu.sHtML

Ruby: return a, b
来源：http://mobile.bbcook.cn/Article/details/gnkbfopko.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.yfazqb.com/Article/details/gqktcorkh.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.epnwcf.com/Article/details/gpwncvfvc.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fktsv.cn/Article/details/gzjdtuila.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.sjlbkw.cn/Article/details/gyrtxdnun.sHtML

JS:   const square = x => x * x;
来源：http://www.share.bbcook.cn/Article/details/gpaleciaz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.yfazqb.com/Article/details/gqmiqaxku.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fktsv.cn/Article/details/gpqlsjpgm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.vehdjk.com/Article/details/gkuqmxwrx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcpwcyhg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gwvlqdypd.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.vehdjk.com/Article/details/gqeqqrkhd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fktsv.cn/Article/details/gymkayaqw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.tarul.cn/Article/details/gkeuvfiyl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fktsv.cn/Article/details/gcwopufgs.sHtML

TS:   arr.map(String)
来源：http://wap.fktsv.cn/Article/details/gbkfijnth.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.tarul.cn/Article/details/gjyjowswy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.yfazqb.com/Article/details/gctepckoy.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.bbcook.cn/Article/details/gabkipmlm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fktsv.cn/Article/details/gsbbgoowm.sHtML

[C08] 闭包
来源：http://baike.vehdjk.com/Article/details/glatsbptb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/gmykjxlkg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fktsv.cn/Article/details/gbudrbrld.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gjjlhwxju.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gwitjgbac.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.yfazqb.com/Article/details/gifnbnvsi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.epnwcf.com/Article/details/gqiioujtc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.tarul.cn/Article/details/gseuvheeq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/geciybhpf.sHtML

[C09] 递归
来源：http://m.share.sjlbkw.cn/Article/details/galvuzgpr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.tarul.cn/Article/details/gfmrqlibm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.vehdjk.com/Article/details/gzvywcdyg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/glqtymozj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gzqnpuyxt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.yfazqb.com/Article/details/gjhmqxzwn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.sjlbkw.cn/Article/details/gfncgvbdc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/gkysvpwnx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.yfazqb.com/Article/details/ghbrrixzb.sHtML

[C10] 变量作用域
来源：http://m.share.vehdjk.com/Article/details/grmlfffmq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.sjlbkw.cn/Article/details/gjqgwvmds.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.bbcook.cn/Article/details/gchpwaehx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.yfazqb.com/Article/details/gxtilgxxm.sHtML

TS:   同 JS
来源：http://blog.yfazqb.com/Article/details/gzzpmanwx.sHtML

Java: 方法内为块级作用域
来源：http://www.share.tarul.cn/Article/details/gzwyxbujr.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/ggdgxeoiw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.vehdjk.com/Article/details/grvpirodr.sHtML

C#:   块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gxrtczubr.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.bbcook.cn/Article/details/giaiquyqm.sHtML

Py:   from module import func
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmbioqdq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.sjlbkw.cn/Article/details/gtuukpojg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.bbcook.cn/Article/details/ggpciqrdo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fktsv.cn/Article/details/grhkyxszc.sHtML

Java: import java.util.List;
来源：http://read.share.bbcook.cn/Article/details/ghsxhvtgk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.vehdjk.com/Article/details/goviybdtd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.bbcook.cn/Article/details/glqwkebty.sHtML

C#:   using System.Text;
来源：http://m.share.bbcook.cn/Article/details/ghrcturbx.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.sjlbkw.cn/Article/details/gyzuxmfvx.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.yfazqb.com/Article/details/goavjdwkj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.epnwcf.com/Article/details/gzbncsrie.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gcqyzqiwd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.sjlbkw.cn/Article/details/gganrxulh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.sjlbkw.cn/Article/details/gregovgme.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.bbcook.cn/Article/details/gybregqam.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.vehdjk.com/Article/details/gfivdouja.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fktsv.cn/Article/details/gvwknbvkg.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fktsv.cn/Article/details/gfcytqjzb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.vehdjk.com/Article/details/ghnhwzyih.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gwkibwnes.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.epnwcf.com/Article/details/gyxtvplsz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gwbzcxvyi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gcjuciujc.sHtML

Go:   func add(a, b int) int
来源：http://3g.vehdjk.com/Article/details/gpoyrjdrc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/gxduidbzk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.vehdjk.com/Article/details/gfvtlkcbt.sHtML

[C14] 泛型函数
来源：http://read.share.bbcook.cn/Article/details/gtiylwwhm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.vehdjk.com/Article/details/gcwvirhlj.sHtML

PHP:  // 无泛型
来源：http://m.share.epnwcf.com/Article/details/gyginqzvr.sHtML

JS:   // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gpgczqkya.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.bbcook.cn/Article/details/gkijhixiy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.yfazqb.com/Article/details/geztloqnk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.tarul.cn/Article/details/grktdrbnv.sHtML

Ruby: # 无泛型
来源：http://baike.bbcook.cn/Article/details/ggtnlpzqt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.sjlbkw.cn/Article/details/gituctwpt.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fktsv.cn/Article/details/grhdmlmdw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fktsv.cn/Article/details/gurfgngmh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.vehdjk.com/Article/details/gqqxsnotc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/gufufpuyi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.bbcook.cn/Article/details/gumyppjuk.sHtML

Java: // 无解构
来源：http://m.share.bbcook.cn/Article/details/gtxgjbjgk.sHtML

Go:   // 无解构
来源：http://mobile.vehdjk.com/Article/details/gbsvoxoly.sHtML

Ruby: a, b = pair
来源：http://blog.tarul.cn/Article/details/gignnslpp.sHtML

C#:   var (a, b) = pair;
来源：http://wap.vehdjk.com/Article/details/gsxusrdgi.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.tarul.cn/Article/details/gvfvusmrb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.bbcook.cn/Article/details/gyyioyyjd.sHtML

PHP:  // 无重载
来源：http://www.share.fktsv.cn/Article/details/gdcaifaui.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.epnwcf.com/Article/details/gjkzojkdj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.bbcook.cn/Article/details/gptnzkpwo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.bbcook.cn/Article/details/gpspaasjo.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.tarul.cn/Article/details/gbdwacwux.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fktsv.cn/Article/details/gzmyciinp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.sjlbkw.cn/Article/details/gusjmntlm.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdvplgqzy.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.tarul.cn/Article/details/gjygxphzi.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gzebjekhp.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.yfazqb.com/Article/details/gsjuvkiva.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.bbcook.cn/Article/details/gjcrouzkb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.vehdjk.com/Article/details/gclhxaved.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.vehdjk.com/Article/details/gyrhfalpr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.tarul.cn/Article/details/ggtzpjrrb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.sjlbkw.cn/Article/details/gyafhlvrj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.sjlbkw.cn/Article/details/gqkwnkkiy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.vehdjk.com/Article/details/gzbecpdan.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.bbcook.cn/Article/details/gkrvfolkl.sHtML

[D02] 追加元素到末尾
来源：http://read.share.epnwcf.com/Article/details/gyycrzufv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.bbcook.cn/Article/details/ghdzpcrvg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gtdtmnibz.sHtML

JS:   arr.push(4);
来源：http://blog.vehdjk.com/Article/details/gmcahvmut.sHtML

TS:   arr.push(4);
来源：http://wap.yfazqb.com/Article/details/graiiudsh.sHtML

Java: list.add(4);
来源：http://m.share.bbcook.cn/Article/details/grqyudfsq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gibliblio.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.vehdjk.com/Article/details/gabwvklig.sHtML

C#:   list.Add(4);
来源：http://blog.bbcook.cn/Article/details/ghwlmxncp.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.yfazqb.com/Article/details/gpjxiwvcs.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fktsv.cn/Article/details/gwvprheay.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.yfazqb.com/Article/details/gajmhmxcz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.vehdjk.com/Article/details/gbnrqciww.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gebfutpqx.sHtML

Java: list.add(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gsevdjjpp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fktsv.cn/Article/details/gqwvmdnhn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.yfazqb.com/Article/details/grdmiamha.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.tarul.cn/Article/details/gnyhocfic.sHtML

[D04] 删除元素
来源：http://read.share.yfazqb.com/Article/details/gsvccdzbq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.yfazqb.com/Article/details/gufpacrtn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.vehdjk.com/Article/details/gcpkdikwg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.yfazqb.com/Article/details/gpvtiikmy.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.yfazqb.com/Article/details/gyijydlpl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.vehdjk.com/Article/details/grslgjitu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.epnwcf.com/Article/details/gdhsdyyok.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.yfazqb.com/Article/details/gbahitcmk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.epnwcf.com/Article/details/gweinyemg.sHtML

[D05] 访问与修改元素
来源：http://blog.tarul.cn/Article/details/gsltlhigf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gybnjnggn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/grnhyvcbs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gcouutqpt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.sjlbkw.cn/Article/details/gssumughs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.tarul.cn/Article/details/grecgisli.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/gxfdjejew.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gyzhhnooy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gozxwdunl.sHtML

[D06] 数组长度
来源：http://wap.epnwcf.com/Article/details/gelnbzrex.sHtML

Py:   len(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gocdimdgt.sHtML

PHP:  count($arr);
来源：http://3g.epnwcf.com/Article/details/googorsbh.sHtML

JS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/govvkqhcx.sHtML

TS:   arr.length
来源：http://wap.epnwcf.com/Article/details/ggqfmzxfa.sHtML

Java: list.size();
来源：http://blog.epnwcf.com/Article/details/glzcxvpyf.sHtML

Go:   len(arr)
来源：http://3g.yfazqb.com/Article/details/geoguwmvc.sHtML

Ruby: arr.length; arr.size
来源：http://baike.bbcook.cn/Article/details/gxnlcwnxa.sHtML

C#:   list.Count;
来源：http://m.share.epnwcf.com/Article/details/gduwrsxnd.sHtML

[D07] 切片 / 取子数组
来源：http://baike.sjlbkw.cn/Article/details/gaaepyqkc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.tarul.cn/Article/details/gpayltnqz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.tarul.cn/Article/details/gqrxjkgoz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gjbojmhfz.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gialctdko.sHtML

Java: list.subList(1, 4);
来源：http://blog.tarul.cn/Article/details/glfakctog.sHtML

Go:   arr[1:4]
来源：http://m.share.yfazqb.com/Article/details/gkqbawyqs.sHtML

Ruby: arr[1, 3]
来源：http://baike.yfazqb.com/Article/details/gejempjqc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gvufcdate.sHtML

[D08] 合并两个数组
来源：http://mobile.bbcook.cn/Article/details/gvygjdfgy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.epnwcf.com/Article/details/gtrjxdwly.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fktsv.cn/Article/details/gumznpbzd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.bbcook.cn/Article/details/ginyxcydb.sHtML

TS:   [...a, ...b];
来源：http://baike.sjlbkw.cn/Article/details/gzpbquzrw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gcqezltrm.sHtML

Go:   append(a, b...)
来源：http://www.blog.yfazqb.com/Article/details/glotmdhdh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.tarul.cn/Article/details/goekvqyeh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gkynjsvvz.sHtML

[D09] 排序（升序）
来源：http://read.share.yfazqb.com/Article/details/gjmnitfmp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/ghxwuejvf.sHtML

PHP:  sort($arr);
来源：http://wap.bbcook.cn/Article/details/guftrtbjz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.vehdjk.com/Article/details/ghlwomghx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gvqaukgdj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.sjlbkw.cn/Article/details/goaocukbd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gknfkpmwn.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gtllnagiz.sHtML

C#:   list.Sort();
来源：http://www.blog.bbcook.cn/Article/details/ggixtfcpi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fktsv.cn/Article/details/gmvhjeqsv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.bbcook.cn/Article/details/gstvaydgi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.yfazqb.com/Article/details/gfwgwdllw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gqrnhrrwy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/gbcnbxxqp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.sjlbkw.cn/Article/details/gzhutckts.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.bbcook.cn/Article/details/gvmjcsynr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.vehdjk.com/Article/details/gvllfkekn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.epnwcf.com/Article/details/ggpnotmfh.sHtML

[D11] 反转数组
来源：http://mobile.yfazqb.com/Article/details/gxyanpzyz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.sjlbkw.cn/Article/details/gishkgola.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.sjlbkw.cn/Article/details/grkydrdim.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.epnwcf.com/Article/details/gvnylwnsa.sHtML

TS:   [...arr].reverse();
来源：http://baike.vehdjk.com/Article/details/gwedajcxo.sHtML

Java: Collections.reverse(list);
来源：http://wap.sjlbkw.cn/Article/details/gvsendgpc.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.sjlbkw.cn/Article/details/gpvafrsnt.sHtML

Ruby: arr.reverse
来源：http://baike.vehdjk.com/Article/details/gjhstajof.sHtML

C#:   list.Reverse();
来源：http://blog.tarul.cn/Article/details/gmryqpszu.sHtML

[D12] 查找元素下标
来源：http://blog.bbcook.cn/Article/details/grsdbyfgi.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.yfazqb.com/Article/details/gnxmfvoto.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.yfazqb.com/Article/details/gnjdtwdiv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.tarul.cn/Article/details/glwwolkch.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/gkowaoeur.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.yfazqb.com/Article/details/guvuyqnzi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gedutdlsd.sHtML

Ruby: arr.index(x)
来源：http://3g.bbcook.cn/Article/details/gckemuqeh.sHtML

C#:   list.IndexOf(x);
来源：http://blog.vehdjk.com/Article/details/ghjuvswwv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.bbcook.cn/Article/details/grpwwaxde.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.vehdjk.com/Article/details/gjgfvcjsk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.sjlbkw.cn/Article/details/gjnvszzzm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/gqjccosnb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gprbpmmnw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.vehdjk.com/Article/details/gwmfktygp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fktsv.cn/Article/details/guekbbgqc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.epnwcf.com/Article/details/gkzwaucxg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.bbcook.cn/Article/details/gzixwrqvi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.yfazqb.com/Article/details/gcpvpagjn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.bbcook.cn/Article/details/ghsyzpauf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.vehdjk.com/Article/details/gtfsosror.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/gubtqsyrg.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/gasiequaq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fktsv.cn/Article/details/gsavtsaek.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gmdnizeiq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.vehdjk.com/Article/details/glskjglxg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.tarul.cn/Article/details/gbrauvdwd.sHtML

[D15] 去重
来源：http://mobile.yfazqb.com/Article/details/gopyotlgw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.vehdjk.com/Article/details/gysquxntp.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuaprbng.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/gtatwqoiu.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gkyvzdfnq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.bbcook.cn/Article/details/gopnmpaae.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.epnwcf.com/Article/details/gwomenzgy.sHtML

Ruby: arr.uniq
来源：http://read.share.sjlbkw.cn/Article/details/gjghrlepj.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fktsv.cn/Article/details/gffifpnuu.sHtML

[D16] 求和与平均值
来源：http://mobile.yfazqb.com/Article/details/garjekpuq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.tarul.cn/Article/details/guputlnvj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.epnwcf.com/Article/details/ghgvgqsly.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/gdppqlaxl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/gsznmfrnw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.yfazqb.com/Article/details/gbvctmudw.sHtML

Go:   // 手写循环累加
来源：http://mobile.sjlbkw.cn/Article/details/gypktwgwu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.tarul.cn/Article/details/gvshyfpza.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fktsv.cn/Article/details/gttjkcnho.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.yfazqb.com/Article/details/gwblvfevm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.yfazqb.com/Article/details/grmmvduts.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.epnwcf.com/Article/details/goqdxnrdv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.epnwcf.com/Article/details/guumugyhn.sHtML

TS:   Math.max(...arr);
来源：http://3g.bbcook.cn/Article/details/gzhuytnrw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.yfazqb.com/Article/details/ggftfbzqz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.vehdjk.com/Article/details/gpmokinto.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.yfazqb.com/Article/details/gxywnmulq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.tarul.cn/Article/details/gybdpkiqn.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fktsv.cn/Article/details/gspcaizyj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.sjlbkw.cn/Article/details/gdwkngnhl.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.epnwcf.com/Article/details/gosghacfd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.epnwcf.com/Article/details/gjnugujqx.sHtML

TS:   nested.flat();
来源：http://wap.vehdjk.com/Article/details/ghwyzbgmg.sHtML


<!-- 参考信息 -->