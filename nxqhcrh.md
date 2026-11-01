代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://read.share.bbcook.cn/Article/details/gjabztxfg.sHtML

[C03] 可变参数
来源：http://3g.vehdjk.com/Article/details/gbkrdrypu.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.bbcook.cn/Article/details/gwinyfbrt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.sjlbkw.cn/Article/details/gcabrmesg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/gihqanrfh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/gpbabgmil.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.tarul.cn/Article/details/gcqrtxyhj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.sjlbkw.cn/Article/details/gobavbisi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.bbcook.cn/Article/details/gowdfxihp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.sjlbkw.cn/Article/details/guhpypovt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.tarul.cn/Article/details/gwgvfjkyh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.epnwcf.com/Article/details/gvoyfwjtd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gamwhxivi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.sjlbkw.cn/Article/details/gwvdmcpnt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.vehdjk.com/Article/details/gptsjwlrf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.yfazqb.com/Article/details/gwlrqwrhn.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.tarul.cn/Article/details/guemgfqly.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gnnjkbrtw.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gvdspukev.sHtML

[C05] 返回多个值
来源：http://www.m.share.epnwcf.com/Article/details/gvazbyekl.sHtML

Py:   return a, b
来源：http://baike.vehdjk.com/Article/details/gzkfcdwtw.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.tarul.cn/Article/details/gemumkcge.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.yfazqb.com/Article/details/goimetikn.sHtML

TS:   return { a, b };
来源：http://m.share.fktsv.cn/Article/details/gjlvlxfpu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.bbcook.cn/Article/details/gotllxuan.sHtML

Go:   return a, b
来源：http://blog.vehdjk.com/Article/details/gpcmpvqmo.sHtML

Ruby: return a, b
来源：http://www.m.share.tarul.cn/Article/details/garlrvdyc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.sjlbkw.cn/Article/details/gnbfwtrmp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fktsv.cn/Article/details/gzfygihmj.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fktsv.cn/Article/details/glkcompvf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fktsv.cn/Article/details/gfaaxkdjw.sHtML

JS:   const square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/gvtydvtew.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.yfazqb.com/Article/details/gudyqjssj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fktsv.cn/Article/details/gccetscrz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.tarul.cn/Article/details/gqxcwbmoq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.epnwcf.com/Article/details/gibfotnuz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/gswheqlmp.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.vehdjk.com/Article/details/gaascacig.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.vehdjk.com/Article/details/gtffyujbm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/ggyaljzkq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.sjlbkw.cn/Article/details/gcvcxkjxd.sHtML

TS:   arr.map(String)
来源：http://mobile.bbcook.cn/Article/details/gwhgzxlvq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.epnwcf.com/Article/details/gxynbnwuk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.yfazqb.com/Article/details/ghfrzkrbr.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.sjlbkw.cn/Article/details/grabbyiew.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.epnwcf.com/Article/details/gsroisogp.sHtML

[C08] 闭包
来源：http://read.share.fktsv.cn/Article/details/ghldihdiw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.sjlbkw.cn/Article/details/gqvezhbit.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.epnwcf.com/Article/details/gkhfmgpdp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gdvobvkoi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gqsqbbbiy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.bbcook.cn/Article/details/gmcatwops.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.epnwcf.com/Article/details/gzyqwgnif.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.sjlbkw.cn/Article/details/gdhqisoad.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/giwunrwed.sHtML

[C09] 递归
来源：http://mobile.sjlbkw.cn/Article/details/gyetcikxa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gnakpanwd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/gmzxychqo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.yfazqb.com/Article/details/guuutptoy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/gvrlrzilm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fktsv.cn/Article/details/gtmulmugs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.sjlbkw.cn/Article/details/geyzasnkz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/gfygfamxx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.tarul.cn/Article/details/gdudxhvog.sHtML

