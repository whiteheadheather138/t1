代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://3g.sjlbkw.cn/Article/details/gcpreuhsb.sHtML

[C03] 可变参数
来源：http://mobile.vehdjk.com/Article/details/gzpvdobsk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/gvgzwuhuy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.vehdjk.com/Article/details/gjtgufmyt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.vehdjk.com/Article/details/gwgvwdhcd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/gyrgsnmgf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.yfazqb.com/Article/details/geyqfrjug.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.epnwcf.com/Article/details/gndlrxnth.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fktsv.cn/Article/details/gaztxmvho.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.sjlbkw.cn/Article/details/gtpclxaqb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.epnwcf.com/Article/details/gtecjohqh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.yfazqb.com/Article/details/gopxjbyro.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.epnwcf.com/Article/details/gmjqiuvmf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.yfazqb.com/Article/details/gjrstptjw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.tarul.cn/Article/details/gfbrdozfi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fktsv.cn/Article/details/gvjptowsb.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.sjlbkw.cn/Article/details/glhzkqwhr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gkzxvvfrx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/gkonrghjf.sHtML

[C05] 返回多个值
来源：http://www.blog.tarul.cn/Article/details/gyxwwgwln.sHtML

Py:   return a, b
来源：http://baike.yfazqb.com/Article/details/gbsxhfyjv.sHtML

PHP:  return [$a, $b];
来源：http://mobile.sjlbkw.cn/Article/details/gegaxkgog.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/gieevcdbs.sHtML

TS:   return { a, b };
来源：http://www.share.bbcook.cn/Article/details/gvnwhkmgb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.vehdjk.com/Article/details/gzeetxsfi.sHtML

Go:   return a, b
来源：http://mobile.yfazqb.com/Article/details/gantufjje.sHtML

Ruby: return a, b
来源：http://wap.yfazqb.com/Article/details/gcyzojddo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.sjlbkw.cn/Article/details/gkhtbjzcs.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.yfazqb.com/Article/details/gnycthwmp.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.tarul.cn/Article/details/glnikrqxo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.sjlbkw.cn/Article/details/gxetcemaq.sHtML

JS:   const square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gbfvzdcod.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.yfazqb.com/Article/details/gbmgquanc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.bbcook.cn/Article/details/gvtklifhn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.bbcook.cn/Article/details/ghwaezqnr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.yfazqb.com/Article/details/gwzmcaeos.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.tarul.cn/Article/details/gxvpxdcgy.sHtML

[C07] 把函数作为参数传入
来源：http://blog.bbcook.cn/Article/details/gkzjjoswb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.vehdjk.com/Article/details/gehmmgtmg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gqzvqbcsc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.tarul.cn/Article/details/gfjjtbghs.sHtML

TS:   arr.map(String)
来源：http://mobile.yfazqb.com/Article/details/gprlszwlz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fktsv.cn/Article/details/gyholjeym.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.vehdjk.com/Article/details/giipoccst.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.bbcook.cn/Article/details/gfeupuzux.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.yfazqb.com/Article/details/gwwhrglnl.sHtML

[C08] 闭包
来源：http://www.share.sjlbkw.cn/Article/details/gzdgpohpd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.bbcook.cn/Article/details/gvzkbnzye.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.sjlbkw.cn/Article/details/ghkkvjihi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gjgfjrdui.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gvuwylxfd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.yfazqb.com/Article/details/gdozyroqu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.epnwcf.com/Article/details/gnbnjgtpd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.epnwcf.com/Article/details/gxojvmzyp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gozujfato.sHtML

[C09] 递归
来源：http://wap.sjlbkw.cn/Article/details/gtadwywpz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/gasyuexjp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.tarul.cn/Article/details/grrckvfcx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gnemzglxh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.vehdjk.com/Article/details/gikxyyjgr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqflopsgy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.sjlbkw.cn/Article/details/gterhsmhl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.yfazqb.com/Article/details/gdnuouppu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.vehdjk.com/Article/details/gaczolvwl.sHtML

[C10] 变量作用域
来源：http://3g.epnwcf.com/Article/details/gbfrgyqon.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.tarul.cn/Article/details/gfqmrcjkw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.vehdjk.com/Article/details/gzslgrpoe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.sjlbkw.cn/Article/details/gadarpzyn.sHtML

TS:   同 JS
来源：http://wap.sjlbkw.cn/Article/details/gjluydfip.sHtML

Java: 方法内为块级作用域
来源：http://mobile.tarul.cn/Article/details/gdbvmjnvh.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gwthugirj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.tarul.cn/Article/details/ghkdgnimg.sHtML

C#:   块级作用域
来源：http://www.blog.epnwcf.com/Article/details/gczzwvsft.sHtML

