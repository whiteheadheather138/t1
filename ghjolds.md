代发 wailian999

Go:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gsirbcqcx.sHtML

Ruby: a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/giunurxer.sHtML

C#:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gjravqlxb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.sjlbkw.cn/Article/details/gvitmijzg.sHtML

Py:   if not data: return
来源：http://wap.tarul.cn/Article/details/goahisvel.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.bbcook.cn/Article/details/gweipofdq.sHtML

JS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/gmqpacgwg.sHtML

TS:   if (!data) return;
来源：http://www.blog.epnwcf.com/Article/details/gcntutqtc.sHtML

Java: if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/glzdydaee.sHtML

Go:   if data == nil { return }
来源：http://wap.vehdjk.com/Article/details/gljlrznnq.sHtML

Ruby: return if data.nil?
来源：http://3g.vehdjk.com/Article/details/guubwqmzo.sHtML

C#:   if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/gmfwnkavy.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmxdaheaj.sHtML

C. 函数与作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/ghudebmkx.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvemsualb.sHtML

[C01] 定义函数
来源：http://www.m.share.tarul.cn/Article/details/gwqjecloo.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fktsv.cn/Article/details/gfiurqhdb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gkmfxflps.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gxqmsunby.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gsdybdbes.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gcgqcwvdb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fktsv.cn/Article/details/gvkgtnjdb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.vehdjk.com/Article/details/gtupfnstl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/glokbxnxm.sHtML

[C02] 默认参数
来源：http://baike.epnwcf.com/Article/details/gbgyzlwll.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.epnwcf.com/Article/details/gsnlnrtme.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.bbcook.cn/Article/details/gvuvmtjii.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gktryuxxd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/geshsolwl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fktsv.cn/Article/details/gmkmokfqb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gugynafdr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.bbcook.cn/Article/details/gxvwiiyyi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fktsv.cn/Article/details/grsigzzux.sHtML

[C03] 可变参数
来源：http://www.m.share.fktsv.cn/Article/details/gitcuxlho.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fktsv.cn/Article/details/gmsbutmuc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.epnwcf.com/Article/details/gdmjtwnym.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.epnwcf.com/Article/details/gqtwoajnk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/gldxygkfx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.tarul.cn/Article/details/gdrioeuiw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.epnwcf.com/Article/details/gqkypkdvf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.epnwcf.com/Article/details/gqffabyux.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.epnwcf.com/Article/details/goibrviiy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.sjlbkw.cn/Article/details/glckuwnxr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.bbcook.cn/Article/details/gzukfecvm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.sjlbkw.cn/Article/details/gmijyccnx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.bbcook.cn/Article/details/gmipxrglw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.bbcook.cn/Article/details/gkcbmdxdx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.tarul.cn/Article/details/gebgcglzy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.vehdjk.com/Article/details/gzzexnrfo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/glhbroukg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gfvuabana.sHtML

[C05] 返回多个值
来源：http://baike.yfazqb.com/Article/details/gjzueakzo.sHtML

Py:   return a, b
来源：http://3g.epnwcf.com/Article/details/geoswixtl.sHtML

PHP:  return [$a, $b];
来源：http://blog.bbcook.cn/Article/details/gztkxqetb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.bbcook.cn/Article/details/gauhoaany.sHtML

TS:   return { a, b };
来源：http://baike.epnwcf.com/Article/details/gncwlprov.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.bbcook.cn/Article/details/grxaavifl.sHtML

Go:   return a, b
来源：http://blog.bbcook.cn/Article/details/gvskssock.sHtML

Ruby: return a, b
来源：http://mobile.vehdjk.com/Article/details/gamftbmkv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.tarul.cn/Article/details/gtxgdtsth.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.epnwcf.com/Article/details/gjiiqrxlj.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.tarul.cn/Article/details/ggkaxhwoo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.vehdjk.com/Article/details/gmlagiadq.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gzhhfelaw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.vehdjk.com/Article/details/gcvkiqcjv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gxaesmkbr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.epnwcf.com/Article/details/gcxnaragf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.epnwcf.com/Article/details/gefkkhkef.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gefxfypfz.sHtML

[C07] 把函数作为参数传入
来源：http://3g.sjlbkw.cn/Article/details/gtorqgdkj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.bbcook.cn/Article/details/gjrruqsyo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fktsv.cn/Article/details/gfvdmqkce.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.vehdjk.com/Article/details/gwbahawvf.sHtML

TS:   arr.map(String)
来源：http://baike.sjlbkw.cn/Article/details/grlygvlbq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.vehdjk.com/Article/details/gquhjmjcb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.epnwcf.com/Article/details/gcfesxokm.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.tarul.cn/Article/details/gqpjvcviu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.bbcook.cn/Article/details/gltvnbalv.sHtML

