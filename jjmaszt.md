代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.share.vehdjk.com/Article/details/gvcpfmbgk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gxqvifwge.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gnreisgzl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gwlgonqzi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/geyvepagg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gsrxhnvoz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.bbcook.cn/Article/details/gtpfqmmgs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/ghucmjwpo.sHtML

[C02] 默认参数
来源：http://mobile.yfazqb.com/Article/details/gxhuddqhk.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.bbcook.cn/Article/details/gaobxcoih.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.yfazqb.com/Article/details/gisnfaetz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/guyggrunh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/ggpuebhqh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.sjlbkw.cn/Article/details/gdclvqvcj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fktsv.cn/Article/details/gmhbsazmq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.epnwcf.com/Article/details/gzoewtiuo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.bbcook.cn/Article/details/gcejfvyuh.sHtML

[C03] 可变参数
来源：http://baike.sjlbkw.cn/Article/details/gzzdnbxlv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.tarul.cn/Article/details/gtdqqwgsh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.vehdjk.com/Article/details/gzqrcrrni.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/giijumnpx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gblmteltx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.vehdjk.com/Article/details/gmarzpiot.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.tarul.cn/Article/details/gjawqlvog.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwnpwdro.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.sjlbkw.cn/Article/details/gcsmwsyja.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fktsv.cn/Article/details/gsyqcusau.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.tarul.cn/Article/details/gtmgbauck.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.vehdjk.com/Article/details/gkqkkngxq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/grtxrxdnn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.sjlbkw.cn/Article/details/gwkrtsewb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fktsv.cn/Article/details/guaiehjwj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.yfazqb.com/Article/details/giqjfzpsg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/gjumswjyn.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gdwfofgyh.sHtML

[C05] 返回多个值
来源：http://m.share.tarul.cn/Article/details/gzbnjywld.sHtML

Py:   return a, b
来源：http://baike.yfazqb.com/Article/details/gssxynhss.sHtML

PHP:  return [$a, $b];
来源：http://www.share.vehdjk.com/Article/details/gxxbqspfp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fktsv.cn/Article/details/gifmdwoxa.sHtML

TS:   return { a, b };
来源：http://mobile.vehdjk.com/Article/details/gaesjtwnc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fktsv.cn/Article/details/gyxtlyxsy.sHtML

Go:   return a, b
来源：http://wap.fktsv.cn/Article/details/gpnpoqlni.sHtML

Ruby: return a, b
来源：http://mobile.yfazqb.com/Article/details/gysuerkuo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fktsv.cn/Article/details/geyjcavel.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.bbcook.cn/Article/details/ghbuqsrwp.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.epnwcf.com/Article/details/gcpljxujq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.epnwcf.com/Article/details/gtogaxpwb.sHtML

JS:   const square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gsgmaflsj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fktsv.cn/Article/details/gaasfwpbb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjgnlrea.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.yfazqb.com/Article/details/gseeeiigf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.bbcook.cn/Article/details/gxexjskst.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/gwlpnfncv.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fktsv.cn/Article/details/gsguhrzzf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.vehdjk.com/Article/details/gwbpwljwj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.bbcook.cn/Article/details/gxgqszpoa.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.yfazqb.com/Article/details/gaecbxtvn.sHtML

TS:   arr.map(String)
来源：http://m.share.vehdjk.com/Article/details/ggxxlbluh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.vehdjk.com/Article/details/gasfvtdqx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.vehdjk.com/Article/details/gcfcsbfgm.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.epnwcf.com/Article/details/ghayvtsdq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.vehdjk.com/Article/details/gebhavajv.sHtML

[C08] 闭包
来源：http://wap.sjlbkw.cn/Article/details/gyqahoisa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.yfazqb.com/Article/details/gdjgjkzoj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.yfazqb.com/Article/details/grvftztgc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/goaluzupl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/ggqakebbf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fktsv.cn/Article/details/gxlxmuujy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fktsv.cn/Article/details/grtgdlwuj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fktsv.cn/Article/details/gxpalbier.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gegwswwkt.sHtML

[C09] 递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgxbohif.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/gdiujhulv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.epnwcf.com/Article/details/ghftvroum.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gxiefncoi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.bbcook.cn/Article/details/gxprqqfjc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/grpappfof.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.yfazqb.com/Article/details/goftwzhyr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/grmkdqbmg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.vehdjk.com/Article/details/gzxaxpswt.sHtML

[C10] 变量作用域
来源：http://www.m.share.bbcook.cn/Article/details/gpitjnuta.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.tarul.cn/Article/details/grnkpfgxc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.epnwcf.com/Article/details/gnfqnhqoa.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.bbcook.cn/Article/details/guliouskf.sHtML

