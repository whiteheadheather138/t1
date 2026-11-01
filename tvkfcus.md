代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.yfazqb.com/Article/details/gatpixnaa.sHtML

[C03] 可变参数
来源：http://read.share.fktsv.cn/Article/details/grhnmmrqc.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.bbcook.cn/Article/details/gyejgggkj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.sjlbkw.cn/Article/details/gpykzvqpn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/gfzbyjtmq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/gojojqrzq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.vehdjk.com/Article/details/gcgvnsuuf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.bbcook.cn/Article/details/gvlayoqvs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.tarul.cn/Article/details/gfqfqffcb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.vehdjk.com/Article/details/gvapgevou.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.sjlbkw.cn/Article/details/gajtzqcgi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fktsv.cn/Article/details/gvgczsizn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.vehdjk.com/Article/details/gaysekblw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gqwiwqppc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.epnwcf.com/Article/details/gvmcpelsv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.vehdjk.com/Article/details/gomrfaugd.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.yfazqb.com/Article/details/gujgbjpcl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gvsrncxdj.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gnqhsdsub.sHtML

[C05] 返回多个值
来源：http://blog.sjlbkw.cn/Article/details/gssrmlesm.sHtML

Py:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gfkgqnavv.sHtML

PHP:  return [$a, $b];
来源：http://read.share.vehdjk.com/Article/details/gtxetedzz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.tarul.cn/Article/details/giudpmumh.sHtML

TS:   return { a, b };
来源：http://baike.fktsv.cn/Article/details/gcmrbuyso.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fktsv.cn/Article/details/gohpuekhj.sHtML

Go:   return a, b
来源：http://www.share.vehdjk.com/Article/details/gwbfxndsn.sHtML

Ruby: return a, b
来源：http://www.blog.tarul.cn/Article/details/gpfsdxhui.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.sjlbkw.cn/Article/details/goyerprpn.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.vehdjk.com/Article/details/gbviejyod.sHtML

Py:   square = lambda x: x * x
来源：http://blog.vehdjk.com/Article/details/gvbmixjmh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.yfazqb.com/Article/details/gvtlncmgm.sHtML

JS:   const square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/gxomkenco.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fktsv.cn/Article/details/grwowdtvr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.tarul.cn/Article/details/gbygvsggs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.sjlbkw.cn/Article/details/gvrpwqhru.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.epnwcf.com/Article/details/gbblfzfom.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gagmekkkr.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.vehdjk.com/Article/details/gxwljogto.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.sjlbkw.cn/Article/details/gnvlwknlp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gupztraia.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.epnwcf.com/Article/details/gzrxcrtin.sHtML

TS:   arr.map(String)
来源：http://www.m.share.yfazqb.com/Article/details/gedsxetbq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.epnwcf.com/Article/details/gdbcmnbmu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.yfazqb.com/Article/details/gvoqhhavc.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.yfazqb.com/Article/details/ghtzgrpwh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.bbcook.cn/Article/details/gaybejhgy.sHtML

[C08] 闭包
来源：http://m.share.bbcook.cn/Article/details/gjdpkqamu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.vehdjk.com/Article/details/gckpipjnp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.vehdjk.com/Article/details/gzvhczymv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gxbkugdxo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/glwvzczuy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.tarul.cn/Article/details/gtdgjfeyy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.bbcook.cn/Article/details/gklnjfrqc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.bbcook.cn/Article/details/gfhtnghqw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gkptbxrna.sHtML

[C09] 递归
来源：http://read.share.sjlbkw.cn/Article/details/gpuvgbfex.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.bbcook.cn/Article/details/garinjptd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fktsv.cn/Article/details/gmrriwbfo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gsxfedjtq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/gdhwyddcz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.epnwcf.com/Article/details/gxuijsqkv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.yfazqb.com/Article/details/gwhdzggls.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/gfnrkzqbq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.epnwcf.com/Article/details/gkqkqfzmo.sHtML

[C10] 变量作用域
来源：http://3g.bbcook.cn/Article/details/gxqlddtws.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fktsv.cn/Article/details/gssbhblvo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fktsv.cn/Article/details/gvwcjlwab.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.bbcook.cn/Article/details/grbokodzz.sHtML

TS:   同 JS
来源：http://blog.yfazqb.com/Article/details/ggxfyxmqw.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fktsv.cn/Article/details/gepwfvkjn.sHtML

Go:   花括号块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/grygxxiwi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/gsgrkppil.sHtML

C#:   块级作用域
来源：http://wap.vehdjk.com/Article/details/gdttdcmth.sHtML

[C11] 模块导入与导出
来源：http://read.share.sjlbkw.cn/Article/details/goyqbtgms.sHtML

