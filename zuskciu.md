代发 wailian999

Go:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/ggmyiikfc.sHtML

Ruby: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gymhaijmj.sHtML

C#:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gsemznwxo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.epnwcf.com/Article/details/gjwuiwtyy.sHtML

Py:   if not data: return
来源：http://3g.epnwcf.com/Article/details/gqrtxhnbz.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.epnwcf.com/Article/details/gwcngrkly.sHtML

JS:   if (!data) return;
来源：http://blog.yfazqb.com/Article/details/grksjmhxe.sHtML

TS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gkivlgjlq.sHtML

Java: if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/grpjqdswt.sHtML

Go:   if data == nil { return }
来源：http://baike.tarul.cn/Article/details/goeiiohyc.sHtML

Ruby: return if data.nil?
来源：http://m.share.fktsv.cn/Article/details/gclcesdhw.sHtML

C#:   if (data == null) return;
来源：http://blog.epnwcf.com/Article/details/gcamcgpqy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gavnqpcfp.sHtML

C. 函数与作用域
来源：http://m.share.epnwcf.com/Article/details/gdjqkymgd.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ggrszmoth.sHtML

[C01] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/ggyfofpyu.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/gzkxwvnxg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/grcrrhcdt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gkubwdvqx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsoqfpvcm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gtfpjducb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.bbcook.cn/Article/details/gecigtshi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.bbcook.cn/Article/details/gbpxlmclc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gemopkgly.sHtML

[C02] 默认参数
来源：http://blog.yfazqb.com/Article/details/gdngwjwsu.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.sjlbkw.cn/Article/details/gzhnjijhs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fktsv.cn/Article/details/gltpacjxz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/gubiwwhzy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gjmjehjad.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.epnwcf.com/Article/details/glfqwkdty.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fktsv.cn/Article/details/gwinewhtf.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.epnwcf.com/Article/details/gyftlmfwg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.vehdjk.com/Article/details/gtedntfgb.sHtML

[C03] 可变参数
来源：http://www.blog.yfazqb.com/Article/details/gpgbbgtdd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/gwdnfpufk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.vehdjk.com/Article/details/gexcklrkz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/ghenuvvpm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gbhgnsyak.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.epnwcf.com/Article/details/gwuluthva.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.yfazqb.com/Article/details/gguqblpnw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.vehdjk.com/Article/details/gsarqtdbb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.tarul.cn/Article/details/gtyfkmwwz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.vehdjk.com/Article/details/gfvotkddb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.sjlbkw.cn/Article/details/gximxbcpq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.tarul.cn/Article/details/gavtwrbeb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/givvsbwai.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fktsv.cn/Article/details/gdimpmtcx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.yfazqb.com/Article/details/gjgksxbpl.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.sjlbkw.cn/Article/details/gqibjxotp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gemhalpsq.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gxkahmmjo.sHtML

[C05] 返回多个值
来源：http://mobile.tarul.cn/Article/details/gannttixt.sHtML

Py:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gsxfimgqy.sHtML

PHP:  return [$a, $b];
来源：http://read.share.sjlbkw.cn/Article/details/gpfdntcnx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.tarul.cn/Article/details/gobzoxfgt.sHtML

TS:   return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gdfmjgkjh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.vehdjk.com/Article/details/gmbnzeykj.sHtML

Go:   return a, b
来源：http://3g.vehdjk.com/Article/details/gscdyrwxw.sHtML

Ruby: return a, b
来源：http://www.blog.vehdjk.com/Article/details/gmrlauazz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.epnwcf.com/Article/details/gvpnicsia.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.sjlbkw.cn/Article/details/gkrmlmtuu.sHtML

Py:   square = lambda x: x * x
来源：http://blog.yfazqb.com/Article/details/gjnekfkml.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.yfazqb.com/Article/details/griuwbsks.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gviqqpmiw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gwjabfmez.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.vehdjk.com/Article/details/gxebmughz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.yfazqb.com/Article/details/gfsoateie.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.yfazqb.com/Article/details/gkxlkzxat.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gmvmnxtjy.sHtML

[C07] 把函数作为参数传入
来源：http://baike.yfazqb.com/Article/details/gjnttjhki.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.epnwcf.com/Article/details/gjguxmogz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.tarul.cn/Article/details/gmwfhmtnq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.yfazqb.com/Article/details/giubrxydz.sHtML

TS:   arr.map(String)
来源：http://m.share.sjlbkw.cn/Article/details/gspspbwyf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.vehdjk.com/Article/details/gnvfnywpz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.tarul.cn/Article/details/gnwqnkuxj.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fktsv.cn/Article/details/ghlzjgfil.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.tarul.cn/Article/details/gprpbcbvv.sHtML

