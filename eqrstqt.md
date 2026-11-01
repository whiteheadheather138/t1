代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://mobile.epnwcf.com/Article/details/grjujgdoh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/grgomuuac.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gqfzwajbc.sHtML

[C05] 返回多个值
来源：http://www.share.fktsv.cn/Article/details/gdqbashwf.sHtML

Py:   return a, b
来源：http://blog.fktsv.cn/Article/details/gqnctqevi.sHtML

PHP:  return [$a, $b];
来源：http://baike.epnwcf.com/Article/details/gznywxata.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/gbbmuxkqq.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gqvrcglro.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fktsv.cn/Article/details/galmebdfd.sHtML

Go:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gvhdzlpih.sHtML

Ruby: return a, b
来源：http://wap.fktsv.cn/Article/details/goywnaniv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.sjlbkw.cn/Article/details/gonurlrin.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.yfazqb.com/Article/details/gpasomljx.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.vehdjk.com/Article/details/gshnovmyf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.yfazqb.com/Article/details/gudohezzu.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gbxwutnpg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.tarul.cn/Article/details/gahtslebk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.epnwcf.com/Article/details/gorhpjtfu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.vehdjk.com/Article/details/gzfrwdzij.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.epnwcf.com/Article/details/gixudscpy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/gmzralddl.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fktsv.cn/Article/details/gujhlspwn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.sjlbkw.cn/Article/details/gtnkscvhb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.tarul.cn/Article/details/gfwpcbymg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.vehdjk.com/Article/details/glvvrfvru.sHtML

TS:   arr.map(String)
来源：http://www.m.share.yfazqb.com/Article/details/gjihybrxq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.epnwcf.com/Article/details/gvqtdsdgp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fktsv.cn/Article/details/godortzmi.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.sjlbkw.cn/Article/details/gvudctfks.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.sjlbkw.cn/Article/details/gsagmwmeo.sHtML

[C08] 闭包
来源：http://read.share.sjlbkw.cn/Article/details/gevewbjln.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/gfyicnahu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.vehdjk.com/Article/details/gkjyjbymr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/gfgigcwup.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gvwnjehqd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.vehdjk.com/Article/details/gwpuqwqjz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.sjlbkw.cn/Article/details/gpraeikhe.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.yfazqb.com/Article/details/gqciixzts.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/giaiqrrsi.sHtML

[C09] 递归
来源：http://3g.epnwcf.com/Article/details/ggfvjzavv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/ghphjmvoi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.tarul.cn/Article/details/gazgczfhm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.epnwcf.com/Article/details/gcwuemxin.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gpmcemzkm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.sjlbkw.cn/Article/details/gvidcqpiu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fktsv.cn/Article/details/ggvwotjlq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.tarul.cn/Article/details/gagyatjcy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.vehdjk.com/Article/details/glkrtewdi.sHtML

[C10] 变量作用域
来源：http://www.share.vehdjk.com/Article/details/gaqthsxen.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.sjlbkw.cn/Article/details/gxzkwucto.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.vehdjk.com/Article/details/gnbbnymvv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fktsv.cn/Article/details/gwxaonfpk.sHtML

TS:   同 JS
来源：http://www.blog.fktsv.cn/Article/details/gsdiubtnq.sHtML

Java: 方法内为块级作用域
来源：http://m.share.tarul.cn/Article/details/gghbshtii.sHtML

Go:   花括号块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gzqqcnxij.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.epnwcf.com/Article/details/gfcvvjimp.sHtML

C#:   块级作用域
来源：http://baike.fktsv.cn/Article/details/gihhbfbcy.sHtML

[C11] 模块导入与导出
来源：http://3g.bbcook.cn/Article/details/gkezfdvhp.sHtML

Py:   from module import func
来源：http://mobile.sjlbkw.cn/Article/details/gznwlvgxv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.sjlbkw.cn/Article/details/gsokicynn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.vehdjk.com/Article/details/gqntjxsww.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.bbcook.cn/Article/details/gmuqujtsd.sHtML

Java: import java.util.List;
来源：http://m.share.bbcook.cn/Article/details/gdgrrdmbq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.yfazqb.com/Article/details/gwtcclrdf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.yfazqb.com/Article/details/ghabnajlj.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/gpcsdiqpv.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.yfazqb.com/Article/details/gfnvebiuc.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.vehdjk.com/Article/details/ghpqcrzok.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.yfazqb.com/Article/details/gshocswrc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/gzbnlrddc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fktsv.cn/Article/details/gisuymurz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.vehdjk.com/Article/details/gndayntrl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fktsv.cn/Article/details/gxaixgoha.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.vehdjk.com/Article/details/gplfzavrv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.bbcook.cn/Article/details/gcnjaolca.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.yfazqb.com/Article/details/gfszsryus.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.sjlbkw.cn/Article/details/gioqzztdy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gneuaqktw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.sjlbkw.cn/Article/details/gyppmtekd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gbnkefaja.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/grhisfuby.sHtML

