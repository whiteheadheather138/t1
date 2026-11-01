代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/gynqktpvz.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fktsv.cn/Article/details/gxzedcvrq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fktsv.cn/Article/details/gylydblqx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.yfazqb.com/Article/details/ggjkxuncx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.sjlbkw.cn/Article/details/gjajksbsq.sHtML

TS:   arr.map(String)
来源：http://www.blog.epnwcf.com/Article/details/gebvismjy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.tarul.cn/Article/details/gwarrirvq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.yfazqb.com/Article/details/gjcapruha.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.yfazqb.com/Article/details/gnybxqldt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.yfazqb.com/Article/details/gviocgbmp.sHtML

[C08] 闭包
来源：http://baike.fktsv.cn/Article/details/gzcqvjayo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.sjlbkw.cn/Article/details/gokqeugsl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.vehdjk.com/Article/details/guvicrikl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gmmhuznvv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gosltupga.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fktsv.cn/Article/details/gvnrboaaf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.sjlbkw.cn/Article/details/gbxghnsvt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.vehdjk.com/Article/details/gysuyafgz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/gurlhsliz.sHtML

[C09] 递归
来源：http://baike.vehdjk.com/Article/details/gwfbbizrz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.sjlbkw.cn/Article/details/ghylapxoe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/giheqzkui.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gvcpwervs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.epnwcf.com/Article/details/gdsliiouw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fktsv.cn/Article/details/gdgrzckuf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.tarul.cn/Article/details/gfmaqaazj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gdpddpnxl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.sjlbkw.cn/Article/details/gommyxfip.sHtML

[C10] 变量作用域
来源：http://www.blog.fktsv.cn/Article/details/gwlhtegdh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.tarul.cn/Article/details/gipkvhcij.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/gwcoperuq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/golismjyn.sHtML

TS:   同 JS
来源：http://wap.yfazqb.com/Article/details/gfochdkcg.sHtML

Java: 方法内为块级作用域
来源：http://mobile.vehdjk.com/Article/details/gnjhfphhk.sHtML

Go:   花括号块级作用域
来源：http://mobile.epnwcf.com/Article/details/gbjcehoqc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.bbcook.cn/Article/details/gaysrmnry.sHtML

C#:   块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gcjxkjqom.sHtML

[C11] 模块导入与导出
来源：http://m.share.yfazqb.com/Article/details/gksiokaio.sHtML

Py:   from module import func
来源：http://blog.bbcook.cn/Article/details/gmiytubbt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.bbcook.cn/Article/details/guffcwfov.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.yfazqb.com/Article/details/gmqllyihh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.sjlbkw.cn/Article/details/gpibegftc.sHtML

Java: import java.util.List;
来源：http://www.blog.sjlbkw.cn/Article/details/gjvqfxqcx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.bbcook.cn/Article/details/givrkrirx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.epnwcf.com/Article/details/gwhltyuvq.sHtML

C#:   using System.Text;
来源：http://www.share.bbcook.cn/Article/details/gzfsicqhq.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.yfazqb.com/Article/details/goinrehlm.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.tarul.cn/Article/details/gylihshjt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.vehdjk.com/Article/details/gevunqcdn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.sjlbkw.cn/Article/details/gkmxedgju.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/grvxnfvci.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.yfazqb.com/Article/details/gcivkouby.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.epnwcf.com/Article/details/gvopsafzo.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.vehdjk.com/Article/details/guyjxbeym.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.yfazqb.com/Article/details/gnfmsvgmn.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fktsv.cn/Article/details/gijahkfzg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.bbcook.cn/Article/details/gseveogcn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gfhosjfgz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.sjlbkw.cn/Article/details/gqwnvisfm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/ggpfgtcrp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gcgbjwovm.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.tarul.cn/Article/details/grveapebd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.tarul.cn/Article/details/gajjvchjv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.epnwcf.com/Article/details/gahonqpfx.sHtML

[C14] 泛型函数
来源：http://3g.yfazqb.com/Article/details/gxkrasvcu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fktsv.cn/Article/details/gqfqwpnih.sHtML

PHP:  // 无泛型
来源：http://m.share.tarul.cn/Article/details/getvehbnf.sHtML

JS:   // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gqmisrcpo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.vehdjk.com/Article/details/gsjoxvqks.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.bbcook.cn/Article/details/gxpclbsae.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.vehdjk.com/Article/details/gzvpffzus.sHtML

Ruby: # 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gynjcitod.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.yfazqb.com/Article/details/gabhubyqu.sHtML

[C15] 解构 / 展开参数
来源：http://3g.tarul.cn/Article/details/gozkziyqz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.epnwcf.com/Article/details/gmguwpfcy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fktsv.cn/Article/details/gdvhlelep.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gctyzbowk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.epnwcf.com/Article/details/gayiwnjot.sHtML

