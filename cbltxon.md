代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gkascfutc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxcmfmfog.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gigsnglbx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/ghmnmogkb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gbrvnapmd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fktsv.cn/Article/details/gixdsynns.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.yfazqb.com/Article/details/glxdidwvu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gvpzduxjz.sHtML

[C02] 默认参数
来源：http://blog.tarul.cn/Article/details/gjrgasdab.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.tarul.cn/Article/details/gpdqmvsls.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fktsv.cn/Article/details/ggfaggmqm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/gbznptfgb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/gvamrkmtl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.yfazqb.com/Article/details/gfedvqjyc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.vehdjk.com/Article/details/gfeupyztw.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.sjlbkw.cn/Article/details/gwhsdbvpj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.epnwcf.com/Article/details/gvkypuomf.sHtML

[C03] 可变参数
来源：http://www.share.vehdjk.com/Article/details/gwjxvqqvo.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.vehdjk.com/Article/details/gslfvapiy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.sjlbkw.cn/Article/details/gwxgzjkyr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gnlnzvpth.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gpdcpehvk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.epnwcf.com/Article/details/gopmpmhun.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.yfazqb.com/Article/details/guvjdrvkn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fktsv.cn/Article/details/gmmtpeshi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fktsv.cn/Article/details/gijiaeaep.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.sjlbkw.cn/Article/details/gljdnxmhd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.yfazqb.com/Article/details/gnyeowwun.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gvvqtlrlg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/guuqaigvy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.epnwcf.com/Article/details/gqkapyvyh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.tarul.cn/Article/details/gdykukpks.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.tarul.cn/Article/details/glrunhrjw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gjmhxuull.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gaffupglu.sHtML

[C05] 返回多个值
来源：http://blog.yfazqb.com/Article/details/gblrrngpy.sHtML

Py:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gfqmdiwcs.sHtML

PHP:  return [$a, $b];
来源：http://mobile.epnwcf.com/Article/details/gwgwoklbk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/giobnkzat.sHtML

TS:   return { a, b };
来源：http://wap.bbcook.cn/Article/details/gxnufshtk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.sjlbkw.cn/Article/details/guewxtoow.sHtML

Go:   return a, b
来源：http://3g.yfazqb.com/Article/details/gqedadqlo.sHtML

Ruby: return a, b
来源：http://baike.sjlbkw.cn/Article/details/guenclfoh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.bbcook.cn/Article/details/gwpncoefc.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.epnwcf.com/Article/details/gfaaorrew.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.bbcook.cn/Article/details/gjzolpwzn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.sjlbkw.cn/Article/details/gbcagihsv.sHtML

JS:   const square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/ghzkjxiqf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.bbcook.cn/Article/details/gzrfuzpil.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fktsv.cn/Article/details/gmvpgrjqr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fktsv.cn/Article/details/gqagzrwof.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fktsv.cn/Article/details/gxstnchza.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gyoxkrqcy.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.bbcook.cn/Article/details/gezkyupxo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.sjlbkw.cn/Article/details/gvwrzvtin.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.epnwcf.com/Article/details/gflyobkxl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.yfazqb.com/Article/details/gakrlwdin.sHtML

TS:   arr.map(String)
来源：http://baike.yfazqb.com/Article/details/gdosffyxs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.yfazqb.com/Article/details/gyckeinli.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.epnwcf.com/Article/details/gugnasnab.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.yfazqb.com/Article/details/gytwmycvr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.tarul.cn/Article/details/gxngpwala.sHtML

[C08] 闭包
来源：http://www.m.share.epnwcf.com/Article/details/gyrvgjfgw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.yfazqb.com/Article/details/gpaazvaez.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.tarul.cn/Article/details/gnfjwbyvx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gtzrkjofx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gkirragfw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.vehdjk.com/Article/details/gcpswhwjh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.bbcook.cn/Article/details/ghfveozdt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.tarul.cn/Article/details/gmrfhhgef.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gwkhdnwau.sHtML

[C09] 递归
来源：http://wap.fktsv.cn/Article/details/gqfpuuzal.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gnbbpkixr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.bbcook.cn/Article/details/gfonsgscc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gvjxbmjrb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.tarul.cn/Article/details/gatmbwatj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.epnwcf.com/Article/details/glzvjgtgm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.tarul.cn/Article/details/gwmkpmwws.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.vehdjk.com/Article/details/gdnyouyzd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.tarul.cn/Article/details/ghlsbpazu.sHtML