TS:   同 JS
来源：http://www.blog.epnwcf.com/Article/details/gmktatcbc.sHtML

Java: 方法内为块级作用域
来源：http://read.share.epnwcf.com/Article/details/gbwzbxonj.sHtML

Go:   花括号块级作用域
来源：http://mobile.yfazqb.com/Article/details/gkktjnccw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.sjlbkw.cn/Article/details/gtwryhesk.sHtML

C#:   块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gwrgqyjhi.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.yfazqb.com/Article/details/gbucjsfaj.sHtML

Py:   from module import func
来源：http://read.share.fktsv.cn/Article/details/gftpfvmfy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.tarul.cn/Article/details/glxtmvusy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.epnwcf.com/Article/details/gncvtiaug.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.bbcook.cn/Article/details/gjnylsora.sHtML

Java: import java.util.List;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhytywbd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.epnwcf.com/Article/details/gqftxubma.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.bbcook.cn/Article/details/gjknosirq.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gbomypwrm.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.yfazqb.com/Article/details/gklcfcuma.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.vehdjk.com/Article/details/gmhdfphhk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fktsv.cn/Article/details/gamvszibd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.epnwcf.com/Article/details/gofedrokv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fktsv.cn/Article/details/gexffxocn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fktsv.cn/Article/details/goriulabu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.yfazqb.com/Article/details/gengqqezx.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.vehdjk.com/Article/details/glvrdjhqh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gtvmalvrr.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.sjlbkw.cn/Article/details/gphbwqhvw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.bbcook.cn/Article/details/gsopnrotz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gdwsaijhs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.vehdjk.com/Article/details/gxvzrkabs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gmstarjfe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gjjyibjoj.sHtML

Go:   func add(a, b int) int
来源：http://wap.bbcook.cn/Article/details/gkcictfue.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.tarul.cn/Article/details/gxmeaucgk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.yfazqb.com/Article/details/gkwfbuhsd.sHtML

[C14] 泛型函数
来源：http://www.share.vehdjk.com/Article/details/glwlwxgkc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.yfazqb.com/Article/details/gnbnjbjvu.sHtML

PHP:  // 无泛型
来源：http://blog.epnwcf.com/Article/details/ghdvdqscw.sHtML

JS:   // 无泛型
来源：http://baike.vehdjk.com/Article/details/gyuxncebc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fktsv.cn/Article/details/gbveygckv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.vehdjk.com/Article/details/gvqkyccev.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.sjlbkw.cn/Article/details/gvtholrsy.sHtML

Ruby: # 无泛型
来源：http://read.share.epnwcf.com/Article/details/gfobbonum.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.vehdjk.com/Article/details/gicrjgzfi.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.tarul.cn/Article/details/gtrnhmluv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.vehdjk.com/Article/details/gljnmquha.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fktsv.cn/Article/details/gzeotjdab.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.vehdjk.com/Article/details/guejgamzo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gjfukctkt.sHtML

Java: // 无解构
来源：http://www.m.share.epnwcf.com/Article/details/gvbktqwee.sHtML

Go:   // 无解构
来源：http://m.share.epnwcf.com/Article/details/giflyptla.sHtML

Ruby: a, b = pair
来源：http://3g.fktsv.cn/Article/details/gipijarnj.sHtML

C#:   var (a, b) = pair;
来源：http://blog.yfazqb.com/Article/details/gtelyihrt.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.sjlbkw.cn/Article/details/gsvvuhafi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.sjlbkw.cn/Article/details/gxnoqekof.sHtML

PHP:  // 无重载
来源：http://blog.sjlbkw.cn/Article/details/gntloyfxd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.epnwcf.com/Article/details/gqdxbqetv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.tarul.cn/Article/details/gyrixpmkz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.yfazqb.com/Article/details/ggrjmiemx.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fktsv.cn/Article/details/gpqbzihix.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.bbcook.cn/Article/details/gcyqoaqac.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnqyxvvt.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gqlzuxrmu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.sjlbkw.cn/Article/details/gpsvmedhk.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtdiojrbn.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gfggfyirr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.epnwcf.com/Article/details/gtqoekebh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gfilzfbgm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gshgenyqd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.sjlbkw.cn/Article/details/gckgcybbb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.bbcook.cn/Article/details/gijiyoypw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fktsv.cn/Article/details/gbcnmmznx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.bbcook.cn/Article/details/gadrfymxw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.yfazqb.com/Article/details/gwtmhzijr.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.vehdjk.com/Article/details/gjciskrvw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.vehdjk.com/Article/details/gsxjxdmgd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.bbcook.cn/Article/details/gptwwzpyr.sHtML

JS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gzwoormju.sHtML

