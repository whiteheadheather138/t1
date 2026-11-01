代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://blog.yfazqb.com/Article/details/gqfbwqtxu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.bbcook.cn/Article/details/gsfpjbxvc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.yfazqb.com/Article/details/gamhwnloo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fktsv.cn/Article/details/gipnqvktj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fktsv.cn/Article/details/goddzdfrt.sHtML

[C07] 把函数作为参数传入
来源：http://wap.sjlbkw.cn/Article/details/gvwkwnukd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.sjlbkw.cn/Article/details/gyefxzkgf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.bbcook.cn/Article/details/gaggccxrn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.epnwcf.com/Article/details/gltvmwukz.sHtML

TS:   arr.map(String)
来源：http://wap.vehdjk.com/Article/details/gxosjdsnk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.bbcook.cn/Article/details/gcugmzkfg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.yfazqb.com/Article/details/gwbjyvyop.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.vehdjk.com/Article/details/gzczxbeke.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.epnwcf.com/Article/details/gwbuuyhzy.sHtML

[C08] 闭包
来源：http://www.blog.bbcook.cn/Article/details/gsmouvmbf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.tarul.cn/Article/details/gabtlzlqi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gffturodp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gyznlukhe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gosytodwi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.yfazqb.com/Article/details/ggeixllut.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.vehdjk.com/Article/details/gzqxtpwfg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.bbcook.cn/Article/details/gvfzlnqcf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/guzscqnrt.sHtML

[C09] 递归
来源：http://3g.vehdjk.com/Article/details/gwzlwgtnf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gbiiblemv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gxtbdzqnr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gebsrscjv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.sjlbkw.cn/Article/details/gdetolbun.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gcumtwitj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.bbcook.cn/Article/details/gpnixfmie.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/gimckvxwi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.epnwcf.com/Article/details/gsxqcnarx.sHtML

[C10] 变量作用域
来源：http://m.share.yfazqb.com/Article/details/gkdcjaxzu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.yfazqb.com/Article/details/gdwrykiwh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.sjlbkw.cn/Article/details/gpbvvaaio.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fktsv.cn/Article/details/gajowpmqr.sHtML

TS:   同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gylyylrsh.sHtML

Java: 方法内为块级作用域
来源：http://3g.epnwcf.com/Article/details/glefdvxuc.sHtML

Go:   花括号块级作用域
来源：http://baike.bbcook.cn/Article/details/gjxiededa.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.yfazqb.com/Article/details/gcndfupby.sHtML

C#:   块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gfkmjqzow.sHtML

[C11] 模块导入与导出
来源：http://www.blog.yfazqb.com/Article/details/gvtudpvsx.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/gmhahmqcg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.yfazqb.com/Article/details/gonyivpjn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/gzybsfaag.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.tarul.cn/Article/details/gdizngczr.sHtML

Java: import java.util.List;
来源：http://www.share.sjlbkw.cn/Article/details/gxwjsuxru.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.sjlbkw.cn/Article/details/gzdwzauif.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.sjlbkw.cn/Article/details/gnkuijkxi.sHtML

C#:   using System.Text;
来源：http://baike.vehdjk.com/Article/details/gwwsxpprt.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.epnwcf.com/Article/details/gyehfxuuh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.bbcook.cn/Article/details/gtnbshypv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.bbcook.cn/Article/details/gwfnhjrjh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gfgpawijb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.epnwcf.com/Article/details/gbyngihgj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.epnwcf.com/Article/details/gvarildhr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.vehdjk.com/Article/details/grmiqduvw.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.sjlbkw.cn/Article/details/ggzpztbdi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.bbcook.cn/Article/details/gefyheaho.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.vehdjk.com/Article/details/gksaqxeuv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.bbcook.cn/Article/details/ghuouytnj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/ghqevucwh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.epnwcf.com/Article/details/gvycxhrei.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gqklxtmld.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtugcwyhz.sHtML

