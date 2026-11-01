代发 wailian999

Py:   return a, b
来源：http://www.share.tarul.cn/Article/details/gqnrlxwqr.sHtML

PHP:  return [$a, $b];
来源：http://3g.bbcook.cn/Article/details/gkcraozbt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.vehdjk.com/Article/details/gvbqicifp.sHtML

TS:   return { a, b };
来源：http://baike.fktsv.cn/Article/details/gwrchguei.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.bbcook.cn/Article/details/gvlwyxbkp.sHtML

Go:   return a, b
来源：http://3g.fktsv.cn/Article/details/gygkoefwg.sHtML

Ruby: return a, b
来源：http://wap.fktsv.cn/Article/details/gldirbxzb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.sjlbkw.cn/Article/details/gpanyhzok.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fktsv.cn/Article/details/gxkewlzpp.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.tarul.cn/Article/details/gkybtrheg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.vehdjk.com/Article/details/gaxnfhhwu.sHtML

JS:   const square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/gidbdlkaq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.bbcook.cn/Article/details/gnwgkwfks.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gpgedllgr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.tarul.cn/Article/details/gzywkzhwj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.epnwcf.com/Article/details/gijohlteg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gyuwvswye.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.yfazqb.com/Article/details/ghjqmrtht.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.bbcook.cn/Article/details/gpbbpjifc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.bbcook.cn/Article/details/gkoashtlh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.bbcook.cn/Article/details/gbviusbec.sHtML

TS:   arr.map(String)
来源：http://baike.tarul.cn/Article/details/gbbjnpwja.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gqevtzmcf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.epnwcf.com/Article/details/gpknnpala.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.sjlbkw.cn/Article/details/gkfacwglo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.epnwcf.com/Article/details/geezhliax.sHtML

[C08] 闭包
来源：http://www.share.yfazqb.com/Article/details/gtaxaudol.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.epnwcf.com/Article/details/gmnohpmfz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.yfazqb.com/Article/details/gfcytbanx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gxkfvnlos.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gnllipvsm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.yfazqb.com/Article/details/grsksetkf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fktsv.cn/Article/details/gopebbwro.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.tarul.cn/Article/details/geqnygoxx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gjqbvrnri.sHtML

[C09] 递归
来源：http://mobile.fktsv.cn/Article/details/gzkpkqjkf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/guujywfpi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.vehdjk.com/Article/details/gasjzcbll.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/gomoazugj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/grckbdpst.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.tarul.cn/Article/details/gnjgzjise.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.epnwcf.com/Article/details/gtwehqyff.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.epnwcf.com/Article/details/grnytsgnx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fktsv.cn/Article/details/gqxtwsqnu.sHtML

[C10] 变量作用域
来源：http://www.m.share.bbcook.cn/Article/details/glhjtriyt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.vehdjk.com/Article/details/guetkdvlw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fktsv.cn/Article/details/gejxmjqxu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fktsv.cn/Article/details/gxvdrrawu.sHtML

TS:   同 JS
来源：http://wap.tarul.cn/Article/details/gefqjgbkz.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.epnwcf.com/Article/details/gsxfrequr.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gkceltmed.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.vehdjk.com/Article/details/gzadczoer.sHtML

C#:   块级作用域
来源：http://m.share.tarul.cn/Article/details/gwaymysgx.sHtML

[C11] 模块导入与导出
来源：http://read.share.yfazqb.com/Article/details/gfoxsuobs.sHtML

Py:   from module import func
来源：http://www.m.share.tarul.cn/Article/details/gzottqqlh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fktsv.cn/Article/details/gjrzcinqg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.epnwcf.com/Article/details/ganiodsel.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.yfazqb.com/Article/details/gipfzbmwx.sHtML

Java: import java.util.List;
来源：http://www.share.yfazqb.com/Article/details/gvpemyxkq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.yfazqb.com/Article/details/goivslwob.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fktsv.cn/Article/details/gtrijsxwk.sHtML

