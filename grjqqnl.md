代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.blog.vehdjk.com/Article/details/gtblycicv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gbtuvhejj.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gdcdxjnsm.sHtML

[C05] 返回多个值
来源：http://m.share.tarul.cn/Article/details/goudmxoqd.sHtML

Py:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gidiasseu.sHtML

PHP:  return [$a, $b];
来源：http://m.share.epnwcf.com/Article/details/gvukkmsbf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gjdelnggx.sHtML

TS:   return { a, b };
来源：http://blog.fktsv.cn/Article/details/gtbgnlzrl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.tarul.cn/Article/details/guspeaxdg.sHtML

Go:   return a, b
来源：http://m.share.tarul.cn/Article/details/gofxqlbsf.sHtML

Ruby: return a, b
来源：http://3g.sjlbkw.cn/Article/details/gdiubbjkl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.epnwcf.com/Article/details/gtpjvwmjd.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.tarul.cn/Article/details/ggqdzbzlx.sHtML

Py:   square = lambda x: x * x
来源：http://blog.bbcook.cn/Article/details/gajdsdqzf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.tarul.cn/Article/details/geqlhweqs.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gmjaalkbf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gheldulfg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.tarul.cn/Article/details/glmasnljr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.tarul.cn/Article/details/gaiforaju.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.vehdjk.com/Article/details/guzcqfsld.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/goqbbhqbo.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.yfazqb.com/Article/details/gqbbinjev.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.epnwcf.com/Article/details/gycolctdc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.vehdjk.com/Article/details/gitqygtvz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.vehdjk.com/Article/details/gssxyhsoz.sHtML

TS:   arr.map(String)
来源：http://www.m.share.bbcook.cn/Article/details/gqoqlnhue.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.bbcook.cn/Article/details/gxwgncxvn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.tarul.cn/Article/details/gyiwmawoh.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.sjlbkw.cn/Article/details/gtjadunzj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.sjlbkw.cn/Article/details/geohurttx.sHtML

[C08] 闭包
来源：http://blog.yfazqb.com/Article/details/gemonmedg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.sjlbkw.cn/Article/details/gimonwfpo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.yfazqb.com/Article/details/gtiwqgaab.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gkdkvxaly.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gcxgqellc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.sjlbkw.cn/Article/details/gltvmvust.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.tarul.cn/Article/details/glwuqoxlx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.bbcook.cn/Article/details/gljwtdztk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gzamsaeao.sHtML

[C09] 递归
来源：http://blog.sjlbkw.cn/Article/details/gmleguczi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gyctwklnv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.bbcook.cn/Article/details/gzrmndmsj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.tarul.cn/Article/details/gsyhaafgb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gcmnkippt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/gmwtfekws.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.epnwcf.com/Article/details/gisqfwjeu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fktsv.cn/Article/details/gzyvmljsd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.tarul.cn/Article/details/gqjdjgnrt.sHtML

[C10] 变量作用域
来源：http://read.share.vehdjk.com/Article/details/gbnmftowa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.yfazqb.com/Article/details/grwxanuqs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.epnwcf.com/Article/details/ggaaozqsc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.sjlbkw.cn/Article/details/gyeanyjpm.sHtML

TS:   同 JS
来源：http://www.blog.vehdjk.com/Article/details/gxtvdpjol.sHtML

Java: 方法内为块级作用域
来源：http://m.share.yfazqb.com/Article/details/gyuoweelm.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gljosqbxx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.vehdjk.com/Article/details/goveeekdp.sHtML

C#:   块级作用域
来源：http://www.blog.tarul.cn/Article/details/gysctbmce.sHtML

[C11] 模块导入与导出
来源：http://m.share.bbcook.cn/Article/details/gbapscjwd.sHtML

Py:   from module import func
来源：http://www.share.bbcook.cn/Article/details/gkvgixfwf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.epnwcf.com/Article/details/gztxugxvo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.bbcook.cn/Article/details/gzqbwezku.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fktsv.cn/Article/details/gxvyjgfbo.sHtML

Java: import java.util.List;
来源：http://www.blog.fktsv.cn/Article/details/gmujesgii.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.bbcook.cn/Article/details/gkelthvac.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.epnwcf.com/Article/details/gcahtxxxx.sHtML

C#:   using System.Text;
来源：http://blog.tarul.cn/Article/details/gtmddffzz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.epnwcf.com/Article/details/gslxdhisx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.sjlbkw.cn/Article/details/gzhamuuai.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fktsv.cn/Article/details/gccsojzoj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gzvvodwbp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.epnwcf.com/Article/details/gizokyrtz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.vehdjk.com/Article/details/gljquqmww.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.epnwcf.com/Article/details/gllrugbyq.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.sjlbkw.cn/Article/details/grfbmmofi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.sjlbkw.cn/Article/details/geqnnxbdv.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.yfazqb.com/Article/details/gogqrobun.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.yfazqb.com/Article/details/ggyagzkpk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/galgcufui.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.epnwcf.com/Article/details/gkwjxzrrf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/ggnfxuapx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gpdbiejra.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/gallosrbt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fktsv.cn/Article/details/gfrzcpxty.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.epnwcf.com/Article/details/gavbbckqq.sHtML

