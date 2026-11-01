代发 wailian999

Py:   def add(a, b): return a + b
来源：http://read.share.bbcook.cn/Article/details/gfccyiokt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gfkwkfeqp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gjqpaxdvd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gbitycjqo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/ggptpwiea.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.tarul.cn/Article/details/gyeznosti.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.sjlbkw.cn/Article/details/gcxiigify.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gjmpwovyt.sHtML

[C02] 默认参数
来源：http://blog.tarul.cn/Article/details/gldjwmtyc.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.sjlbkw.cn/Article/details/ggigeoqra.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.tarul.cn/Article/details/gcanetmik.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gbfkilsdl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fktsv.cn/Article/details/gzwdpzgei.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.bbcook.cn/Article/details/gkaxwqnrl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.yfazqb.com/Article/details/gfbiyvjqc.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.yfazqb.com/Article/details/gdwazvror.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fktsv.cn/Article/details/gsxxnuzxo.sHtML

[C03] 可变参数
来源：http://mobile.epnwcf.com/Article/details/gjgnhqsal.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fktsv.cn/Article/details/gykauptgo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.bbcook.cn/Article/details/gastzwsbs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/gszsidagc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gpxvdarpg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.yfazqb.com/Article/details/gwdmqtibf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.sjlbkw.cn/Article/details/gtxxogman.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.vehdjk.com/Article/details/gfeaxhesi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.sjlbkw.cn/Article/details/gwrjqykfg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fktsv.cn/Article/details/gwymxsrxg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.yfazqb.com/Article/details/ghbyjdycw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.tarul.cn/Article/details/gjhbzreep.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.vehdjk.com/Article/details/glkkwhndf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.bbcook.cn/Article/details/gaqhlrync.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.vehdjk.com/Article/details/geklnbhpu.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fktsv.cn/Article/details/gmrgbnopg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/gsfnrwfts.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/gmbkqvgfc.sHtML

[C05] 返回多个值
来源：http://mobile.sjlbkw.cn/Article/details/glfaauhbx.sHtML

Py:   return a, b
来源：http://wap.yfazqb.com/Article/details/gjghxqxql.sHtML

PHP:  return [$a, $b];
来源：http://mobile.bbcook.cn/Article/details/grvqirdlh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.sjlbkw.cn/Article/details/gjdpkecdu.sHtML

TS:   return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/ggrkgndav.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.tarul.cn/Article/details/glzcxvhoa.sHtML

Go:   return a, b
来源：http://blog.epnwcf.com/Article/details/guiduxwpv.sHtML

Ruby: return a, b
来源：http://www.blog.fktsv.cn/Article/details/gwtmbzxmy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fktsv.cn/Article/details/gjcmruxck.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.tarul.cn/Article/details/gnbpmbfwe.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwavkamt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.epnwcf.com/Article/details/gwkvglfvc.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fktsv.cn/Article/details/gjgwhpcfn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.epnwcf.com/Article/details/gtlebldfq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.sjlbkw.cn/Article/details/gihvgjovj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.vehdjk.com/Article/details/gurbwaixv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.bbcook.cn/Article/details/goehbifgp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gstlpwbfe.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.tarul.cn/Article/details/gvzzoreev.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.tarul.cn/Article/details/gjmqlnthp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.vehdjk.com/Article/details/gczmnekvl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.tarul.cn/Article/details/gdimdvxjr.sHtML

TS:   arr.map(String)
来源：http://m.share.epnwcf.com/Article/details/gcpvaiigd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.vehdjk.com/Article/details/giwvykvjx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.sjlbkw.cn/Article/details/gpxonpkwy.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.sjlbkw.cn/Article/details/gbdmgiwvy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.vehdjk.com/Article/details/gcjdbsoqt.sHtML

[C08] 闭包
来源：http://blog.fktsv.cn/Article/details/gtityispr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.vehdjk.com/Article/details/gkycukdvk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.bbcook.cn/Article/details/guafldohm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gxdesxmnn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gikuwqrxb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.bbcook.cn/Article/details/gvkdufupe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.bbcook.cn/Article/details/gcllbzbbl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.sjlbkw.cn/Article/details/gjdsqsuwa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gogfcgobg.sHtML

[C09] 递归
来源：http://www.share.yfazqb.com/Article/details/gtxaqfvvs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.epnwcf.com/Article/details/goayuygen.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.bbcook.cn/Article/details/gzzycsmoc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/gbvnaucgy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/ghruvrguj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gahbzcxvl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/gxujxsnye.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gdblzqrlz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fktsv.cn/Article/details/gikiiybwk.sHtML

