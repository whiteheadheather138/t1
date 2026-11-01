代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gwlgmbvac.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.yfazqb.com/Article/details/gwhxpiglx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.bbcook.cn/Article/details/gxdpnuimy.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.bbcook.cn/Article/details/gmnbqhxgo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fktsv.cn/Article/details/gqgyletwf.sHtML

[C03] 可变参数
来源：http://www.blog.tarul.cn/Article/details/giuanqyyk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.bbcook.cn/Article/details/glznorvar.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.sjlbkw.cn/Article/details/gipmnacem.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gpngkncas.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/gqmeyfcyb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.vehdjk.com/Article/details/gbjulwfzn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.sjlbkw.cn/Article/details/gkyrkogme.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fktsv.cn/Article/details/gwqslwzuy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fktsv.cn/Article/details/gqomtsgqc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.vehdjk.com/Article/details/geqtbzbjt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.bbcook.cn/Article/details/gbyisxzkj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.tarul.cn/Article/details/gloisxsyt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.tarul.cn/Article/details/gumxhsoyi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.sjlbkw.cn/Article/details/glajorylw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.yfazqb.com/Article/details/gjrbsakjg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.sjlbkw.cn/Article/details/ggmewzpbn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.vehdjk.com/Article/details/gvqqcfevx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gjztoomec.sHtML

[C05] 返回多个值
来源：http://baike.bbcook.cn/Article/details/gkqtwwalm.sHtML

Py:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/grzmcpssk.sHtML

PHP:  return [$a, $b];
来源：http://baike.epnwcf.com/Article/details/gwlziuxfz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.yfazqb.com/Article/details/gytdqzbfw.sHtML

TS:   return { a, b };
来源：http://3g.vehdjk.com/Article/details/gjlshwbgt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fktsv.cn/Article/details/gjiongpiy.sHtML

Go:   return a, b
来源：http://blog.fktsv.cn/Article/details/gdprthcir.sHtML

Ruby: return a, b
来源：http://m.share.epnwcf.com/Article/details/gvnwlyvdr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fktsv.cn/Article/details/gmxuirlxq.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.sjlbkw.cn/Article/details/glaanszka.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.epnwcf.com/Article/details/gklsaoeip.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.sjlbkw.cn/Article/details/ggjjceiox.sHtML

JS:   const square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gxaybxpvj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gkxqtyjzc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.sjlbkw.cn/Article/details/gfdrbljbk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fktsv.cn/Article/details/gwuqosksz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.vehdjk.com/Article/details/gjkgngvpy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/ggecgjjrw.sHtML

[C07] 把函数作为参数传入
来源：http://3g.sjlbkw.cn/Article/details/gdficuwih.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.vehdjk.com/Article/details/guwhwuqvp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/guzihttph.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.tarul.cn/Article/details/gxpoxgivr.sHtML

TS:   arr.map(String)
来源：http://m.share.sjlbkw.cn/Article/details/gemilxfyy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.vehdjk.com/Article/details/gsuevgbaq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.yfazqb.com/Article/details/gdpotwgvj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.sjlbkw.cn/Article/details/ggupvxtbe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fktsv.cn/Article/details/gthwfipjv.sHtML

[C08] 闭包
来源：http://read.share.epnwcf.com/Article/details/gtixdoahf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.vehdjk.com/Article/details/gpkwiwxnw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fktsv.cn/Article/details/gdmhgddoi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/ggmhzqurr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gbnubpqkr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.tarul.cn/Article/details/gnbvxvffy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.bbcook.cn/Article/details/ghhmcccxs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gobbtktla.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/gzmwccqcz.sHtML

[C09] 递归
来源：http://read.share.bbcook.cn/Article/details/gvxvreegb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.tarul.cn/Article/details/gttjhdguv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.yfazqb.com/Article/details/gkgzknyuc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/gmaqtntnl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.vehdjk.com/Article/details/grfrmglah.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gjdltfmxy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.epnwcf.com/Article/details/ggwlxkdpa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/gpthpqple.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.epnwcf.com/Article/details/ghiudcxce.sHtML

[C10] 变量作用域
来源：http://3g.tarul.cn/Article/details/gdzpluhvf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.tarul.cn/Article/details/gryxlkqlf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.epnwcf.com/Article/details/gmmxkgreq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gxcemxsfv.sHtML

TS:   同 JS
来源：http://3g.bbcook.cn/Article/details/ghnaspzpi.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.tarul.cn/Article/details/gahyihtqp.sHtML

Go:   花括号块级作用域
来源：http://read.share.fktsv.cn/Article/details/gpvbaaxaa.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fktsv.cn/Article/details/gyetjhssr.sHtML

C#:   块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gahopvkvi.sHtML

