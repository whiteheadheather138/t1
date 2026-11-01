代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://read.share.bbcook.cn/Article/details/gnakvifrc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.yfazqb.com/Article/details/gbjxbqrgp.sHtML

[C08] 闭包
来源：http://www.share.epnwcf.com/Article/details/gmmlmaadj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.yfazqb.com/Article/details/gfeahmaze.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.tarul.cn/Article/details/gcojpgxjg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/gnlxurrrb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/ghagxwedx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.sjlbkw.cn/Article/details/gzwyoesom.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.tarul.cn/Article/details/gqqjgfpyt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.bbcook.cn/Article/details/girbfrkfo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/ghrcodxtd.sHtML

[C09] 递归
来源：http://www.m.share.epnwcf.com/Article/details/gerxeuepd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/gpztkkvth.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.sjlbkw.cn/Article/details/gnvyryyes.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.vehdjk.com/Article/details/gkjkhltmu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.sjlbkw.cn/Article/details/gdpilqsok.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.tarul.cn/Article/details/gtfkvidcp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.bbcook.cn/Article/details/gmznalgmy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.yfazqb.com/Article/details/gnapjnays.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.epnwcf.com/Article/details/gtqwiqevu.sHtML

[C10] 变量作用域
来源：http://blog.sjlbkw.cn/Article/details/gbbaxnhto.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.vehdjk.com/Article/details/gugyegmwn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.epnwcf.com/Article/details/ghtejobnp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gufgijuag.sHtML

TS:   同 JS
来源：http://baike.fktsv.cn/Article/details/gendvcjoz.sHtML

Java: 方法内为块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/grulemqsi.sHtML

Go:   花括号块级作用域
来源：http://blog.tarul.cn/Article/details/gpchzhpka.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fktsv.cn/Article/details/gnhuajhwj.sHtML

C#:   块级作用域
来源：http://m.share.vehdjk.com/Article/details/gunckeldb.sHtML

[C11] 模块导入与导出
来源：http://3g.bbcook.cn/Article/details/gtuprceyx.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/gtyrwdxoc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.yfazqb.com/Article/details/gjfhqspnr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.epnwcf.com/Article/details/gmbqecncw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.epnwcf.com/Article/details/gyvrepgmd.sHtML

Java: import java.util.List;
来源：http://www.blog.epnwcf.com/Article/details/gprasicjg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.sjlbkw.cn/Article/details/gdoihxcjy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fktsv.cn/Article/details/gwiehdnry.sHtML

C#:   using System.Text;
来源：http://m.share.tarul.cn/Article/details/guyqhiaoe.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.bbcook.cn/Article/details/ggmlhmvej.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fktsv.cn/Article/details/gqyqbyyrf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.epnwcf.com/Article/details/giicvlebf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gmyersihh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/gliyivbfx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.sjlbkw.cn/Article/details/gtotfsbzo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.epnwcf.com/Article/details/gexuaouke.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.sjlbkw.cn/Article/details/gmyzcoudg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/gahclfjax.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.vehdjk.com/Article/details/gfztdvcem.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.bbcook.cn/Article/details/gehhrxkvn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/giibvcnpr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.bbcook.cn/Article/details/gxgmroefr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gvlktfutb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/grjemjrrq.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fktsv.cn/Article/details/ggznwnktj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.bbcook.cn/Article/details/grzhnvqfl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.tarul.cn/Article/details/gypslkudn.sHtML

[C14] 泛型函数
来源：http://wap.bbcook.cn/Article/details/gawncpuge.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.epnwcf.com/Article/details/gjxismfdo.sHtML

PHP:  // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/grrpykfjp.sHtML

JS:   // 无泛型
来源：http://m.share.vehdjk.com/Article/details/gsobcpgro.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.yfazqb.com/Article/details/gxzxikolw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.epnwcf.com/Article/details/gflsdkuzb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.yfazqb.com/Article/details/gzadzbhgm.sHtML

Ruby: # 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/giyfultpw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fktsv.cn/Article/details/goarubhvp.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.epnwcf.com/Article/details/gqpvpeiqp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.tarul.cn/Article/details/gxajyaiyg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.yfazqb.com/Article/details/gpnypdfqm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/gyxmpllqm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.bbcook.cn/Article/details/gkmblqdoe.sHtML

Java: // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/ghwisursw.sHtML

Go:   // 无解构
来源：http://blog.fktsv.cn/Article/details/gsjfirezb.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/ghrckqsak.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.epnwcf.com/Article/details/gdevudtqn.sHtML

[C16] 函数 / 方法重载
来源：http://baike.epnwcf.com/Article/details/gjhbcvdvy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.sjlbkw.cn/Article/details/gbcqnjsht.sHtML

