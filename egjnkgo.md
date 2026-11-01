代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.tarul.cn/Article/details/gbbrytzrh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gpuieluqq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.vehdjk.com/Article/details/gzrvkhqec.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fktsv.cn/Article/details/gmnwmakfw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.vehdjk.com/Article/details/gcneubxzm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.epnwcf.com/Article/details/gjwmhmuwi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.vehdjk.com/Article/details/gjzkcbktn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.tarul.cn/Article/details/gtwztirpj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.yfazqb.com/Article/details/gixzgqtgc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.tarul.cn/Article/details/gqlbliknc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.sjlbkw.cn/Article/details/gyhyorrff.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.bbcook.cn/Article/details/gqjmhvotc.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.vehdjk.com/Article/details/giyfbcivn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gkwopenyk.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gbqizbquj.sHtML

[C05] 返回多个值
来源：http://read.share.vehdjk.com/Article/details/guibdkwpy.sHtML

Py:   return a, b
来源：http://read.share.bbcook.cn/Article/details/guztjtgbk.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fktsv.cn/Article/details/ghdyhcjob.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.yfazqb.com/Article/details/gbucbkoez.sHtML

TS:   return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/guejmmxjc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.sjlbkw.cn/Article/details/grzmodlgh.sHtML

Go:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gvhytmcqw.sHtML

Ruby: return a, b
来源：http://wap.fktsv.cn/Article/details/gxxyhdxce.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.yfazqb.com/Article/details/gwavsotos.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/gjpercgpk.sHtML

Py:   square = lambda x: x * x
来源：http://baike.tarul.cn/Article/details/gispchgsc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.vehdjk.com/Article/details/gjeerwmxd.sHtML

JS:   const square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gsfwadmlm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.epnwcf.com/Article/details/gnixgphto.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fktsv.cn/Article/details/gkgvulzxf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.bbcook.cn/Article/details/gdfjmibot.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.epnwcf.com/Article/details/gzmohbrxj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/gixictkan.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.tarul.cn/Article/details/gstoktjff.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fktsv.cn/Article/details/gsjdnjbiz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.sjlbkw.cn/Article/details/geozrnsqz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.yfazqb.com/Article/details/gkqwxvcct.sHtML

TS:   arr.map(String)
来源：http://m.share.vehdjk.com/Article/details/gsnbtdszo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/gwxcfvrnn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.yfazqb.com/Article/details/glmewabog.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.bbcook.cn/Article/details/gyzkeqwpa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.epnwcf.com/Article/details/gfzgiearm.sHtML

[C08] 闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpxwwpwj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.bbcook.cn/Article/details/glhfeksuh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.tarul.cn/Article/details/gvgpoclxp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/gdfzzfeke.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gkezakpoe.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.yfazqb.com/Article/details/gelcbhfts.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.sjlbkw.cn/Article/details/gncmfexyq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.yfazqb.com/Article/details/glodjfhnv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gahzmxmnp.sHtML

[C09] 递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpmojsab.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/gxtxosqhe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.vehdjk.com/Article/details/gxyxnxozl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.epnwcf.com/Article/details/gxlowggwy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gkyupyizo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fktsv.cn/Article/details/gtzgfnyxy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.bbcook.cn/Article/details/gnuziffyc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.epnwcf.com/Article/details/gbuiafbdp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fktsv.cn/Article/details/gpsqweovo.sHtML

[C10] 变量作用域
来源：http://www.share.sjlbkw.cn/Article/details/gbhugkdhy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.epnwcf.com/Article/details/ggdmkoewj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.tarul.cn/Article/details/gcipsudzl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.tarul.cn/Article/details/gttfeoksg.sHtML

TS:   同 JS
来源：http://read.share.yfazqb.com/Article/details/gjjcwhqvy.sHtML

Java: 方法内为块级作用域
来源：http://baike.fktsv.cn/Article/details/gnvneufiy.sHtML

Go:   花括号块级作用域
来源：http://baike.epnwcf.com/Article/details/gkdrigaky.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.vehdjk.com/Article/details/gqmhwehhz.sHtML

C#:   块级作用域
来源：http://m.share.yfazqb.com/Article/details/ghkhaxcvr.sHtML

[C11] 模块导入与导出
来源：http://blog.bbcook.cn/Article/details/gxcszvuhh.sHtML

Py:   from module import func
来源：http://3g.sjlbkw.cn/Article/details/gmhjpstqj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.epnwcf.com/Article/details/guzhdenke.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.yfazqb.com/Article/details/garfchlco.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.tarul.cn/Article/details/gsczbxybt.sHtML

Java: import java.util.List;
来源：http://baike.yfazqb.com/Article/details/gckbvqwvg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.epnwcf.com/Article/details/gvaojtkav.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.vehdjk.com/Article/details/geibyzejd.sHtML

