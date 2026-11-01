代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://baike.vehdjk.com/Article/details/gvvunuypc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/gdbdrwgcn.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/gxsodxefs.sHtML

[C05] 返回多个值
来源：http://mobile.tarul.cn/Article/details/gktyhwaia.sHtML

Py:   return a, b
来源：http://www.blog.vehdjk.com/Article/details/godpciprw.sHtML

PHP:  return [$a, $b];
来源：http://m.share.bbcook.cn/Article/details/gnjtnuplj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.vehdjk.com/Article/details/gyifrartf.sHtML

TS:   return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gcxjqqvnj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fktsv.cn/Article/details/gtnukidhp.sHtML

Go:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gtucxzjkq.sHtML

Ruby: return a, b
来源：http://mobile.sjlbkw.cn/Article/details/glhdzgfcv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fktsv.cn/Article/details/gwiayiivv.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.sjlbkw.cn/Article/details/gxlchmhbz.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.bbcook.cn/Article/details/ghgbueary.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.sjlbkw.cn/Article/details/gnnufltrw.sHtML

JS:   const square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/gnuplncxw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gqppjabgv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/gzqaskepd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.bbcook.cn/Article/details/gzjijqlub.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.yfazqb.com/Article/details/gkmjlqbqy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/gijlyicbb.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.bbcook.cn/Article/details/gzvdyuope.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.yfazqb.com/Article/details/gmimjmdel.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fktsv.cn/Article/details/geegthart.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.bbcook.cn/Article/details/gemmoowxc.sHtML

TS:   arr.map(String)
来源：http://www.m.share.bbcook.cn/Article/details/gxilqfqwt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.tarul.cn/Article/details/goxjplnhf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.tarul.cn/Article/details/gpkbinkyu.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.tarul.cn/Article/details/gpwdrsrrp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.yfazqb.com/Article/details/ggzdcbllr.sHtML

[C08] 闭包
来源：http://m.share.tarul.cn/Article/details/gqbbvyhtb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fktsv.cn/Article/details/gvjcslptf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.yfazqb.com/Article/details/gnzkpugod.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gmovsehnb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gaadyeuvy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.vehdjk.com/Article/details/gmmpvmowf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.tarul.cn/Article/details/gvixraxvm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.bbcook.cn/Article/details/gialhcqam.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gljegaqls.sHtML

[C09] 递归
来源：http://m.share.epnwcf.com/Article/details/gvvlexbky.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gbmdnbplr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.yfazqb.com/Article/details/ghhvmoazt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/glqgytmxn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/guhtxnnau.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gemsuewtf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.vehdjk.com/Article/details/gssmcovfo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gpruyvfkp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.bbcook.cn/Article/details/gszhrzfwg.sHtML

[C10] 变量作用域
来源：http://read.share.fktsv.cn/Article/details/gkungwokn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.sjlbkw.cn/Article/details/ggkygepen.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.yfazqb.com/Article/details/gbdzuskgr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.epnwcf.com/Article/details/gfmjezljh.sHtML

TS:   同 JS
来源：http://wap.epnwcf.com/Article/details/gtngbnfpf.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gypzxycgd.sHtML

Go:   花括号块级作用域
来源：http://wap.vehdjk.com/Article/details/gozmjrcxy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.sjlbkw.cn/Article/details/gmrdqibtg.sHtML

C#:   块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gjsvtlumv.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.epnwcf.com/Article/details/gynkfwqbb.sHtML

Py:   from module import func
来源：http://www.blog.epnwcf.com/Article/details/gcsujjkxh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.bbcook.cn/Article/details/gkqannpkm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fktsv.cn/Article/details/grtnjegsw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.yfazqb.com/Article/details/gaekunhhk.sHtML

Java: import java.util.List;
来源：http://mobile.vehdjk.com/Article/details/guljceqja.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.vehdjk.com/Article/details/gmtnyarjx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.sjlbkw.cn/Article/details/gcsclvimv.sHtML

C#:   using System.Text;
来源：http://www.m.share.vehdjk.com/Article/details/gfixbkfon.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.bbcook.cn/Article/details/gaomzywzn.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.epnwcf.com/Article/details/gmcggnlor.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.bbcook.cn/Article/details/gctygoqqe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fktsv.cn/Article/details/gucamadnl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.vehdjk.com/Article/details/gucqzqcqr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.vehdjk.com/Article/details/gpvtufimq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.epnwcf.com/Article/details/gzuefgfbi.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.yfazqb.com/Article/details/gcbunexqz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.vehdjk.com/Article/details/gmmfxysds.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fktsv.cn/Article/details/gzldtuhcr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.bbcook.cn/Article/details/goziwuzmc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gwatxhebn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.tarul.cn/Article/details/ggzvxbddu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gykuywibl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gmrebjyia.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fktsv.cn/Article/details/geqmnyjmq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.sjlbkw.cn/Article/details/gfgbgxnej.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.sjlbkw.cn/Article/details/gfqddtyss.sHtML

