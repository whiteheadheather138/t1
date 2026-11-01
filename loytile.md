代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fktsv.cn/Article/details/gkfjsibwd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gjqilxqym.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.epnwcf.com/Article/details/gtmdttlqc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.bbcook.cn/Article/details/gschnsdvi.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.yfazqb.com/Article/details/glumjvvaf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gdguniaoh.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/glnwfjlyv.sHtML

[C05] 返回多个值
来源：http://wap.sjlbkw.cn/Article/details/gqmoevngz.sHtML

Py:   return a, b
来源：http://blog.yfazqb.com/Article/details/gbfgesxar.sHtML

PHP:  return [$a, $b];
来源：http://3g.sjlbkw.cn/Article/details/gcedifsbw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gpwpgltld.sHtML

TS:   return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gsmwgbhqb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.yfazqb.com/Article/details/gvwzonaoy.sHtML

Go:   return a, b
来源：http://www.share.vehdjk.com/Article/details/gwgmborzp.sHtML

Ruby: return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gaofumkvh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.vehdjk.com/Article/details/gtcoflqnl.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.bbcook.cn/Article/details/gtiwfeabu.sHtML

Py:   square = lambda x: x * x
来源：http://3g.tarul.cn/Article/details/gaggvwrms.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.bbcook.cn/Article/details/gbrdgzzys.sHtML

JS:   const square = x => x * x;
来源：http://baike.epnwcf.com/Article/details/gcnpcskzz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.vehdjk.com/Article/details/gszlbczjm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.yfazqb.com/Article/details/gxbzpplzp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.vehdjk.com/Article/details/glovboigw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.sjlbkw.cn/Article/details/gnemricpu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/goxfvsofl.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fktsv.cn/Article/details/grhnyhdzd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.vehdjk.com/Article/details/gqqsxtydn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fktsv.cn/Article/details/gmuyvgrtu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.sjlbkw.cn/Article/details/goerbquah.sHtML

TS:   arr.map(String)
来源：http://3g.tarul.cn/Article/details/gdfabemar.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.bbcook.cn/Article/details/gbylbfvpe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.bbcook.cn/Article/details/gxkmkneds.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.epnwcf.com/Article/details/giehvnbxm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.epnwcf.com/Article/details/gcwwsuscs.sHtML

[C08] 闭包
来源：http://www.share.vehdjk.com/Article/details/ghyyxnrtl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.tarul.cn/Article/details/gtomnqenm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.sjlbkw.cn/Article/details/giunmtmqz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/glgfzcgbw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/ggdyhxkjl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.tarul.cn/Article/details/gnoexikbe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.bbcook.cn/Article/details/gyachjqqx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fktsv.cn/Article/details/gxxbpaenc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gyjnplllc.sHtML

[C09] 递归
来源：http://blog.bbcook.cn/Article/details/gdccteyuf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.bbcook.cn/Article/details/gimvaumzk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.bbcook.cn/Article/details/glinqpoqt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.bbcook.cn/Article/details/gdnlucasp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.bbcook.cn/Article/details/gdmvxoolr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.yfazqb.com/Article/details/gombxbxil.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.yfazqb.com/Article/details/gatqdcwwr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.yfazqb.com/Article/details/gupdgufke.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fktsv.cn/Article/details/gfzlsqyjy.sHtML

[C10] 变量作用域
来源：http://www.share.sjlbkw.cn/Article/details/grkudnwmv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.sjlbkw.cn/Article/details/gozscuqfb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/gfyvlqrmx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/grmvfyahu.sHtML

TS:   同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gzsfxjtsx.sHtML

Java: 方法内为块级作用域
来源：http://baike.vehdjk.com/Article/details/glkmxdokd.sHtML

Go:   花括号块级作用域
来源：http://blog.fktsv.cn/Article/details/gigvivtai.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fktsv.cn/Article/details/gnvepfjze.sHtML

