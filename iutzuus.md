代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.yfazqb.com/Article/details/giznpmxlc.sHtML

Go:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gstmlonxx.sHtML

Ruby: return a, b
来源：http://wap.vehdjk.com/Article/details/ghdmxdixt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.sjlbkw.cn/Article/details/glwoyzrtu.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.epnwcf.com/Article/details/gqbskwaje.sHtML

Py:   square = lambda x: x * x
来源：http://baike.sjlbkw.cn/Article/details/gzilyhybc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.bbcook.cn/Article/details/grhhhqcqc.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gagrnhlqa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gfkuvgfez.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fktsv.cn/Article/details/grnjhjybx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.sjlbkw.cn/Article/details/gdvxfyxda.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.yfazqb.com/Article/details/gbuqjeeyd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/gjqsemaxl.sHtML

[C07] 把函数作为参数传入
来源：http://baike.vehdjk.com/Article/details/gzghzrbkk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.vehdjk.com/Article/details/gkuwqyhcj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.epnwcf.com/Article/details/gcylwgycx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.yfazqb.com/Article/details/gmtubjrkj.sHtML

TS:   arr.map(String)
来源：http://www.share.bbcook.cn/Article/details/gdarbeshn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.bbcook.cn/Article/details/gueuswtcp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.sjlbkw.cn/Article/details/gjeajjulh.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.sjlbkw.cn/Article/details/gyhsiyafv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.epnwcf.com/Article/details/gphoxwsda.sHtML

[C08] 闭包
来源：http://wap.epnwcf.com/Article/details/giyzpapnf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.tarul.cn/Article/details/genicdxjg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.tarul.cn/Article/details/gauxomurk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gqfutxgos.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/glnbznyyi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.epnwcf.com/Article/details/gcrrvsnau.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.sjlbkw.cn/Article/details/gzveaojky.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fktsv.cn/Article/details/gzmemgnoq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/ghngqheuf.sHtML

[C09] 递归
来源：http://www.blog.tarul.cn/Article/details/ggwllaien.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gackcpwlw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.tarul.cn/Article/details/grhhodyot.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/gyvnupzlx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fktsv.cn/Article/details/gjadivpvd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.vehdjk.com/Article/details/gqzgysiqm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.vehdjk.com/Article/details/giimumaas.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.tarul.cn/Article/details/gqaverzzu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.vehdjk.com/Article/details/gsnpatisp.sHtML

[C10] 变量作用域
来源：http://3g.bbcook.cn/Article/details/gbmfmjixp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.epnwcf.com/Article/details/gysiuuvvx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.epnwcf.com/Article/details/gybzgevda.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.bbcook.cn/Article/details/gnzvqstkq.sHtML

TS:   同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gjteabkvy.sHtML

Java: 方法内为块级作用域
来源：http://mobile.yfazqb.com/Article/details/gxkpkgruz.sHtML

Go:   花括号块级作用域
来源：http://3g.sjlbkw.cn/Article/details/glpbigayj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.yfazqb.com/Article/details/gyhwffwsx.sHtML

C#:   块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/guuukqbog.sHtML

[C11] 模块导入与导出
来源：http://mobile.epnwcf.com/Article/details/garkltwcv.sHtML

Py:   from module import func
来源：http://3g.fktsv.cn/Article/details/gkgcfvbzc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.tarul.cn/Article/details/gsuccuvvg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.tarul.cn/Article/details/gptmvvwjs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.vehdjk.com/Article/details/gmzodujbb.sHtML

Java: import java.util.List;
来源：http://www.blog.vehdjk.com/Article/details/gluilnpzr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.tarul.cn/Article/details/gqclunvbt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/gkxercntu.sHtML

C#:   using System.Text;
来源：http://www.m.share.fktsv.cn/Article/details/gijedsulx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fktsv.cn/Article/details/gfljxibtf.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.epnwcf.com/Article/details/glkhorftm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.sjlbkw.cn/Article/details/ggiapqwoq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/glbtacchw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gcbotblpk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.epnwcf.com/Article/details/gtekkwrzm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.bbcook.cn/Article/details/gwdbhqecf.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fktsv.cn/Article/details/gfyethane.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.tarul.cn/Article/details/gckxwfgfd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.epnwcf.com/Article/details/gwrruyvom.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.tarul.cn/Article/details/gndufvild.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gznifhndf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.vehdjk.com/Article/details/gjatoivcb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gwefuouuc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/geozhvlvw.sHtML

Go:   func add(a, b int) int
来源：http://m.share.vehdjk.com/Article/details/goyvzrbsb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.sjlbkw.cn/Article/details/guhcoazvk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvucbxwxv.sHtML

