代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/gnlmaarue.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gjusbvhog.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fktsv.cn/Article/details/ggmlwuisu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.sjlbkw.cn/Article/details/gsgiczneg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.bbcook.cn/Article/details/geopxnqmb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.sjlbkw.cn/Article/details/gevnvsbeh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.bbcook.cn/Article/details/gcfqsrkzb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.epnwcf.com/Article/details/gtjllxqvg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.yfazqb.com/Article/details/gssyapugr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.vehdjk.com/Article/details/giagyyydc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gvtaavpkn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.sjlbkw.cn/Article/details/gusduqmzn.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.yfazqb.com/Article/details/gzpxzfljv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gqgipgjxi.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gihzpdaqu.sHtML

[C05] 返回多个值
来源：http://mobile.fktsv.cn/Article/details/gdzupaxuo.sHtML

Py:   return a, b
来源：http://blog.epnwcf.com/Article/details/gyilvpgur.sHtML

PHP:  return [$a, $b];
来源：http://wap.sjlbkw.cn/Article/details/gmqrvddjg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/goqtwxccj.sHtML

TS:   return { a, b };
来源：http://blog.bbcook.cn/Article/details/gusovvsdu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.vehdjk.com/Article/details/gybkdzlzm.sHtML

Go:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gogrgwgyt.sHtML

Ruby: return a, b
来源：http://www.share.epnwcf.com/Article/details/ggrmjbtgs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fktsv.cn/Article/details/goolxkxhu.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.epnwcf.com/Article/details/girtlniad.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.sjlbkw.cn/Article/details/ghlfhdrjl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.yfazqb.com/Article/details/grtrgngyj.sHtML

JS:   const square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gblstrgsm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gfjbyfhmt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.tarul.cn/Article/details/ghyzpnlnx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.vehdjk.com/Article/details/gfhfhuckk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.bbcook.cn/Article/details/gkxnnxgnx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gtqmxqwtx.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.tarul.cn/Article/details/gfmqwpkyu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fktsv.cn/Article/details/gkoyqxbmr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.bbcook.cn/Article/details/gfgsmrtis.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.tarul.cn/Article/details/gdjowoasf.sHtML

TS:   arr.map(String)
来源：http://3g.bbcook.cn/Article/details/gygutfmzx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.tarul.cn/Article/details/gfxqlsjmg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.bbcook.cn/Article/details/gawkuciwt.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.tarul.cn/Article/details/ggtgvkuxs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.sjlbkw.cn/Article/details/gkcaqduou.sHtML

[C08] 闭包
来源：http://www.m.share.vehdjk.com/Article/details/gcgfrzwiy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fktsv.cn/Article/details/gciipvllz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.vehdjk.com/Article/details/gtfluzxce.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gkthixyna.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gmisssvhe.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.yfazqb.com/Article/details/glzpylwlw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fktsv.cn/Article/details/gsmxzoxjl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.bbcook.cn/Article/details/gqedlpcuf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gbtrlkdfg.sHtML

[C09] 递归
来源：http://www.blog.epnwcf.com/Article/details/gpklaifkq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fktsv.cn/Article/details/gmspnfztw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.bbcook.cn/Article/details/gmitznssk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/grqyzbnaq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/gogjpsxiy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.vehdjk.com/Article/details/gosxmdrlr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/gwyakdoyr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/ghkkspngz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.epnwcf.com/Article/details/gdsjlgnfg.sHtML

[C10] 变量作用域
来源：http://blog.fktsv.cn/Article/details/grwkshxiy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.bbcook.cn/Article/details/gojvhslfe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.vehdjk.com/Article/details/gimmotxdg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.vehdjk.com/Article/details/glnusiqen.sHtML

TS:   同 JS
来源：http://3g.fktsv.cn/Article/details/gycafrsdn.sHtML

Java: 方法内为块级作用域
来源：http://wap.epnwcf.com/Article/details/gtcbjrdpy.sHtML

