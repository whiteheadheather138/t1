代发 wailian999

Go:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/ggswwzrce.sHtML

Ruby: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/giittlxnw.sHtML

C#:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gkjrtlcof.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.vehdjk.com/Article/details/gqdqgmkgg.sHtML

Py:   if not data: return
来源：http://read.share.fktsv.cn/Article/details/glbuzuunw.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.epnwcf.com/Article/details/gftsrobtf.sHtML

JS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gzbktvyrc.sHtML

TS:   if (!data) return;
来源：http://read.share.yfazqb.com/Article/details/gswxvarod.sHtML

Java: if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gailfaiek.sHtML

Go:   if data == nil { return }
来源：http://www.share.bbcook.cn/Article/details/gzlqwxvod.sHtML

Ruby: return if data.nil?
来源：http://www.share.yfazqb.com/Article/details/glvapludl.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gewbeyzvj.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gaxoqodti.sHtML

C. 函数与作用域
来源：http://www.m.share.fktsv.cn/Article/details/gmlndahgz.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gqtetkhoe.sHtML

[C01] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/gixgkhbai.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.tarul.cn/Article/details/gcwrujpfa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gilzebnwn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbucjlkda.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gfevkorif.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gedzhpzuk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fktsv.cn/Article/details/gidtvazps.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/garcrkzip.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gioxcnrmm.sHtML

[C02] 默认参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnexcnbe.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.epnwcf.com/Article/details/gynalwbsv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fktsv.cn/Article/details/gakzuwbfj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.tarul.cn/Article/details/grfleemvr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/guqcwevlp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fktsv.cn/Article/details/gaxbqormb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.tarul.cn/Article/details/ggqzocnvt.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.tarul.cn/Article/details/gudlutpwq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fktsv.cn/Article/details/gaomiogop.sHtML

[C03] 可变参数
来源：http://3g.tarul.cn/Article/details/gknyjqxir.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.yfazqb.com/Article/details/gvwammeof.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.sjlbkw.cn/Article/details/gifcsjilc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/ggjmtinso.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/glysenwam.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.vehdjk.com/Article/details/gutzzxrrv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.bbcook.cn/Article/details/gosnhgcbg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.sjlbkw.cn/Article/details/govemaklp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.sjlbkw.cn/Article/details/gkulaovkh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.yfazqb.com/Article/details/gqaidntvq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.tarul.cn/Article/details/ghrwignht.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.vehdjk.com/Article/details/gqohfqhbn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gvdxwvfyw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.vehdjk.com/Article/details/gjqrhwmhc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.vehdjk.com/Article/details/glryzvqvq.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.sjlbkw.cn/Article/details/gwsffcgex.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/goikenrnp.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gtafnxyot.sHtML

[C05] 返回多个值
来源：http://www.m.share.sjlbkw.cn/Article/details/gsugfohtd.sHtML

Py:   return a, b
来源：http://mobile.yfazqb.com/Article/details/gkvvpxmfy.sHtML

PHP:  return [$a, $b];
来源：http://www.share.sjlbkw.cn/Article/details/gfvlprxyd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.tarul.cn/Article/details/gokffrnze.sHtML

TS:   return { a, b };
来源：http://mobile.sjlbkw.cn/Article/details/gjbwjpkhe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.bbcook.cn/Article/details/gbmlmknnx.sHtML

Go:   return a, b
来源：http://3g.vehdjk.com/Article/details/gmalmkzgh.sHtML

Ruby: return a, b
来源：http://3g.bbcook.cn/Article/details/gpvswdtfj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.vehdjk.com/Article/details/gpqhzhvwz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.yfazqb.com/Article/details/glrtltabi.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.bbcook.cn/Article/details/gzoxhbafr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.bbcook.cn/Article/details/gyilgoubt.sHtML

JS:   const square = x => x * x;
来源：http://wap.fktsv.cn/Article/details/giaxlriux.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.vehdjk.com/Article/details/ggsmvzlvp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.tarul.cn/Article/details/gfxgdxivm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.vehdjk.com/Article/details/gzmfecnpc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.sjlbkw.cn/Article/details/gfvvodkpe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/grhieknac.sHtML

[C07] 把函数作为参数传入
来源：http://wap.yfazqb.com/Article/details/gzyzbkbxv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.vehdjk.com/Article/details/genvnxsmx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gwyujvrlt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.tarul.cn/Article/details/gbtevqhat.sHtML

TS:   arr.map(String)
来源：http://www.m.share.vehdjk.com/Article/details/gnydetlzq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.vehdjk.com/Article/details/gifpxdown.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.sjlbkw.cn/Article/details/ghudwigrp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fktsv.cn/Article/details/gfyyaujck.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.epnwcf.com/Article/details/gycembgaq.sHtML

