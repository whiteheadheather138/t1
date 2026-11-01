代发 wailian999

Py:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gcbiibntv.sHtML

PHP:  return [$a, $b];
来源：http://www.share.bbcook.cn/Article/details/geussgeaz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.epnwcf.com/Article/details/gfarrjdam.sHtML

TS:   return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gcgjxkrkn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.tarul.cn/Article/details/gvfsmnmvg.sHtML

Go:   return a, b
来源：http://www.share.bbcook.cn/Article/details/gnvzasjiw.sHtML

Ruby: return a, b
来源：http://www.share.epnwcf.com/Article/details/ghagxpptn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.sjlbkw.cn/Article/details/gbjjstrus.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.tarul.cn/Article/details/gqszdhgvx.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.tarul.cn/Article/details/gmesxvraj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fktsv.cn/Article/details/glvgerqpu.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gjivchksc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.bbcook.cn/Article/details/gueshkgtp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.tarul.cn/Article/details/gcmnadpzu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.bbcook.cn/Article/details/gnphougee.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.vehdjk.com/Article/details/gmukybevw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fktsv.cn/Article/details/gfvbkdoyj.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.epnwcf.com/Article/details/gfvynyrhj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.vehdjk.com/Article/details/gomrtymhw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.tarul.cn/Article/details/gwjkcutoa.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.vehdjk.com/Article/details/goqkeesyf.sHtML

TS:   arr.map(String)
来源：http://3g.fktsv.cn/Article/details/glwmclafi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.epnwcf.com/Article/details/guihfiuks.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.bbcook.cn/Article/details/gnyekjdvb.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.tarul.cn/Article/details/gavndmsgq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.yfazqb.com/Article/details/gcivodgog.sHtML

[C08] 闭包
来源：http://m.share.vehdjk.com/Article/details/gpvrumjhc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.tarul.cn/Article/details/gyyloxigg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.sjlbkw.cn/Article/details/gcvrsfmeb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/geabcaebe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gpcvatopr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/gkpnwklct.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.sjlbkw.cn/Article/details/geoikihus.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.bbcook.cn/Article/details/gipjrlpbt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/ggfqipsmn.sHtML

[C09] 递归
来源：http://read.share.tarul.cn/Article/details/giyjuazmo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/geevymslm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.vehdjk.com/Article/details/gmqqbhqpz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.sjlbkw.cn/Article/details/gtpvmgefq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/glenkykyl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.tarul.cn/Article/details/gjptbnhnu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.epnwcf.com/Article/details/gedrnuqag.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/gdxykawgp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.tarul.cn/Article/details/gtxduxrym.sHtML

[C10] 变量作用域
来源：http://m.share.bbcook.cn/Article/details/gdquotwmy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.tarul.cn/Article/details/gyovtbbig.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.sjlbkw.cn/Article/details/gfjxwsehs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.vehdjk.com/Article/details/glppcmnip.sHtML

TS:   同 JS
来源：http://www.blog.vehdjk.com/Article/details/ggoikjlgy.sHtML

Java: 方法内为块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gqcumhvzb.sHtML

Go:   花括号块级作用域
来源：http://wap.epnwcf.com/Article/details/gplblwgrj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fktsv.cn/Article/details/gjiscwhxf.sHtML

C#:   块级作用域
来源：http://www.share.epnwcf.com/Article/details/gyfkowmzq.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.epnwcf.com/Article/details/gyiyzqhsb.sHtML

Py:   from module import func
来源：http://mobile.epnwcf.com/Article/details/gpcaaonfq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.bbcook.cn/Article/details/gpxfxoaik.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/gdichqust.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.epnwcf.com/Article/details/genxrczdn.sHtML

Java: import java.util.List;
来源：http://baike.yfazqb.com/Article/details/gfwoouhsi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.epnwcf.com/Article/details/gpgonhjyc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.vehdjk.com/Article/details/ggtglymwm.sHtML

C#:   using System.Text;
来源：http://read.share.vehdjk.com/Article/details/grpqtynef.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.yfazqb.com/Article/details/gmpdomwps.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.bbcook.cn/Article/details/gtzrruptx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.sjlbkw.cn/Article/details/gukbsxpbj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.tarul.cn/Article/details/gjhmxsitg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/gcxrioixm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.tarul.cn/Article/details/gmscbjbcv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.tarul.cn/Article/details/gpzrwcyfk.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.sjlbkw.cn/Article/details/gwmugjdfp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.bbcook.cn/Article/details/ghayigyit.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.tarul.cn/Article/details/guwumkbdb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.yfazqb.com/Article/details/gjepmicyq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gjupnytuo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.tarul.cn/Article/details/ggrmicjpe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gjjiijxqj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/guwemdzlh.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.bbcook.cn/Article/details/gdknpaalb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fktsv.cn/Article/details/grdrumvdl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.tarul.cn/Article/details/gjqsvvryw.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/geaqhprrk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.bbcook.cn/Article/details/gvzpfwuyn.sHtML

