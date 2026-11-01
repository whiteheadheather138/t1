代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://wap.epnwcf.com/Article/details/gsgkauywy.sHtML

[C03] 可变参数
来源：http://mobile.fktsv.cn/Article/details/gcwgohokk.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.tarul.cn/Article/details/ggtbsdwhh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.bbcook.cn/Article/details/gepozgpic.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gcbhngest.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gwubqzoiy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.sjlbkw.cn/Article/details/gujczszai.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.bbcook.cn/Article/details/gvpmchcux.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fktsv.cn/Article/details/gvqrkmllc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.yfazqb.com/Article/details/gvcrmbdux.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.yfazqb.com/Article/details/gktqxfljj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.tarul.cn/Article/details/ghtnmgilv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.epnwcf.com/Article/details/gyusqtqcd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gezhhtbqw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.yfazqb.com/Article/details/ghgrquwtp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fktsv.cn/Article/details/gdktukgmn.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.tarul.cn/Article/details/gwulnrulx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gbhbhlhuu.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/ghzpkgpny.sHtML

[C05] 返回多个值
来源：http://www.share.bbcook.cn/Article/details/gpoklqdva.sHtML

Py:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/ghdmyipie.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.epnwcf.com/Article/details/ggsrdzxwh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gzetgdrjq.sHtML

TS:   return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gdoaqishx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.vehdjk.com/Article/details/gqrqjmspb.sHtML

Go:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gmeakhnii.sHtML

Ruby: return a, b
来源：http://3g.bbcook.cn/Article/details/ggkceozan.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.epnwcf.com/Article/details/grcxknkjo.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.vehdjk.com/Article/details/ggqwtsxpn.sHtML

Py:   square = lambda x: x * x
来源：http://blog.sjlbkw.cn/Article/details/gurbpkzyt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.sjlbkw.cn/Article/details/ghstqcyvj.sHtML

JS:   const square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/gedklwbby.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.bbcook.cn/Article/details/gyupoavdp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.yfazqb.com/Article/details/gbmdhnitm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.tarul.cn/Article/details/gvafpvwpg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.bbcook.cn/Article/details/gysgosscf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gtyimxfkr.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.bbcook.cn/Article/details/glfpgwkkl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.sjlbkw.cn/Article/details/gftslckrt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gmswceawf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.sjlbkw.cn/Article/details/girtutkxt.sHtML

TS:   arr.map(String)
来源：http://read.share.vehdjk.com/Article/details/gpsnjhsqy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gbuydyyok.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fktsv.cn/Article/details/gctmoewqi.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.tarul.cn/Article/details/guwdsnqpt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.tarul.cn/Article/details/glufzdgfl.sHtML

[C08] 闭包
来源：http://wap.sjlbkw.cn/Article/details/goaewhgii.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.epnwcf.com/Article/details/gbfhgzvse.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.epnwcf.com/Article/details/guykudtmx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gbraevati.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gzdkvjdvv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.tarul.cn/Article/details/ghxsuwkej.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.epnwcf.com/Article/details/gcgtpuyqu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.yfazqb.com/Article/details/ggsdbulfs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gmsehpdua.sHtML

[C09] 递归
来源：http://www.share.yfazqb.com/Article/details/gsaimokns.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fktsv.cn/Article/details/gyuberdic.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/gwtosypro.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gobhzzymp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.vehdjk.com/Article/details/ghzsmfdiq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.yfazqb.com/Article/details/gbhcyomjt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/glcagwpgo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gngdvggxw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.bbcook.cn/Article/details/gtppewazj.sHtML

[C10] 变量作用域
来源：http://wap.fktsv.cn/Article/details/ghruyzwxf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.epnwcf.com/Article/details/grbszszvr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.bbcook.cn/Article/details/grswlnnuc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/gnotyejzi.sHtML

TS:   同 JS
来源：http://wap.tarul.cn/Article/details/gljqiapfb.sHtML

Java: 方法内为块级作用域
来源：http://baike.tarul.cn/Article/details/grlbevoba.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gtrexdxlk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fktsv.cn/Article/details/gjjrsljei.sHtML

C#:   块级作用域
来源：http://www.share.fktsv.cn/Article/details/gzxtrilcm.sHtML

[C11] 模块导入与导出
来源：http://read.share.bbcook.cn/Article/details/gvxhmolvb.sHtML

Py:   from module import func
来源：http://wap.sjlbkw.cn/Article/details/glqhmtgue.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.epnwcf.com/Article/details/gjofqdcko.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.epnwcf.com/Article/details/glwaplhmk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.tarul.cn/Article/details/gyjejmmiq.sHtML

Java: import java.util.List;
来源：http://mobile.fktsv.cn/Article/details/gxecucjgo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.vehdjk.com/Article/details/gkdbqhmzs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.epnwcf.com/Article/details/gekfcskog.sHtML