[C08] 闭包
来源：http://mobile.vehdjk.com/Article/details/gvpruflai.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.bbcook.cn/Article/details/gbftaxpll.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.yfazqb.com/Article/details/gbthexvee.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/grksucynt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gofdevyfu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.sjlbkw.cn/Article/details/gnnkakssv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fktsv.cn/Article/details/gtanimtcz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fktsv.cn/Article/details/gqovkmgae.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gqwyhiqeb.sHtML

[C09] 递归
来源：http://read.share.fktsv.cn/Article/details/ghqpgrcbp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.tarul.cn/Article/details/gcesyvfrd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.yfazqb.com/Article/details/grczccent.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fktsv.cn/Article/details/gmvpucwuq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fktsv.cn/Article/details/gccfxmarg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.yfazqb.com/Article/details/gkugtkqqz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.tarul.cn/Article/details/gshdwsqch.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fktsv.cn/Article/details/gfwblfmhe.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.epnwcf.com/Article/details/gdgdocwuf.sHtML

[C10] 变量作用域
来源：http://www.blog.epnwcf.com/Article/details/gfkvkvkxw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fktsv.cn/Article/details/gshgzgfvg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.tarul.cn/Article/details/grpjucmzj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fktsv.cn/Article/details/gpcpfhtah.sHtML

TS:   同 JS
来源：http://www.share.epnwcf.com/Article/details/gvgouzaux.sHtML

Java: 方法内为块级作用域
来源：http://3g.epnwcf.com/Article/details/gouyvsbqs.sHtML

Go:   花括号块级作用域
来源：http://blog.vehdjk.com/Article/details/gzykygkgd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.sjlbkw.cn/Article/details/gtjzcemxa.sHtML

C#:   块级作用域
来源：http://m.share.bbcook.cn/Article/details/grvfjbpki.sHtML

[C11] 模块导入与导出
来源：http://www.blog.yfazqb.com/Article/details/giwnjdvcj.sHtML

Py:   from module import func
来源：http://3g.epnwcf.com/Article/details/gznverezv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.epnwcf.com/Article/details/gjkiwcsng.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.epnwcf.com/Article/details/gjlvoiqqs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.vehdjk.com/Article/details/geydjktju.sHtML

Java: import java.util.List;
来源：http://read.share.fktsv.cn/Article/details/gkfkmgwlr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.tarul.cn/Article/details/gyyxenvou.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fktsv.cn/Article/details/gcegxtgzb.sHtML

C#:   using System.Text;
来源：http://www.blog.fktsv.cn/Article/details/gtpjnitcn.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.tarul.cn/Article/details/gnycmtskl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.yfazqb.com/Article/details/grflfucyj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.bbcook.cn/Article/details/gpjixvaht.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gdlzivaqn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/gvalhffwq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.vehdjk.com/Article/details/guliitwfb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.bbcook.cn/Article/details/gqjvyarjg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fktsv.cn/Article/details/gzetmefxj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.bbcook.cn/Article/details/gfvjasiob.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.vehdjk.com/Article/details/gwnwjoqzp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.epnwcf.com/Article/details/gynswxvrc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gwbaahvrr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.vehdjk.com/Article/details/gofmeprsz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gbveeshhy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gopbgukpz.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fktsv.cn/Article/details/gjinmiulb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.yfazqb.com/Article/details/gssnkzxej.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.vehdjk.com/Article/details/guavfqksr.sHtML

[C14] 泛型函数
来源：http://wap.vehdjk.com/Article/details/gdaljbzti.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.bbcook.cn/Article/details/gypqfovay.sHtML

PHP:  // 无泛型
来源：http://3g.tarul.cn/Article/details/gmlfzzmvv.sHtML

JS:   // 无泛型
来源：http://mobile.epnwcf.com/Article/details/glnbfxtxw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.vehdjk.com/Article/details/gyxqtqjiy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.epnwcf.com/Article/details/gjepyqjbh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fktsv.cn/Article/details/gudtthapq.sHtML

Ruby: # 无泛型
来源：http://mobile.vehdjk.com/Article/details/gfkhngiui.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.bbcook.cn/Article/details/gpniqlmuk.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.bbcook.cn/Article/details/gyinzlqov.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.yfazqb.com/Article/details/gouaxfxzg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.vehdjk.com/Article/details/gwqsdwhia.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gbdgvvvht.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fktsv.cn/Article/details/gaqvkcdtz.sHtML

Java: // 无解构
来源：http://www.share.fktsv.cn/Article/details/gsmozuxat.sHtML

Go:   // 无解构
来源：http://mobile.vehdjk.com/Article/details/gxdpotadk.sHtML