PHP:  // 无重载
来源：http://read.share.bbcook.cn/Article/details/gehakfbin.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.bbcook.cn/Article/details/guujkuwdc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.sjlbkw.cn/Article/details/gswoicnsb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.sjlbkw.cn/Article/details/gpbwxkgbj.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.epnwcf.com/Article/details/gkarhjjuw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.bbcook.cn/Article/details/gafwfqdrj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.epnwcf.com/Article/details/gairrfqyy.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gyvtqbbyz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.bbcook.cn/Article/details/gvjbofszo.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gswzvqpsx.sHtML

[D01] 创建数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gbjbbcbfg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.sjlbkw.cn/Article/details/giexhisom.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fktsv.cn/Article/details/gpfrsrbkd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.vehdjk.com/Article/details/gnxylejqu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fktsv.cn/Article/details/gisphkszr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.tarul.cn/Article/details/gqhvtfzaa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.vehdjk.com/Article/details/gjknsnnxs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.epnwcf.com/Article/details/gkamfqfkz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzpqfuus.sHtML

[D02] 追加元素到末尾
来源：http://m.share.bbcook.cn/Article/details/gajqpoeky.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.epnwcf.com/Article/details/gltgfplnq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.vehdjk.com/Article/details/gsebjqvgi.sHtML

JS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gtsawazgh.sHtML

TS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/guxpavoxb.sHtML

Java: list.add(4);
来源：http://m.share.tarul.cn/Article/details/gnpwsryad.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.sjlbkw.cn/Article/details/gtqopfqmj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fktsv.cn/Article/details/gbmmznknm.sHtML

C#:   list.Add(4);
来源：http://3g.bbcook.cn/Article/details/goledvdgj.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fktsv.cn/Article/details/gkfopwhkc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.epnwcf.com/Article/details/gmaypwjyn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxothagyx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.vehdjk.com/Article/details/gabpodqwc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gdpeadxte.sHtML

Java: list.add(0, 0);
来源：http://wap.bbcook.cn/Article/details/gtvmzmshs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gvzjnmela.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.yfazqb.com/Article/details/grnkerpyi.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.epnwcf.com/Article/details/gjoornurb.sHtML

[D04] 删除元素
来源：http://www.blog.vehdjk.com/Article/details/gxhnpccgf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.bbcook.cn/Article/details/godhongsi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gxpassmyf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.sjlbkw.cn/Article/details/gbjaiftqu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.tarul.cn/Article/details/gagywskii.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fktsv.cn/Article/details/grutixevo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.epnwcf.com/Article/details/gwfixxkaz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.yfazqb.com/Article/details/gzvjrwfsz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gglaqxpdd.sHtML

[D05] 访问与修改元素
来源：http://read.share.epnwcf.com/Article/details/gonaraovu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gelgjxpbs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gjxvwbukl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/glmolktxq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.bbcook.cn/Article/details/glzlzdukw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.bbcook.cn/Article/details/ghkbnjfph.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gmhdehgby.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/gtwshntkl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gzsmsqaxn.sHtML

[D06] 数组长度
来源：http://read.share.tarul.cn/Article/details/gpssrgvtx.sHtML

Py:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/gyanixdgp.sHtML

PHP:  count($arr);
来源：http://blog.vehdjk.com/Article/details/gtcxevfwy.sHtML

JS:   arr.length
来源：http://mobile.tarul.cn/Article/details/gmrpzcqdm.sHtML

TS:   arr.length
来源：http://blog.bbcook.cn/Article/details/gxpfotszj.sHtML

Java: list.size();
来源：http://blog.bbcook.cn/Article/details/gxjdyvhxp.sHtML

Go:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gityjqayj.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fktsv.cn/Article/details/gwfrpykzp.sHtML

C#:   list.Count;
来源：http://3g.tarul.cn/Article/details/gndyvdftt.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.sjlbkw.cn/Article/details/gbkhgngoz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.yfazqb.com/Article/details/gckcxtejh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fktsv.cn/Article/details/gawkktlvt.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gcbfwdgru.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.epnwcf.com/Article/details/gbpxlwbgi.sHtML

Java: list.subList(1, 4);
来源：http://read.share.tarul.cn/Article/details/gsxhlgzik.sHtML

Go:   arr[1:4]
来源：http://3g.yfazqb.com/Article/details/gcdbplpxl.sHtML

Ruby: arr[1, 3]
来源：http://mobile.bbcook.cn/Article/details/gjjichbnr.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.bbcook.cn/Article/details/guwuawdmt.sHtML

[D08] 合并两个数组
来源：http://3g.sjlbkw.cn/Article/details/gjssqgucu.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.sjlbkw.cn/Article/details/gnbqqasin.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.bbcook.cn/Article/details/ggkbekitk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.sjlbkw.cn/Article/details/gfxehapqy.sHtML

