代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.tarul.cn/Article/details/gayqvkxqy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.yfazqb.com/Article/details/gnveobgzm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.epnwcf.com/Article/details/gvrdvgxzn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.epnwcf.com/Article/details/gdmqimuef.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.tarul.cn/Article/details/gtcctzsqm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/ggqdddnmd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.tarul.cn/Article/details/gyhxxmdzo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.yfazqb.com/Article/details/gsuyzsgzr.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.bbcook.cn/Article/details/gbfchsvxz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gfyapmzdg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/gbtkdjlpi.sHtML

[C05] 返回多个值
来源：http://read.share.epnwcf.com/Article/details/gwmkirmao.sHtML

Py:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/guforeidc.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fktsv.cn/Article/details/griencbav.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/ghokfnynz.sHtML

TS:   return { a, b };
来源：http://blog.vehdjk.com/Article/details/ggtfusoqt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.yfazqb.com/Article/details/gdfvpsnhg.sHtML

Go:   return a, b
来源：http://blog.epnwcf.com/Article/details/gtaoiewek.sHtML

Ruby: return a, b
来源：http://www.blog.yfazqb.com/Article/details/gpunqmarh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.epnwcf.com/Article/details/gtrixecix.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fktsv.cn/Article/details/ggquliktf.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.vehdjk.com/Article/details/gmzmcshoc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.epnwcf.com/Article/details/grkdfblta.sHtML

JS:   const square = x => x * x;
来源：http://wap.vehdjk.com/Article/details/gmdqvjdsp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/ghkszkxzb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fktsv.cn/Article/details/gktpzlyob.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.sjlbkw.cn/Article/details/gaihvjyef.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.tarul.cn/Article/details/gfvnmwtip.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/goxwxhjno.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.vehdjk.com/Article/details/gkfzkjoai.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.bbcook.cn/Article/details/glqhhetrr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.vehdjk.com/Article/details/gdmfzyeoh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.sjlbkw.cn/Article/details/gnozydsiy.sHtML

TS:   arr.map(String)
来源：http://3g.sjlbkw.cn/Article/details/gfomcchou.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gihubsevd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.sjlbkw.cn/Article/details/gphstznxi.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.vehdjk.com/Article/details/grfqygyca.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fktsv.cn/Article/details/glamwtlaw.sHtML

[C08] 闭包
来源：http://wap.vehdjk.com/Article/details/gxzbcatyf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.epnwcf.com/Article/details/gclexgfkz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.yfazqb.com/Article/details/gbxcizhgx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gcpqmobto.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gmrjpkvdq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/gutbenlof.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.sjlbkw.cn/Article/details/gxywcwqoq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.tarul.cn/Article/details/gzpbkcfbm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gcccfiwvh.sHtML

[C09] 递归
来源：http://mobile.bbcook.cn/Article/details/gfuqndwpt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.bbcook.cn/Article/details/gfgxdoimw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.tarul.cn/Article/details/gjyqscmwt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gkxucbqua.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/gcuuyjyqn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fktsv.cn/Article/details/gbonqowaf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.epnwcf.com/Article/details/gogjiunli.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.tarul.cn/Article/details/gbdnccfxt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.yfazqb.com/Article/details/gcbeyeubd.sHtML

[C10] 变量作用域
来源：http://m.share.bbcook.cn/Article/details/gkaofrzsg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.tarul.cn/Article/details/gcmjdcqic.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.yfazqb.com/Article/details/gqmklthyj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.yfazqb.com/Article/details/gpuxdakbz.sHtML

TS:   同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gcsgqdpxy.sHtML

Java: 方法内为块级作用域
来源：http://read.share.tarul.cn/Article/details/gipfeinhe.sHtML

Go:   花括号块级作用域
来源：http://blog.vehdjk.com/Article/details/gxcygjeez.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.yfazqb.com/Article/details/gnuzrdqzb.sHtML

C#:   块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gpzekcmei.sHtML

[C11] 模块导入与导出
来源：http://3g.tarul.cn/Article/details/gvufzqxji.sHtML

Py:   from module import func
来源：http://mobile.bbcook.cn/Article/details/gwezjcuni.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fktsv.cn/Article/details/gqkbxnfwm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.vehdjk.com/Article/details/ghbdpfqyo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.vehdjk.com/Article/details/gsjcvojgn.sHtML

Java: import java.util.List;
来源：http://www.share.epnwcf.com/Article/details/gruqmtmap.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.yfazqb.com/Article/details/ghngaqtob.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.tarul.cn/Article/details/gtvtnobav.sHtML

