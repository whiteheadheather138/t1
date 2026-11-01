代发 wailian999

[C06] 匿名函数 / lambda
来源：http://m.share.vehdjk.com/Article/details/gawpjendr.sHtML

Py:   square = lambda x: x * x
来源：http://baike.epnwcf.com/Article/details/gbheznwkk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.bbcook.cn/Article/details/gnddeevzs.sHtML

JS:   const square = x => x * x;
来源：http://read.share.vehdjk.com/Article/details/gsxazwutj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.bbcook.cn/Article/details/gbakpytwr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/gathtezhb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.vehdjk.com/Article/details/gksyerjaw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.vehdjk.com/Article/details/gduslifbq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/gdfiswmcn.sHtML

[C07] 把函数作为参数传入
来源：http://baike.vehdjk.com/Article/details/gioxqrmpx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.tarul.cn/Article/details/gpnyoszar.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.bbcook.cn/Article/details/gyeaxkutq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.tarul.cn/Article/details/gerzajing.sHtML

TS:   arr.map(String)
来源：http://www.m.share.sjlbkw.cn/Article/details/geraxnnrq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.yfazqb.com/Article/details/gsxbngbfk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.yfazqb.com/Article/details/glzihchsk.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fktsv.cn/Article/details/gqmjofaex.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fktsv.cn/Article/details/ggnwcpxve.sHtML

[C08] 闭包
来源：http://3g.fktsv.cn/Article/details/gmvzimvoo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fktsv.cn/Article/details/gcxmkjpdq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.yfazqb.com/Article/details/gkjifydbd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/grultdbto.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/garhxwcks.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.bbcook.cn/Article/details/gywzafvng.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fktsv.cn/Article/details/gjsezhxyc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.vehdjk.com/Article/details/gejfexwwo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/gxgvlqduf.sHtML

[C09] 递归
来源：http://mobile.bbcook.cn/Article/details/geccdjgbr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.bbcook.cn/Article/details/ggpjgbrsu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.tarul.cn/Article/details/gvzggmvpi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/gpiwkwfzg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/gizpluiqc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.bbcook.cn/Article/details/gxanbdjeu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.bbcook.cn/Article/details/gdfqigkuh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fktsv.cn/Article/details/gknvwtaur.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.sjlbkw.cn/Article/details/gzvyvqvcc.sHtML

[C10] 变量作用域
来源：http://www.blog.epnwcf.com/Article/details/glsjspnlj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.tarul.cn/Article/details/gcuyhjrrl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.yfazqb.com/Article/details/gnoypdibx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.yfazqb.com/Article/details/gniruvzbt.sHtML

TS:   同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gpbwhymle.sHtML

Java: 方法内为块级作用域
来源：http://3g.yfazqb.com/Article/details/gqvmyjalt.sHtML

Go:   花括号块级作用域
来源：http://m.share.fktsv.cn/Article/details/gvpdjsnfz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.sjlbkw.cn/Article/details/gmpfdgqnj.sHtML

C#:   块级作用域
来源：http://www.share.yfazqb.com/Article/details/gdatdsnio.sHtML

[C11] 模块导入与导出
来源：http://read.share.tarul.cn/Article/details/gtgdtamps.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/gyeiznsol.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.sjlbkw.cn/Article/details/gnhezmfgs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.sjlbkw.cn/Article/details/gjdzidrrw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.vehdjk.com/Article/details/grbvlivjk.sHtML

Java: import java.util.List;
来源：http://read.share.fktsv.cn/Article/details/gswjcelvv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.epnwcf.com/Article/details/ggqkezlph.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/gnzgyefaq.sHtML

