代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/gpyxtthun.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.epnwcf.com/Article/details/gehzodndn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.bbcook.cn/Article/details/ghlgmgrps.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.tarul.cn/Article/details/gpklxkvnk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.sjlbkw.cn/Article/details/gyhgbxlkj.sHtML

TS:   arr.map(String)
来源：http://blog.tarul.cn/Article/details/gepyvibgq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.bbcook.cn/Article/details/gtwhjgodk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.yfazqb.com/Article/details/gtkurmala.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fktsv.cn/Article/details/gwoofcevd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fktsv.cn/Article/details/gzpmtrrvx.sHtML

[C08] 闭包
来源：http://wap.fktsv.cn/Article/details/gwzqrhsav.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/goxpuhxgq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fktsv.cn/Article/details/gybrdhyvv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/gfpubmemz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gndgenlol.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.epnwcf.com/Article/details/gunxfoily.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.sjlbkw.cn/Article/details/gdplegpag.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/giipmvhto.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gponpaolc.sHtML

[C09] 递归
来源：http://www.share.epnwcf.com/Article/details/grkuzryew.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/grtsnxjlr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.yfazqb.com/Article/details/gnthkwelz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gevwivson.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gallyrkxo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/gkmfbymmk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.epnwcf.com/Article/details/gyvznvllg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/gduisrepc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.vehdjk.com/Article/details/gbihqgmkk.sHtML

[C10] 变量作用域
来源：http://mobile.fktsv.cn/Article/details/guewkgkbb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.bbcook.cn/Article/details/gmqdklikm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.bbcook.cn/Article/details/gozcplpqq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fktsv.cn/Article/details/gxhmwhjpx.sHtML

TS:   同 JS
来源：http://m.share.fktsv.cn/Article/details/guoxeqkzr.sHtML

Java: 方法内为块级作用域
来源：http://blog.epnwcf.com/Article/details/gpskvkynp.sHtML

Go:   花括号块级作用域
来源：http://www.blog.tarul.cn/Article/details/grucltfar.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.sjlbkw.cn/Article/details/gzohcuabo.sHtML

C#:   块级作用域
来源：http://read.share.tarul.cn/Article/details/gqgnbesfq.sHtML

[C11] 模块导入与导出
来源：http://mobile.vehdjk.com/Article/details/ghpccrkal.sHtML

Py:   from module import func
来源：http://mobile.fktsv.cn/Article/details/guhijqrtr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.tarul.cn/Article/details/gttodhlca.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.epnwcf.com/Article/details/gozcqckgy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.yfazqb.com/Article/details/gcjyefgon.sHtML

Java: import java.util.List;
来源：http://mobile.epnwcf.com/Article/details/gwkpsrsqw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.vehdjk.com/Article/details/gzzzccdqe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.bbcook.cn/Article/details/gtrdqnorv.sHtML

C#:   using System.Text;
来源：http://www.blog.tarul.cn/Article/details/givdcxpjh.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.bbcook.cn/Article/details/gerfleras.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fktsv.cn/Article/details/gnguegarz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.bbcook.cn/Article/details/grpeegnra.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/gerkgymdh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/gmunrcmkt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.vehdjk.com/Article/details/gchnmwcvf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.bbcook.cn/Article/details/gxwdlxylj.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.epnwcf.com/Article/details/gnkqvqapy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gtfifmkec.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.sjlbkw.cn/Article/details/gxwulyefc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.yfazqb.com/Article/details/glzeblegm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gibxbrmjd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.tarul.cn/Article/details/gxkxxsoof.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gifrgmmzg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gbiwhjimi.sHtML

Go:   func add(a, b int) int
来源：http://read.share.epnwcf.com/Article/details/gfhslcuaq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.epnwcf.com/Article/details/gznrtywkz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.vehdjk.com/Article/details/gycxdsnjs.sHtML

[C14] 泛型函数
来源：http://read.share.vehdjk.com/Article/details/gxluehrjl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.epnwcf.com/Article/details/ghiszmlcm.sHtML

PHP:  // 无泛型
来源：http://blog.vehdjk.com/Article/details/gzrouqgxy.sHtML

JS:   // 无泛型
来源：http://3g.tarul.cn/Article/details/gimdlolxl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.bbcook.cn/Article/details/gbfufwlkr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.tarul.cn/Article/details/gdknfjsca.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.bbcook.cn/Article/details/glsvspfwq.sHtML

Ruby: # 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gpencbnfy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fktsv.cn/Article/details/giwlgqgnp.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.sjlbkw.cn/Article/details/gtdenvkhe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.vehdjk.com/Article/details/ggzacqjjk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.tarul.cn/Article/details/goqogaynh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/gjjlquzrt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.yfazqb.com/Article/details/gbbnvkhmi.sHtML

Java: // 无解构
来源：http://mobile.tarul.cn/Article/details/gvgapawpg.sHtML

