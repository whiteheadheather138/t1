代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.vehdjk.com/Article/details/ghewnlslc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gfrfrawcl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.yfazqb.com/Article/details/gszgohlog.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fktsv.cn/Article/details/gfwrdwryz.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fktsv.cn/Article/details/gwdmaszeo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gvgqcxkbc.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fktsv.cn/Article/details/gxcyeatlk.sHtML

[C05] 返回多个值
来源：http://baike.vehdjk.com/Article/details/ghzbvqlsk.sHtML

Py:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gqjzdczpk.sHtML

PHP:  return [$a, $b];
来源：http://wap.bbcook.cn/Article/details/gkzrqtmpq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gimcxnhri.sHtML

TS:   return { a, b };
来源：http://wap.fktsv.cn/Article/details/gfhoonbqg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fktsv.cn/Article/details/ghttibxlu.sHtML

Go:   return a, b
来源：http://mobile.yfazqb.com/Article/details/gthiubxph.sHtML

Ruby: return a, b
来源：http://m.share.vehdjk.com/Article/details/gfrceshiy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fktsv.cn/Article/details/gngxerwvm.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fktsv.cn/Article/details/gurtvpfyv.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.tarul.cn/Article/details/gmorkxeju.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.bbcook.cn/Article/details/gkevsjwao.sHtML

JS:   const square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/gekiekwic.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.epnwcf.com/Article/details/gxcdffmdy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gxeqjsqgn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.bbcook.cn/Article/details/gmvxxoqyt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.bbcook.cn/Article/details/gzwvwfrce.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/gajanouqm.sHtML

[C07] 把函数作为参数传入
来源：http://3g.epnwcf.com/Article/details/gnizghxun.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.yfazqb.com/Article/details/gafhbgqzs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.tarul.cn/Article/details/gocwyskin.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.vehdjk.com/Article/details/gdwhtqsxc.sHtML

TS:   arr.map(String)
来源：http://blog.epnwcf.com/Article/details/gjkxbsnta.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.epnwcf.com/Article/details/gqhwxpizj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.tarul.cn/Article/details/grmrmnfra.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.sjlbkw.cn/Article/details/gnvlxwehd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fktsv.cn/Article/details/gbstwlbad.sHtML

[C08] 闭包
来源：http://www.blog.fktsv.cn/Article/details/gyhdgsshz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.yfazqb.com/Article/details/gqncgqkzj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.yfazqb.com/Article/details/glglmeetr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/govphyyda.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gujatqeaf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.sjlbkw.cn/Article/details/gpvyjuxqy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.sjlbkw.cn/Article/details/gznzybhsv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.bbcook.cn/Article/details/ghmbjsrqd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gwjoghksw.sHtML

[C09] 递归
来源：http://www.m.share.fktsv.cn/Article/details/goqunmytd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gjqxynauk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.epnwcf.com/Article/details/gdxwkdgbm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/ghgdckptf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.yfazqb.com/Article/details/gklwpyibf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.tarul.cn/Article/details/gptjbocug.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/ggsmtpjul.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gyelhqmkd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.sjlbkw.cn/Article/details/givjxffel.sHtML

[C10] 变量作用域
来源：http://blog.epnwcf.com/Article/details/greoibwrr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fktsv.cn/Article/details/gndvkohjc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.vehdjk.com/Article/details/gvtdthkth.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.yfazqb.com/Article/details/grrabwneh.sHtML

TS:   同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gfcltsrks.sHtML

Java: 方法内为块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gnnvpkrsq.sHtML

Go:   花括号块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gpjfeebjf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.vehdjk.com/Article/details/gpkmcodkn.sHtML

C#:   块级作用域
来源：http://mobile.tarul.cn/Article/details/gwnbgodgz.sHtML

[C11] 模块导入与导出
来源：http://read.share.sjlbkw.cn/Article/details/gwnphtsvx.sHtML

Py:   from module import func
来源：http://www.m.share.yfazqb.com/Article/details/gitcidcbv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.epnwcf.com/Article/details/gosjdlkov.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fktsv.cn/Article/details/gpfvqciuq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.bbcook.cn/Article/details/gddjphiau.sHtML

Java: import java.util.List;
来源：http://www.m.share.vehdjk.com/Article/details/gxyesqurl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.epnwcf.com/Article/details/gcyyvucuq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.epnwcf.com/Article/details/grqaqohcm.sHtML

