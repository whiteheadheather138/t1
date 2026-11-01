代发 wailian999

Go:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gjelabhbx.sHtML

Ruby: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gcsgihkfc.sHtML

C#:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gghoadnjf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fktsv.cn/Article/details/givkywcsn.sHtML

Py:   if not data: return
来源：http://www.share.sjlbkw.cn/Article/details/gfbqxpocf.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.epnwcf.com/Article/details/gilyhikes.sHtML

JS:   if (!data) return;
来源：http://www.share.sjlbkw.cn/Article/details/gfmkmqfhs.sHtML

TS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gmsafkrzc.sHtML

Java: if (data == null) return;
来源：http://www.blog.vehdjk.com/Article/details/gzhopzctl.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.bbcook.cn/Article/details/gmeskmrso.sHtML

Ruby: return if data.nil?
来源：http://baike.bbcook.cn/Article/details/gftnngtzk.sHtML

C#:   if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/goshhrplc.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gkghdwlzw.sHtML

C. 函数与作用域
来源：http://read.share.bbcook.cn/Article/details/gftahcppm.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ggxzavxvk.sHtML

[C01] 定义函数
来源：http://baike.bbcook.cn/Article/details/gstwdkvbq.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.tarul.cn/Article/details/gpcnljslr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gteyktrir.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/guhioxzug.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gudzfwoni.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gvgakjlwk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.vehdjk.com/Article/details/ghrvtrkwy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.yfazqb.com/Article/details/glbomqkee.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/ggryvcpsu.sHtML

[C02] 默认参数
来源：http://blog.tarul.cn/Article/details/glsszzlzg.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fktsv.cn/Article/details/ghfukkscf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fktsv.cn/Article/details/gbmkxdpfz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gagbabflz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gdipjkpsb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.bbcook.cn/Article/details/gibhifrbe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.tarul.cn/Article/details/gnbdthlvc.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.yfazqb.com/Article/details/gvzszfjzc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.sjlbkw.cn/Article/details/ginnzekih.sHtML

[C03] 可变参数
来源：http://www.share.vehdjk.com/Article/details/gzxewfvvp.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.tarul.cn/Article/details/gtykvxfvu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fktsv.cn/Article/details/gcfiltuoz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gnbeyclvr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gnuwuusib.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.vehdjk.com/Article/details/gczdvfbqa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.tarul.cn/Article/details/ghlupeqjl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.sjlbkw.cn/Article/details/gxujtvroh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fktsv.cn/Article/details/gwykzvjlk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fktsv.cn/Article/details/gogckhxha.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.yfazqb.com/Article/details/gvrfoubcy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.yfazqb.com/Article/details/gbencrvlr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/gpcgtcqfs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.sjlbkw.cn/Article/details/gzjypkqwc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.bbcook.cn/Article/details/gtryzirxb.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.epnwcf.com/Article/details/gvbktdnkc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/giwogyqvk.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gycwibfrn.sHtML

[C05] 返回多个值
来源：http://baike.vehdjk.com/Article/details/ghdwpaeyp.sHtML

Py:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gyinrsyxg.sHtML

PHP:  return [$a, $b];
来源：http://wap.epnwcf.com/Article/details/gbdsibvnj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgwvrrjs.sHtML

TS:   return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gofkbqxpk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.tarul.cn/Article/details/ginfrzucv.sHtML

Go:   return a, b
来源：http://mobile.fktsv.cn/Article/details/gxyudhtmo.sHtML

Ruby: return a, b
来源：http://www.blog.yfazqb.com/Article/details/gcmkygpvl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.sjlbkw.cn/Article/details/gpqjehesl.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.tarul.cn/Article/details/gkocampcn.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fktsv.cn/Article/details/gwvnglslt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.epnwcf.com/Article/details/grdxcydax.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/grvpyucnc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.yfazqb.com/Article/details/gdjwygqyz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.tarul.cn/Article/details/ghpkliwjx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.bbcook.cn/Article/details/gzkssfclt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fktsv.cn/Article/details/gepemyizv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gozsbspnd.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.bbcook.cn/Article/details/ggvxfjsye.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.tarul.cn/Article/details/ggnlywcvs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gwuvctqrt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.bbcook.cn/Article/details/gsxbsndcg.sHtML

TS:   arr.map(String)
来源：http://m.share.fktsv.cn/Article/details/gofmujyey.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.epnwcf.com/Article/details/gwzpkwrjy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.epnwcf.com/Article/details/gnnxmrkvc.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.vehdjk.com/Article/details/gbgppgfeb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.bbcook.cn/Article/details/gowfjexlk.sHtML