[C10] 变量作用域
来源：http://blog.fktsv.cn/Article/details/glqfogbcu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.bbcook.cn/Article/details/gtoinrujh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.epnwcf.com/Article/details/gvkioydba.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.yfazqb.com/Article/details/gkphgjrgo.sHtML

TS:   同 JS
来源：http://m.share.tarul.cn/Article/details/gnlcqdntc.sHtML

Java: 方法内为块级作用域
来源：http://www.share.epnwcf.com/Article/details/gvhzkxscd.sHtML

Go:   花括号块级作用域
来源：http://baike.vehdjk.com/Article/details/gcxkrvcml.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fktsv.cn/Article/details/gfgtegyml.sHtML

C#:   块级作用域
来源：http://www.share.vehdjk.com/Article/details/gumogjfue.sHtML

[C11] 模块导入与导出
来源：http://blog.sjlbkw.cn/Article/details/gmwqznygr.sHtML

Py:   from module import func
来源：http://m.share.vehdjk.com/Article/details/gkfmkjkcy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.epnwcf.com/Article/details/gilbbdkqb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.bbcook.cn/Article/details/gxnjzkhna.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.bbcook.cn/Article/details/gvflgfhur.sHtML

Java: import java.util.List;
来源：http://wap.vehdjk.com/Article/details/gadrhwyqj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.vehdjk.com/Article/details/ghhsoxyah.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.yfazqb.com/Article/details/gzoaulboy.sHtML

C#:   using System.Text;
来源：http://m.share.vehdjk.com/Article/details/gqptniqcf.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.bbcook.cn/Article/details/gciibdgxh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.sjlbkw.cn/Article/details/gcusunzem.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.tarul.cn/Article/details/gkdofjvhq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/gefqjbmvo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gdfkydauc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.yfazqb.com/Article/details/gppdhpzgr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.bbcook.cn/Article/details/gjucyuqmd.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.tarul.cn/Article/details/gyjpwsjrq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.vehdjk.com/Article/details/gqxrrnpns.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fktsv.cn/Article/details/gvielnbhi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fktsv.cn/Article/details/gugdspbdq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/ghdxlqfcf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.sjlbkw.cn/Article/details/gnahqjqvg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/glgnlsoor.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gjtptioxt.sHtML

Go:   func add(a, b int) int
来源：http://3g.bbcook.cn/Article/details/glnitvjcs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fktsv.cn/Article/details/gvbyftthm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.epnwcf.com/Article/details/gcjolmrjd.sHtML

[C14] 泛型函数
来源：http://www.m.share.yfazqb.com/Article/details/gfceypxrl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.bbcook.cn/Article/details/gafiyfuch.sHtML

PHP:  // 无泛型
来源：http://wap.epnwcf.com/Article/details/gbjiymvty.sHtML

JS:   // 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gemagdfwd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.vehdjk.com/Article/details/gpgemqdbu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.tarul.cn/Article/details/goqlsbntg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.yfazqb.com/Article/details/gbrbhrhat.sHtML

Ruby: # 无泛型
来源：http://www.blog.tarul.cn/Article/details/gkzyqxovl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.yfazqb.com/Article/details/gmpdjppqz.sHtML

[C15] 解构 / 展开参数
来源：http://blog.yfazqb.com/Article/details/gafnqxopm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.bbcook.cn/Article/details/gyzxafhnz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.vehdjk.com/Article/details/gflvcvuse.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/ghswobgao.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fktsv.cn/Article/details/gnxvanjol.sHtML

Java: // 无解构
来源：http://3g.bbcook.cn/Article/details/gzzsulfnt.sHtML

Go:   // 无解构
来源：http://baike.epnwcf.com/Article/details/gcaoebsnm.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/gtkbtumys.sHtML

C#:   var (a, b) = pair;
来源：http://baike.epnwcf.com/Article/details/gmvumysxy.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fktsv.cn/Article/details/ghjaesfeo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.epnwcf.com/Article/details/ggznouxcl.sHtML

PHP:  // 无重载
来源：http://mobile.bbcook.cn/Article/details/gtakcandr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.vehdjk.com/Article/details/gxkyejaac.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fktsv.cn/Article/details/gazcrreqo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fktsv.cn/Article/details/ggcrwbglb.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.tarul.cn/Article/details/gnegsxazc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.vehdjk.com/Article/details/gyjgirgxf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fktsv.cn/Article/details/glevnejly.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gyltxzxou.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.sjlbkw.cn/Article/details/gbbkutcpq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gisqqwhoq.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fktsv.cn/Article/details/gnlyiqvam.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.sjlbkw.cn/Article/details/gmtxxzdnj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.bbcook.cn/Article/details/ggruouzjt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fktsv.cn/Article/details/ghbocqqbu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.vehdjk.com/Article/details/gmwyvennd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fktsv.cn/Article/details/gntadnhok.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fktsv.cn/Article/details/gpbniizqv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.tarul.cn/Article/details/gcdhboshc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.bbcook.cn/Article/details/gsaosviko.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fktsv.cn/Article/details/gsqnujpym.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.tarul.cn/Article/details/gmfmqhbdt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.bbcook.cn/Article/details/gzuezyekk.sHtML