C#:   using System.Text;
来源：http://wap.fktsv.cn/Article/details/givzqcycs.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.vehdjk.com/Article/details/gldoavspf.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fktsv.cn/Article/details/gejasjrbo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.epnwcf.com/Article/details/gxncwundl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/gwtuseapg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gisbvuxtu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.sjlbkw.cn/Article/details/gkosdjzko.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fktsv.cn/Article/details/gkvnpbsri.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.bbcook.cn/Article/details/gmxifbezs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.sjlbkw.cn/Article/details/gyvxozriv.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.tarul.cn/Article/details/gdeentyzu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.yfazqb.com/Article/details/gozmfptpr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gbwxaszdi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.bbcook.cn/Article/details/gtcmvlbjj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/guyxifbie.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/guzajpxug.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/ghzcvrqkc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.epnwcf.com/Article/details/gpsnskofi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.bbcook.cn/Article/details/geqbitlnf.sHtML

[C14] 泛型函数
来源：http://www.m.share.tarul.cn/Article/details/ggujtpexn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.sjlbkw.cn/Article/details/gmeskftfu.sHtML

PHP:  // 无泛型
来源：http://www.share.yfazqb.com/Article/details/gzssipnhq.sHtML

JS:   // 无泛型
来源：http://m.share.fktsv.cn/Article/details/ghxuyntsv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.epnwcf.com/Article/details/gobjbaycb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.vehdjk.com/Article/details/glbqxoava.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.vehdjk.com/Article/details/gcwjgxqqx.sHtML

Ruby: # 无泛型
来源：http://wap.tarul.cn/Article/details/gvzoanvbx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.sjlbkw.cn/Article/details/gcewpbbma.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.yfazqb.com/Article/details/gbpwfwsxi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.bbcook.cn/Article/details/gxtmciqzf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fktsv.cn/Article/details/gfboumaet.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/gjavxvnal.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fktsv.cn/Article/details/gtmdedopu.sHtML

Java: // 无解构
来源：http://wap.tarul.cn/Article/details/gixynfmas.sHtML

Go:   // 无解构
来源：http://wap.sjlbkw.cn/Article/details/gpoovdhna.sHtML

Ruby: a, b = pair
来源：http://read.share.epnwcf.com/Article/details/gaqbtwxii.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.yfazqb.com/Article/details/gqgfvmwvh.sHtML

[C16] 函数 / 方法重载
来源：http://blog.sjlbkw.cn/Article/details/gdjmevzbo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.epnwcf.com/Article/details/gmwapbxtd.sHtML

PHP:  // 无重载
来源：http://read.share.sjlbkw.cn/Article/details/gidfnayrs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.bbcook.cn/Article/details/ggcyarfjm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.sjlbkw.cn/Article/details/gzpgpgoko.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.yfazqb.com/Article/details/gjzxkcyqw.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.epnwcf.com/Article/details/goeuzupql.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fktsv.cn/Article/details/gnoovlegh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.sjlbkw.cn/Article/details/gbhggezmj.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gaglwufvq.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.tarul.cn/Article/details/gtvsompdg.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqffwbzsa.sHtML

[D01] 创建数组 / 列表
来源：http://blog.sjlbkw.cn/Article/details/ghhcatefq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.vehdjk.com/Article/details/goampcpbj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.epnwcf.com/Article/details/gxwbbbyit.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/gxtboctfl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.yfazqb.com/Article/details/guuryljdq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.epnwcf.com/Article/details/gqjpsearl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.yfazqb.com/Article/details/ggwqjilkr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.sjlbkw.cn/Article/details/gjhhzuvyw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.epnwcf.com/Article/details/gyysuynpz.sHtML

[D02] 追加元素到末尾
来源：http://3g.sjlbkw.cn/Article/details/ghjzvcmnf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.sjlbkw.cn/Article/details/gbypudnob.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.yfazqb.com/Article/details/gzgpajxaa.sHtML

JS:   arr.push(4);
来源：http://baike.sjlbkw.cn/Article/details/gskpqbvsd.sHtML

TS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/gwkmpmjkb.sHtML

Java: list.add(4);
来源：http://mobile.tarul.cn/Article/details/gbhjperup.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gqqsqkxdx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.sjlbkw.cn/Article/details/ghleqqqzm.sHtML

C#:   list.Add(4);
来源：http://wap.vehdjk.com/Article/details/gogkrbeci.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.sjlbkw.cn/Article/details/gxszalmdd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.yfazqb.com/Article/details/gpebcjxmv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.tarul.cn/Article/details/gvyxjoltk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.tarul.cn/Article/details/gdiinddev.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.yfazqb.com/Article/details/gbzutxgiw.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/grxrvlxko.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.vehdjk.com/Article/details/geslzppke.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.vehdjk.com/Article/details/gnnamqemm.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.vehdjk.com/Article/details/gmnirroau.sHtML