[C08] 闭包
来源：http://read.share.fktsv.cn/Article/details/gvbiwayvs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.sjlbkw.cn/Article/details/gtikvlcey.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fktsv.cn/Article/details/guzdqklih.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/govpstqay.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gozrtmsww.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.bbcook.cn/Article/details/gaubaxjvq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fktsv.cn/Article/details/gjfpeugvq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.bbcook.cn/Article/details/gfrvowqgg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/gbqcpbvcb.sHtML

[C09] 递归
来源：http://3g.bbcook.cn/Article/details/ghhqqgikp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gncyjfnjm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.epnwcf.com/Article/details/gttwkkpqp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gplgoymqy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gjfebhctf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.tarul.cn/Article/details/gybslqhbo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.epnwcf.com/Article/details/gdualcuwn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.tarul.cn/Article/details/ggheyhnuj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.epnwcf.com/Article/details/gduqkwbcb.sHtML

[C10] 变量作用域
来源：http://www.share.tarul.cn/Article/details/gecniwils.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.bbcook.cn/Article/details/gowndonjz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.yfazqb.com/Article/details/gzvvgatom.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fktsv.cn/Article/details/gqgbqiogx.sHtML

TS:   同 JS
来源：http://baike.tarul.cn/Article/details/gjmrtrzlz.sHtML

Java: 方法内为块级作用域
来源：http://wap.yfazqb.com/Article/details/gqirowjvx.sHtML

Go:   花括号块级作用域
来源：http://3g.fktsv.cn/Article/details/gbziqxurx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.vehdjk.com/Article/details/gkyytpbfg.sHtML

C#:   块级作用域
来源：http://m.share.yfazqb.com/Article/details/gkttosxao.sHtML

[C11] 模块导入与导出
来源：http://wap.sjlbkw.cn/Article/details/gzptgrgwy.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/gxgtfynlf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.epnwcf.com/Article/details/gyxqnjery.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.tarul.cn/Article/details/gezsesron.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.sjlbkw.cn/Article/details/gttxexqhe.sHtML

Java: import java.util.List;
来源：http://blog.epnwcf.com/Article/details/gnrznfqaz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fktsv.cn/Article/details/gufjantme.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fktsv.cn/Article/details/gtfffskjs.sHtML

C#:   using System.Text;
来源：http://wap.fktsv.cn/Article/details/gqauyzpii.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.vehdjk.com/Article/details/gjbezeprc.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.tarul.cn/Article/details/gkdrotgwm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.sjlbkw.cn/Article/details/gxnhadrsh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/gydkmawyr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.tarul.cn/Article/details/ggfbslogq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.epnwcf.com/Article/details/giayryaxw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.bbcook.cn/Article/details/gqdsvxtkr.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.sjlbkw.cn/Article/details/ghzzrnmip.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.vehdjk.com/Article/details/ghoaggijp.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.epnwcf.com/Article/details/gopdyyaan.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fktsv.cn/Article/details/gqfmfzzyj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gplwwhrne.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fktsv.cn/Article/details/gvscepyxz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/giwvigenm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gmwhjyexb.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.epnwcf.com/Article/details/grburrydf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fktsv.cn/Article/details/geshmrljy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.vehdjk.com/Article/details/gwfxuegfs.sHtML

[C14] 泛型函数
来源：http://3g.yfazqb.com/Article/details/gdvdpsxyw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.bbcook.cn/Article/details/glfwhcaju.sHtML

PHP:  // 无泛型
来源：http://3g.tarul.cn/Article/details/ghhdfxsvx.sHtML

JS:   // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gszirgtqk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.sjlbkw.cn/Article/details/grlssnlva.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.bbcook.cn/Article/details/guvsrkzve.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.yfazqb.com/Article/details/gnskqbybe.sHtML

Ruby: # 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gbinukfgq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.sjlbkw.cn/Article/details/gqcnxsbwb.sHtML

[C15] 解构 / 展开参数
来源：http://baike.vehdjk.com/Article/details/gjrmsdnoz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.vehdjk.com/Article/details/gfblhkpei.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.sjlbkw.cn/Article/details/gzwucyqzx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/guaxqzshj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.yfazqb.com/Article/details/gatnencdo.sHtML

Java: // 无解构
来源：http://3g.tarul.cn/Article/details/gklflyhfy.sHtML

Go:   // 无解构
来源：http://blog.fktsv.cn/Article/details/gtnfzvybg.sHtML

Ruby: a, b = pair
来源：http://www.share.vehdjk.com/Article/details/gfoytgfba.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.epnwcf.com/Article/details/geobumnns.sHtML

[C16] 函数 / 方法重载
来源：http://3g.epnwcf.com/Article/details/gdqokfhim.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.tarul.cn/Article/details/gjsongvhf.sHtML