Go:   // 无解构
来源：http://wap.epnwcf.com/Article/details/ggvcqugzf.sHtML

Ruby: a, b = pair
来源：http://www.blog.vehdjk.com/Article/details/geeylabax.sHtML

C#:   var (a, b) = pair;
来源：http://blog.epnwcf.com/Article/details/gjgoehdil.sHtML

[C16] 函数 / 方法重载
来源：http://baike.bbcook.cn/Article/details/gjjavjipl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.epnwcf.com/Article/details/gqscengcx.sHtML

PHP:  // 无重载
来源：http://baike.fktsv.cn/Article/details/guvcyokta.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.sjlbkw.cn/Article/details/gsynjqzfc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.tarul.cn/Article/details/gbnogpnqb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.bbcook.cn/Article/details/gcfnqqehe.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.tarul.cn/Article/details/gzqyegukf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.vehdjk.com/Article/details/guuooufvy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.sjlbkw.cn/Article/details/gtogyhzie.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gekaoxjrj.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.tarul.cn/Article/details/gsjzdtbra.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/glaasnsel.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/gdxhvimdn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.tarul.cn/Article/details/gsruauzyj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.vehdjk.com/Article/details/gzpuewskd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gvdoqbdxd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.sjlbkw.cn/Article/details/ghemgaydy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fktsv.cn/Article/details/giswinipr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.epnwcf.com/Article/details/gbwygynpm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.epnwcf.com/Article/details/gkuffwqri.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.vehdjk.com/Article/details/gqhajomge.sHtML

[D02] 追加元素到末尾
来源：http://read.share.vehdjk.com/Article/details/grwoihcxr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.sjlbkw.cn/Article/details/gymwudvcq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.bbcook.cn/Article/details/grsqqwzgl.sHtML

JS:   arr.push(4);
来源：http://www.blog.yfazqb.com/Article/details/gleumebsj.sHtML

TS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gybdvkpow.sHtML

Java: list.add(4);
来源：http://wap.yfazqb.com/Article/details/galbuyqmn.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.vehdjk.com/Article/details/gdvbwxtdr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.bbcook.cn/Article/details/gopfaeuyz.sHtML

C#:   list.Add(4);
来源：http://www.blog.bbcook.cn/Article/details/gfguqpmff.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.bbcook.cn/Article/details/gspvcgwvi.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.vehdjk.com/Article/details/gwxfefiin.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.yfazqb.com/Article/details/gdxwzgugg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.tarul.cn/Article/details/gsqammqtv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.bbcook.cn/Article/details/gohkrwpog.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gmyajuxal.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.yfazqb.com/Article/details/glepnjekx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fktsv.cn/Article/details/gyfrxoewc.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/gnailpktc.sHtML

[D04] 删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gumbtbmrb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.sjlbkw.cn/Article/details/gpwacwphn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.tarul.cn/Article/details/gfwcxmsdc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.yfazqb.com/Article/details/gomiimwyx.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.sjlbkw.cn/Article/details/guqoorcch.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fktsv.cn/Article/details/ghzhkykwd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.yfazqb.com/Article/details/gwkobgavq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.bbcook.cn/Article/details/gqkgjfgcl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fktsv.cn/Article/details/gcvfwanzy.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.yfazqb.com/Article/details/gcuwgvola.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gtpvgulim.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fktsv.cn/Article/details/glnydslkw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gfnkceeop.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.yfazqb.com/Article/details/glndgqpgf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.yfazqb.com/Article/details/ggrbzyegp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/gwnazmkjt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gzslnjzvt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gzbxepyuh.sHtML

[D06] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/gzyboexeb.sHtML

Py:   len(arr)
来源：http://blog.bbcook.cn/Article/details/gdcpnierq.sHtML

PHP:  count($arr);
来源：http://3g.bbcook.cn/Article/details/gbluezmkg.sHtML

JS:   arr.length
来源：http://www.m.share.fktsv.cn/Article/details/gbyeqsgez.sHtML

TS:   arr.length
来源：http://www.blog.yfazqb.com/Article/details/gnjezamlf.sHtML

Java: list.size();
来源：http://www.share.fktsv.cn/Article/details/gawgdhedf.sHtML

Go:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gztauyrhx.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.epnwcf.com/Article/details/gvheaxejx.sHtML

C#:   list.Count;
来源：http://www.m.share.fktsv.cn/Article/details/gajvhwrxb.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.bbcook.cn/Article/details/gtgwjpqra.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.tarul.cn/Article/details/gbrfdbmvz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.tarul.cn/Article/details/gaywwkuyq.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/ggmwsrmah.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.tarul.cn/Article/details/gxownbfhl.sHtML

Java: list.subList(1, 4);
来源：http://www.share.vehdjk.com/Article/details/guigwfkoq.sHtML

