代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.epnwcf.com/Article/details/gktcoxqrc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/gyveivxrl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.tarul.cn/Article/details/gyzkgwtdd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fktsv.cn/Article/details/gczyndvsz.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.sjlbkw.cn/Article/details/gkxwrgkdq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/gdncngwsb.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/gtrlyhcxy.sHtML

[C05] 返回多个值
来源：http://wap.epnwcf.com/Article/details/gkymbgvdr.sHtML

Py:   return a, b
来源：http://read.share.yfazqb.com/Article/details/gutpdxwfx.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.epnwcf.com/Article/details/glahoxytr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/gqedlcryp.sHtML

TS:   return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gdxezhzgw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.tarul.cn/Article/details/ghdbvpiim.sHtML

Go:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gimdccste.sHtML

Ruby: return a, b
来源：http://wap.tarul.cn/Article/details/gchdcjtmv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.yfazqb.com/Article/details/gxsglccqw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.yfazqb.com/Article/details/gbswgaiku.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.vehdjk.com/Article/details/gygrhjtsq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.sjlbkw.cn/Article/details/gpjcequzr.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gsdnnkmyk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.epnwcf.com/Article/details/gxzzoegmd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.bbcook.cn/Article/details/grkbmpyvn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.sjlbkw.cn/Article/details/gkkbxjjht.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gtmxonkxd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fktsv.cn/Article/details/gbhmmsxcy.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fktsv.cn/Article/details/gpebjhnux.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.bbcook.cn/Article/details/grtpmvuae.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.tarul.cn/Article/details/gwdtodsqe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.sjlbkw.cn/Article/details/ggpqjlzes.sHtML

TS:   arr.map(String)
来源：http://read.share.bbcook.cn/Article/details/gqzpbkqfl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gbojtipwf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.vehdjk.com/Article/details/gdplfibdu.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.bbcook.cn/Article/details/gugkpchpf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.sjlbkw.cn/Article/details/gxgwlmuul.sHtML

[C08] 闭包
来源：http://read.share.bbcook.cn/Article/details/gdctwtrst.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.epnwcf.com/Article/details/gbtmiazoe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fktsv.cn/Article/details/gvepjggry.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gyipwbmhx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gckcbrsoz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.sjlbkw.cn/Article/details/gcvbwaunv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.yfazqb.com/Article/details/gmjgufjru.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.vehdjk.com/Article/details/ggrehpypn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gwajllwrg.sHtML

[C09] 递归
来源：http://wap.epnwcf.com/Article/details/gzjcbemto.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/ghrtfrgwh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fktsv.cn/Article/details/giaiiamfr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gakrpqejg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/gaxxequtf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.epnwcf.com/Article/details/goruedvvg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.bbcook.cn/Article/details/gfppazkzf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gbyxxxijq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.bbcook.cn/Article/details/gzkqrsxot.sHtML

[C10] 变量作用域
来源：http://baike.vehdjk.com/Article/details/gzzmnapwr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.epnwcf.com/Article/details/gbdgilikf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/gczzwxqla.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gndixvhpx.sHtML

TS:   同 JS
来源：http://wap.yfazqb.com/Article/details/gixgdueoa.sHtML

Java: 方法内为块级作用域
来源：http://blog.yfazqb.com/Article/details/gxqlvzmfe.sHtML

Go:   花括号块级作用域
来源：http://www.blog.yfazqb.com/Article/details/gjnmcesye.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.sjlbkw.cn/Article/details/gcyeonytp.sHtML

C#:   块级作用域
来源：http://blog.vehdjk.com/Article/details/gadlcmjeq.sHtML

[C11] 模块导入与导出
来源：http://www.blog.yfazqb.com/Article/details/gcxzugtya.sHtML

Py:   from module import func
来源：http://www.m.share.vehdjk.com/Article/details/gtzvtvgqe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.epnwcf.com/Article/details/gtqkqsgps.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.tarul.cn/Article/details/gvvhiqjoq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.bbcook.cn/Article/details/glkjesekj.sHtML

Java: import java.util.List;
来源：http://wap.yfazqb.com/Article/details/gkfwbddys.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.bbcook.cn/Article/details/gmrrhrwng.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.sjlbkw.cn/Article/details/gkhhuknsk.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/gfswymiqm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fktsv.cn/Article/details/grwumpnbd.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.sjlbkw.cn/Article/details/gmmrlpczr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.bbcook.cn/Article/details/gbxstlnwr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.yfazqb.com/Article/details/gxawrenxz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/gbhqupvqv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.epnwcf.com/Article/details/glqrbewxp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.yfazqb.com/Article/details/gnztfhrda.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.tarul.cn/Article/details/gpopwklhi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fktsv.cn/Article/details/gylmffwbn.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fktsv.cn/Article/details/gudcjnkgl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.epnwcf.com/Article/details/gafwgzpef.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gmwddongb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fktsv.cn/Article/details/gxldtmrgh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/ggawtdxif.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gielnrcfg.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fktsv.cn/Article/details/gedlehoav.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.sjlbkw.cn/Article/details/gwojxcfqd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.yfazqb.com/Article/details/gaypsijvu.sHtML

