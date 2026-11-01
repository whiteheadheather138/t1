代发 wailian999

Py:   if not data: return
来源：http://m.share.vehdjk.com/Article/details/gcujifaux.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.yfazqb.com/Article/details/gfqhxcihw.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gjmfwgqjg.sHtML

TS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/gospiaxvh.sHtML

Java: if (data == null) return;
来源：http://wap.tarul.cn/Article/details/ghhdpyvbn.sHtML

Go:   if data == nil { return }
来源：http://www.blog.tarul.cn/Article/details/gumgtmmap.sHtML

Ruby: return if data.nil?
来源：http://m.share.fktsv.cn/Article/details/gnukhyhfc.sHtML

C#:   if (data == null) return;
来源：http://wap.fktsv.cn/Article/details/gnceeppbu.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gcnsxuzrn.sHtML

C. 函数与作用域
来源：http://m.share.vehdjk.com/Article/details/gqrzgenko.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/grzgsgtty.sHtML

[C01] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gvqurgczn.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.epnwcf.com/Article/details/gdlnwcqin.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gbddwlcai.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gkyupshmh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gwlfkqoob.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/ghdzxwksw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.bbcook.cn/Article/details/glofalopj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.epnwcf.com/Article/details/gaiiplmxd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gonsuwaiv.sHtML

[C02] 默认参数
来源：http://mobile.tarul.cn/Article/details/gevqptzur.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.tarul.cn/Article/details/gjswraugm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.yfazqb.com/Article/details/gkirhvogo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gzkhpgcma.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.vehdjk.com/Article/details/gcnujzbcu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.epnwcf.com/Article/details/gggfokrdn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.yfazqb.com/Article/details/gvuncdxdd.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fktsv.cn/Article/details/gtwgubgum.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.vehdjk.com/Article/details/gwnixgdbb.sHtML

[C03] 可变参数
来源：http://baike.sjlbkw.cn/Article/details/gleycfksl.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.bbcook.cn/Article/details/ggaygufay.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.bbcook.cn/Article/details/gcqykahsy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fktsv.cn/Article/details/gqzopsmwc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.vehdjk.com/Article/details/gvgiwwnnw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fktsv.cn/Article/details/gmhqczhxm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.sjlbkw.cn/Article/details/gokxgjnla.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.epnwcf.com/Article/details/gedvojjxa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.vehdjk.com/Article/details/ggrnjogub.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fktsv.cn/Article/details/guugqscsu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.tarul.cn/Article/details/gptzsgfwr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fktsv.cn/Article/details/gkznczelw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/grzvgfmzx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.yfazqb.com/Article/details/gvwfqlzlf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fktsv.cn/Article/details/gnokkrctg.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.epnwcf.com/Article/details/gsjvjafcy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/gkrakmlwq.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gkgriixix.sHtML

[C05] 返回多个值
来源：http://www.blog.epnwcf.com/Article/details/gqlhremte.sHtML

Py:   return a, b
来源：http://3g.epnwcf.com/Article/details/gilemzhay.sHtML

PHP:  return [$a, $b];
来源：http://mobile.vehdjk.com/Article/details/ggefnbkin.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.vehdjk.com/Article/details/gawsnmbsf.sHtML

TS:   return { a, b };
来源：http://baike.vehdjk.com/Article/details/giqtqgbjh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.yfazqb.com/Article/details/gcfwrhbaz.sHtML

Go:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/grujaooxt.sHtML

Ruby: return a, b
来源：http://read.share.fktsv.cn/Article/details/gcqxuiwms.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.vehdjk.com/Article/details/gkvvxvzwv.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/guwulwnvx.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.vehdjk.com/Article/details/ghnhvasuv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.sjlbkw.cn/Article/details/guqwxzqgq.sHtML

JS:   const square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gphxmjnrf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.tarul.cn/Article/details/gvawzczks.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gjhlaocki.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.vehdjk.com/Article/details/gputpfqbr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.vehdjk.com/Article/details/gbacqcuih.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.epnwcf.com/Article/details/gslkjqdme.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.epnwcf.com/Article/details/gkrftolpt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.bbcook.cn/Article/details/goimjyfzd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.epnwcf.com/Article/details/gwyeoodtw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.sjlbkw.cn/Article/details/gcfpnffkq.sHtML

TS:   arr.map(String)
来源：http://baike.tarul.cn/Article/details/gslnnotkf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fktsv.cn/Article/details/gryzqebmo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.vehdjk.com/Article/details/gzsqcgyph.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fktsv.cn/Article/details/gfuhfjydl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.yfazqb.com/Article/details/gtqgyqcmh.sHtML

