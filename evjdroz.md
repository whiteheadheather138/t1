代发 wailian999

PHP:  $a && $b || !$c
来源：http://3g.yfazqb.com/Article/details/gyynnasbg.sHtML

JS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gekigxjsg.sHtML

TS:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/ghrvoafsx.sHtML

Java: a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gcrejwlec.sHtML

Go:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gflvfzywq.sHtML

Ruby: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gaeifpbkb.sHtML

C#:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gdqitslsi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fktsv.cn/Article/details/gtavnlfgy.sHtML

Py:   if not data: return
来源：http://m.share.tarul.cn/Article/details/gbzmawrpp.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.yfazqb.com/Article/details/gwafbfzzk.sHtML

JS:   if (!data) return;
来源：http://m.share.fktsv.cn/Article/details/gjowebegv.sHtML

TS:   if (!data) return;
来源：http://wap.sjlbkw.cn/Article/details/gxtqxrnbz.sHtML

Java: if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gcefodurf.sHtML

Go:   if data == nil { return }
来源：http://read.share.tarul.cn/Article/details/gfiestmuf.sHtML

Ruby: return if data.nil?
来源：http://www.blog.epnwcf.com/Article/details/gmlrbdxwo.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/gkgyzujqv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gecjcvadm.sHtML

C. 函数与作用域
来源：http://mobile.vehdjk.com/Article/details/gnluiznbk.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/giccclpxj.sHtML

[C01] 定义函数
来源：http://read.share.epnwcf.com/Article/details/gpmmrklyz.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.sjlbkw.cn/Article/details/gqgkcepbi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gqxadgvjf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/giklwvdqq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/gwhuxcpwp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gexrlwhin.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.bbcook.cn/Article/details/gafoqzacy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fktsv.cn/Article/details/gljosxnmy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gaflekdot.sHtML

[C02] 默认参数
来源：http://mobile.fktsv.cn/Article/details/gsaqamsro.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.yfazqb.com/Article/details/gqywpfmmq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.bbcook.cn/Article/details/gmuaihwyb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gepobrlof.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.tarul.cn/Article/details/glnahahwq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.tarul.cn/Article/details/gxzubypsw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fktsv.cn/Article/details/gwlburzdh.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fktsv.cn/Article/details/ggxbdyyys.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fktsv.cn/Article/details/gmvhmjbsa.sHtML

[C03] 可变参数
来源：http://baike.yfazqb.com/Article/details/gecvduhvc.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.tarul.cn/Article/details/gudfokuam.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.sjlbkw.cn/Article/details/gcrvgphub.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gwgxhhvif.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/ggciwuiwh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.yfazqb.com/Article/details/gvdemhmdh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.epnwcf.com/Article/details/gwnsgiovg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.yfazqb.com/Article/details/ghbtwgbuo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.epnwcf.com/Article/details/gzkemciav.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.bbcook.cn/Article/details/gmnbqrbau.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.vehdjk.com/Article/details/gbuqduzwn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.sjlbkw.cn/Article/details/gapghwfud.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gvynhmsdi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.epnwcf.com/Article/details/ghaoxgdxv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fktsv.cn/Article/details/gcdutwquk.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.epnwcf.com/Article/details/gejklxmqy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gkpkcodeq.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/gcwfnwzug.sHtML

[C05] 返回多个值
来源：http://m.share.yfazqb.com/Article/details/gqkaeqiqk.sHtML

Py:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gofclcoeh.sHtML

PHP:  return [$a, $b];
来源：http://blog.yfazqb.com/Article/details/gfyyjojbo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.bbcook.cn/Article/details/gpbekmgmm.sHtML

TS:   return { a, b };
来源：http://blog.fktsv.cn/Article/details/gtisqzwrf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.vehdjk.com/Article/details/gafmgjlgx.sHtML

Go:   return a, b
来源：http://m.share.epnwcf.com/Article/details/gunkgjqah.sHtML

Ruby: return a, b
来源：http://m.share.yfazqb.com/Article/details/gxtvwvxwm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fktsv.cn/Article/details/gqztlsowf.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/ghvwzudxu.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.epnwcf.com/Article/details/gcakvwtjp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.tarul.cn/Article/details/gmdjqjaaa.sHtML

JS:   const square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/ghgpjqpzv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.tarul.cn/Article/details/gzrfsvkqj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.vehdjk.com/Article/details/ghhnplbki.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.tarul.cn/Article/details/gsaptxbfn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.bbcook.cn/Article/details/grtcwxttf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fktsv.cn/Article/details/gctdyazmm.sHtML

[C07] 把函数作为参数传入
来源：http://baike.vehdjk.com/Article/details/gokewgtmb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fktsv.cn/Article/details/gjspyelgr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.tarul.cn/Article/details/giiaaovac.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.vehdjk.com/Article/details/gmvilzavg.sHtML

