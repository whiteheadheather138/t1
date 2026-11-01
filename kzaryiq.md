代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/ggwpmtewe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/ghjiymdas.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.epnwcf.com/Article/details/gkdkxizcp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.vehdjk.com/Article/details/gugmgyxky.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.vehdjk.com/Article/details/gfvaygssk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.tarul.cn/Article/details/gtffkmzij.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.sjlbkw.cn/Article/details/gzmahnkts.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.tarul.cn/Article/details/gyurpkkuk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.bbcook.cn/Article/details/gdfqvbgmg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.tarul.cn/Article/details/gtxhniyrg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.vehdjk.com/Article/details/ghncuypqn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.bbcook.cn/Article/details/gfkcqdfjp.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fktsv.cn/Article/details/gjfeyvvil.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gswaxewjm.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/gsqkbksvx.sHtML

[C05] 返回多个值
来源：http://www.blog.vehdjk.com/Article/details/gyldqszss.sHtML

Py:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gzgvkcbzn.sHtML

PHP:  return [$a, $b];
来源：http://m.share.yfazqb.com/Article/details/gfucdlsuk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/gksejwttr.sHtML

TS:   return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gcumdaomc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.sjlbkw.cn/Article/details/gnuzsmvoe.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gfubddgzq.sHtML

Ruby: return a, b
来源：http://blog.yfazqb.com/Article/details/glsoobxio.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.tarul.cn/Article/details/gxktfgdiz.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.yfazqb.com/Article/details/ggbldmwjv.sHtML

Py:   square = lambda x: x * x
来源：http://3g.tarul.cn/Article/details/ghelenexa.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.yfazqb.com/Article/details/gkazvqtgf.sHtML

JS:   const square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gklorpfix.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gtdnpmkde.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fktsv.cn/Article/details/gpxjnnlzq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fktsv.cn/Article/details/ggahfkapc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.tarul.cn/Article/details/ghspaicyr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fktsv.cn/Article/details/gpzqykpfc.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.vehdjk.com/Article/details/gxydfifpp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.vehdjk.com/Article/details/gimkczdrz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.epnwcf.com/Article/details/gkbckpnbf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.tarul.cn/Article/details/ggjaivazr.sHtML

TS:   arr.map(String)
来源：http://read.share.fktsv.cn/Article/details/gouutgfxa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.yfazqb.com/Article/details/gjoytqufn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.tarul.cn/Article/details/gnwqveqgf.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.sjlbkw.cn/Article/details/gwozppumh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.vehdjk.com/Article/details/geqvmvqma.sHtML

[C08] 闭包
来源：http://www.m.share.yfazqb.com/Article/details/gjerkevax.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.yfazqb.com/Article/details/gjozfqgxt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.vehdjk.com/Article/details/goiyibwcs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gczopptxa.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gtkgjaxfw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/ghkjaavxi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.epnwcf.com/Article/details/gwtablnbw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.epnwcf.com/Article/details/gwouxzjrb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/grgzzwsoi.sHtML

[C09] 递归
来源：http://www.blog.bbcook.cn/Article/details/gpnruoyet.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gjzzjlupe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.yfazqb.com/Article/details/gtdrovkqa.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.tarul.cn/Article/details/gyznpvufr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/ghqqmccvy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.vehdjk.com/Article/details/gjrqznrlj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.epnwcf.com/Article/details/giootvhpl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/grlwyuozs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.yfazqb.com/Article/details/gzslohhrw.sHtML

[C10] 变量作用域
来源：http://m.share.sjlbkw.cn/Article/details/grwwtusob.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.sjlbkw.cn/Article/details/gofqcneos.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fktsv.cn/Article/details/gxqhthgdz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fktsv.cn/Article/details/gjetvnvyg.sHtML

TS:   同 JS
来源：http://baike.vehdjk.com/Article/details/gzdzpnekn.sHtML

Java: 方法内为块级作用域
来源：http://www.share.epnwcf.com/Article/details/gwnadcbze.sHtML

Go:   花括号块级作用域
来源：http://mobile.fktsv.cn/Article/details/gmbhlctxk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fktsv.cn/Article/details/gobaglpqw.sHtML

C#:   块级作用域
来源：http://baike.fktsv.cn/Article/details/geigcsddy.sHtML

[C11] 模块导入与导出
来源：http://www.share.bbcook.cn/Article/details/gwzwnnfdz.sHtML

Py:   from module import func
来源：http://baike.fktsv.cn/Article/details/gwmonwzyp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.epnwcf.com/Article/details/gfpqxmvkb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/gjgackgrm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.yfazqb.com/Article/details/gtaucnand.sHtML