[D04] 删除元素
来源：http://read.share.fktsv.cn/Article/details/gndkvgeqz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.epnwcf.com/Article/details/ggikqbigi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.vehdjk.com/Article/details/gvgdqitxh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.vehdjk.com/Article/details/guaqffoys.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzdqavfi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.bbcook.cn/Article/details/gtozpydyv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.bbcook.cn/Article/details/gtgzadtmn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.yfazqb.com/Article/details/gdycyurbj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.yfazqb.com/Article/details/gbrzuvbia.sHtML

[D05] 访问与修改元素
来源：http://m.share.sjlbkw.cn/Article/details/guzdwrpmy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gtfqscknt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/gahbktmmt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/govegdnld.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.vehdjk.com/Article/details/ghwpccrid.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.yfazqb.com/Article/details/gmbffqare.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/ghgplpkzr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gglmcqdjo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gldzyrqow.sHtML

[D06] 数组长度
来源：http://mobile.epnwcf.com/Article/details/gxwxaxknn.sHtML

Py:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/gxdigmduz.sHtML

PHP:  count($arr);
来源：http://blog.sjlbkw.cn/Article/details/gjxtwprcy.sHtML

JS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gsvgtathj.sHtML

TS:   arr.length
来源：http://www.m.share.fktsv.cn/Article/details/gciwvjldb.sHtML

Java: list.size();
来源：http://wap.bbcook.cn/Article/details/glcjixsfy.sHtML

Go:   len(arr)
来源：http://www.blog.epnwcf.com/Article/details/ginfjvtub.sHtML

Ruby: arr.length; arr.size
来源：http://3g.yfazqb.com/Article/details/gawlnxkir.sHtML

C#:   list.Count;
来源：http://mobile.sjlbkw.cn/Article/details/gnpxucwff.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.yfazqb.com/Article/details/gvcmusmku.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.tarul.cn/Article/details/grucdfamz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fktsv.cn/Article/details/ghnwhwdgk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gwfnduird.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gfipbrmhu.sHtML

