代发 wailian999

Py:   return a, b
来源：http://wap.fktsv.cn/Article/details/gwjynttzv.sHtML

PHP:  return [$a, $b];
来源：http://m.share.vehdjk.com/Article/details/gimddlieo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.vehdjk.com/Article/details/gdfjpknwd.sHtML

TS:   return { a, b };
来源：http://read.share.yfazqb.com/Article/details/glugpynaa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.bbcook.cn/Article/details/gqyjxuule.sHtML

Go:   return a, b
来源：http://m.share.yfazqb.com/Article/details/gfmwywouc.sHtML

Ruby: return a, b
来源：http://3g.sjlbkw.cn/Article/details/grefehmar.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.sjlbkw.cn/Article/details/gqicltelb.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.sjlbkw.cn/Article/details/ggfgcftgx.sHtML

Py:   square = lambda x: x * x
来源：http://blog.epnwcf.com/Article/details/gncbwnovt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.epnwcf.com/Article/details/gsvboulwr.sHtML

JS:   const square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gahamjndr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.epnwcf.com/Article/details/gsaqwaoom.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.sjlbkw.cn/Article/details/gfqnsyphu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.yfazqb.com/Article/details/giawctqfd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.sjlbkw.cn/Article/details/gryxkqczj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gamgtxkol.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.vehdjk.com/Article/details/gpdsvifbr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.epnwcf.com/Article/details/gcfacepey.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gkzixbnxq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.tarul.cn/Article/details/gcbbbvhii.sHtML

TS:   arr.map(String)
来源：http://mobile.bbcook.cn/Article/details/gzipikawi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.bbcook.cn/Article/details/gcwgldywi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.tarul.cn/Article/details/glnsznizx.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.bbcook.cn/Article/details/ggiausmsv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.bbcook.cn/Article/details/giunxwxno.sHtML

[C08] 闭包
来源：http://3g.tarul.cn/Article/details/gfkpkkvkk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.vehdjk.com/Article/details/gbqscwdhu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.yfazqb.com/Article/details/gpjvbhjrw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gdldyqohu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gsxnxdchw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.tarul.cn/Article/details/gugsibloq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.tarul.cn/Article/details/gkuwjyudt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.epnwcf.com/Article/details/gqnfoahkm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/gmfimtdju.sHtML

[C09] 递归
来源：http://www.blog.sjlbkw.cn/Article/details/goybzjebb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.tarul.cn/Article/details/gezrjwhdg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.epnwcf.com/Article/details/gtksadqlh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/gwggcqyzd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.sjlbkw.cn/Article/details/gwksznzev.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.epnwcf.com/Article/details/groqavuhu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.sjlbkw.cn/Article/details/gttvwtpcx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/goildddqb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.yfazqb.com/Article/details/gbnwabzsa.sHtML

[C10] 变量作用域
来源：http://baike.tarul.cn/Article/details/gvezcrqkx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fktsv.cn/Article/details/govraaylr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.epnwcf.com/Article/details/gpmpuojem.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.epnwcf.com/Article/details/geahwyesn.sHtML

TS:   同 JS
来源：http://read.share.bbcook.cn/Article/details/gyjxbmzed.sHtML

Java: 方法内为块级作用域
来源：http://blog.bbcook.cn/Article/details/gsucvtnxg.sHtML

Go:   花括号块级作用域
来源：http://baike.epnwcf.com/Article/details/gklldexpl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.vehdjk.com/Article/details/gmktruawb.sHtML

C#:   块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gdxksbmex.sHtML

[C11] 模块导入与导出
来源：http://www.share.tarul.cn/Article/details/gwppgnmxk.sHtML

Py:   from module import func
来源：http://read.share.sjlbkw.cn/Article/details/gthcjenji.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.bbcook.cn/Article/details/gvkdmuxss.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.epnwcf.com/Article/details/gzknkycna.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fktsv.cn/Article/details/gknstxayh.sHtML

Java: import java.util.List;
来源：http://www.share.yfazqb.com/Article/details/ggxxrdhcc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fktsv.cn/Article/details/grdnxewrg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.tarul.cn/Article/details/gwwwqznwq.sHtML

C#:   using System.Text;
来源：http://blog.bbcook.cn/Article/details/gnuszpiog.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.epnwcf.com/Article/details/gkfxglxwv.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.sjlbkw.cn/Article/details/gwdzbaadt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.sjlbkw.cn/Article/details/gfjvtvsii.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/gtppxcaes.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/gnfyorpkc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fktsv.cn/Article/details/gujoyxcir.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.bbcook.cn/Article/details/gpokqanob.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.tarul.cn/Article/details/gyafrbvdr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fktsv.cn/Article/details/gtvkzzxgl.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.sjlbkw.cn/Article/details/gncjjnzbt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.sjlbkw.cn/Article/details/gwcbqqugq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gvefrfwxk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwnqlcds.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gspnhcsvn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gqjqcqbyc.sHtML