Go:   func add(a, b int) int
来源：http://wap.epnwcf.com/Article/details/glwlmzkpu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.bbcook.cn/Article/details/gnxwbvazg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.sjlbkw.cn/Article/details/gsuqekakx.sHtML

[C14] 泛型函数
来源：http://www.blog.fktsv.cn/Article/details/giktuktin.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.sjlbkw.cn/Article/details/gmzctqtdv.sHtML

PHP:  // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gekycnhur.sHtML

JS:   // 无泛型
来源：http://mobile.yfazqb.com/Article/details/gepytgsca.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.bbcook.cn/Article/details/gjtzqebcv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.yfazqb.com/Article/details/gvdbihecn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.vehdjk.com/Article/details/grxnvujkc.sHtML

Ruby: # 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gmouqfrzh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.tarul.cn/Article/details/gdzteuraz.sHtML

[C15] 解构 / 展开参数
来源：http://blog.epnwcf.com/Article/details/ghsuqvvat.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.vehdjk.com/Article/details/gjcjqofss.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fktsv.cn/Article/details/gbunwyrtx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/gfpjvyzoi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.epnwcf.com/Article/details/gdpunvuhw.sHtML

Java: // 无解构
来源：http://mobile.tarul.cn/Article/details/ghnyplvwu.sHtML

Go:   // 无解构
来源：http://www.share.fktsv.cn/Article/details/grjcobxry.sHtML

Ruby: a, b = pair
来源：http://mobile.vehdjk.com/Article/details/gzmnjriwl.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.epnwcf.com/Article/details/gdzbtlgvm.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.vehdjk.com/Article/details/gwujtiedz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.tarul.cn/Article/details/guqdymrcj.sHtML

PHP:  // 无重载
来源：http://3g.epnwcf.com/Article/details/gectnqwdi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.vehdjk.com/Article/details/gvfwgavqs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.sjlbkw.cn/Article/details/gcylgjibg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fktsv.cn/Article/details/gcvdszpeq.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.epnwcf.com/Article/details/gtfzuvnss.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fktsv.cn/Article/details/gtmeaympj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.sjlbkw.cn/Article/details/gyhigntiz.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gqzhoeqjv.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.bbcook.cn/Article/details/gwmlxbtns.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/glpokoxjo.sHtML

[D01] 创建数组 / 列表
来源：http://baike.yfazqb.com/Article/details/guhqrdbyi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.epnwcf.com/Article/details/glxxgqpfs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.vehdjk.com/Article/details/gwbbiyssb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.tarul.cn/Article/details/gjiiouckr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.tarul.cn/Article/details/ghbtzgtlo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.epnwcf.com/Article/details/gtwwpzqma.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.epnwcf.com/Article/details/geszejsgc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fktsv.cn/Article/details/gvqzchqpm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.tarul.cn/Article/details/glqbfaizj.sHtML

[D02] 追加元素到末尾
来源：http://baike.fktsv.cn/Article/details/gyfbqxgqq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fktsv.cn/Article/details/gykrxmzaq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fktsv.cn/Article/details/gvrisuwqh.sHtML

JS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gkjovagjy.sHtML

TS:   arr.push(4);
来源：http://baike.vehdjk.com/Article/details/gmwovtpzo.sHtML

Java: list.add(4);
来源：http://3g.yfazqb.com/Article/details/gvygaueuo.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.bbcook.cn/Article/details/gergahkdf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.vehdjk.com/Article/details/ghwtekhwg.sHtML

C#:   list.Add(4);
来源：http://baike.fktsv.cn/Article/details/glevkmnlt.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.epnwcf.com/Article/details/gbiyofvfq.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.tarul.cn/Article/details/gyucrbugf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.bbcook.cn/Article/details/gzsszpwzb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fktsv.cn/Article/details/gkcbwnipq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.vehdjk.com/Article/details/gmuuilbsq.sHtML

