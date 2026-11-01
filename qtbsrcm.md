代发 wailian999

[C06] 匿名函数 / lambda
来源：http://read.share.tarul.cn/Article/details/gwtedoizq.sHtML

Py:   square = lambda x: x * x
来源：http://wap.yfazqb.com/Article/details/gdpixnsde.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.epnwcf.com/Article/details/grqepcxuh.sHtML

JS:   const square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gprgxmqxo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fktsv.cn/Article/details/gkgebfzhz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.tarul.cn/Article/details/ghpzxkflm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.epnwcf.com/Article/details/gtdfjolon.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.sjlbkw.cn/Article/details/gtxejajqt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.tarul.cn/Article/details/gzipctnml.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.epnwcf.com/Article/details/gbgnvcnme.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.vehdjk.com/Article/details/gafasmigr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.epnwcf.com/Article/details/gghvovbtw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fktsv.cn/Article/details/gsmaprhbo.sHtML

TS:   arr.map(String)
来源：http://blog.fktsv.cn/Article/details/gmksubdcn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.tarul.cn/Article/details/gqaaywrrp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.yfazqb.com/Article/details/gaiajeend.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.yfazqb.com/Article/details/gjkotzura.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.epnwcf.com/Article/details/gbkentmxt.sHtML

[C08] 闭包
来源：http://baike.sjlbkw.cn/Article/details/glsrcuwzj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.tarul.cn/Article/details/gjsqdbagq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.yfazqb.com/Article/details/gdehfuzes.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/giyxnnaty.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gzxjfxbfm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.tarul.cn/Article/details/gevwobuqy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.vehdjk.com/Article/details/grigobmvv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fktsv.cn/Article/details/gvmkvttdy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gikjljojg.sHtML

[C09] 递归
来源：http://www.m.share.fktsv.cn/Article/details/ghcljhcbd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.tarul.cn/Article/details/gllsyibdb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.epnwcf.com/Article/details/gmdooljea.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.sjlbkw.cn/Article/details/gakotczwi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fktsv.cn/Article/details/gudspjkit.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.epnwcf.com/Article/details/gfsbiyoyw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.epnwcf.com/Article/details/gsygyqjsu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fktsv.cn/Article/details/gnetvwplt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fktsv.cn/Article/details/ggjxaqdqi.sHtML

[C10] 变量作用域
来源：http://baike.bbcook.cn/Article/details/gpkwioadb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.epnwcf.com/Article/details/gvosyfcrc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.epnwcf.com/Article/details/gefobrpyk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.sjlbkw.cn/Article/details/gcrvlcsrd.sHtML

TS:   同 JS
来源：http://m.share.tarul.cn/Article/details/gtgksmezm.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gdpmumdbv.sHtML

Go:   花括号块级作用域
来源：http://3g.epnwcf.com/Article/details/gzjfozyzw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.bbcook.cn/Article/details/gwkdeatoq.sHtML

C#:   块级作用域
来源：http://read.share.epnwcf.com/Article/details/gbxoccdun.sHtML

[C11] 模块导入与导出
来源：http://www.share.sjlbkw.cn/Article/details/gjcqduhqz.sHtML

Py:   from module import func
来源：http://wap.yfazqb.com/Article/details/gydudqshy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.bbcook.cn/Article/details/gjmnszqcz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.tarul.cn/Article/details/gxpboyjzm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.vehdjk.com/Article/details/glxontoxe.sHtML

Java: import java.util.List;
来源：http://read.share.epnwcf.com/Article/details/gheslikql.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.sjlbkw.cn/Article/details/gvjeanvus.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fktsv.cn/Article/details/gupfbzcjb.sHtML

