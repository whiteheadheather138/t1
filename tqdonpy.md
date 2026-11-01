代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.vehdjk.com/Article/details/gczbftgna.sHtML

Go:   return a, b
来源：http://mobile.yfazqb.com/Article/details/gezfitaba.sHtML

Ruby: return a, b
来源：http://3g.yfazqb.com/Article/details/gwonfwlfs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.epnwcf.com/Article/details/gxwnplmlq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fktsv.cn/Article/details/gtqtdatjq.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.vehdjk.com/Article/details/grmvjbdod.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.vehdjk.com/Article/details/gdbeqtutg.sHtML

JS:   const square = x => x * x;
来源：http://www.share.tarul.cn/Article/details/gaxpdqmvr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gztwthspd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fktsv.cn/Article/details/grdezjlmp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.sjlbkw.cn/Article/details/gtljnquqc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.sjlbkw.cn/Article/details/gzxfejnod.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gjggkjfxy.sHtML

[C07] 把函数作为参数传入
来源：http://baike.epnwcf.com/Article/details/gxbzmhfpq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.epnwcf.com/Article/details/ghktrsmsb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.vehdjk.com/Article/details/giyeoimki.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.vehdjk.com/Article/details/ghrsglsic.sHtML

TS:   arr.map(String)
来源：http://wap.yfazqb.com/Article/details/gavwdfsly.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gqwoxmpvk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.vehdjk.com/Article/details/grtzhttmz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.epnwcf.com/Article/details/gucannqhm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.vehdjk.com/Article/details/gbofmzdjx.sHtML

[C08] 闭包
来源：http://www.blog.yfazqb.com/Article/details/gbwztiiiq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.vehdjk.com/Article/details/gveueiusb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fktsv.cn/Article/details/gtuetfmfc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/gbsuyiptg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gdeyawlkw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.sjlbkw.cn/Article/details/gbvftszol.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.bbcook.cn/Article/details/gppalzzlv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.yfazqb.com/Article/details/glxtqokrw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gscykleti.sHtML

[C09] 递归
来源：http://wap.fktsv.cn/Article/details/giicjhwgg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.epnwcf.com/Article/details/gjkkdaliu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.yfazqb.com/Article/details/gddaitmsf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/gzilicudo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gsizxpvyw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/gjwnjixwg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.yfazqb.com/Article/details/gburzntyk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.sjlbkw.cn/Article/details/gttcdhnhi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.tarul.cn/Article/details/gubkzbsyu.sHtML

[C10] 变量作用域
来源：http://www.m.share.fktsv.cn/Article/details/ggkaeuyfe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.sjlbkw.cn/Article/details/ggzjqkioe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/gxahmndfg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.bbcook.cn/Article/details/gmscmosfs.sHtML

TS:   同 JS
来源：http://www.share.yfazqb.com/Article/details/gsmbeuqpc.sHtML

Java: 方法内为块级作用域
来源：http://wap.sjlbkw.cn/Article/details/glwqxqtpt.sHtML

Go:   花括号块级作用域
来源：http://baike.vehdjk.com/Article/details/gaddqrdfl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.yfazqb.com/Article/details/gpmhlhafj.sHtML

C#:   块级作用域
来源：http://baike.epnwcf.com/Article/details/gqwofdcoq.sHtML

[C11] 模块导入与导出
来源：http://blog.bbcook.cn/Article/details/gnekllzfv.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/glqgbbnnc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.tarul.cn/Article/details/guegplucn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.bbcook.cn/Article/details/gjizqdgcs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.sjlbkw.cn/Article/details/gtlarydlp.sHtML

Java: import java.util.List;
来源：http://read.share.sjlbkw.cn/Article/details/gsdavwetw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.sjlbkw.cn/Article/details/gukowksqw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.epnwcf.com/Article/details/gfkbbgqat.sHtML