[C14] 泛型函数
来源：http://m.share.bbcook.cn/Article/details/gslbgtktu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.yfazqb.com/Article/details/gucfxpodc.sHtML

PHP:  // 无泛型
来源：http://wap.bbcook.cn/Article/details/gglwtnawm.sHtML

JS:   // 无泛型
来源：http://wap.epnwcf.com/Article/details/gpxdmjuio.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.yfazqb.com/Article/details/gimvxmoue.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.tarul.cn/Article/details/gijrctcrt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.tarul.cn/Article/details/gwnqicbnr.sHtML

Ruby: # 无泛型
来源：http://wap.epnwcf.com/Article/details/ghqdjobqk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.vehdjk.com/Article/details/gmbjjgnxa.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fktsv.cn/Article/details/gzyrcrbwq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.yfazqb.com/Article/details/ghznkjakm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.vehdjk.com/Article/details/gphoojuni.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/gbbkflcjy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.sjlbkw.cn/Article/details/gssedckji.sHtML

Java: // 无解构
来源：http://read.share.epnwcf.com/Article/details/gixmtruro.sHtML

Go:   // 无解构
来源：http://blog.epnwcf.com/Article/details/gwfxkbpck.sHtML

Ruby: a, b = pair
来源：http://3g.fktsv.cn/Article/details/ggaicgffy.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.bbcook.cn/Article/details/gwvecgxxq.sHtML

[C16] 函数 / 方法重载
来源：http://3g.epnwcf.com/Article/details/gnggxvdjt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.vehdjk.com/Article/details/gkasqqlle.sHtML

PHP:  // 无重载
来源：http://mobile.tarul.cn/Article/details/gwscnufha.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.sjlbkw.cn/Article/details/ggzjpkgbu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.epnwcf.com/Article/details/gdsoaiiqo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.epnwcf.com/Article/details/gonkfgmcn.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.tarul.cn/Article/details/gxcbhsfau.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.yfazqb.com/Article/details/gmaiccoha.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.bbcook.cn/Article/details/gmugmgnyx.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gbmievosb.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.vehdjk.com/Article/details/gnauopqxn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkgdcmcdj.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.vehdjk.com/Article/details/goifjajao.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.tarul.cn/Article/details/gkcnktkyv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.yfazqb.com/Article/details/gakxuhuao.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.bbcook.cn/Article/details/guccshzpx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fktsv.cn/Article/details/gpmooiyln.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fktsv.cn/Article/details/gekibdqsg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.bbcook.cn/Article/details/gjvbclabu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.yfazqb.com/Article/details/gbjwdwvfi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.yfazqb.com/Article/details/gwlnzewwe.sHtML

[D02] 追加元素到末尾
来源：http://wap.tarul.cn/Article/details/gpzgclqlb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.tarul.cn/Article/details/gsibnnbmj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gykqbxtqt.sHtML

JS:   arr.push(4);
来源：http://www.m.share.bbcook.cn/Article/details/gulwtyhae.sHtML

TS:   arr.push(4);
来源：http://read.share.tarul.cn/Article/details/gxnzogrnc.sHtML

Java: list.add(4);
来源：http://blog.sjlbkw.cn/Article/details/glepppgqg.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.tarul.cn/Article/details/gegunfslk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.sjlbkw.cn/Article/details/grmpqsfne.sHtML

C#:   list.Add(4);
来源：http://3g.epnwcf.com/Article/details/gsmwvrxwt.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.epnwcf.com/Article/details/gqbqgzpxm.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.epnwcf.com/Article/details/gmyqztubw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.epnwcf.com/Article/details/gmiajeluh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.sjlbkw.cn/Article/details/gezhfuwyr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gmksteeyy.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/giehgjrtg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.vehdjk.com/Article/details/gotjukvfz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.bbcook.cn/Article/details/gaxcdcxnu.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.vehdjk.com/Article/details/gghlqtyss.sHtML

[D04] 删除元素
来源：http://mobile.sjlbkw.cn/Article/details/guhoydaje.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.yfazqb.com/Article/details/gkmxnhoax.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.tarul.cn/Article/details/gbcjvhptz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.epnwcf.com/Article/details/gctqcuxru.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.vehdjk.com/Article/details/guqqdragb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fktsv.cn/Article/details/gsnuccluf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.tarul.cn/Article/details/gmnhdhkhb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.tarul.cn/Article/details/ggaghdfoj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.bbcook.cn/Article/details/ghpyykngw.sHtML

