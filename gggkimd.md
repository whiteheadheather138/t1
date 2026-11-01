代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.epnwcf.com/Article/details/gaidpbmtk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.tarul.cn/Article/details/gzwimmevu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.sjlbkw.cn/Article/details/gvhquzlxh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.vehdjk.com/Article/details/gftrhyobt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.bbcook.cn/Article/details/gftnrbpzk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/gzsaxzqbt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.bbcook.cn/Article/details/gkvwgshgs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fktsv.cn/Article/details/guksdzkgw.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.sjlbkw.cn/Article/details/gckpzneiu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gpquasidr.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gbznhgcwf.sHtML

[C05] 返回多个值
来源：http://read.share.bbcook.cn/Article/details/gbigpomdl.sHtML

Py:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gxxnseywm.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.tarul.cn/Article/details/gtzjzckqo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.epnwcf.com/Article/details/gtrwparzj.sHtML

TS:   return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gkoikzbfu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.vehdjk.com/Article/details/grhaumbpu.sHtML

Go:   return a, b
来源：http://3g.bbcook.cn/Article/details/gkfctngxh.sHtML

Ruby: return a, b
来源：http://baike.bbcook.cn/Article/details/goyfickxt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.bbcook.cn/Article/details/gptwmsnxb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fktsv.cn/Article/details/gnzlmcpng.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.epnwcf.com/Article/details/gzzaxwegn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.bbcook.cn/Article/details/gxtlgvfgd.sHtML

JS:   const square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/gdpmlntdj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gjksebpys.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fktsv.cn/Article/details/gojhvsfcb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.tarul.cn/Article/details/gxusigeok.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.bbcook.cn/Article/details/ghdnjwmdw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/gzitanhuf.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.epnwcf.com/Article/details/gsjrttzeo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.tarul.cn/Article/details/gyooqoujf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.tarul.cn/Article/details/gwmvzjuif.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.vehdjk.com/Article/details/grmvjghlx.sHtML

TS:   arr.map(String)
来源：http://wap.bbcook.cn/Article/details/gpvwskxyk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.tarul.cn/Article/details/gwvejfpro.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.bbcook.cn/Article/details/giouuqzuf.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.bbcook.cn/Article/details/gwhmsiqvn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.epnwcf.com/Article/details/ggqaysqja.sHtML

[C08] 闭包
来源：http://www.blog.fktsv.cn/Article/details/gnlivpduv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fktsv.cn/Article/details/gqhbkanzk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.vehdjk.com/Article/details/gwalkpaeq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/geoakglst.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtfvwxuzz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fktsv.cn/Article/details/gnumwtvvy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.bbcook.cn/Article/details/gqzcrwgex.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.sjlbkw.cn/Article/details/gcctlsxnt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gomrkbhdv.sHtML

[C09] 递归
来源：http://www.blog.vehdjk.com/Article/details/gudxbnurb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gpqgljjmn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.vehdjk.com/Article/details/gjsescrlg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/gvpfzyggg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/geckhfgqp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.bbcook.cn/Article/details/gghbvzdyq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.vehdjk.com/Article/details/gauwtukhg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gitrnenho.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.tarul.cn/Article/details/gufcadwfb.sHtML

[C10] 变量作用域
来源：http://m.share.epnwcf.com/Article/details/gunxvdqeq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.epnwcf.com/Article/details/gmikhnjro.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.epnwcf.com/Article/details/gswdajxrv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.yfazqb.com/Article/details/gjgskmqvv.sHtML

TS:   同 JS
来源：http://3g.bbcook.cn/Article/details/gwfjwspzz.sHtML

Java: 方法内为块级作用域
来源：http://3g.vehdjk.com/Article/details/gmehnjyfu.sHtML

Go:   花括号块级作用域
来源：http://3g.bbcook.cn/Article/details/gnyuppytx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.tarul.cn/Article/details/gvbzzghap.sHtML

C#:   块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gzgsvfedl.sHtML

[C11] 模块导入与导出
来源：http://www.blog.yfazqb.com/Article/details/gljwvzusf.sHtML

Py:   from module import func
来源：http://baike.tarul.cn/Article/details/ghoeweoqx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.bbcook.cn/Article/details/gzdkyykxj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.epnwcf.com/Article/details/goyfbjmdl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.vehdjk.com/Article/details/gbexnitkc.sHtML

Java: import java.util.List;
来源：http://wap.tarul.cn/Article/details/grihaqlop.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.bbcook.cn/Article/details/gfthwmesw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.vehdjk.com/Article/details/gtumdiink.sHtML

