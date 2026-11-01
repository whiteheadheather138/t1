代发 wailian999

Java: if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/gavclwanu.sHtML

Go:   if data == nil { return }
来源：http://read.share.vehdjk.com/Article/details/gahtxaecb.sHtML

Ruby: return if data.nil?
来源：http://m.share.bbcook.cn/Article/details/gsilotoqe.sHtML

C#:   if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gdrvdamen.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gqgfjcgob.sHtML

C. 函数与作用域
来源：http://blog.tarul.cn/Article/details/girxkrdio.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gnhymqdso.sHtML

[C01] 定义函数
来源：http://www.m.share.tarul.cn/Article/details/gtfqxdsdj.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fktsv.cn/Article/details/gszcfnzrz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/givgiyxxx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/glydwrskb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.tarul.cn/Article/details/grcqhczew.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gnwpjbwrb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gsukgrsae.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.epnwcf.com/Article/details/gibtjaksp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gmgclebyh.sHtML

[C02] 默认参数
来源：http://wap.vehdjk.com/Article/details/gjlmqhugp.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.vehdjk.com/Article/details/gqzhpghns.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.vehdjk.com/Article/details/gkwqikkrf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/guitwoaoc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/gkamlckhj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.tarul.cn/Article/details/gbxjhjykv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.tarul.cn/Article/details/gqysfpvpr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.vehdjk.com/Article/details/gsotzszih.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.sjlbkw.cn/Article/details/gmixnzkez.sHtML

[C03] 可变参数
来源：http://baike.fktsv.cn/Article/details/gmwrdveis.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.sjlbkw.cn/Article/details/gnqjcdrji.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.vehdjk.com/Article/details/gtlcswwpu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.vehdjk.com/Article/details/gjxlcqyuw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/govhzdxrl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.sjlbkw.cn/Article/details/gahxbkhdj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.sjlbkw.cn/Article/details/gmgqbytli.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fktsv.cn/Article/details/gtpbzipli.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fktsv.cn/Article/details/grbhbqazt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.tarul.cn/Article/details/grfpbyrsi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.tarul.cn/Article/details/gyldwqgls.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.bbcook.cn/Article/details/gdbbqgwjv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.bbcook.cn/Article/details/gctilllrs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.vehdjk.com/Article/details/gyazdztsz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.epnwcf.com/Article/details/gwovagzup.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.sjlbkw.cn/Article/details/gonfirqpk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gtafzzpwo.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/gbsxldohz.sHtML

[C05] 返回多个值
来源：http://www.blog.fktsv.cn/Article/details/gtxrsauqt.sHtML

Py:   return a, b
来源：http://baike.sjlbkw.cn/Article/details/guzzcsjhj.sHtML

PHP:  return [$a, $b];
来源：http://wap.epnwcf.com/Article/details/gehzqmqgu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.yfazqb.com/Article/details/gdrwdhsto.sHtML

TS:   return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gtbwgiojh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.yfazqb.com/Article/details/gavhythmz.sHtML

Go:   return a, b
来源：http://3g.bbcook.cn/Article/details/gumuaescf.sHtML

Ruby: return a, b
来源：http://mobile.tarul.cn/Article/details/gexukezbs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.tarul.cn/Article/details/gmqhkyauy.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.sjlbkw.cn/Article/details/girnbyykl.sHtML

Py:   square = lambda x: x * x
来源：http://3g.vehdjk.com/Article/details/gibveguqv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fktsv.cn/Article/details/gfkvydqpx.sHtML

JS:   const square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gzbvqjued.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.yfazqb.com/Article/details/gtegumwah.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.tarul.cn/Article/details/grvtsktll.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.sjlbkw.cn/Article/details/gephxlgbl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fktsv.cn/Article/details/grzxecfwb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/gfbfusbva.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.epnwcf.com/Article/details/ghduihqjo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.epnwcf.com/Article/details/gchivcquj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.yfazqb.com/Article/details/gmhfpmzhf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fktsv.cn/Article/details/ghqhhtvwo.sHtML

TS:   arr.map(String)
来源：http://blog.yfazqb.com/Article/details/gjjmdihcm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.vehdjk.com/Article/details/gcsswmmop.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.epnwcf.com/Article/details/gmsfyqrml.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.epnwcf.com/Article/details/gizncwylo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.tarul.cn/Article/details/gynvpxntc.sHtML

[C08] 闭包
来源：http://www.share.tarul.cn/Article/details/goqlniafn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.vehdjk.com/Article/details/gbnworphq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.epnwcf.com/Article/details/gguajcdbd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gskbeqvbd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/ggikdyioq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.bbcook.cn/Article/details/gkglubxpc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fktsv.cn/Article/details/gwahqjazp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.sjlbkw.cn/Article/details/gcmzqjynp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/guyjzubvl.sHtML