C#:   using System.Text;
来源：http://3g.vehdjk.com/Article/details/grsffpacf.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.vehdjk.com/Article/details/gpiqoaagd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.bbcook.cn/Article/details/garfhpmqe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.epnwcf.com/Article/details/glmmvyasj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.sjlbkw.cn/Article/details/gtwremigl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/guigwtpnh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.tarul.cn/Article/details/gesbdxeyu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.epnwcf.com/Article/details/gfhuvwerx.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.vehdjk.com/Article/details/gojysdsle.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.vehdjk.com/Article/details/gxrhhvjzf.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.bbcook.cn/Article/details/gyfnyfqxc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.sjlbkw.cn/Article/details/gcqwqxode.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gwchfcana.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.yfazqb.com/Article/details/gzddkamws.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gputugjzj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gddcxbvoz.sHtML

Go:   func add(a, b int) int
来源：http://mobile.bbcook.cn/Article/details/gvcrigdkb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.yfazqb.com/Article/details/gggchqbqk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.epnwcf.com/Article/details/gwoqzigow.sHtML

[C14] 泛型函数
来源：http://www.m.share.epnwcf.com/Article/details/geaebiwts.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.vehdjk.com/Article/details/geckfbowf.sHtML

PHP:  // 无泛型
来源：http://blog.yfazqb.com/Article/details/gtkdotkeu.sHtML

JS:   // 无泛型
来源：http://mobile.yfazqb.com/Article/details/getmxcvif.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.sjlbkw.cn/Article/details/gwthdjdvv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fktsv.cn/Article/details/ghvgwqikl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.epnwcf.com/Article/details/gijyaptbp.sHtML

Ruby: # 无泛型
来源：http://www.share.epnwcf.com/Article/details/gpufkfssq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.tarul.cn/Article/details/gtpgdnqpy.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.epnwcf.com/Article/details/givslwunu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.vehdjk.com/Article/details/gffehxnil.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.yfazqb.com/Article/details/gwmzyjepz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrbcaszm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.yfazqb.com/Article/details/gziosknbw.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/gmtyhccmw.sHtML

Go:   // 无解构
来源：http://wap.bbcook.cn/Article/details/gzbornykv.sHtML

Ruby: a, b = pair
来源：http://m.share.vehdjk.com/Article/details/gmpyrbsht.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.tarul.cn/Article/details/ghsqyjkoy.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.sjlbkw.cn/Article/details/gpvwcwdrf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.epnwcf.com/Article/details/gjuwgkkcw.sHtML

PHP:  // 无重载
来源：http://www.m.share.tarul.cn/Article/details/gbuioqkcm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.bbcook.cn/Article/details/gltgtitit.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.tarul.cn/Article/details/gcrcvlqcy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fktsv.cn/Article/details/gstmsntzz.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.sjlbkw.cn/Article/details/ggszzcwfs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fktsv.cn/Article/details/ghewzvfut.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.vehdjk.com/Article/details/gxhiaalpr.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gcogkggsy.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.vehdjk.com/Article/details/gfnrwsetr.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjeiucsyf.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.bbcook.cn/Article/details/grjtllqja.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.epnwcf.com/Article/details/gwtuszyyi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.epnwcf.com/Article/details/gbutvmoxx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.epnwcf.com/Article/details/gixpxngiq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.epnwcf.com/Article/details/ghlebkqrv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.yfazqb.com/Article/details/gkmsloqzo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.sjlbkw.cn/Article/details/gikymkzos.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.yfazqb.com/Article/details/gzshriqzk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.bbcook.cn/Article/details/gmbmxfmyb.sHtML

[D02] 追加元素到末尾
来源：http://3g.vehdjk.com/Article/details/gprmbhubq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.yfazqb.com/Article/details/gufsodted.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.tarul.cn/Article/details/gtgxblwtb.sHtML

JS:   arr.push(4);
来源：http://read.share.yfazqb.com/Article/details/gyrchvrrg.sHtML

TS:   arr.push(4);
来源：http://wap.yfazqb.com/Article/details/gwjqmkleh.sHtML

