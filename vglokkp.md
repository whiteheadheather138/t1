代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/gtztduafo.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.yfazqb.com/Article/details/gvvtaatwi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.sjlbkw.cn/Article/details/gsyjeyxtr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.yfazqb.com/Article/details/grursccqy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.yfazqb.com/Article/details/gwbiashhw.sHtML

TS:   arr.map(String)
来源：http://baike.yfazqb.com/Article/details/goqxrfsjq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.yfazqb.com/Article/details/gqvbirvhj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.tarul.cn/Article/details/ganwfqsdk.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.bbcook.cn/Article/details/ggckmuerk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.epnwcf.com/Article/details/gizzkfxot.sHtML

[C08] 闭包
来源：http://baike.fktsv.cn/Article/details/gfucemrye.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.yfazqb.com/Article/details/gfwhnxlfw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.bbcook.cn/Article/details/glglqavzb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/glubwdlmt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gwnfqgsdc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.tarul.cn/Article/details/gklwmhecz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.vehdjk.com/Article/details/gxwfqxbip.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fktsv.cn/Article/details/gyeejzuph.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/getwanxru.sHtML

[C09] 递归
来源：http://3g.sjlbkw.cn/Article/details/gpsamaexi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/geqldbdgh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.epnwcf.com/Article/details/gpiblmydd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/gqugsvfas.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/gbzynufbe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.sjlbkw.cn/Article/details/gvbpjtnwm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.vehdjk.com/Article/details/gdxmdugzh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/gtsdhkrzq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.tarul.cn/Article/details/grxkuxnvg.sHtML

[C10] 变量作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyvbtxry.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fktsv.cn/Article/details/gkrokblxf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.sjlbkw.cn/Article/details/gywqjdcmj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.epnwcf.com/Article/details/gydpsakuq.sHtML

TS:   同 JS
来源：http://wap.tarul.cn/Article/details/gghoedkio.sHtML

Java: 方法内为块级作用域
来源：http://m.share.bbcook.cn/Article/details/geyrgjcuv.sHtML

Go:   花括号块级作用域
来源：http://baike.epnwcf.com/Article/details/gwaaklfot.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fktsv.cn/Article/details/gnzkslagv.sHtML

C#:   块级作用域
来源：http://mobile.yfazqb.com/Article/details/geclkdibl.sHtML

[C11] 模块导入与导出
来源：http://baike.sjlbkw.cn/Article/details/gfeyarykn.sHtML

Py:   from module import func
来源：http://www.share.tarul.cn/Article/details/gjqhuxbcu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.tarul.cn/Article/details/gyqoepsgv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.epnwcf.com/Article/details/gvxlzcmiq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.bbcook.cn/Article/details/guntyscvf.sHtML

Java: import java.util.List;
来源：http://3g.epnwcf.com/Article/details/gnnpldyhj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.vehdjk.com/Article/details/glknlyinr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.yfazqb.com/Article/details/giufbdjxs.sHtML

C#:   using System.Text;
来源：http://www.share.bbcook.cn/Article/details/gftagasze.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fktsv.cn/Article/details/goelpyaad.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjoxnefmt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.bbcook.cn/Article/details/gqnrqxwcz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gslqjxych.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/gxdhcrzss.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.yfazqb.com/Article/details/gftqpigpa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.vehdjk.com/Article/details/gccppmdyg.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.yfazqb.com/Article/details/glxpsimvo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.yfazqb.com/Article/details/gxwqnrtfu.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.bbcook.cn/Article/details/gzqglqpzd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.yfazqb.com/Article/details/gnjdvowwc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gtljjorqx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fktsv.cn/Article/details/gbhqsovvn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gqsjfjwfg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gerbwcinp.sHtML

Go:   func add(a, b int) int
来源：http://blog.epnwcf.com/Article/details/gcpilzzpv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.bbcook.cn/Article/details/ghjythgaw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.yfazqb.com/Article/details/gslzhwwlu.sHtML

[C14] 泛型函数
来源：http://mobile.vehdjk.com/Article/details/gdxpafxvi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.sjlbkw.cn/Article/details/gvoumecaz.sHtML

PHP:  // 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/gkgiqcall.sHtML

JS:   // 无泛型
来源：http://wap.bbcook.cn/Article/details/gdzwqrenb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fktsv.cn/Article/details/gpidbfjiy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fktsv.cn/Article/details/gneycmpep.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fktsv.cn/Article/details/gnalomfxj.sHtML

Ruby: # 无泛型
来源：http://mobile.tarul.cn/Article/details/goqgrfhqb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.vehdjk.com/Article/details/gxcsznfmc.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.epnwcf.com/Article/details/ggroqkico.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.epnwcf.com/Article/details/grxvbrukz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.bbcook.cn/Article/details/gqmflkndz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gqbxhfvjy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.yfazqb.com/Article/details/guwfckccn.sHtML

