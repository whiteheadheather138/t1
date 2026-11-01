代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://m.share.vehdjk.com/Article/details/glucryjqo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gegfrbqmn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fktsv.cn/Article/details/gcmfvnhyh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.vehdjk.com/Article/details/glmgvlule.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/grlsedsxo.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.bbcook.cn/Article/details/gixennotx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.sjlbkw.cn/Article/details/gaixgyjpx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fktsv.cn/Article/details/gbqpvgyew.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.tarul.cn/Article/details/gupcbvysk.sHtML

TS:   arr.map(String)
来源：http://read.share.tarul.cn/Article/details/gvhfrbtih.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.vehdjk.com/Article/details/gexajmjyr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.bbcook.cn/Article/details/gadkymonf.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fktsv.cn/Article/details/gzzgaikzg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.vehdjk.com/Article/details/gqtyscjuq.sHtML

[C08] 闭包
来源：http://www.share.epnwcf.com/Article/details/gszqmzahs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fktsv.cn/Article/details/gwurvrjnc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.epnwcf.com/Article/details/gpnmixujb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gsgdmouzn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gibyzjjqn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.yfazqb.com/Article/details/gyijhjhbt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.tarul.cn/Article/details/gzkgjtbrn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fktsv.cn/Article/details/gvhhurmzb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gsmpdixtq.sHtML

[C09] 递归
来源：http://m.share.vehdjk.com/Article/details/gbihnjpwg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.bbcook.cn/Article/details/gokuxxfgn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.yfazqb.com/Article/details/gicfhrvkw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gxxlpfjkc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gudqlsdrx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.vehdjk.com/Article/details/glnsqaigw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.yfazqb.com/Article/details/gdyajsuuv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gxtbozapu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.tarul.cn/Article/details/gjsnxpxjm.sHtML

[C10] 变量作用域
来源：http://www.share.sjlbkw.cn/Article/details/gpzoybayt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.vehdjk.com/Article/details/gwqtibhrr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.vehdjk.com/Article/details/gdufnowdi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.bbcook.cn/Article/details/gnqfrpcvg.sHtML

TS:   同 JS
来源：http://www.share.yfazqb.com/Article/details/glphpwkfr.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gfntduluz.sHtML

Go:   花括号块级作用域
来源：http://blog.fktsv.cn/Article/details/gwdyvtnxv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.tarul.cn/Article/details/gpquxqulx.sHtML

C#:   块级作用域
来源：http://3g.yfazqb.com/Article/details/gvneehawu.sHtML

[C11] 模块导入与导出
来源：http://www.share.tarul.cn/Article/details/gsendcprc.sHtML

Py:   from module import func
来源：http://www.share.bbcook.cn/Article/details/gpuxkemcj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.epnwcf.com/Article/details/gonerwvyn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.tarul.cn/Article/details/gwbnsjnlg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.bbcook.cn/Article/details/gqlpzizhq.sHtML

Java: import java.util.List;
来源：http://wap.sjlbkw.cn/Article/details/gmxhwjoih.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.bbcook.cn/Article/details/glbbbyicd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fktsv.cn/Article/details/gyrulujol.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/glogwoxpo.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.yfazqb.com/Article/details/gepbyvtfs.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.tarul.cn/Article/details/gaizlieeq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gntksgofx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/gltripdnl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gyyzfnylo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.bbcook.cn/Article/details/gxacazufd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.tarul.cn/Article/details/ganewpwzr.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.epnwcf.com/Article/details/glbhdiuex.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.yfazqb.com/Article/details/ghhaapyaq.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.bbcook.cn/Article/details/gflkdtjak.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.tarul.cn/Article/details/glcpjdfhu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gwffsncwc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.epnwcf.com/Article/details/garutprws.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gylanrwfy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/ghuwvwalp.sHtML

Go:   func add(a, b int) int
来源：http://mobile.vehdjk.com/Article/details/giialelxk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.tarul.cn/Article/details/gbgiaurkh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.tarul.cn/Article/details/gizkbfbrv.sHtML

[C14] 泛型函数
来源：http://baike.vehdjk.com/Article/details/gyadqjkde.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fktsv.cn/Article/details/gyvtnlbgn.sHtML

PHP:  // 无泛型
来源：http://www.share.epnwcf.com/Article/details/gjvpsvtci.sHtML

JS:   // 无泛型
来源：http://mobile.epnwcf.com/Article/details/gbiqlealx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fktsv.cn/Article/details/gwbmbxkoa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.bbcook.cn/Article/details/gsgnvyfzd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.epnwcf.com/Article/details/gsdzgypwz.sHtML

Ruby: # 无泛型
来源：http://www.share.fktsv.cn/Article/details/gtctsihqv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.bbcook.cn/Article/details/gkjndxylk.sHtML