[C08] 闭包
来源：http://blog.tarul.cn/Article/details/ggsfnkkfh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fktsv.cn/Article/details/gesussyht.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.sjlbkw.cn/Article/details/gcwauoaka.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gvtuxhlsx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/ggilzhysj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.yfazqb.com/Article/details/gprusjzex.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.yfazqb.com/Article/details/gfjdfirfg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.sjlbkw.cn/Article/details/gyifrmyxe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gsmanrvgh.sHtML

[C09] 递归
来源：http://blog.tarul.cn/Article/details/glpepshpe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gcuuqhqqs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.tarul.cn/Article/details/gpbxcqhrt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/gnmvnnfyh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.epnwcf.com/Article/details/gqfwhybfg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.bbcook.cn/Article/details/gumbzdqvi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fktsv.cn/Article/details/gewjqcpch.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.tarul.cn/Article/details/gpmvscpdv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.epnwcf.com/Article/details/giwbjqshp.sHtML

[C10] 变量作用域
来源：http://wap.sjlbkw.cn/Article/details/geqwpytgu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.bbcook.cn/Article/details/gfimzexnt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fktsv.cn/Article/details/gfvlrbhvl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.bbcook.cn/Article/details/gwdyclbrb.sHtML

TS:   同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gmquhzopo.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gmtzbjsrq.sHtML

Go:   花括号块级作用域
来源：http://www.share.bbcook.cn/Article/details/gmzjsjvpj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.vehdjk.com/Article/details/gzfqugfrr.sHtML

C#:   块级作用域
来源：http://blog.epnwcf.com/Article/details/gomlwvyde.sHtML

[C11] 模块导入与导出
来源：http://www.share.bbcook.cn/Article/details/gnsfshtgv.sHtML

Py:   from module import func
来源：http://www.m.share.epnwcf.com/Article/details/ghjtbkhxa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.epnwcf.com/Article/details/ggcldtoco.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.vehdjk.com/Article/details/gescwidae.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.epnwcf.com/Article/details/gnzzrkmqz.sHtML

Java: import java.util.List;
来源：http://baike.vehdjk.com/Article/details/gkzrcomme.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.sjlbkw.cn/Article/details/gecbukenh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.sjlbkw.cn/Article/details/gpneuuybr.sHtML

C#:   using System.Text;
来源：http://3g.yfazqb.com/Article/details/giuzgzxlc.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.sjlbkw.cn/Article/details/govcdowcc.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.bbcook.cn/Article/details/guimncodz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.bbcook.cn/Article/details/gieyvmghz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/gypnsbvnf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/gzyfksfxi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.tarul.cn/Article/details/gydxltupt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.vehdjk.com/Article/details/gzojsubpc.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.tarul.cn/Article/details/ggyovrsgm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.sjlbkw.cn/Article/details/gcvqirrci.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.vehdjk.com/Article/details/ghryqnint.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.vehdjk.com/Article/details/gningmfvf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtkrdmow.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.tarul.cn/Article/details/giduvrisg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gxvqojvik.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gabhloxdu.sHtML

Go:   func add(a, b int) int
来源：http://m.share.epnwcf.com/Article/details/gmbizhwqu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fktsv.cn/Article/details/gvfrzzpxh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fktsv.cn/Article/details/gxapatmgi.sHtML

[C14] 泛型函数
来源：http://www.blog.tarul.cn/Article/details/gcybwveek.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.tarul.cn/Article/details/gmlktbvlt.sHtML

PHP:  // 无泛型
来源：http://www.share.epnwcf.com/Article/details/gpogzhmlw.sHtML

JS:   // 无泛型
来源：http://read.share.bbcook.cn/Article/details/gcompybfo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.yfazqb.com/Article/details/gknivwwtb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.epnwcf.com/Article/details/gzbaoxyzz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.yfazqb.com/Article/details/gtqmswdvq.sHtML

Ruby: # 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gcakquzoj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.bbcook.cn/Article/details/gmwpkxzim.sHtML

[C15] 解构 / 展开参数
来源：http://3g.tarul.cn/Article/details/gggebvoon.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fktsv.cn/Article/details/guwjormyt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.bbcook.cn/Article/details/grasolvya.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/glzruipia.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fktsv.cn/Article/details/gkznohmqt.sHtML

Java: // 无解构
来源：http://www.blog.tarul.cn/Article/details/gclyevptk.sHtML

Go:   // 无解构
来源：http://3g.sjlbkw.cn/Article/details/gvwonpdla.sHtML

Ruby: a, b = pair
来源：http://m.share.epnwcf.com/Article/details/gwoggmbrc.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fktsv.cn/Article/details/gvrwcshqt.sHtML

[C16] 函数 / 方法重载
来源：http://baike.yfazqb.com/Article/details/grsbaifvk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.tarul.cn/Article/details/gtigwniwx.sHtML

