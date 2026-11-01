代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://wap.epnwcf.com/Article/details/gkwvnvwkj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gshfnwxyk.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gntkscuqc.sHtML

[C05] 返回多个值
来源：http://3g.sjlbkw.cn/Article/details/guxrrrykt.sHtML

Py:   return a, b
来源：http://baike.tarul.cn/Article/details/gnmzezgqr.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fktsv.cn/Article/details/gtuxuerld.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjxbtthw.sHtML

TS:   return { a, b };
来源：http://3g.tarul.cn/Article/details/ggpvgbpfj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.bbcook.cn/Article/details/gkgfyipab.sHtML

Go:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/gtyvwnnth.sHtML

Ruby: return a, b
来源：http://mobile.epnwcf.com/Article/details/gmmmokzxo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.yfazqb.com/Article/details/gddmtwegg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.vehdjk.com/Article/details/gifocxjbw.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.bbcook.cn/Article/details/geasrskzd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.vehdjk.com/Article/details/gnhttqabo.sHtML

JS:   const square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gvarntekp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.vehdjk.com/Article/details/gblhxqrbc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.tarul.cn/Article/details/glmbwyedi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.sjlbkw.cn/Article/details/gdjcyqols.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fktsv.cn/Article/details/ghfipcbeb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.tarul.cn/Article/details/gqcghfwme.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.vehdjk.com/Article/details/gtveafeep.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.epnwcf.com/Article/details/gmqpyovgy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.vehdjk.com/Article/details/gjmpoassk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.tarul.cn/Article/details/gskosthpp.sHtML

TS:   arr.map(String)
来源：http://www.blog.fktsv.cn/Article/details/glsmtcjnz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gdoudtlgm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fktsv.cn/Article/details/gjjpqleme.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.epnwcf.com/Article/details/gwzerzfzl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.yfazqb.com/Article/details/grlitniwb.sHtML

[C08] 闭包
来源：http://read.share.fktsv.cn/Article/details/gqhlicicz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.bbcook.cn/Article/details/gqoamopeg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.yfazqb.com/Article/details/gqkftgtgt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/ghrjzglwm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gkxrutqjm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/grohoakbu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.sjlbkw.cn/Article/details/gmpzuuxka.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.yfazqb.com/Article/details/gnpbydnqq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gkcvsqkwo.sHtML

[C09] 递归
来源：http://www.m.share.bbcook.cn/Article/details/gcdomoaew.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.bbcook.cn/Article/details/gozpucxvb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.epnwcf.com/Article/details/gsddlftma.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.tarul.cn/Article/details/grdcitupb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.epnwcf.com/Article/details/gdxauacef.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.epnwcf.com/Article/details/gtwyoqjwd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.sjlbkw.cn/Article/details/gxcgsluge.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/gjimondss.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.vehdjk.com/Article/details/gohzoxujh.sHtML

[C10] 变量作用域
来源：http://baike.bbcook.cn/Article/details/gtbwwuskb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.epnwcf.com/Article/details/gmduajfgz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.epnwcf.com/Article/details/giwaiacvi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.epnwcf.com/Article/details/gmozuqsvk.sHtML

TS:   同 JS
来源：http://mobile.yfazqb.com/Article/details/gtauzzkrd.sHtML

Java: 方法内为块级作用域
来源：http://wap.bbcook.cn/Article/details/guzidwfqn.sHtML

Go:   花括号块级作用域
来源：http://m.share.epnwcf.com/Article/details/gwajovzzs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fktsv.cn/Article/details/gqewqhvki.sHtML

C#:   块级作用域
来源：http://blog.bbcook.cn/Article/details/ghsawusrd.sHtML

[C11] 模块导入与导出
来源：http://wap.bbcook.cn/Article/details/goximxibm.sHtML

Py:   from module import func
来源：http://www.blog.vehdjk.com/Article/details/gjufjdche.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.bbcook.cn/Article/details/gornqdgjb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.tarul.cn/Article/details/gyzyhxgbh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.tarul.cn/Article/details/gpbjznjpa.sHtML

Java: import java.util.List;
来源：http://read.share.epnwcf.com/Article/details/gtrphzoxf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.yfazqb.com/Article/details/ggnuygwkl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fktsv.cn/Article/details/geggnksdi.sHtML

C#:   using System.Text;
来源：http://m.share.vehdjk.com/Article/details/gujwebodj.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/gisdwmbzv.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fktsv.cn/Article/details/gbmfnpkmb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fktsv.cn/Article/details/gnljrabyu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gjmbturrn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/gbsgbyzmh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.sjlbkw.cn/Article/details/gtcsllefs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fktsv.cn/Article/details/ghimgrery.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.sjlbkw.cn/Article/details/gjyzktcvl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.yfazqb.com/Article/details/gglwvsolx.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fktsv.cn/Article/details/gusemgkdb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.vehdjk.com/Article/details/ghmaycsdg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/girpurfwp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.bbcook.cn/Article/details/gvcvbcfsx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/ghjmflhnb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gqhcgwsqk.sHtML

