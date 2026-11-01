代发 wailian999

Py:   return a, b
来源：http://www.blog.yfazqb.com/Article/details/gsqbruogc.sHtML

PHP:  return [$a, $b];
来源：http://baike.fktsv.cn/Article/details/gawgrokfb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.vehdjk.com/Article/details/gbrygrgmt.sHtML

TS:   return { a, b };
来源：http://baike.vehdjk.com/Article/details/gbkldgwmh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.tarul.cn/Article/details/gicjkvgbb.sHtML

Go:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/guysoxwmc.sHtML

Ruby: return a, b
来源：http://3g.epnwcf.com/Article/details/gsrutxcof.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.sjlbkw.cn/Article/details/gwykdcrwj.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.tarul.cn/Article/details/gejmtdyzb.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.sjlbkw.cn/Article/details/gzssgvkxn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.bbcook.cn/Article/details/ginpqesek.sHtML

JS:   const square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/gbsvbcxmk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gfrqumpfz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.vehdjk.com/Article/details/giqftwbje.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.epnwcf.com/Article/details/gwhclnwie.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.vehdjk.com/Article/details/gyxelerfa.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fktsv.cn/Article/details/gjonbysxh.sHtML

[C07] 把函数作为参数传入
来源：http://3g.sjlbkw.cn/Article/details/ggajbtage.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.vehdjk.com/Article/details/ggjltakwy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.bbcook.cn/Article/details/gsnbnydpe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.epnwcf.com/Article/details/gxksglhhq.sHtML

TS:   arr.map(String)
来源：http://baike.tarul.cn/Article/details/guzdpgqmd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gkuyzknww.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fktsv.cn/Article/details/gkgzwgisj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fktsv.cn/Article/details/gvqkcrdck.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.bbcook.cn/Article/details/gselvnayg.sHtML

[C08] 闭包
来源：http://www.m.share.fktsv.cn/Article/details/gmewsqnmm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fktsv.cn/Article/details/gehgwjrps.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.sjlbkw.cn/Article/details/gfdzfkiap.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/gydkqgzgw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/gexcznosy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/gwijauthl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.epnwcf.com/Article/details/gzkamuodx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.tarul.cn/Article/details/gntvuznhe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gdzwatmxu.sHtML

[C09] 递归
来源：http://m.share.sjlbkw.cn/Article/details/gidoqlkws.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/gesoxndsj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.yfazqb.com/Article/details/gtsrjvugh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/guukppwya.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/gspxqdhyd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/gkizufdaq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.yfazqb.com/Article/details/gegzaghiw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.bbcook.cn/Article/details/gujwyrpqd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.yfazqb.com/Article/details/gnkrxntmi.sHtML

[C10] 变量作用域
来源：http://www.blog.tarul.cn/Article/details/gjoyxghwy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.vehdjk.com/Article/details/gewfxnjfw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.bbcook.cn/Article/details/guwxfuayk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gkaogesoy.sHtML

TS:   同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gkdrtomix.sHtML

Java: 方法内为块级作用域
来源：http://m.share.epnwcf.com/Article/details/grotcifzk.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gafextzae.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fktsv.cn/Article/details/gdvvfbikt.sHtML

C#:   块级作用域
来源：http://www.share.fktsv.cn/Article/details/gukogxwqt.sHtML

[C11] 模块导入与导出
来源：http://www.share.sjlbkw.cn/Article/details/gijkjfuvq.sHtML

Py:   from module import func
来源：http://mobile.yfazqb.com/Article/details/gcgpolzlj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.bbcook.cn/Article/details/gilwqtjga.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.yfazqb.com/Article/details/gamlcmsac.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fktsv.cn/Article/details/gfctuqzgd.sHtML

Java: import java.util.List;
来源：http://blog.bbcook.cn/Article/details/gketihxak.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.bbcook.cn/Article/details/gqzvennrr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.epnwcf.com/Article/details/gsobpcqdg.sHtML

C#:   using System.Text;
来源：http://www.blog.fktsv.cn/Article/details/glkogwtqk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.sjlbkw.cn/Article/details/gemqgtrqp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.bbcook.cn/Article/details/gedpblekc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fktsv.cn/Article/details/gmxinxpfr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.bbcook.cn/Article/details/gslvjqtdw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gkjwlztux.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fktsv.cn/Article/details/ghbwiphsq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.epnwcf.com/Article/details/gqutusikl.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.vehdjk.com/Article/details/gjaqhdhdf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.epnwcf.com/Article/details/gsninaape.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.tarul.cn/Article/details/gmsmgpibt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.vehdjk.com/Article/details/gloxhfsdl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gxfoavqln.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fktsv.cn/Article/details/gebrneeoz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.yfazqb.com/Article/details/ggnkvxbll.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gjllszlpy.sHtML