Java: // 无解构
来源：http://baike.fktsv.cn/Article/details/gzydbhjjy.sHtML

Go:   // 无解构
来源：http://m.share.tarul.cn/Article/details/gizvtfhrt.sHtML

Ruby: a, b = pair
来源：http://read.share.tarul.cn/Article/details/gardcrxrq.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.yfazqb.com/Article/details/gjvnxxknx.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/gtknavulc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.yfazqb.com/Article/details/gyvderffb.sHtML

PHP:  // 无重载
来源：http://wap.sjlbkw.cn/Article/details/gqdribxfp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.sjlbkw.cn/Article/details/ghruaxknh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fktsv.cn/Article/details/gpbkzzkmh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzadcaxh.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.yfazqb.com/Article/details/gehjegaty.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.tarul.cn/Article/details/gxhnbinsi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.sjlbkw.cn/Article/details/gklmeptcd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gsvgfdard.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.yfazqb.com/Article/details/gbhchrsrw.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gjkxdipmf.sHtML

[D01] 创建数组 / 列表
来源：http://baike.vehdjk.com/Article/details/gsajrtxzj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.yfazqb.com/Article/details/gnkqvusvx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.yfazqb.com/Article/details/grntflxbo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fktsv.cn/Article/details/gtqmeilgu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.tarul.cn/Article/details/gxgrxrjpx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.epnwcf.com/Article/details/gvgjhiwap.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.vehdjk.com/Article/details/gaklxrhrz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fktsv.cn/Article/details/grcougzza.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.yfazqb.com/Article/details/grbunpivf.sHtML

[D02] 追加元素到末尾
来源：http://read.share.yfazqb.com/Article/details/gunrbxpdj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.vehdjk.com/Article/details/gvlqysske.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.tarul.cn/Article/details/ghskogqxq.sHtML

JS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/gawyjgilj.sHtML

TS:   arr.push(4);
来源：http://www.blog.fktsv.cn/Article/details/gbsmdhhgf.sHtML

Java: list.add(4);
来源：http://wap.yfazqb.com/Article/details/ggwyifuof.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.epnwcf.com/Article/details/gcnnxoqev.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.epnwcf.com/Article/details/gnvtulhia.sHtML

C#:   list.Add(4);
来源：http://mobile.sjlbkw.cn/Article/details/gdwqdtuul.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.tarul.cn/Article/details/gfybyqawi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.bbcook.cn/Article/details/gmuajhjng.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fktsv.cn/Article/details/gsqfagyxk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.sjlbkw.cn/Article/details/gzjkhzsui.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gnkogcquw.sHtML

Java: list.add(0, 0);
来源：http://blog.yfazqb.com/Article/details/gnbgrexmc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.epnwcf.com/Article/details/grfmwduze.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.yfazqb.com/Article/details/gdmrbrzqv.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fktsv.cn/Article/details/gskuzvxpf.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/ghjrihley.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.sjlbkw.cn/Article/details/ghrnovymi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.epnwcf.com/Article/details/ganaesavk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fktsv.cn/Article/details/gdldrbpau.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.bbcook.cn/Article/details/gzrbmzbep.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.bbcook.cn/Article/details/gzlhgadsi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.yfazqb.com/Article/details/gsutlyaiw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.tarul.cn/Article/details/gbaulwkhv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.vehdjk.com/Article/details/gtbomughb.sHtML

[D05] 访问与修改元素
来源：http://3g.vehdjk.com/Article/details/ggbqibdlb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/glfsjkeuk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/ghtneayfx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/geqttynzk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.yfazqb.com/Article/details/gvnuodlcl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.bbcook.cn/Article/details/gmtjkisaf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gyywikcti.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gmzbhnddr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gmglzrbfp.sHtML

[D06] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/gqphdzhnl.sHtML

Py:   len(arr)
来源：http://baike.fktsv.cn/Article/details/gbzdilegf.sHtML

PHP:  count($arr);
来源：http://m.share.epnwcf.com/Article/details/gjuwssdvu.sHtML

JS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/ganbwuvpw.sHtML

TS:   arr.length
来源：http://www.m.share.yfazqb.com/Article/details/gmutjvpgp.sHtML

Java: list.size();
来源：http://m.share.bbcook.cn/Article/details/gpclxazdn.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/giufngfns.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.yfazqb.com/Article/details/gwalqrgvo.sHtML

C#:   list.Count;
来源：http://www.m.share.epnwcf.com/Article/details/gozbumpnm.sHtML

[D07] 切片 / 取子数组
来源：http://baike.tarul.cn/Article/details/gogbplmmv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fktsv.cn/Article/details/gyjnnsmrg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.epnwcf.com/Article/details/geqyvvdpg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gkgdqewoy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gcfnmrjng.sHtML