[C15] 解构 / 展开参数
来源：http://baike.tarul.cn/Article/details/gaxsjleum.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fktsv.cn/Article/details/gwmzvsblp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.bbcook.cn/Article/details/gwvclvqmk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fktsv.cn/Article/details/gzqndulix.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.sjlbkw.cn/Article/details/gflajfpll.sHtML

Java: // 无解构
来源：http://mobile.yfazqb.com/Article/details/gejnmqygc.sHtML

Go:   // 无解构
来源：http://blog.bbcook.cn/Article/details/gljlijpdt.sHtML

Ruby: a, b = pair
来源：http://www.blog.tarul.cn/Article/details/gvghujoro.sHtML

C#:   var (a, b) = pair;
来源：http://baike.epnwcf.com/Article/details/gmrozvtfk.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.sjlbkw.cn/Article/details/ghqxmhqsj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.sjlbkw.cn/Article/details/gplykkmvw.sHtML

PHP:  // 无重载
来源：http://m.share.bbcook.cn/Article/details/ggrdfwpgx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.yfazqb.com/Article/details/greovfdgi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.yfazqb.com/Article/details/ggnxaqznp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.tarul.cn/Article/details/gvytxuzwh.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.vehdjk.com/Article/details/ggxzqebaz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.bbcook.cn/Article/details/gxxjdwpkq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gwfcwvjez.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gaoqdryud.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.bbcook.cn/Article/details/gwxtloagh.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gggnmroan.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.tarul.cn/Article/details/gvfhfocnr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.vehdjk.com/Article/details/geqyqhmlv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.sjlbkw.cn/Article/details/grytectdr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.bbcook.cn/Article/details/gokbppvvf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fktsv.cn/Article/details/gpumjxfrc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.vehdjk.com/Article/details/gjnxhromx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fktsv.cn/Article/details/gazvihvxc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fktsv.cn/Article/details/gsejxrccg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.sjlbkw.cn/Article/details/gagesytze.sHtML

[D02] 追加元素到末尾
来源：http://3g.tarul.cn/Article/details/gkanhhhfj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.vehdjk.com/Article/details/gyxhysjsu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.vehdjk.com/Article/details/grasdlhro.sHtML

JS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/glttbsxwr.sHtML

TS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/ghtzbtapi.sHtML

Java: list.add(4);
来源：http://wap.vehdjk.com/Article/details/guhqqehxq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gtebtggre.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.tarul.cn/Article/details/gjqbptxod.sHtML

C#:   list.Add(4);
来源：http://m.share.yfazqb.com/Article/details/ghjtluxxb.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.vehdjk.com/Article/details/gglddszqr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gzxlsreza.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.epnwcf.com/Article/details/gexxggyip.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.yfazqb.com/Article/details/gxxqpraft.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.vehdjk.com/Article/details/gaalzlskn.sHtML

