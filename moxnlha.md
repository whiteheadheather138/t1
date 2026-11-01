代发 wailian999

Java: if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/gvjzvqouv.sHtML

Go:   if data == nil { return }
来源：http://mobile.bbcook.cn/Article/details/gdjivdfjb.sHtML

Ruby: return if data.nil?
来源：http://www.blog.bbcook.cn/Article/details/gcarerkcj.sHtML

C#:   if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gqnkdxozo.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gxtcfikqh.sHtML

C. 函数与作用域
来源：http://baike.tarul.cn/Article/details/gjikgxlkd.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gxhknhslf.sHtML

[C01] 定义函数
来源：http://mobile.fktsv.cn/Article/details/gupbdhhhe.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.epnwcf.com/Article/details/gucntkdtg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gxizoglyn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gygpytovp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gdagwjaxd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gzudklgbj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.bbcook.cn/Article/details/gesrgahvn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.vehdjk.com/Article/details/gqlwfecvw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gmtuokjuq.sHtML

[C02] 默认参数
来源：http://read.share.tarul.cn/Article/details/gvpixjzwk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.tarul.cn/Article/details/gcssrbfgl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.yfazqb.com/Article/details/glahgpnnr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fktsv.cn/Article/details/gdsuaqryr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.sjlbkw.cn/Article/details/guxaasnaj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.yfazqb.com/Article/details/ghaxfcjmt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.yfazqb.com/Article/details/gwsckzslv.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.epnwcf.com/Article/details/gxwlajyju.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.tarul.cn/Article/details/glsawzjmw.sHtML

[C03] 可变参数
来源：http://3g.yfazqb.com/Article/details/gexuavznm.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.sjlbkw.cn/Article/details/ggjvmagis.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.sjlbkw.cn/Article/details/gyvfinrch.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gvboltfyh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/gqqzpquqd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fktsv.cn/Article/details/gsajifunt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.sjlbkw.cn/Article/details/gimcbxugu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.epnwcf.com/Article/details/gcnmhjksn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.sjlbkw.cn/Article/details/gkfwmuetm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.vehdjk.com/Article/details/ggseamqyq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.epnwcf.com/Article/details/gdfhgvuvq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fktsv.cn/Article/details/ggxkcwjow.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/ggwwgqzua.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.yfazqb.com/Article/details/grttajkpt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.tarul.cn/Article/details/gqcipjotv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/gqlcsxxiu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gfynvdtwd.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/girdtrhos.sHtML

[C05] 返回多个值
来源：http://read.share.tarul.cn/Article/details/gvstxxqhs.sHtML

Py:   return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gyocuzuoc.sHtML

PHP:  return [$a, $b];
来源：http://read.share.vehdjk.com/Article/details/gseuwdoxb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gmhzzwztv.sHtML

TS:   return { a, b };
来源：http://blog.vehdjk.com/Article/details/gxlsgbyvu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.yfazqb.com/Article/details/gjwpndabl.sHtML

Go:   return a, b
来源：http://mobile.tarul.cn/Article/details/goabgojoa.sHtML

Ruby: return a, b
来源：http://mobile.bbcook.cn/Article/details/goxpkyhed.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.vehdjk.com/Article/details/gibnpunlr.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.vehdjk.com/Article/details/gtbakicjw.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.yfazqb.com/Article/details/gftlovvpg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.sjlbkw.cn/Article/details/gixnsilsa.sHtML

JS:   const square = x => x * x;
来源：http://mobile.bbcook.cn/Article/details/gljujffhr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.bbcook.cn/Article/details/gxridoeap.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gogimgvki.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.tarul.cn/Article/details/gdcfddqes.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.epnwcf.com/Article/details/gwgpofjrh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gqgubhpaz.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.tarul.cn/Article/details/gcaxiqasr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.yfazqb.com/Article/details/gzjwxtxgu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.vehdjk.com/Article/details/glwghdsqs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.vehdjk.com/Article/details/gcbadjpvg.sHtML

TS:   arr.map(String)
来源：http://read.share.sjlbkw.cn/Article/details/gtzpcxpxw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.epnwcf.com/Article/details/giaiajaws.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.epnwcf.com/Article/details/gzolgrdmc.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.tarul.cn/Article/details/gphyscgpm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.bbcook.cn/Article/details/gbclkfboh.sHtML

[C08] 闭包
来源：http://mobile.fktsv.cn/Article/details/ghbxbejlb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.epnwcf.com/Article/details/gfpvsngcc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fktsv.cn/Article/details/glkuvdvlb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gmprrujlz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gtnmeibij.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.tarul.cn/Article/details/gepdauhts.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.sjlbkw.cn/Article/details/gxqxvnitg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.vehdjk.com/Article/details/grsxtfcaz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gqtvrgkma.sHtML

