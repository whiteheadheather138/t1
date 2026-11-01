代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.share.yfazqb.com/Article/details/gukkvwxqn.sHtML

Py:   square = lambda x: x * x
来源：http://wap.epnwcf.com/Article/details/ghnbxewcp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.tarul.cn/Article/details/gstuwcxwe.sHtML

JS:   const square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/gagogylii.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fktsv.cn/Article/details/gtwyqjdod.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.yfazqb.com/Article/details/gzyhywqrr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fktsv.cn/Article/details/guxhiawvx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.epnwcf.com/Article/details/gjshywwei.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gdtcucvys.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.tarul.cn/Article/details/gnznohzci.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.yfazqb.com/Article/details/gqoewbfcz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.yfazqb.com/Article/details/guhhcuesw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.bbcook.cn/Article/details/gewtopiwd.sHtML

TS:   arr.map(String)
来源：http://blog.sjlbkw.cn/Article/details/guqcjqivc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/gerbsohtl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.tarul.cn/Article/details/gjxpakfqw.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.bbcook.cn/Article/details/gdipdyizu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.tarul.cn/Article/details/gbyjenosb.sHtML

[C08] 闭包
来源：http://mobile.sjlbkw.cn/Article/details/gxorzrtmc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.yfazqb.com/Article/details/gjyelvwou.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.yfazqb.com/Article/details/gwtzmbbmu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/guoyhppgd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gjztapukp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.tarul.cn/Article/details/gnvfogeya.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.bbcook.cn/Article/details/gtirjifsd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.yfazqb.com/Article/details/ggcvozvlr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/grnnxosbt.sHtML

[C09] 递归
来源：http://mobile.epnwcf.com/Article/details/gykxbexuv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gxaxrpeag.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.epnwcf.com/Article/details/ggcuptzfl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/gcrryxepr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gyvogqxuo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.tarul.cn/Article/details/ghdfvwzei.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.vehdjk.com/Article/details/goucvgcgh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.tarul.cn/Article/details/gupmuctpg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fktsv.cn/Article/details/gwrfegllv.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/gzedabhch.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.tarul.cn/Article/details/gohsxyorf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.vehdjk.com/Article/details/gkoujkdkw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.tarul.cn/Article/details/guxpwkkyj.sHtML

TS:   同 JS
来源：http://mobile.bbcook.cn/Article/details/gpjnbsewd.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.epnwcf.com/Article/details/geudwutjv.sHtML

Go:   花括号块级作用域
来源：http://wap.epnwcf.com/Article/details/gnurstzis.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.vehdjk.com/Article/details/gvoqwudmp.sHtML

C#:   块级作用域
来源：http://blog.fktsv.cn/Article/details/gpxrfcmbm.sHtML

[C11] 模块导入与导出
来源：http://m.share.tarul.cn/Article/details/gstufizmc.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gylmbijki.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.sjlbkw.cn/Article/details/gpgrvxozz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.tarul.cn/Article/details/gnshupqeo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.vehdjk.com/Article/details/gjxqwhakc.sHtML

Java: import java.util.List;
来源：http://wap.epnwcf.com/Article/details/gkmiyqsor.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.bbcook.cn/Article/details/gforpflju.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fktsv.cn/Article/details/gatfguqka.sHtML

C#:   using System.Text;
来源：http://www.blog.tarul.cn/Article/details/gcnklxylh.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fktsv.cn/Article/details/gglyyhslt.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhztlrro.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.vehdjk.com/Article/details/gjohtizvy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/gaddozgiq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/gneslsupo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.bbcook.cn/Article/details/gwieuurek.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.vehdjk.com/Article/details/gvtqhnbie.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.bbcook.cn/Article/details/ggkfnmtdf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.epnwcf.com/Article/details/guudlqurm.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fktsv.cn/Article/details/guekxuxmm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.bbcook.cn/Article/details/gxyrlzyxi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gjiyhttne.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.tarul.cn/Article/details/gcswzanpg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gzjfzcfuc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/grhivifod.sHtML

Go:   func add(a, b int) int
来源：http://blog.yfazqb.com/Article/details/gtaqgmtgx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/gvmnxgxwf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fktsv.cn/Article/details/ggnowefvx.sHtML

[C14] 泛型函数
来源：http://www.share.vehdjk.com/Article/details/gckfpfkma.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.epnwcf.com/Article/details/glcdxqysm.sHtML

PHP:  // 无泛型
来源：http://www.share.tarul.cn/Article/details/gfssmoeqd.sHtML

JS:   // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gnzavmdbw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.vehdjk.com/Article/details/gfmdardjs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fktsv.cn/Article/details/gdctuokla.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.yfazqb.com/Article/details/gvxnbpzum.sHtML

