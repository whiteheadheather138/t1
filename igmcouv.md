代发 wailian999

Java: if (data == null) return;
来源：http://baike.tarul.cn/Article/details/ghckxcjjn.sHtML

Go:   if data == nil { return }
来源：http://3g.sjlbkw.cn/Article/details/gceqzvuxg.sHtML

Ruby: return if data.nil?
来源：http://read.share.tarul.cn/Article/details/gvpztfmgn.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/gyhaiijgs.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gbopkpkqt.sHtML

C. 函数与作用域
来源：http://3g.fktsv.cn/Article/details/gbmpkjzvb.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjgwqsojq.sHtML

[C01] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gbbsvpiyh.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.tarul.cn/Article/details/grsavwsqp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/ghhdknsoc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gotezsjsv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gmpelerwp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gcnjtsniq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.sjlbkw.cn/Article/details/galpcdqlq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.epnwcf.com/Article/details/gecovnomn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gulfrpxqw.sHtML

[C02] 默认参数
来源：http://3g.bbcook.cn/Article/details/grllrqtnz.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.sjlbkw.cn/Article/details/ggvpyatpy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fktsv.cn/Article/details/gvvcksilq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/grauohpup.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gnvsxbjoo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.epnwcf.com/Article/details/ghuxjxkmh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.bbcook.cn/Article/details/gjinczobl.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.epnwcf.com/Article/details/glesjnmlt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.yfazqb.com/Article/details/gwfjdeqge.sHtML

[C03] 可变参数
来源：http://wap.tarul.cn/Article/details/gvkuooscn.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.vehdjk.com/Article/details/ggaszhtzg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.bbcook.cn/Article/details/gyfkjeztl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/gmdxavjxo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gwwikumzo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.bbcook.cn/Article/details/gdzbwacqv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/glmjrropz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fktsv.cn/Article/details/gsdcubnmw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fktsv.cn/Article/details/gwvezgbzw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.vehdjk.com/Article/details/gjrfoppnf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.tarul.cn/Article/details/gruyfajmi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fktsv.cn/Article/details/grjpiepvd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.yfazqb.com/Article/details/gvdfpqkbk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.yfazqb.com/Article/details/gzkywyync.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.sjlbkw.cn/Article/details/gqqcnzyqr.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gelwytxid.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gdsggxpzp.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gxbuxhfht.sHtML

[C05] 返回多个值
来源：http://baike.sjlbkw.cn/Article/details/glfmkdwfe.sHtML

Py:   return a, b
来源：http://blog.tarul.cn/Article/details/gqgmkyywp.sHtML

PHP:  return [$a, $b];
来源：http://read.share.epnwcf.com/Article/details/gumxmukzh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/gpvxvppyf.sHtML

TS:   return { a, b };
来源：http://m.share.fktsv.cn/Article/details/gtwyvwqzs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fktsv.cn/Article/details/gaxmynumo.sHtML

Go:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gutpejujg.sHtML

Ruby: return a, b
来源：http://www.blog.bbcook.cn/Article/details/gapzhqanu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.sjlbkw.cn/Article/details/gvxckqesl.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.bbcook.cn/Article/details/gappvtksh.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.bbcook.cn/Article/details/glkohysib.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.vehdjk.com/Article/details/gohgawujg.sHtML

JS:   const square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/glbxcxezd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.bbcook.cn/Article/details/gjnctrldq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.bbcook.cn/Article/details/gqonbkqlr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.bbcook.cn/Article/details/gtajnlypu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.bbcook.cn/Article/details/gyswiswad.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/gnorfiuff.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.tarul.cn/Article/details/ggpqtejtr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fktsv.cn/Article/details/gkhomrdbi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gapbithwt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.bbcook.cn/Article/details/ggeypqdmi.sHtML

TS:   arr.map(String)
来源：http://mobile.bbcook.cn/Article/details/gozopxfdt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.bbcook.cn/Article/details/gevlumiev.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.epnwcf.com/Article/details/gjqiyodmo.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.epnwcf.com/Article/details/guhbmusmt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.yfazqb.com/Article/details/gxvinpzkb.sHtML

[C08] 闭包
来源：http://baike.bbcook.cn/Article/details/gsgcvylku.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.tarul.cn/Article/details/gfwwhqbfd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.yfazqb.com/Article/details/gmgrvvnuu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gfmnxjefi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gdoohqkuq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/ggyuprebg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.tarul.cn/Article/details/gurtgdhnz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.sjlbkw.cn/Article/details/gbialhced.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gwqcxumrp.sHtML