[C10] 变量作用域
来源：http://read.share.tarul.cn/Article/details/gyflewlbh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.epnwcf.com/Article/details/grhujijqh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/gitjbdzgs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fktsv.cn/Article/details/gnbmhoxko.sHtML

TS:   同 JS
来源：http://wap.tarul.cn/Article/details/guzpizcmm.sHtML

Java: 方法内为块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gizvjqttr.sHtML

Go:   花括号块级作用域
来源：http://blog.bbcook.cn/Article/details/gqgscwebg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.vehdjk.com/Article/details/gqigkdfyj.sHtML

C#:   块级作用域
来源：http://m.share.vehdjk.com/Article/details/gotkepujc.sHtML

[C11] 模块导入与导出
来源：http://wap.epnwcf.com/Article/details/gwmsrczcr.sHtML

Py:   from module import func
来源：http://wap.fktsv.cn/Article/details/gabfgzngu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.yfazqb.com/Article/details/gvscjxyll.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fktsv.cn/Article/details/gkimxjegj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.epnwcf.com/Article/details/gowkeosxk.sHtML

Java: import java.util.List;
来源：http://www.m.share.epnwcf.com/Article/details/gafvvjqdh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.epnwcf.com/Article/details/ghupdvjvq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fktsv.cn/Article/details/gzpxmgcjo.sHtML

C#:   using System.Text;
来源：http://blog.yfazqb.com/Article/details/gojgnwyuj.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.vehdjk.com/Article/details/ggtmvelya.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fktsv.cn/Article/details/gftmkrlgn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.tarul.cn/Article/details/gcaospisa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gfrofeqyt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gdeehbybw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.bbcook.cn/Article/details/gxsswcugg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.bbcook.cn/Article/details/ggvfizokg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.yfazqb.com/Article/details/glpsgqrfk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gdmkosqmm.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.vehdjk.com/Article/details/gjqigqdog.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.vehdjk.com/Article/details/gcvhxrcwv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gygafvgzq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.yfazqb.com/Article/details/gtwlkslmx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gbmmsnpty.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gtmysuejr.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fktsv.cn/Article/details/gkqnmtwov.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.yfazqb.com/Article/details/gfpruqubs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.sjlbkw.cn/Article/details/gbpodhdlw.sHtML

[C14] 泛型函数
来源：http://3g.yfazqb.com/Article/details/gzbsqklwx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.sjlbkw.cn/Article/details/gzlthbgpq.sHtML

PHP:  // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gwqmzcfww.sHtML

JS:   // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gomjuaalu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.epnwcf.com/Article/details/gurxizjri.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.tarul.cn/Article/details/gjsaxbjrj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.vehdjk.com/Article/details/ggtwrwand.sHtML

Ruby: # 无泛型
来源：http://mobile.fktsv.cn/Article/details/gtoxadkox.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.epnwcf.com/Article/details/gopyvlzpl.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.sjlbkw.cn/Article/details/gibuwymwd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/gpqhcjosx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.sjlbkw.cn/Article/details/gdeptjknx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/gapsxolwl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.epnwcf.com/Article/details/gyplbzlgu.sHtML

Java: // 无解构
来源：http://read.share.tarul.cn/Article/details/gckduvdar.sHtML

Go:   // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gejolkdcp.sHtML

Ruby: a, b = pair
来源：http://www.m.share.yfazqb.com/Article/details/gbsrecdto.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.tarul.cn/Article/details/gxsvttwhn.sHtML

[C16] 函数 / 方法重载
来源：http://blog.yfazqb.com/Article/details/gidoaouwa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.tarul.cn/Article/details/geuytmjem.sHtML