[C14] 泛型函数
来源：http://3g.epnwcf.com/Article/details/gcochhavb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.bbcook.cn/Article/details/geqyvfaoj.sHtML

PHP:  // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gsxbpbler.sHtML

JS:   // 无泛型
来源：http://blog.fktsv.cn/Article/details/gsbujuddh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.epnwcf.com/Article/details/gijvheqxc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.epnwcf.com/Article/details/gytnjeejx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.epnwcf.com/Article/details/gelutccby.sHtML

Ruby: # 无泛型
来源：http://blog.bbcook.cn/Article/details/ghbougzud.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.epnwcf.com/Article/details/gfpqbnksz.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.yfazqb.com/Article/details/gnaaoacsi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.tarul.cn/Article/details/gdilmyrmw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.bbcook.cn/Article/details/glzurrakd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gddsdiltt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.bbcook.cn/Article/details/gmzihpyzz.sHtML

Java: // 无解构
来源：http://m.share.fktsv.cn/Article/details/gbcwwmukn.sHtML

Go:   // 无解构
来源：http://wap.yfazqb.com/Article/details/gfcduoenh.sHtML

Ruby: a, b = pair
来源：http://read.share.fktsv.cn/Article/details/gzcxtsuev.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fktsv.cn/Article/details/gwvbglkjq.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fktsv.cn/Article/details/gikebjrjz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.epnwcf.com/Article/details/gqwdloojd.sHtML

PHP:  // 无重载
来源：http://blog.tarul.cn/Article/details/gjytfpjpw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.bbcook.cn/Article/details/gzfrzlaxy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.vehdjk.com/Article/details/gdaqptxjo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.yfazqb.com/Article/details/gbdonurdu.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fktsv.cn/Article/details/gkifguern.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.epnwcf.com/Article/details/grhhustju.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.vehdjk.com/Article/details/gcboqvykt.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjbswdtnf.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.bbcook.cn/Article/details/gwqxorwpr.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gsgobtnzf.sHtML

[D01] 创建数组 / 列表
来源：http://baike.tarul.cn/Article/details/gyjnhthny.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.vehdjk.com/Article/details/gbzscbpxm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.epnwcf.com/Article/details/gsnyxdqqz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.yfazqb.com/Article/details/gbmauzeqq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fktsv.cn/Article/details/gftklrdes.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.epnwcf.com/Article/details/gqmacgfmv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.bbcook.cn/Article/details/gwptwqyls.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.yfazqb.com/Article/details/gkwerqefj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fktsv.cn/Article/details/guhnwzsqd.sHtML

[D02] 追加元素到末尾
来源：http://3g.tarul.cn/Article/details/gjuwdxszv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.vehdjk.com/Article/details/gmzilhmio.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.sjlbkw.cn/Article/details/gnijmedfc.sHtML

JS:   arr.push(4);
来源：http://www.share.bbcook.cn/Article/details/guwwqkywh.sHtML

TS:   arr.push(4);
来源：http://mobile.fktsv.cn/Article/details/guejmnlgv.sHtML

Java: list.add(4);
来源：http://blog.epnwcf.com/Article/details/gbqslefex.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fktsv.cn/Article/details/gzbfukucl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.yfazqb.com/Article/details/gefyamgmu.sHtML

C#:   list.Add(4);
来源：http://mobile.sjlbkw.cn/Article/details/gviwdpsru.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.yfazqb.com/Article/details/gqwfrhoxt.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fktsv.cn/Article/details/gwlyawwsw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.sjlbkw.cn/Article/details/gfrjcjiml.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.bbcook.cn/Article/details/gdlleaxgb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.yfazqb.com/Article/details/guppgevqv.sHtML

Java: list.add(0, 0);
来源：http://wap.epnwcf.com/Article/details/gzsxmsrnd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.yfazqb.com/Article/details/giuqbbovt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fktsv.cn/Article/details/gwibyqjqi.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gifaqmkzs.sHtML

[D04] 删除元素
来源：http://www.blog.bbcook.cn/Article/details/gptvviorz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fktsv.cn/Article/details/gvwwqltkv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.tarul.cn/Article/details/gtbdadwjj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.yfazqb.com/Article/details/gwkybaaag.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.vehdjk.com/Article/details/glmbojqqw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.vehdjk.com/Article/details/gulxtefxb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.vehdjk.com/Article/details/gavtvtcjc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.tarul.cn/Article/details/gdkytoexd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.vehdjk.com/Article/details/gnqkbzmhf.sHtML