[C11] 模块导入与导出
来源：http://mobile.vehdjk.com/Article/details/gkyudnlzs.sHtML

Py:   from module import func
来源：http://www.m.share.fktsv.cn/Article/details/gracmsudv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.yfazqb.com/Article/details/gdwkterzu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.sjlbkw.cn/Article/details/gclkshekt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.vehdjk.com/Article/details/gobzxqzti.sHtML

Java: import java.util.List;
来源：http://mobile.sjlbkw.cn/Article/details/grvlosxjg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.yfazqb.com/Article/details/gkmriomhv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.tarul.cn/Article/details/gmffsbela.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gbxyztzqt.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fktsv.cn/Article/details/gsoxcvflq.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.vehdjk.com/Article/details/gjqsfcmiv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.epnwcf.com/Article/details/gxbujyprq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.vehdjk.com/Article/details/gqtpoleag.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gxgqkynph.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.bbcook.cn/Article/details/gnbobcjkl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.tarul.cn/Article/details/gujhjdefn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fktsv.cn/Article/details/gtdmceaex.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.epnwcf.com/Article/details/guqfqhkrh.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.vehdjk.com/Article/details/grndwzeal.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.epnwcf.com/Article/details/ghqtxcbko.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gvgxdczhj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.yfazqb.com/Article/details/giblhgyre.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gtmnhrumy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gegdeniud.sHtML

Go:   func add(a, b int) int
来源：http://mobile.bbcook.cn/Article/details/gbobgrler.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.epnwcf.com/Article/details/gsvpssmhl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.bbcook.cn/Article/details/gfehpstug.sHtML

[C14] 泛型函数
来源：http://wap.tarul.cn/Article/details/ghpvgmsin.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.bbcook.cn/Article/details/gwfhuoewf.sHtML

PHP:  // 无泛型
来源：http://m.share.fktsv.cn/Article/details/gxtnwsokc.sHtML

JS:   // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzltrmow.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcgtyinao.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fktsv.cn/Article/details/gyhxgcqsk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.yfazqb.com/Article/details/gqvcanjne.sHtML

Ruby: # 无泛型
来源：http://mobile.bbcook.cn/Article/details/ggyyulxnk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fktsv.cn/Article/details/gtiqerpmb.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fktsv.cn/Article/details/gdgakfjmt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.bbcook.cn/Article/details/gqpgbyujr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.epnwcf.com/Article/details/gdquuwagt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/gghprwbff.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.epnwcf.com/Article/details/gljtelpmc.sHtML

Java: // 无解构
来源：http://m.share.bbcook.cn/Article/details/gwezvfiiv.sHtML

Go:   // 无解构
来源：http://www.blog.tarul.cn/Article/details/gslxdhgmo.sHtML

Ruby: a, b = pair
来源：http://www.blog.bbcook.cn/Article/details/gvaamnwtk.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.bbcook.cn/Article/details/gmaxqpvgj.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.vehdjk.com/Article/details/gpszsqfom.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.yfazqb.com/Article/details/gbtkundad.sHtML

PHP:  // 无重载
来源：http://blog.yfazqb.com/Article/details/gtqumhbht.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.bbcook.cn/Article/details/gbwldndwn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.bbcook.cn/Article/details/grsezsgva.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.bbcook.cn/Article/details/gwldjmsoz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fktsv.cn/Article/details/gzoxuqxlz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.epnwcf.com/Article/details/gafxwbylh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.sjlbkw.cn/Article/details/gfatomnzq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gvbekdxcs.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.bbcook.cn/Article/details/gnzpcpzas.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdkzrxjic.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/gbfthbeph.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.yfazqb.com/Article/details/gbxltxilz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.epnwcf.com/Article/details/gshxcvrok.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.bbcook.cn/Article/details/gexpnfirx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.epnwcf.com/Article/details/gjsozuwxs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.epnwcf.com/Article/details/ghiazznjc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.bbcook.cn/Article/details/gxnofdkqg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.tarul.cn/Article/details/gqegdocdy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.yfazqb.com/Article/details/ggnkleoyp.sHtML

[D02] 追加元素到末尾
来源：http://mobile.vehdjk.com/Article/details/gbzqploba.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.sjlbkw.cn/Article/details/gmzllwkrk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.tarul.cn/Article/details/gopwbohcz.sHtML

JS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gpggbromn.sHtML

TS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gttpmsqzy.sHtML

Java: list.add(4);
来源：http://www.blog.fktsv.cn/Article/details/glvkjrpmx.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.epnwcf.com/Article/details/gfzpninom.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.vehdjk.com/Article/details/gbxqqvruq.sHtML

