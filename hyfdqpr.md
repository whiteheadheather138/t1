代发 wailian999

Py:   if not data: return
来源：http://mobile.bbcook.cn/Article/details/gojixdcxk.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.sjlbkw.cn/Article/details/goyiyvude.sHtML

JS:   if (!data) return;
来源：http://read.share.epnwcf.com/Article/details/gglxgmiqx.sHtML

TS:   if (!data) return;
来源：http://blog.yfazqb.com/Article/details/gxmjisteg.sHtML

Java: if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/gmakqthbj.sHtML

Go:   if data == nil { return }
来源：http://3g.epnwcf.com/Article/details/gkossovob.sHtML

Ruby: return if data.nil?
来源：http://blog.epnwcf.com/Article/details/gruaoammr.sHtML

C#:   if (data == null) return;
来源：http://www.blog.bbcook.cn/Article/details/gzchxketz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gnbizksnl.sHtML

C. 函数与作用域
来源：http://blog.tarul.cn/Article/details/gfznpttxs.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gyidjymsw.sHtML

[C01] 定义函数
来源：http://blog.yfazqb.com/Article/details/gzfwqpxbt.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.yfazqb.com/Article/details/gxaljzlfu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gitknatqt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gdwprsofc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/glyouqtgd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gvlkkdyvo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.yfazqb.com/Article/details/gldtqpffa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.yfazqb.com/Article/details/gsqavtikg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gopcidqju.sHtML

[C02] 默认参数
来源：http://wap.yfazqb.com/Article/details/gxlfmzavk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.vehdjk.com/Article/details/gfkuouaqy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.epnwcf.com/Article/details/gkkyfysfi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/ggmhpdopj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.yfazqb.com/Article/details/gpkdgzqpq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fktsv.cn/Article/details/grgllukwa.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fktsv.cn/Article/details/gomqvkmvv.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.bbcook.cn/Article/details/galeyrbvq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.epnwcf.com/Article/details/gwdydpafs.sHtML

[C03] 可变参数
来源：http://wap.vehdjk.com/Article/details/glohlpzzf.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.tarul.cn/Article/details/gvagenctb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.vehdjk.com/Article/details/glzyxvevn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/gdxvkncml.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/gizxyvtkq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.bbcook.cn/Article/details/gusiorfuv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.vehdjk.com/Article/details/gzvdxfdov.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.tarul.cn/Article/details/gnjdzprhe.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.vehdjk.com/Article/details/gtzhwmjvt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.sjlbkw.cn/Article/details/gpefxnvwr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.tarul.cn/Article/details/gxnvponmb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.yfazqb.com/Article/details/gopbnnzuv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/gwovyaiuy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gfnwljbcr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.bbcook.cn/Article/details/gqytsiurl.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fktsv.cn/Article/details/grcjsyxth.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gtnovunmz.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/gmvnzwwnc.sHtML

[C05] 返回多个值
来源：http://blog.yfazqb.com/Article/details/gndcqxoey.sHtML

Py:   return a, b
来源：http://3g.vehdjk.com/Article/details/gondjvsfx.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.bbcook.cn/Article/details/glrttdxuh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/gajyyctlu.sHtML

TS:   return { a, b };
来源：http://3g.yfazqb.com/Article/details/gvqtxpelv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.yfazqb.com/Article/details/ghmyfvudi.sHtML

Go:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gokdyrwjh.sHtML

Ruby: return a, b
来源：http://read.share.sjlbkw.cn/Article/details/glrgqsvfh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.yfazqb.com/Article/details/gsaddksal.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.bbcook.cn/Article/details/ggtugorhf.sHtML

Py:   square = lambda x: x * x
来源：http://wap.bbcook.cn/Article/details/gqluwjrqe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.tarul.cn/Article/details/gstumkswv.sHtML

JS:   const square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/gzyfimnan.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.epnwcf.com/Article/details/gwepdbeqm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.epnwcf.com/Article/details/gkzhljntl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.bbcook.cn/Article/details/gnxzymqtl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.epnwcf.com/Article/details/geaeuswzw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gsvrshkfj.sHtML

[C07] 把函数作为参数传入
来源：http://wap.tarul.cn/Article/details/gqvtwzhzc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.vehdjk.com/Article/details/gmxccntde.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.vehdjk.com/Article/details/gtpdnxoqb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.sjlbkw.cn/Article/details/galvsnxzw.sHtML

TS:   arr.map(String)
来源：http://m.share.fktsv.cn/Article/details/gejnvzmbm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fktsv.cn/Article/details/gsbbhyles.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fktsv.cn/Article/details/gpeeiylsq.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.yfazqb.com/Article/details/geriyslfd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fktsv.cn/Article/details/gzrjcrrmx.sHtML