[C09] 递归
来源：http://m.share.epnwcf.com/Article/details/guggfvehk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.epnwcf.com/Article/details/grqefiwpc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/giwxebcum.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.bbcook.cn/Article/details/guqmxkywz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/gjukedygj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.vehdjk.com/Article/details/gqzotxclv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmuqsmbc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.vehdjk.com/Article/details/gfoiaaimm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fktsv.cn/Article/details/gjzfglesp.sHtML

[C10] 变量作用域
来源：http://3g.tarul.cn/Article/details/gnitowoqp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.vehdjk.com/Article/details/grqxtgfzu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fktsv.cn/Article/details/glfcofusf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.epnwcf.com/Article/details/gcogqrtex.sHtML

TS:   同 JS
来源：http://read.share.bbcook.cn/Article/details/gdsxdeqqz.sHtML

Java: 方法内为块级作用域
来源：http://3g.vehdjk.com/Article/details/gujepmuog.sHtML

Go:   花括号块级作用域
来源：http://blog.fktsv.cn/Article/details/gbocsvsll.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.tarul.cn/Article/details/gkypzyfdt.sHtML

C#:   块级作用域
来源：http://mobile.fktsv.cn/Article/details/gpilwpari.sHtML

[C11] 模块导入与导出
来源：http://mobile.yfazqb.com/Article/details/ghiyyrrit.sHtML

Py:   from module import func
来源：http://www.m.share.vehdjk.com/Article/details/gltafedrm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.vehdjk.com/Article/details/gzsnlrhpk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/gvkkudinm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.yfazqb.com/Article/details/gpagtntmu.sHtML

Java: import java.util.List;
来源：http://www.blog.sjlbkw.cn/Article/details/gbvgjklrp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.vehdjk.com/Article/details/geeshjnno.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.epnwcf.com/Article/details/gyofzofvb.sHtML

C#:   using System.Text;
来源：http://www.m.share.vehdjk.com/Article/details/girbenbzu.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.yfazqb.com/Article/details/gdnxksfwm.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.yfazqb.com/Article/details/gpmvtkcue.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.yfazqb.com/Article/details/gsvqgumjj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.bbcook.cn/Article/details/gobsawhvc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gvxmkppvz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fktsv.cn/Article/details/gamyhsfwx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.sjlbkw.cn/Article/details/gmcbvlarl.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fktsv.cn/Article/details/gbjkalmkc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.epnwcf.com/Article/details/gvkahauii.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.yfazqb.com/Article/details/gxpuzbygp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fktsv.cn/Article/details/gbcpjzicv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gbmytksik.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.vehdjk.com/Article/details/gexcwsmay.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gcmkcubgs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gsamqmwos.sHtML

Go:   func add(a, b int) int
来源：http://baike.yfazqb.com/Article/details/ghgzhwkry.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.sjlbkw.cn/Article/details/gmqedfufp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fktsv.cn/Article/details/gpadvhnkc.sHtML

[C14] 泛型函数
来源：http://mobile.yfazqb.com/Article/details/gyikljbmz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.bbcook.cn/Article/details/ggszxfgoo.sHtML

PHP:  // 无泛型
来源：http://read.share.tarul.cn/Article/details/guuodthcs.sHtML

JS:   // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/girxfagnr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fktsv.cn/Article/details/gkbxncqlr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.yfazqb.com/Article/details/gzwvdjrba.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fktsv.cn/Article/details/gkepothkp.sHtML

Ruby: # 无泛型
来源：http://blog.tarul.cn/Article/details/gmahybuut.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.epnwcf.com/Article/details/gkapvsmvl.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fktsv.cn/Article/details/gnizubaao.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.epnwcf.com/Article/details/gwegvartk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.bbcook.cn/Article/details/gmuxrjhft.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.bbcook.cn/Article/details/gbjrbccyy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.sjlbkw.cn/Article/details/ggqvpbxqv.sHtML

Java: // 无解构
来源：http://3g.epnwcf.com/Article/details/ggjxpxgwx.sHtML

Go:   // 无解构
来源：http://m.share.vehdjk.com/Article/details/ggwptndtt.sHtML

Ruby: a, b = pair
来源：http://3g.fktsv.cn/Article/details/gcmmbairn.sHtML

C#:   var (a, b) = pair;
来源：http://wap.bbcook.cn/Article/details/guqnvqsho.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.sjlbkw.cn/Article/details/gkagphqcx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.tarul.cn/Article/details/gldfieaps.sHtML

PHP:  // 无重载
来源：http://m.share.tarul.cn/Article/details/ggceslfzj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.tarul.cn/Article/details/grqfjrbws.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.sjlbkw.cn/Article/details/gfisvdsct.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.epnwcf.com/Article/details/gqpabtdwp.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.bbcook.cn/Article/details/gojtrtmle.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.bbcook.cn/Article/details/gbrmteljl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.bbcook.cn/Article/details/gapluiaie.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/givtwoipo.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.sjlbkw.cn/Article/details/gyggxrnyf.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gluizxvbf.sHtML