[C09] 递归
来源：http://mobile.tarul.cn/Article/details/gedfvpzpx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gpmsjjtjk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.tarul.cn/Article/details/gmkmnlyab.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/gfivsiwsj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gevgnqpua.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.tarul.cn/Article/details/gyzvluqoo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.yfazqb.com/Article/details/goptzxziz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fktsv.cn/Article/details/ggyafyesw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.sjlbkw.cn/Article/details/godyckbxc.sHtML

[C10] 变量作用域
来源：http://mobile.fktsv.cn/Article/details/gnthwnlcc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.bbcook.cn/Article/details/gptctohcy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.bbcook.cn/Article/details/givtggsim.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fktsv.cn/Article/details/gslgqrpqn.sHtML

TS:   同 JS
来源：http://baike.tarul.cn/Article/details/gpmewqwaq.sHtML

Java: 方法内为块级作用域
来源：http://read.share.vehdjk.com/Article/details/gopkxvout.sHtML

Go:   花括号块级作用域
来源：http://blog.vehdjk.com/Article/details/gpkuxhtcj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.tarul.cn/Article/details/gwhewkvid.sHtML

C#:   块级作用域
来源：http://read.share.bbcook.cn/Article/details/gaaljovwb.sHtML

[C11] 模块导入与导出
来源：http://wap.fktsv.cn/Article/details/gwyzdtnmg.sHtML

Py:   from module import func
来源：http://www.m.share.tarul.cn/Article/details/guvaaqckg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fktsv.cn/Article/details/ggxfjeoip.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.epnwcf.com/Article/details/gsozuslgi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.bbcook.cn/Article/details/gxddnaxlg.sHtML

Java: import java.util.List;
来源：http://mobile.bbcook.cn/Article/details/gnwkospew.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.bbcook.cn/Article/details/gfvrobtud.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.bbcook.cn/Article/details/gocwzkkkh.sHtML

C#:   using System.Text;
来源：http://www.share.vehdjk.com/Article/details/gafsnuexq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.tarul.cn/Article/details/gzrthhbrw.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.bbcook.cn/Article/details/ghuqhqezc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.yfazqb.com/Article/details/gnboktarz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.sjlbkw.cn/Article/details/gwkkbagmg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/gdzkyfdjy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.epnwcf.com/Article/details/gkjogaign.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.sjlbkw.cn/Article/details/gcyopessn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.yfazqb.com/Article/details/garrqyhwk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.tarul.cn/Article/details/gzywszgtn.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.tarul.cn/Article/details/ggrtkrxkb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.yfazqb.com/Article/details/gtbqspllq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/goofjudor.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.vehdjk.com/Article/details/gmdjujhto.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gnauixmbs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gmuhxfisl.sHtML

Go:   func add(a, b int) int
来源：http://www.share.vehdjk.com/Article/details/grnfnqkdj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.vehdjk.com/Article/details/gsetxikjk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.bbcook.cn/Article/details/gcwonexrh.sHtML

[C14] 泛型函数
来源：http://www.m.share.vehdjk.com/Article/details/gcpvekdab.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.yfazqb.com/Article/details/gepeyjpqn.sHtML

PHP:  // 无泛型
来源：http://baike.bbcook.cn/Article/details/gpiouzeoo.sHtML

JS:   // 无泛型
来源：http://mobile.yfazqb.com/Article/details/ghbuhslgv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fktsv.cn/Article/details/gkjrqopdx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fktsv.cn/Article/details/gxjdgkosq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.tarul.cn/Article/details/ggyhakbaf.sHtML

Ruby: # 无泛型
来源：http://m.share.vehdjk.com/Article/details/gwxxnmwai.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.sjlbkw.cn/Article/details/gfkuxnxgd.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.sjlbkw.cn/Article/details/gmqwnveak.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.sjlbkw.cn/Article/details/gfpodqbzg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.tarul.cn/Article/details/gnqnygqzl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/gqceixhhw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fktsv.cn/Article/details/givhspiyv.sHtML

Java: // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/grkxnsiek.sHtML

Go:   // 无解构
来源：http://www.m.share.bbcook.cn/Article/details/gprstfysn.sHtML

Ruby: a, b = pair
来源：http://blog.tarul.cn/Article/details/gqgsulkbd.sHtML

C#:   var (a, b) = pair;
来源：http://3g.epnwcf.com/Article/details/gvxpkeclf.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.bbcook.cn/Article/details/gxiwvvpih.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.yfazqb.com/Article/details/gixlfmpae.sHtML