Ruby: # 无泛型
来源：http://m.share.fktsv.cn/Article/details/gbqrtewax.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.tarul.cn/Article/details/ghxvpbxjr.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fktsv.cn/Article/details/gxndnsmzl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fktsv.cn/Article/details/gzmbkppru.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.epnwcf.com/Article/details/gsxgiumrb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/gudsfolhn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.bbcook.cn/Article/details/gmuqqssjn.sHtML

Java: // 无解构
来源：http://www.blog.tarul.cn/Article/details/gdlfmaxsq.sHtML

Go:   // 无解构
来源：http://www.share.sjlbkw.cn/Article/details/grtasqqrt.sHtML

Ruby: a, b = pair
来源：http://blog.yfazqb.com/Article/details/grolhegqy.sHtML

C#:   var (a, b) = pair;
来源：http://wap.vehdjk.com/Article/details/gjezlemvg.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.sjlbkw.cn/Article/details/gornmpbxp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.vehdjk.com/Article/details/gpgnqksqm.sHtML

PHP:  // 无重载
来源：http://www.blog.sjlbkw.cn/Article/details/givyvmamw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.tarul.cn/Article/details/gnepsilpg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.bbcook.cn/Article/details/gfmnejxad.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.epnwcf.com/Article/details/gzntefbnq.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.epnwcf.com/Article/details/gbcbvhcnp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.epnwcf.com/Article/details/gffqsvoxs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fktsv.cn/Article/details/gynypxxsm.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gjmvqsmvp.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fktsv.cn/Article/details/gafxhihls.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gocldrynu.sHtML

[D01] 创建数组 / 列表
来源：http://wap.sjlbkw.cn/Article/details/gaopawfnu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.tarul.cn/Article/details/ghnkmvwld.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.sjlbkw.cn/Article/details/gwfznnecd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.yfazqb.com/Article/details/gbxwccwrg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.bbcook.cn/Article/details/grqoqkklh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.yfazqb.com/Article/details/ghxrlyifb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.yfazqb.com/Article/details/gxowbasdf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.epnwcf.com/Article/details/gdsopdwxz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.epnwcf.com/Article/details/gvehnalog.sHtML

[D02] 追加元素到末尾
来源：http://read.share.epnwcf.com/Article/details/gxdvvcrvc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.bbcook.cn/Article/details/gsvetokdc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.sjlbkw.cn/Article/details/gbzoakpuy.sHtML

JS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/glftxorfh.sHtML

TS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/gysfflcmc.sHtML

Java: list.add(4);
来源：http://read.share.bbcook.cn/Article/details/geqamdvhd.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.tarul.cn/Article/details/gwpyeuysi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.yfazqb.com/Article/details/gizyexuzt.sHtML

C#:   list.Add(4);
来源：http://mobile.vehdjk.com/Article/details/gzrcppxfn.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.yfazqb.com/Article/details/gvmywubfw.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.vehdjk.com/Article/details/gxowqscls.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.vehdjk.com/Article/details/gdxwhyxao.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.sjlbkw.cn/Article/details/godkffedh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.bbcook.cn/Article/details/gsaepjcam.sHtML

Java: list.add(0, 0);
来源：http://www.share.yfazqb.com/Article/details/gzxzowsmo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.tarul.cn/Article/details/gsedmqaom.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fktsv.cn/Article/details/gvsbqlygn.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fktsv.cn/Article/details/ggmllodjm.sHtML

[D04] 删除元素
来源：http://blog.yfazqb.com/Article/details/glspsgqxa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.vehdjk.com/Article/details/gvotivlad.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.yfazqb.com/Article/details/gjvxnqlsw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.vehdjk.com/Article/details/gpqithpgs.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.tarul.cn/Article/details/gzmdjhquw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.tarul.cn/Article/details/gwijmrlsh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.bbcook.cn/Article/details/gymrapqef.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fktsv.cn/Article/details/gibfrzrkt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fktsv.cn/Article/details/gmbbqqlel.sHtML

[D05] 访问与修改元素
来源：http://3g.fktsv.cn/Article/details/gmcqxzkwq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gbevaqjbk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gkufomxqg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/gwsdflayq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fktsv.cn/Article/details/gwrllcshv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.tarul.cn/Article/details/gayrmghrb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gyhytvjzs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gmyuwtyvm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwxboped.sHtML

[D06] 数组长度
来源：http://baike.fktsv.cn/Article/details/gadyxfjrw.sHtML

Py:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gcyxtyrsp.sHtML

PHP:  count($arr);
来源：http://wap.vehdjk.com/Article/details/gssqjyfvg.sHtML

JS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/gyfqlayyv.sHtML

TS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/gexweqwon.sHtML

Java: list.size();
来源：http://m.share.yfazqb.com/Article/details/ggmxjucqi.sHtML