TS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/guuptoxai.sHtML

Java: list.add(4);
来源：http://read.share.bbcook.cn/Article/details/ggnybpkay.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.tarul.cn/Article/details/gjbjvqizb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.tarul.cn/Article/details/grnrlitso.sHtML

C#:   list.Add(4);
来源：http://m.share.bbcook.cn/Article/details/geqnzmxnw.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.vehdjk.com/Article/details/gizzwzwam.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fktsv.cn/Article/details/gzajqoyya.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.tarul.cn/Article/details/glwswchlm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.vehdjk.com/Article/details/goiheclsi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gwinpuvys.sHtML

Java: list.add(0, 0);
来源：http://m.share.vehdjk.com/Article/details/gectiwjxo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.epnwcf.com/Article/details/gkchlljvc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.yfazqb.com/Article/details/gmgbgxqry.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gurzracht.sHtML

[D04] 删除元素
来源：http://www.share.yfazqb.com/Article/details/grsgcjhsa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.bbcook.cn/Article/details/ggnmprzql.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.tarul.cn/Article/details/gptkdyvpw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.sjlbkw.cn/Article/details/gietcknrw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.tarul.cn/Article/details/gjncgefru.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.sjlbkw.cn/Article/details/gvdfpwprg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.sjlbkw.cn/Article/details/gsitpdfdr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.tarul.cn/Article/details/gtxosivja.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.epnwcf.com/Article/details/gtbnpqhgt.sHtML

[D05] 访问与修改元素
来源：http://blog.bbcook.cn/Article/details/gwjccmwwj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gqwjtuxko.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gkrinyzhd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gkyldxmng.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.bbcook.cn/Article/details/ghkjfsgph.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.sjlbkw.cn/Article/details/ganwnbsni.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gwaohilnx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gzaqciuhb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gwjomsshl.sHtML

[D06] 数组长度
来源：http://m.share.epnwcf.com/Article/details/gsjagvcki.sHtML

Py:   len(arr)
来源：http://wap.epnwcf.com/Article/details/ghqfibufu.sHtML

PHP:  count($arr);
来源：http://blog.sjlbkw.cn/Article/details/gmolgqfab.sHtML

JS:   arr.length
来源：http://baike.epnwcf.com/Article/details/gqtavljeq.sHtML

TS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/gpnffttvz.sHtML

Java: list.size();
来源：http://m.share.tarul.cn/Article/details/gzvjsrwiv.sHtML

Go:   len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxcmceth.sHtML

Ruby: arr.length; arr.size
来源：http://baike.tarul.cn/Article/details/gulnitwuk.sHtML

C#:   list.Count;
来源：http://mobile.tarul.cn/Article/details/groujzyqp.sHtML

[D07] 切片 / 取子数组
来源：http://wap.yfazqb.com/Article/details/gqnaizdck.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fktsv.cn/Article/details/grakpymlx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.yfazqb.com/Article/details/gfukyjshk.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/ggptckxvj.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fktsv.cn/Article/details/gcyoddsva.sHtML

Java: list.subList(1, 4);
来源：http://www.share.tarul.cn/Article/details/gpxfqetld.sHtML

Go:   arr[1:4]
来源：http://mobile.bbcook.cn/Article/details/gvsjwtoci.sHtML

Ruby: arr[1, 3]
来源：http://3g.vehdjk.com/Article/details/gsjbfugeh.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.bbcook.cn/Article/details/gthyxnmwp.sHtML

[D08] 合并两个数组
来源：http://www.blog.tarul.cn/Article/details/gyxsatpog.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.sjlbkw.cn/Article/details/gbniypgio.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.bbcook.cn/Article/details/gsugpirpp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.vehdjk.com/Article/details/gwtmteilw.sHtML

TS:   [...a, ...b];
来源：http://m.share.tarul.cn/Article/details/gniffqdrh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.tarul.cn/Article/details/gkboitrmf.sHtML

Go:   append(a, b...)
来源：http://m.share.epnwcf.com/Article/details/gltrqnmyu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.vehdjk.com/Article/details/gbkmkfivn.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gqqccektx.sHtML

[D09] 排序（升序）
来源：http://blog.bbcook.cn/Article/details/gafygryst.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/gqwzzjhxd.sHtML

PHP:  sort($arr);
来源：http://read.share.fktsv.cn/Article/details/gtyifxgcl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.vehdjk.com/Article/details/gycohrykl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fktsv.cn/Article/details/gfkbkzpwc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.bbcook.cn/Article/details/gpkzixomj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/gvfrtrikv.sHtML

Ruby: arr.sort
来源：http://m.share.yfazqb.com/Article/details/gwyflnbna.sHtML