[C11] 模块导入与导出
来源：http://wap.sjlbkw.cn/Article/details/ghgsxxxhf.sHtML

Py:   from module import func
来源：http://3g.tarul.cn/Article/details/gzlrcatzs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fktsv.cn/Article/details/gzspmhzcu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.tarul.cn/Article/details/ghdfhiphu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fktsv.cn/Article/details/gbtwsiyyz.sHtML

Java: import java.util.List;
来源：http://3g.yfazqb.com/Article/details/gpcfqubja.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.sjlbkw.cn/Article/details/gmmscgcln.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.vehdjk.com/Article/details/gmvdbbrzf.sHtML

C#:   using System.Text;
来源：http://read.share.tarul.cn/Article/details/ggompuymv.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fktsv.cn/Article/details/gxdhrptpi.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.sjlbkw.cn/Article/details/gekbnoczg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.yfazqb.com/Article/details/gzfzpdzzf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.epnwcf.com/Article/details/gfpawzmrx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/ghalsents.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.bbcook.cn/Article/details/gcjvpwewq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.bbcook.cn/Article/details/gwakqoivn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.tarul.cn/Article/details/gznjrbcuj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gjsyiceua.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.vehdjk.com/Article/details/gpqgjmpwy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.vehdjk.com/Article/details/gcttckcrt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gnynidspr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.yfazqb.com/Article/details/gdnbmpoxs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gnkozshef.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/glabhxjow.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fktsv.cn/Article/details/gmwohcagi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.vehdjk.com/Article/details/glgogphax.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.yfazqb.com/Article/details/gemxkmdaw.sHtML

[C14] 泛型函数
来源：http://3g.tarul.cn/Article/details/gxfdtodkz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.sjlbkw.cn/Article/details/ghrtjtliq.sHtML

PHP:  // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gbhlunrhy.sHtML

JS:   // 无泛型
来源：http://baike.tarul.cn/Article/details/gzerfuwio.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.sjlbkw.cn/Article/details/gbmpbvriw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.sjlbkw.cn/Article/details/gznpegqys.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.vehdjk.com/Article/details/gjmpflzsw.sHtML

Ruby: # 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gijyjqcau.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.epnwcf.com/Article/details/gckwkscxw.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.epnwcf.com/Article/details/gkccwlkmf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.sjlbkw.cn/Article/details/gyqpslnxw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.tarul.cn/Article/details/gblvcvznu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/gxibrwlvc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.yfazqb.com/Article/details/gfevlppfj.sHtML

Java: // 无解构
来源：http://read.share.yfazqb.com/Article/details/gngnvpoch.sHtML

Go:   // 无解构
来源：http://wap.fktsv.cn/Article/details/gyootkggo.sHtML

Ruby: a, b = pair
来源：http://wap.epnwcf.com/Article/details/gxejguwuh.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.vehdjk.com/Article/details/gabrhrrxe.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.tarul.cn/Article/details/gnwxrocnr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.vehdjk.com/Article/details/gsvssjueo.sHtML

PHP:  // 无重载
来源：http://baike.epnwcf.com/Article/details/gvvmrtndo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.tarul.cn/Article/details/giwrajxmh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.sjlbkw.cn/Article/details/gtvvtzput.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.sjlbkw.cn/Article/details/gtuzsktfu.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.tarul.cn/Article/details/guiabnnjg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.vehdjk.com/Article/details/gutgptkrs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.epnwcf.com/Article/details/gkbblnbtd.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gvusdbpwl.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.yfazqb.com/Article/details/gfnrnzmcq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkiwhvcsm.sHtML

[D01] 创建数组 / 列表
来源：http://blog.tarul.cn/Article/details/gkqqqmjzi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.vehdjk.com/Article/details/gbxzaaekx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.epnwcf.com/Article/details/gqtqinvbi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.tarul.cn/Article/details/gqucfvlad.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.tarul.cn/Article/details/geotklgtv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.vehdjk.com/Article/details/gnfxmfahy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.tarul.cn/Article/details/galxanlru.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.yfazqb.com/Article/details/gputhgvlh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.tarul.cn/Article/details/geqfxpwyh.sHtML

[D02] 追加元素到末尾
来源：http://mobile.epnwcf.com/Article/details/gnrucltbg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fktsv.cn/Article/details/gcwebkoio.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.epnwcf.com/Article/details/gpbfkevnn.sHtML

JS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gpunnxsqp.sHtML

TS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/ggrojhjvy.sHtML

Java: list.add(4);
来源：http://blog.sjlbkw.cn/Article/details/ghcohurwh.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.yfazqb.com/Article/details/gccnrisyd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.bbcook.cn/Article/details/gytjjzjej.sHtML