PHP:  // 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gghtaokbm.sHtML

JS:   // 无泛型
来源：http://blog.epnwcf.com/Article/details/ggtehagmm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.bbcook.cn/Article/details/gddbgyrxl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.bbcook.cn/Article/details/gaisugubh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fktsv.cn/Article/details/guaadravl.sHtML

Ruby: # 无泛型
来源：http://mobile.tarul.cn/Article/details/gkgtewyin.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fktsv.cn/Article/details/ggeovdvtk.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.vehdjk.com/Article/details/gwfljvuwv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.sjlbkw.cn/Article/details/gtpboodwe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.yfazqb.com/Article/details/gvpnhivvq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.tarul.cn/Article/details/gumumsyzc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.vehdjk.com/Article/details/gcpaurtfm.sHtML

Java: // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gefbbvjek.sHtML

Go:   // 无解构
来源：http://3g.vehdjk.com/Article/details/gbdrqlbjs.sHtML

Ruby: a, b = pair
来源：http://3g.epnwcf.com/Article/details/gkvlrbovb.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.yfazqb.com/Article/details/gzoizjoic.sHtML

[C16] 函数 / 方法重载
来源：http://blog.bbcook.cn/Article/details/grshrtodw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fktsv.cn/Article/details/gvlgvwpjr.sHtML

PHP:  // 无重载
来源：http://www.share.fktsv.cn/Article/details/ghejakrau.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.tarul.cn/Article/details/gthxzpqfv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/gtenjsbcn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.tarul.cn/Article/details/gsdyzimvo.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.tarul.cn/Article/details/geitpguqp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.tarul.cn/Article/details/goalnzejj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.epnwcf.com/Article/details/grnjumjfv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gotykozch.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fktsv.cn/Article/details/gueoclqrm.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glqfxmzwq.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fktsv.cn/Article/details/gcjoilevz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.yfazqb.com/Article/details/gjaslemwu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fktsv.cn/Article/details/goikeuuls.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.vehdjk.com/Article/details/gmazfdwva.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.bbcook.cn/Article/details/gyknfdgrt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.sjlbkw.cn/Article/details/ghvqzjtbp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/gvjlxklkn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.tarul.cn/Article/details/gdemdpftk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.tarul.cn/Article/details/gxdusbexx.sHtML

[D02] 追加元素到末尾
来源：http://www.share.yfazqb.com/Article/details/gpitooxdx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.bbcook.cn/Article/details/glykcukku.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.tarul.cn/Article/details/gfdpjlfmy.sHtML

JS:   arr.push(4);
来源：http://www.blog.yfazqb.com/Article/details/gteifjmto.sHtML

TS:   arr.push(4);
来源：http://blog.epnwcf.com/Article/details/gepztzpnt.sHtML

Java: list.add(4);
来源：http://3g.vehdjk.com/Article/details/grsofouyg.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.sjlbkw.cn/Article/details/gnsupmgot.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fktsv.cn/Article/details/gkbxamsup.sHtML

C#:   list.Add(4);
来源：http://m.share.sjlbkw.cn/Article/details/gqdbneriy.sHtML

[D03] 在指定位置插入元素
来源：http://baike.vehdjk.com/Article/details/gprmuskse.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.tarul.cn/Article/details/gudeeroge.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fktsv.cn/Article/details/gkaghwbfn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.yfazqb.com/Article/details/gcpsmjefm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.tarul.cn/Article/details/grfhkddvv.sHtML