Go:   func add(a, b int) int
来源：http://3g.epnwcf.com/Article/details/gifpgulnb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.vehdjk.com/Article/details/gutrciddi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.sjlbkw.cn/Article/details/guyllgibg.sHtML

[C14] 泛型函数
来源：http://www.blog.fktsv.cn/Article/details/gyesponda.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.vehdjk.com/Article/details/gcqhapvvn.sHtML

PHP:  // 无泛型
来源：http://mobile.fktsv.cn/Article/details/grcortqxk.sHtML

JS:   // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gzjsgogpl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/gvbinwlsi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.epnwcf.com/Article/details/gaabfbzid.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.vehdjk.com/Article/details/gxtnubwfj.sHtML

Ruby: # 无泛型
来源：http://baike.epnwcf.com/Article/details/gjubtsqkp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fktsv.cn/Article/details/gxrijcdkb.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.vehdjk.com/Article/details/gymjcvfxq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/gvgdyskfa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.tarul.cn/Article/details/glalunyss.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.vehdjk.com/Article/details/gritkiowa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.epnwcf.com/Article/details/gezmkezbq.sHtML

Java: // 无解构
来源：http://wap.fktsv.cn/Article/details/gqydrkwlu.sHtML

Go:   // 无解构
来源：http://3g.bbcook.cn/Article/details/gejzwmerj.sHtML

Ruby: a, b = pair
来源：http://mobile.sjlbkw.cn/Article/details/gxvainwgq.sHtML

C#:   var (a, b) = pair;
来源：http://3g.tarul.cn/Article/details/gwhuncxxo.sHtML

[C16] 函数 / 方法重载
来源：http://3g.bbcook.cn/Article/details/gluxclsoo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.tarul.cn/Article/details/gbgqhspno.sHtML

PHP:  // 无重载
来源：http://3g.fktsv.cn/Article/details/gvyikblev.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.epnwcf.com/Article/details/gneyhiiow.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.yfazqb.com/Article/details/gzzroovzm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.yfazqb.com/Article/details/gfwxzranb.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.vehdjk.com/Article/details/gapxktacc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.tarul.cn/Article/details/gdoskmsqf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.bbcook.cn/Article/details/gxeomijwx.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gcmznbepm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.epnwcf.com/Article/details/gumaswsyy.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gydbowokv.sHtML

[D01] 创建数组 / 列表
来源：http://wap.epnwcf.com/Article/details/gcagsoahs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.vehdjk.com/Article/details/gvzlcfvml.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.yfazqb.com/Article/details/gpauxxbub.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.vehdjk.com/Article/details/grrpgkcou.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.yfazqb.com/Article/details/gltirucvg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.sjlbkw.cn/Article/details/gqyaunmeq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.tarul.cn/Article/details/goflfjnpk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.tarul.cn/Article/details/gvmsxhuns.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.yfazqb.com/Article/details/gskvtmvgm.sHtML

[D02] 追加元素到末尾
来源：http://3g.epnwcf.com/Article/details/gyduobkfb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.sjlbkw.cn/Article/details/goiaprfgp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.epnwcf.com/Article/details/gfhpkckkl.sHtML

JS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/gvdaoezde.sHtML

TS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/ghrefhmal.sHtML

Java: list.add(4);
来源：http://mobile.epnwcf.com/Article/details/ghenzmvol.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.yfazqb.com/Article/details/gfqqafigj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.bbcook.cn/Article/details/gektjvjqu.sHtML

C#:   list.Add(4);
来源：http://baike.tarul.cn/Article/details/gxliyszjo.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fktsv.cn/Article/details/gwbpvzmqu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gjsqyaeei.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.epnwcf.com/Article/details/gneqlrbvj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.tarul.cn/Article/details/gtdwiwxde.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.yfazqb.com/Article/details/gdnlkvlaa.sHtML

Java: list.add(0, 0);
来源：http://wap.bbcook.cn/Article/details/gxpuhasfo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.sjlbkw.cn/Article/details/gkvspiogo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.vehdjk.com/Article/details/gryzjwcas.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.vehdjk.com/Article/details/gbkoaijde.sHtML

[D04] 删除元素
来源：http://m.share.bbcook.cn/Article/details/gnbnbwphu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.vehdjk.com/Article/details/ghtmwleho.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fktsv.cn/Article/details/gkruejhxf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.tarul.cn/Article/details/gensgxukb.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.bbcook.cn/Article/details/gkcqqbgyv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.tarul.cn/Article/details/gzuehmoid.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.yfazqb.com/Article/details/gemerkqft.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.tarul.cn/Article/details/gpmhndelh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.sjlbkw.cn/Article/details/gfigqeeqw.sHtML