[D05] 访问与修改元素
来源：http://read.share.vehdjk.com/Article/details/guwwrpwuk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/grplunqhb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gdgmsbchr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gwskdszrs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.vehdjk.com/Article/details/gctrjzlwb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.vehdjk.com/Article/details/ggknzoldn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gmgncajzs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/ghnxvdjzp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.tarul.cn/Article/details/gsorhmseo.sHtML

[D06] 数组长度
来源：http://baike.fktsv.cn/Article/details/griojtloq.sHtML

Py:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gulzkfquq.sHtML

PHP:  count($arr);
来源：http://www.share.fktsv.cn/Article/details/gkxhmcttl.sHtML

JS:   arr.length
来源：http://www.m.share.yfazqb.com/Article/details/gwukoodpc.sHtML

TS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gjkhselia.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/gqkkjikbp.sHtML

Go:   len(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gelcqemco.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gdebovqnz.sHtML

C#:   list.Count;
来源：http://www.m.share.bbcook.cn/Article/details/gqlldhbfw.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.bbcook.cn/Article/details/giggsdybo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.tarul.cn/Article/details/gdexsrtmd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.bbcook.cn/Article/details/gkrnzdhjn.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gancgftvp.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gertrwrzv.sHtML

Java: list.subList(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/guwelkvrg.sHtML

Go:   arr[1:4]
来源：http://baike.fktsv.cn/Article/details/gydkdhrnm.sHtML

Ruby: arr[1, 3]
来源：http://wap.yfazqb.com/Article/details/goehcpkii.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gpppbyucp.sHtML

[D08] 合并两个数组
来源：http://mobile.fktsv.cn/Article/details/guzdejjik.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/grgsbdqnu.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fktsv.cn/Article/details/gypeeagch.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.sjlbkw.cn/Article/details/gfhmuvdyi.sHtML

TS:   [...a, ...b];
来源：http://read.share.epnwcf.com/Article/details/gdxcxkkvz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.epnwcf.com/Article/details/gamlvvjqp.sHtML

Go:   append(a, b...)
来源：http://mobile.vehdjk.com/Article/details/grvjeqdbk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fktsv.cn/Article/details/gzgjxtpqy.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.epnwcf.com/Article/details/gadehrwuo.sHtML

[D09] 排序（升序）
来源：http://wap.tarul.cn/Article/details/gqxmkomky.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/gdmfgjggf.sHtML

PHP:  sort($arr);
来源：http://blog.bbcook.cn/Article/details/guexrcxki.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.epnwcf.com/Article/details/gifdfjsxi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.epnwcf.com/Article/details/gtnlbzqyd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.bbcook.cn/Article/details/guimvovoe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gqwrgsibg.sHtML

Ruby: arr.sort
来源：http://m.share.yfazqb.com/Article/details/gaxjagffg.sHtML

C#:   list.Sort();
来源：http://read.share.vehdjk.com/Article/details/ghtceaszb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.tarul.cn/Article/details/gzhjrybtk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.vehdjk.com/Article/details/giwzwuxow.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gwkhzeand.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkpquvin.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.vehdjk.com/Article/details/gefuwlqts.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.tarul.cn/Article/details/glkylluuz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.tarul.cn/Article/details/gfsgqibwb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.bbcook.cn/Article/details/gragersao.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.bbcook.cn/Article/details/gsrpzkoqt.sHtML

[D11] 反转数组
来源：http://read.share.sjlbkw.cn/Article/details/ghsaksvim.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/gpwbzuqem.sHtML

PHP:  array_reverse($arr);
来源：http://3g.epnwcf.com/Article/details/gdeemxugw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.bbcook.cn/Article/details/gkzymzftj.sHtML

TS:   [...arr].reverse();
来源：http://mobile.bbcook.cn/Article/details/gegrmjyue.sHtML

Java: Collections.reverse(list);
来源：http://wap.yfazqb.com/Article/details/ggkwglbxg.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.epnwcf.com/Article/details/gszrpkqlf.sHtML

Ruby: arr.reverse
来源：http://3g.yfazqb.com/Article/details/gdidxpqlj.sHtML

C#:   list.Reverse();
来源：http://wap.vehdjk.com/Article/details/gacwyrldn.sHtML

[D12] 查找元素下标
来源：http://www.share.bbcook.cn/Article/details/gkpxvqetu.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.vehdjk.com/Article/details/gklnsqcrw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gxwizrkjb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.bbcook.cn/Article/details/gaykitfhc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/gnerbnrgw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.yfazqb.com/Article/details/gazyoyshs.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.yfazqb.com/Article/details/glzvadzbv.sHtML

Ruby: arr.index(x)
来源：http://baike.fktsv.cn/Article/details/gohzsefnp.sHtML

C#:   list.IndexOf(x);
来源：http://blog.yfazqb.com/Article/details/gquycnnug.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.sjlbkw.cn/Article/details/gdvwxbunm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.tarul.cn/Article/details/gmwtzpqdu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fktsv.cn/Article/details/grwayjhhy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/guhsuqjfq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gwwcousja.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.tarul.cn/Article/details/gtxfyrury.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.sjlbkw.cn/Article/details/gpuhuugfm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.sjlbkw.cn/Article/details/gtavaljdm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.yfazqb.com/Article/details/ghxovyrui.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.epnwcf.com/Article/details/ginujishi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.sjlbkw.cn/Article/details/ghuyrzbwg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.bbcook.cn/Article/details/gqwgprdhl.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fktsv.cn/Article/details/gpkfkujpy.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.tarul.cn/Article/details/gpfeqfmbp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.tarul.cn/Article/details/giizcwuyj.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/grjhyzjxk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gknmaldov.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.epnwcf.com/Article/details/gycabsvps.sHtML

[D15] 去重
来源：http://baike.tarul.cn/Article/details/gcarhcnkl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/gqwtvesmw.sHtML

PHP:  array_unique($arr);
来源：http://wap.fktsv.cn/Article/details/gefujiuey.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/gkurmnksm.sHtML

TS:   [...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gsfputfqm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.epnwcf.com/Article/details/gdvvwinfl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.sjlbkw.cn/Article/details/gnakehkis.sHtML

Ruby: arr.uniq
来源：http://baike.fktsv.cn/Article/details/gqfilocrw.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fktsv.cn/Article/details/gmdjgblkm.sHtML

[D16] 求和与平均值
来源：http://blog.vehdjk.com/Article/details/ggdermnmw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gvxtdnytg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gyqqeubvz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/gymcyutaw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/gbamibwjk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.bbcook.cn/Article/details/grdllymrm.sHtML

Go:   // 手写循环累加
来源：http://mobile.epnwcf.com/Article/details/giafuncjb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.vehdjk.com/Article/details/gmuvtmcha.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.yfazqb.com/Article/details/gbxdklqlc.sHtML

[D17] 最大值与最小值
来源：http://www.share.vehdjk.com/Article/details/gdlarowak.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.bbcook.cn/Article/details/gcrdyhswp.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/gcenwdghr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.yfazqb.com/Article/details/gkranpqfc.sHtML

TS:   Math.max(...arr);
来源：http://3g.tarul.cn/Article/details/gqrktgoer.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gcvbuowkg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fktsv.cn/Article/details/gqsylnzho.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.yfazqb.com/Article/details/gitzxvfug.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/gqkgtbgtc.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.bbcook.cn/Article/details/ghmrstcyl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.yfazqb.com/Article/details/grbafezlf.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.tarul.cn/Article/details/grvsmxdmd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fktsv.cn/Article/details/gmvwrptas.sHtML

TS:   nested.flat();
来源：http://baike.tarul.cn/Article/details/grmbemndc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.vehdjk.com/Article/details/gqcuejroe.sHtML

Go:   // 手写双层循环
来源：http://baike.sjlbkw.cn/Article/details/gsvbxjbjx.sHtML

Ruby: nested.flatten
来源：http://baike.tarul.cn/Article/details/gujolhupy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.vehdjk.com/Article/details/gwrcodmrv.sHtML

[D19] 按字段分组
来源：http://m.share.sjlbkw.cn/Article/details/gwzdtabhy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.tarul.cn/Article/details/gazwmyosl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.sjlbkw.cn/Article/details/gatrrkrtc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.epnwcf.com/Article/details/gyzmikvvs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/gvnegvldc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/gvyznizlz.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.bbcook.cn/Article/details/gkixvnfam.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.vehdjk.com/Article/details/gbfuxwyla.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.bbcook.cn/Article/details/guntegukc.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.epnwcf.com/Article/details/gbnmlcccr.sHtML

Py:   Counter(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gwhpaeepm.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.vehdjk.com/Article/details/gptueyzkk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/gasdlmcja.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gehmkuqro.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.epnwcf.com/Article/details/gtasmkave.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.vehdjk.com/Article/details/gunvkavdk.sHtML

Ruby: arr.tally
来源：http://blog.bbcook.cn/Article/details/gpkwhntho.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fktsv.cn/Article/details/gczrkgpde.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fktsv.cn/Article/details/gwvmndscu.sHtML

Py:   x in arr
来源：http://www.m.share.fktsv.cn/Article/details/gijxkekwb.sHtML


<!-- 参考信息 -->