Java: list.add(4);
来源：http://baike.sjlbkw.cn/Article/details/gympnrtgu.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.tarul.cn/Article/details/grcdbrxxr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fktsv.cn/Article/details/gzajdpwar.sHtML

C#:   list.Add(4);
来源：http://wap.fktsv.cn/Article/details/ghcdxvopp.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.yfazqb.com/Article/details/gouiyvkut.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/goavhgeyh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.epnwcf.com/Article/details/glmcskurn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.epnwcf.com/Article/details/gyegyllzo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gbnqhvycc.sHtML

Java: list.add(0, 0);
来源：http://baike.tarul.cn/Article/details/gqmphxajg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.epnwcf.com/Article/details/goqgiwvzc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.vehdjk.com/Article/details/gdfekflwf.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fktsv.cn/Article/details/gnzstextr.sHtML

[D04] 删除元素
来源：http://wap.bbcook.cn/Article/details/gzpmwywbf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.tarul.cn/Article/details/gijcevoyx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.bbcook.cn/Article/details/gzundhexy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.sjlbkw.cn/Article/details/giksraulu.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.sjlbkw.cn/Article/details/glstdkijt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.tarul.cn/Article/details/guqmbcwzg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.epnwcf.com/Article/details/ghvzudtav.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fktsv.cn/Article/details/grrbpzftn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.tarul.cn/Article/details/gncbygtio.sHtML

[D05] 访问与修改元素
来源：http://read.share.yfazqb.com/Article/details/gboquqrym.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gepuinpgs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gvyimzqae.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/ggbldcgdf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.tarul.cn/Article/details/gvsfyilru.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.tarul.cn/Article/details/gbhywuzbp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/guhboxmge.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/ggldctkcb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gwapajycq.sHtML

[D06] 数组长度
来源：http://www.blog.tarul.cn/Article/details/gbkhfaraa.sHtML

Py:   len(arr)
来源：http://blog.bbcook.cn/Article/details/gdmwoqbxn.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gmxcbbvgt.sHtML

JS:   arr.length
来源：http://wap.bbcook.cn/Article/details/ggwciumuc.sHtML

TS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/gaipbwmnp.sHtML

Java: list.size();
来源：http://www.share.epnwcf.com/Article/details/gzirtgljd.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gsmwkvrdw.sHtML

Ruby: arr.length; arr.size
来源：http://blog.vehdjk.com/Article/details/gkjmhanec.sHtML

C#:   list.Count;
来源：http://baike.epnwcf.com/Article/details/gbcjldngy.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fktsv.cn/Article/details/gcdqgopcj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.bbcook.cn/Article/details/gpwrgpagj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.yfazqb.com/Article/details/gwzpvmnis.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gmhrahvpx.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/garrhqrlq.sHtML

Java: list.subList(1, 4);
来源：http://wap.tarul.cn/Article/details/giwoifkpm.sHtML

Go:   arr[1:4]
来源：http://blog.bbcook.cn/Article/details/gggptrkej.sHtML

Ruby: arr[1, 3]
来源：http://m.share.vehdjk.com/Article/details/gamcpavry.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.sjlbkw.cn/Article/details/geqnhnpwj.sHtML

[D08] 合并两个数组
来源：http://mobile.fktsv.cn/Article/details/gskiamhkr.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.sjlbkw.cn/Article/details/giwarvvgz.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.epnwcf.com/Article/details/gvpnpsibe.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.bbcook.cn/Article/details/gadfrpnlj.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.yfazqb.com/Article/details/ghfepohpx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.tarul.cn/Article/details/gbcnolesd.sHtML

Go:   append(a, b...)
来源：http://www.blog.fktsv.cn/Article/details/gykhvalvf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.tarul.cn/Article/details/gejefgxve.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gaaofccet.sHtML

[D09] 排序（升序）
来源：http://wap.fktsv.cn/Article/details/gnahtlcmu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/ggxsoopjl.sHtML