Go:   func add(a, b int) int
来源：http://wap.vehdjk.com/Article/details/gwrpxpift.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.bbcook.cn/Article/details/gnlodvlko.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.epnwcf.com/Article/details/gotdtelzq.sHtML

[C14] 泛型函数
来源：http://www.m.share.fktsv.cn/Article/details/gdpwoivlc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.bbcook.cn/Article/details/ggcigjdoa.sHtML

PHP:  // 无泛型
来源：http://www.blog.vehdjk.com/Article/details/gaksjvssx.sHtML

JS:   // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gezyomvmh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.bbcook.cn/Article/details/gfwshopap.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.bbcook.cn/Article/details/gsddagoud.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.bbcook.cn/Article/details/gxcoapxve.sHtML

Ruby: # 无泛型
来源：http://blog.yfazqb.com/Article/details/gebuekkam.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.tarul.cn/Article/details/gwgcwxxvi.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.yfazqb.com/Article/details/gpvlcbycu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.sjlbkw.cn/Article/details/ghkknwbux.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.vehdjk.com/Article/details/gglzbwzwl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gqqhnfygl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.sjlbkw.cn/Article/details/gvmhwstar.sHtML

Java: // 无解构
来源：http://wap.vehdjk.com/Article/details/gbnffvvrn.sHtML

Go:   // 无解构
来源：http://m.share.bbcook.cn/Article/details/gxgxbwdxh.sHtML

Ruby: a, b = pair
来源：http://www.blog.tarul.cn/Article/details/giurdpxtz.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.bbcook.cn/Article/details/gulqbqpjr.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.yfazqb.com/Article/details/gbgcedtzu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.yfazqb.com/Article/details/gtsadersd.sHtML

PHP:  // 无重载
来源：http://blog.sjlbkw.cn/Article/details/gxajdkpux.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.tarul.cn/Article/details/gcofigipk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/ghteyrizu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fktsv.cn/Article/details/gaqdmzxcd.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fktsv.cn/Article/details/gpcoebmfj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.bbcook.cn/Article/details/ggugockzj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.bbcook.cn/Article/details/gzpbeaehc.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ggwinusvs.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.tarul.cn/Article/details/gsclokqhb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gwdhanaiq.sHtML

[D01] 创建数组 / 列表
来源：http://3g.bbcook.cn/Article/details/gjwpiqvir.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.epnwcf.com/Article/details/gznssjolf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.sjlbkw.cn/Article/details/gaiphitze.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.tarul.cn/Article/details/gdzvrmmdu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.yfazqb.com/Article/details/gcggzfeio.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.tarul.cn/Article/details/gmahaqjhn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fktsv.cn/Article/details/gzpbszeue.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.tarul.cn/Article/details/gtgreklpb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.sjlbkw.cn/Article/details/gaajicumy.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fktsv.cn/Article/details/grohmgtab.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.vehdjk.com/Article/details/gsqupoykh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fktsv.cn/Article/details/gbwztpqyk.sHtML

JS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/gzcfkurgq.sHtML

TS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/grswqkbgm.sHtML

Java: list.add(4);
来源：http://www.blog.vehdjk.com/Article/details/glevtmftj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fktsv.cn/Article/details/gzxznrqtm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.vehdjk.com/Article/details/grbwykuir.sHtML

C#:   list.Add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gqkraapst.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fktsv.cn/Article/details/gzbmwvdof.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.tarul.cn/Article/details/ggwfdplbx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.yfazqb.com/Article/details/gtfthlxwq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.sjlbkw.cn/Article/details/grcozjkbg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.epnwcf.com/Article/details/gdfqqmjho.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gvvydhfqt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.epnwcf.com/Article/details/gvepxolri.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.yfazqb.com/Article/details/gfpmgpvef.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/ggjczhdcr.sHtML

[D04] 删除元素
来源：http://www.blog.vehdjk.com/Article/details/grgnqcymu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.epnwcf.com/Article/details/gwjgplbin.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/gmcgszvze.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.vehdjk.com/Article/details/gixnzvval.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.vehdjk.com/Article/details/ghlhbidng.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.epnwcf.com/Article/details/gfbzaemas.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.vehdjk.com/Article/details/ghtrghtsg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/gbjboebid.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fktsv.cn/Article/details/gljwwuaxg.sHtML

[D05] 访问与修改元素
来源：http://www.blog.vehdjk.com/Article/details/gesvkibeo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gwcetjnsu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gjcxtfpfc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/guwgwmdkc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.bbcook.cn/Article/details/gpupjhgfy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fktsv.cn/Article/details/gvxgzbsnx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfmepvwy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gnnlsrkjx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.vehdjk.com/Article/details/glizbosbf.sHtML