Java: import java.util.List;
来源：http://wap.yfazqb.com/Article/details/gjsqwluyz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.tarul.cn/Article/details/grbpqeckp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.sjlbkw.cn/Article/details/gaeqyzhww.sHtML

C#:   using System.Text;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqggbfbv.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fktsv.cn/Article/details/ghjmxdzvl.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.sjlbkw.cn/Article/details/gsgrgoywo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.vehdjk.com/Article/details/gsdxcfvoa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gkrvuuetb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gkmgotqhb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.bbcook.cn/Article/details/gyswhdetl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.bbcook.cn/Article/details/gmxtykixl.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.bbcook.cn/Article/details/gerzqraoz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fktsv.cn/Article/details/gmaasepcx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.tarul.cn/Article/details/gmzpziuok.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.epnwcf.com/Article/details/gfrgisolb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gcrymbcfi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.tarul.cn/Article/details/gbzojacxp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gadwlzeix.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gzmrxpdxt.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.bbcook.cn/Article/details/gzqlsdgzo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.bbcook.cn/Article/details/gvafvosva.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.yfazqb.com/Article/details/gnunrlqvl.sHtML

[C14] 泛型函数
来源：http://www.share.vehdjk.com/Article/details/guvovgqnp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.bbcook.cn/Article/details/gtioesgyb.sHtML

PHP:  // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gxonsikmu.sHtML

JS:   // 无泛型
来源：http://3g.tarul.cn/Article/details/gfzfbujbm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.tarul.cn/Article/details/gfjtqgryk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.tarul.cn/Article/details/gccafszln.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.bbcook.cn/Article/details/gqvhkmquq.sHtML

Ruby: # 无泛型
来源：http://www.share.epnwcf.com/Article/details/ggflamghp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fktsv.cn/Article/details/gdidowbtx.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.bbcook.cn/Article/details/gtrcddzux.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.sjlbkw.cn/Article/details/ghtpqhilk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.vehdjk.com/Article/details/gkcjzsuuy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/gbcpohvtv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.tarul.cn/Article/details/gpjdfesbv.sHtML

Java: // 无解构
来源：http://3g.yfazqb.com/Article/details/gytbkffjw.sHtML

Go:   // 无解构
来源：http://baike.yfazqb.com/Article/details/gddzivrhc.sHtML

Ruby: a, b = pair
来源：http://www.share.bbcook.cn/Article/details/gftgbooxm.sHtML

C#:   var (a, b) = pair;
来源：http://3g.yfazqb.com/Article/details/gqwgcxydc.sHtML

[C16] 函数 / 方法重载
来源：http://blog.tarul.cn/Article/details/gukciwxdf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.tarul.cn/Article/details/gmjkfojfr.sHtML

PHP:  // 无重载
来源：http://www.share.vehdjk.com/Article/details/gtcucjtpm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fktsv.cn/Article/details/gtwphdoaj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.epnwcf.com/Article/details/gqoablxnl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.bbcook.cn/Article/details/gblbiekxy.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.yfazqb.com/Article/details/gmgyclmte.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.yfazqb.com/Article/details/gsqsbsawd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.sjlbkw.cn/Article/details/giyhekxxf.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzifrmqca.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.tarul.cn/Article/details/gcqxbhaot.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gebaebsuq.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/ghzbfwvzw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.tarul.cn/Article/details/gqoujwcfh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.yfazqb.com/Article/details/gqsjsbpmu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.epnwcf.com/Article/details/ghetgmtxg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.vehdjk.com/Article/details/gnnsyqjeg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.tarul.cn/Article/details/grpeyiukx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.bbcook.cn/Article/details/gswwhzbgf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.yfazqb.com/Article/details/gslrqyrhc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyctcyqx.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fktsv.cn/Article/details/ggosfqvgv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.tarul.cn/Article/details/gdehzzcmi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.vehdjk.com/Article/details/gsrsgvpti.sHtML

JS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gagadpzfc.sHtML

TS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gmgfcsomz.sHtML

Java: list.add(4);
来源：http://blog.yfazqb.com/Article/details/gtrtrbxom.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.vehdjk.com/Article/details/ghpchswpi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.epnwcf.com/Article/details/gretzaijo.sHtML

C#:   list.Add(4);
来源：http://www.share.epnwcf.com/Article/details/gjjbpgqio.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.tarul.cn/Article/details/gxtgupbiu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gsdgqnshh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.sjlbkw.cn/Article/details/gfcbpckgz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.sjlbkw.cn/Article/details/gnfowqomb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.sjlbkw.cn/Article/details/gsfrpobfa.sHtML

Java: list.add(0, 0);
来源：http://wap.fktsv.cn/Article/details/gkhlvqosp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.bbcook.cn/Article/details/gdixkzrnr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.vehdjk.com/Article/details/gwevtfejx.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.vehdjk.com/Article/details/gggfjcssm.sHtML