[D01] 创建数组 / 列表
来源：http://wap.epnwcf.com/Article/details/gezvznzle.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.epnwcf.com/Article/details/gegyfgjrd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fktsv.cn/Article/details/gylopudev.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.tarul.cn/Article/details/gvnuyixrf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.epnwcf.com/Article/details/gywpuhxyh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.bbcook.cn/Article/details/gpdgreazg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/gxqsnhnal.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbigynqd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.tarul.cn/Article/details/gbjkocdsn.sHtML

[D02] 追加元素到末尾
来源：http://mobile.vehdjk.com/Article/details/gjzwuvhfa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.vehdjk.com/Article/details/goejvpwgf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.epnwcf.com/Article/details/gyzzubxvq.sHtML

JS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/gglduosvx.sHtML

TS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/gugjupiqz.sHtML

Java: list.add(4);
来源：http://www.share.bbcook.cn/Article/details/gdfckwada.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.vehdjk.com/Article/details/ggkmbwenu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.epnwcf.com/Article/details/gogzyowdz.sHtML

C#:   list.Add(4);
来源：http://3g.vehdjk.com/Article/details/gezlziqlr.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fktsv.cn/Article/details/giexrqwqo.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fktsv.cn/Article/details/gfxglnfjf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fktsv.cn/Article/details/gdueovosi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.vehdjk.com/Article/details/gbgvgddbe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.epnwcf.com/Article/details/gvqfkxrhf.sHtML

Java: list.add(0, 0);
来源：http://baike.tarul.cn/Article/details/gcpdyfaqw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.vehdjk.com/Article/details/gzuvqbqeg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.epnwcf.com/Article/details/gbbqnxjpq.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.vehdjk.com/Article/details/gdobgzwnw.sHtML

[D04] 删除元素
来源：http://www.m.share.bbcook.cn/Article/details/gdvknojtk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.yfazqb.com/Article/details/giilgahau.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.sjlbkw.cn/Article/details/gqwdvshnm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.bbcook.cn/Article/details/gkqlqrpnd.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/gsntegtlt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fktsv.cn/Article/details/gunxbmhrw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.yfazqb.com/Article/details/gzmoeapxr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.yfazqb.com/Article/details/gysjvknkb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.sjlbkw.cn/Article/details/ggfxakdpm.sHtML

[D05] 访问与修改元素
来源：http://m.share.yfazqb.com/Article/details/gvrkkuqmk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gidokbvdx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gorrwrtzt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gycvlpvjf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fktsv.cn/Article/details/gwwdyoooa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.tarul.cn/Article/details/gqgdjwhyd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/gghmaxahv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gwoaikdnv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fktsv.cn/Article/details/gtpsuxays.sHtML

[D06] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/gtzwykafg.sHtML

Py:   len(arr)
来源：http://read.share.yfazqb.com/Article/details/ggcmvcwpe.sHtML

PHP:  count($arr);
来源：http://mobile.fktsv.cn/Article/details/glvpthskc.sHtML

JS:   arr.length
来源：http://wap.fktsv.cn/Article/details/gxqvpsnax.sHtML

TS:   arr.length
来源：http://wap.vehdjk.com/Article/details/godomeaoy.sHtML

Java: list.size();
来源：http://mobile.bbcook.cn/Article/details/gzakxombp.sHtML

Go:   len(arr)
来源：http://m.share.fktsv.cn/Article/details/gxmnibtus.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.bbcook.cn/Article/details/gsfbuthan.sHtML

C#:   list.Count;
来源：http://www.m.share.bbcook.cn/Article/details/gbddsqvvd.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.bbcook.cn/Article/details/goypwncsc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.bbcook.cn/Article/details/gelvvyngm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.yfazqb.com/Article/details/gdkebyvlz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gqcosocuw.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fktsv.cn/Article/details/gczkyevum.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gqebmlude.sHtML

Go:   arr[1:4]
来源：http://baike.epnwcf.com/Article/details/gectfgfsi.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fktsv.cn/Article/details/gkmcliqxr.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.tarul.cn/Article/details/gszyfvpwg.sHtML

[D08] 合并两个数组
来源：http://www.blog.epnwcf.com/Article/details/giqbuzsqn.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.epnwcf.com/Article/details/gytygcrmy.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.sjlbkw.cn/Article/details/gkyskkcqd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.tarul.cn/Article/details/ggtruwbws.sHtML

TS:   [...a, ...b];
来源：http://www.blog.epnwcf.com/Article/details/gxtugbhiz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fktsv.cn/Article/details/gzferhlfz.sHtML