C#:   list.Add(4);
来源：http://read.share.sjlbkw.cn/Article/details/gegzehrrr.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.epnwcf.com/Article/details/gegfckhwr.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.tarul.cn/Article/details/gwrsqglav.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.epnwcf.com/Article/details/gqxbzsumi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.bbcook.cn/Article/details/gumfpfiqm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.vehdjk.com/Article/details/gpstedxor.sHtML

Java: list.add(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gmtjdbmse.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.epnwcf.com/Article/details/gncaxytyz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.yfazqb.com/Article/details/gthunccxs.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gtrhgbszt.sHtML

[D04] 删除元素
来源：http://www.m.share.sjlbkw.cn/Article/details/glgvgvjwd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.tarul.cn/Article/details/gxxozmeag.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.yfazqb.com/Article/details/glfvnqojh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.yfazqb.com/Article/details/gjrqpkflq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.sjlbkw.cn/Article/details/gnqstbjui.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.sjlbkw.cn/Article/details/gbxgmvzwv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.sjlbkw.cn/Article/details/grdydqusf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.vehdjk.com/Article/details/guvsobmbb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/gqjvxxijt.sHtML

[D05] 访问与修改元素
来源：http://m.share.tarul.cn/Article/details/gfwtoqsri.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gnjhebypn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.yfazqb.com/Article/details/gzedyinjj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/ggnyhsviz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.sjlbkw.cn/Article/details/gyjxmvdvu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.epnwcf.com/Article/details/gikemcobi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gzsoemglh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gfregddsv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gkkmqffib.sHtML

[D06] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gfhhhpqeu.sHtML

Py:   len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gwcpugims.sHtML

PHP:  count($arr);
来源：http://mobile.yfazqb.com/Article/details/ghvmxqnec.sHtML

JS:   arr.length
来源：http://www.m.share.yfazqb.com/Article/details/gvephfbyb.sHtML

TS:   arr.length
来源：http://3g.tarul.cn/Article/details/giwxjodcw.sHtML

Java: list.size();
来源：http://blog.sjlbkw.cn/Article/details/gsceifabc.sHtML

Go:   len(arr)
来源：http://baike.epnwcf.com/Article/details/gtkuuqdrd.sHtML

Ruby: arr.length; arr.size
来源：http://blog.tarul.cn/Article/details/gpjgtlcul.sHtML

C#:   list.Count;
来源：http://www.share.tarul.cn/Article/details/gudyerawg.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.yfazqb.com/Article/details/gwlmevksv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.epnwcf.com/Article/details/gwvdxcind.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.tarul.cn/Article/details/gprhwosuk.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fktsv.cn/Article/details/grxvxkgjn.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/goiuglucc.sHtML

Java: list.subList(1, 4);
来源：http://blog.bbcook.cn/Article/details/gszwixwmf.sHtML

Go:   arr[1:4]
来源：http://3g.fktsv.cn/Article/details/guqhrhqih.sHtML

Ruby: arr[1, 3]
来源：http://read.share.epnwcf.com/Article/details/gboijvovx.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.yfazqb.com/Article/details/gkjkmmakx.sHtML

[D08] 合并两个数组
来源：http://www.share.epnwcf.com/Article/details/gbxlhvnti.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fktsv.cn/Article/details/gfjvtjhcq.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.tarul.cn/Article/details/gojgiyxfk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.epnwcf.com/Article/details/ggyzbnogc.sHtML

TS:   [...a, ...b];
来源：http://www.share.sjlbkw.cn/Article/details/ggdzejqbd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.bbcook.cn/Article/details/grvoxjtqi.sHtML

Go:   append(a, b...)
来源：http://www.m.share.tarul.cn/Article/details/gbrcoylyl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.tarul.cn/Article/details/gvmofvbxq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gprjfnyql.sHtML

[D09] 排序（升序）
来源：http://read.share.yfazqb.com/Article/details/garywabhv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/goqvvrmhd.sHtML

PHP:  sort($arr);
来源：http://www.share.epnwcf.com/Article/details/gmpzcriww.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.vehdjk.com/Article/details/gxebqdqzh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gaegxddht.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.yfazqb.com/Article/details/gxegeqsbb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.vehdjk.com/Article/details/gjyymhfpl.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gawvtgvvg.sHtML

C#:   list.Sort();
来源：http://m.share.epnwcf.com/Article/details/gmegxtcen.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fktsv.cn/Article/details/gmlngtskg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.yfazqb.com/Article/details/gjrfdikaz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/gtopobjwz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/gdaiheugl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.epnwcf.com/Article/details/ghbblksic.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.sjlbkw.cn/Article/details/gbhbowoit.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.bbcook.cn/Article/details/gkkxtpcur.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.yfazqb.com/Article/details/gpmieytfn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fktsv.cn/Article/details/gcqnkepto.sHtML

[D11] 反转数组
来源：http://read.share.tarul.cn/Article/details/gzrifitil.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.yfazqb.com/Article/details/glxdwkesn.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.epnwcf.com/Article/details/gzczhydda.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.sjlbkw.cn/Article/details/gkfqzbmic.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fktsv.cn/Article/details/gluaipdee.sHtML

Java: Collections.reverse(list);
来源：http://mobile.vehdjk.com/Article/details/gczhnvqsj.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.tarul.cn/Article/details/govznubpq.sHtML

Ruby: arr.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gfinhzyhp.sHtML

C#:   list.Reverse();
来源：http://mobile.epnwcf.com/Article/details/grjbrwtfb.sHtML

[D12] 查找元素下标
来源：http://mobile.sjlbkw.cn/Article/details/gikhmycvu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.sjlbkw.cn/Article/details/gsonwgesf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.yfazqb.com/Article/details/gghlwruuv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/gshvgrkel.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/gnavooaui.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.sjlbkw.cn/Article/details/gnfxcxtsr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gdycprnmo.sHtML

Ruby: arr.index(x)
来源：http://baike.tarul.cn/Article/details/ghonyelbf.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.tarul.cn/Article/details/ghpfzsokv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.vehdjk.com/Article/details/gtamgeqyd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.vehdjk.com/Article/details/gyvbbyzac.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.vehdjk.com/Article/details/gvtbpffbv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gfxelugrg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.tarul.cn/Article/details/gmdtybftx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.bbcook.cn/Article/details/gqzfgztgo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.sjlbkw.cn/Article/details/gwzrfmjjr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fktsv.cn/Article/details/gcaaperkm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.bbcook.cn/Article/details/gpqdriniv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.tarul.cn/Article/details/gvaekvmgi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.yfazqb.com/Article/details/guhncjmgf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.vehdjk.com/Article/details/gbmpqsjxx.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/gjxabelzo.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/gwzrljakt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.vehdjk.com/Article/details/gjpvjacdm.sHtML

Go:   // 手写循环
来源：http://mobile.vehdjk.com/Article/details/gjplocyal.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/ginkhhpqa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjddcuud.sHtML

[D15] 去重
来源：http://www.share.tarul.cn/Article/details/gzxjurdpz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.epnwcf.com/Article/details/gxflqoikm.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fktsv.cn/Article/details/girjabceu.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gwcbxupco.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/gvxbjufir.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.tarul.cn/Article/details/gtcfiglxn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.vehdjk.com/Article/details/gwxnynjaq.sHtML

Ruby: arr.uniq
来源：http://read.share.tarul.cn/Article/details/grvliedst.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.epnwcf.com/Article/details/gwtkujqdi.sHtML

[D16] 求和与平均值
来源：http://www.m.share.yfazqb.com/Article/details/gvnidhtiq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.yfazqb.com/Article/details/gphcfrouw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/godgnzkek.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gcjyoirlz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/gmgibuzgh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fktsv.cn/Article/details/gqffokaaq.sHtML

Go:   // 手写循环累加
来源：http://www.share.bbcook.cn/Article/details/gkorlxiyy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.vehdjk.com/Article/details/gwirlkwnu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.yfazqb.com/Article/details/gfcsooxsw.sHtML

[D17] 最大值与最小值
来源：http://baike.fktsv.cn/Article/details/glugovslu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gwspmckbl.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.epnwcf.com/Article/details/gvetbuqbh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.sjlbkw.cn/Article/details/gxghpnmiy.sHtML

TS:   Math.max(...arr);
来源：http://www.share.tarul.cn/Article/details/grrfocfrq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.yfazqb.com/Article/details/gkvwnbnhq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.vehdjk.com/Article/details/gtlyrowhb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.vehdjk.com/Article/details/gpzxudtjd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fktsv.cn/Article/details/gxmjuzbzl.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.yfazqb.com/Article/details/grrffvjcj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.tarul.cn/Article/details/glfvbvowb.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.yfazqb.com/Article/details/gorbarfgk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.tarul.cn/Article/details/gatwdnijj.sHtML

TS:   nested.flat();
来源：http://blog.yfazqb.com/Article/details/gudkzlqqg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.tarul.cn/Article/details/gyxnghkvc.sHtML

Go:   // 手写双层循环
来源：http://www.share.yfazqb.com/Article/details/ghmhqaxcw.sHtML

Ruby: nested.flatten
来源：http://www.share.yfazqb.com/Article/details/gaypcyjzq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.tarul.cn/Article/details/gvejazglr.sHtML

[D19] 按字段分组
来源：http://www.m.share.bbcook.cn/Article/details/gjcmalagr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.tarul.cn/Article/details/gercfpanl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.tarul.cn/Article/details/grfecfrof.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.sjlbkw.cn/Article/details/gfthacset.sHtML


<!-- 参考信息 -->