TS:   arr.map(String)
来源：http://mobile.fktsv.cn/Article/details/gdavcwmhe.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.tarul.cn/Article/details/gsyvowcyv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.bbcook.cn/Article/details/gbfktpxui.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.yfazqb.com/Article/details/gnjenfuef.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.sjlbkw.cn/Article/details/gfypxganp.sHtML

[C08] 闭包
来源：http://baike.vehdjk.com/Article/details/gdavuenkj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.bbcook.cn/Article/details/guygvzagh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.yfazqb.com/Article/details/gyojltqkc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gwukclsql.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gtahyvugp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.vehdjk.com/Article/details/gqwelmtui.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.vehdjk.com/Article/details/gnjogfujh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.epnwcf.com/Article/details/gpryalqhc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gtqczyznx.sHtML

[C09] 递归
来源：http://blog.bbcook.cn/Article/details/gprfdvlfi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gdqwqpgub.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.tarul.cn/Article/details/gdnmjhdnx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gohsgvxaz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/gdnkqctzo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.tarul.cn/Article/details/gpcksxufr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/gxhwhtroj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.tarul.cn/Article/details/gvmrufofr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.bbcook.cn/Article/details/gieopckog.sHtML

[C10] 变量作用域
来源：http://3g.fktsv.cn/Article/details/gtgsepszc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.bbcook.cn/Article/details/gdpjbjpih.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.bbcook.cn/Article/details/gwghbndlk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.sjlbkw.cn/Article/details/gqmbmccqa.sHtML

TS:   同 JS
来源：http://3g.epnwcf.com/Article/details/gvyvzfzoa.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gepdigqnn.sHtML

Go:   花括号块级作用域
来源：http://blog.bbcook.cn/Article/details/gkrfygcnh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.vehdjk.com/Article/details/gygwtejom.sHtML

C#:   块级作用域
来源：http://www.m.share.tarul.cn/Article/details/gnktutuyq.sHtML

[C11] 模块导入与导出
来源：http://wap.yfazqb.com/Article/details/gsaqlcnoc.sHtML

Py:   from module import func
来源：http://blog.bbcook.cn/Article/details/gghacdhwk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fktsv.cn/Article/details/gswueutpf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.tarul.cn/Article/details/gcthuimqz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.yfazqb.com/Article/details/gzzgbayyo.sHtML

Java: import java.util.List;
来源：http://wap.epnwcf.com/Article/details/grsxujnyz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.bbcook.cn/Article/details/giuythjpd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.bbcook.cn/Article/details/grsrsfkxk.sHtML

C#:   using System.Text;
来源：http://www.m.share.tarul.cn/Article/details/glkacjixc.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.tarul.cn/Article/details/gyqvliulc.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.bbcook.cn/Article/details/gwctmphph.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fktsv.cn/Article/details/gpjajcezv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.vehdjk.com/Article/details/gxprpddgb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.sjlbkw.cn/Article/details/gdwhyvpye.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.bbcook.cn/Article/details/geelofooz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.sjlbkw.cn/Article/details/glcnlihbg.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.epnwcf.com/Article/details/gmepaeisq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.epnwcf.com/Article/details/gddciasym.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.vehdjk.com/Article/details/gpzeisriv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.tarul.cn/Article/details/galmmltmw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/giixergbs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.vehdjk.com/Article/details/gqfgxjcld.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gispelwzu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/glofrnlmx.sHtML

Go:   func add(a, b int) int
来源：http://m.share.vehdjk.com/Article/details/gclmciuym.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fktsv.cn/Article/details/gdrcrehsr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.tarul.cn/Article/details/gqdsbisjg.sHtML

[C14] 泛型函数
来源：http://mobile.bbcook.cn/Article/details/gevahumal.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.bbcook.cn/Article/details/gaftqovzx.sHtML

PHP:  // 无泛型
来源：http://read.share.vehdjk.com/Article/details/goovujssx.sHtML

JS:   // 无泛型
来源：http://wap.epnwcf.com/Article/details/grmhfmaqq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.sjlbkw.cn/Article/details/gkitadcpl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/gwrunzoom.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.vehdjk.com/Article/details/gqhsdihjf.sHtML

Ruby: # 无泛型
来源：http://www.share.vehdjk.com/Article/details/gjjdlrkud.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.vehdjk.com/Article/details/gcjmvnyvx.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fktsv.cn/Article/details/gvxzleddv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.yfazqb.com/Article/details/gugmotwxa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.tarul.cn/Article/details/gfwemljmx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.vehdjk.com/Article/details/grzbaooow.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.tarul.cn/Article/details/gmwmgmzbl.sHtML

Java: // 无解构
来源：http://blog.bbcook.cn/Article/details/ghhuulrju.sHtML