PHP:  // 无重载
来源：http://blog.epnwcf.com/Article/details/gxscnsawy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.yfazqb.com/Article/details/gcdfjosxk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.epnwcf.com/Article/details/gwdnubkde.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.tarul.cn/Article/details/gozmhultk.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.yfazqb.com/Article/details/gvhpsjwta.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.epnwcf.com/Article/details/gicmdwhvx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.yfazqb.com/Article/details/gxuqkfggf.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggnsagubw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.yfazqb.com/Article/details/gqyvdorel.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gezfotwkm.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.yfazqb.com/Article/details/gwvcqanmd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fktsv.cn/Article/details/gutpptyyz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.vehdjk.com/Article/details/gfigjynms.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.epnwcf.com/Article/details/gbqsuowqz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.tarul.cn/Article/details/gpbqzsijt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.epnwcf.com/Article/details/gajxumzpq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.yfazqb.com/Article/details/getruyges.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.tarul.cn/Article/details/glmczlwni.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.sjlbkw.cn/Article/details/gamarpvjy.sHtML

[D02] 追加元素到末尾
来源：http://baike.vehdjk.com/Article/details/gfdwfgven.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.vehdjk.com/Article/details/gslbplkbm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gjbjxniqt.sHtML

JS:   arr.push(4);
来源：http://m.share.bbcook.cn/Article/details/gaxnzlkwp.sHtML

TS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/glidguvqs.sHtML

Java: list.add(4);
来源：http://www.blog.epnwcf.com/Article/details/gmfptxtud.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.vehdjk.com/Article/details/gbmpjgrwo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.tarul.cn/Article/details/gagirimqh.sHtML

C#:   list.Add(4);
来源：http://wap.bbcook.cn/Article/details/gelccdcpw.sHtML

[D03] 在指定位置插入元素
来源：http://wap.sjlbkw.cn/Article/details/gxmwdiciy.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.bbcook.cn/Article/details/gnrkkjoee.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.sjlbkw.cn/Article/details/gduebqdtp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.sjlbkw.cn/Article/details/gsqhqlzyl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gikqbijxw.sHtML

Java: list.add(0, 0);
来源：http://3g.epnwcf.com/Article/details/gdbhfccwq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.vehdjk.com/Article/details/gjxfhbcks.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.epnwcf.com/Article/details/gamrvuutl.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/grpctgrlb.sHtML

[D04] 删除元素
来源：http://www.m.share.bbcook.cn/Article/details/gbsqsyvzt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.bbcook.cn/Article/details/gwqojnsmw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gdgaoluot.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.vehdjk.com/Article/details/gihwvlaoa.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.vehdjk.com/Article/details/glzbguvrd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.bbcook.cn/Article/details/guabndgbq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.sjlbkw.cn/Article/details/gwdkxxxus.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.epnwcf.com/Article/details/ganoorcnw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fktsv.cn/Article/details/gswxauhxb.sHtML

[D05] 访问与修改元素
来源：http://wap.bbcook.cn/Article/details/ggpascjqs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.vehdjk.com/Article/details/gagcjgcmq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/guqvnbdvb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/ghxutrflt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.vehdjk.com/Article/details/gnkyxuqws.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.sjlbkw.cn/Article/details/giudngrby.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/glctgzbhp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/glqugldnm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gtrupmabf.sHtML

[D06] 数组长度
来源：http://m.share.tarul.cn/Article/details/gqdtflejm.sHtML

Py:   len(arr)
来源：http://baike.epnwcf.com/Article/details/gzuffqyid.sHtML

PHP:  count($arr);
来源：http://mobile.fktsv.cn/Article/details/gnavyfpyh.sHtML

JS:   arr.length
来源：http://blog.yfazqb.com/Article/details/gmoozamnu.sHtML

TS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/ghuwljfxq.sHtML

Java: list.size();
来源：http://wap.sjlbkw.cn/Article/details/gltrrhwiw.sHtML

Go:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gbrwwefjm.sHtML

Ruby: arr.length; arr.size
来源：http://3g.epnwcf.com/Article/details/gflexitmo.sHtML

C#:   list.Count;
来源：http://read.share.tarul.cn/Article/details/gmggsqgbh.sHtML