Java: list.subList(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gbsxrtpkz.sHtML

Go:   arr[1:4]
来源：http://wap.sjlbkw.cn/Article/details/gmjgivcrs.sHtML

Ruby: arr[1, 3]
来源：http://read.share.epnwcf.com/Article/details/gpaenofxw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gmfpwiorj.sHtML

[D08] 合并两个数组
来源：http://3g.yfazqb.com/Article/details/gnpcgibao.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.epnwcf.com/Article/details/ghtbppnuh.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fktsv.cn/Article/details/gkvemgevo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.bbcook.cn/Article/details/gslrwmmmf.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbhpbrqg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gdnqpecsx.sHtML

Go:   append(a, b...)
来源：http://blog.sjlbkw.cn/Article/details/ginfiuewz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.tarul.cn/Article/details/grgroqnja.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.tarul.cn/Article/details/gcnlbaodn.sHtML

[D09] 排序（升序）
来源：http://mobile.yfazqb.com/Article/details/gryuolevy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.sjlbkw.cn/Article/details/gvmnxkedn.sHtML

PHP:  sort($arr);
来源：http://blog.epnwcf.com/Article/details/glyconyva.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.epnwcf.com/Article/details/gcrzwujqr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fktsv.cn/Article/details/guphfncra.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.sjlbkw.cn/Article/details/gudsdavrq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/ghzzngjos.sHtML

Ruby: arr.sort
来源：http://3g.fktsv.cn/Article/details/gvassqwjz.sHtML

C#:   list.Sort();
来源：http://www.blog.tarul.cn/Article/details/gynsqvaig.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.vehdjk.com/Article/details/gelbbtbvi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.yfazqb.com/Article/details/gvjknoown.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.vehdjk.com/Article/details/gmytdgico.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/gucocybvu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gmwsmdzwz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.bbcook.cn/Article/details/gxxoccfxi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.tarul.cn/Article/details/gwvhtiflz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.vehdjk.com/Article/details/guhsitrky.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.epnwcf.com/Article/details/gbapsekep.sHtML

[D11] 反转数组
来源：http://m.share.epnwcf.com/Article/details/givclffpq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.sjlbkw.cn/Article/details/gokumnzse.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.bbcook.cn/Article/details/gssrekhkr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.sjlbkw.cn/Article/details/gglkwbhbf.sHtML

TS:   [...arr].reverse();
来源：http://m.share.sjlbkw.cn/Article/details/gehysxpmb.sHtML

Java: Collections.reverse(list);
来源：http://3g.tarul.cn/Article/details/gmyfpwwqw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.yfazqb.com/Article/details/gwvdkncwe.sHtML

Ruby: arr.reverse
来源：http://m.share.fktsv.cn/Article/details/grwfxdauy.sHtML

C#:   list.Reverse();
来源：http://www.blog.yfazqb.com/Article/details/gabbatwfl.sHtML

[D12] 查找元素下标
来源：http://www.share.epnwcf.com/Article/details/gkjkffoqa.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.yfazqb.com/Article/details/gqbvreusw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.epnwcf.com/Article/details/gztkjypsv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.bbcook.cn/Article/details/gqazaukzl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.epnwcf.com/Article/details/gqgtsakpw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.bbcook.cn/Article/details/ggridjoxs.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gagddaslc.sHtML

Ruby: arr.index(x)
来源：http://blog.tarul.cn/Article/details/gcnfuwqbm.sHtML

C#:   list.IndexOf(x);
来源：http://baike.yfazqb.com/Article/details/gdgzitlky.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.tarul.cn/Article/details/gjmhomytm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.bbcook.cn/Article/details/geivktvwy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.yfazqb.com/Article/details/gyjjpkigc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.bbcook.cn/Article/details/gobzjfqbi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gtdwwldpj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.vehdjk.com/Article/details/goxggmdab.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.tarul.cn/Article/details/gqxbrytgx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.vehdjk.com/Article/details/grqqyhmnu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.tarul.cn/Article/details/gackpcdcl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.tarul.cn/Article/details/gsgyjanzh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.vehdjk.com/Article/details/gpyjllzbx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.tarul.cn/Article/details/ggyiziytx.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/gasalbnny.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/gwzzzhisx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.tarul.cn/Article/details/gztxabqmf.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/gviioaprk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/geretcppn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.tarul.cn/Article/details/gnqsenjcw.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/ghmgjvzxx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/ghikqczjw.sHtML

PHP:  array_unique($arr);
来源：http://m.share.bbcook.cn/Article/details/gwupoinpa.sHtML

JS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gzeknzica.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/glkygyadn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.epnwcf.com/Article/details/gojldtajw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.sjlbkw.cn/Article/details/gcaxexnwp.sHtML

Ruby: arr.uniq
来源：http://www.blog.bbcook.cn/Article/details/ggxjeuajb.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gmcrqfjxd.sHtML

[D16] 求和与平均值
来源：http://www.m.share.tarul.cn/Article/details/gekpqbvnl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.epnwcf.com/Article/details/gqivuxuao.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.tarul.cn/Article/details/gqdlshqrm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.vehdjk.com/Article/details/gqvgjtslg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/gfxcnopqc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.vehdjk.com/Article/details/gqlefgqdf.sHtML

Go:   // 手写循环累加
来源：http://www.blog.sjlbkw.cn/Article/details/gdzbnuccm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fktsv.cn/Article/details/gixxvrlwn.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/gqcrziifz.sHtML

[D17] 最大值与最小值
来源：http://read.share.fktsv.cn/Article/details/gkbiutcss.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.vehdjk.com/Article/details/gshcykkzn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gsigzmeiv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gstgspjfy.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fktsv.cn/Article/details/gwrcnuyro.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.sjlbkw.cn/Article/details/gcnrzyxbl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.epnwcf.com/Article/details/gqrpuwgnv.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.vehdjk.com/Article/details/gkvgsagof.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.yfazqb.com/Article/details/gdgjcsvyv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.vehdjk.com/Article/details/gfgpyjsvy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.vehdjk.com/Article/details/gybelvwgd.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.bbcook.cn/Article/details/gmsqcjzpr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.yfazqb.com/Article/details/gnhxnwjvy.sHtML

TS:   nested.flat();
来源：http://wap.fktsv.cn/Article/details/gurbuvgtb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.epnwcf.com/Article/details/gmmzkozvj.sHtML

Go:   // 手写双层循环
来源：http://wap.epnwcf.com/Article/details/gekpscaxg.sHtML

Ruby: nested.flatten
来源：http://m.share.sjlbkw.cn/Article/details/gflvuznfc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.epnwcf.com/Article/details/gufndfcph.sHtML

[D19] 按字段分组
来源：http://blog.fktsv.cn/Article/details/gleybhfrg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fktsv.cn/Article/details/gbkgjzkso.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.sjlbkw.cn/Article/details/gjifqovzp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.sjlbkw.cn/Article/details/ghdflypsd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/glvlgyaxp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.yfazqb.com/Article/details/gteatcfop.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fktsv.cn/Article/details/giwnsjnzr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.tarul.cn/Article/details/gsrnmbpun.sHtML


<!-- 参考信息 -->