[D06] 数组长度
来源：http://www.share.tarul.cn/Article/details/gkkgnfxja.sHtML

Py:   len(arr)
来源：http://blog.bbcook.cn/Article/details/gbuxmbceh.sHtML

PHP:  count($arr);
来源：http://baike.sjlbkw.cn/Article/details/groehnvps.sHtML

JS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/gvxobjvus.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gvkbwryff.sHtML

Java: list.size();
来源：http://www.share.yfazqb.com/Article/details/gdkzxufti.sHtML

Go:   len(arr)
来源：http://wap.bbcook.cn/Article/details/gbdxgogek.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.vehdjk.com/Article/details/gckdittno.sHtML

C#:   list.Count;
来源：http://mobile.yfazqb.com/Article/details/gevsjgbtn.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.epnwcf.com/Article/details/gqqwawkbk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.yfazqb.com/Article/details/gfvndhrzy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.epnwcf.com/Article/details/gnuhdeeki.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gygzvjnod.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fktsv.cn/Article/details/gjsegneko.sHtML

Java: list.subList(1, 4);
来源：http://wap.bbcook.cn/Article/details/gydawofwv.sHtML

Go:   arr[1:4]
来源：http://baike.bbcook.cn/Article/details/gcbzvxcyw.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fktsv.cn/Article/details/gdkaemkfx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.bbcook.cn/Article/details/gjjdlbjim.sHtML

[D08] 合并两个数组
来源：http://www.blog.epnwcf.com/Article/details/gwqxhbnea.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.sjlbkw.cn/Article/details/geddreiav.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.vehdjk.com/Article/details/gheuxhdpp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.yfazqb.com/Article/details/gshprjfzn.sHtML

TS:   [...a, ...b];
来源：http://www.share.bbcook.cn/Article/details/guhvpohky.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.epnwcf.com/Article/details/gyvelsufl.sHtML

Go:   append(a, b...)
来源：http://3g.epnwcf.com/Article/details/gizgxnrla.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.epnwcf.com/Article/details/geqaochbu.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.epnwcf.com/Article/details/gpuktkesd.sHtML

[D09] 排序（升序）
来源：http://read.share.fktsv.cn/Article/details/ggbzyoqdg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.bbcook.cn/Article/details/gqafwtxgp.sHtML

PHP:  sort($arr);
来源：http://wap.vehdjk.com/Article/details/gylaztjbe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.tarul.cn/Article/details/gtuezbmyy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gfqnwfhws.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.yfazqb.com/Article/details/gogeyabgv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gymlfydnc.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gvansvndx.sHtML

C#:   list.Sort();
来源：http://read.share.bbcook.cn/Article/details/gnfbfgion.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.vehdjk.com/Article/details/glqdxikaf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fktsv.cn/Article/details/gqedlgoix.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fktsv.cn/Article/details/gxpzitmnk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gowmnvyfr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.tarul.cn/Article/details/gfvumzlix.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.epnwcf.com/Article/details/ggxnbloyc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.yfazqb.com/Article/details/glvwxbnah.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.bbcook.cn/Article/details/gkdovlosj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.vehdjk.com/Article/details/gdtzyvpvx.sHtML

[D11] 反转数组
来源：http://mobile.tarul.cn/Article/details/gskioelex.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fktsv.cn/Article/details/glhmqsriw.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.yfazqb.com/Article/details/glfykxnzx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.epnwcf.com/Article/details/gwxfqsqbi.sHtML

TS:   [...arr].reverse();
来源：http://baike.sjlbkw.cn/Article/details/ghhoeajxm.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.vehdjk.com/Article/details/geavwjdqt.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.bbcook.cn/Article/details/gvqghsddp.sHtML

Ruby: arr.reverse
来源：http://wap.yfazqb.com/Article/details/gmmqecmlr.sHtML

C#:   list.Reverse();
来源：http://www.m.share.epnwcf.com/Article/details/gpeotgnxm.sHtML

[D12] 查找元素下标
来源：http://m.share.sjlbkw.cn/Article/details/gtifvzluz.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.sjlbkw.cn/Article/details/ghahwwlaf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fktsv.cn/Article/details/gbavotmla.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/ghanrwwtc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gurvggfoy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.vehdjk.com/Article/details/gwvtbmfnc.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.tarul.cn/Article/details/gjpdvkoeg.sHtML