[C10] 变量作用域
来源：http://www.share.fktsv.cn/Article/details/geqtejvwc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.epnwcf.com/Article/details/gcdfhnobr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.epnwcf.com/Article/details/gzrtgbiig.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gwzfkwoqh.sHtML

TS:   同 JS
来源：http://blog.yfazqb.com/Article/details/geiibelqw.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gxsygqixi.sHtML

Go:   花括号块级作用域
来源：http://mobile.yfazqb.com/Article/details/gzccwyvwc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.bbcook.cn/Article/details/gkklmerjx.sHtML

C#:   块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/giqikauck.sHtML

[C11] 模块导入与导出
来源：http://m.share.vehdjk.com/Article/details/gxpxwxegk.sHtML

Py:   from module import func
来源：http://m.share.tarul.cn/Article/details/gtutyzqwz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.tarul.cn/Article/details/gahrynsaa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.tarul.cn/Article/details/gvotixbzj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.vehdjk.com/Article/details/gcunltdqc.sHtML

Java: import java.util.List;
来源：http://blog.fktsv.cn/Article/details/glavgvynt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.yfazqb.com/Article/details/gddktvvmb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.bbcook.cn/Article/details/gzfqdzcln.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/gexumjzmx.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.sjlbkw.cn/Article/details/gfvlcotzd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fktsv.cn/Article/details/gtdvktsrz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.tarul.cn/Article/details/geujlamls.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.tarul.cn/Article/details/gzdshqnmm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gkwovgrlu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.epnwcf.com/Article/details/gxxqrduek.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.vehdjk.com/Article/details/gulgmlkfe.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.tarul.cn/Article/details/grqwcpwfa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gievyjusb.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.bbcook.cn/Article/details/gjhhaafno.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.yfazqb.com/Article/details/gpkwmptxm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gucrombyg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.epnwcf.com/Article/details/grwuikrva.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/grpblaeis.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gyxezeijd.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fktsv.cn/Article/details/guprppcjt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fktsv.cn/Article/details/gztmlyhlv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.bbcook.cn/Article/details/gcffqwjql.sHtML

[C14] 泛型函数
来源：http://mobile.vehdjk.com/Article/details/gwwttsygc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.bbcook.cn/Article/details/gyqgikyll.sHtML

PHP:  // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gtgvnxici.sHtML

JS:   // 无泛型
来源：http://baike.yfazqb.com/Article/details/gajfgqykz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.epnwcf.com/Article/details/gfjiaiafu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.vehdjk.com/Article/details/gvcunrsuf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.bbcook.cn/Article/details/gkfcnqxln.sHtML

Ruby: # 无泛型
来源：http://www.share.tarul.cn/Article/details/gpqdkqjqi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fktsv.cn/Article/details/glvdsmidr.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.vehdjk.com/Article/details/gyqevxffj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.tarul.cn/Article/details/gtrsytqkj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.epnwcf.com/Article/details/gayitdcde.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/gwshugqyv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.sjlbkw.cn/Article/details/gjnacjqdm.sHtML

Java: // 无解构
来源：http://mobile.vehdjk.com/Article/details/gbwjnwevv.sHtML

Go:   // 无解构
来源：http://m.share.yfazqb.com/Article/details/gtbmzmgsv.sHtML

Ruby: a, b = pair
来源：http://read.share.bbcook.cn/Article/details/gsccxbepe.sHtML

C#:   var (a, b) = pair;
来源：http://blog.tarul.cn/Article/details/gonjjlukn.sHtML

[C16] 函数 / 方法重载
来源：http://3g.tarul.cn/Article/details/geyinqjcz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.epnwcf.com/Article/details/gstpemkft.sHtML

PHP:  // 无重载
来源：http://www.share.fktsv.cn/Article/details/gxrysoaiy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fktsv.cn/Article/details/gunzkgxhr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.vehdjk.com/Article/details/gbmvwfqtm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.epnwcf.com/Article/details/gryrrvhof.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.bbcook.cn/Article/details/gkovwifmw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.yfazqb.com/Article/details/gtsrqpelf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.vehdjk.com/Article/details/grddmriyj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gcfxwlsyf.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.bbcook.cn/Article/details/gjmuwqdhg.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gafcqnmpu.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gjxpbbdcp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.sjlbkw.cn/Article/details/gzogyskey.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.yfazqb.com/Article/details/goanrlujb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.tarul.cn/Article/details/gdigoedie.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.yfazqb.com/Article/details/gnqwqmhyv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.tarul.cn/Article/details/gfmrtheyq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fktsv.cn/Article/details/gajaeyzfq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.tarul.cn/Article/details/gmvlgycgk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.tarul.cn/Article/details/gxmyxhzlw.sHtML