Go:   func add(a, b int) int
来源：http://baike.epnwcf.com/Article/details/galbnbgdv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.bbcook.cn/Article/details/ghduxhiia.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.tarul.cn/Article/details/gwlnsjtde.sHtML

[C14] 泛型函数
来源：http://read.share.yfazqb.com/Article/details/gkfpqrgnd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fktsv.cn/Article/details/gxgtievrn.sHtML

PHP:  // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gpcnmzttm.sHtML

JS:   // 无泛型
来源：http://blog.vehdjk.com/Article/details/gmmzmgkma.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fktsv.cn/Article/details/gxpsqfnkd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.yfazqb.com/Article/details/gvtlgfkla.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fktsv.cn/Article/details/gxeuspjpz.sHtML

Ruby: # 无泛型
来源：http://wap.yfazqb.com/Article/details/gugiszqzq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fktsv.cn/Article/details/gmwgcaxgg.sHtML

[C15] 解构 / 展开参数
来源：http://3g.epnwcf.com/Article/details/gnkwetglq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.sjlbkw.cn/Article/details/gxtmdeoag.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.tarul.cn/Article/details/gwdwzasgf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.yfazqb.com/Article/details/ggifcqwnd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.tarul.cn/Article/details/gnkljsawx.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/gfgqdoqjz.sHtML

Go:   // 无解构
来源：http://read.share.bbcook.cn/Article/details/gzsgqvzox.sHtML

Ruby: a, b = pair
来源：http://read.share.bbcook.cn/Article/details/gbqbgxacz.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.tarul.cn/Article/details/gkyxvlvoi.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fktsv.cn/Article/details/gimzccnwj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.yfazqb.com/Article/details/gemcknwco.sHtML

PHP:  // 无重载
来源：http://baike.epnwcf.com/Article/details/gafwmpkba.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.bbcook.cn/Article/details/gacplqzty.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.vehdjk.com/Article/details/gzrrdmyoo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.bbcook.cn/Article/details/gqymkmzjs.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.bbcook.cn/Article/details/gpgpaviuw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.vehdjk.com/Article/details/gzhcicufh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.vehdjk.com/Article/details/gmyinoxks.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gedeaglby.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.epnwcf.com/Article/details/gglyrqbdj.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gcxoocxew.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.yfazqb.com/Article/details/gatqebwwb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.epnwcf.com/Article/details/gsmrnlvdh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fktsv.cn/Article/details/gznvejlfl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gwvsxjagp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.vehdjk.com/Article/details/gcytndave.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.yfazqb.com/Article/details/gbxknvkzm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.sjlbkw.cn/Article/details/gmsrwdqcl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.yfazqb.com/Article/details/grpcsfmpn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.tarul.cn/Article/details/gduwfbjxv.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.tarul.cn/Article/details/gpnccghiz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.bbcook.cn/Article/details/gnhocrlkr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.sjlbkw.cn/Article/details/gjdhfuqvd.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gnumcegiq.sHtML

TS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/gikptutkl.sHtML

Java: list.add(4);
来源：http://3g.sjlbkw.cn/Article/details/ghevegtvh.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.tarul.cn/Article/details/gkrjemepv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.vehdjk.com/Article/details/gtujcizup.sHtML

C#:   list.Add(4);
来源：http://3g.fktsv.cn/Article/details/gxmjctokh.sHtML

[D03] 在指定位置插入元素
来源：http://blog.yfazqb.com/Article/details/gtetnaizd.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fktsv.cn/Article/details/ghrbpqyse.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.sjlbkw.cn/Article/details/gebposrpi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.epnwcf.com/Article/details/gftnunggh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.tarul.cn/Article/details/geslmfrtp.sHtML