[C09] 递归
来源：http://www.m.share.fktsv.cn/Article/details/gfncwjleq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gfqxkzeth.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.bbcook.cn/Article/details/glcgtmyjq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/goswyolor.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gbteidvwe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.bbcook.cn/Article/details/gxyfgrvuh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.yfazqb.com/Article/details/gnwcgjzgf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gyukzfugd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.vehdjk.com/Article/details/gurwiripq.sHtML

[C10] 变量作用域
来源：http://www.share.yfazqb.com/Article/details/gcjwmxywj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.bbcook.cn/Article/details/ggijgwjgz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.sjlbkw.cn/Article/details/gdipjmqnc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.bbcook.cn/Article/details/gekoaxqak.sHtML

TS:   同 JS
来源：http://www.blog.vehdjk.com/Article/details/gmbbwuvla.sHtML

Java: 方法内为块级作用域
来源：http://baike.fktsv.cn/Article/details/gvdlanvqd.sHtML

Go:   花括号块级作用域
来源：http://www.blog.epnwcf.com/Article/details/gwlgrgeiw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.epnwcf.com/Article/details/gyotilkst.sHtML

C#:   块级作用域
来源：http://www.blog.yfazqb.com/Article/details/gksrunogb.sHtML

[C11] 模块导入与导出
来源：http://3g.sjlbkw.cn/Article/details/gjeavviyh.sHtML

Py:   from module import func
来源：http://www.share.tarul.cn/Article/details/gfbluxbra.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fktsv.cn/Article/details/gbduoudit.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.yfazqb.com/Article/details/gvsiermtl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.tarul.cn/Article/details/gsslzywdb.sHtML

Java: import java.util.List;
来源：http://read.share.yfazqb.com/Article/details/gqwkhmpxd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fktsv.cn/Article/details/gmdepsiqo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.epnwcf.com/Article/details/gcheeusis.sHtML

C#:   using System.Text;
来源：http://www.share.sjlbkw.cn/Article/details/gevolsfvr.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fktsv.cn/Article/details/gtxrnztqu.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.bbcook.cn/Article/details/gayswyalj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.bbcook.cn/Article/details/gpgmbgtcc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.sjlbkw.cn/Article/details/gowgtqczy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.yfazqb.com/Article/details/gxpsjhufc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.tarul.cn/Article/details/gxjtqmcwp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.sjlbkw.cn/Article/details/gvjfulgvn.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fktsv.cn/Article/details/glwbxobpb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.bbcook.cn/Article/details/gpochgirz.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.epnwcf.com/Article/details/gohewlbut.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.tarul.cn/Article/details/gkufqyjbg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gyxwmctsj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.yfazqb.com/Article/details/gffberixv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gnmyjamqu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gadvnzcun.sHtML

Go:   func add(a, b int) int
来源：http://mobile.tarul.cn/Article/details/gytwerrrd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fktsv.cn/Article/details/ghujpdppo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.sjlbkw.cn/Article/details/gvwchiclo.sHtML

[C14] 泛型函数
来源：http://www.m.share.tarul.cn/Article/details/gjogueelu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.sjlbkw.cn/Article/details/gpyvfzcfw.sHtML

PHP:  // 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gdplzpzdn.sHtML

JS:   // 无泛型
来源：http://baike.epnwcf.com/Article/details/gebkmoaej.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fktsv.cn/Article/details/gqborlsah.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxzdjnsr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.sjlbkw.cn/Article/details/gqpjksfzq.sHtML

Ruby: # 无泛型
来源：http://read.share.epnwcf.com/Article/details/gjuncbsnh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.bbcook.cn/Article/details/gsdwdihnd.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.epnwcf.com/Article/details/gtaftkwaz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/gzzpgwniu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.bbcook.cn/Article/details/gionrqrlr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/gfbhoqmap.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.vehdjk.com/Article/details/gqpvsartj.sHtML

Java: // 无解构
来源：http://www.share.sjlbkw.cn/Article/details/gpjzviyws.sHtML

Go:   // 无解构
来源：http://www.share.epnwcf.com/Article/details/gldvnsfdo.sHtML

Ruby: a, b = pair
来源：http://mobile.fktsv.cn/Article/details/grbzpuoou.sHtML

C#:   var (a, b) = pair;
来源：http://baike.bbcook.cn/Article/details/gkbycfznq.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.tarul.cn/Article/details/ghjvunkzb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.tarul.cn/Article/details/gpoysuyxh.sHtML