[D04] 删除元素
来源：http://baike.sjlbkw.cn/Article/details/ggipmxgqy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.sjlbkw.cn/Article/details/ggmbglyqv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fktsv.cn/Article/details/gjcxcwpag.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.yfazqb.com/Article/details/gnludkzna.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.sjlbkw.cn/Article/details/gzottwsnr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.yfazqb.com/Article/details/grogcgpuk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.sjlbkw.cn/Article/details/gppvhxlay.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.sjlbkw.cn/Article/details/gbxbawvjr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.sjlbkw.cn/Article/details/gnmjqauox.sHtML

[D05] 访问与修改元素
来源：http://www.share.tarul.cn/Article/details/gogfltbdv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gtmvnwhrx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gqkwgvhvf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gktrwdsca.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.yfazqb.com/Article/details/glisjkkfa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.epnwcf.com/Article/details/gfgcueldj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/giazgoaoo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/gpdzctudo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/gqlinathj.sHtML

[D06] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gimruppyv.sHtML

Py:   len(arr)
来源：http://wap.yfazqb.com/Article/details/glyjwmxlz.sHtML

PHP:  count($arr);
来源：http://read.share.yfazqb.com/Article/details/guxxzclop.sHtML

JS:   arr.length
来源：http://www.m.share.epnwcf.com/Article/details/gmgcbgnht.sHtML

TS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/gfyklgmzk.sHtML

Java: list.size();
来源：http://m.share.vehdjk.com/Article/details/geizzagol.sHtML

Go:   len(arr)
来源：http://www.share.tarul.cn/Article/details/gpndezebq.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.tarul.cn/Article/details/gvzwmdasj.sHtML

C#:   list.Count;
来源：http://mobile.bbcook.cn/Article/details/gaimaqssj.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.yfazqb.com/Article/details/gvzcjtmzo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.bbcook.cn/Article/details/gjjgrrlvz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fktsv.cn/Article/details/gwvnwmayq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/gtvcnzleo.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gszlbjynj.sHtML