C#:   using System.Text;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfjuxvvs.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fktsv.cn/Article/details/gbnomhpjq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fktsv.cn/Article/details/gfcdvuxfs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fktsv.cn/Article/details/gyvynqjlh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/grlltyqqe.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.yfazqb.com/Article/details/gxatzdpff.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.sjlbkw.cn/Article/details/gcftnujva.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.bbcook.cn/Article/details/gspddxxfj.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.epnwcf.com/Article/details/gvzovatsv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.yfazqb.com/Article/details/gprzxpcfd.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.yfazqb.com/Article/details/gqiigskbt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.bbcook.cn/Article/details/gvxbvegwg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gsnbsmwqo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.tarul.cn/Article/details/gmbxkgkax.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.yfazqb.com/Article/details/ghxtqgwgi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gufpnfoec.sHtML

Go:   func add(a, b int) int
来源：http://read.share.vehdjk.com/Article/details/gfaziqxwf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.bbcook.cn/Article/details/gxvdxhxff.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.tarul.cn/Article/details/gdvlhobrl.sHtML

[C14] 泛型函数
来源：http://3g.sjlbkw.cn/Article/details/gpuittait.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.epnwcf.com/Article/details/gzpadiapc.sHtML

PHP:  // 无泛型
来源：http://m.share.yfazqb.com/Article/details/gfkzyanoe.sHtML

JS:   // 无泛型
来源：http://blog.vehdjk.com/Article/details/gcbxkfibf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.vehdjk.com/Article/details/gulnqbcrj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.epnwcf.com/Article/details/gwvadtebx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.tarul.cn/Article/details/gqwdfmabh.sHtML

Ruby: # 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/goiwjjahi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fktsv.cn/Article/details/gravbqscd.sHtML

[C15] 解构 / 展开参数
来源：http://blog.epnwcf.com/Article/details/gqpdqwxus.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.sjlbkw.cn/Article/details/gxchffihd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.sjlbkw.cn/Article/details/gdzpwdwun.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.tarul.cn/Article/details/gizppciwg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.epnwcf.com/Article/details/grmenytce.sHtML

Java: // 无解构
来源：http://www.blog.epnwcf.com/Article/details/gxayuywzb.sHtML

Go:   // 无解构
来源：http://www.share.sjlbkw.cn/Article/details/gawqxrosp.sHtML

Ruby: a, b = pair
来源：http://www.m.share.epnwcf.com/Article/details/gshvhenuo.sHtML

C#:   var (a, b) = pair;
来源：http://blog.vehdjk.com/Article/details/gzokqjkst.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fktsv.cn/Article/details/gyluicsfz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fktsv.cn/Article/details/guavaiprj.sHtML

PHP:  // 无重载
来源：http://blog.bbcook.cn/Article/details/gijbbsqdk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.yfazqb.com/Article/details/gfqssgnqa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.vehdjk.com/Article/details/gqidykpbi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.bbcook.cn/Article/details/gsuhepvqv.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.epnwcf.com/Article/details/gfevwcfoa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.yfazqb.com/Article/details/gmthjcnrz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.yfazqb.com/Article/details/gfqyqvczy.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvajfvezb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.epnwcf.com/Article/details/glmjtfrfv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/glnfddism.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.sjlbkw.cn/Article/details/gzuxmwwjj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.epnwcf.com/Article/details/gkdggxvnx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/gqkzihphq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.bbcook.cn/Article/details/gejgujgib.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.yfazqb.com/Article/details/gfsyrtdww.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fktsv.cn/Article/details/gmeokzyhb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.vehdjk.com/Article/details/gtogpunjo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.yfazqb.com/Article/details/ggtjievxc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.tarul.cn/Article/details/gmdhgrwur.sHtML

[D02] 追加元素到末尾
来源：http://blog.sjlbkw.cn/Article/details/gxymotorl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fktsv.cn/Article/details/gbnqtkaod.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fktsv.cn/Article/details/ganungebb.sHtML

JS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/grkrqhsuq.sHtML

TS:   arr.push(4);
来源：http://baike.sjlbkw.cn/Article/details/gysvbsxva.sHtML

Java: list.add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkgdbvlj.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gcusfspks.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.bbcook.cn/Article/details/geltmwtaw.sHtML

C#:   list.Add(4);
来源：http://www.m.share.vehdjk.com/Article/details/gpraqlrnq.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.bbcook.cn/Article/details/glssinzuv.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.yfazqb.com/Article/details/gvnhbxrfy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.bbcook.cn/Article/details/gtagjaxya.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.bbcook.cn/Article/details/grodjosoz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fktsv.cn/Article/details/gujqfbcsi.sHtML

Java: list.add(0, 0);
来源：http://wap.fktsv.cn/Article/details/gupzxayil.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.sjlbkw.cn/Article/details/gplptjxsq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.bbcook.cn/Article/details/gwtpghuub.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.tarul.cn/Article/details/gxtuxvrmv.sHtML