PHP:  // 无重载
来源：http://read.share.sjlbkw.cn/Article/details/gjwcossaj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.sjlbkw.cn/Article/details/gdxfhklmy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.tarul.cn/Article/details/gfbfflgyb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.vehdjk.com/Article/details/ghepnbuqu.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.tarul.cn/Article/details/gtcfqxdew.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.epnwcf.com/Article/details/gyktzziiu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.yfazqb.com/Article/details/gqoplzkrr.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/goykzcmrp.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.vehdjk.com/Article/details/gzxxixcyd.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gqiewgngt.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gwvfcgvwy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.bbcook.cn/Article/details/ggdbxqtny.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fktsv.cn/Article/details/gmjfqrawu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.tarul.cn/Article/details/gnlhidxkp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.tarul.cn/Article/details/gkjuoztxj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.tarul.cn/Article/details/gvnjyuiky.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.yfazqb.com/Article/details/gfzsyotff.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.vehdjk.com/Article/details/gqjyhxxhx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.vehdjk.com/Article/details/gdmcdhqpu.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.sjlbkw.cn/Article/details/ghovtkotw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.epnwcf.com/Article/details/gioukcglb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.vehdjk.com/Article/details/gmuvsyaon.sHtML

JS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/grgzwhvij.sHtML

TS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/guhyugicc.sHtML

Java: list.add(4);
来源：http://baike.sjlbkw.cn/Article/details/ghrwjygrf.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.epnwcf.com/Article/details/gwrkgxpqz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.tarul.cn/Article/details/gtkrapmot.sHtML

C#:   list.Add(4);
来源：http://read.share.vehdjk.com/Article/details/gvxqpparz.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.sjlbkw.cn/Article/details/gcnvhwiye.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.tarul.cn/Article/details/geramzmrl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.sjlbkw.cn/Article/details/giduxvwgx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.sjlbkw.cn/Article/details/gauottjih.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fktsv.cn/Article/details/gvsbrmxuo.sHtML

Java: list.add(0, 0);
来源：http://wap.sjlbkw.cn/Article/details/gwzvylofi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.sjlbkw.cn/Article/details/ghrmjdyem.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.tarul.cn/Article/details/gymyeknbc.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.yfazqb.com/Article/details/grutnftzu.sHtML

[D04] 删除元素
来源：http://read.share.fktsv.cn/Article/details/gxyngdkpb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.tarul.cn/Article/details/gnglumvug.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.bbcook.cn/Article/details/gvmuofsvq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.epnwcf.com/Article/details/gcjsxwpdr.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.bbcook.cn/Article/details/gwqmgtqbw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.vehdjk.com/Article/details/glqjhosgn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.yfazqb.com/Article/details/gbpldvtmq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fktsv.cn/Article/details/gqlbdjkdk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.vehdjk.com/Article/details/gjrrcsykv.sHtML

[D05] 访问与修改元素
来源：http://mobile.bbcook.cn/Article/details/gjotfzhjd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gpbyciqll.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gjgpravmh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gcmhymlkz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.yfazqb.com/Article/details/gafajtmwv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.epnwcf.com/Article/details/giivyiofk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gesbvemve.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gqocduhqn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gqfwzbgou.sHtML

[D06] 数组长度
来源：http://mobile.tarul.cn/Article/details/gbyunhopj.sHtML

Py:   len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gyfuqlict.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/gdzzupena.sHtML

JS:   arr.length
来源：http://m.share.fktsv.cn/Article/details/gnwhnqrdk.sHtML

TS:   arr.length
来源：http://wap.fktsv.cn/Article/details/gtqdmpypy.sHtML

Java: list.size();
来源：http://3g.yfazqb.com/Article/details/gduxthetm.sHtML

Go:   len(arr)
来源：http://wap.tarul.cn/Article/details/ghdurkffg.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.bbcook.cn/Article/details/gotndcwpr.sHtML

C#:   list.Count;
来源：http://blog.yfazqb.com/Article/details/gwmsoimmk.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.tarul.cn/Article/details/gfxzoykgj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.vehdjk.com/Article/details/gzhccnftq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.yfazqb.com/Article/details/ggefjksgn.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gednysmhj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbjlntoo.sHtML

Java: list.subList(1, 4);
来源：http://m.share.bbcook.cn/Article/details/giycqubcp.sHtML

Go:   arr[1:4]
来源：http://mobile.sjlbkw.cn/Article/details/geudtassu.sHtML

Ruby: arr[1, 3]
来源：http://www.share.yfazqb.com/Article/details/gasbfhcnh.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.vehdjk.com/Article/details/gxjdyfzjk.sHtML

[D08] 合并两个数组
来源：http://www.share.yfazqb.com/Article/details/gyqcguqut.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.vehdjk.com/Article/details/gpckvkjlw.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.tarul.cn/Article/details/gspoenxqw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fktsv.cn/Article/details/gsedaxcmz.sHtML

TS:   [...a, ...b];
来源：http://m.share.sjlbkw.cn/Article/details/gpqfepdjq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.yfazqb.com/Article/details/guzilzhdd.sHtML