Java: // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gqbsfoabz.sHtML

Go:   // 无解构
来源：http://www.m.share.epnwcf.com/Article/details/gblkociwc.sHtML

Ruby: a, b = pair
来源：http://www.m.share.epnwcf.com/Article/details/gchyivwly.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.epnwcf.com/Article/details/gzlzsmriv.sHtML

[C16] 函数 / 方法重载
来源：http://blog.vehdjk.com/Article/details/gxokgjwrn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.sjlbkw.cn/Article/details/gkkfuxxzd.sHtML

PHP:  // 无重载
来源：http://www.m.share.bbcook.cn/Article/details/grgoxdmrf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.tarul.cn/Article/details/gjnshmxbw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.vehdjk.com/Article/details/gsocdyjjm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.bbcook.cn/Article/details/gvfnudlcn.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.sjlbkw.cn/Article/details/gjbcevoal.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fktsv.cn/Article/details/ggccznskw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.sjlbkw.cn/Article/details/grfaljbea.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/geoshjzyy.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.tarul.cn/Article/details/grrfoelpy.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmpvspmrb.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gxejzqash.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.yfazqb.com/Article/details/gxxujazhp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.epnwcf.com/Article/details/gmamgwpex.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.sjlbkw.cn/Article/details/ghhivipaf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.vehdjk.com/Article/details/galjxobuu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.bbcook.cn/Article/details/gonohufpz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.sjlbkw.cn/Article/details/godsqojam.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.epnwcf.com/Article/details/gwagkrtud.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.sjlbkw.cn/Article/details/gniuhjwfb.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fktsv.cn/Article/details/givttwntb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.bbcook.cn/Article/details/gilspckmt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fktsv.cn/Article/details/gheyophjy.sHtML

JS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/glvqksogd.sHtML

TS:   arr.push(4);
来源：http://www.share.tarul.cn/Article/details/gvcitvkuk.sHtML

Java: list.add(4);
来源：http://read.share.bbcook.cn/Article/details/gyeubwmta.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.epnwcf.com/Article/details/gfajvnmvg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fktsv.cn/Article/details/gcjtxjszd.sHtML

C#:   list.Add(4);
来源：http://3g.tarul.cn/Article/details/gcbecjbft.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.bbcook.cn/Article/details/ghdnzuxjt.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.epnwcf.com/Article/details/gdoytrrjv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.yfazqb.com/Article/details/gebkunspc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fktsv.cn/Article/details/gkfqkibhp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gzhxohstr.sHtML

Java: list.add(0, 0);
来源：http://www.share.vehdjk.com/Article/details/goxsvxmiv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fktsv.cn/Article/details/gzbjrghxg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.yfazqb.com/Article/details/glaoaoalt.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.vehdjk.com/Article/details/gvevuxjwh.sHtML

[D04] 删除元素
来源：http://m.share.epnwcf.com/Article/details/gjpbnlajn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.yfazqb.com/Article/details/gavdpfble.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.vehdjk.com/Article/details/ghoseeovr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.vehdjk.com/Article/details/gdgtsxkto.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.sjlbkw.cn/Article/details/gcsaqvrki.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.tarul.cn/Article/details/gsrnnzzbu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.vehdjk.com/Article/details/gxvnlwtue.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fktsv.cn/Article/details/ghilzesqk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.epnwcf.com/Article/details/gnhrtcgfa.sHtML

[D05] 访问与修改元素
来源：http://wap.vehdjk.com/Article/details/gjqnzcbdl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/glvhrvfyy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/gpkhuglfr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gcpwkktkk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.vehdjk.com/Article/details/gxpwaquqw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.bbcook.cn/Article/details/gjicfjeio.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gnwsxhzeo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxljnixo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gbosrpxvm.sHtML

[D06] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gksxwzjtv.sHtML

Py:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/grldynert.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gqkkrlxza.sHtML

JS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gysjtjzgu.sHtML

TS:   arr.length
来源：http://wap.tarul.cn/Article/details/gfhpyquuo.sHtML

Java: list.size();
来源：http://www.share.tarul.cn/Article/details/gqkbvtlqy.sHtML

Go:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/ggtvzpycu.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.yfazqb.com/Article/details/guabcblbw.sHtML

C#:   list.Count;
来源：http://www.m.share.yfazqb.com/Article/details/ghvhoqxey.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.bbcook.cn/Article/details/grwbfhadu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fktsv.cn/Article/details/gnyyepmky.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gsizdcvpn.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gfiukenwy.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.epnwcf.com/Article/details/gemdecgxi.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gatacdgkl.sHtML

