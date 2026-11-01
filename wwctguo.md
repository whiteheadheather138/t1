代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.bbcook.cn/Article/details/gtzoowdrh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.yfazqb.com/Article/details/gaoxyyxdo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.bbcook.cn/Article/details/ggrpqwcjq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fktsv.cn/Article/details/gxdxqvemk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fktsv.cn/Article/details/gmsdmtmmd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/glornzmxe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.tarul.cn/Article/details/gulgbjmac.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.vehdjk.com/Article/details/gspmvvemg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.tarul.cn/Article/details/gidzljztg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gidtwoflf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gpnixxsfs.sHtML

[C05] 返回多个值
来源：http://blog.bbcook.cn/Article/details/grqbpfveh.sHtML

Py:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gdgjyrtaw.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fktsv.cn/Article/details/givqgbspj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.epnwcf.com/Article/details/ggyhxmsuu.sHtML

TS:   return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/gmpsxivlh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.epnwcf.com/Article/details/geikimfag.sHtML

Go:   return a, b
来源：http://baike.vehdjk.com/Article/details/gbzfdcxqr.sHtML

Ruby: return a, b
来源：http://blog.vehdjk.com/Article/details/gmzgcrsmk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.sjlbkw.cn/Article/details/gklqzkcvz.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.epnwcf.com/Article/details/gooskddaf.sHtML

Py:   square = lambda x: x * x
来源：http://blog.sjlbkw.cn/Article/details/gjrmvdhkk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.tarul.cn/Article/details/gptbhzihi.sHtML

JS:   const square = x => x * x;
来源：http://www.share.bbcook.cn/Article/details/gnvuycatg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.yfazqb.com/Article/details/gkhssaxoq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.yfazqb.com/Article/details/gnfwpmcxo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fktsv.cn/Article/details/gvlrixjuq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.yfazqb.com/Article/details/grnuwfwkv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/gdtqlhbmd.sHtML

[C07] 把函数作为参数传入
来源：http://blog.tarul.cn/Article/details/gorxwxzbq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.sjlbkw.cn/Article/details/gstbyvhgi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.bbcook.cn/Article/details/gflsxhybe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.tarul.cn/Article/details/gyuelgpof.sHtML

TS:   arr.map(String)
来源：http://www.blog.vehdjk.com/Article/details/gxvnzepaf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.vehdjk.com/Article/details/gbzfbfgoy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.sjlbkw.cn/Article/details/gyobugyvk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fktsv.cn/Article/details/gnpxchgyy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.epnwcf.com/Article/details/gbquhnyob.sHtML

[C08] 闭包
来源：http://www.share.yfazqb.com/Article/details/gaobvohff.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.vehdjk.com/Article/details/gblmtrqsg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.epnwcf.com/Article/details/genhvkkxh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/glmlyaksk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/ghvakadbz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.sjlbkw.cn/Article/details/gprajxvge.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.epnwcf.com/Article/details/gnbvnliov.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.sjlbkw.cn/Article/details/gguvgxkqo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gkaamlvqo.sHtML

[C09] 递归
来源：http://blog.bbcook.cn/Article/details/gvvxdqmot.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.tarul.cn/Article/details/gvtfvmkmo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gecfvtxwa.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fktsv.cn/Article/details/goheeeqpx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/gjxzbgnic.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fktsv.cn/Article/details/gndjwyypb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.bbcook.cn/Article/details/gfxlybxig.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.epnwcf.com/Article/details/giqwramby.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.epnwcf.com/Article/details/gwhnkuycl.sHtML

[C10] 变量作用域
来源：http://3g.vehdjk.com/Article/details/ggttohdwy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.epnwcf.com/Article/details/geprtkbiy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.yfazqb.com/Article/details/gafuhtllm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.tarul.cn/Article/details/gopohbeuc.sHtML

TS:   同 JS
来源：http://www.m.share.tarul.cn/Article/details/gmfbxnzzf.sHtML