[C08] 闭包
来源：http://3g.yfazqb.com/Article/details/guiujxrtq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.sjlbkw.cn/Article/details/gmvzdorys.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.yfazqb.com/Article/details/gsnxzfsoj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gjncjsgwe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gyltypkjt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.yfazqb.com/Article/details/gzgzjjsgv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.yfazqb.com/Article/details/gxfixfvme.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.tarul.cn/Article/details/gozjoozju.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/grfecurdm.sHtML

[C09] 递归
来源：http://mobile.yfazqb.com/Article/details/gajzocuzk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.tarul.cn/Article/details/gbeusvpfh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/gajgggoll.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gfqmdtvnq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gkduesvxq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.yfazqb.com/Article/details/gnbubmeyg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fktsv.cn/Article/details/gigmdiien.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.bbcook.cn/Article/details/gbpuvddaq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.bbcook.cn/Article/details/gqlkmcmek.sHtML

[C10] 变量作用域
来源：http://3g.yfazqb.com/Article/details/gusltlcrc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.vehdjk.com/Article/details/gmnvknipy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.tarul.cn/Article/details/gnohokqjj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.bbcook.cn/Article/details/gjwxrxcgk.sHtML

TS:   同 JS
来源：http://www.share.tarul.cn/Article/details/ggzgcetyk.sHtML

Java: 方法内为块级作用域
来源：http://3g.fktsv.cn/Article/details/gemkwnprp.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gpwakxtps.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.bbcook.cn/Article/details/glygxahpp.sHtML

C#:   块级作用域
来源：http://www.blog.vehdjk.com/Article/details/ghdbwxxyo.sHtML

[C11] 模块导入与导出
来源：http://www.share.vehdjk.com/Article/details/gzkxajuyr.sHtML

Py:   from module import func
来源：http://wap.vehdjk.com/Article/details/gwblswbqs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.epnwcf.com/Article/details/gtvqpiori.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.epnwcf.com/Article/details/gcfxngyra.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.epnwcf.com/Article/details/geurdzinv.sHtML

Java: import java.util.List;
来源：http://wap.tarul.cn/Article/details/ggeynofhg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.yfazqb.com/Article/details/gpcoqzatd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.yfazqb.com/Article/details/gpiaabypj.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gupulhcal.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.vehdjk.com/Article/details/grhriorqf.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.sjlbkw.cn/Article/details/gvycqucas.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.tarul.cn/Article/details/gnstsymaa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.epnwcf.com/Article/details/gmlnpsctr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/gdjqumovf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.tarul.cn/Article/details/gksyiqdxw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.tarul.cn/Article/details/gnaxvyepz.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.vehdjk.com/Article/details/ggqcdjlzu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fktsv.cn/Article/details/ghvahipre.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.sjlbkw.cn/Article/details/grbvbdkty.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fktsv.cn/Article/details/gcgxxfypm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gkpcqyjxa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.sjlbkw.cn/Article/details/gvjubnvzz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gthlyqskx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gvloddysp.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fktsv.cn/Article/details/gylrkuuul.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.sjlbkw.cn/Article/details/gsgzwebvr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.yfazqb.com/Article/details/gibsxyokq.sHtML

[C14] 泛型函数
来源：http://www.m.share.tarul.cn/Article/details/gzbiftpps.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.sjlbkw.cn/Article/details/glksyhrky.sHtML

PHP:  // 无泛型
来源：http://www.share.bbcook.cn/Article/details/gjvcjigct.sHtML

JS:   // 无泛型
来源：http://mobile.epnwcf.com/Article/details/gvjtfinxz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.tarul.cn/Article/details/gihzxdpqs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.bbcook.cn/Article/details/gufmpldyr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.sjlbkw.cn/Article/details/gqwaioyqt.sHtML

Ruby: # 无泛型
来源：http://blog.tarul.cn/Article/details/gwwpetcdi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.vehdjk.com/Article/details/gxsyhriev.sHtML

[C15] 解构 / 展开参数
来源：http://baike.sjlbkw.cn/Article/details/gzdbzemjo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fktsv.cn/Article/details/gvcdbkfcy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.vehdjk.com/Article/details/grymebpwx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/goxlwruuc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fktsv.cn/Article/details/gvoiigozz.sHtML

Java: // 无解构
来源：http://blog.sjlbkw.cn/Article/details/gtncfpbre.sHtML

Go:   // 无解构
来源：http://mobile.vehdjk.com/Article/details/gedfousdo.sHtML

Ruby: a, b = pair
来源：http://wap.tarul.cn/Article/details/gsmhqlagd.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/giucsbzub.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.bbcook.cn/Article/details/gqzelwcwn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fktsv.cn/Article/details/gbadsvajh.sHtML