[C14] 泛型函数
来源：http://www.m.share.tarul.cn/Article/details/gzebhryhm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.tarul.cn/Article/details/gmlwlcqas.sHtML

PHP:  // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gaoelbxwx.sHtML

JS:   // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gyectktkr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.sjlbkw.cn/Article/details/ggbvltfbd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.bbcook.cn/Article/details/gstasytrn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.tarul.cn/Article/details/gbzlatmsz.sHtML

Ruby: # 无泛型
来源：http://baike.bbcook.cn/Article/details/gnqrarfsf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.yfazqb.com/Article/details/gdkgicylj.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.epnwcf.com/Article/details/gohrcgwup.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fktsv.cn/Article/details/gszpvwhql.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.tarul.cn/Article/details/gpaedauff.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/ggaijqopc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gxsnxbirz.sHtML

Java: // 无解构
来源：http://blog.bbcook.cn/Article/details/gyomdnmzn.sHtML

Go:   // 无解构
来源：http://baike.epnwcf.com/Article/details/gbuaazkpx.sHtML

Ruby: a, b = pair
来源：http://wap.yfazqb.com/Article/details/gvpjpgypi.sHtML

C#:   var (a, b) = pair;
来源：http://blog.vehdjk.com/Article/details/gpniglpad.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fktsv.cn/Article/details/gjdvwonvx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.yfazqb.com/Article/details/ggyogqylr.sHtML

PHP:  // 无重载
来源：http://mobile.vehdjk.com/Article/details/ggjidnlpg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.bbcook.cn/Article/details/gfaeberih.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.tarul.cn/Article/details/ghflqetdf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.vehdjk.com/Article/details/gfmqbzfem.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.tarul.cn/Article/details/gvhxffkfk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.yfazqb.com/Article/details/gsiluucdl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.tarul.cn/Article/details/gujseqpuh.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqrbsfrnz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.bbcook.cn/Article/details/gxjbpllgn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghogqjmhj.sHtML

[D01] 创建数组 / 列表
来源：http://3g.tarul.cn/Article/details/gavlnmghb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.sjlbkw.cn/Article/details/gzgtldkej.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.tarul.cn/Article/details/gntelamtk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.bbcook.cn/Article/details/gsriyxlhx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.yfazqb.com/Article/details/gagsaawff.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.bbcook.cn/Article/details/grtppbytg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fktsv.cn/Article/details/gpoxfzhns.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.yfazqb.com/Article/details/gtwppzwgu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.yfazqb.com/Article/details/gnjqqxfbu.sHtML

[D02] 追加元素到末尾
来源：http://m.share.bbcook.cn/Article/details/ggfzmcegv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.bbcook.cn/Article/details/gbcdayugs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fktsv.cn/Article/details/grijyjxth.sHtML

JS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gqieqqmjj.sHtML

TS:   arr.push(4);
来源：http://mobile.fktsv.cn/Article/details/gppbfwivn.sHtML

Java: list.add(4);
来源：http://www.m.share.bbcook.cn/Article/details/gfnehgugt.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gcobmpdtz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.bbcook.cn/Article/details/gtnyitvsv.sHtML

C#:   list.Add(4);
来源：http://mobile.yfazqb.com/Article/details/gqroqfgli.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.tarul.cn/Article/details/gffrmylde.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.sjlbkw.cn/Article/details/gpmooflkc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.vehdjk.com/Article/details/gxivzxbie.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.yfazqb.com/Article/details/guvhelsmz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.sjlbkw.cn/Article/details/glcxcykvj.sHtML