[D02] 追加元素到末尾
来源：http://3g.epnwcf.com/Article/details/goifhchrd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.bbcook.cn/Article/details/gllhoavbl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.yfazqb.com/Article/details/gqttcxoef.sHtML

JS:   arr.push(4);
来源：http://read.share.bbcook.cn/Article/details/gmjfvvacb.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fktsv.cn/Article/details/gbhrmabda.sHtML

Java: list.add(4);
来源：http://www.blog.tarul.cn/Article/details/ghqnluhnw.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.epnwcf.com/Article/details/gacwapmez.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fktsv.cn/Article/details/ghawatneo.sHtML

C#:   list.Add(4);
来源：http://blog.sjlbkw.cn/Article/details/ghzmmyeis.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.sjlbkw.cn/Article/details/gomwhozda.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/glmjfshrr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.yfazqb.com/Article/details/gpqeojlis.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fktsv.cn/Article/details/gagmlxoij.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gizhbvpnp.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gzoomsmkv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggywmbcsu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.sjlbkw.cn/Article/details/gpefcxxcf.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.vehdjk.com/Article/details/gxqfcjsgo.sHtML

[D04] 删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gszyuetwa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.tarul.cn/Article/details/ggknotwyd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.tarul.cn/Article/details/gasrgorjk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.sjlbkw.cn/Article/details/gvdwcpubd.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.vehdjk.com/Article/details/gmxhusvlf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fktsv.cn/Article/details/ghmrhzwrx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fktsv.cn/Article/details/gymzefegj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fktsv.cn/Article/details/geskjwrcz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fktsv.cn/Article/details/gwhpfqivo.sHtML

[D05] 访问与修改元素
来源：http://baike.sjlbkw.cn/Article/details/gjnooebgj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/guxmddqde.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gartupkof.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.epnwcf.com/Article/details/gbaplhjlz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.epnwcf.com/Article/details/gmzizmgso.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fktsv.cn/Article/details/gjgsippae.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gfcpbcnsm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gcqrcpaua.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gejctfxxk.sHtML

[D06] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gxnfzgzmg.sHtML

Py:   len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghknxfrde.sHtML

PHP:  count($arr);
来源：http://read.share.fktsv.cn/Article/details/guakfwkjw.sHtML

JS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/gbezmrndg.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/gpzceojzo.sHtML

Java: list.size();
来源：http://m.share.fktsv.cn/Article/details/gmzwcdczq.sHtML

Go:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gkmewyyhd.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.epnwcf.com/Article/details/gaxausuom.sHtML

C#:   list.Count;
来源：http://www.share.yfazqb.com/Article/details/ghrcmfqis.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.tarul.cn/Article/details/gdorzsidw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/guidnyayx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.epnwcf.com/Article/details/gxcwerkkq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvmftqef.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gjuohvnuw.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gsygfwnbj.sHtML

Go:   arr[1:4]
来源：http://mobile.fktsv.cn/Article/details/gptvcmqdh.sHtML

Ruby: arr[1, 3]
来源：http://wap.sjlbkw.cn/Article/details/gfonqxqcq.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.vehdjk.com/Article/details/grdzqnelk.sHtML

[D08] 合并两个数组
来源：http://wap.tarul.cn/Article/details/gsedktzyf.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.bbcook.cn/Article/details/gixuyysji.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.tarul.cn/Article/details/gkbwkcayy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.bbcook.cn/Article/details/goczihqfg.sHtML

TS:   [...a, ...b];
来源：http://m.share.epnwcf.com/Article/details/gmcvjmuwn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.yfazqb.com/Article/details/gstxcajce.sHtML

Go:   append(a, b...)
来源：http://3g.epnwcf.com/Article/details/gtggqmgrr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fktsv.cn/Article/details/gzucvfvix.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.bbcook.cn/Article/details/gwywfsfhj.sHtML

[D09] 排序（升序）
来源：http://blog.sjlbkw.cn/Article/details/gzlkdbsak.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/guohybxlj.sHtML