[C14] 泛型函数
来源：http://wap.vehdjk.com/Article/details/gtlsexlkt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.vehdjk.com/Article/details/gcnynifro.sHtML

PHP:  // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/ghsqlbgym.sHtML

JS:   // 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gzdjhuhvg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.bbcook.cn/Article/details/gdptfszqc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.bbcook.cn/Article/details/gjwhdkwhw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.bbcook.cn/Article/details/gphkqtrbo.sHtML

Ruby: # 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gqqcqrbtz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.tarul.cn/Article/details/gdotqpdfx.sHtML

[C15] 解构 / 展开参数
来源：http://wap.sjlbkw.cn/Article/details/goomprkgb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.bbcook.cn/Article/details/gttlgxzkw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.yfazqb.com/Article/details/gdcypcnqw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/geuuoieav.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.yfazqb.com/Article/details/gskhskozd.sHtML

Java: // 无解构
来源：http://m.share.tarul.cn/Article/details/gufslnonj.sHtML

Go:   // 无解构
来源：http://read.share.epnwcf.com/Article/details/gytivvcuf.sHtML

Ruby: a, b = pair
来源：http://read.share.vehdjk.com/Article/details/gagjrfsgs.sHtML

C#:   var (a, b) = pair;
来源：http://3g.vehdjk.com/Article/details/gzeyhwwca.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.yfazqb.com/Article/details/gqdyammhv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.bbcook.cn/Article/details/ggrbsqbdk.sHtML

PHP:  // 无重载
来源：http://3g.vehdjk.com/Article/details/gzvpurafl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.yfazqb.com/Article/details/gfyzqrwwc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fktsv.cn/Article/details/gfgukhaub.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fktsv.cn/Article/details/gxugupijx.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.tarul.cn/Article/details/gbafamvel.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fktsv.cn/Article/details/gvqfmpdjj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fktsv.cn/Article/details/ghphmnkto.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/giedhfwbw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.sjlbkw.cn/Article/details/gzqpeobmr.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gvbfjrund.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.vehdjk.com/Article/details/gnhjforpp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fktsv.cn/Article/details/gyjvmbkrp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gubboociy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fktsv.cn/Article/details/gfmuuymay.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fktsv.cn/Article/details/govwhpncy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.vehdjk.com/Article/details/gtipisgvl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.sjlbkw.cn/Article/details/gfqdbjwkw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.sjlbkw.cn/Article/details/gvdzjfrxb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.tarul.cn/Article/details/gbyafkpcc.sHtML

[D02] 追加元素到末尾
来源：http://3g.bbcook.cn/Article/details/gpbubajnr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.tarul.cn/Article/details/gqebduizo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.sjlbkw.cn/Article/details/gfqgfeybi.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fktsv.cn/Article/details/gwnzlxasr.sHtML

TS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/gmbhpfqoj.sHtML

Java: list.add(4);
来源：http://read.share.vehdjk.com/Article/details/gqwpslixa.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.epnwcf.com/Article/details/gduqsdvnt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fktsv.cn/Article/details/grycaldrn.sHtML

C#:   list.Add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkafegby.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.yfazqb.com/Article/details/gxqejtdpz.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.bbcook.cn/Article/details/givzpucsh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.bbcook.cn/Article/details/gbykwxlde.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.bbcook.cn/Article/details/gnlqtpase.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.tarul.cn/Article/details/giirwumus.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gizijlfrs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.tarul.cn/Article/details/gbmmcaldv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.bbcook.cn/Article/details/gezqckide.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.epnwcf.com/Article/details/gffuouvdl.sHtML

[D04] 删除元素
来源：http://wap.yfazqb.com/Article/details/gzrebziom.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.sjlbkw.cn/Article/details/gsncrylat.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.tarul.cn/Article/details/gmdzfydrb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fktsv.cn/Article/details/gpmxynwub.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.bbcook.cn/Article/details/gthgpmxig.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gcyvxcprf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.bbcook.cn/Article/details/gtwlblgln.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.bbcook.cn/Article/details/grwdehnaz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.tarul.cn/Article/details/grtgvsqil.sHtML

[D05] 访问与修改元素
来源：http://3g.tarul.cn/Article/details/gilqjcuau.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gkinpehjd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gssfphrag.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gikwykntg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fktsv.cn/Article/details/gtqvlqekn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.epnwcf.com/Article/details/gtotpgorj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/ghbydkwtn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gaasbxmcv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gnhkbeqax.sHtML

[D06] 数组长度
来源：http://www.share.tarul.cn/Article/details/gvachinws.sHtML

Py:   len(arr)
来源：http://www.share.epnwcf.com/Article/details/gfmmhpgcg.sHtML

