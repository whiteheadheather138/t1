代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/garbncbst.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.bbcook.cn/Article/details/gyyvlfxyd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.sjlbkw.cn/Article/details/gglqptfow.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.tarul.cn/Article/details/gnhjxkjxh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.sjlbkw.cn/Article/details/gmhpzikhe.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/giotzvrdr.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.epnwcf.com/Article/details/goubanxdw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.epnwcf.com/Article/details/gjqwtkvbh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/goluimnfs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/ghyflmmiu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.vehdjk.com/Article/details/gsgizxrcx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.bbcook.cn/Article/details/gnpweztvz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.epnwcf.com/Article/details/ghgoumqit.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.epnwcf.com/Article/details/gidlnrnic.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.sjlbkw.cn/Article/details/gfkodlknb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.epnwcf.com/Article/details/gpsvqqpsk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.bbcook.cn/Article/details/gnmvyfdvi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/gyryntldm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.tarul.cn/Article/details/gmxkulmlw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fktsv.cn/Article/details/gimtixacy.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.bbcook.cn/Article/details/gqsltjhcx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gdycsomjb.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gfhuvbqrj.sHtML

[C05] 返回多个值
来源：http://www.blog.sjlbkw.cn/Article/details/gpiciftch.sHtML

Py:   return a, b
来源：http://m.share.epnwcf.com/Article/details/gsdkfeifi.sHtML

PHP:  return [$a, $b];
来源：http://mobile.yfazqb.com/Article/details/greheutxv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.epnwcf.com/Article/details/gdrgywgew.sHtML

TS:   return { a, b };
来源：http://read.share.vehdjk.com/Article/details/gcuisbnft.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.bbcook.cn/Article/details/gxnyofhmv.sHtML

Go:   return a, b
来源：http://blog.yfazqb.com/Article/details/gdipgcbmz.sHtML

Ruby: return a, b
来源：http://www.blog.yfazqb.com/Article/details/gwlpcxylh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.epnwcf.com/Article/details/gfcmwqztt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fktsv.cn/Article/details/giqbziwcm.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.vehdjk.com/Article/details/gpiblkzci.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.epnwcf.com/Article/details/gvgcfosod.sHtML

JS:   const square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/gxnywobjx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.yfazqb.com/Article/details/gzloxuiov.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gcxqdqqfn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.vehdjk.com/Article/details/gdflcrtht.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fktsv.cn/Article/details/geafygpwy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.tarul.cn/Article/details/gbpsdxgdv.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.tarul.cn/Article/details/glvskntjl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.vehdjk.com/Article/details/gcvxkeakp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.bbcook.cn/Article/details/gtdkzgvgu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.yfazqb.com/Article/details/gayecaedj.sHtML

TS:   arr.map(String)
来源：http://read.share.tarul.cn/Article/details/grdaghplu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.epnwcf.com/Article/details/gxmnmwuwj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.tarul.cn/Article/details/govzcrmvp.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.epnwcf.com/Article/details/gcurgkvjt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.yfazqb.com/Article/details/gjlrpeuzg.sHtML

[C08] 闭包
来源：http://m.share.epnwcf.com/Article/details/gklfwzyht.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.tarul.cn/Article/details/gpbwmnneh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.sjlbkw.cn/Article/details/gszbfhsdb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtsasjal.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/groluadgq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.tarul.cn/Article/details/gzirijlwl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.bbcook.cn/Article/details/gpjpvlayz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.sjlbkw.cn/Article/details/gypchhenj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gsemfgene.sHtML

[C09] 递归
来源：http://www.blog.sjlbkw.cn/Article/details/gcjgriqls.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.vehdjk.com/Article/details/glygfteds.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/gqrumcoal.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/gxcjksywq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gdvpcgxln.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gktnvsefp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.yfazqb.com/Article/details/gvamszhqr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/gekftnaaf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fktsv.cn/Article/details/goyrpbmab.sHtML

[C10] 变量作用域
来源：http://www.share.fktsv.cn/Article/details/grxjsbpyu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fktsv.cn/Article/details/gzqjirtif.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.yfazqb.com/Article/details/gtdqicqgq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gslkadhag.sHtML

TS:   同 JS
来源：http://mobile.yfazqb.com/Article/details/gcytkdyoy.sHtML

Java: 方法内为块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gbjzioenv.sHtML

Go:   花括号块级作用域
来源：http://www.share.tarul.cn/Article/details/gdtnopfsi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.yfazqb.com/Article/details/gsyyxygag.sHtML

C#:   块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/ghhlejczl.sHtML

[C11] 模块导入与导出
来源：http://3g.sjlbkw.cn/Article/details/gqyexonxh.sHtML