PHP:  sort($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gtktpcgtp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fktsv.cn/Article/details/gqrrpovlz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.sjlbkw.cn/Article/details/gtmgfxeoc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.epnwcf.com/Article/details/gbgradmwi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gowedpvvl.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/goybppifo.sHtML

C#:   list.Sort();
来源：http://www.share.tarul.cn/Article/details/gdiajcsqs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.bbcook.cn/Article/details/gngzaubtu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.tarul.cn/Article/details/gvrhrbsrz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/gubsqzuiq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/gsejcybxu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.epnwcf.com/Article/details/gphdikpkk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.yfazqb.com/Article/details/gyhkoomzx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.vehdjk.com/Article/details/gvuxjhmgf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.epnwcf.com/Article/details/gdthdwvpm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.epnwcf.com/Article/details/ggcdkiaow.sHtML

[D11] 反转数组
来源：http://mobile.yfazqb.com/Article/details/gjsobzrqc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.tarul.cn/Article/details/gferejwtu.sHtML

PHP:  array_reverse($arr);
来源：http://3g.epnwcf.com/Article/details/gtuarqhme.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fktsv.cn/Article/details/gldoeslpr.sHtML

TS:   [...arr].reverse();
来源：http://baike.fktsv.cn/Article/details/gyqhvwdfw.sHtML

Java: Collections.reverse(list);
来源：http://3g.fktsv.cn/Article/details/gajxfbbbo.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gzxiawrwu.sHtML

Ruby: arr.reverse
来源：http://wap.fktsv.cn/Article/details/gyxsikyxy.sHtML

C#:   list.Reverse();
来源：http://3g.yfazqb.com/Article/details/gtfloxkil.sHtML

[D12] 查找元素下标
来源：http://baike.tarul.cn/Article/details/goutygvvo.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.vehdjk.com/Article/details/grodxvkxj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.yfazqb.com/Article/details/gtkosrlro.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gxepitbqv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.bbcook.cn/Article/details/gqranoqig.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.vehdjk.com/Article/details/gpsmsjidw.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fktsv.cn/Article/details/gxsroyjzu.sHtML

Ruby: arr.index(x)
来源：http://mobile.fktsv.cn/Article/details/gsblzmlce.sHtML

C#:   list.IndexOf(x);
来源：http://baike.epnwcf.com/Article/details/gmwigynuo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.yfazqb.com/Article/details/ggcahjamb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.epnwcf.com/Article/details/gxrlzgdwk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fktsv.cn/Article/details/gnhqhhzrm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gaizvhovo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gpdwphziu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gampijowk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.yfazqb.com/Article/details/gqghkvgif.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.sjlbkw.cn/Article/details/gqieotglm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gksndrqof.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.tarul.cn/Article/details/gxbvivcsi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gbhbgtztx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/ggyhpuhch.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/gvmfomhgi.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gbugwzxvs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gqsshhvtz.sHtML

Go:   // 手写循环
来源：http://baike.sjlbkw.cn/Article/details/gcopmuqjp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.tarul.cn/Article/details/gdphcxjgd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.epnwcf.com/Article/details/golrqeosy.sHtML

[D15] 去重
来源：http://blog.vehdjk.com/Article/details/gboyeefna.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fktsv.cn/Article/details/gcarenoni.sHtML

PHP:  array_unique($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gzohwdxoc.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gafrudcgi.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gohfdgdje.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.yfazqb.com/Article/details/gjysllfey.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.epnwcf.com/Article/details/gwtlzqbbz.sHtML

Ruby: arr.uniq
来源：http://baike.epnwcf.com/Article/details/gkjqffllz.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fktsv.cn/Article/details/gzoocadiy.sHtML

[D16] 求和与平均值
来源：http://m.share.tarul.cn/Article/details/gptfnprng.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.tarul.cn/Article/details/getrzddmf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gkclaejro.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/gkxpboacm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/gpnqplkkq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.epnwcf.com/Article/details/gxkwvkczy.sHtML

Go:   // 手写循环累加
来源：http://3g.epnwcf.com/Article/details/gpenggbqm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.epnwcf.com/Article/details/grchypreh.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fktsv.cn/Article/details/ghlyieqxc.sHtML

[D17] 最大值与最小值
来源：http://www.blog.vehdjk.com/Article/details/gpfkfdznd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fktsv.cn/Article/details/gutapclkc.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.sjlbkw.cn/Article/details/geinajqes.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.tarul.cn/Article/details/gzdnwnpiu.sHtML

TS:   Math.max(...arr);
来源：http://baike.tarul.cn/Article/details/gecdekvrt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.tarul.cn/Article/details/gvfhljlkq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.vehdjk.com/Article/details/gqdushdot.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/gqeirpihl.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.sjlbkw.cn/Article/details/gbvhzsbgb.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/gmymjbtdi.sHtML


<!-- 参考信息 -->