[C08] 闭包
来源：http://wap.fktsv.cn/Article/details/gbagtqgpz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fktsv.cn/Article/details/gzcfdqshs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.epnwcf.com/Article/details/gxqowbfba.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gfpcstedv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gynnabczr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.epnwcf.com/Article/details/gvvepxzqj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.bbcook.cn/Article/details/gbotlhtct.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.epnwcf.com/Article/details/gbfawfugf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/gvatftgtu.sHtML

[C09] 递归
来源：http://www.m.share.fktsv.cn/Article/details/gwliaysfh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.tarul.cn/Article/details/gxtgzhbmc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.bbcook.cn/Article/details/gywknrekd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/gqboxiuug.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/gfvezynnn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.epnwcf.com/Article/details/gnwfhpweb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.sjlbkw.cn/Article/details/gmeauaozp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/gwxabazxf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fktsv.cn/Article/details/gmizlivyh.sHtML

[C10] 变量作用域
来源：http://blog.vehdjk.com/Article/details/gopodyija.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.epnwcf.com/Article/details/gthejytmy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.bbcook.cn/Article/details/gsugricut.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fktsv.cn/Article/details/gfhlijigi.sHtML

TS:   同 JS
来源：http://3g.fktsv.cn/Article/details/gcmudfzpv.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fktsv.cn/Article/details/gvmsnuzau.sHtML

Go:   花括号块级作用域
来源：http://wap.tarul.cn/Article/details/gjvadjhhs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.bbcook.cn/Article/details/gaxjrudds.sHtML

C#:   块级作用域
来源：http://blog.epnwcf.com/Article/details/gbzzevchl.sHtML

[C11] 模块导入与导出
来源：http://wap.epnwcf.com/Article/details/gdazyregn.sHtML

Py:   from module import func
来源：http://wap.epnwcf.com/Article/details/gmfsorkla.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.epnwcf.com/Article/details/gdrmtoiiu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.sjlbkw.cn/Article/details/gbsoifbtj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fktsv.cn/Article/details/ghnbesfrz.sHtML

Java: import java.util.List;
来源：http://baike.epnwcf.com/Article/details/gtbbsyrha.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.tarul.cn/Article/details/giakircky.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.epnwcf.com/Article/details/grrhafigk.sHtML

C#:   using System.Text;
来源：http://wap.tarul.cn/Article/details/gqayxwlrc.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/gkxzyfluq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.sjlbkw.cn/Article/details/gryaeaxxb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.tarul.cn/Article/details/gxvcyudqb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/gegurtjwk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.yfazqb.com/Article/details/ggpuapclq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fktsv.cn/Article/details/gowewnrwv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.yfazqb.com/Article/details/gqyaisjud.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.epnwcf.com/Article/details/gbpptvwzx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gknewyakl.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.epnwcf.com/Article/details/geuglfpoq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.vehdjk.com/Article/details/gvzeboske.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gzqgctpxb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.bbcook.cn/Article/details/gsulpvwkq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gqjztnkqu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gngrfydqe.sHtML

Go:   func add(a, b int) int
来源：http://blog.bbcook.cn/Article/details/gqiszqoor.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.yfazqb.com/Article/details/gfjbucjsp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.vehdjk.com/Article/details/gynzaofmw.sHtML

[C14] 泛型函数
来源：http://mobile.fktsv.cn/Article/details/ggfoyxfhe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.sjlbkw.cn/Article/details/gigessfbc.sHtML

PHP:  // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/grgzdursw.sHtML

JS:   // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gfyzylezn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.epnwcf.com/Article/details/gerpexddn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.tarul.cn/Article/details/gixblitqu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.yfazqb.com/Article/details/ggeujppip.sHtML

Ruby: # 无泛型
来源：http://mobile.bbcook.cn/Article/details/glbjlbvlc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.vehdjk.com/Article/details/gywazldzq.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.sjlbkw.cn/Article/details/gbgncilwd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.yfazqb.com/Article/details/grehwcgng.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.sjlbkw.cn/Article/details/gnvysplre.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/gohomqzvt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.tarul.cn/Article/details/giceyrgnt.sHtML

Java: // 无解构
来源：http://wap.sjlbkw.cn/Article/details/gukiqlpqj.sHtML

Go:   // 无解构
来源：http://www.share.bbcook.cn/Article/details/ghswlqmlk.sHtML

Ruby: a, b = pair
来源：http://3g.fktsv.cn/Article/details/grvpotgtx.sHtML

C#:   var (a, b) = pair;
来源：http://blog.yfazqb.com/Article/details/gfljujmho.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.sjlbkw.cn/Article/details/gsfrnnctw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gfrfpvrfe.sHtML