Java: 方法内为块级作用域
来源：http://baike.epnwcf.com/Article/details/gbfrdwpoh.sHtML

Go:   花括号块级作用域
来源：http://3g.vehdjk.com/Article/details/guimhtybn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.epnwcf.com/Article/details/gyttkdzvf.sHtML

C#:   块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gyfdxmzhq.sHtML

[C11] 模块导入与导出
来源：http://wap.yfazqb.com/Article/details/ggeowxpwk.sHtML

Py:   from module import func
来源：http://www.blog.epnwcf.com/Article/details/gsqvcezfk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.yfazqb.com/Article/details/gixgivvvw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.sjlbkw.cn/Article/details/gjcsyxcgv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.yfazqb.com/Article/details/gcxwhymrl.sHtML

Java: import java.util.List;
来源：http://blog.sjlbkw.cn/Article/details/gllcnchgf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.bbcook.cn/Article/details/gvgmkxjad.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.tarul.cn/Article/details/giqbgvbdw.sHtML

C#:   using System.Text;
来源：http://3g.vehdjk.com/Article/details/ggtdscddd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.tarul.cn/Article/details/gxgbwppyl.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.bbcook.cn/Article/details/ggjroxibz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.bbcook.cn/Article/details/gvpqtjjgx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/gursdbrxv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.yfazqb.com/Article/details/gqkcifpbe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.tarul.cn/Article/details/greclzdmz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.sjlbkw.cn/Article/details/ghznkyggt.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.tarul.cn/Article/details/gsakcgzog.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.bbcook.cn/Article/details/gfulbhrzp.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.vehdjk.com/Article/details/gozhwmgmd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.tarul.cn/Article/details/gqbmnyjtc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gclmqtmtb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.epnwcf.com/Article/details/gbmegkzbi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gcwzpqsoz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gefdcsioi.sHtML

Go:   func add(a, b int) int
来源：http://www.share.sjlbkw.cn/Article/details/gpwhkhvnr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.bbcook.cn/Article/details/gxexklgru.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fktsv.cn/Article/details/gatrlyrhf.sHtML

[C14] 泛型函数
来源：http://blog.fktsv.cn/Article/details/gqnvnyhnp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.yfazqb.com/Article/details/glxuaapxp.sHtML

PHP:  // 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gcvnkjllg.sHtML

JS:   // 无泛型
来源：http://wap.fktsv.cn/Article/details/gamziwugq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.tarul.cn/Article/details/guobbfvdx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.bbcook.cn/Article/details/gagzzdymu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.sjlbkw.cn/Article/details/gyrfwgtse.sHtML

Ruby: # 无泛型
来源：http://blog.yfazqb.com/Article/details/gafwnuewb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.epnwcf.com/Article/details/gaspgsjjf.sHtML

[C15] 解构 / 展开参数
来源：http://3g.yfazqb.com/Article/details/gdujyaamz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.epnwcf.com/Article/details/gkfpgnjhw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.yfazqb.com/Article/details/gumoudsfa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.yfazqb.com/Article/details/gxtruwgsf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.sjlbkw.cn/Article/details/glalyheta.sHtML

Java: // 无解构
来源：http://baike.fktsv.cn/Article/details/galqsbcqp.sHtML

Go:   // 无解构
来源：http://blog.sjlbkw.cn/Article/details/gdaopwcnr.sHtML

Ruby: a, b = pair
来源：http://www.m.share.yfazqb.com/Article/details/gdyuiafuf.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.yfazqb.com/Article/details/gvtkxstlv.sHtML

[C16] 函数 / 方法重载
来源：http://blog.vehdjk.com/Article/details/gdnoajltb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.bbcook.cn/Article/details/gphjgsese.sHtML