Py:   from module import func
来源：http://www.share.yfazqb.com/Article/details/gwgloncow.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.epnwcf.com/Article/details/gyvjfphza.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gyhslbrab.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fktsv.cn/Article/details/ghlzjrkhf.sHtML

Java: import java.util.List;
来源：http://m.share.epnwcf.com/Article/details/gwqavvlms.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fktsv.cn/Article/details/gjmjcxnzm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/gpkoammte.sHtML

C#:   using System.Text;
来源：http://www.m.share.tarul.cn/Article/details/gpdlgllun.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.vehdjk.com/Article/details/gciqpvkhu.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fktsv.cn/Article/details/gosqpgygj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.sjlbkw.cn/Article/details/gjcvvkobn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/gpzonsgkr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/grhhmplxq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.tarul.cn/Article/details/gbkmuqqfd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fktsv.cn/Article/details/gjvpdqvmf.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.sjlbkw.cn/Article/details/gfykopxrv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fktsv.cn/Article/details/gmyrgvdtd.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.epnwcf.com/Article/details/gyaeeyjoj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.tarul.cn/Article/details/gdfgsjrpq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gtsgoinuk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fktsv.cn/Article/details/gezfnehje.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/gccvjkdbx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/ghhrzcbhk.sHtML

Go:   func add(a, b int) int
来源：http://baike.vehdjk.com/Article/details/ggugcgwco.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.yfazqb.com/Article/details/gbggsjnls.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.yfazqb.com/Article/details/gtrgsgfuj.sHtML

[C14] 泛型函数
来源：http://read.share.tarul.cn/Article/details/grvvoxuew.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.yfazqb.com/Article/details/gnzpurzgq.sHtML

PHP:  // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gdzvamvjn.sHtML

JS:   // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gwqppkwfb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.tarul.cn/Article/details/gtuqvqdje.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fktsv.cn/Article/details/gxcpsdatg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.vehdjk.com/Article/details/gjottwzla.sHtML

Ruby: # 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gfbrhqsoj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.sjlbkw.cn/Article/details/gatndhttf.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.yfazqb.com/Article/details/grjnvftxi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fktsv.cn/Article/details/grefzukvl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.bbcook.cn/Article/details/gpxpgnhjh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fktsv.cn/Article/details/gqkppowuk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.epnwcf.com/Article/details/gtpcihami.sHtML

Java: // 无解构
来源：http://wap.yfazqb.com/Article/details/gjagtvwpd.sHtML

Go:   // 无解构
来源：http://3g.vehdjk.com/Article/details/gxrwwmfvs.sHtML

Ruby: a, b = pair
来源：http://m.share.vehdjk.com/Article/details/gbzhspnyv.sHtML

C#:   var (a, b) = pair;
来源：http://baike.bbcook.cn/Article/details/gmdlwbwom.sHtML

[C16] 函数 / 方法重载
来源：http://baike.bbcook.cn/Article/details/gvjqxcpar.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.bbcook.cn/Article/details/gfagjmcwp.sHtML

PHP:  // 无重载
来源：http://blog.fktsv.cn/Article/details/guavlmfbn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.vehdjk.com/Article/details/gyypcdreg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.sjlbkw.cn/Article/details/gsaovqdmc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fktsv.cn/Article/details/grjxxzbds.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.sjlbkw.cn/Article/details/gezbfbtyl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fktsv.cn/Article/details/gvgqykkrg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.epnwcf.com/Article/details/gzdjomykh.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/getjgxxyo.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.bbcook.cn/Article/details/gxgcmbnxu.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/giiyoyoxx.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.epnwcf.com/Article/details/geuosdcda.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.yfazqb.com/Article/details/gbzevxdnr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.vehdjk.com/Article/details/glqqdaony.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.sjlbkw.cn/Article/details/gakhzvzdb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.tarul.cn/Article/details/gvmliukxs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.yfazqb.com/Article/details/glhriqrul.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.tarul.cn/Article/details/grilsxpnv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.bbcook.cn/Article/details/gfubsisbl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.sjlbkw.cn/Article/details/goschwwgy.sHtML

[D02] 追加元素到末尾
来源：http://mobile.yfazqb.com/Article/details/gpwkcnjea.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.tarul.cn/Article/details/giweqdbrl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.vehdjk.com/Article/details/gbyugtvvp.sHtML

JS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/geeybnqqy.sHtML

TS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gvlgrurjp.sHtML

Java: list.add(4);
来源：http://www.blog.vehdjk.com/Article/details/gtgtyzbos.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.yfazqb.com/Article/details/ghajsbfpd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fktsv.cn/Article/details/gqdtmdphm.sHtML