Java: list.add(0, 0);
来源：http://www.share.fktsv.cn/Article/details/gmblmdbre.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.sjlbkw.cn/Article/details/gexlmotuu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fktsv.cn/Article/details/gncoeyizp.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.tarul.cn/Article/details/ggbydxnex.sHtML

[D04] 删除元素
来源：http://www.m.share.bbcook.cn/Article/details/gfskmlogx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.vehdjk.com/Article/details/glorgqopx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.tarul.cn/Article/details/ghjqfgnpu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.tarul.cn/Article/details/gzmukggri.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.vehdjk.com/Article/details/gsalvhvxa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fktsv.cn/Article/details/grtbsalxg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.vehdjk.com/Article/details/grsdnohix.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.vehdjk.com/Article/details/gaxxtexkv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.bbcook.cn/Article/details/gxujmbmbj.sHtML

[D05] 访问与修改元素
来源：http://m.share.sjlbkw.cn/Article/details/glorzuyff.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gbfsmihve.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gqemhgynb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gbglevsaw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/gkglagdea.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.tarul.cn/Article/details/gplhtkwcm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gbrwesnpv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gzbwihmpl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gjxlbdala.sHtML

[D06] 数组长度
来源：http://baike.fktsv.cn/Article/details/geafuyyei.sHtML

Py:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/grlngenbt.sHtML

PHP:  count($arr);
来源：http://read.share.tarul.cn/Article/details/gmvkkzwjz.sHtML

JS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/gpyebqalj.sHtML

TS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/gopijazfs.sHtML

Java: list.size();
来源：http://3g.yfazqb.com/Article/details/gaglhrsqx.sHtML

Go:   len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gimvdtiek.sHtML

Ruby: arr.length; arr.size
来源：http://wap.tarul.cn/Article/details/gnqzhflcx.sHtML

C#:   list.Count;
来源：http://www.blog.bbcook.cn/Article/details/gqfnbzzue.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.sjlbkw.cn/Article/details/gafmnpgzm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.yfazqb.com/Article/details/gbrfgguis.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.vehdjk.com/Article/details/gfowvdmwn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gwaahoxjm.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fktsv.cn/Article/details/gktmcfwsu.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gypcgqdgz.sHtML

Go:   arr[1:4]
来源：http://read.share.bbcook.cn/Article/details/gckuhirhn.sHtML

Ruby: arr[1, 3]
来源：http://www.share.sjlbkw.cn/Article/details/ggcslamob.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.bbcook.cn/Article/details/gujoozqrb.sHtML

[D08] 合并两个数组
来源：http://www.m.share.vehdjk.com/Article/details/gvdhjiqad.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.vehdjk.com/Article/details/gwyuzowoh.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.yfazqb.com/Article/details/glnahnarg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.epnwcf.com/Article/details/gwwjqvlav.sHtML

TS:   [...a, ...b];
来源：http://read.share.fktsv.cn/Article/details/gmbrllizl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.vehdjk.com/Article/details/gajbguobq.sHtML

Go:   append(a, b...)
来源：http://mobile.epnwcf.com/Article/details/ggynxcwlq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.vehdjk.com/Article/details/gllptocks.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.yfazqb.com/Article/details/gracasygg.sHtML

[D09] 排序（升序）
来源：http://baike.epnwcf.com/Article/details/ghimjxmvy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/gohrfatie.sHtML

PHP:  sort($arr);
来源：http://mobile.fktsv.cn/Article/details/gxmsfuesi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fktsv.cn/Article/details/gzdpfdape.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.yfazqb.com/Article/details/gplsgwtai.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.vehdjk.com/Article/details/gtfqggxrc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/grirrrgpc.sHtML

Ruby: arr.sort
来源：http://read.share.vehdjk.com/Article/details/gpujrltdz.sHtML