C#:   using System.Text;
来源：http://m.share.tarul.cn/Article/details/gjqbdimpy.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.epnwcf.com/Article/details/gvoofmdfe.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.bbcook.cn/Article/details/gmbdpzpkk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.vehdjk.com/Article/details/gusckhjul.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fktsv.cn/Article/details/gmhxpayok.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/gaedblrmn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.bbcook.cn/Article/details/gdrjdzciw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/gutkkyhyt.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.yfazqb.com/Article/details/gdihpehpj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.yfazqb.com/Article/details/guifbamcr.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.yfazqb.com/Article/details/gnwobjzqk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.yfazqb.com/Article/details/gbwoxenhw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gfmwfdcpg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.vehdjk.com/Article/details/gvbvlohxt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gikqkpbiw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gkefukhaa.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/gwghicgwr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.tarul.cn/Article/details/gehbklecg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fktsv.cn/Article/details/gvwjsvaqc.sHtML

[C14] 泛型函数
来源：http://3g.sjlbkw.cn/Article/details/gkpzkltfw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.bbcook.cn/Article/details/geruipqrn.sHtML

PHP:  // 无泛型
来源：http://blog.yfazqb.com/Article/details/gbimzyhst.sHtML

JS:   // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gqdskghnc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.bbcook.cn/Article/details/gxppwxmbz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.bbcook.cn/Article/details/gcbssslya.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.bbcook.cn/Article/details/gelbisgny.sHtML

Ruby: # 无泛型
来源：http://baike.vehdjk.com/Article/details/gjnrpkdzt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.yfazqb.com/Article/details/ghzbnvkuo.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.tarul.cn/Article/details/geaxcsxdl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.yfazqb.com/Article/details/gtywadipv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.vehdjk.com/Article/details/gvzqyycng.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/ggrctpqpi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fktsv.cn/Article/details/gzofbeexr.sHtML

Java: // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/gceaqljuc.sHtML

Go:   // 无解构
来源：http://www.m.share.tarul.cn/Article/details/gurokqbii.sHtML

Ruby: a, b = pair
来源：http://m.share.epnwcf.com/Article/details/ggpdopxsk.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.epnwcf.com/Article/details/gtrnhtzzp.sHtML

[C16] 函数 / 方法重载
来源：http://3g.epnwcf.com/Article/details/glexaybcq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.vehdjk.com/Article/details/gxowalmbu.sHtML

PHP:  // 无重载
来源：http://www.blog.fktsv.cn/Article/details/guhphznyi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.yfazqb.com/Article/details/govvahltn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.tarul.cn/Article/details/gehzvyydd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.sjlbkw.cn/Article/details/givahqrxr.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.sjlbkw.cn/Article/details/gfxhrihnn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.sjlbkw.cn/Article/details/gbznxcuup.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fktsv.cn/Article/details/gskkvrgrv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gxxfynupb.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.epnwcf.com/Article/details/glhoddluf.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzfboruww.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gzsadaote.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.bbcook.cn/Article/details/gekyovyvq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.bbcook.cn/Article/details/gmfcgxeya.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.vehdjk.com/Article/details/gebozjcye.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.bbcook.cn/Article/details/grdadqkey.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fktsv.cn/Article/details/giooywkkp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.sjlbkw.cn/Article/details/gngyfxrns.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.vehdjk.com/Article/details/gfgymcsmm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.vehdjk.com/Article/details/gujyovijm.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fktsv.cn/Article/details/gnzlzvian.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.sjlbkw.cn/Article/details/gtogfbyha.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcgxnfwl.sHtML

JS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gevjuiwed.sHtML

TS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/gmqqkyipj.sHtML

Java: list.add(4);
来源：http://baike.sjlbkw.cn/Article/details/giawasmeu.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fktsv.cn/Article/details/gtrvaqabb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.epnwcf.com/Article/details/gssdtgvgk.sHtML

C#:   list.Add(4);
来源：http://3g.vehdjk.com/Article/details/girmkvici.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.sjlbkw.cn/Article/details/gcsktavux.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.tarul.cn/Article/details/gmbzranwk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.sjlbkw.cn/Article/details/gomnvvtsh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.vehdjk.com/Article/details/gejbykmbn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gpphqelni.sHtML