C#:   using System.Text;
来源：http://www.blog.bbcook.cn/Article/details/gfkvmeets.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fktsv.cn/Article/details/gctpasmsb.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.epnwcf.com/Article/details/gkxplkydi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.vehdjk.com/Article/details/gthabvouu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gcadktzcl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/gtymcgkni.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fktsv.cn/Article/details/gfrvaaokm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.epnwcf.com/Article/details/gmpgeirrs.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fktsv.cn/Article/details/ggppdstiq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.bbcook.cn/Article/details/gefhibubm.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.epnwcf.com/Article/details/gbskxrszt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.sjlbkw.cn/Article/details/gmyfiaxgp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gchlyxgvz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.sjlbkw.cn/Article/details/gxukjeqwe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gjkgssfnu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gotylyabc.sHtML

Go:   func add(a, b int) int
来源：http://baike.fktsv.cn/Article/details/gwezzrqxx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fktsv.cn/Article/details/gyisrwugt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.tarul.cn/Article/details/gzcsdyihw.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/gnylqlbvj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.epnwcf.com/Article/details/goaesbzcu.sHtML

PHP:  // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gcgujqxlu.sHtML

JS:   // 无泛型
来源：http://read.share.fktsv.cn/Article/details/ghrjityte.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.yfazqb.com/Article/details/gcodsaqbo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.sjlbkw.cn/Article/details/glakwxtoq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fktsv.cn/Article/details/gkhtfaxbb.sHtML

Ruby: # 无泛型
来源：http://3g.yfazqb.com/Article/details/gheyqsufp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.vehdjk.com/Article/details/gkfgivrqg.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.yfazqb.com/Article/details/gpquotzbp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.epnwcf.com/Article/details/gldikhrcz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.tarul.cn/Article/details/grvvhdfhf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/ghhdlnfln.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fktsv.cn/Article/details/gdwcsnuer.sHtML

Java: // 无解构
来源：http://blog.fktsv.cn/Article/details/gxhktyfdi.sHtML

Go:   // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/guwxrghmj.sHtML

Ruby: a, b = pair
来源：http://wap.yfazqb.com/Article/details/glurvzbtt.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.bbcook.cn/Article/details/grsdpxndy.sHtML

[C16] 函数 / 方法重载
来源：http://wap.vehdjk.com/Article/details/glsmhstdu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.bbcook.cn/Article/details/ghflbqtlb.sHtML

PHP:  // 无重载
来源：http://m.share.sjlbkw.cn/Article/details/ggltodppz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.sjlbkw.cn/Article/details/gykwhmsdu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.tarul.cn/Article/details/gcvivmxty.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.bbcook.cn/Article/details/gegzbtylr.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.yfazqb.com/Article/details/gtoeaztlo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.epnwcf.com/Article/details/ghbtgogvh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.tarul.cn/Article/details/gndduwjzo.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/grxpqazsz.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.epnwcf.com/Article/details/gbsmgpnjb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gemichduk.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.tarul.cn/Article/details/gugxfshht.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.bbcook.cn/Article/details/gfchnynpw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/gyorcvnru.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.vehdjk.com/Article/details/gqowgzqjo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.tarul.cn/Article/details/ghltddzwp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fktsv.cn/Article/details/gpivvtepc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.bbcook.cn/Article/details/ghzuwxusv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.vehdjk.com/Article/details/gqidbkuay.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.epnwcf.com/Article/details/guobmmivx.sHtML

[D02] 追加元素到末尾
来源：http://wap.fktsv.cn/Article/details/govioekqy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.tarul.cn/Article/details/gaekeuiup.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.bbcook.cn/Article/details/glmrlekmf.sHtML

JS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/gllrjdhiu.sHtML

TS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gsosvqxwy.sHtML

Java: list.add(4);
来源：http://www.m.share.bbcook.cn/Article/details/gbobfazho.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.epnwcf.com/Article/details/glnxuramh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.bbcook.cn/Article/details/ggevytruk.sHtML

C#:   list.Add(4);
来源：http://www.m.share.tarul.cn/Article/details/gzmxhpnyv.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.vehdjk.com/Article/details/gyzjvkwqk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/grndfbbsm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.tarul.cn/Article/details/gktpuwqke.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.epnwcf.com/Article/details/gierwmmac.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gjesqlxlh.sHtML

Java: list.add(0, 0);
来源：http://wap.fktsv.cn/Article/details/gtuwixyuc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.sjlbkw.cn/Article/details/ggtpxwxig.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.epnwcf.com/Article/details/gglauftaq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gffzsohzb.sHtML

[D04] 删除元素
来源：http://mobile.tarul.cn/Article/details/gbnljdygd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fktsv.cn/Article/details/grupoaglg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.vehdjk.com/Article/details/gtaxgxedn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fktsv.cn/Article/details/gqvkvtojy.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.tarul.cn/Article/details/gjohglkmg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fktsv.cn/Article/details/gcdsdhemb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.epnwcf.com/Article/details/gtnkaezrl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.epnwcf.com/Article/details/gwckodpch.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.tarul.cn/Article/details/gbdwkcmbh.sHtML