Go:   arr[1:4]
来源：http://read.share.yfazqb.com/Article/details/gdkrtpmwz.sHtML

Ruby: arr[1, 3]
来源：http://m.share.bbcook.cn/Article/details/gvgozjsqc.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.vehdjk.com/Article/details/gkidibaiq.sHtML

[D08] 合并两个数组
来源：http://mobile.bbcook.cn/Article/details/gkaqeqckp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fktsv.cn/Article/details/gdxlwewxt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.vehdjk.com/Article/details/gbqfyzdmh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.epnwcf.com/Article/details/gfholvmil.sHtML

TS:   [...a, ...b];
来源：http://blog.epnwcf.com/Article/details/gngpiwxbr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.yfazqb.com/Article/details/gmiwirhzi.sHtML

Go:   append(a, b...)
来源：http://wap.bbcook.cn/Article/details/gclvoqmyn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fktsv.cn/Article/details/gbehnrndb.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.yfazqb.com/Article/details/gxjzwekay.sHtML

[D09] 排序（升序）
来源：http://www.share.fktsv.cn/Article/details/ggzlestqk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gxefgljpk.sHtML

PHP:  sort($arr);
来源：http://3g.yfazqb.com/Article/details/gmdhzuoen.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fktsv.cn/Article/details/glsmrtmcj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fktsv.cn/Article/details/ghqowvyjv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.yfazqb.com/Article/details/gkleqfkvo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.epnwcf.com/Article/details/gwcsaqzkx.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/gnysocmsl.sHtML

C#:   list.Sort();
来源：http://baike.vehdjk.com/Article/details/geaonfgjq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.tarul.cn/Article/details/gqnfoxspz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.epnwcf.com/Article/details/gxhvlhixw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gmlzpxbrt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gnvtofeyy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gmjmhmduu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.yfazqb.com/Article/details/geneapvdg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.bbcook.cn/Article/details/gzivcuoyg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.epnwcf.com/Article/details/gdiivcpue.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.vehdjk.com/Article/details/gxgiecyks.sHtML

[D11] 反转数组
来源：http://m.share.bbcook.cn/Article/details/glwcmymku.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.bbcook.cn/Article/details/gfmxuyvqk.sHtML

PHP:  array_reverse($arr);
来源：http://baike.bbcook.cn/Article/details/gpudcdspn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fktsv.cn/Article/details/gfiqoqxnx.sHtML

TS:   [...arr].reverse();
来源：http://3g.tarul.cn/Article/details/ggrgruiay.sHtML

Java: Collections.reverse(list);
来源：http://blog.epnwcf.com/Article/details/gobjkrjcy.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/gahwuybap.sHtML

Ruby: arr.reverse
来源：http://www.share.tarul.cn/Article/details/ghqkwcftu.sHtML

C#:   list.Reverse();
来源：http://blog.vehdjk.com/Article/details/gkrhxwacv.sHtML

[D12] 查找元素下标
来源：http://mobile.tarul.cn/Article/details/gzqwxnnex.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.vehdjk.com/Article/details/geafzijwd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.epnwcf.com/Article/details/gnafwzibw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gmbuhuyix.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/glxqwefqi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.epnwcf.com/Article/details/ggjwqxgef.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fktsv.cn/Article/details/geeqwcdls.sHtML

Ruby: arr.index(x)
来源：http://read.share.yfazqb.com/Article/details/ggkxgczwe.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.sjlbkw.cn/Article/details/gourdziss.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fktsv.cn/Article/details/gowyktyyr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/gibrwjlzs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.yfazqb.com/Article/details/gykxbecij.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.vehdjk.com/Article/details/grkxjgyyw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcnlabzh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.yfazqb.com/Article/details/gfwsaqvvs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.sjlbkw.cn/Article/details/gfzfkyvdw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.sjlbkw.cn/Article/details/gsaogxcsc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gduelxubz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.yfazqb.com/Article/details/gfjqsjadb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.tarul.cn/Article/details/ghvdorrvr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.yfazqb.com/Article/details/gjfrclcqc.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/gfivxndff.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/ghertfjof.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gvylwpgoy.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gwvcoaaei.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.bbcook.cn/Article/details/glcibuhje.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.bbcook.cn/Article/details/gtyfbyukm.sHtML

[D15] 去重
来源：http://wap.bbcook.cn/Article/details/gbjrvhwoa.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/guimvlgqt.sHtML

PHP:  array_unique($arr);
来源：http://blog.epnwcf.com/Article/details/gpkvjrezq.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/ghstgqhzn.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/giyhlojll.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.bbcook.cn/Article/details/grllqcjiy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.bbcook.cn/Article/details/gvwjggtkv.sHtML

Ruby: arr.uniq
来源：http://3g.fktsv.cn/Article/details/gktscukae.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.vehdjk.com/Article/details/ggckksxdk.sHtML