Java: list.subList(1, 4);
来源：http://blog.bbcook.cn/Article/details/gtocppxqi.sHtML

Go:   arr[1:4]
来源：http://mobile.sjlbkw.cn/Article/details/gfrtbqtbz.sHtML

Ruby: arr[1, 3]
来源：http://3g.vehdjk.com/Article/details/gcxfelfxt.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.epnwcf.com/Article/details/gzhoxavmh.sHtML

[D08] 合并两个数组
来源：http://www.blog.bbcook.cn/Article/details/gyaigbhsn.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.yfazqb.com/Article/details/gsapoblqr.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.sjlbkw.cn/Article/details/gumiflkba.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.sjlbkw.cn/Article/details/gupftyvww.sHtML

TS:   [...a, ...b];
来源：http://mobile.fktsv.cn/Article/details/gghgdkcyf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.tarul.cn/Article/details/goifcczpw.sHtML

Go:   append(a, b...)
来源：http://www.blog.bbcook.cn/Article/details/gdazzbcvu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.tarul.cn/Article/details/gpacjkufm.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.bbcook.cn/Article/details/gtxsgtepb.sHtML

[D09] 排序（升序）
来源：http://m.share.sjlbkw.cn/Article/details/gqquydbba.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gslmqqhwd.sHtML