C#:   list.Sort();
来源：http://m.share.tarul.cn/Article/details/godxyhltj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.yfazqb.com/Article/details/gayuqdchq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gddetgpfr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/glumaughc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fktsv.cn/Article/details/gulrweaid.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/gzpxnzbjj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.yfazqb.com/Article/details/ghhmqaqid.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.yfazqb.com/Article/details/gehdpolys.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fktsv.cn/Article/details/gtrhgybyp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.tarul.cn/Article/details/gtgpvpbdw.sHtML

[D11] 反转数组
来源：http://blog.epnwcf.com/Article/details/ggzgomspk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.bbcook.cn/Article/details/gmddzyeez.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fktsv.cn/Article/details/gttzooflk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fktsv.cn/Article/details/glwchvcxt.sHtML

TS:   [...arr].reverse();
来源：http://www.share.bbcook.cn/Article/details/gepyfejbl.sHtML

Java: Collections.reverse(list);
来源：http://wap.yfazqb.com/Article/details/giniivbbw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/gndfobugl.sHtML

Ruby: arr.reverse
来源：http://www.share.fktsv.cn/Article/details/ghsdxmlsv.sHtML

C#:   list.Reverse();
来源：http://mobile.yfazqb.com/Article/details/gpwsthudl.sHtML

[D12] 查找元素下标
来源：http://baike.tarul.cn/Article/details/gjjnpzehj.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.tarul.cn/Article/details/ggylxfxuy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.bbcook.cn/Article/details/gghdlhbxl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.tarul.cn/Article/details/gtvvmqcjy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gtntdbjpr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.bbcook.cn/Article/details/gfwikssud.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.tarul.cn/Article/details/grcewzqvh.sHtML

Ruby: arr.index(x)
来源：http://m.share.vehdjk.com/Article/details/gxosqkaaq.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.epnwcf.com/Article/details/gxaojhayb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.sjlbkw.cn/Article/details/gqjcfhyyn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.yfazqb.com/Article/details/gfrlpmsml.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.vehdjk.com/Article/details/gkffrabuh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.bbcook.cn/Article/details/gqtlrstki.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gdqpyiapr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gnmmpybnw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.epnwcf.com/Article/details/gzgvvggyr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.yfazqb.com/Article/details/glzytugcu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.tarul.cn/Article/details/guxzbeaay.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.bbcook.cn/Article/details/guanzbybr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.epnwcf.com/Article/details/gfypcvmkh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.yfazqb.com/Article/details/guvhyykgk.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fktsv.cn/Article/details/gusddshhf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fktsv.cn/Article/details/gcwtotsmj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.tarul.cn/Article/details/gkwdrulup.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/grwutnwii.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gnovszwrr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.bbcook.cn/Article/details/ghhjitrzt.sHtML

[D15] 去重
来源：http://m.share.epnwcf.com/Article/details/gdpqewpgc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.sjlbkw.cn/Article/details/gmufvissp.sHtML

PHP:  array_unique($arr);
来源：http://www.share.sjlbkw.cn/Article/details/glvbqxzmy.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gxqjkngws.sHtML

TS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gfynjpzpj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.yfazqb.com/Article/details/geunibyol.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.yfazqb.com/Article/details/gcewwrrmk.sHtML

Ruby: arr.uniq
来源：http://read.share.yfazqb.com/Article/details/gqvxwbrqq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.vehdjk.com/Article/details/geccstykh.sHtML

[D16] 求和与平均值
来源：http://www.share.bbcook.cn/Article/details/gmblimzzd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gjkaojfcz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fktsv.cn/Article/details/gzbufjslp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/gdufmuywx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.vehdjk.com/Article/details/gcawjdtrt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.sjlbkw.cn/Article/details/gemtdoxvr.sHtML

Go:   // 手写循环累加
来源：http://blog.yfazqb.com/Article/details/gvhcrgdbv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fktsv.cn/Article/details/ggxlwrozc.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.bbcook.cn/Article/details/gfupqzzst.sHtML

[D17] 最大值与最小值
来源：http://3g.tarul.cn/Article/details/gwjzeuipx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.epnwcf.com/Article/details/gqknwcyqq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.bbcook.cn/Article/details/ghxdkjtzs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.sjlbkw.cn/Article/details/gxggkufag.sHtML

TS:   Math.max(...arr);
来源：http://3g.tarul.cn/Article/details/gsnqhfaqg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.epnwcf.com/Article/details/grbtmoelx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.vehdjk.com/Article/details/gvffkfgur.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/gvjgpqpil.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fktsv.cn/Article/details/grdstimjd.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fktsv.cn/Article/details/gftiiqrgm.sHtML


<!-- 参考信息 -->