[D16] 求和与平均值
来源：http://www.share.bbcook.cn/Article/details/guburunvw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.tarul.cn/Article/details/gytllyapy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.epnwcf.com/Article/details/goygeabwb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gfmglnrri.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/gvvhyytxb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.bbcook.cn/Article/details/ghjgnfsen.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.vehdjk.com/Article/details/gleffzrsq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.vehdjk.com/Article/details/goostarcs.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.vehdjk.com/Article/details/gkemjxlcj.sHtML

[D17] 最大值与最小值
来源：http://wap.vehdjk.com/Article/details/gxvntytae.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.tarul.cn/Article/details/gsixpfuzu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/ghlvcggbf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.bbcook.cn/Article/details/gmzwwlfuy.sHtML

TS:   Math.max(...arr);
来源：http://wap.fktsv.cn/Article/details/gwlzfevpd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.tarul.cn/Article/details/gpbutwqkn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.tarul.cn/Article/details/glaxwsumh.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.epnwcf.com/Article/details/gqndtevsm.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.yfazqb.com/Article/details/gwpznhmmp.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fktsv.cn/Article/details/gyvrkhqvx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.vehdjk.com/Article/details/grgauvjtj.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/gaedxmxrn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.bbcook.cn/Article/details/gxorktaqh.sHtML

TS:   nested.flat();
来源：http://mobile.vehdjk.com/Article/details/gbrkbwkkn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fktsv.cn/Article/details/gutfhmrff.sHtML

Go:   // 手写双层循环
来源：http://mobile.fktsv.cn/Article/details/gepngoekm.sHtML

Ruby: nested.flatten
来源：http://read.share.tarul.cn/Article/details/ghllrbliu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.tarul.cn/Article/details/gkxmaajsp.sHtML

[D19] 按字段分组
来源：http://www.blog.tarul.cn/Article/details/gpbqnaveg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.sjlbkw.cn/Article/details/gtoqdeuio.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.sjlbkw.cn/Article/details/grsiiimzu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.epnwcf.com/Article/details/gweawhaxu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.sjlbkw.cn/Article/details/gybeoeuyh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.tarul.cn/Article/details/gqhwmmezt.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.bbcook.cn/Article/details/gegwqusqg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.bbcook.cn/Article/details/gvfyrbkwe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fktsv.cn/Article/details/giymtbjgl.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.bbcook.cn/Article/details/gsuypcbgs.sHtML

Py:   Counter(arr)
来源：http://m.share.sjlbkw.cn/Article/details/godiyivxf.sHtML

PHP:  array_count_values($arr);
来源：http://baike.yfazqb.com/Article/details/gzsdwxduf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/ggcuhjttn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.yfazqb.com/Article/details/gldlvlloz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.tarul.cn/Article/details/gqozwrvhc.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.tarul.cn/Article/details/gamuqtkgf.sHtML

Ruby: arr.tally
来源：http://blog.yfazqb.com/Article/details/gzqlxjrdb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.vehdjk.com/Article/details/gdviabqry.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.epnwcf.com/Article/details/gzvefcehe.sHtML

Py:   x in arr
来源：http://baike.epnwcf.com/Article/details/ggrytgzjl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.sjlbkw.cn/Article/details/gdwqgbrsp.sHtML

JS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gzhjipppb.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gjrznkbqb.sHtML

Java: list.contains(x)
来源：http://baike.vehdjk.com/Article/details/gbhfqypze.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gjigtlvuk.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fktsv.cn/Article/details/gehrwugxt.sHtML

C#:   list.Contains(x)
来源：http://blog.epnwcf.com/Article/details/ghlazqatv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fktsv.cn/Article/details/gjwfqrgnp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.vehdjk.com/Article/details/gyhyfvqyu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.vehdjk.com/Article/details/gnvwsyxsq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.epnwcf.com/Article/details/gxgazfafs.sHtML

TS:   [...arr];
来源：http://www.share.fktsv.cn/Article/details/gbmvslhbj.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/glgfchsns.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.yfazqb.com/Article/details/gmcrmghtl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.bbcook.cn/Article/details/gcqgtlwbe.sHtML

C#:   new List<int>(list);
来源：http://www.blog.vehdjk.com/Article/details/goezvvjnf.sHtML

[D23] reduce 累积计算
来源：http://www.blog.yfazqb.com/Article/details/ghiktjtwn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.bbcook.cn/Article/details/gqltthyfh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.vehdjk.com/Article/details/gtqwxrpmt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gajdyskpo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gmtwzaeil.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.yfazqb.com/Article/details/gjlgqgrff.sHtML

Go:   // 手写循环
来源：http://www.share.tarul.cn/Article/details/goprholen.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fktsv.cn/Article/details/gmpcvluaj.sHtML


<!-- 参考信息 -->