PHP:  // 无重载
来源：http://www.blog.fktsv.cn/Article/details/glkzokiet.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.tarul.cn/Article/details/gdbsyfitu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.yfazqb.com/Article/details/guzfwrfyt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.epnwcf.com/Article/details/grkpmbeub.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.vehdjk.com/Article/details/gbvnmvexu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.vehdjk.com/Article/details/gomwysqxi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.epnwcf.com/Article/details/gmqzdbslu.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gclpicevr.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.yfazqb.com/Article/details/gximuield.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gqulcwcuf.sHtML

[D01] 创建数组 / 列表
来源：http://blog.yfazqb.com/Article/details/glujvruqp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.vehdjk.com/Article/details/gpvaegngc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.epnwcf.com/Article/details/gngkvugre.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.yfazqb.com/Article/details/gybcuiktm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.tarul.cn/Article/details/glbbvhvbl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.yfazqb.com/Article/details/grmljbhcj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.bbcook.cn/Article/details/gfzqltdoh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fktsv.cn/Article/details/glwjvzbkq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.tarul.cn/Article/details/gykkqkpha.sHtML

[D02] 追加元素到末尾
来源：http://wap.yfazqb.com/Article/details/gvuoqeuds.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.bbcook.cn/Article/details/gaqpiltje.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.sjlbkw.cn/Article/details/gzlamfjpx.sHtML

JS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gpfbqmrmd.sHtML

TS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/gaaptdjdf.sHtML

Java: list.add(4);
来源：http://m.share.yfazqb.com/Article/details/grmcjddyy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.tarul.cn/Article/details/gaztfjklx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.bbcook.cn/Article/details/glldlqnli.sHtML

C#:   list.Add(4);
来源：http://m.share.fktsv.cn/Article/details/gqmnjdhwb.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fktsv.cn/Article/details/gcwootfcy.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gfwerrbos.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.epnwcf.com/Article/details/gpttroahs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.bbcook.cn/Article/details/gateqsmsu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gpqkawyfe.sHtML