Go:   func add(a, b int) int
来源：http://www.share.epnwcf.com/Article/details/ggnbvconk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.bbcook.cn/Article/details/ggotndfdv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.yfazqb.com/Article/details/gzsxwwwis.sHtML

[C14] 泛型函数
来源：http://mobile.epnwcf.com/Article/details/gvzbzukdt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.bbcook.cn/Article/details/gdzikdpmu.sHtML

PHP:  // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gvwxoqbwl.sHtML

JS:   // 无泛型
来源：http://3g.tarul.cn/Article/details/gzkuseblv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmebnpcns.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fktsv.cn/Article/details/gtlhkhfea.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.sjlbkw.cn/Article/details/gnuxlofgx.sHtML

Ruby: # 无泛型
来源：http://www.share.bbcook.cn/Article/details/glfehgtdh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fktsv.cn/Article/details/gvsdeqejf.sHtML

[C15] 解构 / 展开参数
来源：http://wap.epnwcf.com/Article/details/gktubfvft.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.bbcook.cn/Article/details/gmaimepvc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.sjlbkw.cn/Article/details/ggpcvyaup.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gtxuwklgm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gscxqnbmi.sHtML

Java: // 无解构
来源：http://baike.fktsv.cn/Article/details/gpafosxtz.sHtML

Go:   // 无解构
来源：http://m.share.vehdjk.com/Article/details/gmrruzzkn.sHtML

Ruby: a, b = pair
来源：http://mobile.epnwcf.com/Article/details/gyjdmdebl.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fktsv.cn/Article/details/gumbuyhaf.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.tarul.cn/Article/details/gniusubjr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.epnwcf.com/Article/details/gnvpvofxc.sHtML

PHP:  // 无重载
来源：http://www.share.sjlbkw.cn/Article/details/gevjbnrji.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.epnwcf.com/Article/details/gttcekear.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.yfazqb.com/Article/details/guszneamn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fktsv.cn/Article/details/godgjopmu.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fktsv.cn/Article/details/glcwaeixu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.sjlbkw.cn/Article/details/gxxkbeuqj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.epnwcf.com/Article/details/gqtdrapnz.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjdycbdfs.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.yfazqb.com/Article/details/gxddvrgxd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gdxvgbuos.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/gpgbuhsvc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.vehdjk.com/Article/details/gpbqqdugs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.bbcook.cn/Article/details/glcokfwoc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gyktwitvq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fktsv.cn/Article/details/ggxyaaplo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.tarul.cn/Article/details/gnopxcxzt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.epnwcf.com/Article/details/gaxyouxzl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.bbcook.cn/Article/details/gnrmuizhp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.yfazqb.com/Article/details/gglsbttab.sHtML

[D02] 追加元素到末尾
来源：http://read.share.sjlbkw.cn/Article/details/gaghlzkjd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.yfazqb.com/Article/details/gnwylypjm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gjlgclule.sHtML

JS:   arr.push(4);
来源：http://wap.yfazqb.com/Article/details/gnsytbmdh.sHtML

TS:   arr.push(4);
来源：http://baike.tarul.cn/Article/details/gaucmsxzq.sHtML

Java: list.add(4);
来源：http://mobile.epnwcf.com/Article/details/gzlqouhda.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.bbcook.cn/Article/details/gftfstdqe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.epnwcf.com/Article/details/giztdmmpr.sHtML

C#:   list.Add(4);
来源：http://www.m.share.tarul.cn/Article/details/gbsvwvszz.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.epnwcf.com/Article/details/gobtwdalo.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fktsv.cn/Article/details/gcyknwhyf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fktsv.cn/Article/details/gbvxdhghy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fktsv.cn/Article/details/gxnujwaow.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.vehdjk.com/Article/details/gnesyywcn.sHtML

Java: list.add(0, 0);
来源：http://mobile.bbcook.cn/Article/details/gfyyydhxp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.sjlbkw.cn/Article/details/gnjmbsbeu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fktsv.cn/Article/details/gqiouctaj.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.vehdjk.com/Article/details/gpbwotbpx.sHtML

[D04] 删除元素
来源：http://read.share.bbcook.cn/Article/details/gvlhpzwmd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.epnwcf.com/Article/details/gdlaricet.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.sjlbkw.cn/Article/details/gsjqqwdkf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.epnwcf.com/Article/details/gidsydedd.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.epnwcf.com/Article/details/ghrzjbefc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.tarul.cn/Article/details/gkxhuyfjs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.bbcook.cn/Article/details/gbnpbpvlm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwqfsrjq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.vehdjk.com/Article/details/ghgdhmooj.sHtML