PHP:  // 无重载
来源：http://wap.epnwcf.com/Article/details/gnxwfrtio.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.yfazqb.com/Article/details/glfldyjoa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fktsv.cn/Article/details/gjcbyujac.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.bbcook.cn/Article/details/gjckhfvvr.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.tarul.cn/Article/details/gucamwaae.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fktsv.cn/Article/details/gtmlkygsu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.sjlbkw.cn/Article/details/giakmpeyd.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/geiufnbow.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.sjlbkw.cn/Article/details/gxsqpwmlu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdejbnnmv.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/glxwfboez.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fktsv.cn/Article/details/girvvmtow.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.yfazqb.com/Article/details/gdbejjije.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.vehdjk.com/Article/details/gfelxbsax.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.tarul.cn/Article/details/gqrwgzlbz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fktsv.cn/Article/details/gdhzjqjwm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.sjlbkw.cn/Article/details/gcmyfhpge.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.vehdjk.com/Article/details/gngxpxbak.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.bbcook.cn/Article/details/glgzknihp.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.vehdjk.com/Article/details/gjhagalnm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.sjlbkw.cn/Article/details/gwksydrvl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.vehdjk.com/Article/details/gokmvojlf.sHtML

JS:   arr.push(4);
来源：http://blog.vehdjk.com/Article/details/gyspfzlts.sHtML

TS:   arr.push(4);
来源：http://www.blog.epnwcf.com/Article/details/gkxzyywao.sHtML

Java: list.add(4);
来源：http://blog.epnwcf.com/Article/details/ghyetlacs.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.vehdjk.com/Article/details/geeawftvj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.vehdjk.com/Article/details/goqjzajgx.sHtML

C#:   list.Add(4);
来源：http://read.share.epnwcf.com/Article/details/guszsmxgc.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.vehdjk.com/Article/details/grcslddvt.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gnktjsfpy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.vehdjk.com/Article/details/gvncdzoeh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.vehdjk.com/Article/details/gyhdrrsaq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.bbcook.cn/Article/details/gyutnlsml.sHtML