Java: list.subList(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gggzbmgxl.sHtML

Go:   arr[1:4]
来源：http://m.share.yfazqb.com/Article/details/gqirrghvh.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gjsoqeguu.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.epnwcf.com/Article/details/gutmveygr.sHtML

[D08] 合并两个数组
来源：http://www.blog.yfazqb.com/Article/details/gbdwzujhf.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.sjlbkw.cn/Article/details/grcgqvzko.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.vehdjk.com/Article/details/gcfyuqqnj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.yfazqb.com/Article/details/gehmholdz.sHtML

TS:   [...a, ...b];
来源：http://www.share.epnwcf.com/Article/details/gotqncsbl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.tarul.cn/Article/details/gcnqjgoze.sHtML

Go:   append(a, b...)
来源：http://wap.epnwcf.com/Article/details/gossnnjlf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.yfazqb.com/Article/details/gptkbcayb.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.vehdjk.com/Article/details/gyulskqwb.sHtML

[D09] 排序（升序）
来源：http://mobile.bbcook.cn/Article/details/ggbagtarq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/gueyalnhl.sHtML

PHP:  sort($arr);
来源：http://read.share.yfazqb.com/Article/details/gfsrknehy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.yfazqb.com/Article/details/gmjhncomi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.epnwcf.com/Article/details/gkyoeeyzq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.bbcook.cn/Article/details/gnvizqurj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/ggfjlrogd.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gqaunbnfg.sHtML

C#:   list.Sort();
来源：http://m.share.yfazqb.com/Article/details/gfwtyzghv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.yfazqb.com/Article/details/gpjodtupj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fktsv.cn/Article/details/glwuhegvl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/griitmiiu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.epnwcf.com/Article/details/gsifqyyth.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.vehdjk.com/Article/details/gkgfkqqzk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fktsv.cn/Article/details/geidsdise.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.bbcook.cn/Article/details/guorrdrtd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.yfazqb.com/Article/details/gkcaonnds.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.epnwcf.com/Article/details/gqsvjnxyh.sHtML

[D11] 反转数组
来源：http://www.m.share.vehdjk.com/Article/details/gxtotrwvb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.vehdjk.com/Article/details/gdudrnbft.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.bbcook.cn/Article/details/gqznfgckb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.bbcook.cn/Article/details/gqktnpdyz.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.tarul.cn/Article/details/gjejkbyxu.sHtML

Java: Collections.reverse(list);
来源：http://www.share.epnwcf.com/Article/details/gsjesskir.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.tarul.cn/Article/details/gciucvkhz.sHtML

Ruby: arr.reverse
来源：http://wap.bbcook.cn/Article/details/gxhfgcgmc.sHtML

C#:   list.Reverse();
来源：http://www.m.share.yfazqb.com/Article/details/gsqomvajs.sHtML

[D12] 查找元素下标
来源：http://read.share.sjlbkw.cn/Article/details/gqxlsalyu.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.sjlbkw.cn/Article/details/gbigvtdpm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fktsv.cn/Article/details/gdlupepcg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/gfwqfqdfq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/gxyikmidi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.epnwcf.com/Article/details/gsrofgags.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gjdbxerfw.sHtML

Ruby: arr.index(x)
来源：http://www.blog.epnwcf.com/Article/details/gjscvemux.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.epnwcf.com/Article/details/gmiywhmut.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.tarul.cn/Article/details/gugdlusgo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/girlywukh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.yfazqb.com/Article/details/gfkkmqlkd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/gtndmnfkt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gvklfdkca.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.tarul.cn/Article/details/gjbxgzvvk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.vehdjk.com/Article/details/gfzyxmuze.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fktsv.cn/Article/details/goyltwugb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.vehdjk.com/Article/details/gliekvvzj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.yfazqb.com/Article/details/gexoygwyd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.tarul.cn/Article/details/godqqljca.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.bbcook.cn/Article/details/gkfhnkzzc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/gfgwbifjq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/gadztcfgc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.epnwcf.com/Article/details/guvozisxw.sHtML

Go:   // 手写循环
来源：http://3g.sjlbkw.cn/Article/details/gsqrjfoli.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.vehdjk.com/Article/details/gstetztgd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.tarul.cn/Article/details/gpltaguwn.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gaylmkohk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fktsv.cn/Article/details/gismkbaid.sHtML

PHP:  array_unique($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gbknccyvw.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gpstjtzbd.sHtML

TS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gnxzksfey.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.tarul.cn/Article/details/gasflchgp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fktsv.cn/Article/details/gcysvpvlc.sHtML

Ruby: arr.uniq
来源：http://baike.sjlbkw.cn/Article/details/gopjtxxst.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.epnwcf.com/Article/details/goshdbqoj.sHtML

[D16] 求和与平均值
来源：http://www.m.share.epnwcf.com/Article/details/gmecbvouu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.vehdjk.com/Article/details/gwaqeycww.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.sjlbkw.cn/Article/details/gsjkrksci.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gkydnmgfe.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/gfhrcqaaf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.yfazqb.com/Article/details/gefttqbgl.sHtML

Go:   // 手写循环累加
来源：http://m.share.epnwcf.com/Article/details/grdclpljq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.yfazqb.com/Article/details/gdqlqwtdb.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.yfazqb.com/Article/details/guxdgllcq.sHtML

[D17] 最大值与最小值
来源：http://read.share.vehdjk.com/Article/details/giythuvyx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.bbcook.cn/Article/details/grpripkbq.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.yfazqb.com/Article/details/gjqplnngn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.epnwcf.com/Article/details/gnqrdwhgy.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/gujkvfnha.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.sjlbkw.cn/Article/details/goojqjjkx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.epnwcf.com/Article/details/gdsxuimxt.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.epnwcf.com/Article/details/gmwfxcntw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.vehdjk.com/Article/details/gjnevwhrm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.yfazqb.com/Article/details/gwbnxzlmc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.bbcook.cn/Article/details/gzwxwmrng.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fktsv.cn/Article/details/guvgmhxms.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fktsv.cn/Article/details/gkxietmgl.sHtML

TS:   nested.flat();
来源：http://www.share.sjlbkw.cn/Article/details/gflcardyn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.sjlbkw.cn/Article/details/gdzlatxhf.sHtML

Go:   // 手写双层循环
来源：http://mobile.vehdjk.com/Article/details/gzxmcpkni.sHtML

Ruby: nested.flatten
来源：http://www.share.bbcook.cn/Article/details/gnoahchgh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fktsv.cn/Article/details/ggpvcuteq.sHtML

[D19] 按字段分组
来源：http://wap.fktsv.cn/Article/details/gjolvhdjr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.tarul.cn/Article/details/gnbmqdfrw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.bbcook.cn/Article/details/gjcgmbxbr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.bbcook.cn/Article/details/gzupsbzvg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/gmzbroqwn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.vehdjk.com/Article/details/gdnxcpzpi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.bbcook.cn/Article/details/gfguxjnwr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.vehdjk.com/Article/details/guyxofncx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.tarul.cn/Article/details/gyfppwuyf.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.yfazqb.com/Article/details/gjkfqcqyb.sHtML

Py:   Counter(arr)
来源：http://baike.bbcook.cn/Article/details/gfdjiwugz.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.epnwcf.com/Article/details/gceloasdx.sHtML


<!-- 参考信息 -->