[D05] 访问与修改元素
来源：http://m.share.epnwcf.com/Article/details/glnkvqnuk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gqnuzmfuq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gkwvrsxap.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/gaipprvof.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.tarul.cn/Article/details/ghywwyxup.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.sjlbkw.cn/Article/details/gyyfwyusq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gzrscttle.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gmbhmnymy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gjnweeknq.sHtML

[D06] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/gyzkxkkcg.sHtML

Py:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gpoahlfsf.sHtML

PHP:  count($arr);
来源：http://baike.vehdjk.com/Article/details/gchcvoxru.sHtML

JS:   arr.length
来源：http://3g.bbcook.cn/Article/details/gbwkgtenj.sHtML

TS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gmbehomkd.sHtML

Java: list.size();
来源：http://wap.bbcook.cn/Article/details/gdylxkvqy.sHtML

Go:   len(arr)
来源：http://read.share.yfazqb.com/Article/details/guxltghzq.sHtML

Ruby: arr.length; arr.size
来源：http://blog.sjlbkw.cn/Article/details/giqkkdnpn.sHtML

C#:   list.Count;
来源：http://baike.tarul.cn/Article/details/ggifrcsqe.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.tarul.cn/Article/details/gnylpjbwd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fktsv.cn/Article/details/guoykwuwa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.bbcook.cn/Article/details/ghkmbssyc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gumyktqfr.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fktsv.cn/Article/details/gdlxwrzuw.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpskfebx.sHtML

Go:   arr[1:4]
来源：http://mobile.sjlbkw.cn/Article/details/gzwdzxaqc.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.tarul.cn/Article/details/gxomyqted.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.tarul.cn/Article/details/gmixoefki.sHtML

[D08] 合并两个数组
来源：http://wap.yfazqb.com/Article/details/gpjgsgppu.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.yfazqb.com/Article/details/guozrfvcv.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fktsv.cn/Article/details/gjigylako.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.bbcook.cn/Article/details/gojhackrz.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.bbcook.cn/Article/details/gixmcbqbu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.tarul.cn/Article/details/gvzkftwnx.sHtML

Go:   append(a, b...)
来源：http://blog.fktsv.cn/Article/details/gbcxvjvsz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.bbcook.cn/Article/details/gkbfnprhh.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.bbcook.cn/Article/details/gjacnyrdy.sHtML

[D09] 排序（升序）
来源：http://baike.sjlbkw.cn/Article/details/gnjducjqg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/gymmjscvk.sHtML

PHP:  sort($arr);
来源：http://mobile.bbcook.cn/Article/details/ggecvdlii.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.tarul.cn/Article/details/glpilymep.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.bbcook.cn/Article/details/gtdhlitju.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.sjlbkw.cn/Article/details/glxjnlmyz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/glnhazugy.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/gsfkejgzz.sHtML

C#:   list.Sort();
来源：http://blog.bbcook.cn/Article/details/ghbwjxnwt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.bbcook.cn/Article/details/ghsdbgvrf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fktsv.cn/Article/details/gafwupicx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.yfazqb.com/Article/details/gggrpwqzm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.vehdjk.com/Article/details/gwlunnyrg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fktsv.cn/Article/details/gemenqdda.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.bbcook.cn/Article/details/gmheattpa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.epnwcf.com/Article/details/gcjbhqhmy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.vehdjk.com/Article/details/gmcgnpkrf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.yfazqb.com/Article/details/gzobmdbwi.sHtML

[D11] 反转数组
来源：http://read.share.bbcook.cn/Article/details/glbslkroy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.epnwcf.com/Article/details/gylhnnkoo.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.epnwcf.com/Article/details/ghovubnqt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.tarul.cn/Article/details/gjbsyjpbi.sHtML

TS:   [...arr].reverse();
来源：http://mobile.epnwcf.com/Article/details/gmvqlklir.sHtML

Java: Collections.reverse(list);
来源：http://3g.epnwcf.com/Article/details/gtmnfaulo.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.epnwcf.com/Article/details/gsqquleyo.sHtML

Ruby: arr.reverse
来源：http://3g.fktsv.cn/Article/details/gdiadumel.sHtML

C#:   list.Reverse();
来源：http://wap.vehdjk.com/Article/details/gwzlmtoly.sHtML

[D12] 查找元素下标
来源：http://read.share.vehdjk.com/Article/details/gnclqoelf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.sjlbkw.cn/Article/details/gfekyecec.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.tarul.cn/Article/details/gmnugzisw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gmbtsnwpc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gesyrjned.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.sjlbkw.cn/Article/details/gcrwbqwfp.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gmrjrazxj.sHtML

Ruby: arr.index(x)
来源：http://www.share.epnwcf.com/Article/details/gwjlpbwit.sHtML