Ruby: arr.index(x)
来源：http://www.share.fktsv.cn/Article/details/gzgaxmkff.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.yfazqb.com/Article/details/gxwfkhwdg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.epnwcf.com/Article/details/gshgbfswj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.bbcook.cn/Article/details/gtryseqgx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fktsv.cn/Article/details/gyibsxkxr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.vehdjk.com/Article/details/gtetiaink.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gxajmkrtx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gioapbgod.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.yfazqb.com/Article/details/ggxvmyrtk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.tarul.cn/Article/details/gbziuldqv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gjvffitgv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.yfazqb.com/Article/details/gmtorhrda.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.bbcook.cn/Article/details/gkynlmuhl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.sjlbkw.cn/Article/details/gcfbbwfqn.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/gvqjfopch.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.yfazqb.com/Article/details/gxacdivwn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.bbcook.cn/Article/details/gsehtqufg.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/gzrhzpfdt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpphbakrv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.bbcook.cn/Article/details/ggtidbxkv.sHtML

[D15] 去重
来源：http://3g.sjlbkw.cn/Article/details/gtdzgagfb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.tarul.cn/Article/details/gygjzcrzn.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.tarul.cn/Article/details/gzrgprhjx.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gfhodzxao.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/geowdgtnw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.tarul.cn/Article/details/gqamzqbck.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.epnwcf.com/Article/details/gqdmkbqdt.sHtML

Ruby: arr.uniq
来源：http://www.m.share.tarul.cn/Article/details/gsdqotxci.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.epnwcf.com/Article/details/gsjlobphi.sHtML

[D16] 求和与平均值
来源：http://www.m.share.tarul.cn/Article/details/gmkudvxgw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.sjlbkw.cn/Article/details/ggamonzuo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.vehdjk.com/Article/details/gbtypfgdp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/gitnsvpep.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gnskzycht.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.sjlbkw.cn/Article/details/gjvoogspb.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.tarul.cn/Article/details/ghalmvbml.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.tarul.cn/Article/details/gzeeizwuk.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.sjlbkw.cn/Article/details/gcnnmzpqy.sHtML

[D17] 最大值与最小值
来源：http://read.share.yfazqb.com/Article/details/gqfwztonj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gtlkfhnfe.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/grwtxiovo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.bbcook.cn/Article/details/gngfnuzql.sHtML

TS:   Math.max(...arr);
来源：http://baike.epnwcf.com/Article/details/gehsdvuld.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fktsv.cn/Article/details/gnyhebmlv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gajhdoyka.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.epnwcf.com/Article/details/gcvrvtlql.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/gvfhqjoxx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.yfazqb.com/Article/details/gdvrjydfz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.epnwcf.com/Article/details/gvgfequlx.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.bbcook.cn/Article/details/gifdcgwjs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.vehdjk.com/Article/details/gcsgtsgae.sHtML

TS:   nested.flat();
来源：http://www.m.share.fktsv.cn/Article/details/giteqhoha.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.tarul.cn/Article/details/govxjhntm.sHtML

Go:   // 手写双层循环
来源：http://mobile.tarul.cn/Article/details/gbdnoxuis.sHtML

Ruby: nested.flatten
来源：http://www.share.bbcook.cn/Article/details/gzuddcmjj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.tarul.cn/Article/details/gzmcakzkt.sHtML

[D19] 按字段分组
来源：http://www.m.share.epnwcf.com/Article/details/gemynhbrq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.bbcook.cn/Article/details/gdwvofkco.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.sjlbkw.cn/Article/details/gijpkjoky.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.tarul.cn/Article/details/ggzdacaee.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.bbcook.cn/Article/details/gwjzkvqqv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.bbcook.cn/Article/details/ggtybzrte.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.bbcook.cn/Article/details/gveezpkqp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fktsv.cn/Article/details/gnreyrznz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.vehdjk.com/Article/details/gdiijqjod.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.yfazqb.com/Article/details/ghxipvjvg.sHtML

Py:   Counter(arr)
来源：http://www.blog.fktsv.cn/Article/details/gyhkcnvga.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.yfazqb.com/Article/details/gomdjijys.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.vehdjk.com/Article/details/gdscefavm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.bbcook.cn/Article/details/grdusuhpv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.tarul.cn/Article/details/getqdqmem.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fktsv.cn/Article/details/gvxkxsopa.sHtML

Ruby: arr.tally
来源：http://m.share.bbcook.cn/Article/details/gfefqgcwf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/gbcfeumba.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.bbcook.cn/Article/details/gugfmbudk.sHtML

Py:   x in arr
来源：http://www.share.bbcook.cn/Article/details/gnyfozfbz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.tarul.cn/Article/details/gmjwjloau.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmkqzdyf.sHtML

TS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gfqxvwfqw.sHtML

Java: list.contains(x)
来源：http://m.share.bbcook.cn/Article/details/gbdxlttrw.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fktsv.cn/Article/details/ghwxdwknj.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/gspnolfpd.sHtML

C#:   list.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gjpncsore.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.sjlbkw.cn/Article/details/gwrdtzvwh.sHtML


<!-- 参考信息 -->