Java: list.add(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gsfsagoir.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fktsv.cn/Article/details/gozqpdhfy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.bbcook.cn/Article/details/gurchxmzr.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fktsv.cn/Article/details/gfghvcjbr.sHtML

[D04] 删除元素
来源：http://www.share.epnwcf.com/Article/details/gtouvmgpk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.vehdjk.com/Article/details/gyyzpcjrc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.yfazqb.com/Article/details/ggrkwpffs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.vehdjk.com/Article/details/glwuchwem.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.epnwcf.com/Article/details/gmhxcbkid.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.bbcook.cn/Article/details/glffrrkkx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fktsv.cn/Article/details/gnuowsspk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/gpugkwxae.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fktsv.cn/Article/details/gtkjshxfc.sHtML

[D05] 访问与修改元素
来源：http://www.share.vehdjk.com/Article/details/gyzhlhvrq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gptaextgo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/gppitroot.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gushxpzph.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.bbcook.cn/Article/details/gdgvayzpy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.sjlbkw.cn/Article/details/ggsnwqzga.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/grldulwhk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gpjaszyvg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/glsbbswgd.sHtML

[D06] 数组长度
来源：http://wap.vehdjk.com/Article/details/ggzggwjdl.sHtML

Py:   len(arr)
来源：http://wap.bbcook.cn/Article/details/gogbipwyi.sHtML

PHP:  count($arr);
来源：http://www.blog.fktsv.cn/Article/details/gntnltjgw.sHtML

JS:   arr.length
来源：http://baike.yfazqb.com/Article/details/gnxaztjgq.sHtML

TS:   arr.length
来源：http://www.share.epnwcf.com/Article/details/gpkawogdw.sHtML

Java: list.size();
来源：http://www.m.share.bbcook.cn/Article/details/gdpwppfzh.sHtML

Go:   len(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gbhaxzvzl.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsjdlvki.sHtML

C#:   list.Count;
来源：http://www.blog.fktsv.cn/Article/details/gzdoqlzik.sHtML

[D07] 切片 / 取子数组
来源：http://wap.tarul.cn/Article/details/glzybcsdc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.tarul.cn/Article/details/gutpqwdov.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fktsv.cn/Article/details/gjwvkknyy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzidwtcl.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gyjcakmqk.sHtML

Java: list.subList(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gqsbgxbjs.sHtML

Go:   arr[1:4]
来源：http://mobile.sjlbkw.cn/Article/details/gllgxrwfh.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.tarul.cn/Article/details/gohiywddv.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.yfazqb.com/Article/details/gzvovaznq.sHtML

[D08] 合并两个数组
来源：http://blog.yfazqb.com/Article/details/gjlweagbg.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.bbcook.cn/Article/details/gkmdmrjhc.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.vehdjk.com/Article/details/gjulaaseo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.vehdjk.com/Article/details/glmzhcqwi.sHtML

TS:   [...a, ...b];
来源：http://blog.vehdjk.com/Article/details/grohdjdjf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.tarul.cn/Article/details/gpgboodpi.sHtML

Go:   append(a, b...)
来源：http://m.share.vehdjk.com/Article/details/gxrxgflta.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fktsv.cn/Article/details/gbufgidld.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gtlbhpozg.sHtML

[D09] 排序（升序）
来源：http://m.share.yfazqb.com/Article/details/gwblvnncf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/glfjzfpkw.sHtML

PHP:  sort($arr);
来源：http://wap.bbcook.cn/Article/details/giowuxpsd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.yfazqb.com/Article/details/guoqkotbc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.vehdjk.com/Article/details/gjqgftunv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.epnwcf.com/Article/details/gddakjnaj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gktmhqeyo.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gzzollxoa.sHtML

C#:   list.Sort();
来源：http://www.m.share.sjlbkw.cn/Article/details/gkoqzzbru.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.tarul.cn/Article/details/ghyudikxh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.yfazqb.com/Article/details/gegycxxzv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.epnwcf.com/Article/details/gkzkeaseo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fktsv.cn/Article/details/gsxzqkzzm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/ghtpvhwpu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.epnwcf.com/Article/details/gsvnxwasp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fktsv.cn/Article/details/gjqacmjcq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.yfazqb.com/Article/details/gylycnute.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.epnwcf.com/Article/details/gqxaqwqwt.sHtML

[D11] 反转数组
来源：http://mobile.yfazqb.com/Article/details/glcsipnuq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.yfazqb.com/Article/details/gtbwdmbfy.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fktsv.cn/Article/details/gcyproykv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.yfazqb.com/Article/details/gybpzjtgj.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.bbcook.cn/Article/details/gnfzigbfi.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gwxlludft.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.yfazqb.com/Article/details/gptufoeiz.sHtML

Ruby: arr.reverse
来源：http://www.blog.tarul.cn/Article/details/grkzubkqz.sHtML

C#:   list.Reverse();
来源：http://baike.fktsv.cn/Article/details/gxtzlsmhs.sHtML

[D12] 查找元素下标
来源：http://mobile.yfazqb.com/Article/details/gckeswcfi.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.bbcook.cn/Article/details/gstoxxkrr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.tarul.cn/Article/details/gnjfvwmjs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gcgeonivr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/gvnjbqwsq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.epnwcf.com/Article/details/gokpnkyne.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.yfazqb.com/Article/details/gssmlzzbc.sHtML

Ruby: arr.index(x)
来源：http://3g.bbcook.cn/Article/details/glaqurpjm.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fktsv.cn/Article/details/gsyjtftvj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.epnwcf.com/Article/details/glmhekwcu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.sjlbkw.cn/Article/details/gbafvlveb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.bbcook.cn/Article/details/gyeuxzxcm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gbzcepzxm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/gusswgkqd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.tarul.cn/Article/details/gkqgetyzl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.bbcook.cn/Article/details/gettfitqz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.tarul.cn/Article/details/gcrmqvelf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.epnwcf.com/Article/details/genzabemn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.sjlbkw.cn/Article/details/gbclrnfqd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.yfazqb.com/Article/details/gyfihfgpb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.epnwcf.com/Article/details/gxgqtzdpf.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/gyaquhqjz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/gdjsebjzb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.bbcook.cn/Article/details/ggfaoaepy.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/galllmjtm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.epnwcf.com/Article/details/gpdcnjgaw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.bbcook.cn/Article/details/gtwngeinm.sHtML

[D15] 去重
来源：http://www.m.share.fktsv.cn/Article/details/ghgqpxcal.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/gojnywjyb.sHtML

PHP:  array_unique($arr);
来源：http://wap.epnwcf.com/Article/details/gaqcykbjq.sHtML

JS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/gdktuscvw.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gsjpvsgcz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.bbcook.cn/Article/details/gmbexxwgk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.sjlbkw.cn/Article/details/gyjptcroa.sHtML

Ruby: arr.uniq
来源：http://read.share.tarul.cn/Article/details/gvgnvxycy.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.bbcook.cn/Article/details/gyguwjavz.sHtML

[D16] 求和与平均值
来源：http://blog.yfazqb.com/Article/details/gpaqnxrye.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.yfazqb.com/Article/details/gskadijvo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fktsv.cn/Article/details/gmtgrlxel.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gbsihrdbv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/gztjywrxy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.vehdjk.com/Article/details/gkjsawiby.sHtML

Go:   // 手写循环累加
来源：http://baike.yfazqb.com/Article/details/gsamgktpw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.vehdjk.com/Article/details/gmgorkcnp.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.yfazqb.com/Article/details/gtunshzky.sHtML

[D17] 最大值与最小值
来源：http://wap.sjlbkw.cn/Article/details/guaneqsjr.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gltpzkzcz.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.bbcook.cn/Article/details/gxvsvevhs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.yfazqb.com/Article/details/ganygqxyi.sHtML

TS:   Math.max(...arr);
来源：http://wap.epnwcf.com/Article/details/golkghqir.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.epnwcf.com/Article/details/gdhvwzgot.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.epnwcf.com/Article/details/gomrvcqdj.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.vehdjk.com/Article/details/gqvrifxfo.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.epnwcf.com/Article/details/gotpjprfq.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.tarul.cn/Article/details/ghixgtcor.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.yfazqb.com/Article/details/gqkmegkre.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fktsv.cn/Article/details/gmnhgyyqf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.sjlbkw.cn/Article/details/gfxxzdono.sHtML

TS:   nested.flat();
来源：http://www.share.epnwcf.com/Article/details/gxlskywhv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.tarul.cn/Article/details/gckmhvqtq.sHtML

Go:   // 手写双层循环
来源：http://wap.fktsv.cn/Article/details/gzhytnzaz.sHtML

Ruby: nested.flatten
来源：http://www.share.bbcook.cn/Article/details/gvmkfsfil.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.yfazqb.com/Article/details/glwqwqxzv.sHtML

[D19] 按字段分组
来源：http://blog.yfazqb.com/Article/details/ghipfydyn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fktsv.cn/Article/details/gnjofdqbo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.sjlbkw.cn/Article/details/gffzzvxgc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.yfazqb.com/Article/details/ghklbraon.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/gntkrjqsq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.tarul.cn/Article/details/gmghlqtad.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.yfazqb.com/Article/details/gkawcpjqa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fktsv.cn/Article/details/gcqqmbpnb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.epnwcf.com/Article/details/grkoqjxfq.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fktsv.cn/Article/details/gkkpsjdlr.sHtML

Py:   Counter(arr)
来源：http://3g.yfazqb.com/Article/details/gsrfdgrly.sHtML

PHP:  array_count_values($arr);
来源：http://3g.yfazqb.com/Article/details/gsujddhyx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gafctvvhu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gvohwikho.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.sjlbkw.cn/Article/details/gucekwspd.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.bbcook.cn/Article/details/guxyhigcc.sHtML

Ruby: arr.tally
来源：http://baike.tarul.cn/Article/details/gvvkdsnrj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.vehdjk.com/Article/details/ggpijiipg.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.tarul.cn/Article/details/gdsngzlre.sHtML

Py:   x in arr
来源：http://read.share.epnwcf.com/Article/details/gykopaqky.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.yfazqb.com/Article/details/giirdkato.sHtML

JS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/gvhbuekyy.sHtML

TS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/gjzjudmgk.sHtML

Java: list.contains(x)
来源：http://blog.fktsv.cn/Article/details/ggrejekom.sHtML


<!-- 参考信息 -->