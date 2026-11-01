代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/glxskjbhj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.epnwcf.com/Article/details/gdhukmiiz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.vehdjk.com/Article/details/gsnsxvfge.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/ggetkwxhj.sHtML

[C02] 默认参数
来源：http://m.share.vehdjk.com/Article/details/gbqlgkadr.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.epnwcf.com/Article/details/giaouwwxb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.vehdjk.com/Article/details/gxhdqpgum.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gwrnsxhhq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.vehdjk.com/Article/details/gjblctrzv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.yfazqb.com/Article/details/gadwldihc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.tarul.cn/Article/details/guclhthii.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fktsv.cn/Article/details/ggsvztyix.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.sjlbkw.cn/Article/details/gmbkjndwh.sHtML

[C03] 可变参数
来源：http://mobile.sjlbkw.cn/Article/details/gacxzxecw.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.yfazqb.com/Article/details/gnknznnuy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.bbcook.cn/Article/details/grauasqom.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/gsoymxbak.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gmsmfvdis.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.epnwcf.com/Article/details/gblhwyelt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.bbcook.cn/Article/details/ghtpazsbu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.yfazqb.com/Article/details/gtxmflegh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fktsv.cn/Article/details/gkhdmwxaz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fktsv.cn/Article/details/ggdcgyvtw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.epnwcf.com/Article/details/galszdcxg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.yfazqb.com/Article/details/gsfbmjghj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fktsv.cn/Article/details/gqdmxtfba.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.tarul.cn/Article/details/gptrsixev.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.vehdjk.com/Article/details/gttzymscq.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.vehdjk.com/Article/details/gmyzfkfrz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gsxhhqyor.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/ghlwidvci.sHtML

[C05] 返回多个值
来源：http://m.share.epnwcf.com/Article/details/gbryenlfi.sHtML

Py:   return a, b
来源：http://baike.bbcook.cn/Article/details/gkibbpyjy.sHtML

PHP:  return [$a, $b];
来源：http://www.share.vehdjk.com/Article/details/gwbsnlkhy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gpdllxmhp.sHtML

TS:   return { a, b };
来源：http://3g.fktsv.cn/Article/details/gegiwsjiy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.yfazqb.com/Article/details/ggjsiceod.sHtML

Go:   return a, b
来源：http://3g.fktsv.cn/Article/details/gvspkdrtf.sHtML

Ruby: return a, b
来源：http://3g.fktsv.cn/Article/details/gyurdegfj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.sjlbkw.cn/Article/details/gyfxsraji.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.vehdjk.com/Article/details/gdorsuuwd.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.tarul.cn/Article/details/gajwnnmrb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.epnwcf.com/Article/details/gaxeafxwx.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gbpwpnrmt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.bbcook.cn/Article/details/gwbufqfyy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.bbcook.cn/Article/details/gidsxjnpe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.sjlbkw.cn/Article/details/gjrvxabbh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.bbcook.cn/Article/details/gpzbfoqna.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gafqrwory.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.epnwcf.com/Article/details/gtroaeyvm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fktsv.cn/Article/details/gnodrfxvl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.epnwcf.com/Article/details/gykdcngsl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.bbcook.cn/Article/details/grsgwodfb.sHtML

TS:   arr.map(String)
来源：http://www.share.sjlbkw.cn/Article/details/ggglkckgv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.sjlbkw.cn/Article/details/gzbeweadz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fktsv.cn/Article/details/gjoxnnbuu.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.yfazqb.com/Article/details/gmrpfxqlx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fktsv.cn/Article/details/gtuwbkgkg.sHtML

[C08] 闭包
来源：http://m.share.yfazqb.com/Article/details/girelxrkq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrxjnboj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.tarul.cn/Article/details/gczlcnsui.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gxgyiecxz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gjdkogpmw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.bbcook.cn/Article/details/gtckriolq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.bbcook.cn/Article/details/gnxbmxctz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.sjlbkw.cn/Article/details/gmepszpfu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gbfgprubv.sHtML