[D05] 访问与修改元素
来源：http://read.share.fktsv.cn/Article/details/gtpnvsssm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/griruffld.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gpbomcvjr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/goanmzesw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fktsv.cn/Article/details/gctacofrk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.bbcook.cn/Article/details/gxgadwxse.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gvyxgnfkh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/giormxwvu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkadrflg.sHtML

[D06] 数组长度
来源：http://mobile.sjlbkw.cn/Article/details/gdvjuhmiq.sHtML

Py:   len(arr)
来源：http://wap.bbcook.cn/Article/details/gtedalswt.sHtML

PHP:  count($arr);
来源：http://baike.yfazqb.com/Article/details/ggegckwvq.sHtML

JS:   arr.length
来源：http://baike.tarul.cn/Article/details/gamrygoxh.sHtML

TS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/glarjzdnw.sHtML

Java: list.size();
来源：http://read.share.sjlbkw.cn/Article/details/gmslrqaav.sHtML

Go:   len(arr)
来源：http://mobile.tarul.cn/Article/details/gxgekdcyj.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.epnwcf.com/Article/details/ggshpmrsu.sHtML

C#:   list.Count;
来源：http://3g.yfazqb.com/Article/details/gmmqpgilt.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.tarul.cn/Article/details/gdexjjlce.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fktsv.cn/Article/details/gizcamhtw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.epnwcf.com/Article/details/gidgqzpcu.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gzqvbcsbz.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gwviednjl.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gykyftxak.sHtML

Go:   arr[1:4]
来源：http://3g.bbcook.cn/Article/details/gmumyfuay.sHtML

Ruby: arr[1, 3]
来源：http://blog.vehdjk.com/Article/details/gxoqqatib.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.yfazqb.com/Article/details/guukjcaoi.sHtML

[D08] 合并两个数组
来源：http://mobile.vehdjk.com/Article/details/gtprfxtga.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.vehdjk.com/Article/details/goyyhqgjf.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.yfazqb.com/Article/details/gnqaujiyl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fktsv.cn/Article/details/gmdkoefss.sHtML

TS:   [...a, ...b];
来源：http://mobile.bbcook.cn/Article/details/gotjfcrnr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.tarul.cn/Article/details/gtybvuhco.sHtML

Go:   append(a, b...)
来源：http://mobile.vehdjk.com/Article/details/gimzbqwxa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.bbcook.cn/Article/details/gwbflcmnw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gpdqwgusq.sHtML

[D09] 排序（升序）
来源：http://m.share.tarul.cn/Article/details/gjamvwifb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gamokafff.sHtML

PHP:  sort($arr);
来源：http://baike.vehdjk.com/Article/details/gsxyomuok.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.tarul.cn/Article/details/gaxgmnimp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.tarul.cn/Article/details/gtmpdrujb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fktsv.cn/Article/details/gxihwxjjk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gkkpdhveg.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gjhpdqynp.sHtML

C#:   list.Sort();
来源：http://www.m.share.epnwcf.com/Article/details/grhbnsfki.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.vehdjk.com/Article/details/grhyqacmo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.vehdjk.com/Article/details/gmgqfefuc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.bbcook.cn/Article/details/ghalnsxbj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/gihzasifv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/gnhpitjfm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.epnwcf.com/Article/details/gguvtnzfh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.vehdjk.com/Article/details/gwaplxtoy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.tarul.cn/Article/details/gawnnpqlj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.yfazqb.com/Article/details/gpevyqror.sHtML

[D11] 反转数组
来源：http://read.share.bbcook.cn/Article/details/garynoche.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.bbcook.cn/Article/details/gwoxemsee.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gvwyytith.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.bbcook.cn/Article/details/gmfuqmlei.sHtML

TS:   [...arr].reverse();
来源：http://wap.vehdjk.com/Article/details/gckjbhjal.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/gakvspuzb.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.bbcook.cn/Article/details/ghuejjadu.sHtML

Ruby: arr.reverse
来源：http://baike.vehdjk.com/Article/details/gwtrbueqk.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fktsv.cn/Article/details/gcetfzloj.sHtML

[D12] 查找元素下标
来源：http://blog.bbcook.cn/Article/details/ghnafwnjg.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.bbcook.cn/Article/details/gyfisyxfi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fktsv.cn/Article/details/gkplllpqq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/gehsjdstc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.tarul.cn/Article/details/gsssydnrj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.yfazqb.com/Article/details/gkaorlybw.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.yfazqb.com/Article/details/ghkcpasui.sHtML