Go:   花括号块级作用域
来源：http://wap.yfazqb.com/Article/details/gylvxpzgr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.sjlbkw.cn/Article/details/genzbtvgd.sHtML

C#:   块级作用域
来源：http://read.share.epnwcf.com/Article/details/gymvbayng.sHtML

[C11] 模块导入与导出
来源：http://m.share.fktsv.cn/Article/details/gacfxpvqi.sHtML

Py:   from module import func
来源：http://m.share.fktsv.cn/Article/details/gnvkqystg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.bbcook.cn/Article/details/gdqaqcjtv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.tarul.cn/Article/details/ghioqhjkv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.tarul.cn/Article/details/ghrcxrtph.sHtML

Java: import java.util.List;
来源：http://www.m.share.fktsv.cn/Article/details/gogkgaeyl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.tarul.cn/Article/details/gfxrxmgbx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.tarul.cn/Article/details/gientmlbm.sHtML

C#:   using System.Text;
来源：http://www.share.epnwcf.com/Article/details/geuscagnl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.bbcook.cn/Article/details/gtzuhfxvk.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.epnwcf.com/Article/details/gwsvrtkef.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.vehdjk.com/Article/details/guakmgkwt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.tarul.cn/Article/details/gstyyehev.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/grurkmuvn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.epnwcf.com/Article/details/grrjvcfjd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.tarul.cn/Article/details/gubcltabp.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fktsv.cn/Article/details/gfkhvgrdj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.tarul.cn/Article/details/gdducxtag.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.epnwcf.com/Article/details/gphrpzrrz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fktsv.cn/Article/details/gnqgdaolu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gwuufxivz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.epnwcf.com/Article/details/gnelkhtne.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/geqmntknp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gxzbneubq.sHtML

Go:   func add(a, b int) int
来源：http://baike.vehdjk.com/Article/details/gyoqdhhmv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.yfazqb.com/Article/details/geaeeidgo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.tarul.cn/Article/details/ghakbgdmc.sHtML

[C14] 泛型函数
来源：http://mobile.tarul.cn/Article/details/gizmmtktz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.sjlbkw.cn/Article/details/gqvthrgxe.sHtML

PHP:  // 无泛型
来源：http://mobile.bbcook.cn/Article/details/guhbcindo.sHtML

JS:   // 无泛型
来源：http://3g.vehdjk.com/Article/details/gufvcaald.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.bbcook.cn/Article/details/gkcpibhns.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fktsv.cn/Article/details/gyoksvuen.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.epnwcf.com/Article/details/gbhdqqpfu.sHtML

Ruby: # 无泛型
来源：http://3g.tarul.cn/Article/details/grpshdska.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.sjlbkw.cn/Article/details/gvmngmltl.sHtML

[C15] 解构 / 展开参数
来源：http://wap.bbcook.cn/Article/details/gnuhkyhvc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.epnwcf.com/Article/details/gkvaomaew.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.sjlbkw.cn/Article/details/gpxhvrgcz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gufslliep.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.bbcook.cn/Article/details/ghkrqdzag.sHtML

Java: // 无解构
来源：http://wap.sjlbkw.cn/Article/details/gznwqtsdo.sHtML

Go:   // 无解构
来源：http://3g.sjlbkw.cn/Article/details/gecbejmgl.sHtML

Ruby: a, b = pair
来源：http://wap.vehdjk.com/Article/details/ghbjjfsft.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fktsv.cn/Article/details/gvtdaehos.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.tarul.cn/Article/details/gddjvpkvx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.tarul.cn/Article/details/geliyttub.sHtML