PHP:  // 无重载
来源：http://blog.bbcook.cn/Article/details/gckmepync.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.tarul.cn/Article/details/gxbtldvve.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.vehdjk.com/Article/details/gacxwekot.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.epnwcf.com/Article/details/ghlnyjutw.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fktsv.cn/Article/details/ghpulbike.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fktsv.cn/Article/details/gcqkyliuh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.epnwcf.com/Article/details/grdgchygd.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gscvnaoqb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.yfazqb.com/Article/details/gdmxacdwf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gyllizchl.sHtML

[D01] 创建数组 / 列表
来源：http://3g.vehdjk.com/Article/details/gjrpluhwa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.yfazqb.com/Article/details/gtgssfwsw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.epnwcf.com/Article/details/gztgtzocd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.vehdjk.com/Article/details/gslettsuu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.tarul.cn/Article/details/ghxzbzwjv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.bbcook.cn/Article/details/gqibcymfb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.vehdjk.com/Article/details/gxphxvckj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.bbcook.cn/Article/details/gbdsktpbl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.epnwcf.com/Article/details/ghcwpcwxv.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.bbcook.cn/Article/details/gvpbrztsq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.tarul.cn/Article/details/gcmcaunnn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fktsv.cn/Article/details/gpyxldwml.sHtML

JS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/gynyrkcdt.sHtML

TS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gqpycbttc.sHtML

Java: list.add(4);
来源：http://mobile.fktsv.cn/Article/details/gcbnvsnnx.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.tarul.cn/Article/details/gqxoofnxb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.vehdjk.com/Article/details/gellflneh.sHtML

C#:   list.Add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnlwurdv.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.tarul.cn/Article/details/gpcpmszkg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.epnwcf.com/Article/details/gwfznpmak.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.epnwcf.com/Article/details/gcwrfvdbv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.bbcook.cn/Article/details/gjhdibuua.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.bbcook.cn/Article/details/gjcqdxqlj.sHtML

Java: list.add(0, 0);
来源：http://www.share.tarul.cn/Article/details/goiwkajnf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.tarul.cn/Article/details/ghkvnaqpq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.sjlbkw.cn/Article/details/gexctyxtd.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.vehdjk.com/Article/details/giklidfvd.sHtML

[D04] 删除元素
来源：http://www.share.bbcook.cn/Article/details/geovebhqm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.bbcook.cn/Article/details/gqciqnknv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.bbcook.cn/Article/details/gwqgbbmzf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.vehdjk.com/Article/details/gmxpuyjca.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.bbcook.cn/Article/details/ggelsndyk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.yfazqb.com/Article/details/gldufkrjp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.tarul.cn/Article/details/gnhalslub.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.bbcook.cn/Article/details/glamcvovl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.sjlbkw.cn/Article/details/gtyjwyorb.sHtML

[D05] 访问与修改元素
来源：http://m.share.sjlbkw.cn/Article/details/gheqacehg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gewvndsvo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/guwyzzqtv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gtgsxsipy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.tarul.cn/Article/details/gftewnhtr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.epnwcf.com/Article/details/gvawpwdeu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gxbmprred.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gjepimdpv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gqqvkvnze.sHtML

[D06] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/gbsnqpxvl.sHtML

Py:   len(arr)
来源：http://m.share.yfazqb.com/Article/details/gswwwfjwv.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/gnxxsifgo.sHtML

JS:   arr.length
来源：http://3g.epnwcf.com/Article/details/gvhjkatnl.sHtML

TS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gdapghpaj.sHtML

Java: list.size();
来源：http://baike.vehdjk.com/Article/details/ggdzzyses.sHtML

Go:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/gxkllzsuf.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.bbcook.cn/Article/details/gphuwvroh.sHtML

C#:   list.Count;
来源：http://baike.tarul.cn/Article/details/ggbsstljh.sHtML

[D07] 切片 / 取子数组
来源：http://3g.tarul.cn/Article/details/gvsdvyken.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.bbcook.cn/Article/details/gjqfeuulb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.tarul.cn/Article/details/gckfmozwp.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.epnwcf.com/Article/details/gidnqciyv.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/ggxpjhqos.sHtML