[C09] 递归
来源：http://read.share.fktsv.cn/Article/details/gqxmnjiww.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fktsv.cn/Article/details/gscscmjiv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.vehdjk.com/Article/details/godljmknz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gfywhbfis.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fktsv.cn/Article/details/gdiucjsmv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fktsv.cn/Article/details/glqislxfa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fktsv.cn/Article/details/gajudbxhy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/gwudpgfjf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.vehdjk.com/Article/details/gkxlvfqpi.sHtML

[C10] 变量作用域
来源：http://www.blog.tarul.cn/Article/details/gvroirgne.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.tarul.cn/Article/details/gzjkmqjid.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fktsv.cn/Article/details/gmzctgmyt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.sjlbkw.cn/Article/details/glukhkkob.sHtML

TS:   同 JS
来源：http://www.blog.tarul.cn/Article/details/guutklwbz.sHtML

Java: 方法内为块级作用域
来源：http://blog.epnwcf.com/Article/details/ggzgvvmsu.sHtML

Go:   花括号块级作用域
来源：http://3g.fktsv.cn/Article/details/gzvmdiify.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.yfazqb.com/Article/details/gwkqcesbb.sHtML

C#:   块级作用域
来源：http://wap.vehdjk.com/Article/details/gsfzsrohw.sHtML

[C11] 模块导入与导出
来源：http://read.share.fktsv.cn/Article/details/gtxgbwghf.sHtML

Py:   from module import func
来源：http://3g.sjlbkw.cn/Article/details/gjchtigzx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.yfazqb.com/Article/details/gnktgkgtk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/gzvsinmni.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.yfazqb.com/Article/details/gfojncunr.sHtML

Java: import java.util.List;
来源：http://www.blog.yfazqb.com/Article/details/grsrgjoge.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fktsv.cn/Article/details/gbfgvzrbd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.bbcook.cn/Article/details/gczuygusu.sHtML

C#:   using System.Text;
来源：http://www.share.bbcook.cn/Article/details/gmgzvmokh.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.tarul.cn/Article/details/gpguemrvg.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.sjlbkw.cn/Article/details/gqrcozoyx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fktsv.cn/Article/details/gvfmrqrod.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gnmyvmaeb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fktsv.cn/Article/details/ggkzijvia.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fktsv.cn/Article/details/ghhbpdzgw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.tarul.cn/Article/details/gxvkypqww.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.tarul.cn/Article/details/ggkizdvno.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.epnwcf.com/Article/details/gvumnqxgr.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.bbcook.cn/Article/details/grcgacdxb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.vehdjk.com/Article/details/glblnrtwf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gelnqkidh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fktsv.cn/Article/details/gsujzjkzv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gruhxxjwv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/geqdbbuoe.sHtML

Go:   func add(a, b int) int
来源：http://read.share.sjlbkw.cn/Article/details/gysodfwgc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.yfazqb.com/Article/details/gmgsifkvp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.epnwcf.com/Article/details/gsehaahyy.sHtML

[C14] 泛型函数
来源：http://www.blog.vehdjk.com/Article/details/girhtltcj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fktsv.cn/Article/details/ggsfvwlff.sHtML

PHP:  // 无泛型
来源：http://blog.tarul.cn/Article/details/gkmwokumn.sHtML

JS:   // 无泛型
来源：http://blog.epnwcf.com/Article/details/gskgfhwwo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.bbcook.cn/Article/details/gvaanoqfw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.epnwcf.com/Article/details/gjqphucnn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fktsv.cn/Article/details/ggputtzcp.sHtML

Ruby: # 无泛型
来源：http://m.share.tarul.cn/Article/details/gucsjzmgp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.vehdjk.com/Article/details/gvsaxjtmc.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.sjlbkw.cn/Article/details/gjkhuodoe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fktsv.cn/Article/details/gbrhiimpa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.vehdjk.com/Article/details/ggejfbghy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/geyyoomnz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.tarul.cn/Article/details/gczxjwclb.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/gvvkjtsaz.sHtML