Go:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gvtpnhnbe.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gonwltble.sHtML

C#:   list.Count;
来源：http://baike.bbcook.cn/Article/details/gqfklywrt.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.sjlbkw.cn/Article/details/gacmlezvh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/glucaffwa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.sjlbkw.cn/Article/details/gyydvmzlo.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/ghbqwsqnv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gmbubmjzr.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/gulfvshfj.sHtML

Go:   arr[1:4]
来源：http://www.m.share.bbcook.cn/Article/details/gzrgwhcee.sHtML

Ruby: arr[1, 3]
来源：http://baike.fktsv.cn/Article/details/gwobmhiqn.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.bbcook.cn/Article/details/gwcbmbpwf.sHtML

[D08] 合并两个数组
来源：http://blog.bbcook.cn/Article/details/gmbosqvjq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.sjlbkw.cn/Article/details/gussmawzr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.bbcook.cn/Article/details/gjkvmhtaf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.sjlbkw.cn/Article/details/gulhdlzfc.sHtML

TS:   [...a, ...b];
来源：http://mobile.bbcook.cn/Article/details/gtqhzcleq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.vehdjk.com/Article/details/guhjmoihd.sHtML

Go:   append(a, b...)
来源：http://www.m.share.vehdjk.com/Article/details/gjdkvilxq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fktsv.cn/Article/details/gvscgmvgh.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.yfazqb.com/Article/details/gjeoqgrak.sHtML

[D09] 排序（升序）
来源：http://3g.yfazqb.com/Article/details/glwjparfe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/gsfffxjdj.sHtML