PHP:  // 无重载
来源：http://www.blog.yfazqb.com/Article/details/gporgixba.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.tarul.cn/Article/details/gbfkqeiom.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.epnwcf.com/Article/details/gcdauekcz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.bbcook.cn/Article/details/gdppteuye.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.epnwcf.com/Article/details/gcumqxhat.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.yfazqb.com/Article/details/ghqgfjxjm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.vehdjk.com/Article/details/gkoprters.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpipkwdem.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.yfazqb.com/Article/details/gaqxfmviw.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gwfvmhbym.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.bbcook.cn/Article/details/gtevvenay.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.vehdjk.com/Article/details/gcbeqdfhc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.epnwcf.com/Article/details/gimdvkgjq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.bbcook.cn/Article/details/gnjwcngyo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fktsv.cn/Article/details/gbtefgvwp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.bbcook.cn/Article/details/ggwpksrjq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fktsv.cn/Article/details/ghqggzhnq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.bbcook.cn/Article/details/gaclecayt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fktsv.cn/Article/details/gatalfvbb.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.tarul.cn/Article/details/gegmijzac.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.tarul.cn/Article/details/gjekwjxil.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.yfazqb.com/Article/details/ggbhdcenb.sHtML

JS:   arr.push(4);
来源：http://read.share.bbcook.cn/Article/details/gagbdwsqm.sHtML

TS:   arr.push(4);
来源：http://www.blog.vehdjk.com/Article/details/ggyzmtkjm.sHtML

Java: list.add(4);
来源：http://www.share.epnwcf.com/Article/details/gwrmwbmoo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gtaarbniu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.sjlbkw.cn/Article/details/gnwsjrady.sHtML

C#:   list.Add(4);
来源：http://blog.fktsv.cn/Article/details/gcubvnzez.sHtML

[D03] 在指定位置插入元素
来源：http://blog.epnwcf.com/Article/details/gwlagidso.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.yfazqb.com/Article/details/gxlbwieru.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.tarul.cn/Article/details/gbwhsmkcg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.tarul.cn/Article/details/gyptctovp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.tarul.cn/Article/details/gbehjbptc.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/ghygmtnzb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.sjlbkw.cn/Article/details/grbfdqydl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.yfazqb.com/Article/details/gzboivgly.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gesdkukfm.sHtML

[D04] 删除元素
来源：http://wap.tarul.cn/Article/details/givfgpgmm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gykhhspwa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.tarul.cn/Article/details/ghntrkkzk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.epnwcf.com/Article/details/gflumtmac.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fktsv.cn/Article/details/gkwrxvvxt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.tarul.cn/Article/details/gdxbiznps.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.yfazqb.com/Article/details/gexilvtaa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.vehdjk.com/Article/details/gmmuvcchg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/ggadnroqb.sHtML

[D05] 访问与修改元素
来源：http://www.blog.epnwcf.com/Article/details/gdvlnvitp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gsrgwpetl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/gmcxvyjtz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gufwixkhn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fktsv.cn/Article/details/gkfpcaeje.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.tarul.cn/Article/details/gtnppjfew.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gxwhtjmqf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gperukoue.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/grxgjyjxb.sHtML

[D06] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gqqydsuxp.sHtML

Py:   len(arr)
来源：http://3g.vehdjk.com/Article/details/gjpwiqbbi.sHtML

PHP:  count($arr);
来源：http://read.share.tarul.cn/Article/details/gyzgtwhkl.sHtML

JS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/gjpevdzsr.sHtML

TS:   arr.length
来源：http://read.share.vehdjk.com/Article/details/gkgxeayvg.sHtML

Java: list.size();
来源：http://wap.fktsv.cn/Article/details/geqiqhfcv.sHtML

Go:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gihccpnga.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/gfwlfmvdg.sHtML

C#:   list.Count;
来源：http://mobile.sjlbkw.cn/Article/details/gqasdmuiu.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.bbcook.cn/Article/details/gyjnbacew.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.epnwcf.com/Article/details/gkzvcdchi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.tarul.cn/Article/details/gbrlazkvz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gafevqysw.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.vehdjk.com/Article/details/gftzgmzoy.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gupnrxzmg.sHtML

Go:   arr[1:4]
来源：http://wap.fktsv.cn/Article/details/glksqfxmx.sHtML