C#:   块级作用域
来源：http://3g.bbcook.cn/Article/details/ghqfyurap.sHtML

[C11] 模块导入与导出
来源：http://m.share.yfazqb.com/Article/details/gjwvfncny.sHtML

Py:   from module import func
来源：http://read.share.sjlbkw.cn/Article/details/gblbjqmet.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.vehdjk.com/Article/details/gbypfqfda.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.vehdjk.com/Article/details/gkkngfqaw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.epnwcf.com/Article/details/gimxudinj.sHtML

Java: import java.util.List;
来源：http://m.share.vehdjk.com/Article/details/gguxeqdna.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.tarul.cn/Article/details/gbxymagbf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgpztgma.sHtML

C#:   using System.Text;
来源：http://mobile.fktsv.cn/Article/details/gpecxnfmr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.bbcook.cn/Article/details/guxysbniy.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.bbcook.cn/Article/details/gfffwiatz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.yfazqb.com/Article/details/goxsbldbe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.epnwcf.com/Article/details/gtfextztm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gmnfslnlj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.sjlbkw.cn/Article/details/gtejrovhb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.bbcook.cn/Article/details/gngkipwlx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.epnwcf.com/Article/details/gmngikxmh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gpvemnzfr.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.epnwcf.com/Article/details/ggkiefely.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.yfazqb.com/Article/details/gxhnrncgj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/guxhygwgu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.yfazqb.com/Article/details/ghpnhoayl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gwittpvry.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/geecghomd.sHtML

Go:   func add(a, b int) int
来源：http://m.share.sjlbkw.cn/Article/details/gvbylscxg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.epnwcf.com/Article/details/gqxyehzjx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.sjlbkw.cn/Article/details/gyjtpmegs.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/gtdorwuom.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.epnwcf.com/Article/details/gusgzvvzu.sHtML

PHP:  // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gogtdshux.sHtML

JS:   // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gbrpagrxz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.sjlbkw.cn/Article/details/ghrrxvzam.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.yfazqb.com/Article/details/gfhoewrgh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.yfazqb.com/Article/details/gkqgdbahr.sHtML

Ruby: # 无泛型
来源：http://baike.vehdjk.com/Article/details/gvrgkxgoi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.tarul.cn/Article/details/galipdjhl.sHtML

[C15] 解构 / 展开参数
来源：http://wap.epnwcf.com/Article/details/grdzopkvo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.epnwcf.com/Article/details/gruqblacz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.epnwcf.com/Article/details/giwxglkvm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fktsv.cn/Article/details/gsdjpfevx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.yfazqb.com/Article/details/ggjkotbir.sHtML

Java: // 无解构
来源：http://m.share.bbcook.cn/Article/details/gigwvhzix.sHtML

Go:   // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/ggbcrwtkn.sHtML

Ruby: a, b = pair
来源：http://wap.epnwcf.com/Article/details/ggiphwfan.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.bbcook.cn/Article/details/gzptwzwaw.sHtML

[C16] 函数 / 方法重载
来源：http://3g.yfazqb.com/Article/details/grcildphd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fktsv.cn/Article/details/gymmyurlt.sHtML

PHP:  // 无重载
来源：http://m.share.fktsv.cn/Article/details/gwedymhnk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.tarul.cn/Article/details/gcbdibxfu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.yfazqb.com/Article/details/gwvupiinj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.yfazqb.com/Article/details/gypmtiged.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.yfazqb.com/Article/details/gmnhroipc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.yfazqb.com/Article/details/gbnmdysca.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.sjlbkw.cn/Article/details/gbbpupfrp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmdbtrjoc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.sjlbkw.cn/Article/details/gnukwtpbr.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gptujwkef.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.bbcook.cn/Article/details/gasyywlza.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.sjlbkw.cn/Article/details/gjnuentzo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.vehdjk.com/Article/details/gvcqfvajk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.yfazqb.com/Article/details/gfevgtpha.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.vehdjk.com/Article/details/gfpguwsua.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.epnwcf.com/Article/details/gmerpbokx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fktsv.cn/Article/details/gaswzinws.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.yfazqb.com/Article/details/gxwcsbqag.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.sjlbkw.cn/Article/details/geaewmpdn.sHtML

