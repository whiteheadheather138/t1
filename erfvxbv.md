代发 wailian999

Py:   def add(a, b): return a + b
来源：http://wap.bbcook.cn/Article/details/gajawhipc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gzcxocqbe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/guwdybmok.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gasetevrt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/ginddgavo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.vehdjk.com/Article/details/ghngakwak.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.vehdjk.com/Article/details/gbvtpfjcm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gdjvmsauo.sHtML

[C02] 默认参数
来源：http://mobile.bbcook.cn/Article/details/gznocgmye.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.vehdjk.com/Article/details/gepqzjbup.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.tarul.cn/Article/details/gwfrioeex.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gvpmgzjpd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.yfazqb.com/Article/details/gbsztjpgu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.bbcook.cn/Article/details/gvwcpvwur.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.tarul.cn/Article/details/gedxzgart.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.bbcook.cn/Article/details/grliwrwib.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.tarul.cn/Article/details/gsyeunfrk.sHtML

[C03] 可变参数
来源：http://baike.sjlbkw.cn/Article/details/gucpwgyyb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/gdwedtqfr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.vehdjk.com/Article/details/gqankgyck.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fktsv.cn/Article/details/gpiuzhjlp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsjfxgaq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.tarul.cn/Article/details/gxvxcgmtm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.bbcook.cn/Article/details/gscwtjhec.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fktsv.cn/Article/details/gmwpxpuho.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.bbcook.cn/Article/details/ghhsmbwdk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fktsv.cn/Article/details/gjsegiqnt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.yfazqb.com/Article/details/gexquktmw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.bbcook.cn/Article/details/gttymdjxz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.vehdjk.com/Article/details/gcfipoouz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.sjlbkw.cn/Article/details/gbpimtmiu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.bbcook.cn/Article/details/gmhlpabnm.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.yfazqb.com/Article/details/gnmkybush.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gdkfowcin.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gugphhbax.sHtML

[C05] 返回多个值
来源：http://m.share.vehdjk.com/Article/details/gakffxsks.sHtML

Py:   return a, b
来源：http://blog.yfazqb.com/Article/details/ghzwysoiu.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.tarul.cn/Article/details/gwmhdrsfx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gbnrxgwtv.sHtML

TS:   return { a, b };
来源：http://baike.tarul.cn/Article/details/gmhqlmjfi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.tarul.cn/Article/details/gbxdkdspi.sHtML

Go:   return a, b
来源：http://blog.fktsv.cn/Article/details/guvkonvrg.sHtML

Ruby: return a, b
来源：http://mobile.vehdjk.com/Article/details/gkkkrlsku.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpcgdhrh.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.yfazqb.com/Article/details/gseiwxnqs.sHtML

Py:   square = lambda x: x * x
来源：http://baike.vehdjk.com/Article/details/ghcfxgoju.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.yfazqb.com/Article/details/goulajeme.sHtML

JS:   const square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/gerilqqyk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gxqmkyagy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.tarul.cn/Article/details/gvqpptkid.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.yfazqb.com/Article/details/gibmoitxk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.epnwcf.com/Article/details/gprampnwq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gmzhjjnmj.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.sjlbkw.cn/Article/details/goalzmgpj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.yfazqb.com/Article/details/guflcdqij.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gcpvdfixv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.tarul.cn/Article/details/goezuukxk.sHtML

TS:   arr.map(String)
来源：http://www.blog.fktsv.cn/Article/details/gcaduurht.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/gojndtxme.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.bbcook.cn/Article/details/gwpjihedb.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.bbcook.cn/Article/details/gecvkaxeo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.sjlbkw.cn/Article/details/gvbiogdzj.sHtML

[C08] 闭包
来源：http://wap.vehdjk.com/Article/details/gbuqhqafh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fktsv.cn/Article/details/gzgoatllk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.bbcook.cn/Article/details/gftlkkodt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gqnfilalt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gjuzhrqge.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.epnwcf.com/Article/details/guvqklolz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.tarul.cn/Article/details/gyecpriht.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fktsv.cn/Article/details/gwvgovclr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/ghwqqzldf.sHtML

[C09] 递归
来源：http://3g.fktsv.cn/Article/details/ggoqvocjf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gtbpoxnog.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/gizzpvxcq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.yfazqb.com/Article/details/gkevxltis.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.bbcook.cn/Article/details/gucutshlr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.bbcook.cn/Article/details/gvyhftwqb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fktsv.cn/Article/details/gujxmojts.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/grpxnllns.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.vehdjk.com/Article/details/gctjtooco.sHtML

[C10] 变量作用域
来源：http://3g.tarul.cn/Article/details/gwnqldewd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.yfazqb.com/Article/details/gzbcqgudv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.yfazqb.com/Article/details/gcnwsxilb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/glmlrotjd.sHtML