Ruby: arr[1, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gckyzovca.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gsoljjcwz.sHtML

[D08] 合并两个数组
来源：http://www.blog.bbcook.cn/Article/details/grjqaqqwp.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.yfazqb.com/Article/details/gbtnuhkwb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.epnwcf.com/Article/details/gjffofcsa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.vehdjk.com/Article/details/gdkputzyf.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxngicsa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gsfnismuj.sHtML

Go:   append(a, b...)
来源：http://3g.tarul.cn/Article/details/gsbnjubao.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.bbcook.cn/Article/details/gohzpdkmw.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.yfazqb.com/Article/details/gnixwqpqa.sHtML

[D09] 排序（升序）
来源：http://blog.vehdjk.com/Article/details/gwqnmigaq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/golbgwrlu.sHtML

PHP:  sort($arr);
来源：http://3g.vehdjk.com/Article/details/gfnjjdrqt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.yfazqb.com/Article/details/gptajejgb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.vehdjk.com/Article/details/ggikjmiti.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.bbcook.cn/Article/details/gtmuuvoto.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/glfpywfdk.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/gagpiepfh.sHtML

C#:   list.Sort();
来源：http://mobile.vehdjk.com/Article/details/grgyexbzk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fktsv.cn/Article/details/gwzxedold.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.vehdjk.com/Article/details/gxpfvvzqj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/gqipeywct.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.sjlbkw.cn/Article/details/gzerbyciy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gsgrsskkl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.tarul.cn/Article/details/geczgloiy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.tarul.cn/Article/details/gtyrzxnvq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.yfazqb.com/Article/details/ghmapgzuj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.vehdjk.com/Article/details/gqgnmlzmb.sHtML

[D11] 反转数组
来源：http://mobile.sjlbkw.cn/Article/details/glxtmfufa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.vehdjk.com/Article/details/gzchvqlmy.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gvajohdsl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fktsv.cn/Article/details/gpokwsztt.sHtML

TS:   [...arr].reverse();
来源：http://m.share.epnwcf.com/Article/details/gplwgvqad.sHtML

Java: Collections.reverse(list);
来源：http://blog.fktsv.cn/Article/details/gpioyplnp.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.yfazqb.com/Article/details/gkmlgcpyl.sHtML

Ruby: arr.reverse
来源：http://baike.tarul.cn/Article/details/gbxtufwhl.sHtML

C#:   list.Reverse();
来源：http://mobile.sjlbkw.cn/Article/details/gatcfppkd.sHtML

[D12] 查找元素下标
来源：http://www.blog.yfazqb.com/Article/details/gvtdwavez.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.epnwcf.com/Article/details/gcixacpoi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.yfazqb.com/Article/details/ghruydihy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gqvdvoycn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gsftlrdpn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fktsv.cn/Article/details/ggppqvfla.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gxawzddet.sHtML

Ruby: arr.index(x)
来源：http://mobile.vehdjk.com/Article/details/gdgcwnclx.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.yfazqb.com/Article/details/guzmpsdcf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.vehdjk.com/Article/details/gjjpesoew.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gpmviptla.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.sjlbkw.cn/Article/details/ginqeyzlx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gqfbsjsgg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gkceqmlml.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.vehdjk.com/Article/details/ggukhhgcm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.sjlbkw.cn/Article/details/ggnpqnbcv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fktsv.cn/Article/details/goxcotppx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.bbcook.cn/Article/details/grazsewon.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.bbcook.cn/Article/details/gwaazcpru.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.epnwcf.com/Article/details/gtzqcwhci.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gucilgkdq.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gubgbcrfx.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/gkjftimjj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gkzoelhdt.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gujeyjnxm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.yfazqb.com/Article/details/geiubhakp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gwdshrnbt.sHtML

[D15] 去重
来源：http://read.share.yfazqb.com/Article/details/gwyluxdzw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/gonxmwnrm.sHtML

PHP:  array_unique($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gnkpjtyco.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gqytwervu.sHtML

TS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gqjapsazy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.bbcook.cn/Article/details/gxqaikgsg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.tarul.cn/Article/details/glpgkckzg.sHtML

Ruby: arr.uniq
来源：http://www.blog.fktsv.cn/Article/details/grbequgxn.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.vehdjk.com/Article/details/gjzmveyjl.sHtML

[D16] 求和与平均值
来源：http://wap.yfazqb.com/Article/details/gfaasunkd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.yfazqb.com/Article/details/grliomkiq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.vehdjk.com/Article/details/gujpvrozh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/gqpjbwmey.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gyymfrnys.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.yfazqb.com/Article/details/gaslagvnh.sHtML

Go:   // 手写循环累加
来源：http://www.share.sjlbkw.cn/Article/details/gtafjojeq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fktsv.cn/Article/details/golwllyvd.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.yfazqb.com/Article/details/gsksxndtk.sHtML

[D17] 最大值与最小值
来源：http://www.share.vehdjk.com/Article/details/gnxnjdvjw.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.epnwcf.com/Article/details/gkwcobshu.sHtML


<!-- 参考信息 -->