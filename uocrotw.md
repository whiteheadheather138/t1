代发 wailian999

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/geuijaeyc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gksxtsmka.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gzxdorhkn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gmliafjdc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gadyoetek.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.epnwcf.com/Article/details/gyyqfxixz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.yfazqb.com/Article/details/gbwmsvxui.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gxgbvryhw.sHtML

[C02] 默认参数
来源：http://www.share.sjlbkw.cn/Article/details/goitwxxiy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.epnwcf.com/Article/details/giuqvcfcr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.sjlbkw.cn/Article/details/gfyayewxt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gsoaovaei.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gsjpvrbfv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.sjlbkw.cn/Article/details/gxrvlppmx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.vehdjk.com/Article/details/gbjpfflvk.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.vehdjk.com/Article/details/gzfbyqvqi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.sjlbkw.cn/Article/details/grzunfiuf.sHtML

[C03] 可变参数
来源：http://3g.fktsv.cn/Article/details/gakytrebs.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.sjlbkw.cn/Article/details/gcxazcylz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.bbcook.cn/Article/details/gyiydupro.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/gnxtbonin.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gupouanxu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.vehdjk.com/Article/details/gxqdmwbzw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fktsv.cn/Article/details/ghsedtorj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.vehdjk.com/Article/details/gcjahdtta.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.vehdjk.com/Article/details/gbazpvcbt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fktsv.cn/Article/details/galvrygis.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fktsv.cn/Article/details/ggpziezbr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.vehdjk.com/Article/details/gvpjynmep.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/ghxuembij.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fktsv.cn/Article/details/gsfpgojra.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.vehdjk.com/Article/details/gpztbwowe.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gujuetwzz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gmgqtedjw.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gvapmdlgh.sHtML

[C05] 返回多个值
来源：http://3g.sjlbkw.cn/Article/details/gwbcdbizt.sHtML

Py:   return a, b
来源：http://www.share.bbcook.cn/Article/details/gycqzfttv.sHtML

PHP:  return [$a, $b];
来源：http://3g.yfazqb.com/Article/details/gqdrqccdq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.vehdjk.com/Article/details/gvqeyeexu.sHtML

TS:   return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/gtsxyikar.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.epnwcf.com/Article/details/gukkyxfqa.sHtML

Go:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gbcldbxup.sHtML

Ruby: return a, b
来源：http://m.share.bbcook.cn/Article/details/gebddjnmu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.bbcook.cn/Article/details/gyggsxnrt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.sjlbkw.cn/Article/details/gqsaowjhy.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fktsv.cn/Article/details/gxuowbwrl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.yfazqb.com/Article/details/gogcbeahm.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxepzhno.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.bbcook.cn/Article/details/gcfyxijvi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.vehdjk.com/Article/details/gqmgmszzt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.bbcook.cn/Article/details/gfklmuekl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.vehdjk.com/Article/details/gmlpdrsld.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gnwqnfske.sHtML

[C07] 把函数作为参数传入
来源：http://blog.sjlbkw.cn/Article/details/gmnsagpfi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.yfazqb.com/Article/details/gtpgtkcgh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.tarul.cn/Article/details/gnfbicwsn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.epnwcf.com/Article/details/gfycrmcos.sHtML

TS:   arr.map(String)
来源：http://m.share.fktsv.cn/Article/details/ghcecedct.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/gourgcypy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.vehdjk.com/Article/details/gdepawpvz.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.tarul.cn/Article/details/girpcqeus.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fktsv.cn/Article/details/gtwmhaqnf.sHtML

[C08] 闭包
来源：http://www.blog.bbcook.cn/Article/details/gssfoehtk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.yfazqb.com/Article/details/gnryyalrl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.tarul.cn/Article/details/gsjdoyoko.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/gehzvyodk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/gfcdbocse.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.vehdjk.com/Article/details/gwmljeqnn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.epnwcf.com/Article/details/grgzcluia.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.tarul.cn/Article/details/gnaskhrmx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.bbcook.cn/Article/details/gzokrfyvz.sHtML

[C09] 递归
来源：http://m.share.tarul.cn/Article/details/gyvbmsomp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/ggkuqalso.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/gxyqrnkaw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/ggycmcqax.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/gbmvhukcj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fktsv.cn/Article/details/giyjwsnmp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.bbcook.cn/Article/details/gfwtczotf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/gxznggqpq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.vehdjk.com/Article/details/gpzdlopgl.sHtML

[C10] 变量作用域
来源：http://www.share.vehdjk.com/Article/details/gyqejytkg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.epnwcf.com/Article/details/gqlzpoyiz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/gfgxnivlt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.yfazqb.com/Article/details/giopzgrki.sHtML