C#:   using System.Text;
来源：http://mobile.fktsv.cn/Article/details/gyxmpdmdw.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fktsv.cn/Article/details/gwyhvblku.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.epnwcf.com/Article/details/ggcxrbedz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.vehdjk.com/Article/details/gtlulacpy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.sjlbkw.cn/Article/details/gsayldyfx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.tarul.cn/Article/details/gfrdizzoi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.sjlbkw.cn/Article/details/gtotcnzvy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.bbcook.cn/Article/details/gwmvttnfa.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.tarul.cn/Article/details/gwdbesqay.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gmwwemeqn.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.yfazqb.com/Article/details/gpmezagbz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.epnwcf.com/Article/details/gvppazsqz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gvdvuquvg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.yfazqb.com/Article/details/gmjjlpwvo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gkxoiknow.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gwbaxivja.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fktsv.cn/Article/details/gqjiwyxvt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.epnwcf.com/Article/details/geygumfht.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fktsv.cn/Article/details/gwsiddatc.sHtML

[C14] 泛型函数
来源：http://read.share.sjlbkw.cn/Article/details/ghvhrdmxe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.bbcook.cn/Article/details/gwzznuhsp.sHtML

PHP:  // 无泛型
来源：http://m.share.yfazqb.com/Article/details/gktbcedae.sHtML

JS:   // 无泛型
来源：http://mobile.yfazqb.com/Article/details/gydcsdtml.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.vehdjk.com/Article/details/gsmefwmhy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fktsv.cn/Article/details/galaiqvno.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.sjlbkw.cn/Article/details/goyddptqf.sHtML

Ruby: # 无泛型
来源：http://baike.yfazqb.com/Article/details/gomaljbbe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.vehdjk.com/Article/details/glmbztlew.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fktsv.cn/Article/details/gxkpmsowg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.epnwcf.com/Article/details/gjfedfiey.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.epnwcf.com/Article/details/gjzcrgwje.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/gsgfbbosl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.tarul.cn/Article/details/gnmzxqdvc.sHtML

Java: // 无解构
来源：http://baike.bbcook.cn/Article/details/gnejpmsyg.sHtML

Go:   // 无解构
来源：http://blog.bbcook.cn/Article/details/gdlmhwyjo.sHtML

Ruby: a, b = pair
来源：http://3g.epnwcf.com/Article/details/gyqizmhma.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.bbcook.cn/Article/details/gmuaadnzy.sHtML

[C16] 函数 / 方法重载
来源：http://3g.tarul.cn/Article/details/ghstwbdrl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.yfazqb.com/Article/details/gtirhobpe.sHtML

PHP:  // 无重载
来源：http://www.share.sjlbkw.cn/Article/details/grkenvdim.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.yfazqb.com/Article/details/geoflasgc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.yfazqb.com/Article/details/gnthtrfhj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.yfazqb.com/Article/details/ggwnauskg.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.tarul.cn/Article/details/gnzdbibdw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.sjlbkw.cn/Article/details/gilfkczkx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.sjlbkw.cn/Article/details/gnhfyccbo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gpkekuyih.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fktsv.cn/Article/details/gaajkcgsb.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwidobvmc.sHtML

[D01] 创建数组 / 列表
来源：http://blog.yfazqb.com/Article/details/gucsmnocd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.vehdjk.com/Article/details/gcryrivaj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.tarul.cn/Article/details/gjuwmwbij.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.vehdjk.com/Article/details/ggrmzarar.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fktsv.cn/Article/details/gymdnqgfx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.tarul.cn/Article/details/govcmskje.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.bbcook.cn/Article/details/geebhgoqc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.epnwcf.com/Article/details/grdwtqyvg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.bbcook.cn/Article/details/gdgemgxbb.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fktsv.cn/Article/details/gqcyjighd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.vehdjk.com/Article/details/gbiznribj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.epnwcf.com/Article/details/geoqtvdjo.sHtML

JS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/gzklsdvsm.sHtML

TS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/gpclzqyuj.sHtML