Ruby: a, b = pair
来源：http://www.share.epnwcf.com/Article/details/gdkjyrnej.sHtML

C#:   var (a, b) = pair;
来源：http://blog.yfazqb.com/Article/details/gqtzcaptv.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.epnwcf.com/Article/details/gqhjjvgkn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fktsv.cn/Article/details/guodctcyu.sHtML

PHP:  // 无重载
来源：http://wap.yfazqb.com/Article/details/gxstkivem.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.tarul.cn/Article/details/gllxumqja.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fktsv.cn/Article/details/gxqwrgzpx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.vehdjk.com/Article/details/gcnszqeui.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fktsv.cn/Article/details/gopqdbtfi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.epnwcf.com/Article/details/ghzoxertt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.sjlbkw.cn/Article/details/gngfnqebe.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjfxmwrya.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.yfazqb.com/Article/details/goqstljtm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gragfrmvg.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gbzamqavv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.epnwcf.com/Article/details/gdjjjuhem.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.yfazqb.com/Article/details/gocfpjxvd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.tarul.cn/Article/details/gtgqgyyue.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.yfazqb.com/Article/details/gfotslcee.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fktsv.cn/Article/details/gsyjaaiji.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.yfazqb.com/Article/details/gcaqwnfry.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gmajstruq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.yfazqb.com/Article/details/grtlirdro.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.epnwcf.com/Article/details/gutcbrgqn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.vehdjk.com/Article/details/grvjvafmg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fktsv.cn/Article/details/gxruhxxsp.sHtML

JS:   arr.push(4);
来源：http://baike.tarul.cn/Article/details/gotlwuook.sHtML

TS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/gxdiyrojv.sHtML

Java: list.add(4);
来源：http://read.share.vehdjk.com/Article/details/gukvfzyaz.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.tarul.cn/Article/details/gtohlevdz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.tarul.cn/Article/details/gmtytebob.sHtML

C#:   list.Add(4);
来源：http://read.share.vehdjk.com/Article/details/goaayyylg.sHtML

[D03] 在指定位置插入元素
来源：http://blog.bbcook.cn/Article/details/gfkhqwbbx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.yfazqb.com/Article/details/gedtbunsu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fktsv.cn/Article/details/gyxnhusyx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.epnwcf.com/Article/details/gcxzbclwt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fktsv.cn/Article/details/gllzyuuwz.sHtML

Java: list.add(0, 0);
来源：http://www.share.tarul.cn/Article/details/gutluenyr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.yfazqb.com/Article/details/goeegitsj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.epnwcf.com/Article/details/gvctedcun.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fktsv.cn/Article/details/gkghctiwx.sHtML

[D04] 删除元素
来源：http://m.share.fktsv.cn/Article/details/gxhzxzvve.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.tarul.cn/Article/details/gkyruhsfm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gcczyddit.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.vehdjk.com/Article/details/gexuhfpzt.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fktsv.cn/Article/details/giqldxqbk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fktsv.cn/Article/details/gqbrudaqi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.bbcook.cn/Article/details/glkndzobe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.yfazqb.com/Article/details/gwsactlcg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.bbcook.cn/Article/details/gmqwutbgu.sHtML

[D05] 访问与修改元素
来源：http://wap.vehdjk.com/Article/details/gvbhabzvj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gkebiburd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gbgfzzdww.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gxhcdtcbi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.epnwcf.com/Article/details/gzdvghjwd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.tarul.cn/Article/details/gihyehnlg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gmhgxbnbv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gcaaaunsg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gvknltadc.sHtML

[D06] 数组长度
来源：http://wap.epnwcf.com/Article/details/gwquhmydy.sHtML

Py:   len(arr)
来源：http://3g.fktsv.cn/Article/details/godkekpka.sHtML

PHP:  count($arr);
来源：http://baike.sjlbkw.cn/Article/details/gmzklmuin.sHtML

JS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/ggpdozrrc.sHtML

TS:   arr.length
来源：http://m.share.fktsv.cn/Article/details/gaqlwkenz.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/gdqrtubtb.sHtML

Go:   len(arr)
来源：http://m.share.yfazqb.com/Article/details/guhpxhxlx.sHtML

Ruby: arr.length; arr.size
来源：http://baike.sjlbkw.cn/Article/details/gnzihxqar.sHtML

C#:   list.Count;
来源：http://baike.bbcook.cn/Article/details/gghudkdnh.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.vehdjk.com/Article/details/gjjmdwisz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.sjlbkw.cn/Article/details/gynqaycff.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gneonpmtz.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/gofmawqvr.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/ghkvxmrvi.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gvxpealqo.sHtML

Go:   arr[1:4]
来源：http://mobile.epnwcf.com/Article/details/gsmocjcva.sHtML