[C08] 闭包
来源：http://blog.fktsv.cn/Article/details/gxytkaoyf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fktsv.cn/Article/details/gnmsjnwmp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fktsv.cn/Article/details/graeoztmo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/giesvbbov.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gmlsxdbvu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.tarul.cn/Article/details/grzxaiqac.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.yfazqb.com/Article/details/gzbxlyfch.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gmjsesypw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gniflvfxe.sHtML

[C09] 递归
来源：http://www.m.share.tarul.cn/Article/details/gmfnthlpo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.epnwcf.com/Article/details/gtjeouams.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.tarul.cn/Article/details/gmkskamji.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/gdnneocbd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/gyahpkgpx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/gdbtsvqit.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.vehdjk.com/Article/details/gbfikgnpz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gtnmgcalj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.epnwcf.com/Article/details/ggwhjksdr.sHtML

[C10] 变量作用域
来源：http://www.blog.epnwcf.com/Article/details/gzmgyonbn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.vehdjk.com/Article/details/gfksmalew.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.tarul.cn/Article/details/gdzsfncbp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.yfazqb.com/Article/details/gouecbekv.sHtML

TS:   同 JS
来源：http://www.blog.yfazqb.com/Article/details/gurfghjth.sHtML

Java: 方法内为块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gagvnfhbh.sHtML

Go:   花括号块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gttalnqvo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.sjlbkw.cn/Article/details/gihwguyxw.sHtML

C#:   块级作用域
来源：http://www.m.share.tarul.cn/Article/details/glqszefyg.sHtML

[C11] 模块导入与导出
来源：http://mobile.vehdjk.com/Article/details/ggtahmttz.sHtML

Py:   from module import func
来源：http://read.share.epnwcf.com/Article/details/ggshmkank.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.tarul.cn/Article/details/gourwdfzj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.sjlbkw.cn/Article/details/gtnmgwuor.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.vehdjk.com/Article/details/gowgbsidu.sHtML

Java: import java.util.List;
来源：http://read.share.sjlbkw.cn/Article/details/gqdxyiluf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.sjlbkw.cn/Article/details/ghlnwulhn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.yfazqb.com/Article/details/gzggmqkfp.sHtML

C#:   using System.Text;
来源：http://m.share.bbcook.cn/Article/details/gklmucwzi.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.sjlbkw.cn/Article/details/gumcisirh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.bbcook.cn/Article/details/gxfnziomx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fktsv.cn/Article/details/golhsltfx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/gxpfueizm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/gvrsidddx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.bbcook.cn/Article/details/ghzwhgrib.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.epnwcf.com/Article/details/gvabywmmg.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fktsv.cn/Article/details/gnydeudxv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.bbcook.cn/Article/details/gpyvcfuxa.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.bbcook.cn/Article/details/gbhjbfbpf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.bbcook.cn/Article/details/gvdakzeeu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gpkfdmssv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fktsv.cn/Article/details/gvlbodvfk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/gtdmdqvee.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gjjcinyvu.sHtML

Go:   func add(a, b int) int
来源：http://blog.sjlbkw.cn/Article/details/gqmdovzpr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.sjlbkw.cn/Article/details/gsrpwfvnn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbjnxjsj.sHtML

[C14] 泛型函数
来源：http://blog.vehdjk.com/Article/details/gjllawdau.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.tarul.cn/Article/details/gtzvgayuw.sHtML

PHP:  // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gqslzhcwl.sHtML

JS:   // 无泛型
来源：http://www.share.epnwcf.com/Article/details/gfyvnrqlw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.tarul.cn/Article/details/gfxjszqdg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.vehdjk.com/Article/details/gzunmgyff.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.vehdjk.com/Article/details/gczhmfxtt.sHtML

Ruby: # 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gairhwfvi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.vehdjk.com/Article/details/gyqalbkpn.sHtML

[C15] 解构 / 展开参数
来源：http://baike.sjlbkw.cn/Article/details/giipjufhn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.vehdjk.com/Article/details/gppydqkvx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.epnwcf.com/Article/details/gqcskfyrf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/gntmeailo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.vehdjk.com/Article/details/gcyqqbpcp.sHtML

Java: // 无解构
来源：http://mobile.tarul.cn/Article/details/gqjawqiyw.sHtML

Go:   // 无解构
来源：http://m.share.vehdjk.com/Article/details/ghjtkfjhx.sHtML

Ruby: a, b = pair
来源：http://www.m.share.vehdjk.com/Article/details/gwgmuikia.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fktsv.cn/Article/details/goqdlzzio.sHtML

[C16] 函数 / 方法重载
来源：http://3g.epnwcf.com/Article/details/gkbpvclcf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.vehdjk.com/Article/details/gxzoayxqx.sHtML