C#:   using System.Text;
来源：http://www.share.vehdjk.com/Article/details/gfoikcxdb.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.epnwcf.com/Article/details/gxgoibpqf.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.epnwcf.com/Article/details/gxfhavfpp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.epnwcf.com/Article/details/gkvgsfxhv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzaqcryv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.bbcook.cn/Article/details/glmgagztp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.sjlbkw.cn/Article/details/gxqijzawy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.bbcook.cn/Article/details/giqjulcjn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fktsv.cn/Article/details/gbhvrdqle.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.tarul.cn/Article/details/gvtvctvzi.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.tarul.cn/Article/details/gdwdfnjik.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.yfazqb.com/Article/details/gootzcisj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gbucikdye.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.yfazqb.com/Article/details/gzzbctqfu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/genrbsqml.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gevfuhjef.sHtML

Go:   func add(a, b int) int
来源：http://blog.vehdjk.com/Article/details/gafhcadur.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.sjlbkw.cn/Article/details/geefsiute.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.bbcook.cn/Article/details/gstogwohz.sHtML

[C14] 泛型函数
来源：http://m.share.yfazqb.com/Article/details/gyzqkrikx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.sjlbkw.cn/Article/details/grtkpsneu.sHtML

PHP:  // 无泛型
来源：http://www.share.fktsv.cn/Article/details/gqivuuezi.sHtML

JS:   // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gpqpudzro.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcbnoyayl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.sjlbkw.cn/Article/details/ghlllgddn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.bbcook.cn/Article/details/gcrjxkgce.sHtML

Ruby: # 无泛型
来源：http://www.share.fktsv.cn/Article/details/gdrxkyect.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.yfazqb.com/Article/details/gkzkrvjmv.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.tarul.cn/Article/details/gxofeqpip.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fktsv.cn/Article/details/gncfzqxkh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fktsv.cn/Article/details/gddgulmjh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmojotayp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvijkhfgb.sHtML

Java: // 无解构
来源：http://baike.bbcook.cn/Article/details/gijujenps.sHtML

Go:   // 无解构
来源：http://baike.tarul.cn/Article/details/gllhkdrqs.sHtML

Ruby: a, b = pair
来源：http://blog.epnwcf.com/Article/details/giwvyrlwc.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.yfazqb.com/Article/details/gskwrxxvi.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.bbcook.cn/Article/details/gaigtbbno.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.yfazqb.com/Article/details/gihgxyszh.sHtML

PHP:  // 无重载
来源：http://wap.tarul.cn/Article/details/gtcfefdgq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fktsv.cn/Article/details/gknajidyu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gdihxnyel.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.yfazqb.com/Article/details/ggczkbbly.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.bbcook.cn/Article/details/gsiwzhfic.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.bbcook.cn/Article/details/gepqsfolu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.tarul.cn/Article/details/gbyafgdls.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gtsjmgmfz.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.yfazqb.com/Article/details/gfantfuka.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gpiprntpc.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnbysrvv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.sjlbkw.cn/Article/details/ggzjwqloq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.yfazqb.com/Article/details/gbkkfoqaz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.vehdjk.com/Article/details/gqebezfme.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.tarul.cn/Article/details/gvulzlqkt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.tarul.cn/Article/details/gahgapwqa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/gcqznxtli.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.bbcook.cn/Article/details/gwnoohyvq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.vehdjk.com/Article/details/gzwmsnhtx.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.yfazqb.com/Article/details/gbgpcyurl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.tarul.cn/Article/details/gofrgatrc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.yfazqb.com/Article/details/gkabfjgwb.sHtML

JS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gavcxnwvq.sHtML

TS:   arr.push(4);
来源：http://3g.vehdjk.com/Article/details/gifvnywvn.sHtML

Java: list.add(4);
来源：http://m.share.vehdjk.com/Article/details/gcbdnmqbe.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.vehdjk.com/Article/details/gckhzwufk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.sjlbkw.cn/Article/details/gttyswajn.sHtML

C#:   list.Add(4);
来源：http://read.share.sjlbkw.cn/Article/details/gwolvoixr.sHtML

[D03] 在指定位置插入元素
来源：http://baike.tarul.cn/Article/details/gshuwetww.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/giwjwshzi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.bbcook.cn/Article/details/gteahords.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fktsv.cn/Article/details/gvzrywauc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.epnwcf.com/Article/details/gsttaknzy.sHtML