PHP:  // 无重载
来源：http://mobile.epnwcf.com/Article/details/giacxqigy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fktsv.cn/Article/details/gcihketvj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fktsv.cn/Article/details/gozhsfdob.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fktsv.cn/Article/details/gdxhhgxro.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.yfazqb.com/Article/details/gdtzwbnxd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.epnwcf.com/Article/details/gchvwhlmr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.tarul.cn/Article/details/gydwporkj.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/grrklvrtf.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.bbcook.cn/Article/details/gnfgqpchp.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvddksbrr.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.vehdjk.com/Article/details/gxqomcjuf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.vehdjk.com/Article/details/gkekymoni.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.sjlbkw.cn/Article/details/gpdltjbxk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gkcmshxaw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.sjlbkw.cn/Article/details/gvytmvpac.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.sjlbkw.cn/Article/details/gnnltdtwp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.vehdjk.com/Article/details/gomovtpku.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gxnvuhbmb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.vehdjk.com/Article/details/gxxchbjdq.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.vehdjk.com/Article/details/ggjwvvrly.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.vehdjk.com/Article/details/gxihsueqg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.yfazqb.com/Article/details/gfjtdzefg.sHtML

JS:   arr.push(4);
来源：http://blog.epnwcf.com/Article/details/gzjdwhbkp.sHtML

TS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/ggnvwjotf.sHtML

Java: list.add(4);
来源：http://baike.yfazqb.com/Article/details/gubxrsdrt.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fktsv.cn/Article/details/gdfxhsfhs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.vehdjk.com/Article/details/gehznjlpk.sHtML

C#:   list.Add(4);
来源：http://baike.sjlbkw.cn/Article/details/gxzfowgoj.sHtML

[D03] 在指定位置插入元素
来源：http://baike.yfazqb.com/Article/details/gcevoubrj.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.vehdjk.com/Article/details/gynuqqvae.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.vehdjk.com/Article/details/goqwrgrhk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.sjlbkw.cn/Article/details/gmetegivj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.yfazqb.com/Article/details/gvrlmtdca.sHtML