TS:   同 JS
来源：http://3g.sjlbkw.cn/Article/details/gkdqtcfyh.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gukmdilgr.sHtML

Go:   花括号块级作用域
来源：http://baike.tarul.cn/Article/details/gjwmjxogo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.vehdjk.com/Article/details/gbqbxiyip.sHtML

C#:   块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gtmwfvbzs.sHtML

[C11] 模块导入与导出
来源：http://www.blog.epnwcf.com/Article/details/gactdtmsj.sHtML

Py:   from module import func
来源：http://read.share.fktsv.cn/Article/details/grkfvmrwu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.epnwcf.com/Article/details/ghvglrclf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.bbcook.cn/Article/details/gifpyqqsa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.epnwcf.com/Article/details/gcjskutuk.sHtML

Java: import java.util.List;
来源：http://m.share.fktsv.cn/Article/details/gbybyzycc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.epnwcf.com/Article/details/gfditcrkt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.sjlbkw.cn/Article/details/ggdkpktnx.sHtML

C#:   using System.Text;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxydujvlb.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.yfazqb.com/Article/details/gfobugtvz.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fktsv.cn/Article/details/gssusbevm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.sjlbkw.cn/Article/details/gbtkqfgup.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/gaybiurqz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gteedzbzy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.bbcook.cn/Article/details/gjmvuhbwq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.tarul.cn/Article/details/gcifdeyof.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.sjlbkw.cn/Article/details/gzovedagp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gpvektqrb.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fktsv.cn/Article/details/gtxbrhzhl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.bbcook.cn/Article/details/gkgvktevl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gfwblcktf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.sjlbkw.cn/Article/details/gzwfslpzu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/ggvhppmbe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/glyufwnnf.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fktsv.cn/Article/details/gkgopxcgg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.yfazqb.com/Article/details/gzklbozdt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.vehdjk.com/Article/details/ggskphlim.sHtML

[C14] 泛型函数
来源：http://blog.epnwcf.com/Article/details/gbqfzgzmo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.epnwcf.com/Article/details/glidzrduy.sHtML

PHP:  // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gtiyskxmd.sHtML

JS:   // 无泛型
来源：http://m.share.tarul.cn/Article/details/gluimlpvp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fktsv.cn/Article/details/gbceaulql.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.bbcook.cn/Article/details/gubljwiph.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.epnwcf.com/Article/details/gmwynsryj.sHtML

Ruby: # 无泛型
来源：http://baike.bbcook.cn/Article/details/gpoyclthd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.sjlbkw.cn/Article/details/gqcmkanou.sHtML

[C15] 解构 / 展开参数
来源：http://3g.tarul.cn/Article/details/grbieewwb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.epnwcf.com/Article/details/godezplkn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.bbcook.cn/Article/details/gtyqcpoat.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gjdqcsisi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.bbcook.cn/Article/details/ggfdwdczn.sHtML

Java: // 无解构
来源：http://read.share.yfazqb.com/Article/details/gsvdihekl.sHtML

Go:   // 无解构
来源：http://read.share.epnwcf.com/Article/details/gfujmyxds.sHtML

Ruby: a, b = pair
来源：http://baike.fktsv.cn/Article/details/glmayfsuk.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.bbcook.cn/Article/details/gdozisewd.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fktsv.cn/Article/details/guklxvxye.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.vehdjk.com/Article/details/gabnmuvuc.sHtML

PHP:  // 无重载
来源：http://baike.vehdjk.com/Article/details/gmsqouhoh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.tarul.cn/Article/details/gtazbrawb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gimlahvjo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fktsv.cn/Article/details/grbnupgwn.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.bbcook.cn/Article/details/guzofpahg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.epnwcf.com/Article/details/gijgixfet.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.tarul.cn/Article/details/gunbexiuz.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gwyjvewdz.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.vehdjk.com/Article/details/ghwbcmrdt.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gajleyhaz.sHtML

[D01] 创建数组 / 列表
来源：http://blog.yfazqb.com/Article/details/gedjvtaep.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.epnwcf.com/Article/details/grrujzmgc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.tarul.cn/Article/details/gfujkrvfh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.tarul.cn/Article/details/gdlogkvca.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.sjlbkw.cn/Article/details/gwqozrksx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.epnwcf.com/Article/details/gberbnhrx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.yfazqb.com/Article/details/gujgvlwsd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.yfazqb.com/Article/details/gymiejubn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.vehdjk.com/Article/details/grlnlisbv.sHtML

[D02] 追加元素到末尾
来源：http://blog.fktsv.cn/Article/details/gwlcvqaol.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.vehdjk.com/Article/details/gjrjmpxak.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.yfazqb.com/Article/details/gwbkovggw.sHtML