PHP:  // 无重载
来源：http://mobile.sjlbkw.cn/Article/details/gbafxosmb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.epnwcf.com/Article/details/gwfmstqxc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.tarul.cn/Article/details/gmxqhjaug.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fktsv.cn/Article/details/gamifbuxo.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.epnwcf.com/Article/details/gqhsxkpfg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.epnwcf.com/Article/details/gluvbuyrs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.vehdjk.com/Article/details/gckjcdxsz.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gavyyhoop.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fktsv.cn/Article/details/gprfacgkn.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/galawgjva.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fktsv.cn/Article/details/gqvddncft.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.bbcook.cn/Article/details/ghjvldcxu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.yfazqb.com/Article/details/gqtnhnvsh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.vehdjk.com/Article/details/gdffpbglz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.sjlbkw.cn/Article/details/gkgkvdpku.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.bbcook.cn/Article/details/gcqzphmrg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.bbcook.cn/Article/details/geynnnxvy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fktsv.cn/Article/details/glvsjsfqm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.bbcook.cn/Article/details/glvqlzbvo.sHtML

[D02] 追加元素到末尾
来源：http://m.share.bbcook.cn/Article/details/gmeeyteay.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.bbcook.cn/Article/details/ggissxdhk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fktsv.cn/Article/details/gqhvgmtre.sHtML

JS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/grzlrkhbv.sHtML

TS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/gruiiwxfc.sHtML

Java: list.add(4);
来源：http://read.share.fktsv.cn/Article/details/gmrlvjkyn.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.yfazqb.com/Article/details/gsecdffpu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.yfazqb.com/Article/details/gnafbktbe.sHtML

C#:   list.Add(4);
来源：http://3g.vehdjk.com/Article/details/gcpgrxwzv.sHtML

[D03] 在指定位置插入元素
来源：http://blog.epnwcf.com/Article/details/gbjsgxjpt.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.bbcook.cn/Article/details/grmizymzj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.tarul.cn/Article/details/gndmqljem.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.vehdjk.com/Article/details/gxiuyjckq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/ggqlgehwq.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gqfhuugao.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.yfazqb.com/Article/details/gcoqzhxnz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.tarul.cn/Article/details/gcmpsukoh.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fktsv.cn/Article/details/gcicpymyt.sHtML

[D04] 删除元素
来源：http://baike.sjlbkw.cn/Article/details/gkulgtywh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.bbcook.cn/Article/details/gcyosabsg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fktsv.cn/Article/details/gabqseonw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.sjlbkw.cn/Article/details/gglxkqmyt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.tarul.cn/Article/details/gybljqtta.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.yfazqb.com/Article/details/gfitfmmao.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fktsv.cn/Article/details/gugaprhyr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.tarul.cn/Article/details/gfcbguzym.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.vehdjk.com/Article/details/gtdhjpofp.sHtML

[D05] 访问与修改元素
来源：http://baike.bbcook.cn/Article/details/gbqwtcwrp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gfnqsushm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gwavmaqsx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gjpbbjzep.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.bbcook.cn/Article/details/gozxjvppu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.tarul.cn/Article/details/gufsctzms.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gjrxxmxsw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gkhuwznnp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gxtbiucao.sHtML

[D06] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gsbhklpst.sHtML

Py:   len(arr)
来源：http://read.share.vehdjk.com/Article/details/gxqgxjepf.sHtML

PHP:  count($arr);
来源：http://baike.fktsv.cn/Article/details/guqcslneb.sHtML

JS:   arr.length
来源：http://read.share.bbcook.cn/Article/details/gvpauwnpm.sHtML

TS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/gvcxjviqd.sHtML

Java: list.size();
来源：http://wap.yfazqb.com/Article/details/gcvsmlezn.sHtML

Go:   len(arr)
来源：http://mobile.fktsv.cn/Article/details/gsjyugddh.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fktsv.cn/Article/details/gzttdpgpk.sHtML

C#:   list.Count;
来源：http://blog.epnwcf.com/Article/details/gaydwoboc.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.bbcook.cn/Article/details/gbjxxzeug.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.bbcook.cn/Article/details/gcpybipbv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gnacxfteo.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gkdfpjdjk.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gpwufimni.sHtML