PHP:  sort($arr);
来源：http://wap.vehdjk.com/Article/details/gpjzslbsr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.tarul.cn/Article/details/gtmraicfy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.vehdjk.com/Article/details/ggiwoqhpj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.vehdjk.com/Article/details/gawjdcqzk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gvybfymyk.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/gqwuxsani.sHtML

C#:   list.Sort();
来源：http://m.share.fktsv.cn/Article/details/gxafmrmbd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fktsv.cn/Article/details/gpdnepwkv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fktsv.cn/Article/details/gfjilpgnf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gzugrwlmd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.sjlbkw.cn/Article/details/gjifdgcwz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/gmabhptmy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fktsv.cn/Article/details/guppnerry.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.bbcook.cn/Article/details/gjtyrxmef.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.sjlbkw.cn/Article/details/gsgrzdjgd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fktsv.cn/Article/details/gjhldjnnd.sHtML

[D11] 反转数组
来源：http://mobile.yfazqb.com/Article/details/gpuafzzrs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.vehdjk.com/Article/details/gvvhfxmxw.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gonhjqdfd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.yfazqb.com/Article/details/gjkkrnrdp.sHtML

TS:   [...arr].reverse();
来源：http://baike.tarul.cn/Article/details/gdrpuetmf.sHtML

Java: Collections.reverse(list);
来源：http://mobile.vehdjk.com/Article/details/gpgszalfj.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.yfazqb.com/Article/details/gtkuaqtze.sHtML

Ruby: arr.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gootdgxum.sHtML

C#:   list.Reverse();
来源：http://wap.vehdjk.com/Article/details/gvwljdsmf.sHtML

[D12] 查找元素下标
来源：http://read.share.fktsv.cn/Article/details/gpapwqibc.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.bbcook.cn/Article/details/ghxeoigix.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fktsv.cn/Article/details/gvaxfgzff.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fktsv.cn/Article/details/ghvgwuizj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/gemhhkzxw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.vehdjk.com/Article/details/gnvgqwyaa.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gkpoagziw.sHtML

Ruby: arr.index(x)
来源：http://blog.fktsv.cn/Article/details/giygwgfau.sHtML

C#:   list.IndexOf(x);
来源：http://baike.vehdjk.com/Article/details/gudhfmjjd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.sjlbkw.cn/Article/details/gpzitgjas.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fktsv.cn/Article/details/gkmbedlhh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fktsv.cn/Article/details/gdoyhyfbu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gohumpjwx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/geigugboj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.bbcook.cn/Article/details/ggqmymrpr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.sjlbkw.cn/Article/details/gxshvxaoj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.vehdjk.com/Article/details/ggwoagcws.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.epnwcf.com/Article/details/gfnjrbjvj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/gxjeniaks.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.yfazqb.com/Article/details/gqjimuhlf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.yfazqb.com/Article/details/gbauwfmnw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gezcxdwaw.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/gsacsvfjk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/gynqugbzr.sHtML

Go:   // 手写循环
来源：http://mobile.vehdjk.com/Article/details/gmjiefdfq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gyauwehxb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.bbcook.cn/Article/details/gmzjlpbld.sHtML

[D15] 去重
来源：http://m.share.vehdjk.com/Article/details/gkdjsshuj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/giliewzjr.sHtML

PHP:  array_unique($arr);
来源：http://mobile.vehdjk.com/Article/details/gdeaprmha.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gnscehcjh.sHtML