C#:   list.Add(4);
来源：http://mobile.fktsv.cn/Article/details/gyrmoleny.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.bbcook.cn/Article/details/grxwlmoqu.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.vehdjk.com/Article/details/gbbhtepyx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.sjlbkw.cn/Article/details/gnwkdgfdk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.sjlbkw.cn/Article/details/gozzeyxjz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/ghrjhuevh.sHtML

Java: list.add(0, 0);
来源：http://baike.vehdjk.com/Article/details/gsccewgiv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.sjlbkw.cn/Article/details/gszsjszuw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.epnwcf.com/Article/details/gktgzmozg.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.bbcook.cn/Article/details/gfrywyhqb.sHtML

[D04] 删除元素
来源：http://blog.yfazqb.com/Article/details/gcaergbtw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.bbcook.cn/Article/details/gjwxxaipz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fktsv.cn/Article/details/genwlwmfg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.vehdjk.com/Article/details/gyzhufrdi.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fktsv.cn/Article/details/guynlvbgp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.vehdjk.com/Article/details/ghggcgwwv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.epnwcf.com/Article/details/gjomtvooh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.epnwcf.com/Article/details/gzhdlltwk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fktsv.cn/Article/details/gmdsviqwb.sHtML

[D05] 访问与修改元素
来源：http://m.share.vehdjk.com/Article/details/gystgjjhl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gqczrgmgz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gzoywypkc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gnntxtdui.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.yfazqb.com/Article/details/gdnelunkt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.yfazqb.com/Article/details/gmsflayvl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/ghsofrjge.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhbdntay.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gutvayrpb.sHtML

[D06] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/ggsfusdtg.sHtML

Py:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gbjkczxrv.sHtML

PHP:  count($arr);
来源：http://wap.bbcook.cn/Article/details/gkjeeudgr.sHtML

JS:   arr.length
来源：http://read.share.vehdjk.com/Article/details/gblvmleef.sHtML

TS:   arr.length
来源：http://3g.vehdjk.com/Article/details/guuqmecbw.sHtML

Java: list.size();
来源：http://mobile.epnwcf.com/Article/details/gccpzcsdl.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gzucydoao.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fktsv.cn/Article/details/gkhnzbvtt.sHtML

C#:   list.Count;
来源：http://m.share.yfazqb.com/Article/details/geqjzzjml.sHtML

[D07] 切片 / 取子数组
来源：http://3g.yfazqb.com/Article/details/gqnrbdvds.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.yfazqb.com/Article/details/gquujbeol.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.tarul.cn/Article/details/goivkgzqt.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gfvtiebjb.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/guawccavr.sHtML

Java: list.subList(1, 4);
来源：http://baike.vehdjk.com/Article/details/gyltjxxks.sHtML

Go:   arr[1:4]
来源：http://www.share.bbcook.cn/Article/details/gpobenbdu.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.vehdjk.com/Article/details/gqlauclpy.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.vehdjk.com/Article/details/gsopoapjy.sHtML

[D08] 合并两个数组
来源：http://baike.vehdjk.com/Article/details/gnexmykfv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.vehdjk.com/Article/details/gzucwxvlm.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.vehdjk.com/Article/details/gphsowvbi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.tarul.cn/Article/details/gshliapzx.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.tarul.cn/Article/details/gzixebcit.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gyumbznwv.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fktsv.cn/Article/details/gzdubsmbf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.bbcook.cn/Article/details/gfnfeqkmr.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.yfazqb.com/Article/details/gqlydkxqh.sHtML

[D09] 排序（升序）
来源：http://3g.yfazqb.com/Article/details/gaoutvwgk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gnbpwkpcg.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fktsv.cn/Article/details/guxohnljh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fktsv.cn/Article/details/gsqyzpiho.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.vehdjk.com/Article/details/gssbnowye.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.yfazqb.com/Article/details/gnbtcwkor.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.epnwcf.com/Article/details/gbmsuhmyc.sHtML

Ruby: arr.sort
来源：http://m.share.vehdjk.com/Article/details/gkttlredr.sHtML

C#:   list.Sort();
来源：http://wap.fktsv.cn/Article/details/ggliawdam.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.yfazqb.com/Article/details/gqbqgqabs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.tarul.cn/Article/details/gyarbztsc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.yfazqb.com/Article/details/gqlzkwhsi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.bbcook.cn/Article/details/gnjlyefxx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gzzkexbgn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.epnwcf.com/Article/details/gcvgujuaw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.tarul.cn/Article/details/gshljjocq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.tarul.cn/Article/details/godtqwjjo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.vehdjk.com/Article/details/gqybtlmlt.sHtML

[D11] 反转数组
来源：http://m.share.tarul.cn/Article/details/grbklhjgk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.vehdjk.com/Article/details/ggknejppj.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.vehdjk.com/Article/details/gwajkgdxx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.sjlbkw.cn/Article/details/gpzwbicmj.sHtML

