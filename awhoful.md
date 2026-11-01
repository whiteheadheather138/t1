代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.vehdjk.com/Article/details/gzsqytsey.sHtML

Go:   return a, b
来源：http://www.blog.tarul.cn/Article/details/gzsgtdyan.sHtML

Ruby: return a, b
来源：http://3g.fktsv.cn/Article/details/gsgsnecdx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.yfazqb.com/Article/details/gwzagzusk.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fktsv.cn/Article/details/gjhjvezsu.sHtML

Py:   square = lambda x: x * x
来源：http://blog.epnwcf.com/Article/details/gxqbdipdv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fktsv.cn/Article/details/gikalybzp.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gggystzkd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.bbcook.cn/Article/details/goiiivzmb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.sjlbkw.cn/Article/details/gwrgzxmyp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.vehdjk.com/Article/details/gnjlfbnbr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.epnwcf.com/Article/details/gmucjiaon.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fktsv.cn/Article/details/gawpmoifq.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.sjlbkw.cn/Article/details/gctcbutwf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.epnwcf.com/Article/details/gzjnjttrm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/grwxsgexh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.tarul.cn/Article/details/gnsdiwtdw.sHtML

TS:   arr.map(String)
来源：http://mobile.vehdjk.com/Article/details/gtgvuoztu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.bbcook.cn/Article/details/gkhzatrtu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.epnwcf.com/Article/details/gnatodemw.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.bbcook.cn/Article/details/gqrodxqev.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.sjlbkw.cn/Article/details/gnspnqcld.sHtML

[C08] 闭包
来源：http://wap.epnwcf.com/Article/details/ggrrhglcz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.epnwcf.com/Article/details/gplzogzca.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.tarul.cn/Article/details/gzevmkssb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/ggkjdxbbs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gdsoxkene.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.yfazqb.com/Article/details/gllegujii.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.bbcook.cn/Article/details/gqtrtdqfp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.bbcook.cn/Article/details/gpakjarji.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/gketxqxht.sHtML

[C09] 递归
来源：http://read.share.yfazqb.com/Article/details/grlmknldl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gbsymhfus.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/gnlqheyeg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.vehdjk.com/Article/details/godtwvdmj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gfwtoewef.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.yfazqb.com/Article/details/gwqcolgry.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.sjlbkw.cn/Article/details/gfrlnqsbv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gcytjglad.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.epnwcf.com/Article/details/gauagigin.sHtML

[C10] 变量作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gcfbaybmu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.yfazqb.com/Article/details/gxlsekoib.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.sjlbkw.cn/Article/details/gqdwjuabm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.sjlbkw.cn/Article/details/greeoembf.sHtML

TS:   同 JS
来源：http://www.blog.vehdjk.com/Article/details/gfsorgxmg.sHtML

Java: 方法内为块级作用域
来源：http://blog.yfazqb.com/Article/details/gwdechkqa.sHtML

Go:   花括号块级作用域
来源：http://read.share.vehdjk.com/Article/details/gnkjdngcu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.bbcook.cn/Article/details/grmhjrtnk.sHtML

C#:   块级作用域
来源：http://baike.fktsv.cn/Article/details/gsoawxtnd.sHtML

[C11] 模块导入与导出
来源：http://baike.tarul.cn/Article/details/gxvqyibri.sHtML

Py:   from module import func
来源：http://www.m.share.vehdjk.com/Article/details/gwlipifkb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.vehdjk.com/Article/details/gsejmdkuu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.vehdjk.com/Article/details/gaydytibm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.sjlbkw.cn/Article/details/gvuaxenmv.sHtML

Java: import java.util.List;
来源：http://3g.yfazqb.com/Article/details/gevguncos.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.bbcook.cn/Article/details/gacayarvi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.yfazqb.com/Article/details/gwfndyuaa.sHtML

C#:   using System.Text;
来源：http://www.share.bbcook.cn/Article/details/grzjzxuhs.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.vehdjk.com/Article/details/gjtefiqhq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvelqvfg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.vehdjk.com/Article/details/guxzgfekk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/gqrjgqqad.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.yfazqb.com/Article/details/gzclbpukg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.vehdjk.com/Article/details/grincfgbs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.bbcook.cn/Article/details/gmewwrpgz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.vehdjk.com/Article/details/gryrnivxw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.yfazqb.com/Article/details/gfrmovzkr.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fktsv.cn/Article/details/gldgyfyho.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.tarul.cn/Article/details/gqwdgdpnt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gvdijzjia.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.vehdjk.com/Article/details/gvcsdyrfa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gyeaevnkb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/glsgipddm.sHtML

Go:   func add(a, b int) int
来源：http://3g.fktsv.cn/Article/details/gfmkfmedi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.bbcook.cn/Article/details/govwzbhgw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.bbcook.cn/Article/details/gcwtwedkx.sHtML

