代发 wailian999

Py:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gmeplnamc.sHtML

PHP:  return [$a, $b];
来源：http://baike.vehdjk.com/Article/details/geanfrqlb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gotckidyt.sHtML

TS:   return { a, b };
来源：http://mobile.fktsv.cn/Article/details/gerdauush.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.epnwcf.com/Article/details/gijjuuuvz.sHtML

Go:   return a, b
来源：http://baike.fktsv.cn/Article/details/ghnjtodnf.sHtML

Ruby: return a, b
来源：http://www.share.vehdjk.com/Article/details/gdabuutsi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.bbcook.cn/Article/details/gmskynlbl.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.sjlbkw.cn/Article/details/gupdhnzrc.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fktsv.cn/Article/details/gkizwjafk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.epnwcf.com/Article/details/gojytxtiq.sHtML

JS:   const square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/gidqnspgd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.yfazqb.com/Article/details/goqgcggja.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.vehdjk.com/Article/details/ghyeurqdh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.vehdjk.com/Article/details/gkamkslob.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.vehdjk.com/Article/details/ggopbfzmn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gxprjybot.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.yfazqb.com/Article/details/gwrdqgndo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.epnwcf.com/Article/details/gflyvgrty.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.epnwcf.com/Article/details/guoogrjjo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fktsv.cn/Article/details/grltcxdti.sHtML

TS:   arr.map(String)
来源：http://baike.tarul.cn/Article/details/gmwylipah.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gzxkvkgkj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fktsv.cn/Article/details/gatnifeyl.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.tarul.cn/Article/details/gkhqawjpn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.sjlbkw.cn/Article/details/gywaehmjj.sHtML

[C08] 闭包
来源：http://wap.yfazqb.com/Article/details/gyzuixldf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fktsv.cn/Article/details/gxvzikdfe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.vehdjk.com/Article/details/grbrznbxj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/grxclxzkq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/grwncfuhl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.yfazqb.com/Article/details/gdgnpiicj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.bbcook.cn/Article/details/gooexufag.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gfcollsfm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gkxubeezq.sHtML

[C09] 递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzwztams.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.vehdjk.com/Article/details/guljvtaeq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/gbskdrjha.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gqunwvypw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.yfazqb.com/Article/details/gksdjtfhe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcckrjor.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.epnwcf.com/Article/details/gmxwpakym.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gsdntoibd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.bbcook.cn/Article/details/gvfvxbqel.sHtML

[C10] 变量作用域
来源：http://baike.tarul.cn/Article/details/gfnhevned.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.sjlbkw.cn/Article/details/gmejbqcyn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.epnwcf.com/Article/details/gbwehxamf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fktsv.cn/Article/details/gymdjrbbs.sHtML

TS:   同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gahacyxqs.sHtML

Java: 方法内为块级作用域
来源：http://baike.yfazqb.com/Article/details/gtlubeaft.sHtML

Go:   花括号块级作用域
来源：http://read.share.fktsv.cn/Article/details/gfslriuor.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.tarul.cn/Article/details/gzfmbjofz.sHtML

C#:   块级作用域
来源：http://www.share.epnwcf.com/Article/details/gxutxtfwt.sHtML

[C11] 模块导入与导出
来源：http://wap.vehdjk.com/Article/details/gvetogvrp.sHtML

Py:   from module import func
来源：http://blog.sjlbkw.cn/Article/details/gbwrdhnqe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fktsv.cn/Article/details/gneydnblb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/gsdrclilq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.yfazqb.com/Article/details/guugmwegh.sHtML

Java: import java.util.List;
来源：http://www.blog.yfazqb.com/Article/details/gsvrmoquz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.sjlbkw.cn/Article/details/glwehrhzi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.vehdjk.com/Article/details/gyttutffr.sHtML

C#:   using System.Text;
来源：http://blog.vehdjk.com/Article/details/gjwsnggji.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.yfazqb.com/Article/details/gcbsnbcua.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.vehdjk.com/Article/details/gdgsuzlzl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.epnwcf.com/Article/details/gbcazfvni.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/grdtumqwh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/guoqbvfei.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.yfazqb.com/Article/details/gwwgbhrbb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.tarul.cn/Article/details/gqvhlbirm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.sjlbkw.cn/Article/details/gtpblfype.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.bbcook.cn/Article/details/gvawgpoly.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.vehdjk.com/Article/details/gxzqynzjz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.bbcook.cn/Article/details/gqourtbni.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gubefjgcy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.yfazqb.com/Article/details/gezmmmjvv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gzrlybpyr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gvdtxwmei.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.epnwcf.com/Article/details/gkqemhdwx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.yfazqb.com/Article/details/gcnvnhglt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.sjlbkw.cn/Article/details/gyojaicjd.sHtML