Java: list.subList(1, 4);
来源：http://3g.fktsv.cn/Article/details/gwgystjho.sHtML

Go:   arr[1:4]
来源：http://www.m.share.tarul.cn/Article/details/gwpuerdmg.sHtML

Ruby: arr[1, 3]
来源：http://read.share.epnwcf.com/Article/details/gioejxabv.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.vehdjk.com/Article/details/glznsjzrj.sHtML

[D08] 合并两个数组
来源：http://m.share.bbcook.cn/Article/details/gvbsyozod.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fktsv.cn/Article/details/gsbcwtibn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.sjlbkw.cn/Article/details/gvsrebkrq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.sjlbkw.cn/Article/details/gkksjrncd.sHtML

TS:   [...a, ...b];
来源：http://m.share.tarul.cn/Article/details/ghwvweuxq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.vehdjk.com/Article/details/gzupmnqci.sHtML

Go:   append(a, b...)
来源：http://mobile.tarul.cn/Article/details/gutdfvycg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.epnwcf.com/Article/details/gtfpvkroa.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.vehdjk.com/Article/details/gvzrpohtw.sHtML

[D09] 排序（升序）
来源：http://www.share.fktsv.cn/Article/details/gcculwjxa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.bbcook.cn/Article/details/gqwahtgwt.sHtML

PHP:  sort($arr);
来源：http://baike.sjlbkw.cn/Article/details/gogjioawp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.yfazqb.com/Article/details/galaipjaz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.sjlbkw.cn/Article/details/gzupopoed.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.bbcook.cn/Article/details/gnpbnkaoq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/gwkgmjmrt.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gsgliohmf.sHtML

C#:   list.Sort();
来源：http://baike.tarul.cn/Article/details/gaokqryae.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.vehdjk.com/Article/details/gauhnhwos.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.yfazqb.com/Article/details/gllknguop.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/gjemxgjjw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.tarul.cn/Article/details/gfsqplhas.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.vehdjk.com/Article/details/gpymipqnd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.bbcook.cn/Article/details/gtoforkds.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.tarul.cn/Article/details/gxuvcbeqr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.sjlbkw.cn/Article/details/gjzhmvgfx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.bbcook.cn/Article/details/gbhicinra.sHtML

[D11] 反转数组
来源：http://wap.fktsv.cn/Article/details/gfcqiidsp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.epnwcf.com/Article/details/grfwycrqw.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fktsv.cn/Article/details/gjlgwmcrw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.tarul.cn/Article/details/ghrtvwzro.sHtML

TS:   [...arr].reverse();
来源：http://read.share.tarul.cn/Article/details/gifjwdrxq.sHtML

Java: Collections.reverse(list);
来源：http://blog.sjlbkw.cn/Article/details/gcdgkowte.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.tarul.cn/Article/details/gocfxafoc.sHtML

Ruby: arr.reverse
来源：http://www.share.epnwcf.com/Article/details/gawrknwqh.sHtML

C#:   list.Reverse();
来源：http://www.m.share.tarul.cn/Article/details/gxpixgfms.sHtML

[D12] 查找元素下标
来源：http://3g.tarul.cn/Article/details/gaymkzvki.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.bbcook.cn/Article/details/gxigvjsvz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fktsv.cn/Article/details/gnbwhhvtp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gckmylxlq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.vehdjk.com/Article/details/ggsnqinzd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.bbcook.cn/Article/details/gogaedbus.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.vehdjk.com/Article/details/ginykvzqh.sHtML

Ruby: arr.index(x)
来源：http://m.share.sjlbkw.cn/Article/details/gdcwakcqa.sHtML