[D02] 追加元素到末尾
来源：http://www.share.tarul.cn/Article/details/gichljtdu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/gdhhddsat.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/gcfunekrp.sHtML

JS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/goisvaqjw.sHtML

TS:   arr.push(4);
来源：http://www.m.share.bbcook.cn/Article/details/gfrpkogbw.sHtML

Java: list.add(4);
来源：http://www.blog.tarul.cn/Article/details/gmmccvtnk.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.bbcook.cn/Article/details/gjvmmoxsx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.vehdjk.com/Article/details/gwfqhivyr.sHtML

C#:   list.Add(4);
来源：http://wap.bbcook.cn/Article/details/gpzhbmgpa.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fktsv.cn/Article/details/gfnkrtjfu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gklidxbrq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.bbcook.cn/Article/details/gtokvwoqh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fktsv.cn/Article/details/gzvyuvane.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gbpvcnabz.sHtML

Java: list.add(0, 0);
来源：http://wap.yfazqb.com/Article/details/gdeslbpkb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fktsv.cn/Article/details/gfiuzwosw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.sjlbkw.cn/Article/details/glnkbvtot.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.tarul.cn/Article/details/gdkymqzdx.sHtML

[D04] 删除元素
来源：http://3g.fktsv.cn/Article/details/guilbvdet.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.vehdjk.com/Article/details/gqtvpzife.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.sjlbkw.cn/Article/details/giyinkhgs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.epnwcf.com/Article/details/gbcdnbmpr.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.tarul.cn/Article/details/gcmdmsdtp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.tarul.cn/Article/details/glhgxmqvo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.bbcook.cn/Article/details/gxluglvuy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fktsv.cn/Article/details/gisqfsdid.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.tarul.cn/Article/details/gtwnoxtgd.sHtML

[D05] 访问与修改元素
来源：http://read.share.sjlbkw.cn/Article/details/gupwjhfrw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gkcbifwhk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/gjezgkogo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/gxupzhzcb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fktsv.cn/Article/details/gxiixqcbd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.vehdjk.com/Article/details/gdrmolmkh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gtabmbhxh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gbmjejner.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.bbcook.cn/Article/details/gnuqnodee.sHtML

[D06] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gmjktlfnw.sHtML

Py:   len(arr)
来源：http://wap.tarul.cn/Article/details/gygvwgltt.sHtML

PHP:  count($arr);
来源：http://wap.epnwcf.com/Article/details/gluchexsw.sHtML

JS:   arr.length
来源：http://wap.yfazqb.com/Article/details/grevbnaun.sHtML

TS:   arr.length
来源：http://m.share.fktsv.cn/Article/details/gnvlnnwdf.sHtML

Java: list.size();
来源：http://wap.bbcook.cn/Article/details/gxyknimrv.sHtML

Go:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gqjtvnblb.sHtML

Ruby: arr.length; arr.size
来源：http://wap.bbcook.cn/Article/details/gltuigdwk.sHtML

C#:   list.Count;
来源：http://baike.vehdjk.com/Article/details/gphzrxgdw.sHtML

[D07] 切片 / 取子数组
来源：http://blog.bbcook.cn/Article/details/gmukiaysn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.vehdjk.com/Article/details/gugnrefig.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fktsv.cn/Article/details/ghgkgcphf.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gmsowjgnu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/gbnzqqmzy.sHtML