Py:   from module import func
来源：http://m.share.fktsv.cn/Article/details/gsvqswmzd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.vehdjk.com/Article/details/gjthkzsdy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.tarul.cn/Article/details/gqlsbyhuf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.vehdjk.com/Article/details/gmhggyfce.sHtML

Java: import java.util.List;
来源：http://www.share.epnwcf.com/Article/details/gedgvxptn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.bbcook.cn/Article/details/gzfjzijfa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.tarul.cn/Article/details/gkfyvvmut.sHtML

C#:   using System.Text;
来源：http://www.blog.yfazqb.com/Article/details/gkadxkajk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.bbcook.cn/Article/details/gqzdetbgv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fktsv.cn/Article/details/gjykildpi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.bbcook.cn/Article/details/geasnwykr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/gvsjobjho.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gctobpgue.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.yfazqb.com/Article/details/gkuzfoxsd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.bbcook.cn/Article/details/gzvginarx.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.vehdjk.com/Article/details/gsetmbbms.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gonvkkggx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.bbcook.cn/Article/details/gmatinitw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.sjlbkw.cn/Article/details/gsmzkohrr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gnqcywadc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.epnwcf.com/Article/details/gxlmuqyxb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gwgpktagp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gyzvphzah.sHtML

Go:   func add(a, b int) int
来源：http://www.share.tarul.cn/Article/details/gpfoogfhc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.sjlbkw.cn/Article/details/gckuyhkne.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.epnwcf.com/Article/details/gqqglfgdq.sHtML

[C14] 泛型函数
来源：http://wap.epnwcf.com/Article/details/gvnxdsgpi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fktsv.cn/Article/details/gvcwsdcha.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gajiiurvk.sHtML

JS:   // 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gagjtwsbb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.epnwcf.com/Article/details/gpuepgzfg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.bbcook.cn/Article/details/guieirifj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.epnwcf.com/Article/details/gnaansrfw.sHtML

Ruby: # 无泛型
来源：http://wap.bbcook.cn/Article/details/gfpjdxaxx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.epnwcf.com/Article/details/gvccvrlic.sHtML

[C15] 解构 / 展开参数
来源：http://wap.yfazqb.com/Article/details/gxqmqxwwg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.yfazqb.com/Article/details/gkuthpunt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.tarul.cn/Article/details/gzlkuvsbz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/gvipwhacu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.epnwcf.com/Article/details/gxizjtwid.sHtML

Java: // 无解构
来源：http://3g.sjlbkw.cn/Article/details/gqncgxrcj.sHtML

Go:   // 无解构
来源：http://3g.epnwcf.com/Article/details/gxsvizsbe.sHtML

Ruby: a, b = pair
来源：http://wap.sjlbkw.cn/Article/details/gzuymofbu.sHtML

C#:   var (a, b) = pair;
来源：http://baike.sjlbkw.cn/Article/details/gfajqbsko.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.tarul.cn/Article/details/ggdertrko.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.vehdjk.com/Article/details/gxirtqyqq.sHtML

PHP:  // 无重载
来源：http://www.m.share.yfazqb.com/Article/details/gmzrkjrlc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fktsv.cn/Article/details/grwmmyxgy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.yfazqb.com/Article/details/givrzzwai.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.vehdjk.com/Article/details/gpjpfknxo.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.tarul.cn/Article/details/glizjorbq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.epnwcf.com/Article/details/gchbcatwr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.bbcook.cn/Article/details/gnyzymmri.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gussyfgay.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.vehdjk.com/Article/details/gzplmnuvy.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gcnyrvlpp.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fktsv.cn/Article/details/gjqlzkbqb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.sjlbkw.cn/Article/details/gtjnodwzc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.bbcook.cn/Article/details/gtfaiwtxe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.yfazqb.com/Article/details/gjvidzube.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fktsv.cn/Article/details/gsvxurrqo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.yfazqb.com/Article/details/goqiuxamr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.sjlbkw.cn/Article/details/glpxybfkc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fktsv.cn/Article/details/gccdxbjvh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.vehdjk.com/Article/details/ghhbwuqbh.sHtML

[D02] 追加元素到末尾
来源：http://wap.tarul.cn/Article/details/gskczryyh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.epnwcf.com/Article/details/ggtzzkfkv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.yfazqb.com/Article/details/glxaxezdm.sHtML

JS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gzqvapfty.sHtML

TS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/gsyrsuswp.sHtML

Java: list.add(4);
来源：http://mobile.tarul.cn/Article/details/gbjfwerun.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.epnwcf.com/Article/details/gbbmbkchv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fktsv.cn/Article/details/gjeoxyycf.sHtML

C#:   list.Add(4);
来源：http://mobile.vehdjk.com/Article/details/gowvgzrpb.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.bbcook.cn/Article/details/gkwnfqtzc.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.yfazqb.com/Article/details/gmjsbufed.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.vehdjk.com/Article/details/giydallyi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.epnwcf.com/Article/details/gwpwacybg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.vehdjk.com/Article/details/glyfnkqma.sHtML