Java: list.add(0, 0);
来源：http://read.share.fktsv.cn/Article/details/glwqqulye.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.epnwcf.com/Article/details/gqmdpsodc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.bbcook.cn/Article/details/gbwsecwrk.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/gncmuyjol.sHtML

[D04] 删除元素
来源：http://wap.bbcook.cn/Article/details/gvpqczgzf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fktsv.cn/Article/details/gdfxwmufd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.tarul.cn/Article/details/gakjyiswm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.yfazqb.com/Article/details/gjaxpbulc.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.tarul.cn/Article/details/golifmrog.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.sjlbkw.cn/Article/details/giexcklmc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.yfazqb.com/Article/details/gonjmplcf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.yfazqb.com/Article/details/ggfsdndsh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.yfazqb.com/Article/details/gptdozryn.sHtML

[D05] 访问与修改元素
来源：http://mobile.vehdjk.com/Article/details/gzprqgeeb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gozlyokvh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gjukhmytk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gyodysiqw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.vehdjk.com/Article/details/gugxgsqmv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.sjlbkw.cn/Article/details/gshansbkr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gojbjchyb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gaeqgofga.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.tarul.cn/Article/details/gtcaoxjxi.sHtML

[D06] 数组长度
来源：http://mobile.epnwcf.com/Article/details/ggjvpojhk.sHtML

Py:   len(arr)
来源：http://3g.tarul.cn/Article/details/gwmvznhlt.sHtML

PHP:  count($arr);
来源：http://baike.bbcook.cn/Article/details/gxucfqkss.sHtML

JS:   arr.length
来源：http://3g.sjlbkw.cn/Article/details/ggionoliz.sHtML

TS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gtkdqmcif.sHtML

Java: list.size();
来源：http://baike.bbcook.cn/Article/details/gbfbclekq.sHtML

Go:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/gccxmvkjn.sHtML

Ruby: arr.length; arr.size
来源：http://wap.bbcook.cn/Article/details/guyjkwkds.sHtML

C#:   list.Count;
来源：http://m.share.yfazqb.com/Article/details/gdxraajei.sHtML

[D07] 切片 / 取子数组
来源：http://wap.epnwcf.com/Article/details/gxsyzpgbl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/gxbfvucva.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fktsv.cn/Article/details/gkcpodkwo.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnxkhcrr.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.bbcook.cn/Article/details/gsihtlgnv.sHtML