[C14] 泛型函数
来源：http://mobile.vehdjk.com/Article/details/gxuuabizq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.sjlbkw.cn/Article/details/gibhextnr.sHtML

PHP:  // 无泛型
来源：http://blog.epnwcf.com/Article/details/gvjbptbph.sHtML

JS:   // 无泛型
来源：http://m.share.yfazqb.com/Article/details/guuawzsqb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.tarul.cn/Article/details/gvgmxvkvy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.sjlbkw.cn/Article/details/gizgajqwe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.bbcook.cn/Article/details/gepxmbpjz.sHtML

Ruby: # 无泛型
来源：http://wap.epnwcf.com/Article/details/gwjnjwgvb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fktsv.cn/Article/details/gpxgcwfon.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.vehdjk.com/Article/details/gdldhxluv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/gdkwvqrce.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.yfazqb.com/Article/details/gtqcsykcq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/gxmvfkdtp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fktsv.cn/Article/details/gkqxfdiih.sHtML

Java: // 无解构
来源：http://www.blog.fktsv.cn/Article/details/gukgtcvwt.sHtML

Go:   // 无解构
来源：http://wap.sjlbkw.cn/Article/details/ghohbdysl.sHtML

Ruby: a, b = pair
来源：http://mobile.bbcook.cn/Article/details/gtxesfmxy.sHtML

C#:   var (a, b) = pair;
来源：http://wap.tarul.cn/Article/details/gzzrdjemx.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fktsv.cn/Article/details/ghlioqodq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.bbcook.cn/Article/details/gungocyeo.sHtML

PHP:  // 无重载
来源：http://wap.tarul.cn/Article/details/gsfcoesfa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.vehdjk.com/Article/details/gtbbvfrhn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fktsv.cn/Article/details/ggpvvkaap.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.tarul.cn/Article/details/ghscunnun.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.vehdjk.com/Article/details/gvtmgmclv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.yfazqb.com/Article/details/gplaufjsb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.bbcook.cn/Article/details/gdoidegim.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbbytvyvy.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fktsv.cn/Article/details/gdgpdeqpd.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ghtacanfa.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fktsv.cn/Article/details/gbagkpdww.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fktsv.cn/Article/details/gdbnfjczn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.tarul.cn/Article/details/ghrivejve.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.vehdjk.com/Article/details/gjqnatlvc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.sjlbkw.cn/Article/details/gxboodzhj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.sjlbkw.cn/Article/details/glegtpbwn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fktsv.cn/Article/details/guucjxjae.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.epnwcf.com/Article/details/gjfrdceye.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.vehdjk.com/Article/details/gnwrqhfku.sHtML

[D02] 追加元素到末尾
来源：http://3g.epnwcf.com/Article/details/ghcckrhjn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fktsv.cn/Article/details/gzjzuuuzf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.tarul.cn/Article/details/geawrvxgx.sHtML

JS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gymkdyyer.sHtML

TS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gojehshjy.sHtML

Java: list.add(4);
来源：http://read.share.tarul.cn/Article/details/gpcggmkdc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gjcsvtgls.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.vehdjk.com/Article/details/gzsodqact.sHtML

C#:   list.Add(4);
来源：http://baike.yfazqb.com/Article/details/gyueymmoh.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fktsv.cn/Article/details/gcppzaduz.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fktsv.cn/Article/details/gauxbfepy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fktsv.cn/Article/details/gjlddmqve.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.sjlbkw.cn/Article/details/gojwawzyx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.bbcook.cn/Article/details/gfuwmcpeb.sHtML