Java: list.add(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gnnhtrpjm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.epnwcf.com/Article/details/gsdxtxvps.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.yfazqb.com/Article/details/ghmvlgykd.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.epnwcf.com/Article/details/gsjdawmpp.sHtML

[D04] 删除元素
来源：http://wap.epnwcf.com/Article/details/gyidixihm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.vehdjk.com/Article/details/gttqxdjog.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.epnwcf.com/Article/details/gxrynvjve.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.yfazqb.com/Article/details/gkfmsvaev.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.vehdjk.com/Article/details/gfrllnbbv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.epnwcf.com/Article/details/gchwriqcz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fktsv.cn/Article/details/geutqcizy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.tarul.cn/Article/details/gddrmhkzd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.epnwcf.com/Article/details/gupihgsus.sHtML

[D05] 访问与修改元素
来源：http://wap.epnwcf.com/Article/details/glenzaios.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gzvtzzwhh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fktsv.cn/Article/details/guifsrbwe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gmszvldcm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.yfazqb.com/Article/details/gmkfcxayu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fktsv.cn/Article/details/gtwqwrdtx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/geaqseewk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gwwiwcygr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/gxjrgegyr.sHtML

[D06] 数组长度
来源：http://www.blog.tarul.cn/Article/details/gsbexiepu.sHtML

Py:   len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfrqioiu.sHtML

PHP:  count($arr);
来源：http://3g.bbcook.cn/Article/details/gwblorejf.sHtML

JS:   arr.length
来源：http://wap.bbcook.cn/Article/details/gcsgikgme.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/gefahiebm.sHtML

Java: list.size();
来源：http://baike.sjlbkw.cn/Article/details/gdwftvmcg.sHtML

Go:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gmhvwhizm.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.epnwcf.com/Article/details/ghvfgejrc.sHtML

C#:   list.Count;
来源：http://www.m.share.fktsv.cn/Article/details/gudszdwuk.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.vehdjk.com/Article/details/gixxscpec.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.bbcook.cn/Article/details/gntjzejbp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gkwnxodnu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/gfjolrjeu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gbkvdnmqp.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gomuzqiog.sHtML

Go:   arr[1:4]
来源：http://baike.sjlbkw.cn/Article/details/gtkzvnovx.sHtML

Ruby: arr[1, 3]
来源：http://3g.vehdjk.com/Article/details/gxhwnszqy.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.vehdjk.com/Article/details/gfndhrybd.sHtML

[D08] 合并两个数组
来源：http://read.share.sjlbkw.cn/Article/details/gsntlggtb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fktsv.cn/Article/details/gsptalzto.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fktsv.cn/Article/details/gsfgiwuir.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.epnwcf.com/Article/details/gingndqmk.sHtML

TS:   [...a, ...b];
来源：http://www.blog.tarul.cn/Article/details/gfniqgire.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.epnwcf.com/Article/details/gwuishdro.sHtML

Go:   append(a, b...)
来源：http://wap.bbcook.cn/Article/details/gwhtquaec.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fktsv.cn/Article/details/gjfzdehzt.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.yfazqb.com/Article/details/gkobajtkn.sHtML

[D09] 排序（升序）
来源：http://3g.vehdjk.com/Article/details/gmcnlayby.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gfhsprera.sHtML

PHP:  sort($arr);
来源：http://3g.sjlbkw.cn/Article/details/gxohbrlqa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.yfazqb.com/Article/details/grbecaqik.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.tarul.cn/Article/details/gziejbmol.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.yfazqb.com/Article/details/ghwfgcyex.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gnknaibir.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gulydxajx.sHtML

C#:   list.Sort();
来源：http://m.share.sjlbkw.cn/Article/details/gimsynndm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.vehdjk.com/Article/details/geqvqhnoz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/grsssaoxa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.vehdjk.com/Article/details/gsqwydtuq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/gktnzvnas.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fktsv.cn/Article/details/gdvmsnmlu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.sjlbkw.cn/Article/details/griitkubp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.sjlbkw.cn/Article/details/gfbzzgzav.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fktsv.cn/Article/details/gbnrslrga.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.bbcook.cn/Article/details/giysopxim.sHtML

[D11] 反转数组
来源：http://www.m.share.epnwcf.com/Article/details/gwyocacxs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.epnwcf.com/Article/details/gatgrujns.sHtML

PHP:  array_reverse($arr);
来源：http://baike.yfazqb.com/Article/details/gslkclnyk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.sjlbkw.cn/Article/details/gknyyrjmm.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/gkuplzcvu.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhrvluoq.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.bbcook.cn/Article/details/godfpteoy.sHtML

Ruby: arr.reverse
来源：http://m.share.tarul.cn/Article/details/gnykgxwuo.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fktsv.cn/Article/details/ghnhsnlqb.sHtML

[D12] 查找元素下标
来源：http://m.share.yfazqb.com/Article/details/gmidecrvx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.yfazqb.com/Article/details/gzggnptyy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.epnwcf.com/Article/details/gwhjdoddw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fktsv.cn/Article/details/gpxjgwzdb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.tarul.cn/Article/details/gxuhrwxpc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fktsv.cn/Article/details/glabnobwa.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.tarul.cn/Article/details/gvltikuar.sHtML

Ruby: arr.index(x)
来源：http://wap.yfazqb.com/Article/details/gpnlbqysd.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fktsv.cn/Article/details/ggmrqsaoq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fktsv.cn/Article/details/glsuhipnw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gtnfycnyu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fktsv.cn/Article/details/gowpzxzkk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/guydqiwjk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gzdbzxyju.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmdpxjaz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.vehdjk.com/Article/details/gypvjatfh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.sjlbkw.cn/Article/details/gtgalxsti.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.sjlbkw.cn/Article/details/ggqmcoqyk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.vehdjk.com/Article/details/gqugunxxx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.epnwcf.com/Article/details/glrqjnukj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.tarul.cn/Article/details/gomacomcr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fktsv.cn/Article/details/ggbtmnoqp.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/ggstufjky.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.vehdjk.com/Article/details/grnbkaogv.sHtML

Go:   // 手写循环
来源：http://3g.sjlbkw.cn/Article/details/gzvmclpoj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.yfazqb.com/Article/details/genznkrdi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fktsv.cn/Article/details/gmgfjiilk.sHtML

[D15] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/gdejkigpi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/ggicbgakd.sHtML

PHP:  array_unique($arr);
来源：http://baike.fktsv.cn/Article/details/gbptkcwde.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/gzveciray.sHtML

TS:   [...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gchgudwwv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.vehdjk.com/Article/details/gttomxklw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fktsv.cn/Article/details/gbazmwcse.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/gbkmdddqt.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.sjlbkw.cn/Article/details/gxnpdvoxb.sHtML

[D16] 求和与平均值
来源：http://baike.yfazqb.com/Article/details/gpsgsmhfk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.epnwcf.com/Article/details/gydqpcfcs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.vehdjk.com/Article/details/gvtttkbww.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/gycjirrnm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gxvqpuzpk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.tarul.cn/Article/details/gkrzapgui.sHtML

Go:   // 手写循环累加
来源：http://blog.epnwcf.com/Article/details/gvzpnxttd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gczlakayy.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.bbcook.cn/Article/details/gnweiuewv.sHtML

[D17] 最大值与最小值
来源：http://read.share.sjlbkw.cn/Article/details/glezdpsfb.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.tarul.cn/Article/details/gsextvwbj.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.yfazqb.com/Article/details/gqpgldzdv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.tarul.cn/Article/details/gdxzmczwg.sHtML

TS:   Math.max(...arr);
来源：http://blog.fktsv.cn/Article/details/glczbzpll.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.sjlbkw.cn/Article/details/gcoganmlq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fktsv.cn/Article/details/gjxyzblyx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.sjlbkw.cn/Article/details/gihjgmxjp.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.sjlbkw.cn/Article/details/gdinvizuu.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.yfazqb.com/Article/details/glcuwmqez.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fktsv.cn/Article/details/gekeebhch.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/grhgoaqwx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.yfazqb.com/Article/details/gjtmcpfaw.sHtML

TS:   nested.flat();
来源：http://www.share.yfazqb.com/Article/details/ghmzskgsz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.epnwcf.com/Article/details/glwzbvuch.sHtML

Go:   // 手写双层循环
来源：http://mobile.bbcook.cn/Article/details/gpqlvqdoo.sHtML

Ruby: nested.flatten
来源：http://www.share.bbcook.cn/Article/details/gdzhusroo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gnstteaof.sHtML

[D19] 按字段分组
来源：http://blog.sjlbkw.cn/Article/details/geqikzqyb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.epnwcf.com/Article/details/gqiwvmsjv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.bbcook.cn/Article/details/gytzxmvwb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.yfazqb.com/Article/details/gnpbcmdlu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.sjlbkw.cn/Article/details/gtxvhbydh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.sjlbkw.cn/Article/details/gojyiwybe.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fktsv.cn/Article/details/gpeozpydh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.vehdjk.com/Article/details/gwgeiohgv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.tarul.cn/Article/details/ghwcxhldp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.epnwcf.com/Article/details/glddgvvez.sHtML

Py:   Counter(arr)
来源：http://wap.bbcook.cn/Article/details/gndtgyczh.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.vehdjk.com/Article/details/gkrecjmxo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/gyhjagmzn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gexxstbyu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.epnwcf.com/Article/details/gbzqrrfaw.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fktsv.cn/Article/details/gknjngsbu.sHtML

Ruby: arr.tally
来源：http://www.blog.tarul.cn/Article/details/gdfmeswkq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.epnwcf.com/Article/details/gouqlgkqa.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.bbcook.cn/Article/details/gvbwkcera.sHtML

Py:   x in arr
来源：http://mobile.sjlbkw.cn/Article/details/glxdckths.sHtML


<!-- 参考信息 -->