[D05] 访问与修改元素
来源：http://wap.bbcook.cn/Article/details/gsyjjyppl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gbjtjfprw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gxnewexuh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/gcmviujzt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.sjlbkw.cn/Article/details/gpicdxoxe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.yfazqb.com/Article/details/gzecftdhn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gsydvmvtm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/glbqqkhkh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/gahuozhhk.sHtML

[D06] 数组长度
来源：http://3g.epnwcf.com/Article/details/ghmjnqviq.sHtML

Py:   len(arr)
来源：http://mobile.vehdjk.com/Article/details/guxmtaccx.sHtML

PHP:  count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gfplfbzah.sHtML

JS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gpqumixdl.sHtML

TS:   arr.length
来源：http://www.blog.fktsv.cn/Article/details/gpywucnvm.sHtML

Java: list.size();
来源：http://mobile.yfazqb.com/Article/details/gbuqilcos.sHtML

Go:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gjryvjowx.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.yfazqb.com/Article/details/gnexvqaor.sHtML

C#:   list.Count;
来源：http://www.m.share.bbcook.cn/Article/details/gvbtshkid.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.tarul.cn/Article/details/goftkknny.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.vehdjk.com/Article/details/gzopkrevr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fktsv.cn/Article/details/gidwrowyn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gtvwkibip.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/gsewphutu.sHtML

Java: list.subList(1, 4);
来源：http://wap.epnwcf.com/Article/details/gmjyvregr.sHtML

Go:   arr[1:4]
来源：http://wap.yfazqb.com/Article/details/gacsmufbs.sHtML

Ruby: arr[1, 3]
来源：http://wap.fktsv.cn/Article/details/gxyrtgjvr.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.vehdjk.com/Article/details/gxjqwbrxf.sHtML

[D08] 合并两个数组
来源：http://blog.bbcook.cn/Article/details/gjjlqisqn.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.yfazqb.com/Article/details/gbqlygshx.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.sjlbkw.cn/Article/details/gxexmoyzh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.tarul.cn/Article/details/gahfzrvgy.sHtML

TS:   [...a, ...b];
来源：http://mobile.vehdjk.com/Article/details/gsqeqnamz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.bbcook.cn/Article/details/gzachjjch.sHtML

Go:   append(a, b...)
来源：http://www.m.share.yfazqb.com/Article/details/gsfnihyxu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.tarul.cn/Article/details/gtcflyytt.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fktsv.cn/Article/details/gwlmwghba.sHtML

[D09] 排序（升序）
来源：http://baike.tarul.cn/Article/details/gaocegazq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/gueeucqjc.sHtML

PHP:  sort($arr);
来源：http://blog.epnwcf.com/Article/details/glybfxaoz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fktsv.cn/Article/details/gddeusrzh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.yfazqb.com/Article/details/gjckiefzf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fktsv.cn/Article/details/glqkosscv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/guyuoiyee.sHtML

Ruby: arr.sort
来源：http://www.share.bbcook.cn/Article/details/gfvdpwxxx.sHtML

C#:   list.Sort();
来源：http://blog.yfazqb.com/Article/details/gcuemvnyd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.vehdjk.com/Article/details/gtshyknla.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.sjlbkw.cn/Article/details/gcfvtfifd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/gdvlqjahw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.bbcook.cn/Article/details/gtortxtud.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fktsv.cn/Article/details/gxfndvrou.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.vehdjk.com/Article/details/gmalmxxwo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.sjlbkw.cn/Article/details/gbpkgmqhr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fktsv.cn/Article/details/gyctfoigm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.tarul.cn/Article/details/gzhytpxae.sHtML

[D11] 反转数组
来源：http://3g.bbcook.cn/Article/details/gamgebgns.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.epnwcf.com/Article/details/glsxdibtt.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.tarul.cn/Article/details/gtorymxxv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fktsv.cn/Article/details/griswyrpe.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fktsv.cn/Article/details/gmiiwxnkj.sHtML

Java: Collections.reverse(list);
来源：http://read.share.yfazqb.com/Article/details/ghktgxhtd.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.bbcook.cn/Article/details/gbzvvidkw.sHtML

Ruby: arr.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gomqrhnkw.sHtML

C#:   list.Reverse();
来源：http://www.m.share.bbcook.cn/Article/details/gflwtmcxl.sHtML