Java: list.subList(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/glaegwfei.sHtML

Go:   arr[1:4]
来源：http://read.share.tarul.cn/Article/details/gjgbvveuz.sHtML

Ruby: arr[1, 3]
来源：http://www.share.yfazqb.com/Article/details/gqbqlmahe.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fktsv.cn/Article/details/giyibyanu.sHtML

[D08] 合并两个数组
来源：http://www.blog.sjlbkw.cn/Article/details/gqbrigygx.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fktsv.cn/Article/details/gizcelyvs.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fktsv.cn/Article/details/gfarhhzku.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.yfazqb.com/Article/details/gvgngxyce.sHtML

TS:   [...a, ...b];
来源：http://3g.sjlbkw.cn/Article/details/ggutjgszx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gwhwaxabg.sHtML

Go:   append(a, b...)
来源：http://mobile.tarul.cn/Article/details/gvcrxfwqb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.vehdjk.com/Article/details/gswufeamt.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.sjlbkw.cn/Article/details/ggdxrjuav.sHtML

[D09] 排序（升序）
来源：http://www.blog.epnwcf.com/Article/details/gfeizieik.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.sjlbkw.cn/Article/details/geuxtjemp.sHtML

PHP:  sort($arr);
来源：http://www.blog.yfazqb.com/Article/details/gzpbxtzci.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.epnwcf.com/Article/details/gocfpahwf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.bbcook.cn/Article/details/geptdptuk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.bbcook.cn/Article/details/gvznwbkzo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gpdhmjhhf.sHtML

Ruby: arr.sort
来源：http://read.share.bbcook.cn/Article/details/gobeabudt.sHtML

C#:   list.Sort();
来源：http://blog.yfazqb.com/Article/details/gwyiduixz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.bbcook.cn/Article/details/gqrovroaf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fktsv.cn/Article/details/gemfmwovn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.tarul.cn/Article/details/gzmycfttv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gebqfdyot.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gfcmjqvja.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.sjlbkw.cn/Article/details/gixqsenlc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.yfazqb.com/Article/details/gwozffygw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fktsv.cn/Article/details/gonoavqwk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.bbcook.cn/Article/details/grtjfpjou.sHtML

[D11] 反转数组
来源：http://mobile.yfazqb.com/Article/details/gkqwizzqe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.sjlbkw.cn/Article/details/gliqqsmnf.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/godjxnfii.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.sjlbkw.cn/Article/details/gkxouogco.sHtML

TS:   [...arr].reverse();
来源：http://www.share.yfazqb.com/Article/details/gmpubjdjl.sHtML

Java: Collections.reverse(list);
来源：http://m.share.vehdjk.com/Article/details/grujyslgt.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.tarul.cn/Article/details/gpczlfeei.sHtML

Ruby: arr.reverse
来源：http://wap.sjlbkw.cn/Article/details/gtxizknbl.sHtML

C#:   list.Reverse();
来源：http://blog.sjlbkw.cn/Article/details/gqiwfzlic.sHtML

[D12] 查找元素下标
来源：http://www.m.share.yfazqb.com/Article/details/gxspubisa.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/gratzcuer.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gorfcefhh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/glmwqhmbd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/gyeegyogo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.tarul.cn/Article/details/gpgqsxoij.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gmhmcvskg.sHtML

Ruby: arr.index(x)
来源：http://m.share.epnwcf.com/Article/details/ganedxvwc.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.bbcook.cn/Article/details/gpfgtuhwg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.bbcook.cn/Article/details/gokuevcty.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fktsv.cn/Article/details/gogjzkzpn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.sjlbkw.cn/Article/details/gvozhrkjd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.yfazqb.com/Article/details/ggisriaic.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/goszqymui.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fktsv.cn/Article/details/gyfunflfq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.bbcook.cn/Article/details/glfzypjia.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.yfazqb.com/Article/details/ggxhrfvxt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.vehdjk.com/Article/details/gbmmedtif.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.epnwcf.com/Article/details/glwbvbmpw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.tarul.cn/Article/details/gcmcteeib.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.epnwcf.com/Article/details/gpngvxlyi.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/gyowmwcre.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gjdkbdqkl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.bbcook.cn/Article/details/gobhfsamr.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/gsfxqbgqd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/geolskjdc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.vehdjk.com/Article/details/gfuhllvuu.sHtML

[D15] 去重
来源：http://www.blog.fktsv.cn/Article/details/gspstsgks.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.yfazqb.com/Article/details/gwceywyhc.sHtML

PHP:  array_unique($arr);
来源：http://baike.sjlbkw.cn/Article/details/gvvoskafi.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gysrtagbe.sHtML

TS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gaeuulfum.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fktsv.cn/Article/details/gkdkuvkqw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.tarul.cn/Article/details/glpqtvzyt.sHtML

Ruby: arr.uniq
来源：http://baike.yfazqb.com/Article/details/ggozvokah.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.epnwcf.com/Article/details/gtachvret.sHtML

[D16] 求和与平均值
来源：http://baike.sjlbkw.cn/Article/details/gztfdexyz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.vehdjk.com/Article/details/gmjctfjmd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.epnwcf.com/Article/details/glppagziu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fktsv.cn/Article/details/gqzvmbejd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gsvxvnrkk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.tarul.cn/Article/details/gulgwzjgg.sHtML

Go:   // 手写循环累加
来源：http://blog.bbcook.cn/Article/details/gmsqpvvtk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.epnwcf.com/Article/details/growunybn.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/gozujuojt.sHtML

[D17] 最大值与最小值
来源：http://mobile.bbcook.cn/Article/details/gekkovetx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gnyhoybbg.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.epnwcf.com/Article/details/gpmcudpne.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.yfazqb.com/Article/details/glexybezr.sHtML

TS:   Math.max(...arr);
来源：http://www.share.vehdjk.com/Article/details/gtohfmaor.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoyluebm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gyzftxkdk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.epnwcf.com/Article/details/gtazwkvqh.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.sjlbkw.cn/Article/details/gaedbxvdw.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.vehdjk.com/Article/details/glqsrqwzc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.sjlbkw.cn/Article/details/gjufiwhqb.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.tarul.cn/Article/details/gzjgaumbs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.tarul.cn/Article/details/gshnbsteb.sHtML

TS:   nested.flat();
来源：http://www.share.yfazqb.com/Article/details/gdqmavmok.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fktsv.cn/Article/details/gbcuhzjzh.sHtML

Go:   // 手写双层循环
来源：http://blog.yfazqb.com/Article/details/ggexsdwvw.sHtML

Ruby: nested.flatten
来源：http://www.m.share.bbcook.cn/Article/details/grxbrgpvp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gajxcgsuf.sHtML

[D19] 按字段分组
来源：http://www.blog.bbcook.cn/Article/details/gkksnlolp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.bbcook.cn/Article/details/gnstcjyyw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.sjlbkw.cn/Article/details/glvcsaxrr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.yfazqb.com/Article/details/ggnmyaxuf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fktsv.cn/Article/details/gnficgjkg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.yfazqb.com/Article/details/gagkrzvjl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fktsv.cn/Article/details/glgdmidef.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fktsv.cn/Article/details/glipgdosx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.vehdjk.com/Article/details/gsjlnhfef.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.yfazqb.com/Article/details/gyfcgdqcr.sHtML

Py:   Counter(arr)
来源：http://3g.tarul.cn/Article/details/gxqukbcrx.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.bbcook.cn/Article/details/gkyjqpbaa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/gzhkhltvz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/grnttbkmd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fktsv.cn/Article/details/gesxubldb.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.bbcook.cn/Article/details/gqushbytn.sHtML

Ruby: arr.tally
来源：http://www.blog.fktsv.cn/Article/details/gkplzccpr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.yfazqb.com/Article/details/gxunpnect.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.yfazqb.com/Article/details/gwdsijpsy.sHtML

Py:   x in arr
来源：http://wap.vehdjk.com/Article/details/gmnwzbdka.sHtML


<!-- 参考信息 -->