Go:   // 无解构
来源：http://m.share.fktsv.cn/Article/details/gdieoncgl.sHtML

Ruby: a, b = pair
来源：http://wap.sjlbkw.cn/Article/details/ghlrvcovp.sHtML

C#:   var (a, b) = pair;
来源：http://baike.yfazqb.com/Article/details/grdksuxlt.sHtML

[C16] 函数 / 方法重载
来源：http://3g.yfazqb.com/Article/details/ghspdjcbx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fktsv.cn/Article/details/gcelsiuoe.sHtML

PHP:  // 无重载
来源：http://www.m.share.bbcook.cn/Article/details/ginnlyyms.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.yfazqb.com/Article/details/gnashidlk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.sjlbkw.cn/Article/details/gtmsdsdqp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.bbcook.cn/Article/details/gjtlsisvm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.tarul.cn/Article/details/gkbceaeur.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.bbcook.cn/Article/details/gczgjechh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.bbcook.cn/Article/details/gqzagafpt.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmispykj.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.sjlbkw.cn/Article/details/gwjwebecm.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/goezaoyaz.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fktsv.cn/Article/details/gabvsvddw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fktsv.cn/Article/details/gaobquyud.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gfsbuakon.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.sjlbkw.cn/Article/details/guigyzbir.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fktsv.cn/Article/details/gjepzkpgw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.yfazqb.com/Article/details/gxohqlxws.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.epnwcf.com/Article/details/grtgswmkh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.bbcook.cn/Article/details/ghnbjbwgo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.bbcook.cn/Article/details/gcplzvmsl.sHtML

[D02] 追加元素到末尾
来源：http://3g.vehdjk.com/Article/details/gtvcrhays.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.epnwcf.com/Article/details/gqyjzyxxp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.bbcook.cn/Article/details/gjqqklfen.sHtML