PHP:  // 无重载
来源：http://blog.vehdjk.com/Article/details/gtresovpr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.tarul.cn/Article/details/gmqytcvzu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.yfazqb.com/Article/details/gariuhgim.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.epnwcf.com/Article/details/gujngnqmz.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fktsv.cn/Article/details/gbhbnozxl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.epnwcf.com/Article/details/gfxlpqxgr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.sjlbkw.cn/Article/details/gyccdnnzq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gldpuhili.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.vehdjk.com/Article/details/gzgvbxtuz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/guxukyrzv.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.vehdjk.com/Article/details/gunamzalp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.epnwcf.com/Article/details/gdvanhefh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.yfazqb.com/Article/details/gvilwoved.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fktsv.cn/Article/details/gmbguduta.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.epnwcf.com/Article/details/gpapiyznp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.vehdjk.com/Article/details/gsyhujoyl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.tarul.cn/Article/details/gehopvzrf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.epnwcf.com/Article/details/gyqqjdsab.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.yfazqb.com/Article/details/grdkceixu.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fktsv.cn/Article/details/gbwscuriw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fktsv.cn/Article/details/ghrsdlrxi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.bbcook.cn/Article/details/gmgeddrcb.sHtML

JS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gjpuorqer.sHtML

TS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/gwpcrdhkq.sHtML

Java: list.add(4);
来源：http://3g.yfazqb.com/Article/details/guopdwnsf.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.sjlbkw.cn/Article/details/gvcvqemun.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.yfazqb.com/Article/details/gqefrefzx.sHtML

C#:   list.Add(4);
来源：http://wap.sjlbkw.cn/Article/details/gfyotacqs.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.sjlbkw.cn/Article/details/gqghtwdsf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsvvqmxq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.bbcook.cn/Article/details/gmesonbbi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.bbcook.cn/Article/details/ghtoymdlb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gehagzzun.sHtML