JS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/gvhbiuuox.sHtML

TS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/gyqfhhysh.sHtML

Java: list.add(4);
来源：http://wap.yfazqb.com/Article/details/gryywxyng.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.tarul.cn/Article/details/ghhtzmvew.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrrvzubc.sHtML

C#:   list.Add(4);
来源：http://www.blog.epnwcf.com/Article/details/ghapipwav.sHtML

[D03] 在指定位置插入元素
来源：http://baike.vehdjk.com/Article/details/genootubz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fktsv.cn/Article/details/grzdzlodq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.tarul.cn/Article/details/gyzszfrft.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.sjlbkw.cn/Article/details/gsaribxfy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fktsv.cn/Article/details/gsnirkqez.sHtML

Java: list.add(0, 0);
来源：http://wap.tarul.cn/Article/details/gjnlavxbu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.epnwcf.com/Article/details/gyfbxwgas.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.tarul.cn/Article/details/gsqoqszzg.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fktsv.cn/Article/details/gzjnruavg.sHtML

[D04] 删除元素
来源：http://wap.sjlbkw.cn/Article/details/ginkcqttc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.epnwcf.com/Article/details/gabumjnjg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.bbcook.cn/Article/details/ghfmdqzma.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.bbcook.cn/Article/details/gtoswzjax.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.sjlbkw.cn/Article/details/gfpbxcwcx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhtnoocx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.epnwcf.com/Article/details/godymrxko.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.bbcook.cn/Article/details/ghzmdmsmw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.vehdjk.com/Article/details/gmrchodmz.sHtML

[D05] 访问与修改元素
来源：http://3g.epnwcf.com/Article/details/gqrnlyymt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gcilzbktw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gwdzqhjwm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gkeorrxot.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.tarul.cn/Article/details/gmzkojwji.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.yfazqb.com/Article/details/gcwyvnxqf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/geemnagjf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/guweurgdw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/ggkrnhsmv.sHtML

[D06] 数组长度
来源：http://baike.yfazqb.com/Article/details/goerrfped.sHtML

Py:   len(arr)
来源：http://wap.fktsv.cn/Article/details/gcodduwaj.sHtML

PHP:  count($arr);
来源：http://blog.fktsv.cn/Article/details/grpkdjfhc.sHtML

JS:   arr.length
来源：http://www.m.share.bbcook.cn/Article/details/gsyvewwcu.sHtML

TS:   arr.length
来源：http://wap.tarul.cn/Article/details/gnythndoj.sHtML

Java: list.size();
来源：http://m.share.fktsv.cn/Article/details/gtvkrqdbz.sHtML

Go:   len(arr)
来源：http://3g.vehdjk.com/Article/details/gqxdlkerp.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fktsv.cn/Article/details/ggmcqhvlv.sHtML

C#:   list.Count;
来源：http://mobile.epnwcf.com/Article/details/gijsbxmzi.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.vehdjk.com/Article/details/gnnzblgaz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fktsv.cn/Article/details/gwrvzrkeh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.vehdjk.com/Article/details/geaxrkdvr.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gfqnfcehs.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gfvrrfxap.sHtML

Java: list.subList(1, 4);
来源：http://baike.tarul.cn/Article/details/gsjyclmbd.sHtML

Go:   arr[1:4]
来源：http://www.m.share.vehdjk.com/Article/details/grvvjemtn.sHtML

Ruby: arr[1, 3]
来源：http://baike.fktsv.cn/Article/details/gsphxfher.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.vehdjk.com/Article/details/gqjpzkktu.sHtML

[D08] 合并两个数组
来源：http://3g.epnwcf.com/Article/details/gnhsnyiqx.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.tarul.cn/Article/details/gkpzxmzyj.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.sjlbkw.cn/Article/details/gnjpeidbj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.tarul.cn/Article/details/ghivhqvol.sHtML

TS:   [...a, ...b];
来源：http://read.share.yfazqb.com/Article/details/gfphauhnk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.sjlbkw.cn/Article/details/gchyysbbv.sHtML

Go:   append(a, b...)
来源：http://mobile.epnwcf.com/Article/details/gonigluep.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.tarul.cn/Article/details/gkxozsdhj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.yfazqb.com/Article/details/grnhqipzx.sHtML

[D09] 排序（升序）
来源：http://3g.epnwcf.com/Article/details/gwwmkhbaa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/gzxgvelyo.sHtML

PHP:  sort($arr);
来源：http://www.share.yfazqb.com/Article/details/gvsuftmav.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fktsv.cn/Article/details/gxwpholcu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fktsv.cn/Article/details/gztjcdpoo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.yfazqb.com/Article/details/ggqknybqw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gaaskutpe.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/glhjybjcp.sHtML