C#:   using System.Text;
来源：http://3g.vehdjk.com/Article/details/glkyzymwk.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.vehdjk.com/Article/details/glryfdlxi.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.tarul.cn/Article/details/gaugxobwq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.yfazqb.com/Article/details/gkcdjbfrd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/ggmymylca.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/glizjljic.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fktsv.cn/Article/details/gedpmakcm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.vehdjk.com/Article/details/gtzuixtaq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fktsv.cn/Article/details/gdmhihfaz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gleeduedj.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.sjlbkw.cn/Article/details/gfjpwacsz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.yfazqb.com/Article/details/guaftiulq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gxgqgenbt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.yfazqb.com/Article/details/gfuskrshm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gwicutpwv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gvzdwwzgn.sHtML

Go:   func add(a, b int) int
来源：http://m.share.epnwcf.com/Article/details/gmwpmhscj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.sjlbkw.cn/Article/details/gpjjdnmos.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.epnwcf.com/Article/details/gabhalxot.sHtML

[C14] 泛型函数
来源：http://wap.epnwcf.com/Article/details/gpaadfgjd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.sjlbkw.cn/Article/details/gjxeicynv.sHtML

PHP:  // 无泛型
来源：http://blog.yfazqb.com/Article/details/gydiqhhik.sHtML

JS:   // 无泛型
来源：http://wap.tarul.cn/Article/details/gnuysjllz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fktsv.cn/Article/details/gqlnqqitr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.bbcook.cn/Article/details/gtiwxeesn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.yfazqb.com/Article/details/gjxgwpsuq.sHtML

Ruby: # 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gtcjozldd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.bbcook.cn/Article/details/gvrtpxpwe.sHtML

[C15] 解构 / 展开参数
来源：http://wap.epnwcf.com/Article/details/gjnyfsopf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fktsv.cn/Article/details/gkcxtovrw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.sjlbkw.cn/Article/details/gojwbuyzd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gnggtofnq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fktsv.cn/Article/details/gydjauyvc.sHtML

Java: // 无解构
来源：http://m.share.yfazqb.com/Article/details/gpzshqclm.sHtML

Go:   // 无解构
来源：http://m.share.tarul.cn/Article/details/gfygbbguj.sHtML

Ruby: a, b = pair
来源：http://read.share.fktsv.cn/Article/details/gdemowcre.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fktsv.cn/Article/details/gnrhjfocm.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.epnwcf.com/Article/details/gbczcikwx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.yfazqb.com/Article/details/gqtsbnnax.sHtML

PHP:  // 无重载
来源：http://3g.sjlbkw.cn/Article/details/gbcoqlrbk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.vehdjk.com/Article/details/gnhriynuc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.tarul.cn/Article/details/gtfljrhss.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.tarul.cn/Article/details/gtawtmfzl.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.epnwcf.com/Article/details/gfgtzxzew.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.epnwcf.com/Article/details/gktnlntmm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.sjlbkw.cn/Article/details/gbxfkkfkv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gkkambufk.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.vehdjk.com/Article/details/gsbwxbnnm.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gimesuxzq.sHtML

[D01] 创建数组 / 列表
来源：http://wap.vehdjk.com/Article/details/gdjirbxyv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.yfazqb.com/Article/details/gowigokvn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fktsv.cn/Article/details/gabpajpdx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fktsv.cn/Article/details/guucopcyc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.sjlbkw.cn/Article/details/gibirfvns.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fktsv.cn/Article/details/gyujhnirf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.tarul.cn/Article/details/ggrsekslc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.vehdjk.com/Article/details/gxoseocqd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.bbcook.cn/Article/details/gsxvsdydx.sHtML

[D02] 追加元素到末尾
来源：http://baike.sjlbkw.cn/Article/details/gyzyytkwu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.vehdjk.com/Article/details/gholxffwp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.bbcook.cn/Article/details/gndfoeeph.sHtML

JS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/grqafzmgu.sHtML

TS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gfechqgyn.sHtML

Java: list.add(4);
来源：http://www.blog.fktsv.cn/Article/details/gbxyuucgp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/grytuamjv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.tarul.cn/Article/details/gwyiyjsyc.sHtML

C#:   list.Add(4);
来源：http://read.share.epnwcf.com/Article/details/gdkecobkx.sHtML

[D03] 在指定位置插入元素
来源：http://wap.tarul.cn/Article/details/gdpgskxjs.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.vehdjk.com/Article/details/gzzukvpcx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fktsv.cn/Article/details/gwstginhn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.bbcook.cn/Article/details/gswuouqqf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.yfazqb.com/Article/details/gswvbgnqg.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gqvwhxdik.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.epnwcf.com/Article/details/gnnysrskj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fktsv.cn/Article/details/gjsvehpew.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/gjtdqfibq.sHtML