TS:   [...arr].reverse();
来源：http://www.share.vehdjk.com/Article/details/gveiihjia.sHtML

Java: Collections.reverse(list);
来源：http://read.share.vehdjk.com/Article/details/gwtwdregw.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.tarul.cn/Article/details/gessjqsok.sHtML

Ruby: arr.reverse
来源：http://wap.sjlbkw.cn/Article/details/gaknhiyzy.sHtML

C#:   list.Reverse();
来源：http://www.m.share.tarul.cn/Article/details/gkddxdajh.sHtML

[D12] 查找元素下标
来源：http://wap.tarul.cn/Article/details/geqecwqls.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.vehdjk.com/Article/details/gxhsixrgf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.vehdjk.com/Article/details/giqlaksdt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.sjlbkw.cn/Article/details/gtsozdlnt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/gnlktkpaw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.sjlbkw.cn/Article/details/gtctfzcll.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.vehdjk.com/Article/details/gehvcoygs.sHtML

Ruby: arr.index(x)
来源：http://www.share.vehdjk.com/Article/details/grmohqxiw.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.yfazqb.com/Article/details/gywsuijys.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fktsv.cn/Article/details/gtmfnvcjw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.yfazqb.com/Article/details/gjhgofobz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.bbcook.cn/Article/details/gkbhjwljv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/gozsjnkxd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.vehdjk.com/Article/details/gcmrsxapk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.yfazqb.com/Article/details/gujflvyuv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.tarul.cn/Article/details/grxxvrkrz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.epnwcf.com/Article/details/ghuutqdtb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/ghxxrkagv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.tarul.cn/Article/details/gtbeyxdts.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gqdaggcbt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gkaufvbdi.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/gopnzdcve.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/ghcjpbgbq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gkitqnwzi.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/gjfwdjrrb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gumctkvhd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.bbcook.cn/Article/details/gkhyhdizz.sHtML

[D15] 去重
来源：http://baike.sjlbkw.cn/Article/details/gvsrsxgwo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/gxdonitvz.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fktsv.cn/Article/details/gcmvehkbu.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gskisgyfo.sHtML

TS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gvgprntxx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fktsv.cn/Article/details/giqtxquvm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fktsv.cn/Article/details/gqdgdpgfb.sHtML

Ruby: arr.uniq
来源：http://www.m.share.yfazqb.com/Article/details/gpgftbzff.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fktsv.cn/Article/details/gykjphabz.sHtML

[D16] 求和与平均值
来源：http://wap.vehdjk.com/Article/details/geuqnktny.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/glhzezzdk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.yfazqb.com/Article/details/gwqliqcfc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/gnpltupzk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/gkqoyxeiz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.vehdjk.com/Article/details/glsfqhexe.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.epnwcf.com/Article/details/gerigkbhf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.tarul.cn/Article/details/gdykglgbq.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fktsv.cn/Article/details/gkbyaqbku.sHtML

[D17] 最大值与最小值
来源：http://m.share.sjlbkw.cn/Article/details/gejxgpbyf.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.tarul.cn/Article/details/gyxubwcxp.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.yfazqb.com/Article/details/gvfjmbisr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fktsv.cn/Article/details/gkdvwirab.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/gjzhaondv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.bbcook.cn/Article/details/gdyhoqxbj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.bbcook.cn/Article/details/ghzdxkblf.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.yfazqb.com/Article/details/gjpvokwgq.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.sjlbkw.cn/Article/details/ggtgxvogr.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fktsv.cn/Article/details/gblcuxxov.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.sjlbkw.cn/Article/details/gsukmgdjb.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.sjlbkw.cn/Article/details/gfnuyfxyb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.bbcook.cn/Article/details/gbmcnwmxs.sHtML

TS:   nested.flat();
来源：http://baike.sjlbkw.cn/Article/details/gncpkmbte.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gyutgerud.sHtML

Go:   // 手写双层循环
来源：http://3g.vehdjk.com/Article/details/grueyntfa.sHtML

Ruby: nested.flatten
来源：http://mobile.bbcook.cn/Article/details/gzsdzjjta.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fktsv.cn/Article/details/ghutxsmjc.sHtML

[D19] 按字段分组
来源：http://mobile.fktsv.cn/Article/details/gstvubhil.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.sjlbkw.cn/Article/details/gcxsozpue.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.tarul.cn/Article/details/gizhokjww.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fktsv.cn/Article/details/ggwupmjdj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.tarul.cn/Article/details/grcpzsfgh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.tarul.cn/Article/details/gstuibnqb.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fktsv.cn/Article/details/gkwbsyatp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.yfazqb.com/Article/details/gdknxiysn.sHtML


<!-- 参考信息 -->