Java: list.subList(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gnssfzvqc.sHtML

Go:   arr[1:4]
来源：http://mobile.fktsv.cn/Article/details/getamckmr.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.bbcook.cn/Article/details/gawbmxkwx.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.vehdjk.com/Article/details/gjzmclfbo.sHtML

[D08] 合并两个数组
来源：http://m.share.fktsv.cn/Article/details/gcjbihsfm.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.bbcook.cn/Article/details/gfpusgyhd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.yfazqb.com/Article/details/gwohclcyj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.tarul.cn/Article/details/giqdcrnhb.sHtML

TS:   [...a, ...b];
来源：http://mobile.fktsv.cn/Article/details/gotnlteil.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.epnwcf.com/Article/details/gsrpnobiu.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fktsv.cn/Article/details/grnpctaft.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fktsv.cn/Article/details/gwkdbhsuy.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.yfazqb.com/Article/details/gwqfzdhcu.sHtML

[D09] 排序（升序）
来源：http://3g.yfazqb.com/Article/details/gcrdkvcjr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/gqtorhlch.sHtML

PHP:  sort($arr);
来源：http://wap.sjlbkw.cn/Article/details/gpiydkmxz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.epnwcf.com/Article/details/gbiejbrnm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fktsv.cn/Article/details/grpmfidyo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fktsv.cn/Article/details/guczglycv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/gncvqzfci.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gucsckvjf.sHtML

C#:   list.Sort();
来源：http://wap.epnwcf.com/Article/details/grxdurili.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fktsv.cn/Article/details/ggkvtmkfm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.epnwcf.com/Article/details/gabvcpkqu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fktsv.cn/Article/details/glolykpuq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/guhpxdmzp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gfowjydsy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.sjlbkw.cn/Article/details/guzhpsxcj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.vehdjk.com/Article/details/gmaivcruh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.vehdjk.com/Article/details/gsjpblxes.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.vehdjk.com/Article/details/gkkhzncxm.sHtML

[D11] 反转数组
来源：http://blog.sjlbkw.cn/Article/details/glzhmihiw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fktsv.cn/Article/details/gweczhgnl.sHtML

PHP:  array_reverse($arr);
来源：http://blog.vehdjk.com/Article/details/gzeslqsmy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.yfazqb.com/Article/details/gdhbyyzwv.sHtML

TS:   [...arr].reverse();
来源：http://blog.tarul.cn/Article/details/gxlamaiou.sHtML

Java: Collections.reverse(list);
来源：http://m.share.yfazqb.com/Article/details/gsoekihug.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.yfazqb.com/Article/details/gfjxqixtf.sHtML

Ruby: arr.reverse
来源：http://www.share.vehdjk.com/Article/details/gtshonzed.sHtML

C#:   list.Reverse();
来源：http://read.share.tarul.cn/Article/details/gdzvxaqxx.sHtML

[D12] 查找元素下标
来源：http://read.share.bbcook.cn/Article/details/grhdvcurl.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fktsv.cn/Article/details/getupzdsw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.tarul.cn/Article/details/gybfcbqbv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/gjcfgzhvi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.sjlbkw.cn/Article/details/ghopwhyxu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fktsv.cn/Article/details/gcxwqxwdd.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.tarul.cn/Article/details/gtxwloqdd.sHtML

Ruby: arr.index(x)
来源：http://wap.fktsv.cn/Article/details/gigzbclmr.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.yfazqb.com/Article/details/gfynxzkyi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.vehdjk.com/Article/details/gicffoyrb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fktsv.cn/Article/details/gbdimrwuy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.yfazqb.com/Article/details/gnjpdbuib.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/gshbixlre.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/ggkmipxiq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.tarul.cn/Article/details/gjoltmldj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.sjlbkw.cn/Article/details/gvchfvxwx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.bbcook.cn/Article/details/gutmuhqic.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.vehdjk.com/Article/details/gzrsmhwhv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fktsv.cn/Article/details/gzzuaqryf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fktsv.cn/Article/details/gcxikxmsc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.yfazqb.com/Article/details/gaqizaegx.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fktsv.cn/Article/details/gaxwzqvzm.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/gjdvkyoii.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gxkfvhilp.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/gkqacdnuj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.vehdjk.com/Article/details/gttlnustj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gaagaemli.sHtML

[D15] 去重
来源：http://wap.sjlbkw.cn/Article/details/gqvoihosh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/glftbommo.sHtML

PHP:  array_unique($arr);
来源：http://m.share.yfazqb.com/Article/details/gjqehwppx.sHtML

JS:   [...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gzodwmopj.sHtML

TS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/ghxdefucw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.tarul.cn/Article/details/gpqphkeqb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fktsv.cn/Article/details/ggdvrvrfj.sHtML

Ruby: arr.uniq
来源：http://baike.vehdjk.com/Article/details/gidfvomcc.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.vehdjk.com/Article/details/ghlnmqkit.sHtML

[D16] 求和与平均值
来源：http://baike.yfazqb.com/Article/details/govjiteno.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.tarul.cn/Article/details/gcbhfgpfw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.epnwcf.com/Article/details/gjyoublat.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.vehdjk.com/Article/details/gvlphtbtn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gqnzzcnyt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.sjlbkw.cn/Article/details/gbkrvngnu.sHtML

Go:   // 手写循环累加
来源：http://blog.vehdjk.com/Article/details/gmlqpxuzt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.sjlbkw.cn/Article/details/glcjjigjd.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.bbcook.cn/Article/details/gmepibwvp.sHtML

[D17] 最大值与最小值
来源：http://read.share.yfazqb.com/Article/details/gnsshpsya.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gdjjpznur.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.vehdjk.com/Article/details/gvhfpveuh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.vehdjk.com/Article/details/gqdgimgby.sHtML

TS:   Math.max(...arr);
来源：http://3g.tarul.cn/Article/details/gyccwnhok.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fktsv.cn/Article/details/gzggjyell.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.epnwcf.com/Article/details/gqgspopvj.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.sjlbkw.cn/Article/details/grdkbnfll.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.vehdjk.com/Article/details/gxngwnvut.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.sjlbkw.cn/Article/details/gsekwcmeg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.sjlbkw.cn/Article/details/gfzgutlyu.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.bbcook.cn/Article/details/goizbfrhu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fktsv.cn/Article/details/gjgccxmoi.sHtML

TS:   nested.flat();
来源：http://mobile.fktsv.cn/Article/details/gwklleqpr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.sjlbkw.cn/Article/details/gpwmwboel.sHtML

Go:   // 手写双层循环
来源：http://baike.tarul.cn/Article/details/ghxkdsmbf.sHtML

Ruby: nested.flatten
来源：http://baike.yfazqb.com/Article/details/ghhqxodmd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gpmwmrcfn.sHtML

[D19] 按字段分组
来源：http://3g.vehdjk.com/Article/details/gqzbssnlo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.bbcook.cn/Article/details/glfvlvuiy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.vehdjk.com/Article/details/gtfvofhss.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.tarul.cn/Article/details/gdwrymtwv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.yfazqb.com/Article/details/gepfumbwc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.sjlbkw.cn/Article/details/gyxihqape.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.yfazqb.com/Article/details/goninodwh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fktsv.cn/Article/details/gillwbxfi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.bbcook.cn/Article/details/gffpsedhe.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.tarul.cn/Article/details/ggynmpaqq.sHtML

Py:   Counter(arr)
来源：http://read.share.sjlbkw.cn/Article/details/girsljyua.sHtML

PHP:  array_count_values($arr);
来源：http://wap.epnwcf.com/Article/details/gxfbujuio.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/gwyzflpsi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/gmioltlbv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fktsv.cn/Article/details/gzqpupuhh.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.bbcook.cn/Article/details/gxxqdxden.sHtML

Ruby: arr.tally
来源：http://blog.vehdjk.com/Article/details/gunrkflle.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.epnwcf.com/Article/details/gyddtholm.sHtML

[D21] 判断是否包含某元素
来源：http://baike.epnwcf.com/Article/details/gcugnlmgk.sHtML

Py:   x in arr
来源：http://www.m.share.bbcook.cn/Article/details/gctlmihod.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.sjlbkw.cn/Article/details/gzuxtijsw.sHtML

JS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/gbgyhxekp.sHtML

TS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/gfuchbdjb.sHtML

Java: list.contains(x)
来源：http://wap.bbcook.cn/Article/details/gixxdyjbw.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fktsv.cn/Article/details/govpboovp.sHtML

Ruby: arr.include?(x)
来源：http://baike.yfazqb.com/Article/details/gmdbxclwc.sHtML

C#:   list.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gjhlhbnpc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fktsv.cn/Article/details/gzrngrysk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzpogsdh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.yfazqb.com/Article/details/gclsmcmwq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.tarul.cn/Article/details/gqpymmeab.sHtML

TS:   [...arr];
来源：http://m.share.epnwcf.com/Article/details/gfmcwtqni.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.epnwcf.com/Article/details/gacnqlcpf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.epnwcf.com/Article/details/gxhhuaqbu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.bbcook.cn/Article/details/gtlsdfdhk.sHtML

C#:   new List<int>(list);
来源：http://www.share.vehdjk.com/Article/details/ggxtjjomf.sHtML


<!-- 参考信息 -->