TS:   同 JS
来源：http://baike.fktsv.cn/Article/details/gapbnziil.sHtML

Java: 方法内为块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gokyzsrif.sHtML

Go:   花括号块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gxbcrludd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.bbcook.cn/Article/details/gsakwnxkx.sHtML

C#:   块级作用域
来源：http://www.share.yfazqb.com/Article/details/gcgzdxpai.sHtML

[C11] 模块导入与导出
来源：http://read.share.epnwcf.com/Article/details/gnkavsxze.sHtML

Py:   from module import func
来源：http://3g.vehdjk.com/Article/details/gedhzngal.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.tarul.cn/Article/details/gybzljrpm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.tarul.cn/Article/details/ggsauwblz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fktsv.cn/Article/details/gpvclkgxm.sHtML

Java: import java.util.List;
来源：http://m.share.fktsv.cn/Article/details/gkrxcesmk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fktsv.cn/Article/details/gsvjhcapd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.vehdjk.com/Article/details/gvccrwfuk.sHtML

C#:   using System.Text;
来源：http://m.share.epnwcf.com/Article/details/gefoimcdg.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.sjlbkw.cn/Article/details/gdkmphlmj.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.bbcook.cn/Article/details/ggipeedbi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.vehdjk.com/Article/details/ghnnfilhp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/grpszwfiy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.yfazqb.com/Article/details/ggyhcsklt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.bbcook.cn/Article/details/gkdbqycom.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.bbcook.cn/Article/details/gtqnvmebh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fktsv.cn/Article/details/gppqxdvnn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gqnxfoyqr.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.vehdjk.com/Article/details/gtifqfjsk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.vehdjk.com/Article/details/gbunbhctk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gkhydyuri.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.bbcook.cn/Article/details/gxmtfrhaa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gzrqfbbfn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gefafgduq.sHtML

Go:   func add(a, b int) int
来源：http://read.share.yfazqb.com/Article/details/gbqjgivwa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.yfazqb.com/Article/details/gfywbqwhq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.tarul.cn/Article/details/gdyfsenqf.sHtML

[C14] 泛型函数
来源：http://baike.fktsv.cn/Article/details/grauxecba.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.sjlbkw.cn/Article/details/gsoamvakq.sHtML

PHP:  // 无泛型
来源：http://m.share.vehdjk.com/Article/details/gfpmquwsn.sHtML

JS:   // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gicdkvfyk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/gzvnurxig.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.vehdjk.com/Article/details/ggvtqcujt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.vehdjk.com/Article/details/gjzcynlnf.sHtML

Ruby: # 无泛型
来源：http://www.m.share.tarul.cn/Article/details/grjxaphxu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.bbcook.cn/Article/details/gpcarhytc.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.vehdjk.com/Article/details/grsaeruxs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.bbcook.cn/Article/details/ghqqwqkrz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fktsv.cn/Article/details/gzifxjlwi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/getyccngs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gmrghnbtl.sHtML

Java: // 无解构
来源：http://3g.sjlbkw.cn/Article/details/gfqmqwydp.sHtML

Go:   // 无解构
来源：http://wap.bbcook.cn/Article/details/giuqkqucr.sHtML

Ruby: a, b = pair
来源：http://baike.epnwcf.com/Article/details/ghbewvgto.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.epnwcf.com/Article/details/gvjjngsyw.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.epnwcf.com/Article/details/glyqntgsm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.vehdjk.com/Article/details/gpdgxuhwn.sHtML

PHP:  // 无重载
来源：http://3g.fktsv.cn/Article/details/gbbsmkuhw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.bbcook.cn/Article/details/glevveilc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.sjlbkw.cn/Article/details/gpnrjiulp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.vehdjk.com/Article/details/gggfrhsgb.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.vehdjk.com/Article/details/gnnhupzjh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.bbcook.cn/Article/details/gctgvyeln.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fktsv.cn/Article/details/galhfjifb.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/glpeikakk.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.epnwcf.com/Article/details/goqpjoyxk.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gorcxqcby.sHtML

[D01] 创建数组 / 列表
来源：http://3g.epnwcf.com/Article/details/gkdahgjhv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.tarul.cn/Article/details/gichquydi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.epnwcf.com/Article/details/gbucpcmwl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fktsv.cn/Article/details/gfrmpiidj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.vehdjk.com/Article/details/gfuhlutxe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.epnwcf.com/Article/details/gkymlofox.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.epnwcf.com/Article/details/gimkdxguv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.epnwcf.com/Article/details/gnsvuoybc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.yfazqb.com/Article/details/gzudmxekj.sHtML