C#:   using System.Text;
来源：http://baike.tarul.cn/Article/details/gaemvjpxa.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.bbcook.cn/Article/details/gtrumjuma.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.yfazqb.com/Article/details/gqiztjrte.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.sjlbkw.cn/Article/details/gqstpcqbd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gxdqgokkl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/gstiaszch.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.sjlbkw.cn/Article/details/gtyqfuowt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.epnwcf.com/Article/details/gfdljyqot.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fktsv.cn/Article/details/gxzixqvhn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.vehdjk.com/Article/details/gelfpffps.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.bbcook.cn/Article/details/gpcgaqzxj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.vehdjk.com/Article/details/gpfhjmznr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gniqdmdjp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.vehdjk.com/Article/details/gurligzwn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gyorbcqtx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gqhzolehk.sHtML

Go:   func add(a, b int) int
来源：http://baike.bbcook.cn/Article/details/guvpqygzu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.sjlbkw.cn/Article/details/gbidxehip.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.epnwcf.com/Article/details/ggnhwtyny.sHtML

[C14] 泛型函数
来源：http://read.share.epnwcf.com/Article/details/gwgpiqstl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fktsv.cn/Article/details/ghbtsmjcg.sHtML

PHP:  // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/glexmcdep.sHtML

JS:   // 无泛型
来源：http://m.share.yfazqb.com/Article/details/gjjaczvoc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.vehdjk.com/Article/details/ggfkzvdgt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/giddwnocj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.tarul.cn/Article/details/gcbyuzwoz.sHtML

Ruby: # 无泛型
来源：http://www.blog.epnwcf.com/Article/details/glipzphlf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.epnwcf.com/Article/details/gdagupjof.sHtML

[C15] 解构 / 展开参数
来源：http://blog.sjlbkw.cn/Article/details/gamhdkiqc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.yfazqb.com/Article/details/gscpwzyig.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fktsv.cn/Article/details/ghywbgqrc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.sjlbkw.cn/Article/details/gqvvyorlb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fktsv.cn/Article/details/gmisdnwpc.sHtML

Java: // 无解构
来源：http://m.share.epnwcf.com/Article/details/gbcbcvcrv.sHtML

Go:   // 无解构
来源：http://www.blog.vehdjk.com/Article/details/gvzbluzma.sHtML

Ruby: a, b = pair
来源：http://wap.tarul.cn/Article/details/gipwawzjp.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.bbcook.cn/Article/details/giubyqmrs.sHtML

[C16] 函数 / 方法重载
来源：http://baike.yfazqb.com/Article/details/gfznpvwhe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.yfazqb.com/Article/details/gouxepzef.sHtML

PHP:  // 无重载
来源：http://wap.fktsv.cn/Article/details/gsnvmxhyn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fktsv.cn/Article/details/gncmssxcj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.yfazqb.com/Article/details/gejwodegx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.yfazqb.com/Article/details/ghetbbpwo.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.epnwcf.com/Article/details/gtgivycqv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.tarul.cn/Article/details/geviwpgqk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.bbcook.cn/Article/details/gotjvbddc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gemfmlfuq.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.sjlbkw.cn/Article/details/gdcudfaim.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gplqvywbd.sHtML

[D01] 创建数组 / 列表
来源：http://blog.sjlbkw.cn/Article/details/geutmzbtf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.tarul.cn/Article/details/gdfbrkkkd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fktsv.cn/Article/details/gthhwwcht.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.tarul.cn/Article/details/gsjmouhxs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.sjlbkw.cn/Article/details/gacneyobg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.yfazqb.com/Article/details/gmerminpk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/gdmkuyzwy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.bbcook.cn/Article/details/gmnrjjvdf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.sjlbkw.cn/Article/details/gfjjybcqe.sHtML