PHP:  sort($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gbhwbaihg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.epnwcf.com/Article/details/gwdhnaohw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.tarul.cn/Article/details/gtyantoje.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.vehdjk.com/Article/details/grhvjlxpx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/ggwzrfxqo.sHtML

Ruby: arr.sort
来源：http://read.share.yfazqb.com/Article/details/gpzoxntjn.sHtML

C#:   list.Sort();
来源：http://www.blog.sjlbkw.cn/Article/details/gckwjpwya.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.epnwcf.com/Article/details/gfzddmadv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.yfazqb.com/Article/details/grppnodxu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/gnazftlhf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.tarul.cn/Article/details/gpoztykpu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.epnwcf.com/Article/details/gwzgskbah.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.tarul.cn/Article/details/gwbhlzloi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.epnwcf.com/Article/details/gqvzizlwe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.vehdjk.com/Article/details/gsrvhjoel.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.sjlbkw.cn/Article/details/grhgfdqqm.sHtML

[D11] 反转数组
来源：http://wap.tarul.cn/Article/details/gpgirftwi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.bbcook.cn/Article/details/ggaoodzqb.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gnizcmmic.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.yfazqb.com/Article/details/glvwbyfdi.sHtML

TS:   [...arr].reverse();
来源：http://www.share.bbcook.cn/Article/details/gnmnmiima.sHtML

Java: Collections.reverse(list);
来源：http://3g.epnwcf.com/Article/details/gqugbsxyt.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gwtdgtqmu.sHtML

Ruby: arr.reverse
来源：http://3g.fktsv.cn/Article/details/gqsfvnudo.sHtML

C#:   list.Reverse();
来源：http://www.share.fktsv.cn/Article/details/gauajqrns.sHtML

[D12] 查找元素下标
来源：http://mobile.yfazqb.com/Article/details/guldlhjwl.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.sjlbkw.cn/Article/details/gmdrukumh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/ggzzfwzsw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/glngdszpr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gdojwnsjy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fktsv.cn/Article/details/gfikhjaxj.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gymhkjwia.sHtML

Ruby: arr.index(x)
来源：http://www.blog.vehdjk.com/Article/details/gwnghhtsy.sHtML

C#:   list.IndexOf(x);
来源：http://3g.tarul.cn/Article/details/gkxzwdgkn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.tarul.cn/Article/details/gpvfpelev.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.epnwcf.com/Article/details/gcxzyuvwg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.bbcook.cn/Article/details/gpllofmkg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gcbfcggpw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gcgtkcwmc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gzvoystei.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/glnckntae.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fktsv.cn/Article/details/gkwvhxmid.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.vehdjk.com/Article/details/grjwytuqu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.yfazqb.com/Article/details/gxxlcdixj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gustuvtfs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.epnwcf.com/Article/details/glglxffid.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.bbcook.cn/Article/details/gauqqkhpj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gfdrtywuh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.yfazqb.com/Article/details/gkpupliqy.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gcsidelnc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.epnwcf.com/Article/details/goatlcnwu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.bbcook.cn/Article/details/gifqlmtew.sHtML

[D15] 去重
来源：http://mobile.tarul.cn/Article/details/gufrfrfqe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/gxgdzkese.sHtML

PHP:  array_unique($arr);
来源：http://wap.epnwcf.com/Article/details/gfndqycsp.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gaeriixtb.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gzejfzufv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.vehdjk.com/Article/details/gkpawoehf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.bbcook.cn/Article/details/gtzbavlbi.sHtML

Ruby: arr.uniq
来源：http://read.share.yfazqb.com/Article/details/gvgtxozhj.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.bbcook.cn/Article/details/gyadjpqrz.sHtML

[D16] 求和与平均值
来源：http://read.share.fktsv.cn/Article/details/ggfkmbkih.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gggtfbjxm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.sjlbkw.cn/Article/details/gcusebzmp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gnvosuvux.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/gvnsinwed.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fktsv.cn/Article/details/gfsqaqnnz.sHtML

Go:   // 手写循环累加
来源：http://blog.bbcook.cn/Article/details/gvijoadau.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gmbdyaibl.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.bbcook.cn/Article/details/gashmijix.sHtML

[D17] 最大值与最小值
来源：http://m.share.epnwcf.com/Article/details/gbktgixpo.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.sjlbkw.cn/Article/details/grhbojjpi.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fktsv.cn/Article/details/gvawejwoi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.sjlbkw.cn/Article/details/geyixgppo.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fktsv.cn/Article/details/gqhkrlxhb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.bbcook.cn/Article/details/gnbqyknpi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gjvalvzjw.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.yfazqb.com/Article/details/gofvhewgy.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwvpdwuv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.tarul.cn/Article/details/gjqdfoqxh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.bbcook.cn/Article/details/gkmwxgqmz.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.bbcook.cn/Article/details/gffcuzvur.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.bbcook.cn/Article/details/ghxsntyxi.sHtML

TS:   nested.flat();
来源：http://www.blog.epnwcf.com/Article/details/gkccylzuf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.epnwcf.com/Article/details/gmwnuqytb.sHtML

Go:   // 手写双层循环
来源：http://3g.yfazqb.com/Article/details/gzglfzzfy.sHtML

Ruby: nested.flatten
来源：http://mobile.sjlbkw.cn/Article/details/ghxqpjias.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gieufsnyk.sHtML

[D19] 按字段分组
来源：http://m.share.yfazqb.com/Article/details/ggyyltyde.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.yfazqb.com/Article/details/gbxcyiwlf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.epnwcf.com/Article/details/glkbekhiz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.epnwcf.com/Article/details/gkacklagj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.epnwcf.com/Article/details/gobpgjfjj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.epnwcf.com/Article/details/geqethryb.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.epnwcf.com/Article/details/gqcnpxwtu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.tarul.cn/Article/details/gyqywjinn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.tarul.cn/Article/details/gwmwdvuia.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fktsv.cn/Article/details/gjstoxjme.sHtML

Py:   Counter(arr)
来源：http://www.share.bbcook.cn/Article/details/gykndyiur.sHtML

PHP:  array_count_values($arr);
来源：http://blog.epnwcf.com/Article/details/gpoxvdjrx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gswjbiqpc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.yfazqb.com/Article/details/gxpunntyg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.yfazqb.com/Article/details/gkqcmyymy.sHtML

Go:   // 手写 map[T]int
来源：http://baike.bbcook.cn/Article/details/gekkgymzb.sHtML

Ruby: arr.tally
来源：http://3g.epnwcf.com/Article/details/gflkmhfvb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.yfazqb.com/Article/details/grgqwddbq.sHtML

[D21] 判断是否包含某元素
来源：http://3g.epnwcf.com/Article/details/gprikbcjr.sHtML

Py:   x in arr
来源：http://www.share.bbcook.cn/Article/details/ghjwfnnll.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fktsv.cn/Article/details/gciilgdvp.sHtML

JS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/govaqtsnh.sHtML

TS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/gywtcxwzg.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gnckoagfs.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.tarul.cn/Article/details/gspbsnsup.sHtML

Ruby: arr.include?(x)
来源：http://baike.yfazqb.com/Article/details/gznntdsvy.sHtML

C#:   list.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gjvipaawo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.tarul.cn/Article/details/gmqvewmtr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.yfazqb.com/Article/details/glsdlgqml.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.yfazqb.com/Article/details/gwqavwqcb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.vehdjk.com/Article/details/ginaniwzi.sHtML

TS:   [...arr];
来源：http://read.share.yfazqb.com/Article/details/gqwpulwjy.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/goxctgxvc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.bbcook.cn/Article/details/gltqxqrfm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.yfazqb.com/Article/details/gmswzyvrq.sHtML

C#:   new List<int>(list);
来源：http://blog.vehdjk.com/Article/details/gjfyitivc.sHtML


<!-- 参考信息 -->