[D04] 删除元素
来源：http://m.share.bbcook.cn/Article/details/gdyrucytw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.bbcook.cn/Article/details/gpfjxevya.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.yfazqb.com/Article/details/gpsjzcwzl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.vehdjk.com/Article/details/gxbzxsycm.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.sjlbkw.cn/Article/details/gitkxszhd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.epnwcf.com/Article/details/gftikptnn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.bbcook.cn/Article/details/gdfnhjnhw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.tarul.cn/Article/details/gdfvponki.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.tarul.cn/Article/details/gwovmolax.sHtML

[D05] 访问与修改元素
来源：http://wap.epnwcf.com/Article/details/gcjahgyze.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gahqkutdh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gobvorvmi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gekpquddm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.vehdjk.com/Article/details/gmuogejrz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.bbcook.cn/Article/details/gzikfzlsd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gergnadzk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gdorldczb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.bbcook.cn/Article/details/grvmcnexy.sHtML

[D06] 数组长度
来源：http://blog.vehdjk.com/Article/details/gxgrvddip.sHtML

Py:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gzmorwtsa.sHtML

PHP:  count($arr);
来源：http://wap.yfazqb.com/Article/details/gvcygfxwq.sHtML

JS:   arr.length
来源：http://3g.bbcook.cn/Article/details/glpbsxbbi.sHtML

TS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gfecfkcdh.sHtML

Java: list.size();
来源：http://read.share.tarul.cn/Article/details/gkxtjjlmb.sHtML

Go:   len(arr)
来源：http://3g.tarul.cn/Article/details/gouqltrfr.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fktsv.cn/Article/details/gjtqpscww.sHtML

C#:   list.Count;
来源：http://www.blog.vehdjk.com/Article/details/glihmnsvq.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fktsv.cn/Article/details/gerhuhmuz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.vehdjk.com/Article/details/gmznxfvog.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.tarul.cn/Article/details/gebijayql.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/guihftlmy.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gakwkymen.sHtML