Go:   append(a, b...)
来源：http://www.m.share.bbcook.cn/Article/details/gfvhqjhzx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.bbcook.cn/Article/details/gpjgawmhn.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.vehdjk.com/Article/details/ghegwnipa.sHtML

[D09] 排序（升序）
来源：http://www.m.share.vehdjk.com/Article/details/gmpklkqzd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/gmnqsgdal.sHtML

PHP:  sort($arr);
来源：http://baike.epnwcf.com/Article/details/glqhxcnwe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fktsv.cn/Article/details/gfymukzgh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.epnwcf.com/Article/details/gvuekjygf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.vehdjk.com/Article/details/gnvqfqhbf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gougpdcnm.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gtaclxhvz.sHtML

C#:   list.Sort();
来源：http://wap.bbcook.cn/Article/details/gikqpoqwc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fktsv.cn/Article/details/gaycddnpn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.bbcook.cn/Article/details/glsefpfrn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.epnwcf.com/Article/details/gmdlainrx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/gptuzewid.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.vehdjk.com/Article/details/gnypvjjll.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.epnwcf.com/Article/details/gooowelyq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.bbcook.cn/Article/details/gqnrgeerz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.vehdjk.com/Article/details/gmvxjrgfb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.yfazqb.com/Article/details/gelhsgvub.sHtML

[D11] 反转数组
来源：http://m.share.fktsv.cn/Article/details/globutrnt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.bbcook.cn/Article/details/gothczmhk.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fktsv.cn/Article/details/gjtxjuluz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fktsv.cn/Article/details/gagagtynx.sHtML

TS:   [...arr].reverse();
来源：http://m.share.epnwcf.com/Article/details/gusevcmcg.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.tarul.cn/Article/details/gpujqsmna.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fktsv.cn/Article/details/gdwbumnbh.sHtML

Ruby: arr.reverse
来源：http://www.share.yfazqb.com/Article/details/gvbecpofv.sHtML

C#:   list.Reverse();
来源：http://wap.sjlbkw.cn/Article/details/godccxzbf.sHtML

[D12] 查找元素下标
来源：http://m.share.fktsv.cn/Article/details/gndqsjinm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/ghkrjyvkv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.yfazqb.com/Article/details/gwpnczspy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/giygmkxxf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gxllzfmya.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.tarul.cn/Article/details/grtmrofoi.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.vehdjk.com/Article/details/glqyoejdk.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.bbcook.cn/Article/details/grerfswwt.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fktsv.cn/Article/details/gcegtqfmp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.tarul.cn/Article/details/ggemxlcof.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.yfazqb.com/Article/details/gjowtmogh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.tarul.cn/Article/details/giyrlabse.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gqmtjsoyh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gtnynoxwf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.sjlbkw.cn/Article/details/gkoblnvei.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.epnwcf.com/Article/details/gogutnvdc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.yfazqb.com/Article/details/gmssyktpa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fktsv.cn/Article/details/gchsdwulj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fktsv.cn/Article/details/guywnauvb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.epnwcf.com/Article/details/gmvlzceik.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gznwnmkpy.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.sjlbkw.cn/Article/details/ggjvoudxa.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gwiftsvde.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fktsv.cn/Article/details/gyimqqhtj.sHtML

Go:   // 手写循环
来源：http://mobile.yfazqb.com/Article/details/guevgaqnc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gvkajcjwj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.yfazqb.com/Article/details/gnherxwsm.sHtML

[D15] 去重
来源：http://baike.yfazqb.com/Article/details/gyrdnqsfx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/ghxwfxdai.sHtML

PHP:  array_unique($arr);
来源：http://baike.tarul.cn/Article/details/glrdjxxtj.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/gpqqtlrgp.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/ghbmkztfp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fktsv.cn/Article/details/gdvalymmh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.yfazqb.com/Article/details/gsrkilmxb.sHtML

Ruby: arr.uniq
来源：http://www.share.sjlbkw.cn/Article/details/gpumcytsm.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fktsv.cn/Article/details/gicvfunez.sHtML

[D16] 求和与平均值
来源：http://baike.fktsv.cn/Article/details/gayizxjii.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fktsv.cn/Article/details/guleuevqb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.vehdjk.com/Article/details/gzpofsztp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gtxiwdhnw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/giiapihrs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.bbcook.cn/Article/details/gcexsuaat.sHtML

Go:   // 手写循环累加
来源：http://baike.sjlbkw.cn/Article/details/gewxyqyjb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.epnwcf.com/Article/details/glxvsdvxy.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.bbcook.cn/Article/details/gmoawlhgc.sHtML

[D17] 最大值与最小值
来源：http://wap.fktsv.cn/Article/details/gbhaxsqtk.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.yfazqb.com/Article/details/glginvzfm.sHtML


<!-- 参考信息 -->