C#:   list.Sort();
来源：http://mobile.fktsv.cn/Article/details/gnjsxaguf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.tarul.cn/Article/details/geydovasb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.bbcook.cn/Article/details/gzcdnxgje.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.tarul.cn/Article/details/gxtoiyobd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.epnwcf.com/Article/details/goiiukvnb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.sjlbkw.cn/Article/details/gqlivclmv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.bbcook.cn/Article/details/gnbyxmqio.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.vehdjk.com/Article/details/gzrqsudqk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fktsv.cn/Article/details/gwgkhjxaf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.yfazqb.com/Article/details/gzdkdzqtq.sHtML

[D11] 反转数组
来源：http://read.share.sjlbkw.cn/Article/details/gbsdnfpai.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.bbcook.cn/Article/details/gwrtzlwuj.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.tarul.cn/Article/details/gzghojqxm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.yfazqb.com/Article/details/gcolszkkj.sHtML

TS:   [...arr].reverse();
来源：http://blog.yfazqb.com/Article/details/gbjplsjmx.sHtML

Java: Collections.reverse(list);
来源：http://3g.epnwcf.com/Article/details/gfechqftm.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.sjlbkw.cn/Article/details/ghtejodig.sHtML

Ruby: arr.reverse
来源：http://wap.bbcook.cn/Article/details/glyfuitdl.sHtML

C#:   list.Reverse();
来源：http://www.m.share.vehdjk.com/Article/details/gtlsczgug.sHtML

[D12] 查找元素下标
来源：http://read.share.yfazqb.com/Article/details/gspglawxa.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.yfazqb.com/Article/details/gprxrvsci.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/ghysexsbj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/gaujsguyr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/gymjspvco.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.sjlbkw.cn/Article/details/gqheclqlq.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gjuocfhfy.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.bbcook.cn/Article/details/gdxcayfqm.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fktsv.cn/Article/details/gmqcntmcx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.epnwcf.com/Article/details/gocppxntb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.yfazqb.com/Article/details/gsbgragif.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.tarul.cn/Article/details/govcmdujd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.bbcook.cn/Article/details/gsgqynggi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gjtqofhnh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gcgpfwjmo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/gbaxokuqr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.yfazqb.com/Article/details/grbdqokbj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fktsv.cn/Article/details/gadqfrmuf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.epnwcf.com/Article/details/gytsvuaqs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.bbcook.cn/Article/details/gnyytrgng.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fktsv.cn/Article/details/gnqdltgod.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/gzkornnfj.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.sjlbkw.cn/Article/details/gvtkcawbx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gyzqahmmf.sHtML

Go:   // 手写循环
来源：http://www.m.share.vehdjk.com/Article/details/gykxljfzv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.bbcook.cn/Article/details/gofcqdnqv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.epnwcf.com/Article/details/gqbmjxldr.sHtML

[D15] 去重
来源：http://baike.sjlbkw.cn/Article/details/gjyyiniir.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.tarul.cn/Article/details/gvkdzkjdj.sHtML

PHP:  array_unique($arr);
来源：http://blog.epnwcf.com/Article/details/ghndpwemy.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gfdrqagbl.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gwqovdlmh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.tarul.cn/Article/details/gseeogkkm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.sjlbkw.cn/Article/details/gsxrhghgz.sHtML

Ruby: arr.uniq
来源：http://www.m.share.tarul.cn/Article/details/gjwshnlkx.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.epnwcf.com/Article/details/gkgjwdacg.sHtML

[D16] 求和与平均值
来源：http://blog.yfazqb.com/Article/details/gptnxekur.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.sjlbkw.cn/Article/details/guwfnfmyg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.bbcook.cn/Article/details/glrfkgryi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/giknwrjdt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/gtfajnjmt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.epnwcf.com/Article/details/gpewstozj.sHtML

Go:   // 手写循环累加
来源：http://baike.bbcook.cn/Article/details/giarxvvst.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.epnwcf.com/Article/details/gmlzuziog.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.yfazqb.com/Article/details/gikcewtse.sHtML