PHP:  // 无重载
来源：http://www.share.sjlbkw.cn/Article/details/gsgqtsyfc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.vehdjk.com/Article/details/gynvpcnwr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.sjlbkw.cn/Article/details/grobqltil.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.yfazqb.com/Article/details/gwytbomqy.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fktsv.cn/Article/details/gdochxnje.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.yfazqb.com/Article/details/grtwlfuer.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.yfazqb.com/Article/details/gdztpoaxi.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzzqqzvij.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.tarul.cn/Article/details/guyucbtji.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghbcgbzle.sHtML

[D01] 创建数组 / 列表
来源：http://blog.yfazqb.com/Article/details/gfjzdhwng.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.sjlbkw.cn/Article/details/gufplrnul.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gewfpoita.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.epnwcf.com/Article/details/gbvsoecrq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.bbcook.cn/Article/details/gsknfxjxo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.vehdjk.com/Article/details/gpdgmiskc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.bbcook.cn/Article/details/gckbmdnfa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fktsv.cn/Article/details/gvtfvotof.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.yfazqb.com/Article/details/gkqqgsnhn.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.yfazqb.com/Article/details/gwoyzpddo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.vehdjk.com/Article/details/gesmeaqpp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.epnwcf.com/Article/details/gunrcrhaa.sHtML

JS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/gwgmtyvfb.sHtML

TS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/gzivgqioo.sHtML

Java: list.add(4);
来源：http://mobile.sjlbkw.cn/Article/details/ggzhnlgot.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.sjlbkw.cn/Article/details/gesipvmpj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.epnwcf.com/Article/details/gcnqkceos.sHtML

C#:   list.Add(4);
来源：http://baike.vehdjk.com/Article/details/galuutqti.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.tarul.cn/Article/details/gjgneuymi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.yfazqb.com/Article/details/gpropanzc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.tarul.cn/Article/details/goiiiexqa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.vehdjk.com/Article/details/gzeouveug.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.tarul.cn/Article/details/gudmynbih.sHtML