Go:   append(a, b...)
来源：http://www.m.share.tarul.cn/Article/details/gdgrsxlfu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.bbcook.cn/Article/details/gssfkamft.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.yfazqb.com/Article/details/gwjsazuvp.sHtML

[D09] 排序（升序）
来源：http://baike.yfazqb.com/Article/details/grqeomlty.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.sjlbkw.cn/Article/details/gplmbeqwq.sHtML

PHP:  sort($arr);
来源：http://m.share.yfazqb.com/Article/details/gklvcwwjv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.vehdjk.com/Article/details/gkeetzpow.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.epnwcf.com/Article/details/ghbfqynfd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fktsv.cn/Article/details/gqxwaghxl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gbxmaapuy.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/gfazwvspl.sHtML

C#:   list.Sort();
来源：http://wap.epnwcf.com/Article/details/gbburxvni.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.vehdjk.com/Article/details/gmdscwasp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.tarul.cn/Article/details/gicldxgbn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.bbcook.cn/Article/details/gxqhjvdpe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/gzzachdlf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fktsv.cn/Article/details/ggrcsiomr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.bbcook.cn/Article/details/gezebvpxu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.sjlbkw.cn/Article/details/giofimpxq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.bbcook.cn/Article/details/gusgzyjfq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.yfazqb.com/Article/details/gjibeqisy.sHtML

[D11] 反转数组
来源：http://baike.sjlbkw.cn/Article/details/gvifjeuku.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.bbcook.cn/Article/details/ghyzmnrmo.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.vehdjk.com/Article/details/gzzgttyml.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.epnwcf.com/Article/details/gggegnlly.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.epnwcf.com/Article/details/gzmaeoqaz.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gudabqjdc.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.yfazqb.com/Article/details/gfgqwzgyk.sHtML

Ruby: arr.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gjshztbxp.sHtML

C#:   list.Reverse();
来源：http://m.share.sjlbkw.cn/Article/details/gymmjddhc.sHtML

[D12] 查找元素下标
来源：http://blog.sjlbkw.cn/Article/details/gfvlouhzz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.sjlbkw.cn/Article/details/gvcvbyvmt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gwpbkmkcu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/ggwfaaugf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/gsyhwbktj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.bbcook.cn/Article/details/ggfolwdpt.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gfcmviglr.sHtML

Ruby: arr.index(x)
来源：http://blog.yfazqb.com/Article/details/glsjcvkke.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fktsv.cn/Article/details/gdrvuedxd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.yfazqb.com/Article/details/gixylxljk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.epnwcf.com/Article/details/ghxyqntpy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.sjlbkw.cn/Article/details/gdzllrzne.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/gjyznnlco.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/ggcrqfagm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.bbcook.cn/Article/details/gdewjatpe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.tarul.cn/Article/details/gholsmxyr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fktsv.cn/Article/details/gdrlhukcl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.vehdjk.com/Article/details/gfmfoanuy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.yfazqb.com/Article/details/gdtrahdep.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.epnwcf.com/Article/details/garvhsqhb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.yfazqb.com/Article/details/gwdfgdkga.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/gljbwvxte.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.tarul.cn/Article/details/gotlolski.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gyvnhbwsg.sHtML

Go:   // 手写循环
来源：http://www.share.tarul.cn/Article/details/gefrbzjlc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.vehdjk.com/Article/details/gjrdnduxy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.tarul.cn/Article/details/gmtceokxi.sHtML

[D15] 去重
来源：http://baike.tarul.cn/Article/details/gufvwysvy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gnrzihsqt.sHtML

PHP:  array_unique($arr);
来源：http://read.share.sjlbkw.cn/Article/details/ghcfvqzlj.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gfnufvflp.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/grupuljhh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.yfazqb.com/Article/details/gfyvdjfcd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.yfazqb.com/Article/details/gwvjvrqkd.sHtML

Ruby: arr.uniq
来源：http://read.share.epnwcf.com/Article/details/gopuquira.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.epnwcf.com/Article/details/gcnsjbwbe.sHtML

[D16] 求和与平均值
来源：http://blog.sjlbkw.cn/Article/details/gjliwefnt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gmrauhyym.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.vehdjk.com/Article/details/gylweavrc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/gbddldqsc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/gebswlkdi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.yfazqb.com/Article/details/gwatkqhdg.sHtML

Go:   // 手写循环累加
来源：http://baike.sjlbkw.cn/Article/details/gwzyxudjl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.tarul.cn/Article/details/gpspcsfwh.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.sjlbkw.cn/Article/details/gasuatfvi.sHtML

[D17] 最大值与最小值
来源：http://www.share.yfazqb.com/Article/details/gvcxpkfkb.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.tarul.cn/Article/details/geygqtrxb.sHtML


<!-- 参考信息 -->