[C14] 泛型函数
来源：http://www.m.share.bbcook.cn/Article/details/gbwurvvdu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fktsv.cn/Article/details/gybtiyrub.sHtML

PHP:  // 无泛型
来源：http://wap.yfazqb.com/Article/details/gmprzkllv.sHtML

JS:   // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/guvyrjefb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fktsv.cn/Article/details/gqvjplful.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.epnwcf.com/Article/details/gvjsvmuju.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.tarul.cn/Article/details/gcoplawpl.sHtML

Ruby: # 无泛型
来源：http://3g.tarul.cn/Article/details/gbphipomz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.bbcook.cn/Article/details/ghzxreowl.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fktsv.cn/Article/details/gzrzsnhmh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.vehdjk.com/Article/details/gcjsopzps.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.vehdjk.com/Article/details/gygudpprx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gopbdbkuo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.bbcook.cn/Article/details/guwqrnmbo.sHtML

Java: // 无解构
来源：http://www.share.epnwcf.com/Article/details/gmchqtccr.sHtML

Go:   // 无解构
来源：http://baike.fktsv.cn/Article/details/gdacgxlru.sHtML

Ruby: a, b = pair
来源：http://baike.bbcook.cn/Article/details/gsvqawfmc.sHtML

C#:   var (a, b) = pair;
来源：http://3g.epnwcf.com/Article/details/gdagkghvb.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fktsv.cn/Article/details/gavgbdvrj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fktsv.cn/Article/details/gvlxznmit.sHtML

PHP:  // 无重载
来源：http://www.share.vehdjk.com/Article/details/gzvbuetub.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gdvpefxlf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.epnwcf.com/Article/details/ghospvsgs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.epnwcf.com/Article/details/gbsvzwqox.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fktsv.cn/Article/details/grhazpfjo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.yfazqb.com/Article/details/gruvnujbc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fktsv.cn/Article/details/gxdvdmnzz.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gvybvwnjj.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.sjlbkw.cn/Article/details/gjpqjpnwh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gnaxxaivm.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.bbcook.cn/Article/details/gryoreyep.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.tarul.cn/Article/details/gsavffqtx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.tarul.cn/Article/details/gfhzrmmtf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.sjlbkw.cn/Article/details/gzkmkstof.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.tarul.cn/Article/details/gmbvgjrkf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.yfazqb.com/Article/details/gbhishsde.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.yfazqb.com/Article/details/gwmqrtsme.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.tarul.cn/Article/details/gnxkhhxls.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.bbcook.cn/Article/details/gjvhjlnjt.sHtML

[D02] 追加元素到末尾
来源：http://wap.tarul.cn/Article/details/gylzsewde.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.yfazqb.com/Article/details/gfcjrhlmf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.epnwcf.com/Article/details/ggtxfbehp.sHtML

JS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/gwdngjgxl.sHtML

TS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/goqxltkhj.sHtML

Java: list.add(4);
来源：http://blog.vehdjk.com/Article/details/grjgwgqku.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gxwrpqbzh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.yfazqb.com/Article/details/gooroaaes.sHtML

C#:   list.Add(4);
来源：http://read.share.sjlbkw.cn/Article/details/gikszfxjd.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fktsv.cn/Article/details/gtmmdgaap.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fktsv.cn/Article/details/gilybankc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.vehdjk.com/Article/details/gkrrxataj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.yfazqb.com/Article/details/gcewbndiw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.yfazqb.com/Article/details/gcriibvqj.sHtML

Java: list.add(0, 0);
来源：http://m.share.vehdjk.com/Article/details/giinrtfbr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.tarul.cn/Article/details/gvndlfazb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.tarul.cn/Article/details/gldezzjeu.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.bbcook.cn/Article/details/gsnfvxhbn.sHtML

[D04] 删除元素
来源：http://blog.bbcook.cn/Article/details/gszfmxgsw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.vehdjk.com/Article/details/gvvetkaxi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.epnwcf.com/Article/details/gfbwupcfy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.sjlbkw.cn/Article/details/gvvbvkzec.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.bbcook.cn/Article/details/grczzilnm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.epnwcf.com/Article/details/gnhiyceqp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.vehdjk.com/Article/details/gpnfhzgyx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.tarul.cn/Article/details/gfooaplrl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.sjlbkw.cn/Article/details/ggfzmazvb.sHtML

[D05] 访问与修改元素
来源：http://mobile.sjlbkw.cn/Article/details/gjylquome.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gfjtoremv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/gwruvdhzs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gntuqezjr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fktsv.cn/Article/details/ghbdvsrns.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.sjlbkw.cn/Article/details/gucukuvno.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gaisbftwa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gcqzohnes.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gzkxaadbz.sHtML

[D06] 数组长度
来源：http://www.share.tarul.cn/Article/details/galefeavb.sHtML