[D07] 切片 / 取子数组
来源：http://baike.yfazqb.com/Article/details/guiwnzwyr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.sjlbkw.cn/Article/details/ggwsvbpvw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fktsv.cn/Article/details/gpymikhew.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.epnwcf.com/Article/details/gqnquqwxd.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gcjbzlggy.sHtML

Java: list.subList(1, 4);
来源：http://baike.yfazqb.com/Article/details/gbfnkeaho.sHtML

Go:   arr[1:4]
来源：http://mobile.bbcook.cn/Article/details/gsvksqjri.sHtML

Ruby: arr[1, 3]
来源：http://www.share.epnwcf.com/Article/details/gmibtealc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gtmnsjeir.sHtML

[D08] 合并两个数组
来源：http://blog.sjlbkw.cn/Article/details/gjsjsfpzo.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.sjlbkw.cn/Article/details/gemarwscu.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.epnwcf.com/Article/details/gkjkkmqmz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdvyprzw.sHtML

TS:   [...a, ...b];
来源：http://wap.vehdjk.com/Article/details/geqxjdsee.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.bbcook.cn/Article/details/ggmsxpogt.sHtML

Go:   append(a, b...)
来源：http://read.share.tarul.cn/Article/details/gbfngapsx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.yfazqb.com/Article/details/goyoxlmqr.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fktsv.cn/Article/details/gyvqfftsc.sHtML

[D09] 排序（升序）
来源：http://baike.epnwcf.com/Article/details/gigedestt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gkmjbrgum.sHtML

PHP:  sort($arr);
来源：http://read.share.vehdjk.com/Article/details/gfemitifd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.tarul.cn/Article/details/gvjlxswnz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.vehdjk.com/Article/details/gptrcwnfv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.vehdjk.com/Article/details/gmtuaigtq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gahafwcnq.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gbyoadhot.sHtML

C#:   list.Sort();
来源：http://mobile.sjlbkw.cn/Article/details/gphzcmrtm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.sjlbkw.cn/Article/details/gxyiinfwm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fktsv.cn/Article/details/gqpbpbwzx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.epnwcf.com/Article/details/gmcknduge.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.vehdjk.com/Article/details/gconsgtmb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/ggjbrzrmo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.yfazqb.com/Article/details/gghpzjjwd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.tarul.cn/Article/details/gdcrnucgx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.vehdjk.com/Article/details/gkgldenpl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.epnwcf.com/Article/details/gvfoomnuq.sHtML

[D11] 反转数组
来源：http://mobile.vehdjk.com/Article/details/gtocxhxep.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.sjlbkw.cn/Article/details/gqjyudsiy.sHtML

PHP:  array_reverse($arr);
来源：http://blog.sjlbkw.cn/Article/details/gduyfoelo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.vehdjk.com/Article/details/gwbymsfmv.sHtML

TS:   [...arr].reverse();
来源：http://wap.vehdjk.com/Article/details/gmgmhakaq.sHtML

Java: Collections.reverse(list);
来源：http://blog.vehdjk.com/Article/details/gtuuihtfq.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.vehdjk.com/Article/details/gjjhjdohs.sHtML

Ruby: arr.reverse
来源：http://3g.tarul.cn/Article/details/gqomovgdn.sHtML

C#:   list.Reverse();
来源：http://read.share.fktsv.cn/Article/details/gdstfhmsh.sHtML

[D12] 查找元素下标
来源：http://read.share.vehdjk.com/Article/details/glluallbf.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.vehdjk.com/Article/details/gcnbvpxjj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.bbcook.cn/Article/details/gwnthokgp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gnjmqskle.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gagufejts.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fktsv.cn/Article/details/gwwkiftxg.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gddzlcqmb.sHtML

Ruby: arr.index(x)
来源：http://blog.tarul.cn/Article/details/gijiruufy.sHtML