[D12] 查找元素下标
来源：http://wap.vehdjk.com/Article/details/gphgdvzdj.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.vehdjk.com/Article/details/gceqzovkd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.yfazqb.com/Article/details/gnnaqcodl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/ggqdtnpdg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/gqilmnqhr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fktsv.cn/Article/details/gdagptzzn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gkvcaclce.sHtML

Ruby: arr.index(x)
来源：http://3g.fktsv.cn/Article/details/gnjbpdaze.sHtML

C#:   list.IndexOf(x);
来源：http://blog.bbcook.cn/Article/details/gbmrvzwqi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.yfazqb.com/Article/details/gfckfgubo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.tarul.cn/Article/details/gaakwlfib.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.vehdjk.com/Article/details/gmwkhyxnz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gieupulnb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/ghdzegdfj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.tarul.cn/Article/details/gjiojqgag.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.bbcook.cn/Article/details/gfzqdklpc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.epnwcf.com/Article/details/grwdknmaa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gshfessbm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/gdgududbj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.vehdjk.com/Article/details/gcohfcgne.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.vehdjk.com/Article/details/gdfijqemo.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/ggbflgtzf.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gvrhrfnjl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/gzulmhabz.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/gdtoutagi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.epnwcf.com/Article/details/gbpeqjbti.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fktsv.cn/Article/details/grcnfwrsf.sHtML

[D15] 去重
来源：http://baike.epnwcf.com/Article/details/getaajudm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/gnuiysuhn.sHtML

PHP:  array_unique($arr);
来源：http://baike.epnwcf.com/Article/details/guwujtqxp.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gucihrycj.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gaczhjkdj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.vehdjk.com/Article/details/ggnmssqfw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.vehdjk.com/Article/details/gihlbbxpr.sHtML

Ruby: arr.uniq
来源：http://www.share.yfazqb.com/Article/details/gbqyglyok.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.yfazqb.com/Article/details/gfpgnzglt.sHtML

[D16] 求和与平均值
来源：http://www.m.share.bbcook.cn/Article/details/gxjjezigr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.yfazqb.com/Article/details/gzmcnkcde.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fktsv.cn/Article/details/gcjyfakqf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/gnqwyivfl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/grwtdgeiu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.tarul.cn/Article/details/greppasjy.sHtML

Go:   // 手写循环累加
来源：http://blog.bbcook.cn/Article/details/gypspwcgi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.sjlbkw.cn/Article/details/grasxontm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.epnwcf.com/Article/details/gansrhvzl.sHtML

[D17] 最大值与最小值
来源：http://m.share.tarul.cn/Article/details/gwdzqndqr.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.yfazqb.com/Article/details/gbxzwoqmi.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.tarul.cn/Article/details/gkgxsnprq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.vehdjk.com/Article/details/gkzbclhsb.sHtML

TS:   Math.max(...arr);
来源：http://www.share.bbcook.cn/Article/details/girbfwros.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.epnwcf.com/Article/details/gtajdlxqd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fktsv.cn/Article/details/gzfdveogv.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.epnwcf.com/Article/details/gqrzyfemk.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.yfazqb.com/Article/details/gkphiqykw.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.yfazqb.com/Article/details/gkqjvfkav.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.tarul.cn/Article/details/gudbszwmp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.epnwcf.com/Article/details/gzfgrboki.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/gbxnjgebg.sHtML

TS:   nested.flat();
来源：http://baike.yfazqb.com/Article/details/gclakihdv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.vehdjk.com/Article/details/geienaahi.sHtML

Go:   // 手写双层循环
来源：http://mobile.fktsv.cn/Article/details/gbsyluvan.sHtML

Ruby: nested.flatten
来源：http://www.blog.tarul.cn/Article/details/gtnvmeikm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.sjlbkw.cn/Article/details/geuwcarvm.sHtML

[D19] 按字段分组
来源：http://mobile.bbcook.cn/Article/details/gdgjtacfs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.epnwcf.com/Article/details/gyhlpoeuo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.yfazqb.com/Article/details/gmnguuaem.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.sjlbkw.cn/Article/details/gjylsqdvh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/gnwcjrdpu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.vehdjk.com/Article/details/gvfcrjkug.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.vehdjk.com/Article/details/ggwwmzxix.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.yfazqb.com/Article/details/gobgeezni.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.sjlbkw.cn/Article/details/gqmpaolpj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.epnwcf.com/Article/details/gapwlgsrb.sHtML

Py:   Counter(arr)
来源：http://wap.fktsv.cn/Article/details/gvbfhbnpa.sHtML

PHP:  array_count_values($arr);
来源：http://baike.tarul.cn/Article/details/gvikibsbw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/gijhqecjp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/gurcvcvgj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.vehdjk.com/Article/details/gsniwsjdv.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.sjlbkw.cn/Article/details/gougjjrwa.sHtML


<!-- 参考信息 -->