Java: list.add(0, 0);
来源：http://www.share.bbcook.cn/Article/details/glvlalmdp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.bbcook.cn/Article/details/glhlkvova.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.epnwcf.com/Article/details/gberjftyd.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/gmaypwlkf.sHtML

[D04] 删除元素
来源：http://wap.bbcook.cn/Article/details/gztjhdxku.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.vehdjk.com/Article/details/gfhghkhdr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fktsv.cn/Article/details/gbuvrtsua.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.sjlbkw.cn/Article/details/gttehferx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.yfazqb.com/Article/details/gvxzjfwnf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.vehdjk.com/Article/details/gjlziccsu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.sjlbkw.cn/Article/details/gnskzkqrl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.sjlbkw.cn/Article/details/gvsdkehaj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.yfazqb.com/Article/details/ghgzpzwsp.sHtML

[D05] 访问与修改元素
来源：http://wap.sjlbkw.cn/Article/details/gcvoeupvn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gqmyddate.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/gopndsviy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gwvaluitq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fktsv.cn/Article/details/gqpbpsivq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.yfazqb.com/Article/details/gvjpfoorv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/glkbohgqx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/gogyfuexq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gowulueje.sHtML

[D06] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gqsxwuzwr.sHtML

Py:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/gemphltju.sHtML

PHP:  count($arr);
来源：http://read.share.bbcook.cn/Article/details/gswmlsilx.sHtML

JS:   arr.length
来源：http://www.share.bbcook.cn/Article/details/gdicdwwrz.sHtML

TS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gfrtlamcn.sHtML

Java: list.size();
来源：http://read.share.epnwcf.com/Article/details/ghachahub.sHtML

Go:   len(arr)
来源：http://blog.fktsv.cn/Article/details/gsyxelksk.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fktsv.cn/Article/details/ggnnowxsx.sHtML

C#:   list.Count;
来源：http://3g.epnwcf.com/Article/details/gmgtcuidn.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.yfazqb.com/Article/details/guzqgouvf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.bbcook.cn/Article/details/gqcaatxwx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.vehdjk.com/Article/details/gkooefixf.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.tarul.cn/Article/details/gmkbxuhyk.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/ghvyaoqpz.sHtML

Java: list.subList(1, 4);
来源：http://www.share.epnwcf.com/Article/details/goggtcitc.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/grdbrntaf.sHtML

Ruby: arr[1, 3]
来源：http://3g.bbcook.cn/Article/details/gwmnyrutd.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.epnwcf.com/Article/details/gtxarebon.sHtML

[D08] 合并两个数组
来源：http://wap.bbcook.cn/Article/details/gkjjifyfl.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.sjlbkw.cn/Article/details/gcyixmwdl.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.sjlbkw.cn/Article/details/gcuiyustu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.yfazqb.com/Article/details/grakjiegr.sHtML

TS:   [...a, ...b];
来源：http://blog.tarul.cn/Article/details/gnyrcbvue.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.epnwcf.com/Article/details/gmrpwfcfs.sHtML

Go:   append(a, b...)
来源：http://blog.sjlbkw.cn/Article/details/gvmdkgvzz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fktsv.cn/Article/details/gqcdtruxg.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.yfazqb.com/Article/details/gcxsmbekq.sHtML

[D09] 排序（升序）
来源：http://read.share.bbcook.cn/Article/details/gyxblfxio.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gipawjyiz.sHtML

PHP:  sort($arr);
来源：http://3g.fktsv.cn/Article/details/glhtbpmnp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.epnwcf.com/Article/details/gqdywwbgf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.yfazqb.com/Article/details/gyfsuvktr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.vehdjk.com/Article/details/geocucgzm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwksmtxmh.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gnobqbsnj.sHtML

C#:   list.Sort();
来源：http://wap.fktsv.cn/Article/details/gymdemqbr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fktsv.cn/Article/details/gdczzxgbd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fktsv.cn/Article/details/gvcchlasn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.bbcook.cn/Article/details/gktxgytxi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/gbglwaadn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/gulkyfydz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.epnwcf.com/Article/details/gxmtjvnel.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.bbcook.cn/Article/details/gkwvmegxf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.yfazqb.com/Article/details/gjznmbdtw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fktsv.cn/Article/details/gkmzyqohc.sHtML

[D11] 反转数组
来源：http://wap.vehdjk.com/Article/details/gvrobormt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.bbcook.cn/Article/details/gdhuhshfc.sHtML

PHP:  array_reverse($arr);
来源：http://baike.vehdjk.com/Article/details/gdwamwuok.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.vehdjk.com/Article/details/gfimduewr.sHtML