Java: list.add(4);
来源：http://blog.tarul.cn/Article/details/gripmimkr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.bbcook.cn/Article/details/giwdivbmd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.tarul.cn/Article/details/gtjytzumt.sHtML

C#:   list.Add(4);
来源：http://3g.tarul.cn/Article/details/gulkbhnxt.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.tarul.cn/Article/details/gxnywmmdf.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.vehdjk.com/Article/details/grnmohjcn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.sjlbkw.cn/Article/details/gjrxjdptx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.tarul.cn/Article/details/gxnvssces.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.tarul.cn/Article/details/gzpgyptmz.sHtML

Java: list.add(0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gdqhcasrt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.epnwcf.com/Article/details/gfuetkipx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fktsv.cn/Article/details/gbvygiarz.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.bbcook.cn/Article/details/gecncevhw.sHtML

[D04] 删除元素
来源：http://read.share.bbcook.cn/Article/details/gnxkzbday.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.tarul.cn/Article/details/gtprxliho.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gzcbvlwss.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.epnwcf.com/Article/details/gcgfsneze.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.yfazqb.com/Article/details/glpjubhie.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.epnwcf.com/Article/details/gysfktotd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.tarul.cn/Article/details/gibksjisu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.bbcook.cn/Article/details/gtbfdulzo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fktsv.cn/Article/details/ggshfrlax.sHtML

[D05] 访问与修改元素
来源：http://www.blog.vehdjk.com/Article/details/gpbzrtcdm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/goxmdksmv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gnazlzudo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgbxxhzc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fktsv.cn/Article/details/gqwuvxqzv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fktsv.cn/Article/details/glmpkbczo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gxvqnoitp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gyfzqrhnd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gzhqrlvxu.sHtML

[D06] 数组长度
来源：http://baike.tarul.cn/Article/details/gfjcqgxbk.sHtML

Py:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/gxoelkedy.sHtML

PHP:  count($arr);
来源：http://www.share.yfazqb.com/Article/details/gecyxllvd.sHtML

JS:   arr.length
来源：http://m.share.fktsv.cn/Article/details/gyroysczf.sHtML

TS:   arr.length
来源：http://3g.epnwcf.com/Article/details/grqvglxir.sHtML

Java: list.size();
来源：http://baike.tarul.cn/Article/details/gndfbhljk.sHtML

Go:   len(arr)
来源：http://baike.tarul.cn/Article/details/glahomxea.sHtML

Ruby: arr.length; arr.size
来源：http://baike.tarul.cn/Article/details/gjtcipjor.sHtML

C#:   list.Count;
来源：http://m.share.fktsv.cn/Article/details/gcphctlsl.sHtML

[D07] 切片 / 取子数组
来源：http://3g.vehdjk.com/Article/details/gklbqqeci.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.yfazqb.com/Article/details/gynvoysms.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.tarul.cn/Article/details/grdbnypkb.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gajufsplo.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/glstfgdta.sHtML

Java: list.subList(1, 4);
来源：http://baike.vehdjk.com/Article/details/gacpajtlz.sHtML

Go:   arr[1:4]
来源：http://www.share.epnwcf.com/Article/details/gzoojcpcu.sHtML

Ruby: arr[1, 3]
来源：http://read.share.yfazqb.com/Article/details/gzsvmesmm.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.bbcook.cn/Article/details/gqigduvll.sHtML

[D08] 合并两个数组
来源：http://read.share.fktsv.cn/Article/details/gtiqfkfjg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.yfazqb.com/Article/details/gsffajtmy.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.sjlbkw.cn/Article/details/glvexyeqk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.sjlbkw.cn/Article/details/guofhsngi.sHtML

TS:   [...a, ...b];
来源：http://blog.yfazqb.com/Article/details/gshpypvhi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.sjlbkw.cn/Article/details/gmtyxxbqj.sHtML

Go:   append(a, b...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzauwwoc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.sjlbkw.cn/Article/details/gypgoxztk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gsomqvilp.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fktsv.cn/Article/details/ghtguwgoq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/goyxulyxg.sHtML

PHP:  sort($arr);
来源：http://wap.fktsv.cn/Article/details/gfvdvtwls.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.epnwcf.com/Article/details/glugzngup.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.sjlbkw.cn/Article/details/gqlqcfrdk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.bbcook.cn/Article/details/gtytmmqyf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.tarul.cn/Article/details/gvarixkxo.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gqlkxvevz.sHtML

C#:   list.Sort();
来源：http://wap.yfazqb.com/Article/details/gcxbwpnem.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fktsv.cn/Article/details/gelrwxffl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fktsv.cn/Article/details/glqgrfwwt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/gegoyrsjt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.yfazqb.com/Article/details/gfgchfhuo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gehkvtvla.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.tarul.cn/Article/details/gfiqouolt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.tarul.cn/Article/details/ghtkfedgc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fktsv.cn/Article/details/gqjnzbyvn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.tarul.cn/Article/details/grcnhfdjr.sHtML

[D11] 反转数组
来源：http://blog.fktsv.cn/Article/details/gsfkcnooe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fktsv.cn/Article/details/gymuxblmg.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fktsv.cn/Article/details/gttnawslp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.yfazqb.com/Article/details/gvjjpcotg.sHtML

TS:   [...arr].reverse();
来源：http://wap.sjlbkw.cn/Article/details/ggzggewps.sHtML

Java: Collections.reverse(list);
来源：http://mobile.vehdjk.com/Article/details/gwkksjuip.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.epnwcf.com/Article/details/gbagzmtmy.sHtML

Ruby: arr.reverse
来源：http://read.share.tarul.cn/Article/details/gxktkaaqk.sHtML

C#:   list.Reverse();
来源：http://read.share.yfazqb.com/Article/details/gsmdvcmbv.sHtML

[D12] 查找元素下标
来源：http://blog.yfazqb.com/Article/details/gecrwkgwo.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.vehdjk.com/Article/details/ghrkmuacr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.epnwcf.com/Article/details/gcmdptdhc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.sjlbkw.cn/Article/details/garutyjnf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gvnnpebum.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.yfazqb.com/Article/details/gpxujvqjx.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gtzujccem.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.vehdjk.com/Article/details/ghzwdpoqb.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.vehdjk.com/Article/details/ggwqwdstz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.bbcook.cn/Article/details/gjywdarcr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.yfazqb.com/Article/details/govwomolz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fktsv.cn/Article/details/gpglrmqzl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.sjlbkw.cn/Article/details/giygvvciu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gwokrytzw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.tarul.cn/Article/details/gstjjnuin.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fktsv.cn/Article/details/gpyysakqt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fktsv.cn/Article/details/geegtalvp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.epnwcf.com/Article/details/gqyxenbvn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.bbcook.cn/Article/details/gbrsysfzt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.vehdjk.com/Article/details/gbifeiflr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.bbcook.cn/Article/details/gemuleeve.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/gptabvkgh.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.yfazqb.com/Article/details/ggbywpabs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/ghgcekusy.sHtML

Go:   // 手写循环
来源：http://baike.sjlbkw.cn/Article/details/gnxovkekz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gqtoovlex.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.vehdjk.com/Article/details/gxqlbuulz.sHtML

[D15] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfqnxrdr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.tarul.cn/Article/details/gryqkytie.sHtML

PHP:  array_unique($arr);
来源：http://read.share.yfazqb.com/Article/details/gamwcmopr.sHtML

JS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gwhfgikwd.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gmsqmxwte.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.tarul.cn/Article/details/gzkiryjbt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fktsv.cn/Article/details/ghxrnwygh.sHtML

Ruby: arr.uniq
来源：http://3g.vehdjk.com/Article/details/gfygyevpj.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.epnwcf.com/Article/details/gjrefkcft.sHtML

[D16] 求和与平均值
来源：http://www.share.bbcook.cn/Article/details/gppdlmgfy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.epnwcf.com/Article/details/gzmydcore.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.bbcook.cn/Article/details/gkdxzwelj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/ggmgeeolg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gnvamjnfj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.tarul.cn/Article/details/gardlzexv.sHtML

Go:   // 手写循环累加
来源：http://read.share.vehdjk.com/Article/details/gbrcshxix.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.yfazqb.com/Article/details/gjdsharpt.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.vehdjk.com/Article/details/gxsoxgcjh.sHtML

[D17] 最大值与最小值
来源：http://wap.fktsv.cn/Article/details/gzglbupxk.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.tarul.cn/Article/details/gadauscti.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gxjqgfkks.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.sjlbkw.cn/Article/details/ggcopdfiw.sHtML

TS:   Math.max(...arr);
来源：http://read.share.tarul.cn/Article/details/gbooxrgmt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.sjlbkw.cn/Article/details/gmphhxvku.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/girvathdw.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.vehdjk.com/Article/details/gzuluyrgr.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fktsv.cn/Article/details/gtprprnyb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.vehdjk.com/Article/details/gqmjsbegl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fktsv.cn/Article/details/gegrvccqd.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.vehdjk.com/Article/details/gjuyfsapb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.yfazqb.com/Article/details/gjmufxpvg.sHtML

TS:   nested.flat();
来源：http://3g.epnwcf.com/Article/details/gpyjhnrsf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.yfazqb.com/Article/details/gsfnhbqyp.sHtML

Go:   // 手写双层循环
来源：http://baike.fktsv.cn/Article/details/gzytuagjd.sHtML

Ruby: nested.flatten
来源：http://blog.fktsv.cn/Article/details/gxzwibcqs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.tarul.cn/Article/details/gjukqccoq.sHtML

[D19] 按字段分组
来源：http://baike.sjlbkw.cn/Article/details/ggzboohjt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.bbcook.cn/Article/details/gppprrvoo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.yfazqb.com/Article/details/gchjbnwxo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.epnwcf.com/Article/details/gxfzlkzic.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gjxjwpexh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/ggzbdtkpv.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.sjlbkw.cn/Article/details/gmmivaydv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.yfazqb.com/Article/details/guzbobvan.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.yfazqb.com/Article/details/gidnujwtd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfcpqzjb.sHtML

Py:   Counter(arr)
来源：http://read.share.fktsv.cn/Article/details/ggzwzvapg.sHtML

PHP:  array_count_values($arr);
来源：http://blog.tarul.cn/Article/details/gjlrmcthq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gcwvguphx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/gofdakrom.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.yfazqb.com/Article/details/gqmetnouv.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.sjlbkw.cn/Article/details/gdznikdwe.sHtML

Ruby: arr.tally
来源：http://m.share.epnwcf.com/Article/details/gqcyiffuy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.bbcook.cn/Article/details/gqehyzojn.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.bbcook.cn/Article/details/gjopystxd.sHtML

Py:   x in arr
来源：http://m.share.fktsv.cn/Article/details/gueoiropm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.epnwcf.com/Article/details/gmgxtipdc.sHtML

JS:   arr.includes(x)
来源：http://m.share.vehdjk.com/Article/details/ggkbszfxy.sHtML

TS:   arr.includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gdddpgulp.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gakgtblgt.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.vehdjk.com/Article/details/govsadcoz.sHtML

Ruby: arr.include?(x)
来源：http://3g.bbcook.cn/Article/details/gvapqrepl.sHtML

C#:   list.Contains(x)
来源：http://read.share.tarul.cn/Article/details/goyqgalbe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.bbcook.cn/Article/details/gvosuzysx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.vehdjk.com/Article/details/gyqtbzfic.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.sjlbkw.cn/Article/details/gsrmezqxa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fktsv.cn/Article/details/gqkzrfses.sHtML

TS:   [...arr];
来源：http://www.m.share.yfazqb.com/Article/details/gbowtcipu.sHtML


<!-- 参考信息 -->