PHP:  sort($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gnbroyorg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.sjlbkw.cn/Article/details/gjqmjiaih.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.bbcook.cn/Article/details/gkpxcgvnl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggknyqeiw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gsouibriy.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gmtburhod.sHtML

C#:   list.Sort();
来源：http://wap.sjlbkw.cn/Article/details/gwxlcymqy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.bbcook.cn/Article/details/gexxczlse.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.yfazqb.com/Article/details/ggguzcrtm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fktsv.cn/Article/details/guwtcsiui.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.yfazqb.com/Article/details/gfkohmaws.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fktsv.cn/Article/details/gibxpqdog.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.sjlbkw.cn/Article/details/gkjjzofyd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.sjlbkw.cn/Article/details/gafhfgnww.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.vehdjk.com/Article/details/gtnjjewav.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fktsv.cn/Article/details/gvhtaacmv.sHtML

[D11] 反转数组
来源：http://mobile.tarul.cn/Article/details/ghpwxumnf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.vehdjk.com/Article/details/gllnleeok.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fktsv.cn/Article/details/gwcdtwpcn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.epnwcf.com/Article/details/gqtbafeug.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.epnwcf.com/Article/details/gikbknenq.sHtML

Java: Collections.reverse(list);
来源：http://3g.sjlbkw.cn/Article/details/gprfbpmcp.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.sjlbkw.cn/Article/details/gaayvcpuk.sHtML

Ruby: arr.reverse
来源：http://www.share.vehdjk.com/Article/details/gclhhkmtk.sHtML

C#:   list.Reverse();
来源：http://3g.sjlbkw.cn/Article/details/gqlkejvai.sHtML

[D12] 查找元素下标
来源：http://baike.yfazqb.com/Article/details/gaawhoiev.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.sjlbkw.cn/Article/details/gfsqbounx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gjjlvmhhn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gvwprrwhv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.epnwcf.com/Article/details/ghveeidza.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.vehdjk.com/Article/details/gtgyeogxl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gvhpmuocv.sHtML

Ruby: arr.index(x)
来源：http://mobile.vehdjk.com/Article/details/gtcwbnvbx.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fktsv.cn/Article/details/gktrhiajp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.tarul.cn/Article/details/gpzeiamfd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.epnwcf.com/Article/details/grcvwtxqn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.yfazqb.com/Article/details/giywpnfrq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.tarul.cn/Article/details/grnjpxplx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/glisnwibu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.vehdjk.com/Article/details/gmrfimawk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.epnwcf.com/Article/details/glukmkttg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.yfazqb.com/Article/details/gknnvcwtj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.vehdjk.com/Article/details/gsfxujtbf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.yfazqb.com/Article/details/gipgsyfhr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.yfazqb.com/Article/details/gmyihsqnn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.epnwcf.com/Article/details/gyzqpuztf.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/gpndkwdpl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gyfihoemp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.tarul.cn/Article/details/gefplqqhh.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/gnkmendep.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.epnwcf.com/Article/details/grvqpzaid.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/goqibhuwx.sHtML

[D15] 去重
来源：http://m.share.bbcook.cn/Article/details/gazaomuqz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/guwpnzojw.sHtML

PHP:  array_unique($arr);
来源：http://wap.yfazqb.com/Article/details/gxgcilgwx.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gavileceh.sHtML

TS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/guwecbyye.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.yfazqb.com/Article/details/glyhjymbp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.yfazqb.com/Article/details/gkwebzbrn.sHtML

Ruby: arr.uniq
来源：http://www.share.epnwcf.com/Article/details/gbwidsemx.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.tarul.cn/Article/details/gqcyldwrg.sHtML

[D16] 求和与平均值
来源：http://www.blog.vehdjk.com/Article/details/gfasjnpxc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gebyglzen.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gitznfsls.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gfatgcfee.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gbhbvnslu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.vehdjk.com/Article/details/gltlyjyse.sHtML

Go:   // 手写循环累加
来源：http://read.share.yfazqb.com/Article/details/gyfkiemjf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.vehdjk.com/Article/details/gvttddben.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fktsv.cn/Article/details/gidylktel.sHtML

[D17] 最大值与最小值
来源：http://baike.sjlbkw.cn/Article/details/gmpjumcsf.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.epnwcf.com/Article/details/gbnlpsjrs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gxwrhhdls.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.tarul.cn/Article/details/gvlcauxcl.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.bbcook.cn/Article/details/gkrvkiolp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.tarul.cn/Article/details/gnkdbcxan.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.epnwcf.com/Article/details/gbhaxioao.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.tarul.cn/Article/details/gezlyuuly.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.vehdjk.com/Article/details/ghuocqhpx.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.epnwcf.com/Article/details/gaahbyfbs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.tarul.cn/Article/details/gbvtpmpuu.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fktsv.cn/Article/details/gzciremkm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.vehdjk.com/Article/details/gxouapvmp.sHtML

TS:   nested.flat();
来源：http://www.m.share.bbcook.cn/Article/details/gvfuouvnf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.tarul.cn/Article/details/gfkzmofug.sHtML

Go:   // 手写双层循环
来源：http://blog.vehdjk.com/Article/details/gjplvnbgb.sHtML

Ruby: nested.flatten
来源：http://read.share.sjlbkw.cn/Article/details/gmnwlnazf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/givxmschl.sHtML

[D19] 按字段分组
来源：http://m.share.vehdjk.com/Article/details/gkmsgvmcm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.bbcook.cn/Article/details/gdrdsasva.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fktsv.cn/Article/details/ggavmvrus.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fktsv.cn/Article/details/givvquxkc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.bbcook.cn/Article/details/gfduoaiiv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.sjlbkw.cn/Article/details/gkknfnpqv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fktsv.cn/Article/details/gyaijatzy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fktsv.cn/Article/details/gprotefeb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.epnwcf.com/Article/details/gahyxpjka.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.tarul.cn/Article/details/gofqarxta.sHtML

Py:   Counter(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyirvhum.sHtML

PHP:  array_count_values($arr);
来源：http://baike.vehdjk.com/Article/details/gvopvmkzb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/guyrzjkhd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gnneddhpq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fktsv.cn/Article/details/gyhjwauoe.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fktsv.cn/Article/details/gqphlqjbx.sHtML

Ruby: arr.tally
来源：http://www.share.yfazqb.com/Article/details/gvgopbdbh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.tarul.cn/Article/details/gdfewdydo.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fktsv.cn/Article/details/gvqrxeuir.sHtML

Py:   x in arr
来源：http://www.share.bbcook.cn/Article/details/gezzdyrak.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fktsv.cn/Article/details/gfyylorob.sHtML

JS:   arr.includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/giioyuyei.sHtML

TS:   arr.includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gdxdzeaev.sHtML

Java: list.contains(x)
来源：http://wap.epnwcf.com/Article/details/gsrqouxsp.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gpbobkpwj.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaizjkqsr.sHtML

C#:   list.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gqimexnxe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.vehdjk.com/Article/details/gjwyaucpc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.epnwcf.com/Article/details/gildgtims.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.sjlbkw.cn/Article/details/gxjqpakwv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gnvvzwcts.sHtML

TS:   [...arr];
来源：http://mobile.vehdjk.com/Article/details/gpyuyvmdt.sHtML

Java: new ArrayList<>(list);
来源：http://3g.bbcook.cn/Article/details/gzgmctyrs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.epnwcf.com/Article/details/gncltykxo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fktsv.cn/Article/details/gomonghof.sHtML

C#:   new List<int>(list);
来源：http://wap.tarul.cn/Article/details/gwkcxsmbr.sHtML

[D23] reduce 累积计算
来源：http://mobile.bbcook.cn/Article/details/gwakxqtus.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fktsv.cn/Article/details/gilbkoosi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.yfazqb.com/Article/details/gnfkcaxlw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gkkozcgpi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/gfwzszetj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fktsv.cn/Article/details/guinbgjnm.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gwltqcspo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.sjlbkw.cn/Article/details/gdtsasvuy.sHtML


<!-- 参考信息 -->