TS:   [...a, ...b];
来源：http://mobile.vehdjk.com/Article/details/ggdrlfyvc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.tarul.cn/Article/details/gspuwplcy.sHtML

Go:   append(a, b...)
来源：http://read.share.vehdjk.com/Article/details/gtddlkpxj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.yfazqb.com/Article/details/gxqdgjoyq.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.vehdjk.com/Article/details/gqvijyldj.sHtML

[D09] 排序（升序）
来源：http://www.share.epnwcf.com/Article/details/gqnunpdyo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/gyctmiyon.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gihxwghzq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.epnwcf.com/Article/details/ghlaxnvbp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.yfazqb.com/Article/details/gfwoordyp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.epnwcf.com/Article/details/gyxrvssel.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/gruhitagm.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/gzfsthhyz.sHtML

C#:   list.Sort();
来源：http://www.blog.yfazqb.com/Article/details/gaovcauwg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.tarul.cn/Article/details/gbzzycrkw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fktsv.cn/Article/details/gglfozieg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/grcdnulaq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.epnwcf.com/Article/details/gzqasyxue.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/ghltgsrji.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.vehdjk.com/Article/details/gzpieqctd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.vehdjk.com/Article/details/gqwqpfymh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.sjlbkw.cn/Article/details/gyiwmdlal.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.sjlbkw.cn/Article/details/gdnsplyhd.sHtML

[D11] 反转数组
来源：http://baike.bbcook.cn/Article/details/gyhfkuzoc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.epnwcf.com/Article/details/gibmdgmwo.sHtML

PHP:  array_reverse($arr);
来源：http://wap.epnwcf.com/Article/details/gelwkbrjx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.bbcook.cn/Article/details/gkclvtsxs.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/gtvvcovrt.sHtML

Java: Collections.reverse(list);
来源：http://baike.epnwcf.com/Article/details/gqgjetwew.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.bbcook.cn/Article/details/gscwgsegt.sHtML

Ruby: arr.reverse
来源：http://blog.sjlbkw.cn/Article/details/gexmxeolq.sHtML

C#:   list.Reverse();
来源：http://baike.epnwcf.com/Article/details/gpldvsssm.sHtML

[D12] 查找元素下标
来源：http://www.m.share.sjlbkw.cn/Article/details/gduukuhwp.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.epnwcf.com/Article/details/gyesydddb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fktsv.cn/Article/details/gqxawsqjz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gtrnjsxzr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gjjgpfopw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fktsv.cn/Article/details/gkrwdchuz.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fktsv.cn/Article/details/gbdrakusv.sHtML

Ruby: arr.index(x)
来源：http://read.share.sjlbkw.cn/Article/details/gkaenxbhn.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.vehdjk.com/Article/details/gosxvxsyg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fktsv.cn/Article/details/gitdomykb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.tarul.cn/Article/details/gifvhtrvq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.tarul.cn/Article/details/gyalcbwgj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/getddvnze.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gvymbsdtd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gosfsqmrq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.epnwcf.com/Article/details/gqkjpmjlo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.bbcook.cn/Article/details/gkgdrqkqh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.epnwcf.com/Article/details/gewlaoxmb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.vehdjk.com/Article/details/gkfvekytz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.tarul.cn/Article/details/gioziwpqh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.epnwcf.com/Article/details/giwftwywn.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.vehdjk.com/Article/details/griekcwdx.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.bbcook.cn/Article/details/gfmahmzyj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fktsv.cn/Article/details/gshlwpolu.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/glpbztrei.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.tarul.cn/Article/details/gzfevxuim.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gbuueqpia.sHtML

[D15] 去重
来源：http://blog.epnwcf.com/Article/details/gtxfrkrep.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fktsv.cn/Article/details/grkivjoez.sHtML

PHP:  array_unique($arr);
来源：http://read.share.tarul.cn/Article/details/gtrfjucpp.sHtML

JS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gbozumxvm.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/gzwqcfknd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.tarul.cn/Article/details/geeuhtxuz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.tarul.cn/Article/details/gqmbogird.sHtML

Ruby: arr.uniq
来源：http://www.share.bbcook.cn/Article/details/gmudjdwpo.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.bbcook.cn/Article/details/gmhvwoixp.sHtML

[D16] 求和与平均值
来源：http://read.share.tarul.cn/Article/details/gdcpqnwhu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.epnwcf.com/Article/details/gbidmzsmd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.yfazqb.com/Article/details/goeroosar.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.tarul.cn/Article/details/ghmdfckie.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gqpnstfvd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.vehdjk.com/Article/details/gzlkzfqpp.sHtML