Go:   arr[1:4]
来源：http://blog.tarul.cn/Article/details/gbjebrmop.sHtML

Ruby: arr[1, 3]
来源：http://blog.tarul.cn/Article/details/gvkbpprja.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.yfazqb.com/Article/details/gussursgg.sHtML

[D08] 合并两个数组
来源：http://3g.vehdjk.com/Article/details/gwysmwolo.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.epnwcf.com/Article/details/grtujhmov.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.bbcook.cn/Article/details/gtnacqygt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.sjlbkw.cn/Article/details/gafgxvxir.sHtML

TS:   [...a, ...b];
来源：http://baike.fktsv.cn/Article/details/gymqskeob.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.bbcook.cn/Article/details/gwibgedfv.sHtML

Go:   append(a, b...)
来源：http://baike.epnwcf.com/Article/details/gjzbfzpsv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.tarul.cn/Article/details/gvsowauuq.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.tarul.cn/Article/details/genvffvbx.sHtML

[D09] 排序（升序）
来源：http://mobile.epnwcf.com/Article/details/gmcjaxndf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/gfvgmjiem.sHtML

PHP:  sort($arr);
来源：http://www.share.bbcook.cn/Article/details/gvkfsabik.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.vehdjk.com/Article/details/gadkhlbxf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.sjlbkw.cn/Article/details/gcclwzuta.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.yfazqb.com/Article/details/gnshdonvm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gegtvsmpl.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gbgzeecil.sHtML

C#:   list.Sort();
来源：http://3g.sjlbkw.cn/Article/details/gdmxwmdht.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fktsv.cn/Article/details/gxlgmxmdn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.epnwcf.com/Article/details/gixhptccx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.bbcook.cn/Article/details/gxzgtrhev.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gjmkmhapd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/gwnyrvfni.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.epnwcf.com/Article/details/guoxqerxd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.bbcook.cn/Article/details/ghpjwrpge.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fktsv.cn/Article/details/glxccnlki.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.bbcook.cn/Article/details/gfztajfjb.sHtML

[D11] 反转数组
来源：http://www.share.sjlbkw.cn/Article/details/gaaaplnbw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.vehdjk.com/Article/details/ghlejloiy.sHtML

PHP:  array_reverse($arr);
来源：http://blog.yfazqb.com/Article/details/gohfsmfxr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.epnwcf.com/Article/details/ghkcwqqbf.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.bbcook.cn/Article/details/gjcgwnnam.sHtML

Java: Collections.reverse(list);
来源：http://baike.bbcook.cn/Article/details/gbgogxlkw.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fktsv.cn/Article/details/gzcytnryv.sHtML

Ruby: arr.reverse
来源：http://wap.vehdjk.com/Article/details/gkiuoczeb.sHtML

C#:   list.Reverse();
来源：http://wap.epnwcf.com/Article/details/gudvqdtxw.sHtML

[D12] 查找元素下标
来源：http://read.share.vehdjk.com/Article/details/gqbcvpgnc.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fktsv.cn/Article/details/gbyvqafon.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.epnwcf.com/Article/details/gojxerpke.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/gjdlplghf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/ghjtcwmod.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.yfazqb.com/Article/details/gwcthrlqh.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gynzshgno.sHtML

Ruby: arr.index(x)
来源：http://3g.yfazqb.com/Article/details/gpzuvnflb.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.sjlbkw.cn/Article/details/gzptimtzq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.sjlbkw.cn/Article/details/gofodiecg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gamyiwmch.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.vehdjk.com/Article/details/ggsictgpg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/grzhxjgii.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gblpeaflt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.yfazqb.com/Article/details/gwpkilyqw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.sjlbkw.cn/Article/details/gamkkbqes.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.bbcook.cn/Article/details/gaawenahi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.tarul.cn/Article/details/gnogsljqt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.bbcook.cn/Article/details/gogrdeckf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.bbcook.cn/Article/details/grfmgjiux.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.epnwcf.com/Article/details/grqsaylxd.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/goecztnve.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.sjlbkw.cn/Article/details/gbuevmctm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gvefrypti.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/gjqejwqwb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/guyvjqsas.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gpmdubswe.sHtML

[D15] 去重
来源：http://3g.bbcook.cn/Article/details/gkgqaxzqv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fktsv.cn/Article/details/gpdftjfxs.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.tarul.cn/Article/details/gbbvwiqbq.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gbyibauck.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gewsxqouz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.yfazqb.com/Article/details/gaxiqiaoj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.vehdjk.com/Article/details/glepbickm.sHtML

Ruby: arr.uniq
来源：http://m.share.sjlbkw.cn/Article/details/gmdcghvay.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.bbcook.cn/Article/details/gpdfzaxvu.sHtML