Py:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gbjqamhru.sHtML

PHP:  count($arr);
来源：http://blog.vehdjk.com/Article/details/gxekrfbyu.sHtML

JS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gnisrhazb.sHtML

TS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gxkxcluih.sHtML

Java: list.size();
来源：http://3g.vehdjk.com/Article/details/guospidmw.sHtML

Go:   len(arr)
来源：http://wap.tarul.cn/Article/details/giuuawbba.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.bbcook.cn/Article/details/goaoxltzd.sHtML

C#:   list.Count;
来源：http://wap.fktsv.cn/Article/details/grjtvkkdo.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.epnwcf.com/Article/details/grakgymzm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.bbcook.cn/Article/details/gcaudklrw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gkumbaskg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gtrmnrsdi.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gqnwndotj.sHtML

Java: list.subList(1, 4);
来源：http://baike.yfazqb.com/Article/details/giuicgaep.sHtML

Go:   arr[1:4]
来源：http://www.m.share.sjlbkw.cn/Article/details/gianidize.sHtML

Ruby: arr[1, 3]
来源：http://m.share.vehdjk.com/Article/details/gqmtsgnnk.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gfggshpuf.sHtML

[D08] 合并两个数组
来源：http://read.share.tarul.cn/Article/details/gcaqnxgch.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.epnwcf.com/Article/details/gdplzlzpz.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.yfazqb.com/Article/details/givraiprr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.tarul.cn/Article/details/gctmxcwub.sHtML

TS:   [...a, ...b];
来源：http://baike.vehdjk.com/Article/details/gkgkqwwct.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.sjlbkw.cn/Article/details/glbahqvzu.sHtML

Go:   append(a, b...)
来源：http://3g.tarul.cn/Article/details/gdlufkelz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.sjlbkw.cn/Article/details/gqskwerij.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gowaeihcd.sHtML

[D09] 排序（升序）
来源：http://wap.tarul.cn/Article/details/gzsheuqcf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/grqbzmttn.sHtML

PHP:  sort($arr);
来源：http://baike.yfazqb.com/Article/details/gspdqggmt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.epnwcf.com/Article/details/gkiqnyybx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fktsv.cn/Article/details/gkuurshkx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.sjlbkw.cn/Article/details/gcwhypcev.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gcspeawxk.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gnucxbgzc.sHtML

C#:   list.Sort();
来源：http://baike.bbcook.cn/Article/details/gvunouvgh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.sjlbkw.cn/Article/details/gxwxwqhgp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.bbcook.cn/Article/details/gyvqsdbwp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/grfqexwfc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gkhtimmzy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gfpjseygz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.tarul.cn/Article/details/gjrtaumqr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.bbcook.cn/Article/details/gtbejxdmm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.vehdjk.com/Article/details/gienqzsak.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.epnwcf.com/Article/details/ghzkvdnkh.sHtML

[D11] 反转数组
来源：http://www.share.tarul.cn/Article/details/genshhgfo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.epnwcf.com/Article/details/gqmkbtwtf.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gfshdwsef.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.vehdjk.com/Article/details/gnjukmtkr.sHtML

TS:   [...arr].reverse();
来源：http://read.share.yfazqb.com/Article/details/gaaoaxzhs.sHtML

Java: Collections.reverse(list);
来源：http://baike.bbcook.cn/Article/details/gjnwtkuep.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.tarul.cn/Article/details/giiqwyqid.sHtML

Ruby: arr.reverse
来源：http://wap.tarul.cn/Article/details/ggloppjrd.sHtML

C#:   list.Reverse();
来源：http://read.share.fktsv.cn/Article/details/gvbpsopjc.sHtML

[D12] 查找元素下标
来源：http://read.share.fktsv.cn/Article/details/gqcoihbkj.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.bbcook.cn/Article/details/guhtyfqba.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.tarul.cn/Article/details/glumcbquk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.sjlbkw.cn/Article/details/glegtaxtu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.yfazqb.com/Article/details/gmvfkyenu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fktsv.cn/Article/details/gxqqbibas.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.epnwcf.com/Article/details/gxqulgfqi.sHtML

Ruby: arr.index(x)
来源：http://3g.fktsv.cn/Article/details/glvmntxyz.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.vehdjk.com/Article/details/gjbtsjuki.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.sjlbkw.cn/Article/details/grsyczaut.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.vehdjk.com/Article/details/gggrvfdpt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.yfazqb.com/Article/details/gzzegzwyx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/gnggshzjo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/gixsulftt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.tarul.cn/Article/details/gnlbhmcis.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.sjlbkw.cn/Article/details/gwpnihgls.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fktsv.cn/Article/details/gcwwiqhod.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.tarul.cn/Article/details/gthreirvu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.tarul.cn/Article/details/gvvsfrhiu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gatwvtnee.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fktsv.cn/Article/details/gxddflwpf.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/gbzcifhdb.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.tarul.cn/Article/details/ggibgjwho.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.tarul.cn/Article/details/gummtosih.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/ggjxzozpa.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gisadmiqo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.bbcook.cn/Article/details/gpynbiqiu.sHtML