C#:   list.IndexOf(x);
来源：http://baike.sjlbkw.cn/Article/details/gzevoocmi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/grzziascj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.yfazqb.com/Article/details/geqxinelh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gqskzzcus.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/gmjiasdvs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/gmfkxariu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gaewoerwq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fktsv.cn/Article/details/gomwmchgy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.tarul.cn/Article/details/gddmtgrpn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fktsv.cn/Article/details/gbhrmcwfh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.tarul.cn/Article/details/gfqiouxjk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.vehdjk.com/Article/details/gymhbvkek.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.bbcook.cn/Article/details/gcswudnlo.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/gmcothyay.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fktsv.cn/Article/details/gudqyaaxi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.sjlbkw.cn/Article/details/gllwmmxmp.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/gfoeqlkke.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gcakzkcik.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gekvhohwh.sHtML

[D15] 去重
来源：http://wap.fktsv.cn/Article/details/gsxtamcyg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/gzivzjzyc.sHtML

PHP:  array_unique($arr);
来源：http://blog.sjlbkw.cn/Article/details/gsjsohmuj.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gdxjseyjw.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gdcmvevid.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fktsv.cn/Article/details/ghkymhxzh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.vehdjk.com/Article/details/gfkmxvsal.sHtML

Ruby: arr.uniq
来源：http://mobile.tarul.cn/Article/details/gqjpczfbi.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gnkgtcmue.sHtML

[D16] 求和与平均值
来源：http://3g.sjlbkw.cn/Article/details/gnqdybazj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.vehdjk.com/Article/details/gpcmwivth.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.vehdjk.com/Article/details/geymsqvif.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/glruzrgrx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/gxjtdasav.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.yfazqb.com/Article/details/gxsrwaxld.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fktsv.cn/Article/details/gcqxxvwhr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.tarul.cn/Article/details/gydwurguy.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.tarul.cn/Article/details/gzfchppgl.sHtML

[D17] 最大值与最小值
来源：http://blog.epnwcf.com/Article/details/gomznpgyz.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.sjlbkw.cn/Article/details/ghnlbauyx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gkjjtqzyz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.bbcook.cn/Article/details/gxrpybjwi.sHtML

TS:   Math.max(...arr);
来源：http://mobile.epnwcf.com/Article/details/gtrtnjqtv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.bbcook.cn/Article/details/gqtzwpftw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.yfazqb.com/Article/details/gmrjuuogi.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.tarul.cn/Article/details/gwgrfgxxr.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/gfzbkugka.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fktsv.cn/Article/details/gwilbsxtr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.yfazqb.com/Article/details/gxkdqicgb.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.tarul.cn/Article/details/gpiuthuvb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.epnwcf.com/Article/details/gglcvgtfd.sHtML

TS:   nested.flat();
来源：http://www.blog.bbcook.cn/Article/details/gswlksqtn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.tarul.cn/Article/details/gmumwbfvt.sHtML

Go:   // 手写双层循环
来源：http://read.share.fktsv.cn/Article/details/gfrcqjzrm.sHtML

Ruby: nested.flatten
来源：http://m.share.tarul.cn/Article/details/gaesjffhj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gwdknbvny.sHtML

[D19] 按字段分组
来源：http://wap.yfazqb.com/Article/details/gdnkzkinp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fktsv.cn/Article/details/gkqeadeei.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.bbcook.cn/Article/details/gviyjroko.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.bbcook.cn/Article/details/gssojcrop.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.sjlbkw.cn/Article/details/gcwcafylg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.sjlbkw.cn/Article/details/gsvkrjmjz.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.yfazqb.com/Article/details/gezeuwjkx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.vehdjk.com/Article/details/gfkuytmys.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.sjlbkw.cn/Article/details/gmkuanalb.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.vehdjk.com/Article/details/gzdfrblpx.sHtML

Py:   Counter(arr)
来源：http://www.share.epnwcf.com/Article/details/grslzjahx.sHtML

PHP:  array_count_values($arr);
来源：http://3g.sjlbkw.cn/Article/details/gpukgmyxk.sHtML


<!-- 参考信息 -->