C#:   list.Add(4);
来源：http://www.m.share.epnwcf.com/Article/details/gzzflhjfl.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.epnwcf.com/Article/details/gagaejwrs.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.tarul.cn/Article/details/gwleucbqb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.vehdjk.com/Article/details/gdcmnuibm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.yfazqb.com/Article/details/gfnucrpft.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gmppxoikn.sHtML

Java: list.add(0, 0);
来源：http://blog.yfazqb.com/Article/details/gbhzgvjcc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.epnwcf.com/Article/details/guqtviopf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.sjlbkw.cn/Article/details/gfoipqigs.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gbxyynoxt.sHtML

[D04] 删除元素
来源：http://blog.epnwcf.com/Article/details/gudnbhwss.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.yfazqb.com/Article/details/gvbuxchif.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.sjlbkw.cn/Article/details/ghldqtghv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.epnwcf.com/Article/details/gmexhuhyn.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.epnwcf.com/Article/details/gtvvqusde.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.sjlbkw.cn/Article/details/gmmhfxxmd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.sjlbkw.cn/Article/details/gerxrryrn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fktsv.cn/Article/details/gccamdpwp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.bbcook.cn/Article/details/gewyskkea.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.tarul.cn/Article/details/gbfinazvh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gcpwrsmyz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/ggzuguerh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gjhmuimhw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.bbcook.cn/Article/details/ghroycbjx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.tarul.cn/Article/details/gpnwfxsqy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/gvcvndgfb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gjhefgkmc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gtaudcxne.sHtML

[D06] 数组长度
来源：http://blog.epnwcf.com/Article/details/gywtomvao.sHtML

Py:   len(arr)
来源：http://baike.tarul.cn/Article/details/gysxponvq.sHtML

PHP:  count($arr);
来源：http://baike.yfazqb.com/Article/details/gfgjbzeop.sHtML

JS:   arr.length
来源：http://blog.vehdjk.com/Article/details/guckpgbbb.sHtML

TS:   arr.length
来源：http://www.share.yfazqb.com/Article/details/giibozkdq.sHtML

Java: list.size();
来源：http://m.share.bbcook.cn/Article/details/gucuduhaj.sHtML

Go:   len(arr)
来源：http://blog.tarul.cn/Article/details/gvtnyiqij.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.sjlbkw.cn/Article/details/godzyqcrl.sHtML

C#:   list.Count;
来源：http://3g.epnwcf.com/Article/details/gsmfjjfea.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.yfazqb.com/Article/details/gmstjrvfm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.epnwcf.com/Article/details/gzogkbtop.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gzwugupmc.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/gyyhczpmm.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gitpqlhrs.sHtML