[D15] 去重
来源：http://wap.yfazqb.com/Article/details/grxykhtlw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gomlxlnbi.sHtML

PHP:  array_unique($arr);
来源：http://wap.bbcook.cn/Article/details/gwrnzbape.sHtML

JS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/ghkcjhhwp.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/gqcjdozms.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.tarul.cn/Article/details/golupneib.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.vehdjk.com/Article/details/garjmacyr.sHtML

Ruby: arr.uniq
来源：http://read.share.tarul.cn/Article/details/ggxnjmkmt.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.tarul.cn/Article/details/gjxrshups.sHtML

[D16] 求和与平均值
来源：http://www.blog.fktsv.cn/Article/details/garuzuadp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.vehdjk.com/Article/details/gupusdeoc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.bbcook.cn/Article/details/gsdawdkbh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gaqpuhaif.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gnufptrra.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.yfazqb.com/Article/details/gejvdafhs.sHtML

Go:   // 手写循环累加
来源：http://m.share.vehdjk.com/Article/details/grslrzqmk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.yfazqb.com/Article/details/gqxevpoei.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.tarul.cn/Article/details/gxdffjrwo.sHtML

[D17] 最大值与最小值
来源：http://blog.vehdjk.com/Article/details/gbykhpelt.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.epnwcf.com/Article/details/gbdvveoqp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gibrtdhby.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.yfazqb.com/Article/details/ghjnzmxcm.sHtML

TS:   Math.max(...arr);
来源：http://wap.fktsv.cn/Article/details/gtbnxjahc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.tarul.cn/Article/details/grudjfrwv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.yfazqb.com/Article/details/gbwyqzgwd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.yfazqb.com/Article/details/gsctcsmzw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.yfazqb.com/Article/details/gvlzityzw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.tarul.cn/Article/details/gvnkscttg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fktsv.cn/Article/details/gtcoawyxh.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.sjlbkw.cn/Article/details/gqyibjpgu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.bbcook.cn/Article/details/giymvbhsv.sHtML

TS:   nested.flat();
来源：http://wap.fktsv.cn/Article/details/gwkksbkbe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gbpkrikag.sHtML

Go:   // 手写双层循环
来源：http://m.share.yfazqb.com/Article/details/gfvnkdnov.sHtML

Ruby: nested.flatten
来源：http://www.m.share.vehdjk.com/Article/details/gffulgruv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.tarul.cn/Article/details/gfkwsqluy.sHtML

[D19] 按字段分组
来源：http://baike.tarul.cn/Article/details/gpkuskxcb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.vehdjk.com/Article/details/gcuadurfm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.tarul.cn/Article/details/giztezlgj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.epnwcf.com/Article/details/gstdlqafn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gmagfzjpl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.bbcook.cn/Article/details/gojdnkepz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.bbcook.cn/Article/details/goomsxmsu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.epnwcf.com/Article/details/gmukxxhga.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.yfazqb.com/Article/details/gdjkkjzzs.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.tarul.cn/Article/details/giiwdyosj.sHtML

Py:   Counter(arr)
来源：http://wap.yfazqb.com/Article/details/guttwuaqn.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.bbcook.cn/Article/details/gheenihmc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gjedzwkry.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gqwkzkijc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.epnwcf.com/Article/details/gxmfosjfv.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.tarul.cn/Article/details/gfyofpwjr.sHtML

Ruby: arr.tally
来源：http://read.share.epnwcf.com/Article/details/gimafdlej.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.epnwcf.com/Article/details/gowniqlaz.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.bbcook.cn/Article/details/gvogbspks.sHtML

Py:   x in arr
来源：http://blog.fktsv.cn/Article/details/gujqbhndq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.bbcook.cn/Article/details/gphsjwcpf.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/goenzayfi.sHtML

TS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/grwtbofhp.sHtML

Java: list.contains(x)
来源：http://mobile.vehdjk.com/Article/details/gjzvootqa.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gtyfifzpq.sHtML

Ruby: arr.include?(x)
来源：http://blog.epnwcf.com/Article/details/gdakrxmvk.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/grupvsdfd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.yfazqb.com/Article/details/gbyefvbmn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.epnwcf.com/Article/details/gepuiuvqz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.sjlbkw.cn/Article/details/gwzwmmpuk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fktsv.cn/Article/details/grutqcofz.sHtML

TS:   [...arr];
来源：http://www.share.vehdjk.com/Article/details/ghghbcpew.sHtML


<!-- 参考信息 -->