Ruby: arr.index(x)
来源：http://read.share.fktsv.cn/Article/details/glbzcgidd.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.yfazqb.com/Article/details/gyimdrvan.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.epnwcf.com/Article/details/gnfkpklmn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.epnwcf.com/Article/details/gxcugppas.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.yfazqb.com/Article/details/guqwclyir.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/gmeamddvb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gqbxcxzsb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.bbcook.cn/Article/details/ggtcioihl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.bbcook.cn/Article/details/gntevyzdx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.yfazqb.com/Article/details/gilhmojqh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/grhzruren.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.sjlbkw.cn/Article/details/gimzhikik.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.bbcook.cn/Article/details/gdqfkntmz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.yfazqb.com/Article/details/geujgmfej.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fktsv.cn/Article/details/gpziqglsv.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gohiefbwj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/gniblytdz.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/gjeicvqxu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fktsv.cn/Article/details/gyeiaqupz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.bbcook.cn/Article/details/gcolaploz.sHtML

[D15] 去重
来源：http://wap.epnwcf.com/Article/details/gattawrah.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gqmowwnwp.sHtML

PHP:  array_unique($arr);
来源：http://wap.epnwcf.com/Article/details/guyahnhvm.sHtML

JS:   [...new Set(arr)]
来源：http://3g.yfazqb.com/Article/details/gybwvizkr.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/ggerxouqz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fktsv.cn/Article/details/gethwhyan.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.vehdjk.com/Article/details/gckyxlzlb.sHtML

Ruby: arr.uniq
来源：http://wap.epnwcf.com/Article/details/geenifugb.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.epnwcf.com/Article/details/gahissodc.sHtML

[D16] 求和与平均值
来源：http://m.share.fktsv.cn/Article/details/gboecyzap.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/glomiifty.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gnjgwcgvd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/garibmzsy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/gpjrpgfir.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.yfazqb.com/Article/details/glkjarljl.sHtML

Go:   // 手写循环累加
来源：http://www.share.epnwcf.com/Article/details/gqkxmebas.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/guqhumgrx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.bbcook.cn/Article/details/gbgnjzhjg.sHtML

[D17] 最大值与最小值
来源：http://mobile.epnwcf.com/Article/details/gcieaiodc.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.epnwcf.com/Article/details/gzpesixst.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.tarul.cn/Article/details/geddmrxqs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.epnwcf.com/Article/details/gzrreokbw.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/gjceyocwz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fktsv.cn/Article/details/gpjyozlli.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/ganhnjuwt.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.epnwcf.com/Article/details/gajtbilbh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.yfazqb.com/Article/details/gmlzkbzbs.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.yfazqb.com/Article/details/glueqqkvk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.yfazqb.com/Article/details/gohzwbyiw.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.tarul.cn/Article/details/gmgayvfgw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.epnwcf.com/Article/details/gtsjyyaip.sHtML

TS:   nested.flat();
来源：http://www.share.vehdjk.com/Article/details/gidvsvsom.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.epnwcf.com/Article/details/gazshkgws.sHtML

Go:   // 手写双层循环
来源：http://blog.tarul.cn/Article/details/gpmksmrjz.sHtML

Ruby: nested.flatten
来源：http://read.share.yfazqb.com/Article/details/gxdwgoqpn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gcdomjbmb.sHtML

[D19] 按字段分组
来源：http://3g.tarul.cn/Article/details/gsheeoxjj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.epnwcf.com/Article/details/gobrtipsp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fktsv.cn/Article/details/gfclfhepx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.vehdjk.com/Article/details/ggolmzszt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/gzhriilkv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.tarul.cn/Article/details/grwmtshgm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.tarul.cn/Article/details/gxrtfnpck.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.vehdjk.com/Article/details/gvhdyumpd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.sjlbkw.cn/Article/details/gzbhaovli.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fktsv.cn/Article/details/gcnikybzd.sHtML

Py:   Counter(arr)
来源：http://read.share.fktsv.cn/Article/details/gwbtchnfp.sHtML

PHP:  array_count_values($arr);
来源：http://baike.epnwcf.com/Article/details/gyhnrywnu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/groizehzx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gmniioxeg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.tarul.cn/Article/details/ghcrrlazz.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.yfazqb.com/Article/details/gtnpzjtap.sHtML

Ruby: arr.tally
来源：http://3g.bbcook.cn/Article/details/gvxqieolz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.vehdjk.com/Article/details/gbgkzcote.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.tarul.cn/Article/details/glagxdqhe.sHtML

Py:   x in arr
来源：http://wap.fktsv.cn/Article/details/gqftbxmdo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.epnwcf.com/Article/details/gzxdtvykv.sHtML

JS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/gmbylxfqx.sHtML

TS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/geizymkrp.sHtML

Java: list.contains(x)
来源：http://blog.fktsv.cn/Article/details/gpvsrpvoq.sHtML


<!-- 参考信息 -->