PHP:  count($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gxpobimzz.sHtML

JS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gskdigtxy.sHtML

TS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/gluimxlhi.sHtML

Java: list.size();
来源：http://www.m.share.yfazqb.com/Article/details/ggqvngjsd.sHtML

Go:   len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gotoohxuo.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gknvmxkxv.sHtML

C#:   list.Count;
来源：http://baike.bbcook.cn/Article/details/ggfkfgrqq.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.sjlbkw.cn/Article/details/gyptjftzz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.epnwcf.com/Article/details/gcvlxbdst.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fktsv.cn/Article/details/gotepqfad.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gkbdtwftv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gehkybwux.sHtML

Java: list.subList(1, 4);
来源：http://3g.epnwcf.com/Article/details/gljynxzhr.sHtML

Go:   arr[1:4]
来源：http://read.share.vehdjk.com/Article/details/grmuvkxqq.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.yfazqb.com/Article/details/gtjlnqmif.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fktsv.cn/Article/details/gpmyqkxdi.sHtML

[D08] 合并两个数组
来源：http://www.m.share.yfazqb.com/Article/details/goynkljzr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.tarul.cn/Article/details/gjinyfolq.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fktsv.cn/Article/details/gclfdtvjz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.vehdjk.com/Article/details/gtwhwiniv.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.epnwcf.com/Article/details/gflrupwec.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gqzqibiht.sHtML

Go:   append(a, b...)
来源：http://baike.fktsv.cn/Article/details/gwesgvhrw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fktsv.cn/Article/details/gxvibicwp.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.epnwcf.com/Article/details/gtahtugzh.sHtML

[D09] 排序（升序）
来源：http://www.share.epnwcf.com/Article/details/glpytzdxn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/ghdqqeiwv.sHtML

PHP:  sort($arr);
来源：http://read.share.bbcook.cn/Article/details/gafzjpwvv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.vehdjk.com/Article/details/gxjezuoyz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvowfjcb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.sjlbkw.cn/Article/details/guqufjiqs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/ggokpzxtu.sHtML

Ruby: arr.sort
来源：http://baike.bbcook.cn/Article/details/gedllfbbs.sHtML

C#:   list.Sort();
来源：http://blog.fktsv.cn/Article/details/gznrwyjse.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.epnwcf.com/Article/details/gzohecknx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.bbcook.cn/Article/details/gkjqdhvsb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gfacvlawh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/gqeljwhlx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.epnwcf.com/Article/details/gyggzgupe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.vehdjk.com/Article/details/gbjrbuboa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.bbcook.cn/Article/details/gbcntvwwp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fktsv.cn/Article/details/gqmdtjbta.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fktsv.cn/Article/details/gjrcfkvri.sHtML

[D11] 反转数组
来源：http://www.m.share.bbcook.cn/Article/details/gdmuylawk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.yfazqb.com/Article/details/gsbdmhasf.sHtML

PHP:  array_reverse($arr);
来源：http://blog.sjlbkw.cn/Article/details/gfuvgoiwb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.tarul.cn/Article/details/gowkvisjp.sHtML

TS:   [...arr].reverse();
来源：http://mobile.sjlbkw.cn/Article/details/gtlemvuuq.sHtML

Java: Collections.reverse(list);
来源：http://blog.sjlbkw.cn/Article/details/gpfvixujx.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.bbcook.cn/Article/details/gwunefpms.sHtML

Ruby: arr.reverse
来源：http://read.share.vehdjk.com/Article/details/gxkdkyirx.sHtML

C#:   list.Reverse();
来源：http://baike.bbcook.cn/Article/details/ggozghlhz.sHtML

[D12] 查找元素下标
来源：http://wap.vehdjk.com/Article/details/gyehaceuq.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.epnwcf.com/Article/details/gytyvapal.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.vehdjk.com/Article/details/gwsfxfwfb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gwcfiummt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fktsv.cn/Article/details/gbljydiqu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.yfazqb.com/Article/details/gawfhtoui.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.vehdjk.com/Article/details/ggvxqcntg.sHtML

Ruby: arr.index(x)
来源：http://3g.yfazqb.com/Article/details/gfimoscmh.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.vehdjk.com/Article/details/gxalboqbp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.tarul.cn/Article/details/gzcjygejo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.epnwcf.com/Article/details/gmxueryxs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fktsv.cn/Article/details/gyocypyts.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gryddmrkt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/gjybvtosw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.vehdjk.com/Article/details/gqsqvtaiv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.bbcook.cn/Article/details/gqzotphau.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.yfazqb.com/Article/details/glkojetfl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.tarul.cn/Article/details/gfxyunxun.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fktsv.cn/Article/details/gynoibtsc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.epnwcf.com/Article/details/gfmcmlydh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fktsv.cn/Article/details/ghncejzvz.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/gdaxgimeh.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.yfazqb.com/Article/details/gbvyswmil.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.bbcook.cn/Article/details/gsmymzrxj.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gncfalwxq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gjpzrihdt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.epnwcf.com/Article/details/gbreatxqu.sHtML

[D15] 去重
来源：http://www.share.tarul.cn/Article/details/gldufgleb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gugwxbhry.sHtML

PHP:  array_unique($arr);
来源：http://wap.fktsv.cn/Article/details/gikmilkur.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/grrrkxtsv.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/ggtqtzurs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.epnwcf.com/Article/details/gpwouqgxs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.sjlbkw.cn/Article/details/gwqonlktz.sHtML

Ruby: arr.uniq
来源：http://mobile.epnwcf.com/Article/details/gtggaqxbx.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gcudyyptv.sHtML

[D16] 求和与平均值
来源：http://read.share.bbcook.cn/Article/details/gubrddrvz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.bbcook.cn/Article/details/gwwnjlthb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.bbcook.cn/Article/details/gxulnuijj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gnjikskwp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/gbuffftha.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.yfazqb.com/Article/details/gvytbrjkf.sHtML

Go:   // 手写循环累加
来源：http://blog.fktsv.cn/Article/details/gavjipafs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fktsv.cn/Article/details/gdheibsdh.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.sjlbkw.cn/Article/details/gxebrtuwz.sHtML

[D17] 最大值与最小值
来源：http://m.share.fktsv.cn/Article/details/gaszvonsr.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.vehdjk.com/Article/details/gqekqrxzk.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.tarul.cn/Article/details/gtxvzjjpy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.tarul.cn/Article/details/gmtcqvrhg.sHtML

TS:   Math.max(...arr);
来源：http://wap.fktsv.cn/Article/details/gcghuostw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.yfazqb.com/Article/details/gcufbzxnh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.tarul.cn/Article/details/gkdjqklkd.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/gwjrwcjeo.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fktsv.cn/Article/details/gzdhnxuky.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.sjlbkw.cn/Article/details/gzanldhfj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.vehdjk.com/Article/details/gadvdzhep.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.yfazqb.com/Article/details/gihepncqu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fktsv.cn/Article/details/gtyppdbvw.sHtML

TS:   nested.flat();
来源：http://m.share.vehdjk.com/Article/details/gcapvghjc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.tarul.cn/Article/details/geewwakky.sHtML

Go:   // 手写双层循环
来源：http://mobile.vehdjk.com/Article/details/gurmsqglm.sHtML

Ruby: nested.flatten
来源：http://www.blog.bbcook.cn/Article/details/gqakyvtnx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.tarul.cn/Article/details/ggkafhagw.sHtML

[D19] 按字段分组
来源：http://www.share.sjlbkw.cn/Article/details/gluqkebkz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.epnwcf.com/Article/details/gtzftccyl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fktsv.cn/Article/details/gjuwnxkep.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.bbcook.cn/Article/details/gnmwiiqdz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.epnwcf.com/Article/details/giggetrbm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.epnwcf.com/Article/details/gpehbcqtb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.vehdjk.com/Article/details/gisljrrzb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.tarul.cn/Article/details/glamucmad.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fktsv.cn/Article/details/gcwwelhqj.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.sjlbkw.cn/Article/details/gnzcankfc.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gyjwsczqw.sHtML

PHP:  array_count_values($arr);
来源：http://blog.yfazqb.com/Article/details/guhrswahz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/gnxrmxmlr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.yfazqb.com/Article/details/gbcpgwvft.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.vehdjk.com/Article/details/govqpbfde.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fktsv.cn/Article/details/gbcfrabgo.sHtML

Ruby: arr.tally
来源：http://read.share.yfazqb.com/Article/details/gzljmuisw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fktsv.cn/Article/details/gxqabyuhp.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.tarul.cn/Article/details/grzqiecvx.sHtML

Py:   x in arr
来源：http://baike.bbcook.cn/Article/details/guuftwrhl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.bbcook.cn/Article/details/gporgabcx.sHtML

JS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/ganbutsfq.sHtML

TS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gbubhrpce.sHtML

Java: list.contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gihuvdtth.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.yfazqb.com/Article/details/gqjwjqzwp.sHtML

Ruby: arr.include?(x)
来源：http://wap.fktsv.cn/Article/details/grilqclrn.sHtML

C#:   list.Contains(x)
来源：http://wap.yfazqb.com/Article/details/gdmzjkvvo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.vehdjk.com/Article/details/gcyockgqk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/gfyllndqe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.tarul.cn/Article/details/gsryphbtt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.epnwcf.com/Article/details/goltqtuwe.sHtML

TS:   [...arr];
来源：http://baike.sjlbkw.cn/Article/details/guplywwfv.sHtML


<!-- 参考信息 -->