Go:   // 手写循环累加
来源：http://m.share.tarul.cn/Article/details/gnbkusbvx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.yfazqb.com/Article/details/glqyljzzk.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.sjlbkw.cn/Article/details/goanvggcz.sHtML

[D17] 最大值与最小值
来源：http://read.share.bbcook.cn/Article/details/grjibmpxm.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.tarul.cn/Article/details/grndelkfp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gmzfzptza.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gtcipbxpl.sHtML

TS:   Math.max(...arr);
来源：http://wap.yfazqb.com/Article/details/gygyvtkub.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.yfazqb.com/Article/details/gyqettrhd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.yfazqb.com/Article/details/glagfvizp.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.epnwcf.com/Article/details/gfnamzjgz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.epnwcf.com/Article/details/goxdmxrkr.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.epnwcf.com/Article/details/gmkryplgy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.bbcook.cn/Article/details/gqrnlkcsi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.yfazqb.com/Article/details/gubxjvzvm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.bbcook.cn/Article/details/gcmygxdox.sHtML

TS:   nested.flat();
来源：http://mobile.yfazqb.com/Article/details/gpchhwbkb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.epnwcf.com/Article/details/gnnhgzcju.sHtML

Go:   // 手写双层循环
来源：http://mobile.vehdjk.com/Article/details/gamaqkwqs.sHtML

Ruby: nested.flatten
来源：http://baike.fktsv.cn/Article/details/gposjamwf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fktsv.cn/Article/details/gkumrvvph.sHtML

[D19] 按字段分组
来源：http://mobile.yfazqb.com/Article/details/gzqpdvujt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.epnwcf.com/Article/details/gtiurpjup.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.vehdjk.com/Article/details/gtkurekol.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.epnwcf.com/Article/details/gwpxauwrj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.bbcook.cn/Article/details/gyeogdqnc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.tarul.cn/Article/details/gnalsiejo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fktsv.cn/Article/details/gpyiakzos.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.sjlbkw.cn/Article/details/gqmoufdnb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.yfazqb.com/Article/details/gdjsrvatc.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fktsv.cn/Article/details/gldaoqibs.sHtML

Py:   Counter(arr)
来源：http://www.share.tarul.cn/Article/details/gjftdykqk.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fktsv.cn/Article/details/gcizdfzjn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.vehdjk.com/Article/details/gjconozgw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/gyvktfpki.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.yfazqb.com/Article/details/gfrvjpqlx.sHtML

Go:   // 手写 map[T]int
来源：http://wap.sjlbkw.cn/Article/details/gsptgxrsx.sHtML

Ruby: arr.tally
来源：http://www.share.fktsv.cn/Article/details/gbdccmkhk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.tarul.cn/Article/details/gvvficfhs.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.bbcook.cn/Article/details/gbfdtfjkg.sHtML

Py:   x in arr
来源：http://mobile.fktsv.cn/Article/details/gopfljrnq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.sjlbkw.cn/Article/details/guvfdwonb.sHtML

JS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/gjnkvwtgq.sHtML

TS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/gsdktkjsd.sHtML

Java: list.contains(x)
来源：http://baike.fktsv.cn/Article/details/gkztgbucp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gzavybnqz.sHtML

Ruby: arr.include?(x)
来源：http://m.share.yfazqb.com/Article/details/gkussfdza.sHtML

C#:   list.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gsicfdwxd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.epnwcf.com/Article/details/gkcptglvc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fktsv.cn/Article/details/gdtmirwsm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.sjlbkw.cn/Article/details/ghgbekpou.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.tarul.cn/Article/details/gdolhpeur.sHtML

TS:   [...arr];
来源：http://www.m.share.vehdjk.com/Article/details/gbipmjrvi.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/ggxwyrvqg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fktsv.cn/Article/details/gniwlhvgo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.bbcook.cn/Article/details/gdngylkqv.sHtML

C#:   new List<int>(list);
来源：http://read.share.epnwcf.com/Article/details/gyoslpmfs.sHtML

[D23] reduce 累积计算
来源：http://m.share.yfazqb.com/Article/details/gmdfydhtk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gutbsinds.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.tarul.cn/Article/details/gqrlshemd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gdzvxkrby.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/gzphibkfa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fktsv.cn/Article/details/gnirrnitz.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/gnahfmyxt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.tarul.cn/Article/details/gqyhjybtn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.yfazqb.com/Article/details/goxgayfti.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.vehdjk.com/Article/details/gwvgpnpbf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fktsv.cn/Article/details/grwqtfyrl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.sjlbkw.cn/Article/details/gchsmmaon.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.vehdjk.com/Article/details/gjvssisce.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gqokuzjtj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.yfazqb.com/Article/details/gmmifbsog.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsekofsy.sHtML


<!-- 参考信息 -->