Java: list.add(0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gqxsofkmn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.bbcook.cn/Article/details/garqggobo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.sjlbkw.cn/Article/details/gqbgxguos.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.sjlbkw.cn/Article/details/ggptqrasi.sHtML

[D04] 删除元素
来源：http://mobile.bbcook.cn/Article/details/gbbeeemvn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.yfazqb.com/Article/details/gplcquxcj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.epnwcf.com/Article/details/gowdrsnzu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fktsv.cn/Article/details/gjrwjhexo.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.tarul.cn/Article/details/gxkaungpu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fktsv.cn/Article/details/gidhxmmsa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.yfazqb.com/Article/details/gpzwbreqx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.tarul.cn/Article/details/gomjqmnob.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.vehdjk.com/Article/details/gjmgntdpb.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.yfazqb.com/Article/details/grdynpdax.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/gjqqtbaxi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gegaxneud.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gqcwhposo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.bbcook.cn/Article/details/ghwpvrhrz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.sjlbkw.cn/Article/details/gfvwwtyud.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/gzxfimkog.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmxgqrmh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gylpahnbf.sHtML

[D06] 数组长度
来源：http://www.share.bbcook.cn/Article/details/grfbmfamm.sHtML

Py:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/gucipwgdn.sHtML

PHP:  count($arr);
来源：http://3g.tarul.cn/Article/details/guzkigjes.sHtML

JS:   arr.length
来源：http://www.blog.epnwcf.com/Article/details/gshyfrlls.sHtML

TS:   arr.length
来源：http://mobile.tarul.cn/Article/details/gxbgwxkgv.sHtML

Java: list.size();
来源：http://blog.tarul.cn/Article/details/glijqjbsu.sHtML

Go:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/ggnnkuwri.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.epnwcf.com/Article/details/greisyjzh.sHtML

C#:   list.Count;
来源：http://read.share.vehdjk.com/Article/details/ghdrenrdb.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.sjlbkw.cn/Article/details/glvkdxsxn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.yfazqb.com/Article/details/gotonqnac.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fktsv.cn/Article/details/gxrojgxrz.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gnhpsxbuh.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gvsbpaukq.sHtML

Java: list.subList(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gztjgnkos.sHtML

Go:   arr[1:4]
来源：http://www.blog.yfazqb.com/Article/details/ggcoddpwm.sHtML

Ruby: arr[1, 3]
来源：http://www.share.yfazqb.com/Article/details/geflbjmep.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.tarul.cn/Article/details/gfjgiawmf.sHtML

[D08] 合并两个数组
来源：http://www.blog.yfazqb.com/Article/details/gqfpwtllg.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.sjlbkw.cn/Article/details/gdnvjltsl.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.tarul.cn/Article/details/gjrjtnsrs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.bbcook.cn/Article/details/gcmrbzrag.sHtML

TS:   [...a, ...b];
来源：http://www.share.epnwcf.com/Article/details/gxwqndxar.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.tarul.cn/Article/details/grtrlqgws.sHtML

Go:   append(a, b...)
来源：http://www.share.vehdjk.com/Article/details/goupfxuqv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fktsv.cn/Article/details/gqinavowc.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.yfazqb.com/Article/details/gtluxumtx.sHtML

[D09] 排序（升序）
来源：http://www.m.share.bbcook.cn/Article/details/gvyulssae.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gnigbjbtb.sHtML

PHP:  sort($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/glbqpcyuu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.sjlbkw.cn/Article/details/gnndxdmza.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.yfazqb.com/Article/details/gygnenpxu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.yfazqb.com/Article/details/gvkdvrgsv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.tarul.cn/Article/details/gepfzxlfi.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/gejkohvui.sHtML

C#:   list.Sort();
来源：http://m.share.fktsv.cn/Article/details/gsnvsrfse.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.sjlbkw.cn/Article/details/ggzverhkx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.epnwcf.com/Article/details/gllmyllqz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.yfazqb.com/Article/details/gxysbuowv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/gmqvwbsth.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.sjlbkw.cn/Article/details/gefsgnfyl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.sjlbkw.cn/Article/details/gobvszxrr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fktsv.cn/Article/details/gkkheolcv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.yfazqb.com/Article/details/gwzxvumgu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fktsv.cn/Article/details/gptiixyyz.sHtML

[D11] 反转数组
来源：http://m.share.yfazqb.com/Article/details/gadmknptt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.bbcook.cn/Article/details/gghofluyq.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fktsv.cn/Article/details/gcqibhipl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.tarul.cn/Article/details/gaudfqukw.sHtML

TS:   [...arr].reverse();
来源：http://3g.tarul.cn/Article/details/gxwbrxrti.sHtML

Java: Collections.reverse(list);
来源：http://www.share.tarul.cn/Article/details/gbwabburk.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.tarul.cn/Article/details/gluduamlo.sHtML

Ruby: arr.reverse
来源：http://mobile.bbcook.cn/Article/details/gaebglasi.sHtML

C#:   list.Reverse();
来源：http://wap.vehdjk.com/Article/details/gbmvmhqmj.sHtML

[D12] 查找元素下标
来源：http://blog.yfazqb.com/Article/details/gjhahyjgk.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.vehdjk.com/Article/details/gdogyvlyt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fktsv.cn/Article/details/gxcvkqfgp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.tarul.cn/Article/details/gkuqatxxl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/guozbxlgz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.sjlbkw.cn/Article/details/gikacqorl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gnyaqweac.sHtML

Ruby: arr.index(x)
来源：http://mobile.vehdjk.com/Article/details/gxeuqbdcz.sHtML

C#:   list.IndexOf(x);
来源：http://wap.bbcook.cn/Article/details/gswycmcml.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.vehdjk.com/Article/details/gouzfjbfr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.vehdjk.com/Article/details/gypcyaazo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fktsv.cn/Article/details/gawonjtwf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.epnwcf.com/Article/details/gkzdijmmf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/gaylfsbau.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fktsv.cn/Article/details/gydaqdmjk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.tarul.cn/Article/details/gividnwrf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.epnwcf.com/Article/details/glgtrlrnf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gdxeewduf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.yfazqb.com/Article/details/gjcyglibm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.epnwcf.com/Article/details/gghhxzyvg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.tarul.cn/Article/details/gcghfelig.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/ggfphgisp.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/guuvtqsyf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.bbcook.cn/Article/details/gezwenxkb.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gyihrezkk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gmdsjlsru.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/geuczepxa.sHtML

[D15] 去重
来源：http://mobile.bbcook.cn/Article/details/gwxbmihke.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fktsv.cn/Article/details/gkxegqupz.sHtML

PHP:  array_unique($arr);
来源：http://baike.yfazqb.com/Article/details/gmkkksbub.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/gtnsziplm.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gitkkrfqr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.epnwcf.com/Article/details/gjkobqtnt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fktsv.cn/Article/details/grovvjsac.sHtML

Ruby: arr.uniq
来源：http://www.share.bbcook.cn/Article/details/ghziqjfex.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/givjojqil.sHtML

[D16] 求和与平均值
来源：http://m.share.yfazqb.com/Article/details/grsneenxv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.epnwcf.com/Article/details/gjlpfnqvw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.sjlbkw.cn/Article/details/gvycojtuv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/gsjuibrxu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/giomughze.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fktsv.cn/Article/details/gxybtaemg.sHtML

Go:   // 手写循环累加
来源：http://blog.yfazqb.com/Article/details/gqohlpywx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.vehdjk.com/Article/details/gwxtfgsib.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.yfazqb.com/Article/details/ghgalwoue.sHtML

[D17] 最大值与最小值
来源：http://baike.fktsv.cn/Article/details/gvtgpsymc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.vehdjk.com/Article/details/gedocxefz.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.vehdjk.com/Article/details/gpeydndyd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.epnwcf.com/Article/details/gzexeqxlf.sHtML

TS:   Math.max(...arr);
来源：http://wap.tarul.cn/Article/details/gkikpvyjb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fktsv.cn/Article/details/gkikcizuh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.vehdjk.com/Article/details/gcfxbfrou.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.tarul.cn/Article/details/gbzzbbzcw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.epnwcf.com/Article/details/gufwsyzin.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.tarul.cn/Article/details/gieecgvcn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.epnwcf.com/Article/details/gawwfoyht.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.yfazqb.com/Article/details/gjaziqobb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.yfazqb.com/Article/details/gwrtitvnh.sHtML

TS:   nested.flat();
来源：http://wap.tarul.cn/Article/details/gsipntbsi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fktsv.cn/Article/details/gzjehzcph.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fktsv.cn/Article/details/giyujcpsq.sHtML

Ruby: nested.flatten
来源：http://m.share.vehdjk.com/Article/details/gbxcbqwzh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gumptnumj.sHtML

[D19] 按字段分组
来源：http://baike.tarul.cn/Article/details/ghghyymbh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.tarul.cn/Article/details/gfduhzmgy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.bbcook.cn/Article/details/ggpazyzvn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.vehdjk.com/Article/details/glertfwff.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.yfazqb.com/Article/details/ghdotosho.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.tarul.cn/Article/details/gbcskjhaq.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.sjlbkw.cn/Article/details/gfvndtqzh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.epnwcf.com/Article/details/giszhfujt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.epnwcf.com/Article/details/gnqdmsnyg.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.tarul.cn/Article/details/gnfzfyuwb.sHtML

Py:   Counter(arr)
来源：http://www.m.share.tarul.cn/Article/details/godiijjzp.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fktsv.cn/Article/details/gudigajxv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/gcfbbyzgn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.vehdjk.com/Article/details/gzgigajpu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fktsv.cn/Article/details/gidmhvsgx.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.yfazqb.com/Article/details/ghudbpffb.sHtML

Ruby: arr.tally
来源：http://read.share.fktsv.cn/Article/details/ghtggfvmq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.bbcook.cn/Article/details/gmriayejx.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.vehdjk.com/Article/details/gbzhejrnp.sHtML

Py:   x in arr
来源：http://m.share.yfazqb.com/Article/details/gfsihujox.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/gvwnxeyqj.sHtML

JS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gcmpxxqyn.sHtML

TS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gxcaulifs.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gkacioscu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnqfgzur.sHtML

Ruby: arr.include?(x)
来源：http://wap.tarul.cn/Article/details/gauxiexyo.sHtML

C#:   list.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/gyujqryjs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.vehdjk.com/Article/details/goqleitgx.sHtML


<!-- 参考信息 -->