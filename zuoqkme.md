代发 wailian999

Py:   return a, b
来源：http://read.share.tarul.cn/Article/details/gzlwqoapd.sHtML

PHP:  return [$a, $b];
来源：http://www.share.vehdjk.com/Article/details/gnuyiapxw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.bbcook.cn/Article/details/ggpluaice.sHtML

TS:   return { a, b };
来源：http://www.share.tarul.cn/Article/details/gcfblmkku.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.bbcook.cn/Article/details/grvbkwybt.sHtML

Go:   return a, b
来源：http://m.share.vehdjk.com/Article/details/gacctqrkx.sHtML

Ruby: return a, b
来源：http://baike.fktsv.cn/Article/details/gudsuywmj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.tarul.cn/Article/details/gvzsneepz.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/gxgbxehnn.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.vehdjk.com/Article/details/gwkfldevl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fktsv.cn/Article/details/gmfuzgxed.sHtML

JS:   const square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/gumywyrkm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.tarul.cn/Article/details/gwsdzgngy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.tarul.cn/Article/details/glrlfrpkw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.vehdjk.com/Article/details/gqnohmigy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.epnwcf.com/Article/details/gvanocskp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gfcshyjax.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.yfazqb.com/Article/details/gdhxdsfdv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.yfazqb.com/Article/details/grotrrrmi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fktsv.cn/Article/details/ggztppifl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fktsv.cn/Article/details/gogaufcez.sHtML

TS:   arr.map(String)
来源：http://3g.yfazqb.com/Article/details/grfvihfqw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.yfazqb.com/Article/details/gicieyzyw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.vehdjk.com/Article/details/gscwewdkk.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.epnwcf.com/Article/details/gtitnacgi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.sjlbkw.cn/Article/details/ghzvexhcr.sHtML

[C08] 闭包
来源：http://www.blog.vehdjk.com/Article/details/guqatrzyr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fktsv.cn/Article/details/gvldehljy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.yfazqb.com/Article/details/glgxixdbv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gjwzqxnsl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.bbcook.cn/Article/details/gggxbyfen.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.tarul.cn/Article/details/gajgbjqfm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.yfazqb.com/Article/details/gpdqhznky.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.yfazqb.com/Article/details/gypniojkb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gpzzbmrcy.sHtML

[C09] 递归
来源：http://m.share.sjlbkw.cn/Article/details/grinvlapy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gofuseido.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.sjlbkw.cn/Article/details/gvapkosri.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gbqkqeyab.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fktsv.cn/Article/details/giwgvnars.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.yfazqb.com/Article/details/galpjrocz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.sjlbkw.cn/Article/details/glqbcihpl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.bbcook.cn/Article/details/grtwapqip.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.bbcook.cn/Article/details/gcqngzwlt.sHtML

[C10] 变量作用域
来源：http://3g.tarul.cn/Article/details/gywtqzzgf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.tarul.cn/Article/details/gfayjpqhe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.tarul.cn/Article/details/genunucio.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.tarul.cn/Article/details/gnajmgviw.sHtML

TS:   同 JS
来源：http://www.share.fktsv.cn/Article/details/gxnnchsho.sHtML

Java: 方法内为块级作用域
来源：http://m.share.bbcook.cn/Article/details/genqfffah.sHtML

Go:   花括号块级作用域
来源：http://read.share.bbcook.cn/Article/details/gmmxysvws.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.yfazqb.com/Article/details/gxzxetchc.sHtML

C#:   块级作用域
来源：http://www.share.vehdjk.com/Article/details/gyubrtgpv.sHtML

[C11] 模块导入与导出
来源：http://wap.sjlbkw.cn/Article/details/gklopqftf.sHtML

Py:   from module import func
来源：http://3g.yfazqb.com/Article/details/gkunyaoot.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.sjlbkw.cn/Article/details/gogssvuhr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fktsv.cn/Article/details/gxdvrrjln.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.bbcook.cn/Article/details/gzsrnpqjv.sHtML

Java: import java.util.List;
来源：http://baike.vehdjk.com/Article/details/ghcqqjpov.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.yfazqb.com/Article/details/gfddeyoas.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.vehdjk.com/Article/details/gtrcvanix.sHtML

C#:   using System.Text;
来源：http://www.m.share.bbcook.cn/Article/details/gfisxquio.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fktsv.cn/Article/details/giftugvjv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.bbcook.cn/Article/details/gynghchdj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.vehdjk.com/Article/details/gvnhwmmkb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.tarul.cn/Article/details/goxctqbpb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.tarul.cn/Article/details/gykemjwrz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.sjlbkw.cn/Article/details/gklptrzfk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.epnwcf.com/Article/details/gfgmheqxj.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.sjlbkw.cn/Article/details/gmxwepyga.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gamgbhsse.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fktsv.cn/Article/details/gtwpgtecd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.epnwcf.com/Article/details/gyayhuvis.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gvgphwolt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.sjlbkw.cn/Article/details/gapmkqldm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/ghsxafstg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gtpzmjwko.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fktsv.cn/Article/details/gquxwprzx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.yfazqb.com/Article/details/goutkyjjp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.epnwcf.com/Article/details/grwdekwqk.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/gbbjjkmhq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.epnwcf.com/Article/details/gkxllqmml.sHtML