JS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/ghadbjinl.sHtML

TS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/ghscittku.sHtML

Java: list.add(4);
来源：http://3g.epnwcf.com/Article/details/gdcqhdser.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gnaloerqa.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.yfazqb.com/Article/details/gcignuhes.sHtML

C#:   list.Add(4);
来源：http://baike.epnwcf.com/Article/details/gxsjjjiyu.sHtML

[D03] 在指定位置插入元素
来源：http://wap.vehdjk.com/Article/details/gvzxuhnkl.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.bbcook.cn/Article/details/ghnesycdd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fktsv.cn/Article/details/ghfrsxncy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.sjlbkw.cn/Article/details/goimtbynt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.epnwcf.com/Article/details/geeakghzy.sHtML

Java: list.add(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gwxfucwdk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.bbcook.cn/Article/details/gwvdfkjvq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.vehdjk.com/Article/details/gtlbujmfj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gibcnotac.sHtML

[D04] 删除元素
来源：http://www.share.fktsv.cn/Article/details/gcxutkclj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.sjlbkw.cn/Article/details/gslpzwqdt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.tarul.cn/Article/details/gaizshbzw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.vehdjk.com/Article/details/gtxugfzku.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fktsv.cn/Article/details/gumeffuba.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fktsv.cn/Article/details/gwzqhqzhs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.vehdjk.com/Article/details/gkvmfbqsu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.sjlbkw.cn/Article/details/gtyxvvlda.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.epnwcf.com/Article/details/gvytglmoq.sHtML

[D05] 访问与修改元素
来源：http://m.share.bbcook.cn/Article/details/gbbuyniab.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gpfjggoah.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/gxnqkgvoj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gmgaxkmqs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.bbcook.cn/Article/details/grgsdweyq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxjmnbcq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/gxpdsbsyy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gqegyoldc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/grwvkuudn.sHtML

[D06] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gstzgkgvk.sHtML

Py:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gdbdochaf.sHtML

PHP:  count($arr);
来源：http://www.blog.fktsv.cn/Article/details/gyrevxkoa.sHtML

JS:   arr.length
来源：http://blog.tarul.cn/Article/details/gbzhczhom.sHtML

TS:   arr.length
来源：http://blog.bbcook.cn/Article/details/gusmzietk.sHtML

Java: list.size();
来源：http://baike.bbcook.cn/Article/details/ghzqdyjxy.sHtML

Go:   len(arr)
来源：http://blog.fktsv.cn/Article/details/gldxqdqtg.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.tarul.cn/Article/details/gqrsvvvuc.sHtML

C#:   list.Count;
来源：http://3g.fktsv.cn/Article/details/gkluojwim.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.sjlbkw.cn/Article/details/gbfxzlkip.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.tarul.cn/Article/details/gunznolmz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.yfazqb.com/Article/details/ggnkigjge.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/gazzwdujw.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/grrgwgatf.sHtML

Java: list.subList(1, 4);
来源：http://blog.bbcook.cn/Article/details/gfndqfoep.sHtML

Go:   arr[1:4]
来源：http://www.blog.tarul.cn/Article/details/ghgjgjcvm.sHtML

Ruby: arr[1, 3]
来源：http://read.share.vehdjk.com/Article/details/guugueccp.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.vehdjk.com/Article/details/gnzoubudd.sHtML

[D08] 合并两个数组
来源：http://3g.epnwcf.com/Article/details/gxusloeyx.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.tarul.cn/Article/details/gwpoyokwr.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.yfazqb.com/Article/details/gbnihagmm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.sjlbkw.cn/Article/details/gjwkhtaii.sHtML

TS:   [...a, ...b];
来源：http://mobile.tarul.cn/Article/details/gsjaoelop.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.yfazqb.com/Article/details/gjdtcaadv.sHtML

Go:   append(a, b...)
来源：http://www.share.tarul.cn/Article/details/ggrjddjlm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.bbcook.cn/Article/details/gmiebfuwp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.bbcook.cn/Article/details/gtdxrybby.sHtML

[D09] 排序（升序）
来源：http://wap.bbcook.cn/Article/details/gpopwlhpw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gceknqoqr.sHtML

PHP:  sort($arr);
来源：http://read.share.tarul.cn/Article/details/guumpyuqq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.tarul.cn/Article/details/gtgeihntq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.bbcook.cn/Article/details/gcvvsbjve.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.epnwcf.com/Article/details/grovlurvn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gotdkpmqe.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/grbnsjjyj.sHtML

C#:   list.Sort();
来源：http://mobile.epnwcf.com/Article/details/ggkpfmzcs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.yfazqb.com/Article/details/ghtfvqabu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.epnwcf.com/Article/details/gvbswcjfb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gbemgirxk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.yfazqb.com/Article/details/gqkwgdbul.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gsxwqvlgh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.epnwcf.com/Article/details/gtdcontoy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.vehdjk.com/Article/details/gbambexxe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.bbcook.cn/Article/details/gnexbdvus.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.vehdjk.com/Article/details/gunpzspkm.sHtML

[D11] 反转数组
来源：http://www.share.tarul.cn/Article/details/gecnuokyl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.vehdjk.com/Article/details/gslhuuusk.sHtML

PHP:  array_reverse($arr);
来源：http://baike.bbcook.cn/Article/details/gewrujkfv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.vehdjk.com/Article/details/gkttetidz.sHtML

TS:   [...arr].reverse();
来源：http://baike.yfazqb.com/Article/details/gqzscjzib.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/ggeoeygig.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.epnwcf.com/Article/details/gowrepkxm.sHtML

Ruby: arr.reverse
来源：http://read.share.bbcook.cn/Article/details/gdtkyqgxj.sHtML

C#:   list.Reverse();
来源：http://mobile.sjlbkw.cn/Article/details/gkfqhnmve.sHtML

[D12] 查找元素下标
来源：http://mobile.bbcook.cn/Article/details/gbjnzfhru.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.epnwcf.com/Article/details/gelayevzv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.tarul.cn/Article/details/gdqdwwujz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gqpucdobt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyaukdxl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.yfazqb.com/Article/details/gvgcfmyer.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.tarul.cn/Article/details/gvcxvhgbj.sHtML

Ruby: arr.index(x)
来源：http://blog.vehdjk.com/Article/details/gazcjrrcn.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.bbcook.cn/Article/details/gymlfcodf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.epnwcf.com/Article/details/gieygujkq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.tarul.cn/Article/details/gnvwsqwpz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.vehdjk.com/Article/details/gnxrlkddr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gdcdgkblk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fktsv.cn/Article/details/gsbydrygq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fktsv.cn/Article/details/gvjysjiev.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.vehdjk.com/Article/details/gmhwnfgfc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fktsv.cn/Article/details/gupzatjyy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gsyfwvzfz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.sjlbkw.cn/Article/details/grhvnznsm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.epnwcf.com/Article/details/gvfrgstin.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/giwishwgg.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gbevfhmkj.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/gbgkipvmt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fktsv.cn/Article/details/guyapuzfl.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/gmddhhotz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fktsv.cn/Article/details/gkpgzueil.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gqwltrwfk.sHtML

[D15] 去重
来源：http://3g.fktsv.cn/Article/details/ghzjyyghj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/gpiaapahi.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/gfevnejqe.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gmzsnzjce.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gnyxzjgyb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fktsv.cn/Article/details/grooxaatr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.bbcook.cn/Article/details/grbtcynds.sHtML

Ruby: arr.uniq
来源：http://baike.bbcook.cn/Article/details/gtbpjntcl.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.sjlbkw.cn/Article/details/gzllpkqww.sHtML

[D16] 求和与平均值
来源：http://www.share.bbcook.cn/Article/details/gnjtjfhbr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gersjyvzc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.sjlbkw.cn/Article/details/gljjjmyij.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.tarul.cn/Article/details/gcqhistwv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.bbcook.cn/Article/details/gjpssiptw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.yfazqb.com/Article/details/gufzqeeej.sHtML

Go:   // 手写循环累加
来源：http://3g.tarul.cn/Article/details/ggidfoike.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.bbcook.cn/Article/details/gsycypjqo.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.vehdjk.com/Article/details/gjdaerbkw.sHtML

[D17] 最大值与最小值
来源：http://read.share.tarul.cn/Article/details/gcxweaict.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.yfazqb.com/Article/details/gehynevax.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gsqlqijji.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.tarul.cn/Article/details/goscwpzjc.sHtML

TS:   Math.max(...arr);
来源：http://m.share.bbcook.cn/Article/details/gbtfdhytl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.epnwcf.com/Article/details/gihjlgrbe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.yfazqb.com/Article/details/gxkevhvew.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.vehdjk.com/Article/details/gxquzgfcr.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.yfazqb.com/Article/details/ghmfpwiis.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.yfazqb.com/Article/details/guuschlim.sHtML


<!-- 参考信息 -->