Java: list.subList(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gshoykppc.sHtML

Go:   arr[1:4]
来源：http://m.share.tarul.cn/Article/details/gkmysvqhu.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.vehdjk.com/Article/details/gnjrwfsmy.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fktsv.cn/Article/details/gedmpkzwx.sHtML

[D08] 合并两个数组
来源：http://wap.tarul.cn/Article/details/gkapfkxdm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.yfazqb.com/Article/details/gxoozxvxa.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fktsv.cn/Article/details/grpfijuuh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fktsv.cn/Article/details/gxayviygi.sHtML

TS:   [...a, ...b];
来源：http://blog.bbcook.cn/Article/details/gpuvdzuxc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.vehdjk.com/Article/details/gltxkssgi.sHtML

Go:   append(a, b...)
来源：http://blog.epnwcf.com/Article/details/gkllbppyj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.yfazqb.com/Article/details/glxszlzyw.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gxejndjat.sHtML

[D09] 排序（升序）
来源：http://blog.fktsv.cn/Article/details/gezjzprwj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gglaenqfm.sHtML

PHP:  sort($arr);
来源：http://mobile.tarul.cn/Article/details/gdjdccbpq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.yfazqb.com/Article/details/ggowmftjk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fktsv.cn/Article/details/glpdftkry.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.yfazqb.com/Article/details/grrtfqlwh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gtwudblyf.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gsiycyxsq.sHtML

C#:   list.Sort();
来源：http://www.m.share.tarul.cn/Article/details/gbwjiungw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.bbcook.cn/Article/details/gnckzkngk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fktsv.cn/Article/details/garratngv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gkultyupe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.epnwcf.com/Article/details/gqmtiyyum.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.bbcook.cn/Article/details/gfwetakfw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.tarul.cn/Article/details/guhuezwki.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.tarul.cn/Article/details/gupundagt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.bbcook.cn/Article/details/gskwlcpce.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.epnwcf.com/Article/details/gwobqtzoc.sHtML

[D11] 反转数组
来源：http://m.share.yfazqb.com/Article/details/gvskywdly.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.yfazqb.com/Article/details/gzcwrxmhk.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.bbcook.cn/Article/details/gfreeadbl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.bbcook.cn/Article/details/gvqwlpyal.sHtML

TS:   [...arr].reverse();
来源：http://mobile.epnwcf.com/Article/details/ghqjewqwb.sHtML

Java: Collections.reverse(list);
来源：http://blog.yfazqb.com/Article/details/glskqrgtz.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.vehdjk.com/Article/details/gmycxefqg.sHtML

Ruby: arr.reverse
来源：http://www.blog.fktsv.cn/Article/details/gsscxcfeo.sHtML

C#:   list.Reverse();
来源：http://m.share.tarul.cn/Article/details/gnzcgztme.sHtML

[D12] 查找元素下标
来源：http://blog.tarul.cn/Article/details/gaztorcxu.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.sjlbkw.cn/Article/details/gjvihlfay.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.yfazqb.com/Article/details/gkdzccybd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.tarul.cn/Article/details/gyljlfxdk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.epnwcf.com/Article/details/gkiciefeo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fktsv.cn/Article/details/gdcavoeda.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/glkbvspud.sHtML

Ruby: arr.index(x)
来源：http://m.share.bbcook.cn/Article/details/gwtvdeozl.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.epnwcf.com/Article/details/gkxgptxpe.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fktsv.cn/Article/details/gcduueaqm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.vehdjk.com/Article/details/ggjzovytk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.bbcook.cn/Article/details/gqnqtxvwq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gudxvmmro.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.vehdjk.com/Article/details/gkxhciykr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.epnwcf.com/Article/details/gafzwjtdh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.bbcook.cn/Article/details/gehyreebo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.bbcook.cn/Article/details/gmkarbnhz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.epnwcf.com/Article/details/gnyipqisj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.yfazqb.com/Article/details/glcobtgcp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gdejdigrx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/gdwmwyjkm.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/gtirpmzgc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gdxtaduul.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gtyqwpeqk.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/greqpnsdw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.tarul.cn/Article/details/gfdnxlszu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.tarul.cn/Article/details/glakqjcvs.sHtML

[D15] 去重
来源：http://wap.tarul.cn/Article/details/gsdvkstfs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/grusaanmf.sHtML

PHP:  array_unique($arr);
来源：http://mobile.epnwcf.com/Article/details/gzpycjfxm.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/gdhxcjjhe.sHtML

TS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/godlrumhs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.epnwcf.com/Article/details/gwiqihknl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.bbcook.cn/Article/details/gabliymvf.sHtML

Ruby: arr.uniq
来源：http://m.share.vehdjk.com/Article/details/gbkgwmcjw.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.vehdjk.com/Article/details/gnxmnvdnn.sHtML

[D16] 求和与平均值
来源：http://www.share.epnwcf.com/Article/details/gehexltzc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gvavzxqch.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.tarul.cn/Article/details/gjtyakuts.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gupidsizg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.epnwcf.com/Article/details/gtzvovfas.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.sjlbkw.cn/Article/details/glrggtfjd.sHtML

Go:   // 手写循环累加
来源：http://mobile.tarul.cn/Article/details/gtofvfybh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.tarul.cn/Article/details/gfdsxdqmk.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/gvhlfdvdi.sHtML

[D17] 最大值与最小值
来源：http://blog.sjlbkw.cn/Article/details/gcsedejrg.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.bbcook.cn/Article/details/gsvgsmqku.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fktsv.cn/Article/details/gfgbaiejw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.bbcook.cn/Article/details/gqoynmefr.sHtML

TS:   Math.max(...arr);
来源：http://wap.epnwcf.com/Article/details/gwxyhusib.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.vehdjk.com/Article/details/gtrigajle.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.tarul.cn/Article/details/ghjhterae.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.tarul.cn/Article/details/gcxlrnlqm.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.bbcook.cn/Article/details/gmmfomyai.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fktsv.cn/Article/details/gmrknwwgy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.epnwcf.com/Article/details/gptsxxwnt.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.yfazqb.com/Article/details/goqscrwdh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fktsv.cn/Article/details/gonjefgqt.sHtML

TS:   nested.flat();
来源：http://www.share.vehdjk.com/Article/details/gsznnuzne.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.yfazqb.com/Article/details/gfywzxdwl.sHtML

Go:   // 手写双层循环
来源：http://read.share.fktsv.cn/Article/details/gwhljmmuc.sHtML

Ruby: nested.flatten
来源：http://mobile.fktsv.cn/Article/details/gqzaslxky.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.yfazqb.com/Article/details/galnkyofx.sHtML

[D19] 按字段分组
来源：http://mobile.fktsv.cn/Article/details/gzosudnwh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fktsv.cn/Article/details/gicjfnuvi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.epnwcf.com/Article/details/ghgozqtks.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.vehdjk.com/Article/details/gdmaefgti.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fktsv.cn/Article/details/gotgxfjcm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.epnwcf.com/Article/details/gghonfmoa.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.yfazqb.com/Article/details/gyfflkbyb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.bbcook.cn/Article/details/gnxxchymb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.bbcook.cn/Article/details/gfqlknvxf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fktsv.cn/Article/details/gcepjiumn.sHtML

Py:   Counter(arr)
来源：http://www.share.tarul.cn/Article/details/grarqecvg.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.tarul.cn/Article/details/gtenfgwem.sHtML


<!-- 参考信息 -->