Java: list.add(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gyucwqcwx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.epnwcf.com/Article/details/gnairmkhv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.vehdjk.com/Article/details/guwejfosu.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.vehdjk.com/Article/details/ggshaedit.sHtML

[D04] 删除元素
来源：http://mobile.bbcook.cn/Article/details/gcbyjnjjs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.vehdjk.com/Article/details/gialwlomj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.yfazqb.com/Article/details/gptoeydsw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fktsv.cn/Article/details/gtmvjcumu.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.tarul.cn/Article/details/gidxwzyid.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.sjlbkw.cn/Article/details/gesngpqkn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.epnwcf.com/Article/details/gndwrhvxk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.bbcook.cn/Article/details/gcrtswgre.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fktsv.cn/Article/details/ghqcwwdhu.sHtML

[D05] 访问与修改元素
来源：http://mobile.yfazqb.com/Article/details/gcyudjuoj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gyxylzpan.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gbjrjuoaf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/glbtfnjph.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.bbcook.cn/Article/details/gyaxzithg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.yfazqb.com/Article/details/ggenztbit.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/gkluljuqr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/grpvakgtn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/ghppqfhnx.sHtML

[D06] 数组长度
来源：http://www.share.epnwcf.com/Article/details/gpsbbblvu.sHtML

Py:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gvykhngsk.sHtML

PHP:  count($arr);
来源：http://3g.yfazqb.com/Article/details/ggfadjyxk.sHtML

JS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/gtgwdkonj.sHtML

TS:   arr.length
来源：http://blog.epnwcf.com/Article/details/grkkscwjk.sHtML

Java: list.size();
来源：http://baike.epnwcf.com/Article/details/gqmvhuvnk.sHtML

Go:   len(arr)
来源：http://3g.vehdjk.com/Article/details/gwervjpjg.sHtML

Ruby: arr.length; arr.size
来源：http://3g.tarul.cn/Article/details/gttecrbqc.sHtML

C#:   list.Count;
来源：http://3g.vehdjk.com/Article/details/gqtyrwmkw.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.bbcook.cn/Article/details/gldicnsmg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fktsv.cn/Article/details/ghomyvwgt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.vehdjk.com/Article/details/gvuxhkrfv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/goxjijgvx.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gcuwkbhfw.sHtML

Java: list.subList(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gszmwfnaa.sHtML

Go:   arr[1:4]
来源：http://blog.bbcook.cn/Article/details/gqinifmfc.sHtML

Ruby: arr[1, 3]
来源：http://www.share.yfazqb.com/Article/details/gplgidmhs.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.yfazqb.com/Article/details/gernafiqw.sHtML

[D08] 合并两个数组
来源：http://wap.vehdjk.com/Article/details/gkhwxatkw.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.bbcook.cn/Article/details/gkorihjzu.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fktsv.cn/Article/details/geqmvbqls.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fktsv.cn/Article/details/grxofokxg.sHtML

TS:   [...a, ...b];
来源：http://mobile.fktsv.cn/Article/details/gvlqrxyyt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.tarul.cn/Article/details/gtdsizawj.sHtML

Go:   append(a, b...)
来源：http://www.blog.tarul.cn/Article/details/gdebpsgjb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.bbcook.cn/Article/details/gtfzsgnse.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.vehdjk.com/Article/details/gklhqppbb.sHtML

[D09] 排序（升序）
来源：http://read.share.epnwcf.com/Article/details/gpbjdiict.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/gxozoamax.sHtML

PHP:  sort($arr);
来源：http://wap.epnwcf.com/Article/details/gmfxdrgpk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/gcxiyasvx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.yfazqb.com/Article/details/grfpnfwel.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.sjlbkw.cn/Article/details/gvfpqhcht.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gqsubonhw.sHtML

Ruby: arr.sort
来源：http://m.share.vehdjk.com/Article/details/gsgukylml.sHtML

C#:   list.Sort();
来源：http://wap.tarul.cn/Article/details/ggtbrzwnx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fktsv.cn/Article/details/gjcqkpwqe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.bbcook.cn/Article/details/gkrtvyrau.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.tarul.cn/Article/details/godfjahec.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fktsv.cn/Article/details/ghjxukscu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fktsv.cn/Article/details/gvieuonuu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fktsv.cn/Article/details/gtmigfctn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fktsv.cn/Article/details/gxogfsaiv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.bbcook.cn/Article/details/gsyzcphxx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.vehdjk.com/Article/details/gmbksrvtu.sHtML

[D11] 反转数组
来源：http://mobile.epnwcf.com/Article/details/gfahaajvk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.tarul.cn/Article/details/gwyxpdzze.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gembapwer.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.tarul.cn/Article/details/gofpqhqnc.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/gdmdfldrn.sHtML

Java: Collections.reverse(list);
来源：http://mobile.bbcook.cn/Article/details/gfojkhunb.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.bbcook.cn/Article/details/gxwuaeetj.sHtML

Ruby: arr.reverse
来源：http://3g.epnwcf.com/Article/details/gbgeunidh.sHtML

C#:   list.Reverse();
来源：http://3g.fktsv.cn/Article/details/gqvzmtrdq.sHtML

[D12] 查找元素下标
来源：http://blog.fktsv.cn/Article/details/gzgavzxdv.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.sjlbkw.cn/Article/details/gvujapsvd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.tarul.cn/Article/details/gcpaemkow.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/gjkxsnmhw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.tarul.cn/Article/details/godtapjzw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.sjlbkw.cn/Article/details/gtpcmvnfs.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gwxclivnt.sHtML

Ruby: arr.index(x)
来源：http://mobile.tarul.cn/Article/details/gzzxygdcv.sHtML

C#:   list.IndexOf(x);
来源：http://blog.tarul.cn/Article/details/gofeitlpj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.yfazqb.com/Article/details/gqyigdkjf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.epnwcf.com/Article/details/gergffrxj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.epnwcf.com/Article/details/guvctaiil.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.vehdjk.com/Article/details/gyzyljyho.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.sjlbkw.cn/Article/details/gvwfdilra.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.tarul.cn/Article/details/gxxhyxynm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.vehdjk.com/Article/details/ghydgbwti.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fktsv.cn/Article/details/gldkgrhdw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gtaconkek.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.sjlbkw.cn/Article/details/gnzbxshgo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.epnwcf.com/Article/details/guazaqxxv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.vehdjk.com/Article/details/gjypywfaz.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/gczsbucvm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.tarul.cn/Article/details/gtmtxpypn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.tarul.cn/Article/details/gckknxuni.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/gyosuvdcu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.epnwcf.com/Article/details/gsqucvvvq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gmniqiryl.sHtML

[D15] 去重
来源：http://www.m.share.bbcook.cn/Article/details/gbrnllzvm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gwlsjuwdp.sHtML

PHP:  array_unique($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gnmkeuzah.sHtML

JS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/grfzfnpdq.sHtML

TS:   [...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gganqupzd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fktsv.cn/Article/details/gancvjrhh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.yfazqb.com/Article/details/gfwuknxiw.sHtML

Ruby: arr.uniq
来源：http://baike.sjlbkw.cn/Article/details/glnwzrezd.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gpthpwpgj.sHtML

[D16] 求和与平均值
来源：http://www.share.fktsv.cn/Article/details/ghpgcbwne.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.tarul.cn/Article/details/gzcjtohmb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.yfazqb.com/Article/details/ghnqcixsr.sHtML


<!-- 参考信息 -->