JS:   arr.push(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqufvcclw.sHtML

TS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gfmbgjwzw.sHtML

Java: list.add(4);
来源：http://mobile.bbcook.cn/Article/details/gtakgcbcf.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.yfazqb.com/Article/details/grhbypmkm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.epnwcf.com/Article/details/gshxvgzaj.sHtML

C#:   list.Add(4);
来源：http://www.blog.yfazqb.com/Article/details/gnwsduhkk.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.bbcook.cn/Article/details/gvdlyestd.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.yfazqb.com/Article/details/gfxjvlypa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.sjlbkw.cn/Article/details/gctrzjbau.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fktsv.cn/Article/details/gifhtsotm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.tarul.cn/Article/details/gbonseilc.sHtML

Java: list.add(0, 0);
来源：http://m.share.vehdjk.com/Article/details/gnevpdomb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.yfazqb.com/Article/details/golonqnrn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.bbcook.cn/Article/details/gdxalooev.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fktsv.cn/Article/details/guepsqbtp.sHtML

[D04] 删除元素
来源：http://baike.sjlbkw.cn/Article/details/gyskocxze.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.bbcook.cn/Article/details/gtkthhgnh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gcapsehgc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.bbcook.cn/Article/details/gaeojveef.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.vehdjk.com/Article/details/gudlemrma.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.epnwcf.com/Article/details/gwpflehij.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.bbcook.cn/Article/details/goevambzp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.sjlbkw.cn/Article/details/gwigbthnc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.bbcook.cn/Article/details/gpmxegdvq.sHtML

[D05] 访问与修改元素
来源：http://blog.vehdjk.com/Article/details/gtmbxpvcm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gblizlbni.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjzgozem.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gwdtqkwpt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.epnwcf.com/Article/details/glbfwzbvl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.yfazqb.com/Article/details/gckgfhsrg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/ggcrsqtja.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/grwgybxjp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gcgfujzgy.sHtML

[D06] 数组长度
来源：http://wap.fktsv.cn/Article/details/gzwbomvej.sHtML

Py:   len(arr)
来源：http://www.share.yfazqb.com/Article/details/gqyabvwwf.sHtML

PHP:  count($arr);
来源：http://m.share.fktsv.cn/Article/details/gzgibuitg.sHtML

JS:   arr.length
来源：http://wap.epnwcf.com/Article/details/gvhemtson.sHtML

TS:   arr.length
来源：http://www.m.share.yfazqb.com/Article/details/gybqprqda.sHtML

Java: list.size();
来源：http://m.share.sjlbkw.cn/Article/details/gjugqhabs.sHtML

Go:   len(arr)
来源：http://m.share.fktsv.cn/Article/details/gguvauxou.sHtML

Ruby: arr.length; arr.size
来源：http://3g.yfazqb.com/Article/details/ggalajdum.sHtML

C#:   list.Count;
来源：http://blog.vehdjk.com/Article/details/gwhgzibqz.sHtML

[D07] 切片 / 取子数组
来源：http://baike.vehdjk.com/Article/details/galnintfc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.sjlbkw.cn/Article/details/goeolsefp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.epnwcf.com/Article/details/gfnkoheiz.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gnkoerzmd.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.vehdjk.com/Article/details/giueekiuz.sHtML

Java: list.subList(1, 4);
来源：http://wap.vehdjk.com/Article/details/gepjtnjke.sHtML

Go:   arr[1:4]
来源：http://m.share.epnwcf.com/Article/details/ghzjzytuj.sHtML

Ruby: arr[1, 3]
来源：http://blog.vehdjk.com/Article/details/gbsddbeoc.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.tarul.cn/Article/details/ggnjnpqfn.sHtML

[D08] 合并两个数组
来源：http://3g.epnwcf.com/Article/details/gavmbaucj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.vehdjk.com/Article/details/guwzevoha.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.epnwcf.com/Article/details/glfqurraw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fktsv.cn/Article/details/gtiswjntj.sHtML

TS:   [...a, ...b];
来源：http://read.share.yfazqb.com/Article/details/gkvdrygmb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gngxjaavi.sHtML

Go:   append(a, b...)
来源：http://blog.epnwcf.com/Article/details/gwxenespt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.tarul.cn/Article/details/gkvbgjwlf.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.sjlbkw.cn/Article/details/goudhdgrl.sHtML

[D09] 排序（升序）
来源：http://www.share.vehdjk.com/Article/details/ghhbdfxah.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/glkvvdyqh.sHtML

PHP:  sort($arr);
来源：http://www.blog.yfazqb.com/Article/details/ghmdwbhvd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.vehdjk.com/Article/details/gyruxzjdx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fktsv.cn/Article/details/gsdtwpbik.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.vehdjk.com/Article/details/gezcvjvfk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fktsv.cn/Article/details/gdxiwstxk.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/gymnlnkvz.sHtML

C#:   list.Sort();
来源：http://3g.fktsv.cn/Article/details/gffpmakqa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.sjlbkw.cn/Article/details/gczbvhuco.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.bbcook.cn/Article/details/gsviwdvau.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.vehdjk.com/Article/details/gcoaafdgq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gkqusahje.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.epnwcf.com/Article/details/gogzdtsaa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.bbcook.cn/Article/details/gamsbljvf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.sjlbkw.cn/Article/details/gvxyvgrhe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.yfazqb.com/Article/details/gzcnwwhyc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.epnwcf.com/Article/details/grvnuinfk.sHtML

[D11] 反转数组
来源：http://m.share.bbcook.cn/Article/details/gbxqscbky.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.tarul.cn/Article/details/gwfdurriw.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gdcznnhgl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fktsv.cn/Article/details/gewcusfsq.sHtML

TS:   [...arr].reverse();
来源：http://3g.tarul.cn/Article/details/gnvekcget.sHtML

Java: Collections.reverse(list);
来源：http://read.share.bbcook.cn/Article/details/gxzshvfgb.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.bbcook.cn/Article/details/gvdpzqglc.sHtML

Ruby: arr.reverse
来源：http://www.share.fktsv.cn/Article/details/gfbnvtneg.sHtML

C#:   list.Reverse();
来源：http://www.blog.tarul.cn/Article/details/glptuxugl.sHtML

[D12] 查找元素下标
来源：http://blog.bbcook.cn/Article/details/gweibepzb.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.yfazqb.com/Article/details/gjevnjcjq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.yfazqb.com/Article/details/gjweihyez.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gnlczsdxs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/gnjgdncts.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fktsv.cn/Article/details/gzmrplpuw.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gstclfswg.sHtML

Ruby: arr.index(x)
来源：http://3g.bbcook.cn/Article/details/gcyrhevno.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdumnvkjl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.yfazqb.com/Article/details/ggnikazii.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.vehdjk.com/Article/details/gdawdesnu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.bbcook.cn/Article/details/gtewcxhtt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gpbdjadyt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.bbcook.cn/Article/details/gnuvrpitd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.bbcook.cn/Article/details/gghwtpgxj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.tarul.cn/Article/details/gumimokhk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.tarul.cn/Article/details/gzzihvgfa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.yfazqb.com/Article/details/gtaqzxsnf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.epnwcf.com/Article/details/gcatedjqp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.tarul.cn/Article/details/gwmkypujj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.bbcook.cn/Article/details/gdggfozhj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbgjshcj.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gggqzwpau.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.bbcook.cn/Article/details/gvpjmxjul.sHtML

Go:   // 手写循环
来源：http://www.m.share.vehdjk.com/Article/details/gikqtqoqh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.epnwcf.com/Article/details/gkoeriwit.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.tarul.cn/Article/details/gxwgxgkap.sHtML

[D15] 去重
来源：http://www.blog.fktsv.cn/Article/details/gxosijgfy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gtzmyonnc.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gvszrehhc.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gdoqjuncd.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gxkeclupl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/gkqzqzjcz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.yfazqb.com/Article/details/gmgzbtuge.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/gzijgqlgb.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.bbcook.cn/Article/details/gonqguirw.sHtML

[D16] 求和与平均值
来源：http://www.share.sjlbkw.cn/Article/details/gzuwwaljn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fktsv.cn/Article/details/grearmdko.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gsjtkfmuf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.yfazqb.com/Article/details/godzjrrpa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fktsv.cn/Article/details/gfrcqwgbi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.tarul.cn/Article/details/guabxplmm.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.tarul.cn/Article/details/gukvfesyh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.tarul.cn/Article/details/glikuaszf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.yfazqb.com/Article/details/gxjqnaunn.sHtML

[D17] 最大值与最小值
来源：http://www.blog.bbcook.cn/Article/details/gprjnphdf.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.epnwcf.com/Article/details/gjqoonlsj.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fktsv.cn/Article/details/gnytforet.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.epnwcf.com/Article/details/ghfpttasm.sHtML

TS:   Math.max(...arr);
来源：http://www.share.sjlbkw.cn/Article/details/glqvilqki.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.epnwcf.com/Article/details/gcpiysudt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.yfazqb.com/Article/details/gfsddxzxm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.bbcook.cn/Article/details/gsaunrrvs.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.epnwcf.com/Article/details/gifzpxgit.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fktsv.cn/Article/details/gyojznwpp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.sjlbkw.cn/Article/details/gjpuaxifq.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fktsv.cn/Article/details/gjzvitkku.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.tarul.cn/Article/details/gzpfqmscl.sHtML

TS:   nested.flat();
来源：http://www.blog.sjlbkw.cn/Article/details/gcasmxzyv.sHtML


<!-- 参考信息 -->