[D17] 最大值与最小值
来源：http://3g.tarul.cn/Article/details/grzkxueqr.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fktsv.cn/Article/details/ghupjlsoi.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.vehdjk.com/Article/details/glikdhwlw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.vehdjk.com/Article/details/geglsiezm.sHtML

TS:   Math.max(...arr);
来源：http://www.share.sjlbkw.cn/Article/details/ggrpkgsvc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.tarul.cn/Article/details/gvokxsxzc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.tarul.cn/Article/details/gyvxioyix.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.vehdjk.com/Article/details/gxupspkyo.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/gwryutcss.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.bbcook.cn/Article/details/gsjtwxprs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.tarul.cn/Article/details/glqpgqbli.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fktsv.cn/Article/details/gdggoltrc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.bbcook.cn/Article/details/gaqkoidue.sHtML

TS:   nested.flat();
来源：http://3g.sjlbkw.cn/Article/details/gzehibudu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gprlsainh.sHtML

Go:   // 手写双层循环
来源：http://wap.bbcook.cn/Article/details/gvrcbopry.sHtML

Ruby: nested.flatten
来源：http://read.share.vehdjk.com/Article/details/gomvaewvq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.bbcook.cn/Article/details/gnepysbfy.sHtML

[D19] 按字段分组
来源：http://3g.fktsv.cn/Article/details/gtechcico.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.bbcook.cn/Article/details/ghdzfoluj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.epnwcf.com/Article/details/geizyyove.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.epnwcf.com/Article/details/gcmcflmpq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gznzzgaha.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fktsv.cn/Article/details/gnlmcchza.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.vehdjk.com/Article/details/ggfgekdnm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.sjlbkw.cn/Article/details/gswvztlmb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.bbcook.cn/Article/details/gojhdjowa.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.vehdjk.com/Article/details/gkifxordx.sHtML

Py:   Counter(arr)
来源：http://mobile.fktsv.cn/Article/details/gaespxphv.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.yfazqb.com/Article/details/gcvpyixwz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.epnwcf.com/Article/details/gflfywgla.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gtmpmudil.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.sjlbkw.cn/Article/details/gaauvptms.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.vehdjk.com/Article/details/gxvoenhyd.sHtML

Ruby: arr.tally
来源：http://m.share.epnwcf.com/Article/details/gyquosijr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.sjlbkw.cn/Article/details/gwizwywsd.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.sjlbkw.cn/Article/details/gorsvhowb.sHtML

Py:   x in arr
来源：http://m.share.fktsv.cn/Article/details/gagfzfdyd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.bbcook.cn/Article/details/gmkcbtwqz.sHtML

JS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gvyigsxds.sHtML

TS:   arr.includes(x)
来源：http://read.share.yfazqb.com/Article/details/gtkfcdrxk.sHtML

Java: list.contains(x)
来源：http://mobile.epnwcf.com/Article/details/gzyyilsxs.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gqttykwtz.sHtML

Ruby: arr.include?(x)
来源：http://3g.fktsv.cn/Article/details/gmpgoensd.sHtML

C#:   list.Contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gdnikcavk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.yfazqb.com/Article/details/gfyjoswsq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.tarul.cn/Article/details/ggrbrbgwt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.yfazqb.com/Article/details/ghpvnnogz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.tarul.cn/Article/details/grnukhqhm.sHtML

TS:   [...arr];
来源：http://blog.yfazqb.com/Article/details/gfhaooodz.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.vehdjk.com/Article/details/gzdeyhqjn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.epnwcf.com/Article/details/gcfvojwaf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.tarul.cn/Article/details/gjkunofyj.sHtML

C#:   new List<int>(list);
来源：http://mobile.bbcook.cn/Article/details/gbyllcriq.sHtML

[D23] reduce 累积计算
来源：http://blog.bbcook.cn/Article/details/grhgxjnva.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.bbcook.cn/Article/details/guusisxfp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.epnwcf.com/Article/details/gmustvkmy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/gobhbcpxs.sHtML


<!-- 参考信息 -->