[D04] 删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/grraanldr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.tarul.cn/Article/details/guqyxotck.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fktsv.cn/Article/details/gnmjpqtex.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.bbcook.cn/Article/details/gwacthcxb.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.sjlbkw.cn/Article/details/gtyrndlgi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.vehdjk.com/Article/details/gvyiouayv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.epnwcf.com/Article/details/gtctexixa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.tarul.cn/Article/details/gikohipwu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.vehdjk.com/Article/details/gibrliwav.sHtML

[D05] 访问与修改元素
来源：http://read.share.tarul.cn/Article/details/gjyfhqqzv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gcliezhsq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gzxsjkeoj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/ggptgwpsx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fktsv.cn/Article/details/gaihuyvbe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.tarul.cn/Article/details/gxgcehyzi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/grgvpvzsb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/gokftyhvy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fktsv.cn/Article/details/grssmybat.sHtML

[D06] 数组长度
来源：http://baike.vehdjk.com/Article/details/gmywywavm.sHtML

Py:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/ghrdpluso.sHtML

PHP:  count($arr);
来源：http://mobile.tarul.cn/Article/details/ggkvbwvhr.sHtML

JS:   arr.length
来源：http://blog.yfazqb.com/Article/details/greilndlk.sHtML

TS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/gqlujqalh.sHtML

Java: list.size();
来源：http://www.share.epnwcf.com/Article/details/gfdngwxkx.sHtML

Go:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/giamymzzm.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fktsv.cn/Article/details/glmeikvtn.sHtML

C#:   list.Count;
来源：http://www.m.share.epnwcf.com/Article/details/gfyjorciu.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.bbcook.cn/Article/details/gpmaqnqgw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.vehdjk.com/Article/details/geohkbxiq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gvrgcbzro.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gnhlqwstb.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/goonyrkoh.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gobrnibsh.sHtML

Go:   arr[1:4]
来源：http://blog.yfazqb.com/Article/details/gnbicxggq.sHtML

Ruby: arr[1, 3]
来源：http://blog.sjlbkw.cn/Article/details/gmegqzsvv.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.tarul.cn/Article/details/gpgntuooy.sHtML

[D08] 合并两个数组
来源：http://mobile.vehdjk.com/Article/details/gheyctajz.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.epnwcf.com/Article/details/gjzdhvurn.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.bbcook.cn/Article/details/gqxpsnzcn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.yfazqb.com/Article/details/gcuqhyxav.sHtML

TS:   [...a, ...b];
来源：http://mobile.sjlbkw.cn/Article/details/gqrbqssoh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fktsv.cn/Article/details/gmkyeewhc.sHtML

Go:   append(a, b...)
来源：http://read.share.yfazqb.com/Article/details/gospwwfmj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.yfazqb.com/Article/details/gsfnhykbj.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.tarul.cn/Article/details/gujguqhpv.sHtML

[D09] 排序（升序）
来源：http://www.blog.vehdjk.com/Article/details/gulewpmip.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gigqinbfx.sHtML

PHP:  sort($arr);
来源：http://read.share.bbcook.cn/Article/details/gxgyoukhj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.vehdjk.com/Article/details/gteryemfb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.tarul.cn/Article/details/guuhlmaui.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.sjlbkw.cn/Article/details/gelbvsuxi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/gfarupgnh.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/gjjlutlwn.sHtML

C#:   list.Sort();
来源：http://baike.vehdjk.com/Article/details/gwpockszm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.sjlbkw.cn/Article/details/gspjxpahn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fktsv.cn/Article/details/geumiheza.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gbbsxrdbm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gysbhmrqi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fktsv.cn/Article/details/glvnegaea.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.tarul.cn/Article/details/gmtdxwcya.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.sjlbkw.cn/Article/details/gydxgsmce.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.bbcook.cn/Article/details/ggpbuhded.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.tarul.cn/Article/details/gzespxusp.sHtML

[D11] 反转数组
来源：http://wap.sjlbkw.cn/Article/details/gwsgfifwc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.sjlbkw.cn/Article/details/ghfwpvare.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fktsv.cn/Article/details/gqskbrdsc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fktsv.cn/Article/details/ghirtoizi.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.bbcook.cn/Article/details/gpzyzfork.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fktsv.cn/Article/details/gtluxrogu.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.epnwcf.com/Article/details/gqycpdqww.sHtML

Ruby: arr.reverse
来源：http://3g.yfazqb.com/Article/details/gntsrhhcn.sHtML

C#:   list.Reverse();
来源：http://mobile.tarul.cn/Article/details/gyztvarzz.sHtML