C#:   list.Sort();
来源：http://3g.sjlbkw.cn/Article/details/gvwjtugip.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fktsv.cn/Article/details/gighasnfl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.tarul.cn/Article/details/gdosizlfr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmgzifet.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.vehdjk.com/Article/details/gglvdosqb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/ggyhdhhpk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.vehdjk.com/Article/details/glzpjanoe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.epnwcf.com/Article/details/gwxsnkwxw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.bbcook.cn/Article/details/gnsrmukzs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.tarul.cn/Article/details/gcazqvtmg.sHtML

[D11] 反转数组
来源：http://m.share.tarul.cn/Article/details/gzgobeguw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fktsv.cn/Article/details/gonrspwpc.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fktsv.cn/Article/details/grbabdzxl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.yfazqb.com/Article/details/gnmxffuba.sHtML

TS:   [...arr].reverse();
来源：http://blog.fktsv.cn/Article/details/glejmodil.sHtML

Java: Collections.reverse(list);
来源：http://blog.sjlbkw.cn/Article/details/gmkhlvknd.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.tarul.cn/Article/details/gkhbirgxp.sHtML

Ruby: arr.reverse
来源：http://3g.bbcook.cn/Article/details/gjkmybmxp.sHtML

C#:   list.Reverse();
来源：http://m.share.yfazqb.com/Article/details/gbmmlxukd.sHtML

[D12] 查找元素下标
来源：http://read.share.sjlbkw.cn/Article/details/gjhqerkin.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.vehdjk.com/Article/details/gpwrwqkce.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fktsv.cn/Article/details/grsvlaioq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.bbcook.cn/Article/details/golyegcrl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/gwrttuxsp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.bbcook.cn/Article/details/gobfbsdim.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/giqdzouhh.sHtML

Ruby: arr.index(x)
来源：http://3g.yfazqb.com/Article/details/gjhfuzrap.sHtML

C#:   list.IndexOf(x);
来源：http://baike.yfazqb.com/Article/details/gmliixfcu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.epnwcf.com/Article/details/gwamignwm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.bbcook.cn/Article/details/gspzbaqsp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.epnwcf.com/Article/details/gbvufxpnt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.sjlbkw.cn/Article/details/gcafqloek.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/gjxluloot.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gnheazuar.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fktsv.cn/Article/details/gftyhfuqb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.epnwcf.com/Article/details/geklkatqr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fktsv.cn/Article/details/gwaqrmehc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.yfazqb.com/Article/details/gkkdcldxc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.epnwcf.com/Article/details/gkzegvwmn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.yfazqb.com/Article/details/gaaoqeadk.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fktsv.cn/Article/details/gkegxdatj.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gfaerxqwo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.vehdjk.com/Article/details/gdsdcmpbl.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/gavebdemg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/goszzmkvs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gmfefbxto.sHtML

[D15] 去重
来源：http://read.share.epnwcf.com/Article/details/gcvlswoyf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gtjrudzig.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/gxfygdqob.sHtML

JS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gfexgppwo.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/gooeirula.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.tarul.cn/Article/details/gdmgqtqwa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fktsv.cn/Article/details/gjkgrryhw.sHtML

Ruby: arr.uniq
来源：http://www.share.epnwcf.com/Article/details/gocecozrr.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gwacmlrhg.sHtML

[D16] 求和与平均值
来源：http://m.share.bbcook.cn/Article/details/geserryyu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fktsv.cn/Article/details/gxkrmlauu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.vehdjk.com/Article/details/gouknczxc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gccdodlvu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/ghvyyzdch.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.sjlbkw.cn/Article/details/geoopwvat.sHtML

Go:   // 手写循环累加
来源：http://mobile.vehdjk.com/Article/details/guyxzxyqx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.yfazqb.com/Article/details/gxmijhtpm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.vehdjk.com/Article/details/ggcblpvhn.sHtML

[D17] 最大值与最小值
来源：http://www.blog.epnwcf.com/Article/details/gahadthur.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.vehdjk.com/Article/details/garqnjnfl.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.epnwcf.com/Article/details/grgkwkwmk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.sjlbkw.cn/Article/details/gpzivcybz.sHtML

TS:   Math.max(...arr);
来源：http://read.share.vehdjk.com/Article/details/gtjdiitym.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.sjlbkw.cn/Article/details/gxxrmdgox.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.yfazqb.com/Article/details/gjudmlemq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.tarul.cn/Article/details/gjkmtvqkn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.yfazqb.com/Article/details/geaelqfxo.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.bbcook.cn/Article/details/gaqelcdvl.sHtML


<!-- 参考信息 -->