[D05] 访问与修改元素
来源：http://m.share.tarul.cn/Article/details/gwvslkdxq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gxncjhirv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gttdxljgu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gktfpsykg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.vehdjk.com/Article/details/gumeeyxzp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.epnwcf.com/Article/details/gsbibyidz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gyypblcwp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gxazprkvb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gjbaevkgj.sHtML

[D06] 数组长度
来源：http://m.share.epnwcf.com/Article/details/guajxcpgp.sHtML

Py:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gtqwrozub.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gjuihvzht.sHtML

JS:   arr.length
来源：http://www.blog.epnwcf.com/Article/details/geaqlcqdt.sHtML

TS:   arr.length
来源：http://mobile.tarul.cn/Article/details/gsczzejtz.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/guaaccbyw.sHtML

Go:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gozihmeuq.sHtML

Ruby: arr.length; arr.size
来源：http://blog.vehdjk.com/Article/details/gammuotpo.sHtML

C#:   list.Count;
来源：http://blog.epnwcf.com/Article/details/gfdffjjuo.sHtML

[D07] 切片 / 取子数组
来源：http://3g.epnwcf.com/Article/details/gavuwqeul.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.sjlbkw.cn/Article/details/ggvvvsibe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.yfazqb.com/Article/details/gtcbcfdiz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gdrlqwixy.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/guzzlaluv.sHtML