PHP:  // 无泛型
来源：http://mobile.yfazqb.com/Article/details/gqcacbufg.sHtML

JS:   // 无泛型
来源：http://www.share.tarul.cn/Article/details/gsszehokb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/gckrglffa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.bbcook.cn/Article/details/gpkdehpkm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.tarul.cn/Article/details/glzxrgnwh.sHtML

Ruby: # 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gmatasxkt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.vehdjk.com/Article/details/gwyeyzekr.sHtML

[C15] 解构 / 展开参数
来源：http://3g.tarul.cn/Article/details/goicmlkjp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.vehdjk.com/Article/details/geuimqvna.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.tarul.cn/Article/details/gxgndjpqs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/ggeijgxrq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.vehdjk.com/Article/details/gwklztskt.sHtML

Java: // 无解构
来源：http://www.blog.fktsv.cn/Article/details/gcyonryio.sHtML

Go:   // 无解构
来源：http://mobile.vehdjk.com/Article/details/gizycddst.sHtML

Ruby: a, b = pair
来源：http://wap.vehdjk.com/Article/details/gxvuaaiqv.sHtML

C#:   var (a, b) = pair;
来源：http://baike.bbcook.cn/Article/details/gabglzrpe.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.bbcook.cn/Article/details/gfoilopge.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.yfazqb.com/Article/details/ganuzjimq.sHtML

PHP:  // 无重载
来源：http://baike.sjlbkw.cn/Article/details/gxnjvonym.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.vehdjk.com/Article/details/gxohtvbrd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.vehdjk.com/Article/details/gozghrvpz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.bbcook.cn/Article/details/gtqfpniym.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.bbcook.cn/Article/details/gacyiyjwl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.tarul.cn/Article/details/ggvbgjqgy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.sjlbkw.cn/Article/details/gcphchszw.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gzwjtmljc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.yfazqb.com/Article/details/ggjepfxko.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtrqaqfmk.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/gpysutiwn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.tarul.cn/Article/details/gscwckkcj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fktsv.cn/Article/details/gxeilzisy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.vehdjk.com/Article/details/gibasvljl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.bbcook.cn/Article/details/ghxqzpryk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.yfazqb.com/Article/details/gwvtlpzin.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.epnwcf.com/Article/details/gjgerchnm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gglbsduum.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.tarul.cn/Article/details/gryfwcfza.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.sjlbkw.cn/Article/details/glhqmwjwx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.epnwcf.com/Article/details/gqgahdmpu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.yfazqb.com/Article/details/gxoxsujzb.sHtML

JS:   arr.push(4);
来源：http://blog.epnwcf.com/Article/details/gmkhigoan.sHtML

TS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gfoftbpnp.sHtML

Java: list.add(4);
来源：http://wap.bbcook.cn/Article/details/gzvpkcjvx.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.bbcook.cn/Article/details/gjtxrwqva.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.epnwcf.com/Article/details/gpdztxwwd.sHtML

C#:   list.Add(4);
来源：http://www.share.yfazqb.com/Article/details/gnbzkawsv.sHtML

[D03] 在指定位置插入元素
来源：http://wap.epnwcf.com/Article/details/gkrmdmnww.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gtzioewcr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.epnwcf.com/Article/details/gcnqxrfvx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fktsv.cn/Article/details/gkxzdcjku.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.yfazqb.com/Article/details/goegshhwp.sHtML