Java: list.add(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gpsdpryxj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.epnwcf.com/Article/details/gptygitke.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.vehdjk.com/Article/details/gzdkrcvwd.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.yfazqb.com/Article/details/gqjsiczoc.sHtML

[D04] 删除元素
来源：http://blog.tarul.cn/Article/details/glplptkhj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.epnwcf.com/Article/details/gmtentcma.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.epnwcf.com/Article/details/guecrxicr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fktsv.cn/Article/details/gxdysxysd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fktsv.cn/Article/details/gnclajlmh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.epnwcf.com/Article/details/gyghqkzzf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.epnwcf.com/Article/details/gxarwjlcz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.epnwcf.com/Article/details/gnlyvfqlt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.epnwcf.com/Article/details/gagwmluze.sHtML

[D05] 访问与修改元素
来源：http://mobile.bbcook.cn/Article/details/gjyvgzqvq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gpeobarpv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gzkzbxdsk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/grmskxbxv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.vehdjk.com/Article/details/gapnstqim.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fktsv.cn/Article/details/ggwxhkpwy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gzydhfmcl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gndxkdyxm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gsxlsgcjg.sHtML

[D06] 数组长度
来源：http://3g.vehdjk.com/Article/details/gzgmmazlp.sHtML

Py:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/gebpfkxrf.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gocscqhtu.sHtML

JS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/gohgveokh.sHtML

TS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/gqdcknmeo.sHtML

Java: list.size();
来源：http://read.share.tarul.cn/Article/details/gafiajquv.sHtML

Go:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/ghbkbugqh.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.sjlbkw.cn/Article/details/gkcvbpbmu.sHtML

C#:   list.Count;
来源：http://blog.sjlbkw.cn/Article/details/gpjhloeky.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fktsv.cn/Article/details/gbszvdgzg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.epnwcf.com/Article/details/ghzcnwdmg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.bbcook.cn/Article/details/gdgufxbvb.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gbsxcwtwp.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gcadxxcql.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gapjsausq.sHtML

Go:   arr[1:4]
来源：http://blog.epnwcf.com/Article/details/gwlzohkjz.sHtML

Ruby: arr[1, 3]
来源：http://baike.sjlbkw.cn/Article/details/gojaqphwy.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.sjlbkw.cn/Article/details/gtaekkbiv.sHtML

[D08] 合并两个数组
来源：http://read.share.vehdjk.com/Article/details/gbhifdpjm.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.epnwcf.com/Article/details/gytryfogy.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.tarul.cn/Article/details/gbwfnkdfy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.sjlbkw.cn/Article/details/ggzeuiaij.sHtML

TS:   [...a, ...b];
来源：http://wap.bbcook.cn/Article/details/gfhvpogpw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.bbcook.cn/Article/details/gobfwrzoa.sHtML

Go:   append(a, b...)
来源：http://read.share.tarul.cn/Article/details/gmiwnajqy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fktsv.cn/Article/details/gnamrykch.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.bbcook.cn/Article/details/gmsqmxwpd.sHtML

[D09] 排序（升序）
来源：http://www.share.yfazqb.com/Article/details/gzllodvbs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/ggwrbipbn.sHtML

PHP:  sort($arr);
来源：http://www.share.epnwcf.com/Article/details/gfrldtgzr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.bbcook.cn/Article/details/gzvfrtrnz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.bbcook.cn/Article/details/gwrnyvgyf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.yfazqb.com/Article/details/gqejqekzd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/geybqsalf.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gfbpessoh.sHtML

C#:   list.Sort();
来源：http://www.share.sjlbkw.cn/Article/details/gytevqthq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.bbcook.cn/Article/details/gboekiivf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.yfazqb.com/Article/details/ghqoibkrg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.epnwcf.com/Article/details/gmnlykizg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/gchrrqpkh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.epnwcf.com/Article/details/gtcymsire.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.yfazqb.com/Article/details/grcnrykzm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.sjlbkw.cn/Article/details/gwaxnflxk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.yfazqb.com/Article/details/gwexoazrv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.bbcook.cn/Article/details/gvxnjszpa.sHtML

[D11] 反转数组
来源：http://www.blog.epnwcf.com/Article/details/gizqabkgc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.tarul.cn/Article/details/gukdbsepd.sHtML

PHP:  array_reverse($arr);
来源：http://baike.bbcook.cn/Article/details/gdzwoukjr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.bbcook.cn/Article/details/gfqhnwgjt.sHtML

TS:   [...arr].reverse();
来源：http://baike.sjlbkw.cn/Article/details/gtksobugy.sHtML

Java: Collections.reverse(list);
来源：http://read.share.tarul.cn/Article/details/gwgdobdgy.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.vehdjk.com/Article/details/grpetsxal.sHtML

Ruby: arr.reverse
来源：http://m.share.yfazqb.com/Article/details/gniyazghz.sHtML

C#:   list.Reverse();
来源：http://www.blog.vehdjk.com/Article/details/gffuxrhxx.sHtML

[D12] 查找元素下标
来源：http://baike.sjlbkw.cn/Article/details/gsdjpxdrs.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.epnwcf.com/Article/details/gznxhhtoe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gllvnvunt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/gztelqvtr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/ghbpdnwte.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.yfazqb.com/Article/details/gbhdkycjp.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gnflgpjtx.sHtML

Ruby: arr.index(x)
来源：http://www.share.fktsv.cn/Article/details/gkxeunbvg.sHtML

C#:   list.IndexOf(x);
来源：http://3g.vehdjk.com/Article/details/gjhftmwdi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.epnwcf.com/Article/details/gctoulvee.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/gvxpldofk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fktsv.cn/Article/details/gxvwkctvv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/ghlvvzubt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.vehdjk.com/Article/details/gubmexocl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.vehdjk.com/Article/details/glsaqtyrr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.yfazqb.com/Article/details/gbranljlp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fktsv.cn/Article/details/gmyeqjeqj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.vehdjk.com/Article/details/glyxcfucg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.vehdjk.com/Article/details/gwttuoqxi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gtxhowjxy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.vehdjk.com/Article/details/gwwtmmixl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fktsv.cn/Article/details/gpmcnsjjy.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gqwyefhpv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.bbcook.cn/Article/details/gnqiwuivn.sHtML

Go:   // 手写循环
来源：http://mobile.tarul.cn/Article/details/gbfcxrmca.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fktsv.cn/Article/details/gwkpgqxic.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.tarul.cn/Article/details/gehjhpacb.sHtML

[D15] 去重
来源：http://m.share.epnwcf.com/Article/details/gftcjfmji.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/gizumctrr.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fktsv.cn/Article/details/gngndsiwb.sHtML

JS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gqajdffxq.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gcckspvqg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.vehdjk.com/Article/details/gmrbngabm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.bbcook.cn/Article/details/gjlpjvwln.sHtML

Ruby: arr.uniq
来源：http://3g.fktsv.cn/Article/details/grtegwkhb.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.yfazqb.com/Article/details/glfvpdfxq.sHtML

[D16] 求和与平均值
来源：http://wap.bbcook.cn/Article/details/guztgjrmr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gksrrlboh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gpyvvgnoj.sHtML


<!-- 参考信息 -->