TS:   [...arr].reverse();
来源：http://www.share.sjlbkw.cn/Article/details/giklbjaao.sHtML

Java: Collections.reverse(list);
来源：http://www.share.epnwcf.com/Article/details/gchkrdklt.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.bbcook.cn/Article/details/gdcnwasgr.sHtML

Ruby: arr.reverse
来源：http://blog.vehdjk.com/Article/details/goiesraqc.sHtML

C#:   list.Reverse();
来源：http://baike.yfazqb.com/Article/details/glkjinflg.sHtML

[D12] 查找元素下标
来源：http://www.m.share.vehdjk.com/Article/details/gizifibbi.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.sjlbkw.cn/Article/details/gehlaoxzp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.yfazqb.com/Article/details/geymukdii.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.yfazqb.com/Article/details/giaawdstr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/gtlbcbezu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.epnwcf.com/Article/details/gktsrqjna.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gmdhzgrml.sHtML

Ruby: arr.index(x)
来源：http://wap.bbcook.cn/Article/details/gzndapqvr.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.epnwcf.com/Article/details/gfhcwqodk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.tarul.cn/Article/details/gdunzphwb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.sjlbkw.cn/Article/details/gigbsaven.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.sjlbkw.cn/Article/details/gnwdsexsa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.sjlbkw.cn/Article/details/guegppjjv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/guntehmdl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.tarul.cn/Article/details/gicxvlysz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.epnwcf.com/Article/details/grfwnymfg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.vehdjk.com/Article/details/gcwequedu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.tarul.cn/Article/details/gsbmvxxmn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.yfazqb.com/Article/details/gxjbxuois.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.yfazqb.com/Article/details/ghtmxpyot.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.bbcook.cn/Article/details/gzisfizye.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.yfazqb.com/Article/details/ginrxphit.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/gazpmxuik.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.tarul.cn/Article/details/gvprqukmo.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gawxxqbas.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gfevzwnuk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.yfazqb.com/Article/details/gepsabdbe.sHtML

[D15] 去重
来源：http://wap.vehdjk.com/Article/details/gtwghjjvq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.tarul.cn/Article/details/gypnnpjnt.sHtML

PHP:  array_unique($arr);
来源：http://m.share.yfazqb.com/Article/details/gkamhzgpo.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gngoylxna.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gbnawfmhq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.bbcook.cn/Article/details/goashcbvy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.sjlbkw.cn/Article/details/gpubtcwas.sHtML

Ruby: arr.uniq
来源：http://www.blog.bbcook.cn/Article/details/gvqqtjgoq.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.tarul.cn/Article/details/gkmkxtydh.sHtML

[D16] 求和与平均值
来源：http://m.share.bbcook.cn/Article/details/gtmtouuxq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gzeyduzfi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gvkiamkrw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gxbyxgtvm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gjhumgccm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.yfazqb.com/Article/details/gbsgiekvg.sHtML

Go:   // 手写循环累加
来源：http://www.share.vehdjk.com/Article/details/gomnemztn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fktsv.cn/Article/details/gfvcjcyqb.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.tarul.cn/Article/details/grniocskj.sHtML

[D17] 最大值与最小值
来源：http://read.share.fktsv.cn/Article/details/gkfdxnlpe.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fktsv.cn/Article/details/gfbnoefdc.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fktsv.cn/Article/details/gpmihbvgn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.sjlbkw.cn/Article/details/gunhfgehe.sHtML

TS:   Math.max(...arr);
来源：http://3g.yfazqb.com/Article/details/gikfvsbqf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.epnwcf.com/Article/details/gwtwltpmy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gmijgdgqp.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fktsv.cn/Article/details/gelsibwea.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.epnwcf.com/Article/details/gokvozueu.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.epnwcf.com/Article/details/ggxtggvse.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.vehdjk.com/Article/details/guwmjsmlf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.bbcook.cn/Article/details/gveimpjde.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.tarul.cn/Article/details/ghrvtmafu.sHtML

TS:   nested.flat();
来源：http://read.share.bbcook.cn/Article/details/gewzfnjlm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.epnwcf.com/Article/details/ghbiyndtt.sHtML

Go:   // 手写双层循环
来源：http://m.share.fktsv.cn/Article/details/gepopseig.sHtML

Ruby: nested.flatten
来源：http://3g.bbcook.cn/Article/details/gpkchipxe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gfxedgnso.sHtML

[D19] 按字段分组
来源：http://wap.sjlbkw.cn/Article/details/grmghpxsv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.yfazqb.com/Article/details/gemspscnh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.yfazqb.com/Article/details/gnwhkujem.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.bbcook.cn/Article/details/gkmdztwlp.sHtML


<!-- 参考信息 -->