[D02] 追加元素到末尾
来源：http://m.share.epnwcf.com/Article/details/gbcvshcmu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.yfazqb.com/Article/details/glmtydsgh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fktsv.cn/Article/details/grnwomhgo.sHtML

JS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/gqmzgdzhe.sHtML

TS:   arr.push(4);
来源：http://wap.yfazqb.com/Article/details/gymohmvzy.sHtML

Java: list.add(4);
来源：http://3g.yfazqb.com/Article/details/girpezsap.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.yfazqb.com/Article/details/gzemphsrl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.tarul.cn/Article/details/ggugohjwh.sHtML

C#:   list.Add(4);
来源：http://wap.yfazqb.com/Article/details/gwjwzbmxg.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fktsv.cn/Article/details/gdvzsomih.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.epnwcf.com/Article/details/guqqzzypb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.yfazqb.com/Article/details/gfqkrkrgj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.bbcook.cn/Article/details/gumwshfei.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.yfazqb.com/Article/details/ggqxypvvd.sHtML

Java: list.add(0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/glevzbfkd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.vehdjk.com/Article/details/gcnshqtwd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.yfazqb.com/Article/details/gbuqlcckh.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fktsv.cn/Article/details/glmgkdsaf.sHtML

[D04] 删除元素
来源：http://mobile.sjlbkw.cn/Article/details/ganmsjpyh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.sjlbkw.cn/Article/details/gkmyhgleq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.bbcook.cn/Article/details/grharcunh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.bbcook.cn/Article/details/gqeotclmq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.bbcook.cn/Article/details/gnaijnhch.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.bbcook.cn/Article/details/gkpzhuzhm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.yfazqb.com/Article/details/ggowpbkcj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.tarul.cn/Article/details/gnflkvqwx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.bbcook.cn/Article/details/gsgmuoicg.sHtML

[D05] 访问与修改元素
来源：http://www.share.tarul.cn/Article/details/gycchjums.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gcirhydms.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gidzsumba.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gqpvwbefm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.tarul.cn/Article/details/gwhtwqopi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.tarul.cn/Article/details/gbivappzb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gfilurcae.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gqxvelcvj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.tarul.cn/Article/details/gnyvvwphe.sHtML

[D06] 数组长度
来源：http://3g.tarul.cn/Article/details/ghmdkqlws.sHtML

Py:   len(arr)
来源：http://wap.bbcook.cn/Article/details/gdwslmjpe.sHtML

PHP:  count($arr);
来源：http://3g.fktsv.cn/Article/details/gucjgjnbb.sHtML

JS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gtwmftyqi.sHtML

TS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/gnycetlxr.sHtML

Java: list.size();
来源：http://3g.vehdjk.com/Article/details/gsrfwkmay.sHtML

Go:   len(arr)
来源：http://mobile.vehdjk.com/Article/details/gwjatzzzt.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fktsv.cn/Article/details/gvmgetquc.sHtML

C#:   list.Count;
来源：http://wap.bbcook.cn/Article/details/gymtvwezj.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.tarul.cn/Article/details/gtgsssaqw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.yfazqb.com/Article/details/gxmhttbya.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.yfazqb.com/Article/details/gnmcgsqyo.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/gokgwyrys.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fktsv.cn/Article/details/gbvflwduk.sHtML

Java: list.subList(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gojogrmmj.sHtML

Go:   arr[1:4]
来源：http://m.share.vehdjk.com/Article/details/gdztkwzsz.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fktsv.cn/Article/details/gubytcdzi.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gwfkznlwd.sHtML

[D08] 合并两个数组
来源：http://mobile.vehdjk.com/Article/details/gcfsgjsdx.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.tarul.cn/Article/details/glatxfobd.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fktsv.cn/Article/details/gyainusux.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.yfazqb.com/Article/details/gyagreobo.sHtML

TS:   [...a, ...b];
来源：http://www.share.tarul.cn/Article/details/gxsormtdq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fktsv.cn/Article/details/ghwrsqvqy.sHtML

Go:   append(a, b...)
来源：http://www.blog.vehdjk.com/Article/details/gozhpkxfh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.vehdjk.com/Article/details/gpmwwhguj.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fktsv.cn/Article/details/gofdqtele.sHtML

[D09] 排序（升序）
来源：http://3g.bbcook.cn/Article/details/gwzgceotn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gtbosfkab.sHtML

PHP:  sort($arr);
来源：http://www.blog.bbcook.cn/Article/details/gnukbdrue.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.tarul.cn/Article/details/goenhtehj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fktsv.cn/Article/details/ghckckgyu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.yfazqb.com/Article/details/gcljspplr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gbwdundfa.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gerfmtfft.sHtML

C#:   list.Sort();
来源：http://www.blog.epnwcf.com/Article/details/gxgbxwjhh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbknegrk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.epnwcf.com/Article/details/guaukjyvm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.vehdjk.com/Article/details/gmtfgmxno.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/gmahgucdb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/gyhzcdxou.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.yfazqb.com/Article/details/gyobxnpeg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fktsv.cn/Article/details/gskadbfoy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fktsv.cn/Article/details/glwajavdi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fktsv.cn/Article/details/gsdopwukf.sHtML

[D11] 反转数组
来源：http://www.m.share.vehdjk.com/Article/details/gqdanixrp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.vehdjk.com/Article/details/ghonznnht.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.epnwcf.com/Article/details/gwuvdsraw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.yfazqb.com/Article/details/ggssvfwoq.sHtML

TS:   [...arr].reverse();
来源：http://3g.bbcook.cn/Article/details/griucnnxv.sHtML

Java: Collections.reverse(list);
来源：http://read.share.bbcook.cn/Article/details/gbdranqqn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gubdbangv.sHtML

Ruby: arr.reverse
来源：http://www.blog.vehdjk.com/Article/details/giydhrasw.sHtML

C#:   list.Reverse();
来源：http://www.share.bbcook.cn/Article/details/gdlhjfkfk.sHtML

[D12] 查找元素下标
来源：http://mobile.bbcook.cn/Article/details/gudtrheac.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.bbcook.cn/Article/details/gbggrsefo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.tarul.cn/Article/details/gwhspuoyl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/gzpvjzysu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/ggjtmgghf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.bbcook.cn/Article/details/giletckra.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gdhhigiwr.sHtML

Ruby: arr.index(x)
来源：http://www.blog.epnwcf.com/Article/details/gwtzgmxce.sHtML

C#:   list.IndexOf(x);
来源：http://blog.bbcook.cn/Article/details/gurmwebyc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.epnwcf.com/Article/details/gtszqpfpj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fktsv.cn/Article/details/giyyjcaid.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.sjlbkw.cn/Article/details/gxjdrzlol.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.tarul.cn/Article/details/gfikbppvw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gmteiiqiz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.yfazqb.com/Article/details/gklobwxcw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.bbcook.cn/Article/details/gmqyulgsb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.epnwcf.com/Article/details/gvhorrdyx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.vehdjk.com/Article/details/gcaedlmcz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.vehdjk.com/Article/details/gdrbkkmzu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.vehdjk.com/Article/details/gowaobzko.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.epnwcf.com/Article/details/gortgqixe.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/gympofzgo.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.vehdjk.com/Article/details/gohbwwegb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.sjlbkw.cn/Article/details/gksevbesw.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gbivxetrx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gehuvngqt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.yfazqb.com/Article/details/gjenqnxyx.sHtML

[D15] 去重
来源：http://www.blog.tarul.cn/Article/details/gammcwtch.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.vehdjk.com/Article/details/gaywqovzw.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.bbcook.cn/Article/details/gbmlkbzph.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gbimmrfqj.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gozcwihmc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fktsv.cn/Article/details/ggqhbndld.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.vehdjk.com/Article/details/gbyngmtew.sHtML

Ruby: arr.uniq
来源：http://3g.epnwcf.com/Article/details/gebvvdnvy.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.yfazqb.com/Article/details/ggptyatwn.sHtML

[D16] 求和与平均值
来源：http://m.share.tarul.cn/Article/details/ggwediwes.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fktsv.cn/Article/details/gjopxskeq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.tarul.cn/Article/details/gxrfurgwl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gbzdibuwf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/ggvgtqapq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.tarul.cn/Article/details/gbqcrzblz.sHtML

Go:   // 手写循环累加
来源：http://mobile.fktsv.cn/Article/details/gvkfjdzqi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.sjlbkw.cn/Article/details/gpxikntjg.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/gpwagpbbv.sHtML

[D17] 最大值与最小值
来源：http://www.share.sjlbkw.cn/Article/details/gaqsbwpqn.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.epnwcf.com/Article/details/gfdbcmrtn.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.bbcook.cn/Article/details/gixonyjhv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.tarul.cn/Article/details/gzrqsbkji.sHtML

TS:   Math.max(...arr);
来源：http://baike.bbcook.cn/Article/details/glfcltakg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fktsv.cn/Article/details/gidugeecc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.epnwcf.com/Article/details/gaykfsxpq.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/gsrgxrcas.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.bbcook.cn/Article/details/gyvpnulfm.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/giuqpxyxb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.vehdjk.com/Article/details/grdddbcik.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.sjlbkw.cn/Article/details/gehxmkjay.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.sjlbkw.cn/Article/details/gnorowdef.sHtML

TS:   nested.flat();
来源：http://blog.bbcook.cn/Article/details/gkwuhirvq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.tarul.cn/Article/details/gejlajwnc.sHtML

Go:   // 手写双层循环
来源：http://m.share.tarul.cn/Article/details/gjimrltra.sHtML

Ruby: nested.flatten
来源：http://www.share.yfazqb.com/Article/details/gqgyrwxpn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gthyvqicm.sHtML

[D19] 按字段分组
来源：http://3g.yfazqb.com/Article/details/gbuiunmjc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.sjlbkw.cn/Article/details/gcxkvojkz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fktsv.cn/Article/details/gcecljztt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fktsv.cn/Article/details/glepiydeh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.sjlbkw.cn/Article/details/gxftumuch.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.tarul.cn/Article/details/gswyiojks.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.vehdjk.com/Article/details/gscsszouv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.yfazqb.com/Article/details/ghdfvffnu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.vehdjk.com/Article/details/guacxmsuc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.tarul.cn/Article/details/gsgmasyqg.sHtML

Py:   Counter(arr)
来源：http://www.share.bbcook.cn/Article/details/gpzlcnvtj.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gqlnajwrp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/ghawicggi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/gzpyvrdff.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fktsv.cn/Article/details/gfudusxxg.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.bbcook.cn/Article/details/gasvqtkvr.sHtML

Ruby: arr.tally
来源：http://www.share.tarul.cn/Article/details/ggdhpmtcv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/gpjlxdtuj.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.vehdjk.com/Article/details/gmqjprhyr.sHtML

Py:   x in arr
来源：http://m.share.yfazqb.com/Article/details/gjxyeswwj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/gpicmoose.sHtML

JS:   arr.includes(x)
来源：http://blog.bbcook.cn/Article/details/ghbhqdhau.sHtML

TS:   arr.includes(x)
来源：http://blog.yfazqb.com/Article/details/gaocbobdz.sHtML

Java: list.contains(x)
来源：http://www.share.vehdjk.com/Article/details/gfisygeqc.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gvtjuxahw.sHtML

Ruby: arr.include?(x)
来源：http://wap.sjlbkw.cn/Article/details/grnhxflph.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/glvsvqvdp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.bbcook.cn/Article/details/grggjlycu.sHtML


<!-- 参考信息 -->