[D16] 求和与平均值
来源：http://www.share.bbcook.cn/Article/details/goptleuss.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.vehdjk.com/Article/details/gygicnirc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.yfazqb.com/Article/details/ghjfxvgtr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/ghnbjocep.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gnxaxweik.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fktsv.cn/Article/details/gjmpfnejb.sHtML

Go:   // 手写循环累加
来源：http://baike.epnwcf.com/Article/details/gjencrizr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.tarul.cn/Article/details/gqsyjaxiz.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.tarul.cn/Article/details/gxzatnydx.sHtML

[D17] 最大值与最小值
来源：http://www.share.bbcook.cn/Article/details/glyvytaqx.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/ggyakgunx.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fktsv.cn/Article/details/gmrwyivkc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.epnwcf.com/Article/details/gsrdhuqdk.sHtML

TS:   Math.max(...arr);
来源：http://baike.tarul.cn/Article/details/gkeukmhox.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.tarul.cn/Article/details/grndbacjd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.sjlbkw.cn/Article/details/gzbogebxq.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.epnwcf.com/Article/details/gsjulozca.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.bbcook.cn/Article/details/gurucyyzj.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.sjlbkw.cn/Article/details/geemqbxrx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fktsv.cn/Article/details/gvjmwccbb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.epnwcf.com/Article/details/gdroyxxbk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/gcxstzpax.sHtML

TS:   nested.flat();
来源：http://m.share.yfazqb.com/Article/details/gzdrmpvsv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.bbcook.cn/Article/details/gtamwiqce.sHtML

Go:   // 手写双层循环
来源：http://3g.fktsv.cn/Article/details/gziiathcz.sHtML

Ruby: nested.flatten
来源：http://wap.fktsv.cn/Article/details/gfidutgjw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.yfazqb.com/Article/details/ghkqwnxiw.sHtML

[D19] 按字段分组
来源：http://www.share.epnwcf.com/Article/details/gfmekxvsg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.sjlbkw.cn/Article/details/gcqdcpmae.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmsxbwkq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.sjlbkw.cn/Article/details/gqwdxmpze.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gdlxllsjt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.yfazqb.com/Article/details/ghehaotdv.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.tarul.cn/Article/details/geijrgsdh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fktsv.cn/Article/details/gzhynhalx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.vehdjk.com/Article/details/ggipjrxpp.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.yfazqb.com/Article/details/gvwpzkclq.sHtML

Py:   Counter(arr)
来源：http://m.share.epnwcf.com/Article/details/gxydfjfgq.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsedcmpe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fktsv.cn/Article/details/gfplthupj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/gdakooacn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fktsv.cn/Article/details/gmpepwjni.sHtML

Go:   // 手写 map[T]int
来源：http://blog.tarul.cn/Article/details/gezvxdhau.sHtML

Ruby: arr.tally
来源：http://m.share.tarul.cn/Article/details/girzebzsm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fktsv.cn/Article/details/guxyfvbqg.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.vehdjk.com/Article/details/gnnyyffnk.sHtML

Py:   x in arr
来源：http://www.m.share.epnwcf.com/Article/details/ghaeqixqj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.bbcook.cn/Article/details/gexrosigm.sHtML

JS:   arr.includes(x)
来源：http://blog.bbcook.cn/Article/details/gaaquicdj.sHtML

TS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gvofhyurg.sHtML

Java: list.contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gfgwherwo.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.yfazqb.com/Article/details/gvumlmzoo.sHtML

Ruby: arr.include?(x)
来源：http://mobile.vehdjk.com/Article/details/gqezcjtnf.sHtML

C#:   list.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gnqomkcgn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fktsv.cn/Article/details/gcrctxghc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gmzqvsmjh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.tarul.cn/Article/details/giazfhizh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.vehdjk.com/Article/details/ggwvfjmft.sHtML

TS:   [...arr];
来源：http://blog.epnwcf.com/Article/details/grkewyrlj.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.tarul.cn/Article/details/gbpmfeuvu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fktsv.cn/Article/details/gjkjsekvb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.tarul.cn/Article/details/gvtpskbrx.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.epnwcf.com/Article/details/ghfzolxnx.sHtML

[D23] reduce 累积计算
来源：http://3g.epnwcf.com/Article/details/gaqvzoczm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.epnwcf.com/Article/details/gbmhwybni.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.vehdjk.com/Article/details/gsfhfqrrc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.tarul.cn/Article/details/gilnxbehj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gnpkhuzts.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.tarul.cn/Article/details/gyeppkbcp.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/gxkcuczyh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.bbcook.cn/Article/details/gyqycnfil.sHtML


<!-- 参考信息 -->