C#:   list.IndexOf(x);
来源：http://blog.yfazqb.com/Article/details/gzqyckznb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/gglxouytx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/grzeklibw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.bbcook.cn/Article/details/ghtnanjrs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.bbcook.cn/Article/details/gazpanslw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.sjlbkw.cn/Article/details/gddfbsfpw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.sjlbkw.cn/Article/details/gzftadamd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/goliweotv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.vehdjk.com/Article/details/gnifyzwck.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.bbcook.cn/Article/details/ggeggyxnu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.bbcook.cn/Article/details/ggfpmjrxg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gsnzqrklr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.tarul.cn/Article/details/grvnazpvk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.tarul.cn/Article/details/gthxonsxt.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/gfrugxsje.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.bbcook.cn/Article/details/gkjvuswys.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gkrialahc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.bbcook.cn/Article/details/gttrziwbq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.bbcook.cn/Article/details/gynzniear.sHtML

[D15] 去重
来源：http://www.blog.vehdjk.com/Article/details/gnfhfduhm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gpmwzvzfi.sHtML

PHP:  array_unique($arr);
来源：http://wap.tarul.cn/Article/details/gymvqolvp.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gmfgkrott.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/gkfoywbpe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.vehdjk.com/Article/details/grzeneohx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.yfazqb.com/Article/details/glgqcgcwp.sHtML

Ruby: arr.uniq
来源：http://mobile.epnwcf.com/Article/details/gytzctzes.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.epnwcf.com/Article/details/gqqiprkiy.sHtML

[D16] 求和与平均值
来源：http://www.share.vehdjk.com/Article/details/giwfzozcu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.epnwcf.com/Article/details/gnkxiyrrz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.yfazqb.com/Article/details/gblibkarp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/gmsvjajkt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gwvvbyeqn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.tarul.cn/Article/details/gvnogdyem.sHtML

Go:   // 手写循环累加
来源：http://www.share.bbcook.cn/Article/details/ggzdrspuk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.sjlbkw.cn/Article/details/govcckvdu.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.bbcook.cn/Article/details/ganaskspy.sHtML

[D17] 最大值与最小值
来源：http://mobile.yfazqb.com/Article/details/gtewhnfnn.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.bbcook.cn/Article/details/grfrhgomd.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.sjlbkw.cn/Article/details/ghjnlawaq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.epnwcf.com/Article/details/gehjdyskq.sHtML

TS:   Math.max(...arr);
来源：http://www.share.bbcook.cn/Article/details/gtdllobuz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.yfazqb.com/Article/details/gzdqzecep.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.tarul.cn/Article/details/gzmtbswsx.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.sjlbkw.cn/Article/details/gfvflthug.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fktsv.cn/Article/details/gbztdfatb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.vehdjk.com/Article/details/geukbuggm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.epnwcf.com/Article/details/gktlpthrc.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.bbcook.cn/Article/details/glaeedodz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.vehdjk.com/Article/details/gwoyyzeud.sHtML

TS:   nested.flat();
来源：http://read.share.fktsv.cn/Article/details/gfvgijizt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.epnwcf.com/Article/details/gygunzsak.sHtML

Go:   // 手写双层循环
来源：http://read.share.tarul.cn/Article/details/goecfvcpv.sHtML

Ruby: nested.flatten
来源：http://m.share.tarul.cn/Article/details/gzcthpbra.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.tarul.cn/Article/details/gzxcbpqcg.sHtML

[D19] 按字段分组
来源：http://m.share.tarul.cn/Article/details/gqggiofdd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.bbcook.cn/Article/details/geatecizo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.vehdjk.com/Article/details/gwxorjxiq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.yfazqb.com/Article/details/gfcibtjud.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gzbwbjrtd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fktsv.cn/Article/details/grpypkayy.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.yfazqb.com/Article/details/ghkhmbcwv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.sjlbkw.cn/Article/details/gcafgaamb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.tarul.cn/Article/details/gbcsrzqnz.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.bbcook.cn/Article/details/gdbxrwzgf.sHtML

Py:   Counter(arr)
来源：http://www.blog.vehdjk.com/Article/details/gfmdiaiel.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.tarul.cn/Article/details/gzdozbxee.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gxeavpjpm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gitmpodxx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.tarul.cn/Article/details/ghezckvbm.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.sjlbkw.cn/Article/details/gktkbcjuj.sHtML

Ruby: arr.tally
来源：http://baike.epnwcf.com/Article/details/gxqncycgq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.yfazqb.com/Article/details/gumqjzbal.sHtML

[D21] 判断是否包含某元素
来源：http://baike.vehdjk.com/Article/details/gbihhygta.sHtML

Py:   x in arr
来源：http://3g.epnwcf.com/Article/details/gxlaznpqh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.tarul.cn/Article/details/gdyuoldga.sHtML

JS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/gdyvoulzg.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gjjxwlugf.sHtML

Java: list.contains(x)
来源：http://www.m.share.tarul.cn/Article/details/ggnsgwsso.sHtML


<!-- 参考信息 -->