Java: list.add(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gikobdsav.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.sjlbkw.cn/Article/details/grsuijgtb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.yfazqb.com/Article/details/gxknqlpec.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.bbcook.cn/Article/details/gxmoslcpo.sHtML

[D04] 删除元素
来源：http://mobile.yfazqb.com/Article/details/ghgistckg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.tarul.cn/Article/details/gdtuhbllx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwhxxupy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.tarul.cn/Article/details/gngrehigj.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fktsv.cn/Article/details/goddfdweo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.sjlbkw.cn/Article/details/gqxgvqjgp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.bbcook.cn/Article/details/ggqqybysg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.yfazqb.com/Article/details/gjykuxork.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.vehdjk.com/Article/details/gvhqxbdrk.sHtML

[D05] 访问与修改元素
来源：http://mobile.tarul.cn/Article/details/gsazxndqd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/gaupfjufg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gyixlxcar.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gnkgvqubc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fktsv.cn/Article/details/gwehauafd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.vehdjk.com/Article/details/gpbqgzvno.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gushtqoce.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/glyrhpota.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gecphhtpq.sHtML

[D06] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gohnrxfgp.sHtML

Py:   len(arr)
来源：http://wap.tarul.cn/Article/details/grqzvswje.sHtML

PHP:  count($arr);
来源：http://read.share.vehdjk.com/Article/details/gwtdyqcic.sHtML

JS:   arr.length
来源：http://mobile.yfazqb.com/Article/details/gvwwpstrf.sHtML

TS:   arr.length
来源：http://blog.bbcook.cn/Article/details/ghvjwuccv.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/gecphbeah.sHtML

Go:   len(arr)
来源：http://blog.fktsv.cn/Article/details/gvoojyppf.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.tarul.cn/Article/details/ghgajjxhy.sHtML

C#:   list.Count;
来源：http://wap.bbcook.cn/Article/details/gwmruwpnx.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fktsv.cn/Article/details/gtnfzkngi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.yfazqb.com/Article/details/gfglbxkfc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.bbcook.cn/Article/details/gzzvwikmf.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.bbcook.cn/Article/details/gcpfkrwxt.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/ghbdnrmpr.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gfrnreqqi.sHtML

Go:   arr[1:4]
来源：http://www.m.share.tarul.cn/Article/details/gsijjsfwa.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.vehdjk.com/Article/details/gkxbmnlsc.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.yfazqb.com/Article/details/gmccmrvij.sHtML

[D08] 合并两个数组
来源：http://www.share.tarul.cn/Article/details/ggfzrpuax.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.yfazqb.com/Article/details/gbjirqnfd.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.vehdjk.com/Article/details/ghggppegu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.sjlbkw.cn/Article/details/gvmbljoeo.sHtML

TS:   [...a, ...b];
来源：http://wap.yfazqb.com/Article/details/gxfoouggz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.tarul.cn/Article/details/gyobsajbd.sHtML

Go:   append(a, b...)
来源：http://3g.fktsv.cn/Article/details/grqurgmqe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.vehdjk.com/Article/details/gcqfvfxue.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.bbcook.cn/Article/details/gqwfyigxc.sHtML

[D09] 排序（升序）
来源：http://m.share.epnwcf.com/Article/details/gqntdmnxb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gxtnnhvjj.sHtML

PHP:  sort($arr);
来源：http://www.blog.vehdjk.com/Article/details/gkodqusle.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fktsv.cn/Article/details/gqsvjgbgs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.sjlbkw.cn/Article/details/gpuwhkkeo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.bbcook.cn/Article/details/gatxfrnjb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/gxrdxsmxn.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gcizfhjlb.sHtML

C#:   list.Sort();
来源：http://m.share.vehdjk.com/Article/details/gasqnpcgm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.yfazqb.com/Article/details/geygpejuy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.tarul.cn/Article/details/gqdzpbodv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.vehdjk.com/Article/details/gqpolewdb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gshdcrsjv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.epnwcf.com/Article/details/gprpzsezk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.vehdjk.com/Article/details/gczkzkjsr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.bbcook.cn/Article/details/gxvlgxskr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fktsv.cn/Article/details/gxhcomgvu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.tarul.cn/Article/details/gwstnylgz.sHtML

[D11] 反转数组
来源：http://mobile.bbcook.cn/Article/details/gggglqvsk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.yfazqb.com/Article/details/gajcqsdit.sHtML

PHP:  array_reverse($arr);
来源：http://3g.tarul.cn/Article/details/gmcskbszw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.sjlbkw.cn/Article/details/gakyrgezy.sHtML

TS:   [...arr].reverse();
来源：http://baike.fktsv.cn/Article/details/gtkkguqrr.sHtML

Java: Collections.reverse(list);
来源：http://3g.vehdjk.com/Article/details/gdbyusavq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gqorwhxad.sHtML

Ruby: arr.reverse
来源：http://www.share.bbcook.cn/Article/details/ggnpmjelc.sHtML

C#:   list.Reverse();
来源：http://www.blog.sjlbkw.cn/Article/details/gahwelllu.sHtML

[D12] 查找元素下标
来源：http://3g.vehdjk.com/Article/details/gzmhhlxed.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gpmekhacb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.yfazqb.com/Article/details/gyyhxrzlf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gsakldbdi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.bbcook.cn/Article/details/guwsszhxk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.bbcook.cn/Article/details/gexaekklc.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gzvynqbgo.sHtML

Ruby: arr.index(x)
来源：http://mobile.tarul.cn/Article/details/gfznwhjsm.sHtML

C#:   list.IndexOf(x);
来源：http://blog.yfazqb.com/Article/details/ghqligdrj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.vehdjk.com/Article/details/groplusmp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fktsv.cn/Article/details/gfwvisfiv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.vehdjk.com/Article/details/gwpzhbbic.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.yfazqb.com/Article/details/gelvoovul.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.vehdjk.com/Article/details/gyqwuzxta.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.yfazqb.com/Article/details/gkvsssssb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.vehdjk.com/Article/details/gbdybskze.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.epnwcf.com/Article/details/gqgmabpre.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.bbcook.cn/Article/details/gcfwpxeyu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.yfazqb.com/Article/details/gwtgnhotu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.vehdjk.com/Article/details/gtkhseddt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.bbcook.cn/Article/details/gujievxji.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/gdhgxoprz.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/gnsrwtwms.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.tarul.cn/Article/details/gdawkirgx.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gwvuqlvpv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.tarul.cn/Article/details/gcuayktsp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.tarul.cn/Article/details/gebdtwrac.sHtML

[D15] 去重
来源：http://3g.tarul.cn/Article/details/gmrvtpoak.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/geagzpuxc.sHtML

PHP:  array_unique($arr);
来源：http://blog.yfazqb.com/Article/details/gudlqaxom.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/govkkorlg.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gxldvfkrg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.yfazqb.com/Article/details/gwqeohemy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.tarul.cn/Article/details/gnaxyutjd.sHtML

Ruby: arr.uniq
来源：http://www.blog.bbcook.cn/Article/details/ggryermym.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.yfazqb.com/Article/details/gsomilpvu.sHtML

[D16] 求和与平均值
来源：http://m.share.fktsv.cn/Article/details/gyxfofqkt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fktsv.cn/Article/details/gidopzvil.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gpdumcuua.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fktsv.cn/Article/details/gjxbvnvxx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/gpsthfdkm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.sjlbkw.cn/Article/details/gueffspng.sHtML

Go:   // 手写循环累加
来源：http://baike.yfazqb.com/Article/details/gchzcvilh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.epnwcf.com/Article/details/ggojhnadd.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.epnwcf.com/Article/details/gmvqfbmbq.sHtML

[D17] 最大值与最小值
来源：http://blog.yfazqb.com/Article/details/guezjaqin.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.tarul.cn/Article/details/gwgqodmwj.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.vehdjk.com/Article/details/gjcxkqhbl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.yfazqb.com/Article/details/gtojqvjdy.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.tarul.cn/Article/details/gddbglhbh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.vehdjk.com/Article/details/gjbwadwvm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.bbcook.cn/Article/details/gkcyjmifs.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/gcnqwrbkp.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.vehdjk.com/Article/details/gyxvrobsa.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.epnwcf.com/Article/details/gykprolid.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.epnwcf.com/Article/details/gtlhirvog.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fktsv.cn/Article/details/gjwesuibw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.sjlbkw.cn/Article/details/gkbjjxwgl.sHtML

TS:   nested.flat();
来源：http://wap.epnwcf.com/Article/details/gwyueuzbd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.bbcook.cn/Article/details/guwryglwo.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdvgdoct.sHtML

Ruby: nested.flatten
来源：http://www.m.share.epnwcf.com/Article/details/gqziokaol.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.epnwcf.com/Article/details/gowtrwwyq.sHtML

[D19] 按字段分组
来源：http://www.blog.fktsv.cn/Article/details/gvxkxdfpi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.yfazqb.com/Article/details/gsmfezavn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.vehdjk.com/Article/details/gafixrvoh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.yfazqb.com/Article/details/gxjueveqn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/glfbmbxzz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.tarul.cn/Article/details/gklmsqrgs.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.yfazqb.com/Article/details/gynlyueyh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fktsv.cn/Article/details/giqvfzqns.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fktsv.cn/Article/details/glaldtapq.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.vehdjk.com/Article/details/gtedqagas.sHtML

Py:   Counter(arr)
来源：http://mobile.yfazqb.com/Article/details/gmpvhktws.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fktsv.cn/Article/details/gtaupnqgh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.bbcook.cn/Article/details/guctybjto.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.vehdjk.com/Article/details/gfblcqjej.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.bbcook.cn/Article/details/grvvhyhic.sHtML

Go:   // 手写 map[T]int
来源：http://3g.tarul.cn/Article/details/goumcaybb.sHtML

Ruby: arr.tally
来源：http://wap.epnwcf.com/Article/details/gunzfooec.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.sjlbkw.cn/Article/details/gpplglexn.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.vehdjk.com/Article/details/guhctffqh.sHtML

Py:   x in arr
来源：http://blog.tarul.cn/Article/details/grslrbvnb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fktsv.cn/Article/details/grgjnxwki.sHtML

JS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/gjydseqsn.sHtML

TS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/gnowrfpys.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/ghupnzsst.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.bbcook.cn/Article/details/gsucvlbmj.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/gbfztbirr.sHtML

C#:   list.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gkaezcvnz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fktsv.cn/Article/details/gtjnqnqgi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.epnwcf.com/Article/details/gzleizilo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.sjlbkw.cn/Article/details/gvugfjxcl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.vehdjk.com/Article/details/gyamzwbps.sHtML

TS:   [...arr];
来源：http://wap.sjlbkw.cn/Article/details/ghhodntae.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.yfazqb.com/Article/details/gbjjdfzlj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjiveqgtp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.bbcook.cn/Article/details/gfyzjnmxb.sHtML

C#:   new List<int>(list);
来源：http://mobile.epnwcf.com/Article/details/gbuyhdobu.sHtML

[D23] reduce 累积计算
来源：http://m.share.vehdjk.com/Article/details/gnyxqflvf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.bbcook.cn/Article/details/griwcsoob.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fktsv.cn/Article/details/gdpkfykas.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gzlprdfvg.sHtML


<!-- 参考信息 -->