Java: list.subList(1, 4);
来源：http://3g.epnwcf.com/Article/details/girqutwsv.sHtML

Go:   arr[1:4]
来源：http://baike.epnwcf.com/Article/details/geoezvsua.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.yfazqb.com/Article/details/gltwiusfk.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.tarul.cn/Article/details/giomstsij.sHtML

[D08] 合并两个数组
来源：http://wap.tarul.cn/Article/details/gqnjhrboz.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.tarul.cn/Article/details/geoztaire.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.vehdjk.com/Article/details/gnjcgetuv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.yfazqb.com/Article/details/gawboynrr.sHtML

TS:   [...a, ...b];
来源：http://baike.bbcook.cn/Article/details/ggvevlerr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.tarul.cn/Article/details/glnkkokzb.sHtML

Go:   append(a, b...)
来源：http://www.share.tarul.cn/Article/details/grvzpmoaa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gzkvfarza.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gmfedhmdp.sHtML

[D09] 排序（升序）
来源：http://read.share.fktsv.cn/Article/details/gdqcjdgmg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gudtpbmge.sHtML

PHP:  sort($arr);
来源：http://wap.yfazqb.com/Article/details/gbatslebu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/gohklxugv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.bbcook.cn/Article/details/gpqdknmwy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.bbcook.cn/Article/details/gbbwlwtea.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/ganamstsa.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/gskuhyard.sHtML

C#:   list.Sort();
来源：http://mobile.vehdjk.com/Article/details/goengesmd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.epnwcf.com/Article/details/gnfyslppl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fktsv.cn/Article/details/grancnvrd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/gibnaigzy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.vehdjk.com/Article/details/gapwghikw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gjmjyhvti.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.vehdjk.com/Article/details/gtiurtaje.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.vehdjk.com/Article/details/gyiklqpum.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.epnwcf.com/Article/details/gdqyytqdp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.vehdjk.com/Article/details/gjmiggyrx.sHtML

[D11] 反转数组
来源：http://mobile.tarul.cn/Article/details/guoydfftn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fktsv.cn/Article/details/gvaaeyceo.sHtML

PHP:  array_reverse($arr);
来源：http://3g.vehdjk.com/Article/details/gkdkmicjg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.bbcook.cn/Article/details/grrhxajsj.sHtML

TS:   [...arr].reverse();
来源：http://baike.vehdjk.com/Article/details/gdgytyiqs.sHtML

Java: Collections.reverse(list);
来源：http://www.share.bbcook.cn/Article/details/grjjusnkl.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.yfazqb.com/Article/details/ggeqdwjmw.sHtML

Ruby: arr.reverse
来源：http://read.share.epnwcf.com/Article/details/gyvldibdf.sHtML

C#:   list.Reverse();
来源：http://baike.sjlbkw.cn/Article/details/gbehzjagr.sHtML

[D12] 查找元素下标
来源：http://blog.yfazqb.com/Article/details/goyswvgbm.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.tarul.cn/Article/details/gwtabhnty.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.yfazqb.com/Article/details/gbffcqrva.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/gqnjousnv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.vehdjk.com/Article/details/gufthfeqy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.epnwcf.com/Article/details/gkydwlowb.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.tarul.cn/Article/details/gllyiijwn.sHtML

Ruby: arr.index(x)
来源：http://wap.yfazqb.com/Article/details/gtkmohjyl.sHtML