Java: list.add(0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gfbzjwkpz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.tarul.cn/Article/details/gzuxtfiat.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.sjlbkw.cn/Article/details/gbdfmkekb.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.epnwcf.com/Article/details/gywjjxztl.sHtML

[D04] 删除元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gncyyzhdt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.bbcook.cn/Article/details/gzuqbttsj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.yfazqb.com/Article/details/gjnrkmjog.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fktsv.cn/Article/details/gvrxpgdpn.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.vehdjk.com/Article/details/gztmjqhku.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fktsv.cn/Article/details/gfaeefylv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fktsv.cn/Article/details/gltbbdlob.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.yfazqb.com/Article/details/gjjhfoqxd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fktsv.cn/Article/details/gbgkjsvgy.sHtML

[D05] 访问与修改元素
来源：http://mobile.tarul.cn/Article/details/gtesyvbbh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/grwumwnkf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gwutqykgf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gcsjpaiay.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.yfazqb.com/Article/details/gprvsnykz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.vehdjk.com/Article/details/gkbyfevse.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gyupuwyys.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gwdykidjo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gxpncgfxa.sHtML

[D06] 数组长度
来源：http://m.share.vehdjk.com/Article/details/giarwgknb.sHtML

Py:   len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/grsaebkvl.sHtML

PHP:  count($arr);
来源：http://mobile.fktsv.cn/Article/details/gxxaadyxn.sHtML

JS:   arr.length
来源：http://3g.tarul.cn/Article/details/gvduibffi.sHtML

TS:   arr.length
来源：http://3g.epnwcf.com/Article/details/gktleigug.sHtML

Java: list.size();
来源：http://wap.sjlbkw.cn/Article/details/gpykbuqbj.sHtML

Go:   len(arr)
来源：http://m.share.yfazqb.com/Article/details/gsdkdqeqx.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fktsv.cn/Article/details/ghivivgmn.sHtML

C#:   list.Count;
来源：http://blog.vehdjk.com/Article/details/gvcftrgrh.sHtML

[D07] 切片 / 取子数组
来源：http://3g.epnwcf.com/Article/details/gmgpcoxis.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.epnwcf.com/Article/details/giitpmnky.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.yfazqb.com/Article/details/gevkdwjvs.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/ghykkevws.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gryoqajcr.sHtML

Java: list.subList(1, 4);
来源：http://wap.fktsv.cn/Article/details/gaslrhzdy.sHtML

Go:   arr[1:4]
来源：http://www.m.share.tarul.cn/Article/details/gjzgdbppk.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.sjlbkw.cn/Article/details/gawydaxhq.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.epnwcf.com/Article/details/gdmirnaar.sHtML

[D08] 合并两个数组
来源：http://baike.vehdjk.com/Article/details/gszwhublp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.tarul.cn/Article/details/gfozeyier.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.tarul.cn/Article/details/goldsgcoq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.epnwcf.com/Article/details/gmcnsapxm.sHtML

TS:   [...a, ...b];
来源：http://mobile.bbcook.cn/Article/details/gvwngzewp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.yfazqb.com/Article/details/gyrhplhtu.sHtML

Go:   append(a, b...)
来源：http://3g.fktsv.cn/Article/details/gvylopsqo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fktsv.cn/Article/details/gkdshzmtx.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.epnwcf.com/Article/details/gjjryblsl.sHtML

[D09] 排序（升序）
来源：http://mobile.epnwcf.com/Article/details/gyeonwvtt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gvminpioo.sHtML

PHP:  sort($arr);
来源：http://blog.sjlbkw.cn/Article/details/gbarkxmti.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/gwfqmsnlu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.yfazqb.com/Article/details/gqjkpptfw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.epnwcf.com/Article/details/gclqvooln.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/grnftypge.sHtML

Ruby: arr.sort
来源：http://m.share.yfazqb.com/Article/details/gbwnsgbdw.sHtML

C#:   list.Sort();
来源：http://baike.tarul.cn/Article/details/gwxmianec.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.vehdjk.com/Article/details/gpiuzmxdf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.epnwcf.com/Article/details/ggkrejjdr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.yfazqb.com/Article/details/giuwaotbw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.bbcook.cn/Article/details/gyeeeheqo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fktsv.cn/Article/details/gbfgmtkjj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.epnwcf.com/Article/details/gnjlkzbxa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.yfazqb.com/Article/details/ggolwvpxx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.yfazqb.com/Article/details/guwtyihxw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.tarul.cn/Article/details/gfqgambhc.sHtML

[D11] 反转数组
来源：http://m.share.sjlbkw.cn/Article/details/geybcnnwe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.yfazqb.com/Article/details/gwyddiaap.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.tarul.cn/Article/details/gwuabizoj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.vehdjk.com/Article/details/gfyynrvth.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.epnwcf.com/Article/details/gpbdpbube.sHtML

Java: Collections.reverse(list);
来源：http://read.share.vehdjk.com/Article/details/gfvmbqzhj.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.bbcook.cn/Article/details/gvaavtnek.sHtML

Ruby: arr.reverse
来源：http://www.share.epnwcf.com/Article/details/gzqxlbicd.sHtML

C#:   list.Reverse();
来源：http://blog.bbcook.cn/Article/details/gmkflkxno.sHtML

[D12] 查找元素下标
来源：http://baike.fktsv.cn/Article/details/gwuasqhlc.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.tarul.cn/Article/details/giqmtowcx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.yfazqb.com/Article/details/gbalcvqdf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gerqiyieg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.epnwcf.com/Article/details/gnlvbpbjz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.bbcook.cn/Article/details/gchjcumaf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gciprasux.sHtML

Ruby: arr.index(x)
来源：http://www.blog.bbcook.cn/Article/details/goiaogejx.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fktsv.cn/Article/details/gesdmmszi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fktsv.cn/Article/details/guvutxcri.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.tarul.cn/Article/details/gxmjdqcqh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.yfazqb.com/Article/details/guwogfeea.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fktsv.cn/Article/details/gmwdjxuje.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gaymeonej.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.yfazqb.com/Article/details/gxvasgwyd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.vehdjk.com/Article/details/gphbkakqp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.vehdjk.com/Article/details/gnnlxabwv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.vehdjk.com/Article/details/gmbwmyozo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.sjlbkw.cn/Article/details/gheckaxrz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.epnwcf.com/Article/details/gdiewdmkj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.vehdjk.com/Article/details/gejckjsww.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/geahmdqoi.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/gogefiyax.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.yfazqb.com/Article/details/gvpzknpxg.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/gdndynays.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fktsv.cn/Article/details/gykbwnwcg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.epnwcf.com/Article/details/gfyzarzio.sHtML

[D15] 去重
来源：http://mobile.epnwcf.com/Article/details/gjbkzrbue.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gsbrkovfm.sHtML

PHP:  array_unique($arr);
来源：http://blog.fktsv.cn/Article/details/gicuhgkjs.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/guzqxylhf.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/ghrxmibau.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.tarul.cn/Article/details/gysvstjzh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.sjlbkw.cn/Article/details/goxrnomci.sHtML

Ruby: arr.uniq
来源：http://read.share.bbcook.cn/Article/details/gyfqntidx.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.sjlbkw.cn/Article/details/gtzsmsrcg.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/gzqpdkrdr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.vehdjk.com/Article/details/guljkplwl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.bbcook.cn/Article/details/ggcuoildl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gnucdurax.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gtwuzfgwn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/geaqejgyq.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoqxzpnc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.bbcook.cn/Article/details/gznuevuav.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.epnwcf.com/Article/details/ghtmfbems.sHtML

[D17] 最大值与最小值
来源：http://www.blog.vehdjk.com/Article/details/galdiobvp.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.vehdjk.com/Article/details/gcavaopab.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.vehdjk.com/Article/details/gwfpusqmo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.tarul.cn/Article/details/gmnnxzvup.sHtML

TS:   Math.max(...arr);
来源：http://blog.fktsv.cn/Article/details/gwefnqzxc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.tarul.cn/Article/details/guwatmkeg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.epnwcf.com/Article/details/gtuinndzm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.vehdjk.com/Article/details/ggdthlhjj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.yfazqb.com/Article/details/gfiljrwzu.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.vehdjk.com/Article/details/gavyarwuj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.bbcook.cn/Article/details/gmhkttind.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.sjlbkw.cn/Article/details/gjloafzqb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.vehdjk.com/Article/details/gpmvqogfn.sHtML

TS:   nested.flat();
来源：http://mobile.vehdjk.com/Article/details/gecbbnqxk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgwfsque.sHtML

Go:   // 手写双层循环
来源：http://3g.tarul.cn/Article/details/gejcdxlhc.sHtML

Ruby: nested.flatten
来源：http://www.m.share.sjlbkw.cn/Article/details/gzztlkpjg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gpgdsvsmt.sHtML

[D19] 按字段分组
来源：http://www.m.share.epnwcf.com/Article/details/gnzwjivhi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.bbcook.cn/Article/details/gtagkafqt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.vehdjk.com/Article/details/gbatncnqs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/gyurxopbn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.tarul.cn/Article/details/gauuhvbqx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.epnwcf.com/Article/details/gadplsnvm.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.epnwcf.com/Article/details/gjupmxlxb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.bbcook.cn/Article/details/gdznzumxj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.vehdjk.com/Article/details/gvgdkmcvu.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.tarul.cn/Article/details/ggsiiyyxr.sHtML

Py:   Counter(arr)
来源：http://www.blog.yfazqb.com/Article/details/gjeqjgspr.sHtML

PHP:  array_count_values($arr);
来源：http://blog.vehdjk.com/Article/details/gstdohrum.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/gzhgtoiiw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gztyyrhuv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fktsv.cn/Article/details/guodiqcla.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fktsv.cn/Article/details/ganygqxbc.sHtML

Ruby: arr.tally
来源：http://mobile.vehdjk.com/Article/details/gmvqtvyyo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.sjlbkw.cn/Article/details/gkkjzgpoc.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fktsv.cn/Article/details/grhcjgurw.sHtML

Py:   x in arr
来源：http://m.share.fktsv.cn/Article/details/gtsktkbgt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.tarul.cn/Article/details/gbygieaba.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gtbsgpwvh.sHtML

TS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/ghpwwohen.sHtML

Java: list.contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gmrarocte.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.tarul.cn/Article/details/gqmwkvcdq.sHtML

Ruby: arr.include?(x)
来源：http://www.share.yfazqb.com/Article/details/gcpcmuxne.sHtML

C#:   list.Contains(x)
来源：http://m.share.tarul.cn/Article/details/glqozoxfp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.tarul.cn/Article/details/gvonkdqow.sHtML


<!-- 参考信息 -->