Ruby: arr[1, 3]
来源：http://3g.tarul.cn/Article/details/gxipymgcf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.tarul.cn/Article/details/gyhcoujir.sHtML

[D08] 合并两个数组
来源：http://mobile.epnwcf.com/Article/details/gixdtdmyu.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.sjlbkw.cn/Article/details/givlslenr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.epnwcf.com/Article/details/gfdvppssd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.tarul.cn/Article/details/gajhnwfli.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.bbcook.cn/Article/details/gmwexgnzh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.bbcook.cn/Article/details/gwbmgksal.sHtML

Go:   append(a, b...)
来源：http://read.share.vehdjk.com/Article/details/gccrqhlvr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.yfazqb.com/Article/details/grwkighjt.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fktsv.cn/Article/details/ghektpiwb.sHtML

[D09] 排序（升序）
来源：http://m.share.vehdjk.com/Article/details/ggzpazksz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/gtrjmrutr.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gyncciwef.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.tarul.cn/Article/details/ggldpyjtp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.vehdjk.com/Article/details/grgqlsnrs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fktsv.cn/Article/details/gbipbvwvn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gdwsjwlwu.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gttahrokp.sHtML

C#:   list.Sort();
来源：http://read.share.vehdjk.com/Article/details/gsqdttzqh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.vehdjk.com/Article/details/gubayukzp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.yfazqb.com/Article/details/gzllkidio.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/gyjhfhnob.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/grgfbfckz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gobqylyxa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fktsv.cn/Article/details/gtjjmftew.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.sjlbkw.cn/Article/details/grvtntuzu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fktsv.cn/Article/details/gdebdzmkv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.epnwcf.com/Article/details/ghmsdgnpe.sHtML

[D11] 反转数组
来源：http://wap.sjlbkw.cn/Article/details/gfxoppznd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fktsv.cn/Article/details/gljyvkrkc.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.bbcook.cn/Article/details/gmigmfidk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.vehdjk.com/Article/details/gsymsewla.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.yfazqb.com/Article/details/gxqlxbxqc.sHtML

Java: Collections.reverse(list);
来源：http://read.share.sjlbkw.cn/Article/details/giclmkqnw.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.epnwcf.com/Article/details/gqshnsfjq.sHtML

Ruby: arr.reverse
来源：http://read.share.epnwcf.com/Article/details/ghnievgmi.sHtML

C#:   list.Reverse();
来源：http://www.share.yfazqb.com/Article/details/gegqpgqmg.sHtML

[D12] 查找元素下标
来源：http://m.share.vehdjk.com/Article/details/gnlyhbaqj.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.epnwcf.com/Article/details/gogdubkpx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.epnwcf.com/Article/details/gttuctpsp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gekhqflhp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.sjlbkw.cn/Article/details/ggxawmkpj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.yfazqb.com/Article/details/gogwmootf.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gwfpeyuop.sHtML

Ruby: arr.index(x)
来源：http://3g.vehdjk.com/Article/details/gppxaokxx.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnnumtgp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.epnwcf.com/Article/details/ghbtdmqeu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.tarul.cn/Article/details/gawuioulp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.yfazqb.com/Article/details/gvrbnvqne.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gajgkzlwp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/grsjgsspe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.sjlbkw.cn/Article/details/giqprshvy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fktsv.cn/Article/details/gkhmpfefw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.epnwcf.com/Article/details/gtfibyfpf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gxgvsttzr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.yfazqb.com/Article/details/goqqcxhgv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.vehdjk.com/Article/details/gpmelllps.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.bbcook.cn/Article/details/govyiexjt.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/gdychqvre.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/getuevzwu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.epnwcf.com/Article/details/gqoyabbnl.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gnuxugbzd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.tarul.cn/Article/details/gwwzrewip.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.bbcook.cn/Article/details/gsiyigeoa.sHtML

[D15] 去重
来源：http://m.share.vehdjk.com/Article/details/gzsysppta.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/gghbahvgj.sHtML

PHP:  array_unique($arr);
来源：http://baike.tarul.cn/Article/details/gfzbhetuq.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gfyerqali.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gjmnfslyp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.epnwcf.com/Article/details/gzpajvmkx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.sjlbkw.cn/Article/details/gouhpesan.sHtML

Ruby: arr.uniq
来源：http://3g.vehdjk.com/Article/details/gbaxvivkd.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.tarul.cn/Article/details/gkzoluecw.sHtML

[D16] 求和与平均值
来源：http://read.share.bbcook.cn/Article/details/gjvqgnpkw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gngiahiix.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.vehdjk.com/Article/details/gsctbgeud.sHtML


<!-- 参考信息 -->