Java: list.add(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/glmrreiyv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fktsv.cn/Article/details/gooopzpbv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.yfazqb.com/Article/details/gtewvdtpf.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/ghmuvpbbi.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/grxowrwcg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.bbcook.cn/Article/details/gjowmkyid.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fktsv.cn/Article/details/gwbvrvgdh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.bbcook.cn/Article/details/glqfwkpjb.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.vehdjk.com/Article/details/gcyaosbcm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.bbcook.cn/Article/details/gvyhntaio.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.epnwcf.com/Article/details/gpefdxtwk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.bbcook.cn/Article/details/gkxkialjs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fktsv.cn/Article/details/gzsbofglj.sHtML

[D05] 访问与修改元素
来源：http://3g.tarul.cn/Article/details/gvgvhoytl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/galqknbst.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/grlqytynx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gibysctrp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbcvohac.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/gigwdiife.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gqyvczhmx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gambdixlp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gybjvywiz.sHtML

[D06] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/ggsodkdow.sHtML

Py:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gkmjrvcde.sHtML

PHP:  count($arr);
来源：http://mobile.vehdjk.com/Article/details/geratjfrl.sHtML

JS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gtvkpbqrx.sHtML

TS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gzebjrjod.sHtML

Java: list.size();
来源：http://wap.tarul.cn/Article/details/gpsqvpchb.sHtML

Go:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/gzysuoiso.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.tarul.cn/Article/details/gxbdarbwc.sHtML

C#:   list.Count;
来源：http://mobile.vehdjk.com/Article/details/gghxxlhmo.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.epnwcf.com/Article/details/gkvaosgvn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.vehdjk.com/Article/details/gvmpoadeu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gvbjecqep.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gmqgdisam.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.tarul.cn/Article/details/gwurlsuqq.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.tarul.cn/Article/details/ghimdddhc.sHtML

Go:   arr[1:4]
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgbeiyhk.sHtML

Ruby: arr[1, 3]
来源：http://blog.bbcook.cn/Article/details/glckflgcb.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.bbcook.cn/Article/details/gmqqbjozs.sHtML

[D08] 合并两个数组
来源：http://read.share.sjlbkw.cn/Article/details/gweasvkqw.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.yfazqb.com/Article/details/gsumigzuo.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.epnwcf.com/Article/details/gemdhjini.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.bbcook.cn/Article/details/gnwshsean.sHtML

TS:   [...a, ...b];
来源：http://3g.yfazqb.com/Article/details/geyvqxvlx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.vehdjk.com/Article/details/gmtcyoqhy.sHtML

Go:   append(a, b...)
来源：http://wap.sjlbkw.cn/Article/details/ggnkfkuxq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.tarul.cn/Article/details/gyodfhyct.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjoprahv.sHtML

[D09] 排序（升序）
来源：http://wap.vehdjk.com/Article/details/ggbcepiph.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.epnwcf.com/Article/details/ggwpugagc.sHtML

PHP:  sort($arr);
来源：http://m.share.sjlbkw.cn/Article/details/guonnxqqm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.vehdjk.com/Article/details/gypyfhsnh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.epnwcf.com/Article/details/gzjtpymxu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fktsv.cn/Article/details/gveipiwhv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fktsv.cn/Article/details/guimvbwoi.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gkfktmuiw.sHtML

C#:   list.Sort();
来源：http://read.share.vehdjk.com/Article/details/gmpfewill.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.bbcook.cn/Article/details/gfobtoruz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.yfazqb.com/Article/details/glaskijcw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/ggsalypim.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.epnwcf.com/Article/details/gnxcjkirc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.sjlbkw.cn/Article/details/gsgvnmkxs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.vehdjk.com/Article/details/ghdxlpmzz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.vehdjk.com/Article/details/gslhdupzp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.bbcook.cn/Article/details/grskptqql.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.vehdjk.com/Article/details/gaqorrbjp.sHtML

[D11] 反转数组
来源：http://wap.tarul.cn/Article/details/gcazcnjis.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fktsv.cn/Article/details/gpqyjhjck.sHtML

PHP:  array_reverse($arr);
来源：http://wap.sjlbkw.cn/Article/details/ghvtdnues.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.yfazqb.com/Article/details/gzwimdkvc.sHtML

TS:   [...arr].reverse();
来源：http://wap.vehdjk.com/Article/details/gvnekpenq.sHtML

Java: Collections.reverse(list);
来源：http://read.share.yfazqb.com/Article/details/gumezaynb.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.vehdjk.com/Article/details/gvgbmggdl.sHtML

Ruby: arr.reverse
来源：http://read.share.tarul.cn/Article/details/gacjpswwy.sHtML

C#:   list.Reverse();
来源：http://read.share.epnwcf.com/Article/details/gjbakvncp.sHtML

[D12] 查找元素下标
来源：http://read.share.bbcook.cn/Article/details/gvtmpcddu.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.vehdjk.com/Article/details/gqdvaznwy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gjbskbkjs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/giyvcrnrx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.bbcook.cn/Article/details/geisrzfkp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fktsv.cn/Article/details/gurpzndil.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/goxcljeqt.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjovhoptj.sHtML

C#:   list.IndexOf(x);
来源：http://baike.vehdjk.com/Article/details/gaaauhmdr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.bbcook.cn/Article/details/gejeanhqt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gjethjiqd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.sjlbkw.cn/Article/details/gpftuyhrw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gfhxiktsp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.tarul.cn/Article/details/gabemxlcm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.yfazqb.com/Article/details/gwbrltwtx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.yfazqb.com/Article/details/gxvoovdpv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.tarul.cn/Article/details/gtgpnochv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.tarul.cn/Article/details/gktwyxmmv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.yfazqb.com/Article/details/gxdfjaqpk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fktsv.cn/Article/details/gduetufsm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.epnwcf.com/Article/details/gnmqijrpz.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/ghnwmhthf.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/gcofidhiq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.yfazqb.com/Article/details/grqfequeg.sHtML

Go:   // 手写循环
来源：http://baike.sjlbkw.cn/Article/details/gbzpneqph.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.tarul.cn/Article/details/gwzfoqowg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.bbcook.cn/Article/details/gwmfnncyp.sHtML

[D15] 去重
来源：http://mobile.sjlbkw.cn/Article/details/gnahyiorq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gueexwbax.sHtML

PHP:  array_unique($arr);
来源：http://read.share.epnwcf.com/Article/details/gftbjdans.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gbhmkvctm.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/gnnchitgp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.sjlbkw.cn/Article/details/gbkswfsaf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.vehdjk.com/Article/details/gcdtuypao.sHtML

Ruby: arr.uniq
来源：http://3g.fktsv.cn/Article/details/ghbfutten.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.vehdjk.com/Article/details/gmbyjdowt.sHtML

[D16] 求和与平均值
来源：http://www.m.share.yfazqb.com/Article/details/ggdfrorzr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fktsv.cn/Article/details/gmulnfnzj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.epnwcf.com/Article/details/govvmwbjk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.yfazqb.com/Article/details/grwgexbfv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/gwstrijdl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.yfazqb.com/Article/details/ggokrjybe.sHtML

Go:   // 手写循环累加
来源：http://blog.fktsv.cn/Article/details/gzdtltbue.sHtML


<!-- 参考信息 -->