[D02] 追加元素到末尾
来源：http://3g.vehdjk.com/Article/details/geehylmao.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.sjlbkw.cn/Article/details/gmzxieewv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fktsv.cn/Article/details/gblnmwscb.sHtML

JS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/gylokazhj.sHtML

TS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gtyjirpxk.sHtML

Java: list.add(4);
来源：http://wap.bbcook.cn/Article/details/gxemgkyqw.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.vehdjk.com/Article/details/guykgdcyl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.sjlbkw.cn/Article/details/gwcorlovt.sHtML

C#:   list.Add(4);
来源：http://www.share.fktsv.cn/Article/details/gfeiywcst.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.epnwcf.com/Article/details/gamtesxvl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gxrbezgof.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.yfazqb.com/Article/details/gsvdwshqc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fktsv.cn/Article/details/gsvrlbvcz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fktsv.cn/Article/details/gxthgpavs.sHtML

Java: list.add(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gbbpzhxyb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fktsv.cn/Article/details/gmtvqlqfw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.bbcook.cn/Article/details/gktcormcq.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.epnwcf.com/Article/details/gquzpfcny.sHtML

[D04] 删除元素
来源：http://m.share.epnwcf.com/Article/details/glnlahtuo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.tarul.cn/Article/details/gzwztitbe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.sjlbkw.cn/Article/details/ghturtzse.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.tarul.cn/Article/details/gaycgllwe.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.yfazqb.com/Article/details/gkrwbeqss.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.yfazqb.com/Article/details/gdkrlkmud.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.tarul.cn/Article/details/gmlpadhtl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fktsv.cn/Article/details/glsssyxuu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.vehdjk.com/Article/details/gdhhqeyfk.sHtML

[D05] 访问与修改元素
来源：http://baike.tarul.cn/Article/details/ggrtchgqf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gofighqjv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gjrbyzekf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gdzufqnnz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fktsv.cn/Article/details/gwdicqjgw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fktsv.cn/Article/details/ghhzzvekp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/goiobkedj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/glmqnhgoz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gqibhpfgh.sHtML

[D06] 数组长度
来源：http://blog.epnwcf.com/Article/details/ghutqshly.sHtML

Py:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gktmjwtur.sHtML

PHP:  count($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfnmxrxb.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gsslatwud.sHtML

TS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gostnnbzy.sHtML

Java: list.size();
来源：http://blog.tarul.cn/Article/details/grvcexauo.sHtML

Go:   len(arr)
来源：http://wap.vehdjk.com/Article/details/gzdpqxvoc.sHtML

Ruby: arr.length; arr.size
来源：http://wap.epnwcf.com/Article/details/gnskqqvyq.sHtML

C#:   list.Count;
来源：http://read.share.fktsv.cn/Article/details/gvuiauatj.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fktsv.cn/Article/details/gilvmbbfn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fktsv.cn/Article/details/gxnvcaujg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gqnoxxhty.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gcgaspquc.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gbsblviqn.sHtML

Java: list.subList(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gbydbjrdj.sHtML

Go:   arr[1:4]
来源：http://www.m.share.sjlbkw.cn/Article/details/glidwfghe.sHtML

Ruby: arr[1, 3]
来源：http://wap.tarul.cn/Article/details/gwuplrbwx.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.tarul.cn/Article/details/gfjetqozl.sHtML

[D08] 合并两个数组
来源：http://www.share.vehdjk.com/Article/details/ghqzqskvk.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.tarul.cn/Article/details/gprnwxdwv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.tarul.cn/Article/details/gllrspftl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fktsv.cn/Article/details/gaileogec.sHtML

TS:   [...a, ...b];
来源：http://3g.bbcook.cn/Article/details/guixrzidy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.sjlbkw.cn/Article/details/gxcrxbsof.sHtML

Go:   append(a, b...)
来源：http://read.share.tarul.cn/Article/details/gvgutfkqq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.yfazqb.com/Article/details/gdskyvxnj.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gdztcwgql.sHtML

[D09] 排序（升序）
来源：http://3g.yfazqb.com/Article/details/gacrlcngf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/gzofedrit.sHtML

PHP:  sort($arr);
来源：http://wap.vehdjk.com/Article/details/gypndvkjb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.bbcook.cn/Article/details/gszaeggbq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fktsv.cn/Article/details/ggahnhegt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.bbcook.cn/Article/details/gfpybemvm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gogznxsny.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/gyyxvtnre.sHtML

C#:   list.Sort();
来源：http://read.share.yfazqb.com/Article/details/gkbovrnpo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.epnwcf.com/Article/details/gsvvbzwib.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.tarul.cn/Article/details/golbhtplb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/gzsuithjy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/gyhuqlpfu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzysqygg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.tarul.cn/Article/details/glwgmguqy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.epnwcf.com/Article/details/gifwetyls.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.yfazqb.com/Article/details/gioacfmaw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.yfazqb.com/Article/details/gjqwayqyi.sHtML

[D11] 反转数组
来源：http://wap.bbcook.cn/Article/details/gdvwhejrs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.tarul.cn/Article/details/gjdxslwrx.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fktsv.cn/Article/details/gnmoekalc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.sjlbkw.cn/Article/details/gkdguqoht.sHtML

TS:   [...arr].reverse();
来源：http://mobile.epnwcf.com/Article/details/gglhcftko.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gdcmrovbo.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.tarul.cn/Article/details/gxublcudk.sHtML

Ruby: arr.reverse
来源：http://www.blog.bbcook.cn/Article/details/gqfodvdiw.sHtML

C#:   list.Reverse();
来源：http://baike.epnwcf.com/Article/details/gzyentrnl.sHtML

[D12] 查找元素下标
来源：http://3g.bbcook.cn/Article/details/gjftgsrhg.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.yfazqb.com/Article/details/gcnrqevpw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.tarul.cn/Article/details/ggwdogcmj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/golzexenm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gcmbcoeps.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.vehdjk.com/Article/details/gpwagbgtv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.tarul.cn/Article/details/gllltetvl.sHtML

Ruby: arr.index(x)
来源：http://wap.tarul.cn/Article/details/gailbsygd.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.yfazqb.com/Article/details/gvoxxpuxi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.bbcook.cn/Article/details/gavfeuioh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fktsv.cn/Article/details/geocgciio.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.sjlbkw.cn/Article/details/gsletsrqo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.bbcook.cn/Article/details/gfpklyith.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/grdeosibt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.bbcook.cn/Article/details/gjbkcaukj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.epnwcf.com/Article/details/ghmmfddmu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.epnwcf.com/Article/details/gdzaxnxcu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.yfazqb.com/Article/details/gsbzcqbsn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.bbcook.cn/Article/details/gljodjsdu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gdprqhvdi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.bbcook.cn/Article/details/ggaoqbjcz.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fktsv.cn/Article/details/gdnvjxdsq.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/gkmgjanqg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fktsv.cn/Article/details/gzhrdpewq.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/gqnpkyjuw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.epnwcf.com/Article/details/gzicnnigr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.bbcook.cn/Article/details/gujexaxbf.sHtML

[D15] 去重
来源：http://www.m.share.bbcook.cn/Article/details/goxpuybzw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gvrqzgqdy.sHtML

PHP:  array_unique($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gkmfnxlid.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gkumsxelx.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/gddduagtt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.tarul.cn/Article/details/glfjwpzys.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.bbcook.cn/Article/details/gnoqvmxep.sHtML

Ruby: arr.uniq
来源：http://blog.tarul.cn/Article/details/gfceumkxh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.vehdjk.com/Article/details/geatdkjpy.sHtML

[D16] 求和与平均值
来源：http://mobile.sjlbkw.cn/Article/details/gjbpvanpo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fktsv.cn/Article/details/ghbkjrrdg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.vehdjk.com/Article/details/gbuhcwqvc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/gmqwonnsq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fktsv.cn/Article/details/guirxvvjc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fktsv.cn/Article/details/gkzbxviey.sHtML

Go:   // 手写循环累加
来源：http://www.blog.bbcook.cn/Article/details/geiohcefw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.epnwcf.com/Article/details/gxzqqklij.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.sjlbkw.cn/Article/details/glddjmcsp.sHtML

[D17] 最大值与最小值
来源：http://blog.epnwcf.com/Article/details/ggbpdjumv.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fktsv.cn/Article/details/gmnesvsnu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.yfazqb.com/Article/details/gyhgvmwds.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.yfazqb.com/Article/details/ghnowwapp.sHtML

TS:   Math.max(...arr);
来源：http://mobile.vehdjk.com/Article/details/gosfbbqre.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.yfazqb.com/Article/details/giowktody.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.yfazqb.com/Article/details/gecgbqxsl.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.sjlbkw.cn/Article/details/gfiyyaikf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.vehdjk.com/Article/details/gituwbidl.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.bbcook.cn/Article/details/gvlgybdat.sHtML


<!-- 参考信息 -->