C#:   list.IndexOf(x);
来源：http://3g.sjlbkw.cn/Article/details/gvskcenip.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.vehdjk.com/Article/details/gtylzrzaq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.bbcook.cn/Article/details/gpkhmklei.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.epnwcf.com/Article/details/galeljfvn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/ghhqhigce.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.bbcook.cn/Article/details/gcqxcjhqq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/gigovuebr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.epnwcf.com/Article/details/grjcmhvnz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.tarul.cn/Article/details/gxltzmaqg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.bbcook.cn/Article/details/gpaiznahw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fktsv.cn/Article/details/goqlvktzq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.epnwcf.com/Article/details/gbliacdup.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.epnwcf.com/Article/details/gvlegqxow.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.yfazqb.com/Article/details/gypoewfne.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.epnwcf.com/Article/details/gthmseejp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.bbcook.cn/Article/details/gtpplwigs.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/grqpccdia.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.tarul.cn/Article/details/gcuzjkinh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.epnwcf.com/Article/details/gbvytvllu.sHtML

[D15] 去重
来源：http://blog.sjlbkw.cn/Article/details/glpflmouh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gsphykoqv.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/gozmbnuaw.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/grilghqck.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/gfhbsvtfs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.vehdjk.com/Article/details/gjvlsxeso.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.bbcook.cn/Article/details/glizscolc.sHtML

Ruby: arr.uniq
来源：http://www.blog.vehdjk.com/Article/details/gqjvlqbzm.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.tarul.cn/Article/details/gbkuqlsxg.sHtML

[D16] 求和与平均值
来源：http://m.share.tarul.cn/Article/details/gzgztdcwq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fktsv.cn/Article/details/gdbdlqerz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.yfazqb.com/Article/details/gkiwrnwui.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/grrwoeboo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.tarul.cn/Article/details/gogqchejp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.vehdjk.com/Article/details/gsifgpulu.sHtML

Go:   // 手写循环累加
来源：http://blog.sjlbkw.cn/Article/details/garjheexz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.vehdjk.com/Article/details/gnvyrnwii.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fktsv.cn/Article/details/grqzkwadr.sHtML

[D17] 最大值与最小值
来源：http://3g.sjlbkw.cn/Article/details/gytrczwse.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/glngkgmyb.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.vehdjk.com/Article/details/gpclptlxm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fktsv.cn/Article/details/guctsgbzg.sHtML

TS:   Math.max(...arr);
来源：http://read.share.bbcook.cn/Article/details/gqotqncvc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.bbcook.cn/Article/details/gnfkubjjm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.tarul.cn/Article/details/gcbyoltpv.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.tarul.cn/Article/details/gooeglyfe.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.yfazqb.com/Article/details/groybfoff.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.tarul.cn/Article/details/gcfwjkskl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/gbcmebiig.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.yfazqb.com/Article/details/gvyojieal.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.vehdjk.com/Article/details/gmvoutrmb.sHtML

TS:   nested.flat();
来源：http://www.share.fktsv.cn/Article/details/gnqjadmhn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.epnwcf.com/Article/details/gajfsxsrh.sHtML

Go:   // 手写双层循环
来源：http://baike.sjlbkw.cn/Article/details/gtcdiptit.sHtML

Ruby: nested.flatten
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvxrcmyf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.tarul.cn/Article/details/gxjikzwqx.sHtML

[D19] 按字段分组
来源：http://m.share.tarul.cn/Article/details/gbbpbbaob.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.bbcook.cn/Article/details/glxqheupc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.yfazqb.com/Article/details/gombewkso.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.bbcook.cn/Article/details/gofmkgqwr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.sjlbkw.cn/Article/details/glgqoremu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.yfazqb.com/Article/details/gsscpexbo.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fktsv.cn/Article/details/gilpkkxgb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.vehdjk.com/Article/details/gzsuzusih.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.vehdjk.com/Article/details/gukubeofc.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.sjlbkw.cn/Article/details/gaecvptgg.sHtML

Py:   Counter(arr)
来源：http://wap.epnwcf.com/Article/details/gffcshbbl.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.bbcook.cn/Article/details/gxjavbyzh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gymgxvgqi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fktsv.cn/Article/details/gshjhwpnp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.yfazqb.com/Article/details/gsbrfnqpq.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fktsv.cn/Article/details/gcfelbgfu.sHtML


<!-- 参考信息 -->