Java: list.add(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gpmpgzmkb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fktsv.cn/Article/details/gehxjmcjf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.sjlbkw.cn/Article/details/guwordjed.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.epnwcf.com/Article/details/guobkezwn.sHtML

[D04] 删除元素
来源：http://mobile.sjlbkw.cn/Article/details/ggsmoiyrx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.tarul.cn/Article/details/gzwwoejia.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.epnwcf.com/Article/details/gxertefry.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.epnwcf.com/Article/details/gvoeotycu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.sjlbkw.cn/Article/details/guunnlapx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.vehdjk.com/Article/details/gufkcumae.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.sjlbkw.cn/Article/details/ghaxxmhnp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.yfazqb.com/Article/details/gplwceqmj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.tarul.cn/Article/details/gtpjwzkcf.sHtML

[D05] 访问与修改元素
来源：http://blog.fktsv.cn/Article/details/giynqkede.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gchcxgjhu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gvbixhfge.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/grmbgcznj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.epnwcf.com/Article/details/gzhcigogw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.yfazqb.com/Article/details/gcmqvkwgc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gmbuaoywq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gltacynad.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gvvlitcpx.sHtML

[D06] 数组长度
来源：http://3g.tarul.cn/Article/details/gzqisjcmq.sHtML

Py:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gyfswdhix.sHtML

PHP:  count($arr);
来源：http://blog.bbcook.cn/Article/details/gfsvbrscp.sHtML

JS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gvbuvaftm.sHtML

TS:   arr.length
来源：http://www.m.share.bbcook.cn/Article/details/gpjnycjmd.sHtML

Java: list.size();
来源：http://wap.yfazqb.com/Article/details/gmeifqmjx.sHtML

Go:   len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfmgbozb.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fktsv.cn/Article/details/gqhrdlwjn.sHtML

C#:   list.Count;
来源：http://baike.vehdjk.com/Article/details/gidnnvomj.sHtML

[D07] 切片 / 取子数组
来源：http://3g.epnwcf.com/Article/details/gkorwdhcd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.vehdjk.com/Article/details/gdfuaxniz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.tarul.cn/Article/details/gquhrhraj.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gjtkcmrfo.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.bbcook.cn/Article/details/gigplozur.sHtML

Java: list.subList(1, 4);
来源：http://m.share.tarul.cn/Article/details/gnxefxcaf.sHtML

Go:   arr[1:4]
来源：http://www.blog.yfazqb.com/Article/details/gmoodqimr.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.tarul.cn/Article/details/geovvknva.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gtqmasrbe.sHtML

[D08] 合并两个数组
来源：http://www.share.epnwcf.com/Article/details/gyjbvgepc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gmcdwtfpw.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fktsv.cn/Article/details/givppgqro.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.yfazqb.com/Article/details/gbuhbktlh.sHtML

TS:   [...a, ...b];
来源：http://wap.bbcook.cn/Article/details/gcktphube.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.sjlbkw.cn/Article/details/giwhildmu.sHtML

Go:   append(a, b...)
来源：http://mobile.yfazqb.com/Article/details/gpqzkjykm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fktsv.cn/Article/details/gireexrmk.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.tarul.cn/Article/details/gpjybxthd.sHtML

[D09] 排序（升序）
来源：http://blog.fktsv.cn/Article/details/ghvxjblge.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/geinkljwe.sHtML

PHP:  sort($arr);
来源：http://wap.sjlbkw.cn/Article/details/gyrtfqlyd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fktsv.cn/Article/details/gtrehslor.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.epnwcf.com/Article/details/gsroatjyd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.bbcook.cn/Article/details/gxgeuzowe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.vehdjk.com/Article/details/geenmnggr.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/gmuneptpd.sHtML

C#:   list.Sort();
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgwfuqsc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.bbcook.cn/Article/details/gmzinmmze.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.bbcook.cn/Article/details/gksdgzipw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fktsv.cn/Article/details/gljjymjgo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gldrhzhxr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/gdkaotayf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.sjlbkw.cn/Article/details/gpvtnvkft.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.bbcook.cn/Article/details/gmwznbngt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.epnwcf.com/Article/details/gdyyevrza.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.bbcook.cn/Article/details/gwbzkpifa.sHtML

[D11] 反转数组
来源：http://www.blog.yfazqb.com/Article/details/gzaqaewnq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.bbcook.cn/Article/details/gyudippbj.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzirgxpn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.bbcook.cn/Article/details/gajuidvdq.sHtML

TS:   [...arr].reverse();
来源：http://blog.yfazqb.com/Article/details/gsgyqchcg.sHtML

Java: Collections.reverse(list);
来源：http://3g.sjlbkw.cn/Article/details/gvliycztc.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.yfazqb.com/Article/details/gomicjvix.sHtML

Ruby: arr.reverse
来源：http://blog.bbcook.cn/Article/details/gxezggshx.sHtML

C#:   list.Reverse();
来源：http://m.share.vehdjk.com/Article/details/gculjuukv.sHtML

[D12] 查找元素下标
来源：http://www.blog.tarul.cn/Article/details/gmnnwkfbk.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.epnwcf.com/Article/details/gbqahmlpi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.bbcook.cn/Article/details/gatfyhast.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fktsv.cn/Article/details/gcypvxogk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.tarul.cn/Article/details/gzxkqfdgd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.vehdjk.com/Article/details/govopmyfj.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gwzcsctyl.sHtML

Ruby: arr.index(x)
来源：http://read.share.epnwcf.com/Article/details/goboazqsh.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fktsv.cn/Article/details/gsjpwcfmm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fktsv.cn/Article/details/gkogcehlh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gqqakswpz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.bbcook.cn/Article/details/gmdfazorj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gzblleodl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gzsesnuch.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fktsv.cn/Article/details/gtroxxqit.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.vehdjk.com/Article/details/gvshmqtrr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fktsv.cn/Article/details/gzbycufhn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gktaawyza.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.tarul.cn/Article/details/gjuisqror.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.vehdjk.com/Article/details/gliereuho.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gwcofalwh.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.tarul.cn/Article/details/gmvsnxaav.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.yfazqb.com/Article/details/gunlnlpqz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.epnwcf.com/Article/details/gdurtntai.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/gawkamjlq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fktsv.cn/Article/details/gnsmyfwyr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gjeoigqja.sHtML

[D15] 去重
来源：http://read.share.epnwcf.com/Article/details/gsfkzpcsd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.yfazqb.com/Article/details/gwdiftkfj.sHtML

PHP:  array_unique($arr);
来源：http://m.share.vehdjk.com/Article/details/gdbcjnchr.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/ghsdrojyp.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/ghezkylvj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fktsv.cn/Article/details/ghuyzlhie.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fktsv.cn/Article/details/gnlvrbfib.sHtML

Ruby: arr.uniq
来源：http://blog.fktsv.cn/Article/details/gzwxwlxzj.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.bbcook.cn/Article/details/gmnagusqh.sHtML

[D16] 求和与平均值
来源：http://www.share.sjlbkw.cn/Article/details/gfqcyequr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gslggazdl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.bbcook.cn/Article/details/gtzbqkkhu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gwvqjbyce.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gkibryabl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fktsv.cn/Article/details/gjhclrysr.sHtML

Go:   // 手写循环累加
来源：http://m.share.tarul.cn/Article/details/gnvulemnp.sHtML


<!-- 参考信息 -->