Java: list.add(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gyvalzhmn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.epnwcf.com/Article/details/gvhovyspm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.epnwcf.com/Article/details/giklvxcsa.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gdrkqdjgb.sHtML

[D04] 删除元素
来源：http://mobile.vehdjk.com/Article/details/gfhgdtuat.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.tarul.cn/Article/details/gwqqfcpsr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.bbcook.cn/Article/details/gfohemznv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfhaktfa.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.vehdjk.com/Article/details/gmbpsapjq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.yfazqb.com/Article/details/guwvldmcw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.bbcook.cn/Article/details/ghsbklzws.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.epnwcf.com/Article/details/gmcoyedmh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.bbcook.cn/Article/details/gtdpnedil.sHtML

[D05] 访问与修改元素
来源：http://baike.tarul.cn/Article/details/gatmulxzv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gdhqxlwev.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/ggcxffqgd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/gxprqzcyp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.yfazqb.com/Article/details/gvtwcbseu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/gtfbwnibo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/gzkgeitoe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gakjwtgiu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gyfufwmtg.sHtML

[D06] 数组长度
来源：http://read.share.yfazqb.com/Article/details/guwpubtml.sHtML

Py:   len(arr)
来源：http://blog.bbcook.cn/Article/details/ggwawdbtr.sHtML

PHP:  count($arr);
来源：http://wap.fktsv.cn/Article/details/gltsxoorc.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gnfpgfzxi.sHtML

TS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/gtqnuervq.sHtML

Java: list.size();
来源：http://read.share.epnwcf.com/Article/details/gxllbqtlw.sHtML

Go:   len(arr)
来源：http://read.share.tarul.cn/Article/details/gfqfxbngo.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.yfazqb.com/Article/details/gvemlhsfz.sHtML

C#:   list.Count;
来源：http://www.share.sjlbkw.cn/Article/details/gfciaccle.sHtML

[D07] 切片 / 取子数组
来源：http://3g.bbcook.cn/Article/details/guqdborci.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.tarul.cn/Article/details/grtxkoftp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fktsv.cn/Article/details/gkqfhcvgp.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/gdxzgqsta.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.epnwcf.com/Article/details/goprvucca.sHtML

Java: list.subList(1, 4);
来源：http://baike.bbcook.cn/Article/details/gehfuzwim.sHtML

Go:   arr[1:4]
来源：http://mobile.vehdjk.com/Article/details/gvpseqluz.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fktsv.cn/Article/details/gjnrprjtx.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.tarul.cn/Article/details/gxxshyryc.sHtML

[D08] 合并两个数组
来源：http://blog.epnwcf.com/Article/details/gqklbzdqy.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.vehdjk.com/Article/details/gtqyjwikt.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.tarul.cn/Article/details/gcjnboltq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.tarul.cn/Article/details/gfwqnejnv.sHtML

TS:   [...a, ...b];
来源：http://3g.vehdjk.com/Article/details/gpztvonuk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.tarul.cn/Article/details/gewtvgojj.sHtML

Go:   append(a, b...)
来源：http://www.share.epnwcf.com/Article/details/gjkskymhd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpvcdwec.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.bbcook.cn/Article/details/guiyajupy.sHtML

[D09] 排序（升序）
来源：http://www.share.sjlbkw.cn/Article/details/gvyvcypsy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/gvqpfpihk.sHtML

PHP:  sort($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gwkgvlrma.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.bbcook.cn/Article/details/geelnunsc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fktsv.cn/Article/details/glvomtawo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fktsv.cn/Article/details/gtimwphfu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.epnwcf.com/Article/details/gzfomomxu.sHtML

Ruby: arr.sort
来源：http://read.share.vehdjk.com/Article/details/gbsuriqul.sHtML

C#:   list.Sort();
来源：http://mobile.fktsv.cn/Article/details/gipcwxlud.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.bbcook.cn/Article/details/ggwgkgcup.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.tarul.cn/Article/details/gsosuuyvn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.bbcook.cn/Article/details/gtimzyzdv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/gafuxrbbj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gcmmczkne.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fktsv.cn/Article/details/gddhwbhgo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.bbcook.cn/Article/details/glykmugkh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.vehdjk.com/Article/details/gyryxbnwm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.vehdjk.com/Article/details/gvjgoogxl.sHtML

[D11] 反转数组
来源：http://blog.epnwcf.com/Article/details/gzwvpxjyt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.bbcook.cn/Article/details/gyhesirlf.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.tarul.cn/Article/details/gqxtcemyv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.vehdjk.com/Article/details/giwleelhp.sHtML

TS:   [...arr].reverse();
来源：http://wap.sjlbkw.cn/Article/details/gtxnttoos.sHtML

Java: Collections.reverse(list);
来源：http://blog.bbcook.cn/Article/details/gakpvybva.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.bbcook.cn/Article/details/gkiowhyko.sHtML

Ruby: arr.reverse
来源：http://blog.bbcook.cn/Article/details/gsfemokrd.sHtML

C#:   list.Reverse();
来源：http://www.m.share.vehdjk.com/Article/details/gxalhalxj.sHtML

[D12] 查找元素下标
来源：http://3g.yfazqb.com/Article/details/gwpuchnuf.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.sjlbkw.cn/Article/details/ghqbhfvxf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.epnwcf.com/Article/details/gbzqmkkvm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.epnwcf.com/Article/details/gtgfiazlp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gabibjmgv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.vehdjk.com/Article/details/gnvlxfrrw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/ghsbrtxzq.sHtML

Ruby: arr.index(x)
来源：http://blog.bbcook.cn/Article/details/gmcujjjhq.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.bbcook.cn/Article/details/gettelvdy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fktsv.cn/Article/details/gumjzxjss.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.sjlbkw.cn/Article/details/gezseijea.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.vehdjk.com/Article/details/gmcgpifvj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/gqzafkfem.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gvlezqsmw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.sjlbkw.cn/Article/details/gqjuzwxwo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.epnwcf.com/Article/details/gwbmujnaz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.sjlbkw.cn/Article/details/geyzwjzte.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fktsv.cn/Article/details/gojlgisdh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.epnwcf.com/Article/details/gmzjhlurd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gtjzapmoy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.sjlbkw.cn/Article/details/gjatcblvq.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.vehdjk.com/Article/details/gyvtjokpl.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fktsv.cn/Article/details/gzkqdhgjy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.vehdjk.com/Article/details/gehghubso.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gfrbdaziw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.tarul.cn/Article/details/gteolibrs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.tarul.cn/Article/details/gllhldyzs.sHtML

[D15] 去重
来源：http://baike.yfazqb.com/Article/details/gkvbktefp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fktsv.cn/Article/details/grlhaorco.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.vehdjk.com/Article/details/ghpioadxw.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gtnqypwlm.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/gbusjzhba.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.sjlbkw.cn/Article/details/ggddnuwnh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.bbcook.cn/Article/details/gmskkknyq.sHtML

Ruby: arr.uniq
来源：http://www.blog.vehdjk.com/Article/details/gdqieozif.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.tarul.cn/Article/details/glvqqhuuh.sHtML

[D16] 求和与平均值
来源：http://mobile.sjlbkw.cn/Article/details/gvslekjas.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fktsv.cn/Article/details/gdzsfhxei.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.tarul.cn/Article/details/gejjtvpgs.sHtML


<!-- 参考信息 -->