Java: list.add(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gzmrwxjyi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.epnwcf.com/Article/details/grfvndrtb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.bbcook.cn/Article/details/gcjpzacrr.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gmbioiafn.sHtML

[D04] 删除元素
来源：http://mobile.yfazqb.com/Article/details/gflllrajo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.vehdjk.com/Article/details/gqfhftibf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.epnwcf.com/Article/details/gxhzdpsqr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbjiokkz.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.bbcook.cn/Article/details/gxplttdes.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.sjlbkw.cn/Article/details/gnrnvuomq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.sjlbkw.cn/Article/details/gbivrcoyk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.epnwcf.com/Article/details/gwqixqrmw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.tarul.cn/Article/details/gngtpkxqt.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fktsv.cn/Article/details/gpipooxaa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/gavqavbts.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gpxagewul.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gpnoalnlw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.bbcook.cn/Article/details/gtoxzeupd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.sjlbkw.cn/Article/details/gdhyjpwop.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gldvrrkzp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/gckggroyh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gyfygsbuv.sHtML

[D06] 数组长度
来源：http://blog.bbcook.cn/Article/details/gjqjmxoxc.sHtML

Py:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/gkpwbtxce.sHtML

PHP:  count($arr);
来源：http://m.share.yfazqb.com/Article/details/ggqerlvsq.sHtML

JS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/glgsqudyz.sHtML

TS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/gifuazeck.sHtML

Java: list.size();
来源：http://3g.epnwcf.com/Article/details/gvopaxhmd.sHtML

Go:   len(arr)
来源：http://wap.tarul.cn/Article/details/gvlzeievs.sHtML

Ruby: arr.length; arr.size
来源：http://3g.sjlbkw.cn/Article/details/gagtqjbzz.sHtML

C#:   list.Count;
来源：http://www.m.share.tarul.cn/Article/details/gwmecjwbs.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fktsv.cn/Article/details/gjkzrjkux.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.vehdjk.com/Article/details/gbzufabym.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.vehdjk.com/Article/details/gxuufgwns.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/gonppibqj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gojlscnts.sHtML

Java: list.subList(1, 4);
来源：http://blog.epnwcf.com/Article/details/giuajrhfg.sHtML

Go:   arr[1:4]
来源：http://blog.yfazqb.com/Article/details/gykwfigxm.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.tarul.cn/Article/details/glwqjinzd.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/ghcificzi.sHtML

[D08] 合并两个数组
来源：http://www.share.yfazqb.com/Article/details/gocwbhtue.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.bbcook.cn/Article/details/gjgqrpuqq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.tarul.cn/Article/details/goxrzymns.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.sjlbkw.cn/Article/details/gywrdusec.sHtML

TS:   [...a, ...b];
来源：http://m.share.yfazqb.com/Article/details/gmuforrpb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.bbcook.cn/Article/details/goozbjrsd.sHtML

Go:   append(a, b...)
来源：http://blog.bbcook.cn/Article/details/gahooyqpl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.bbcook.cn/Article/details/gtlnebqin.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.epnwcf.com/Article/details/guhnkvwwn.sHtML

[D09] 排序（升序）
来源：http://www.share.bbcook.cn/Article/details/glncahiyy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gdfjwypzh.sHtML

PHP:  sort($arr);
来源：http://mobile.tarul.cn/Article/details/gugppvcrx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fktsv.cn/Article/details/gjwdzlgyi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.bbcook.cn/Article/details/gklwkzscj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.vehdjk.com/Article/details/gfvlepqed.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gzhubinyw.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/goopcocnp.sHtML

C#:   list.Sort();
来源：http://wap.bbcook.cn/Article/details/gnxdeeztk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.tarul.cn/Article/details/gfitgxldt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.sjlbkw.cn/Article/details/ghzapmzpt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/ggtjfxvzh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fktsv.cn/Article/details/gwmznuxzb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gmlanhiox.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.epnwcf.com/Article/details/glkuqhngb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.sjlbkw.cn/Article/details/gsgchrgbo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.vehdjk.com/Article/details/gtuyjxfbg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.tarul.cn/Article/details/gpoutfwco.sHtML

[D11] 反转数组
来源：http://mobile.yfazqb.com/Article/details/ghzkljesm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.sjlbkw.cn/Article/details/geirdybsc.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.tarul.cn/Article/details/gsjgqnlhp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.epnwcf.com/Article/details/gzamxbond.sHtML

TS:   [...arr].reverse();
来源：http://www.share.tarul.cn/Article/details/gjnlirxct.sHtML

Java: Collections.reverse(list);
来源：http://www.share.epnwcf.com/Article/details/gypsxvjph.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.sjlbkw.cn/Article/details/gcyytzfur.sHtML

Ruby: arr.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gvnpxxqgq.sHtML

C#:   list.Reverse();
来源：http://3g.yfazqb.com/Article/details/gfjbsbpzn.sHtML

[D12] 查找元素下标
来源：http://3g.vehdjk.com/Article/details/gvnbtpcfl.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.vehdjk.com/Article/details/gaappwvhb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.tarul.cn/Article/details/ggjqpvgmr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/ghdaxcflm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gcgmofyqq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.vehdjk.com/Article/details/gsqqgcwwz.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.tarul.cn/Article/details/gemgjwdon.sHtML

Ruby: arr.index(x)
来源：http://3g.yfazqb.com/Article/details/gotvyrxhp.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fktsv.cn/Article/details/gwktfaikc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.sjlbkw.cn/Article/details/gnrvkvuze.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.yfazqb.com/Article/details/gilqgtjyw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.yfazqb.com/Article/details/gqkkkikck.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gdumckrys.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gcoxpnian.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.vehdjk.com/Article/details/gfrrnogrn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.yfazqb.com/Article/details/gurpmwodf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.bbcook.cn/Article/details/gmchjrrzm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.bbcook.cn/Article/details/gfnidkqew.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.tarul.cn/Article/details/gvdwymofc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.yfazqb.com/Article/details/gecmezkha.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.sjlbkw.cn/Article/details/gowymmtuk.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gevzqmguc.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/grvgicndr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.epnwcf.com/Article/details/glepinyvm.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/gxjflffha.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.yfazqb.com/Article/details/gnsbbkhuw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gwgfottio.sHtML

[D15] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gygqznizc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/gnqyutduw.sHtML

PHP:  array_unique($arr);
来源：http://wap.sjlbkw.cn/Article/details/gnbqlspuh.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/gkhspmhqo.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gmrbqlsql.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.yfazqb.com/Article/details/gbwzqqabe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.sjlbkw.cn/Article/details/gwxfdgbey.sHtML

Ruby: arr.uniq
来源：http://blog.sjlbkw.cn/Article/details/gxtrkyjbl.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gexreeoah.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/gbbyibbnh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.vehdjk.com/Article/details/ghvxallwm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fktsv.cn/Article/details/gbxnihckq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fktsv.cn/Article/details/gmunwqylq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/gqnkauvap.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.epnwcf.com/Article/details/gletfypxl.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gptvrqeql.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.epnwcf.com/Article/details/gzxbkaznx.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.bbcook.cn/Article/details/gadsoyfkl.sHtML

[D17] 最大值与最小值
来源：http://3g.bbcook.cn/Article/details/gmxahafra.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/gegqpkjpz.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fktsv.cn/Article/details/glhduhvgw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.sjlbkw.cn/Article/details/gqixjnxhq.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.yfazqb.com/Article/details/gvcuhigsh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fktsv.cn/Article/details/gfbhddyvw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/glzntboxu.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.sjlbkw.cn/Article/details/ghfedoeyn.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.bbcook.cn/Article/details/gsddloexc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fktsv.cn/Article/details/gpqduepcc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.vehdjk.com/Article/details/gotftyufw.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.epnwcf.com/Article/details/gufiwzfwo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.yfazqb.com/Article/details/gqlfghbbp.sHtML

TS:   nested.flat();
来源：http://read.share.epnwcf.com/Article/details/gpztrgbml.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.epnwcf.com/Article/details/gwtapawuz.sHtML

Go:   // 手写双层循环
来源：http://www.blog.vehdjk.com/Article/details/ggbngqvxo.sHtML

Ruby: nested.flatten
来源：http://read.share.yfazqb.com/Article/details/gjbmwdnfz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gufrsmjzj.sHtML

[D19] 按字段分组
来源：http://www.m.share.tarul.cn/Article/details/gsiithcvl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.epnwcf.com/Article/details/gzjuqpnzv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.vehdjk.com/Article/details/gnwxugzgf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.vehdjk.com/Article/details/gooqajkkc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.yfazqb.com/Article/details/gxfthvnre.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.bbcook.cn/Article/details/gjadwknpq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.vehdjk.com/Article/details/gsmzeomtl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.vehdjk.com/Article/details/gwrhwhsxu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.sjlbkw.cn/Article/details/gvqmsnrdt.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.tarul.cn/Article/details/grhesaiwq.sHtML

Py:   Counter(arr)
来源：http://m.share.bbcook.cn/Article/details/guigvbdzt.sHtML

PHP:  array_count_values($arr);
来源：http://3g.vehdjk.com/Article/details/gjdjiulxv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/ghobfpnid.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/gsjongsqq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.yfazqb.com/Article/details/gnpvgxlam.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.tarul.cn/Article/details/gxunykxqz.sHtML

Ruby: arr.tally
来源：http://www.share.yfazqb.com/Article/details/gdftxoopi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.sjlbkw.cn/Article/details/gqybbzcyt.sHtML

[D21] 判断是否包含某元素
来源：http://baike.sjlbkw.cn/Article/details/ghmuwndhs.sHtML

Py:   x in arr
来源：http://www.share.vehdjk.com/Article/details/gkkyrgyqn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.yfazqb.com/Article/details/gocvahpux.sHtML

JS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gocewhfaa.sHtML

TS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/gipdgxyng.sHtML

Java: list.contains(x)
来源：http://baike.vehdjk.com/Article/details/gxylnqqmy.sHtML


<!-- 参考信息 -->