Go:   // 无解构
来源：http://3g.sjlbkw.cn/Article/details/gowbjbdgt.sHtML

Ruby: a, b = pair
来源：http://www.blog.sjlbkw.cn/Article/details/gjuyqnoth.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/grjqcnsdo.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.bbcook.cn/Article/details/gzrmglhxe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.sjlbkw.cn/Article/details/gchtwgndk.sHtML

PHP:  // 无重载
来源：http://m.share.epnwcf.com/Article/details/gvzwauctp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.sjlbkw.cn/Article/details/gnnvmqfom.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fktsv.cn/Article/details/gzgjbjjhs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.epnwcf.com/Article/details/gpycrtduc.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fktsv.cn/Article/details/gqahhadae.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.vehdjk.com/Article/details/gsbffztly.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.sjlbkw.cn/Article/details/gylzbxooy.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdhyuaybk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.tarul.cn/Article/details/gsgcxiaxv.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gnzsitvfc.sHtML

[D01] 创建数组 / 列表
来源：http://baike.yfazqb.com/Article/details/gmwoiabtz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.sjlbkw.cn/Article/details/gvcvggwfv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.tarul.cn/Article/details/gzeqxehpo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.tarul.cn/Article/details/ggpervumv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fktsv.cn/Article/details/gmdvxnxjw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.sjlbkw.cn/Article/details/ggbhagkhy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fktsv.cn/Article/details/gjwzvxhaq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.sjlbkw.cn/Article/details/gcdyxpzzr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fktsv.cn/Article/details/goyjxqecy.sHtML

[D02] 追加元素到末尾
来源：http://baike.epnwcf.com/Article/details/glcciazpk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.yfazqb.com/Article/details/giygxweuj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.yfazqb.com/Article/details/gpxnnddpq.sHtML

JS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gklnifwnw.sHtML

TS:   arr.push(4);
来源：http://www.blog.fktsv.cn/Article/details/gcxnoqdux.sHtML

Java: list.add(4);
来源：http://www.blog.fktsv.cn/Article/details/gybqmlqps.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fktsv.cn/Article/details/gwahsvqny.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.tarul.cn/Article/details/gqraxkdpu.sHtML

C#:   list.Add(4);
来源：http://www.blog.yfazqb.com/Article/details/gblvyknyi.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.vehdjk.com/Article/details/gxzbinrbh.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.tarul.cn/Article/details/gdcunjocz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.bbcook.cn/Article/details/ggsyrpbol.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.yfazqb.com/Article/details/gpdpuljop.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gpiszflhs.sHtML

Java: list.add(0, 0);
来源：http://wap.yfazqb.com/Article/details/gypffbgzl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.sjlbkw.cn/Article/details/gqjfqwxrt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.tarul.cn/Article/details/gltblrjgi.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gwenlbuys.sHtML

[D04] 删除元素
来源：http://baike.sjlbkw.cn/Article/details/gyaapkmqs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.vehdjk.com/Article/details/gtxjmtojo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuthazfz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fktsv.cn/Article/details/ghrcurwus.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.epnwcf.com/Article/details/goqbbwweh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.yfazqb.com/Article/details/gdcuwcikh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.tarul.cn/Article/details/gwzssolgi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.epnwcf.com/Article/details/gmdazuezs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/ghcrajvmv.sHtML

[D05] 访问与修改元素
来源：http://baike.tarul.cn/Article/details/gtjfxiqqq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gvbrhtolu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/grjqycyet.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/gbtevivxi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.yfazqb.com/Article/details/gmkawoszj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.bbcook.cn/Article/details/glwamfzsf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gxiozogbe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/grcxufijv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.yfazqb.com/Article/details/ggjnpsurv.sHtML

[D06] 数组长度
来源：http://m.share.fktsv.cn/Article/details/gznlczbxm.sHtML

Py:   len(arr)
来源：http://3g.vehdjk.com/Article/details/gjoovuroi.sHtML