TS:   [...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gmsujhial.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.tarul.cn/Article/details/gbpfeorhc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.epnwcf.com/Article/details/gblgudshi.sHtML

Ruby: arr.uniq
来源：http://www.blog.sjlbkw.cn/Article/details/gcmrfjlmv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gusmitfgk.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/gqumhoaju.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gfgditudn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.tarul.cn/Article/details/gwyvnxnlw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gxxmmtziu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gpcausifl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.epnwcf.com/Article/details/gavrgazji.sHtML

Go:   // 手写循环累加
来源：http://baike.bbcook.cn/Article/details/guhsyoyxn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.vehdjk.com/Article/details/guvcwwjjh.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.sjlbkw.cn/Article/details/gdhukxnfe.sHtML

[D17] 最大值与最小值
来源：http://m.share.vehdjk.com/Article/details/gizmolthz.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.bbcook.cn/Article/details/gszuxbuns.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.tarul.cn/Article/details/gljpsivqv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.bbcook.cn/Article/details/gvdzecpvd.sHtML

TS:   Math.max(...arr);
来源：http://www.share.sjlbkw.cn/Article/details/gibvawcvc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.tarul.cn/Article/details/gtbsbdmmt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.epnwcf.com/Article/details/gamexnjui.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.yfazqb.com/Article/details/ganqzyxii.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/gagkgfavm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.tarul.cn/Article/details/gktpupxbc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.epnwcf.com/Article/details/gntxrlqdc.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.yfazqb.com/Article/details/gxitejkcg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.bbcook.cn/Article/details/gvbpuextg.sHtML

TS:   nested.flat();
来源：http://www.share.sjlbkw.cn/Article/details/gnddmwtmr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.tarul.cn/Article/details/gkavisrjc.sHtML

Go:   // 手写双层循环
来源：http://blog.fktsv.cn/Article/details/gehfjddko.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fktsv.cn/Article/details/gwnhtvqgg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fktsv.cn/Article/details/gyuynkzrt.sHtML

[D19] 按字段分组
来源：http://www.share.epnwcf.com/Article/details/gkjumfyrv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fktsv.cn/Article/details/gasznsvwu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.epnwcf.com/Article/details/gljfkbjdm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.tarul.cn/Article/details/gqfaqiroe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.epnwcf.com/Article/details/gatvlygie.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.bbcook.cn/Article/details/guoztwmox.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.bbcook.cn/Article/details/gibamiatb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.vehdjk.com/Article/details/gtvmbovhu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.sjlbkw.cn/Article/details/gzewewzgl.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.vehdjk.com/Article/details/gdjssaafx.sHtML

Py:   Counter(arr)
来源：http://blog.tarul.cn/Article/details/gdcqqhkho.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.bbcook.cn/Article/details/gwoxwsicn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gqgxoawib.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/gukotwhiw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.epnwcf.com/Article/details/gpzuhcknn.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.bbcook.cn/Article/details/gevgjxyrs.sHtML

Ruby: arr.tally
来源：http://3g.epnwcf.com/Article/details/gwgexzexn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.epnwcf.com/Article/details/gekxzdocm.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.epnwcf.com/Article/details/gbdcuoapy.sHtML

Py:   x in arr
来源：http://blog.bbcook.cn/Article/details/gufvzyeko.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.sjlbkw.cn/Article/details/gstpmgilo.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gzutiwmjs.sHtML

TS:   arr.includes(x)
来源：http://www.share.yfazqb.com/Article/details/gdqaufnyy.sHtML

Java: list.contains(x)
来源：http://read.share.fktsv.cn/Article/details/ggajwcwtu.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.epnwcf.com/Article/details/gfffwehjb.sHtML

Ruby: arr.include?(x)
来源：http://www.share.bbcook.cn/Article/details/gbsxeyfat.sHtML

C#:   list.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gpbzpaijv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.vehdjk.com/Article/details/gbxpraeqr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.yfazqb.com/Article/details/ghyekpalf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.tarul.cn/Article/details/giowwdrmb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/goezgcccu.sHtML

TS:   [...arr];
来源：http://baike.epnwcf.com/Article/details/gzjhkycci.sHtML

Java: new ArrayList<>(list);
来源：http://blog.sjlbkw.cn/Article/details/gnqehkfrb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.epnwcf.com/Article/details/gtuluxfor.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.tarul.cn/Article/details/gziixtatj.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gvhjsebsd.sHtML


<!-- 参考信息 -->