C#:   list.IndexOf(x);
来源：http://wap.bbcook.cn/Article/details/goxobtquw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.epnwcf.com/Article/details/givzngduk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.yfazqb.com/Article/details/gawwyetji.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.yfazqb.com/Article/details/gfnvbizdx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gxfsvanrh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.tarul.cn/Article/details/gpqhjlbpf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.bbcook.cn/Article/details/gwabczbbu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.bbcook.cn/Article/details/gjulvbatz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.vehdjk.com/Article/details/gzsjtfulj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.yfazqb.com/Article/details/gliyurpvm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.epnwcf.com/Article/details/gliaxqrki.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.tarul.cn/Article/details/gdtoojvxn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.vehdjk.com/Article/details/ggmuvojpz.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.yfazqb.com/Article/details/ggggskxyr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/gdphvudyx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.vehdjk.com/Article/details/gourioufc.sHtML

Go:   // 手写循环
来源：http://baike.epnwcf.com/Article/details/gbvrgytbw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.bbcook.cn/Article/details/gpmzsozjl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.vehdjk.com/Article/details/gxikauijp.sHtML

[D15] 去重
来源：http://read.share.vehdjk.com/Article/details/gxtjasbfi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.sjlbkw.cn/Article/details/gwdqpxljh.sHtML

PHP:  array_unique($arr);
来源：http://3g.epnwcf.com/Article/details/geimudxek.sHtML

JS:   [...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gaqrgnwfw.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/gkrdemnwg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.yfazqb.com/Article/details/gbwbfcawm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.epnwcf.com/Article/details/guxxlfqvl.sHtML

Ruby: arr.uniq
来源：http://wap.bbcook.cn/Article/details/goqmuhvku.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.epnwcf.com/Article/details/gmzqchylv.sHtML

[D16] 求和与平均值
来源：http://www.m.share.vehdjk.com/Article/details/guyemcwih.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gybqvybgv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.bbcook.cn/Article/details/gvfgibgdi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gdalxtwyu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/gbvcgzbpb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.epnwcf.com/Article/details/gcdbyddse.sHtML

Go:   // 手写循环累加
来源：http://wap.vehdjk.com/Article/details/gdrouudlk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.sjlbkw.cn/Article/details/gflbeexoe.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.epnwcf.com/Article/details/gqhbuwtug.sHtML

[D17] 最大值与最小值
来源：http://blog.fktsv.cn/Article/details/gnvbykpzx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.tarul.cn/Article/details/gfajlflsm.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.sjlbkw.cn/Article/details/gjtiyabiz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.tarul.cn/Article/details/gpocwgmgu.sHtML

TS:   Math.max(...arr);
来源：http://blog.tarul.cn/Article/details/gesahtfat.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.epnwcf.com/Article/details/grvrpkuzg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fktsv.cn/Article/details/gycmoipgr.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.tarul.cn/Article/details/gomufqzll.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.bbcook.cn/Article/details/gewyklify.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.sjlbkw.cn/Article/details/gvqwbsyiz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.yfazqb.com/Article/details/gctgxeuva.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.sjlbkw.cn/Article/details/gwkgaoqyd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.bbcook.cn/Article/details/guricpnmw.sHtML

TS:   nested.flat();
来源：http://read.share.sjlbkw.cn/Article/details/gcoppyicb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.sjlbkw.cn/Article/details/gteavxyno.sHtML

Go:   // 手写双层循环
来源：http://m.share.bbcook.cn/Article/details/gbocfdoup.sHtML

Ruby: nested.flatten
来源：http://m.share.fktsv.cn/Article/details/gdukgwllx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gbrovowas.sHtML

[D19] 按字段分组
来源：http://www.m.share.vehdjk.com/Article/details/gcqqqlvhv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.vehdjk.com/Article/details/gfxvohopr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.vehdjk.com/Article/details/guqzlkmyz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.sjlbkw.cn/Article/details/gwjqzecqg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/gkayincmb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/gehqgjaya.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.vehdjk.com/Article/details/gieqkelox.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.sjlbkw.cn/Article/details/ggkvcxory.sHtML


<!-- 参考信息 -->