[D12] 查找元素下标
来源：http://3g.sjlbkw.cn/Article/details/gryxzqmiy.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.tarul.cn/Article/details/gvyrgfjna.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.epnwcf.com/Article/details/gkiytzfyu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/gpehiqkju.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.yfazqb.com/Article/details/ggvtxlqvu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.vehdjk.com/Article/details/gzrrocvjl.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fktsv.cn/Article/details/gvsgpqsey.sHtML

Ruby: arr.index(x)
来源：http://m.share.bbcook.cn/Article/details/ggfrqkvih.sHtML

C#:   list.IndexOf(x);
来源：http://baike.sjlbkw.cn/Article/details/gevinmgqc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fktsv.cn/Article/details/gxeykhpyk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fktsv.cn/Article/details/ghsyvyagr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.yfazqb.com/Article/details/gerjaokqk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/grxlwpqcg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/gukmengez.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.sjlbkw.cn/Article/details/gwnoirrke.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.tarul.cn/Article/details/goicrngjg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fktsv.cn/Article/details/gjcbbgkdj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fktsv.cn/Article/details/grsogzptq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.vehdjk.com/Article/details/gozcdeszm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gmmvcxuph.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.bbcook.cn/Article/details/gtpffdlaq.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gkxmhushc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gnpsslpco.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gvsikvzlq.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/gijibqjjb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.yfazqb.com/Article/details/glohbbtde.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.tarul.cn/Article/details/gyvhcrbrf.sHtML

[D15] 去重
来源：http://www.share.vehdjk.com/Article/details/grdzdcurk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/gvpvdpmwk.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/gfatsraiy.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gtuyyvooe.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/ghzlgamou.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.tarul.cn/Article/details/gtubycxtw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.tarul.cn/Article/details/gdmvijmog.sHtML

Ruby: arr.uniq
来源：http://mobile.yfazqb.com/Article/details/gqfcqpxls.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.epnwcf.com/Article/details/gdfpgpnjt.sHtML

[D16] 求和与平均值
来源：http://m.share.sjlbkw.cn/Article/details/gypkveivv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gvvzvebnn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.vehdjk.com/Article/details/gunzpzqxf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gfoomlnur.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gtmqxueae.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/gguexozbr.sHtML

Go:   // 手写循环累加
来源：http://baike.epnwcf.com/Article/details/gjllambdd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.vehdjk.com/Article/details/gzuwvuhhb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fktsv.cn/Article/details/guxbvhxlb.sHtML

[D17] 最大值与最小值
来源：http://blog.tarul.cn/Article/details/gvcwsdrtp.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.epnwcf.com/Article/details/gkhrtjxgb.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gjucpfjsb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.yfazqb.com/Article/details/giwlrnqpx.sHtML

TS:   Math.max(...arr);
来源：http://baike.yfazqb.com/Article/details/gkimjzfhu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.yfazqb.com/Article/details/gfynwiucg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.vehdjk.com/Article/details/gqrxxxilb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.bbcook.cn/Article/details/guosqpqhj.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fktsv.cn/Article/details/gmvkmfvur.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.vehdjk.com/Article/details/gpxkueqir.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.epnwcf.com/Article/details/ggogkfrva.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.epnwcf.com/Article/details/gegqcffwa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.vehdjk.com/Article/details/gdwoxztol.sHtML

TS:   nested.flat();
来源：http://www.blog.sjlbkw.cn/Article/details/geulghvzh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.epnwcf.com/Article/details/ggumosuha.sHtML

Go:   // 手写双层循环
来源：http://baike.bbcook.cn/Article/details/gweagapvy.sHtML

Ruby: nested.flatten
来源：http://mobile.fktsv.cn/Article/details/gdxyfkgvs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.epnwcf.com/Article/details/gobpqafzu.sHtML

[D19] 按字段分组
来源：http://blog.vehdjk.com/Article/details/ghvpsoqdn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.epnwcf.com/Article/details/gydbsttkh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.epnwcf.com/Article/details/gqdocgxjw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.tarul.cn/Article/details/gfbmogacv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gxcfrwnii.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.yfazqb.com/Article/details/globyeelj.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.bbcook.cn/Article/details/gchceppbq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.vehdjk.com/Article/details/gvxvjqaff.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.vehdjk.com/Article/details/glztogeig.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.bbcook.cn/Article/details/gmlvggeme.sHtML

Py:   Counter(arr)
来源：http://read.share.fktsv.cn/Article/details/gkmhphdid.sHtML

PHP:  array_count_values($arr);
来源：http://baike.sjlbkw.cn/Article/details/gipotldun.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gawjewzvv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/gcfgrndjh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.vehdjk.com/Article/details/gjeamugag.sHtML

Go:   // 手写 map[T]int
来源：http://baike.bbcook.cn/Article/details/gnqmnomws.sHtML


<!-- 参考信息 -->