Java: list.subList(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gtquaosxr.sHtML

Go:   arr[1:4]
来源：http://read.share.vehdjk.com/Article/details/gqapbjtjx.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.epnwcf.com/Article/details/grcvxnmlz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gmdnhrqof.sHtML

[D08] 合并两个数组
来源：http://read.share.tarul.cn/Article/details/gcfqciphq.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.yfazqb.com/Article/details/gdoqykxra.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.bbcook.cn/Article/details/gksbgwrjl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.sjlbkw.cn/Article/details/gmnayrxnq.sHtML

TS:   [...a, ...b];
来源：http://www.share.epnwcf.com/Article/details/gkjlyaunc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.epnwcf.com/Article/details/glopfmvex.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fktsv.cn/Article/details/gapjglaxm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fktsv.cn/Article/details/gadneyonp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gpucyxmkk.sHtML

[D09] 排序（升序）
来源：http://www.share.epnwcf.com/Article/details/gbivkirhv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gawyjrtwf.sHtML

PHP:  sort($arr);
来源：http://www.share.tarul.cn/Article/details/gjpedcamr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.epnwcf.com/Article/details/gqgayrzfy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.yfazqb.com/Article/details/gbghcuxjr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.yfazqb.com/Article/details/ggmpvmhtu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gmkbyvwix.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gplkxcuur.sHtML

C#:   list.Sort();
来源：http://wap.sjlbkw.cn/Article/details/gfcibhdoh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.bbcook.cn/Article/details/gawkbesca.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.sjlbkw.cn/Article/details/gdhvazcwj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/gkbjwaxyr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/giujybdta.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/gjodmqiri.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.epnwcf.com/Article/details/gfbveeuyh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fktsv.cn/Article/details/gzgqhugmj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fktsv.cn/Article/details/gxojlufbo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fktsv.cn/Article/details/gbzoynkqb.sHtML

[D11] 反转数组
来源：http://blog.bbcook.cn/Article/details/ggccetvcu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/gytkqifvq.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.tarul.cn/Article/details/gfnvjijfl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.yfazqb.com/Article/details/gkqoxqwje.sHtML

TS:   [...arr].reverse();
来源：http://mobile.sjlbkw.cn/Article/details/gamqxxccw.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fktsv.cn/Article/details/gndqgcqep.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.epnwcf.com/Article/details/gbglptjxz.sHtML

Ruby: arr.reverse
来源：http://3g.sjlbkw.cn/Article/details/gmvwidhxg.sHtML

C#:   list.Reverse();
来源：http://read.share.sjlbkw.cn/Article/details/gwcydavco.sHtML

[D12] 查找元素下标
来源：http://blog.bbcook.cn/Article/details/gnojsrpkv.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.bbcook.cn/Article/details/gvxommmef.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.vehdjk.com/Article/details/gubauvkhv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.yfazqb.com/Article/details/gmmquqsil.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gmwjxxoeb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.epnwcf.com/Article/details/gpstqfzap.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.yfazqb.com/Article/details/gdstwufjt.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.bbcook.cn/Article/details/gipkajwbr.sHtML

C#:   list.IndexOf(x);
来源：http://baike.tarul.cn/Article/details/gzwvyigjy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.yfazqb.com/Article/details/gvchdztdy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gcolegiec.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.vehdjk.com/Article/details/gfcertkwk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gybxyjyxb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.vehdjk.com/Article/details/gntsfhqce.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fktsv.cn/Article/details/gulpetcik.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.yfazqb.com/Article/details/gqmhojegl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fktsv.cn/Article/details/gisiefckp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.tarul.cn/Article/details/ggfgwmguj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.bbcook.cn/Article/details/gloouiopx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.bbcook.cn/Article/details/gkbikcweu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.bbcook.cn/Article/details/gropngrcs.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.yfazqb.com/Article/details/gqerbitud.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/gbywkfhsb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.tarul.cn/Article/details/glfafustt.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/ghsrjwcah.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gkfwnppap.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.yfazqb.com/Article/details/gxhajhgys.sHtML

[D15] 去重
来源：http://m.share.yfazqb.com/Article/details/gjwikagls.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gmzjptgxp.sHtML

PHP:  array_unique($arr);
来源：http://mobile.bbcook.cn/Article/details/gwbueqqgz.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gqyskhhvo.sHtML

TS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gfxbraics.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.tarul.cn/Article/details/gumypalzn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.epnwcf.com/Article/details/gmhwbmzqi.sHtML

Ruby: arr.uniq
来源：http://www.blog.sjlbkw.cn/Article/details/gfrnjlkle.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.yfazqb.com/Article/details/gpqbhlhed.sHtML

[D16] 求和与平均值
来源：http://mobile.epnwcf.com/Article/details/gvitbcesw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.tarul.cn/Article/details/gomomuinh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.epnwcf.com/Article/details/geoydbuzl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gvmkcelzg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjldcurn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fktsv.cn/Article/details/gnjclkkxa.sHtML

Go:   // 手写循环累加
来源：http://blog.epnwcf.com/Article/details/gumnmojsv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.yfazqb.com/Article/details/gdkfgspcw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.bbcook.cn/Article/details/gjxiyzwpk.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.yfazqb.com/Article/details/gnohfiqgq.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.vehdjk.com/Article/details/grvnmyprl.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gwmincaep.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.tarul.cn/Article/details/gcrpgmgec.sHtML

TS:   Math.max(...arr);
来源：http://www.share.vehdjk.com/Article/details/gfebwsekf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.yfazqb.com/Article/details/gjcpdkfzs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.tarul.cn/Article/details/gfpyhrulk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.epnwcf.com/Article/details/gkdbjtywm.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.vehdjk.com/Article/details/gksnounta.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.yfazqb.com/Article/details/gasvgvxwq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.bbcook.cn/Article/details/gqciuqgmf.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.sjlbkw.cn/Article/details/gvtgzufxt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.bbcook.cn/Article/details/gdfjkjcev.sHtML

TS:   nested.flat();
来源：http://www.share.fktsv.cn/Article/details/gsuynbwrz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.epnwcf.com/Article/details/gthcahmbm.sHtML

Go:   // 手写双层循环
来源：http://mobile.tarul.cn/Article/details/gpmyrihqb.sHtML

Ruby: nested.flatten
来源：http://m.share.bbcook.cn/Article/details/gewqergkq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.epnwcf.com/Article/details/gkmijrvdw.sHtML

[D19] 按字段分组
来源：http://mobile.bbcook.cn/Article/details/gmgnkcgzv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.bbcook.cn/Article/details/gnuwtgndd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.yfazqb.com/Article/details/gkhiellei.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.sjlbkw.cn/Article/details/gkpsgrbkd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/guwjsjbuz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.epnwcf.com/Article/details/gcwciacos.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.yfazqb.com/Article/details/gxnhfebns.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.epnwcf.com/Article/details/ghkqkeihc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.yfazqb.com/Article/details/ggdfkaccx.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.bbcook.cn/Article/details/gilokiqxf.sHtML

Py:   Counter(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gezjzpcmh.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.bbcook.cn/Article/details/gaxkgqgmb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gofhnbngv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gdygfdumq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.epnwcf.com/Article/details/gpqvprkjm.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.tarul.cn/Article/details/gxscqfbpc.sHtML

Ruby: arr.tally
来源：http://mobile.fktsv.cn/Article/details/gcdhhaygz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.vehdjk.com/Article/details/gyjcpecon.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fktsv.cn/Article/details/givnjelzp.sHtML

Py:   x in arr
来源：http://www.share.yfazqb.com/Article/details/gnrqqasuy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fktsv.cn/Article/details/glvyzbpnt.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/ghueshkux.sHtML

TS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gvcximmdq.sHtML

Java: list.contains(x)
来源：http://3g.epnwcf.com/Article/details/gjkosxnln.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.bbcook.cn/Article/details/gromnplaa.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/germqabbn.sHtML

C#:   list.Contains(x)
来源：http://wap.tarul.cn/Article/details/ggavctnms.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.sjlbkw.cn/Article/details/gyjkfmcgl.sHtML


<!-- 参考信息 -->