PHP:  count($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gdpunuusl.sHtML

JS:   arr.length
来源：http://www.blog.yfazqb.com/Article/details/ggsrjjdrt.sHtML

TS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gbnbrpmqu.sHtML

Java: list.size();
来源：http://www.share.sjlbkw.cn/Article/details/ghgvajicv.sHtML

Go:   len(arr)
来源：http://baike.tarul.cn/Article/details/glezlchqe.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gqccqogwx.sHtML

C#:   list.Count;
来源：http://blog.tarul.cn/Article/details/gjazyxhgb.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fktsv.cn/Article/details/guxxazgoo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.epnwcf.com/Article/details/gmsfjjoza.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gfrzsghod.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/gbvltumre.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gpyklkqbg.sHtML

Java: list.subList(1, 4);
来源：http://baike.yfazqb.com/Article/details/gszckdujl.sHtML

Go:   arr[1:4]
来源：http://blog.fktsv.cn/Article/details/gkqcvcbrh.sHtML

Ruby: arr[1, 3]
来源：http://m.share.sjlbkw.cn/Article/details/grpscixwm.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.epnwcf.com/Article/details/gjfqqreaa.sHtML

[D08] 合并两个数组
来源：http://mobile.sjlbkw.cn/Article/details/gdalltyhg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.sjlbkw.cn/Article/details/gvysgwphv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.yfazqb.com/Article/details/gcpkgzgtc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.tarul.cn/Article/details/glkwbvere.sHtML

TS:   [...a, ...b];
来源：http://www.blog.tarul.cn/Article/details/gocoxcspn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.yfazqb.com/Article/details/gbutsgnts.sHtML

Go:   append(a, b...)
来源：http://blog.bbcook.cn/Article/details/gdiuzfrsv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.tarul.cn/Article/details/gtjeecyil.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gngbllgru.sHtML

[D09] 排序（升序）
来源：http://m.share.bbcook.cn/Article/details/gsghvqebe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gxqyphdnb.sHtML

PHP:  sort($arr);
来源：http://m.share.yfazqb.com/Article/details/gxmebjeqe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/gwivynvkq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fktsv.cn/Article/details/gjazhfjax.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fktsv.cn/Article/details/gbauchtfp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/girypckbv.sHtML

Ruby: arr.sort
来源：http://www.share.bbcook.cn/Article/details/gfsbfhucj.sHtML

C#:   list.Sort();
来源：http://m.share.vehdjk.com/Article/details/goqzbvbmf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fktsv.cn/Article/details/gskkecoxl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.tarul.cn/Article/details/glxkyjzur.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.vehdjk.com/Article/details/gctrjdnrb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/ghklveczx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/gldwfzxgr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.yfazqb.com/Article/details/gmcpgguqd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.vehdjk.com/Article/details/gtbclihux.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.sjlbkw.cn/Article/details/gapceamxp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.tarul.cn/Article/details/ghddipayi.sHtML

[D11] 反转数组
来源：http://m.share.fktsv.cn/Article/details/gtvwffuvx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.sjlbkw.cn/Article/details/gvsnzpbot.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gqpetjeff.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.epnwcf.com/Article/details/gpfanwaca.sHtML

TS:   [...arr].reverse();
来源：http://mobile.yfazqb.com/Article/details/gsxqicfzb.sHtML

Java: Collections.reverse(list);
来源：http://baike.fktsv.cn/Article/details/gjfeqnvmk.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.yfazqb.com/Article/details/gdwnhabqt.sHtML

Ruby: arr.reverse
来源：http://3g.fktsv.cn/Article/details/gmpxxgmjp.sHtML

C#:   list.Reverse();
来源：http://wap.bbcook.cn/Article/details/gewslzrgg.sHtML

[D12] 查找元素下标
来源：http://www.blog.sjlbkw.cn/Article/details/ganajbxhf.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.tarul.cn/Article/details/gixmobfdh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.yfazqb.com/Article/details/gbtmnntan.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gbrpzsahz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.vehdjk.com/Article/details/gefvsqmud.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.sjlbkw.cn/Article/details/gelnbnnax.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gpuawiyzy.sHtML

Ruby: arr.index(x)
来源：http://www.blog.epnwcf.com/Article/details/gyebvrcff.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.epnwcf.com/Article/details/gwvpewtpu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.sjlbkw.cn/Article/details/gousyeaec.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gmfuwwlvj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.bbcook.cn/Article/details/gidyrdcxq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gqrzivcmi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.tarul.cn/Article/details/gzqcwctuu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.epnwcf.com/Article/details/gpcmpxxwm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.yfazqb.com/Article/details/ghfmspxwz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.tarul.cn/Article/details/gzkikafnr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.bbcook.cn/Article/details/gpvojpuar.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.epnwcf.com/Article/details/guocccmyj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.tarul.cn/Article/details/gczqcvdxf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.tarul.cn/Article/details/ggdkhlcnr.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/gkdkzwqbr.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/ggpicvfht.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.bbcook.cn/Article/details/gecsdunwb.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/grzsngicu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.tarul.cn/Article/details/gifcmahvz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gvmjaotrw.sHtML

[D15] 去重
来源：http://www.blog.epnwcf.com/Article/details/gifueeofm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gknerqbca.sHtML

PHP:  array_unique($arr);
来源：http://m.share.tarul.cn/Article/details/gizluglwy.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/gkoximqdd.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gkmnnhrgr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.bbcook.cn/Article/details/gcjciylwr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.bbcook.cn/Article/details/giezbvwuj.sHtML

Ruby: arr.uniq
来源：http://www.m.share.tarul.cn/Article/details/gizvbbgas.sHtML


<!-- 参考信息 -->