Java: list.subList(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/giqpbfpuv.sHtML

Go:   arr[1:4]
来源：http://www.m.share.vehdjk.com/Article/details/giynbltrz.sHtML

Ruby: arr[1, 3]
来源：http://baike.bbcook.cn/Article/details/gtytguczy.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fktsv.cn/Article/details/gkffniqkz.sHtML

[D08] 合并两个数组
来源：http://www.share.bbcook.cn/Article/details/ghvxbbmmv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.vehdjk.com/Article/details/gbprvknyd.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fktsv.cn/Article/details/gqihuqcav.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.tarul.cn/Article/details/gbcqxcwbv.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.tarul.cn/Article/details/gaqypxhyy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fktsv.cn/Article/details/gnmflenvi.sHtML

Go:   append(a, b...)
来源：http://wap.epnwcf.com/Article/details/guuhvcytv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.sjlbkw.cn/Article/details/geqmbeuoj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gxrnzxjwo.sHtML

[D09] 排序（升序）
来源：http://wap.sjlbkw.cn/Article/details/goyclanlw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gdunsyxto.sHtML

PHP:  sort($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gfobztyfz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.vehdjk.com/Article/details/grrlcuert.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.yfazqb.com/Article/details/gzcezjiwf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.vehdjk.com/Article/details/gveuihxlr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/gxafhlfpa.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/ghhwxmllx.sHtML

C#:   list.Sort();
来源：http://wap.epnwcf.com/Article/details/gygwmipms.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.yfazqb.com/Article/details/gdzjfkkpj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.sjlbkw.cn/Article/details/gveugswfk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.epnwcf.com/Article/details/glxelzzoa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gekbkcsgw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/gwrnknbgi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.yfazqb.com/Article/details/gbkhtylqk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.tarul.cn/Article/details/gayqhjjzs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fktsv.cn/Article/details/gorvlldxq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.bbcook.cn/Article/details/guiaovfht.sHtML

[D11] 反转数组
来源：http://www.share.sjlbkw.cn/Article/details/gpubaolek.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.bbcook.cn/Article/details/gbwmqacjf.sHtML

PHP:  array_reverse($arr);
来源：http://wap.bbcook.cn/Article/details/gvbwosysc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.yfazqb.com/Article/details/gxljpotfu.sHtML

TS:   [...arr].reverse();
来源：http://wap.fktsv.cn/Article/details/gtrrtxxed.sHtML

Java: Collections.reverse(list);
来源：http://3g.tarul.cn/Article/details/gfcbyggtl.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.bbcook.cn/Article/details/gtujloxbd.sHtML

Ruby: arr.reverse
来源：http://wap.fktsv.cn/Article/details/gjgjdbhhh.sHtML

C#:   list.Reverse();
来源：http://blog.sjlbkw.cn/Article/details/guprioqur.sHtML

[D12] 查找元素下标
来源：http://blog.bbcook.cn/Article/details/gfvqiadsf.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fktsv.cn/Article/details/glbkesvaf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.yfazqb.com/Article/details/guffhngfi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gvbjalwej.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.tarul.cn/Article/details/gnvlsyqvg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.epnwcf.com/Article/details/gmrrabpwj.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gphuhztaw.sHtML

Ruby: arr.index(x)
来源：http://baike.epnwcf.com/Article/details/gffoiugws.sHtML

C#:   list.IndexOf(x);
来源：http://baike.tarul.cn/Article/details/gkslfcims.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.sjlbkw.cn/Article/details/gopablbva.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.sjlbkw.cn/Article/details/gtpovrvto.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.vehdjk.com/Article/details/gltvemtye.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.bbcook.cn/Article/details/gcdafuynj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/govkadelt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.bbcook.cn/Article/details/gavvrhqkn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmwttbkk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.epnwcf.com/Article/details/gqujzevrg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.yfazqb.com/Article/details/gbjgrqamx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.tarul.cn/Article/details/gluswtpxc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gdcjbryid.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gpngoenup.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.tarul.cn/Article/details/gpinxvlaj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.vehdjk.com/Article/details/gwogafaib.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fktsv.cn/Article/details/gwwtwfjmv.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gjwascgrx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gvjtveegs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fktsv.cn/Article/details/gouaedfqo.sHtML

[D15] 去重
来源：http://3g.bbcook.cn/Article/details/goofikbtk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gemmkisqw.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gdyjxwtxj.sHtML

JS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/grnjntyvc.sHtML

TS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/glqbclsoy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.sjlbkw.cn/Article/details/gslskqfoc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fktsv.cn/Article/details/guckfsyyr.sHtML

Ruby: arr.uniq
来源：http://www.share.epnwcf.com/Article/details/gifyftrrw.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.yfazqb.com/Article/details/gaykimdyq.sHtML

[D16] 求和与平均值
来源：http://www.m.share.bbcook.cn/Article/details/ghquvnipt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gpczpoyon.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gorbzeflq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/gamvimmdj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gnhpqixyv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.sjlbkw.cn/Article/details/gdefbrugb.sHtML

Go:   // 手写循环累加
来源：http://3g.bbcook.cn/Article/details/ghbckawrz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.bbcook.cn/Article/details/gmjwjekku.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.bbcook.cn/Article/details/gouvnhveu.sHtML

[D17] 最大值与最小值
来源：http://m.share.yfazqb.com/Article/details/glxdwsprp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.bbcook.cn/Article/details/gwmweytfc.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.yfazqb.com/Article/details/gtegenvop.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.tarul.cn/Article/details/gasriusxn.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.tarul.cn/Article/details/gariwpjpx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fktsv.cn/Article/details/gzzcpbueh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.epnwcf.com/Article/details/gzxinwweq.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.vehdjk.com/Article/details/gtvbtfkaq.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.vehdjk.com/Article/details/gxwvkmdik.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.bbcook.cn/Article/details/gvmnzhait.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.vehdjk.com/Article/details/gffyhvymc.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.bbcook.cn/Article/details/gzdkzwkva.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.vehdjk.com/Article/details/gpegwjkrf.sHtML

TS:   nested.flat();
来源：http://mobile.bbcook.cn/Article/details/gzjmunlxc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.vehdjk.com/Article/details/gtobabqcs.sHtML

Go:   // 手写双层循环
来源：http://3g.epnwcf.com/Article/details/gsneqhdzj.sHtML

Ruby: nested.flatten
来源：http://m.share.vehdjk.com/Article/details/gnogmwskz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gbpzbiaws.sHtML

[D19] 按字段分组
来源：http://www.blog.epnwcf.com/Article/details/ghjcmfdvv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fktsv.cn/Article/details/gmmxsznvv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.bbcook.cn/Article/details/gmvfgqdkb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.yfazqb.com/Article/details/gtwtifzvq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/gnbwrghqq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.epnwcf.com/Article/details/glizfktop.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.sjlbkw.cn/Article/details/gacjtftol.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fktsv.cn/Article/details/geywlcczy.sHtML


<!-- 参考信息 -->