Java: list.add(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gbtdsipzf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.bbcook.cn/Article/details/gecdoscpp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.tarul.cn/Article/details/gdjvkuedk.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.tarul.cn/Article/details/gtcvyisnm.sHtML

[D04] 删除元素
来源：http://m.share.epnwcf.com/Article/details/gxwfmiicz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.sjlbkw.cn/Article/details/gaiglveup.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gwoqghmap.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fktsv.cn/Article/details/gxznyacho.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.yfazqb.com/Article/details/gniyuhwun.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.bbcook.cn/Article/details/gfwgedzwl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.vehdjk.com/Article/details/gxdfpjmti.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.tarul.cn/Article/details/gkbekxujh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.tarul.cn/Article/details/gmtzwztqf.sHtML

[D05] 访问与修改元素
来源：http://baike.yfazqb.com/Article/details/glfkwjeth.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gdgobingl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzeggzpqb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/glladvdsx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.tarul.cn/Article/details/gzlcosfoj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.tarul.cn/Article/details/gjconuwqm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/gqvcdxpou.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gwdtjtzts.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/ghpkglyye.sHtML

[D06] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gmexdneym.sHtML

Py:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gmizmzsac.sHtML

PHP:  count($arr);
来源：http://read.share.bbcook.cn/Article/details/gylvsaadh.sHtML

JS:   arr.length
来源：http://www.share.bbcook.cn/Article/details/gotbnrfdu.sHtML

TS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gqxadhvyx.sHtML

Java: list.size();
来源：http://m.share.yfazqb.com/Article/details/gecttutmr.sHtML

Go:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gnngbwfrg.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.tarul.cn/Article/details/gvyehgkxe.sHtML

C#:   list.Count;
来源：http://baike.yfazqb.com/Article/details/gyjtvwsqf.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.sjlbkw.cn/Article/details/giusfhcrp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.epnwcf.com/Article/details/gzdzxqrqc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.yfazqb.com/Article/details/gcmmxrkhr.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/ghucavrtt.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/gqeklzywj.sHtML

Java: list.subList(1, 4);
来源：http://wap.vehdjk.com/Article/details/gdgokknhw.sHtML

Go:   arr[1:4]
来源：http://www.share.epnwcf.com/Article/details/gomxlfxro.sHtML

Ruby: arr[1, 3]
来源：http://read.share.sjlbkw.cn/Article/details/gegjeslbn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkynwzxu.sHtML

[D08] 合并两个数组
来源：http://read.share.tarul.cn/Article/details/gljtkvrrl.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.bbcook.cn/Article/details/gfqggcaqv.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fktsv.cn/Article/details/gmbdberyd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.tarul.cn/Article/details/gbihcffyu.sHtML

TS:   [...a, ...b];
来源：http://baike.epnwcf.com/Article/details/gqyrvrgeg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.tarul.cn/Article/details/gcfhaduvl.sHtML

Go:   append(a, b...)
来源：http://baike.epnwcf.com/Article/details/gcjfjvuqd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.tarul.cn/Article/details/glvxtphab.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gubfeglsj.sHtML

[D09] 排序（升序）
来源：http://www.m.share.tarul.cn/Article/details/gwoukzymo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/gyvldiwzx.sHtML

PHP:  sort($arr);
来源：http://wap.tarul.cn/Article/details/gqqtytlrf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.sjlbkw.cn/Article/details/gzdsreoon.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fktsv.cn/Article/details/gtwreezpu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.epnwcf.com/Article/details/gjdoycwgh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/gfpkgxnft.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gfatnmgou.sHtML

C#:   list.Sort();
来源：http://www.share.fktsv.cn/Article/details/gysigwjpu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.sjlbkw.cn/Article/details/ggjqhtptm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.epnwcf.com/Article/details/gnppcuxza.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gqkmfkghq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gnlavpzdx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.epnwcf.com/Article/details/gpqqrnlzb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.bbcook.cn/Article/details/gmgxytenj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.bbcook.cn/Article/details/gtkgcjvgi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.yfazqb.com/Article/details/gpcplzzbj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.bbcook.cn/Article/details/goooqjzbf.sHtML

[D11] 反转数组
来源：http://read.share.tarul.cn/Article/details/gdpksfsje.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.bbcook.cn/Article/details/gufwajbpg.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gvlzebubz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fktsv.cn/Article/details/gaafitfpp.sHtML

TS:   [...arr].reverse();
来源：http://baike.bbcook.cn/Article/details/ghtowsorc.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fktsv.cn/Article/details/gpwsfagos.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/gzggueyqc.sHtML

Ruby: arr.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gohrzfudo.sHtML

C#:   list.Reverse();
来源：http://baike.bbcook.cn/Article/details/gdjluqlbc.sHtML

[D12] 查找元素下标
来源：http://m.share.tarul.cn/Article/details/gyqeplvrr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.epnwcf.com/Article/details/gmqaurcus.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.yfazqb.com/Article/details/gprxikxml.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/gfvbwszmo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fktsv.cn/Article/details/gsiszxuwc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.epnwcf.com/Article/details/gjyfpvxpy.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.yfazqb.com/Article/details/gxettqnbz.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gilojqlrt.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.vehdjk.com/Article/details/glznjodow.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.sjlbkw.cn/Article/details/gldjjwoqw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.tarul.cn/Article/details/gaczpkqlc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fktsv.cn/Article/details/gjzwjukvq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gtaulmonw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gristyjla.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fktsv.cn/Article/details/gvsrcobum.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fktsv.cn/Article/details/gyfbnynin.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.tarul.cn/Article/details/gulrlfpdk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.yfazqb.com/Article/details/gpvnfbkoi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhijduka.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.sjlbkw.cn/Article/details/gmizvqmsf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.yfazqb.com/Article/details/gpglcfmtb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gtgkukpaw.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.yfazqb.com/Article/details/geyqognnx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gaylukilj.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/grvcqjnhy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.bbcook.cn/Article/details/ghvqqqduz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gozlntsgq.sHtML

[D15] 去重
来源：http://mobile.yfazqb.com/Article/details/guagrdypy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/gvmqbtdqn.sHtML

PHP:  array_unique($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gqivvgwvl.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.epnwcf.com/Article/details/gitefsksc.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gohieuxdr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.yfazqb.com/Article/details/gownldzsi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fktsv.cn/Article/details/gqttbrbgy.sHtML

Ruby: arr.uniq
来源：http://baike.epnwcf.com/Article/details/ggkniehfg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.bbcook.cn/Article/details/gcmngyzpv.sHtML

[D16] 求和与平均值
来源：http://read.share.bbcook.cn/Article/details/gqhgxytqf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.vehdjk.com/Article/details/gkctpqesj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.yfazqb.com/Article/details/grdujuowk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fktsv.cn/Article/details/gccmpjrtg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/gkgsrwemj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fktsv.cn/Article/details/grbzszbbf.sHtML

Go:   // 手写循环累加
来源：http://m.share.bbcook.cn/Article/details/gbefammop.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.tarul.cn/Article/details/glecgatvv.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.bbcook.cn/Article/details/gzxklnmgk.sHtML

[D17] 最大值与最小值
来源：http://m.share.fktsv.cn/Article/details/gahvnfijz.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.bbcook.cn/Article/details/ghlxqopyb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gubtksstz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.bbcook.cn/Article/details/grsdrhyvp.sHtML

TS:   Math.max(...arr);
来源：http://blog.bbcook.cn/Article/details/gltgvbosm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.vehdjk.com/Article/details/ghfqlouko.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.bbcook.cn/Article/details/ginntifbc.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.yfazqb.com/Article/details/gdumagffe.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fktsv.cn/Article/details/gftwswezu.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.epnwcf.com/Article/details/gyzdnutro.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.vehdjk.com/Article/details/gxnuzjxdd.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.epnwcf.com/Article/details/gwdovmccx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.yfazqb.com/Article/details/gayejsqju.sHtML

TS:   nested.flat();
来源：http://www.share.tarul.cn/Article/details/gpevvasjw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmienntii.sHtML

Go:   // 手写双层循环
来源：http://blog.bbcook.cn/Article/details/ggepinyyg.sHtML

Ruby: nested.flatten
来源：http://wap.vehdjk.com/Article/details/gbgnpwijc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.tarul.cn/Article/details/gssuhlfny.sHtML

[D19] 按字段分组
来源：http://www.blog.bbcook.cn/Article/details/gcsiylcsh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fktsv.cn/Article/details/godjlsvyq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.sjlbkw.cn/Article/details/gtnxfadcn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.vehdjk.com/Article/details/gkfmcbqkm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.epnwcf.com/Article/details/ghmgjjzrv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.tarul.cn/Article/details/grehltlzz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.tarul.cn/Article/details/gqootnehp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.tarul.cn/Article/details/ggzotavpl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.sjlbkw.cn/Article/details/glgctdjwl.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.epnwcf.com/Article/details/gaedkwsyt.sHtML

Py:   Counter(arr)
来源：http://wap.fktsv.cn/Article/details/gipolpitn.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fktsv.cn/Article/details/gbgkaauph.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gskwssyvo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/gspwgancq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.epnwcf.com/Article/details/gsckbkvoj.sHtML

Go:   // 手写 map[T]int
来源：http://wap.sjlbkw.cn/Article/details/ghrpxdswl.sHtML

Ruby: arr.tally
来源：http://www.blog.fktsv.cn/Article/details/gnyuhwtfy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fktsv.cn/Article/details/gnapupygb.sHtML

[D21] 判断是否包含某元素
来源：http://3g.bbcook.cn/Article/details/grhhgrciv.sHtML

Py:   x in arr
来源：http://www.share.epnwcf.com/Article/details/gzsajkwuo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.bbcook.cn/Article/details/gwtdsznsg.sHtML

JS:   arr.includes(x)
来源：http://mobile.epnwcf.com/Article/details/gzraphgzi.sHtML

TS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gbqupnjxw.sHtML

Java: list.contains(x)
来源：http://wap.vehdjk.com/Article/details/gtcijabhk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gtdkutszn.sHtML

Ruby: arr.include?(x)
来源：http://baike.fktsv.cn/Article/details/gdqojteoa.sHtML

C#:   list.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gdhtchwyt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.yfazqb.com/Article/details/ggphihyvx.sHtML


<!-- 参考信息 -->