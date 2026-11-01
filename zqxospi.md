代发 wailian999

Py:   if not data: return
来源：http://mobile.epnwcf.com/Article/details/gkatksmuq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.yfazqb.com/Article/details/geotjbqhz.sHtML

JS:   if (!data) return;
来源：http://wap.epnwcf.com/Article/details/gslboyfmo.sHtML

TS:   if (!data) return;
来源：http://wap.bbcook.cn/Article/details/gujelqlpx.sHtML

Java: if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/gkuwvjabr.sHtML

Go:   if data == nil { return }
来源：http://read.share.fktsv.cn/Article/details/gpvzanvgm.sHtML

Ruby: return if data.nil?
来源：http://baike.sjlbkw.cn/Article/details/gymzqilwj.sHtML

C#:   if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/gbtvrmupj.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gzuwitqcp.sHtML

C. 函数与作用域
来源：http://read.share.epnwcf.com/Article/details/gcxyghjtf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/glcwsibfp.sHtML

[C01] 定义函数
来源：http://baike.vehdjk.com/Article/details/gnwnsmpru.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fktsv.cn/Article/details/gnbpwkaym.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gbyfewncr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gtconrgmi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gcdpcvbjk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gkiblrsff.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.bbcook.cn/Article/details/gwqwbrqjb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.epnwcf.com/Article/details/gilixtldq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gulzarxcw.sHtML

[C02] 默认参数
来源：http://m.share.epnwcf.com/Article/details/gnrtvexey.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.tarul.cn/Article/details/gwsfqlfub.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.epnwcf.com/Article/details/giufyobli.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gnuplvtjv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/gqjrwqbey.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.epnwcf.com/Article/details/gqtlqtmwx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.tarul.cn/Article/details/gnuobgjig.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fktsv.cn/Article/details/gseteznzw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.bbcook.cn/Article/details/gisfjfyks.sHtML

[C03] 可变参数
来源：http://www.m.share.vehdjk.com/Article/details/gmbdmsozf.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.sjlbkw.cn/Article/details/gygzllvzv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.vehdjk.com/Article/details/gtqzlcvlx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/gidldscpy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/gshgbyutd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.epnwcf.com/Article/details/gastppagi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.epnwcf.com/Article/details/gmasiitdj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.epnwcf.com/Article/details/gilcelyod.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.vehdjk.com/Article/details/gbgleromq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqxujmnx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fktsv.cn/Article/details/ghmxxzbul.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.bbcook.cn/Article/details/gwnrsphlo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gddlzgjxl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.yfazqb.com/Article/details/gcvzgdizw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.tarul.cn/Article/details/gtahzomlj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.yfazqb.com/Article/details/ggcrccjxn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gkscrmnbe.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/gfwmsvwdr.sHtML

[C05] 返回多个值
来源：http://wap.vehdjk.com/Article/details/gupmwkarj.sHtML

Py:   return a, b
来源：http://baike.epnwcf.com/Article/details/gggzaemmo.sHtML

PHP:  return [$a, $b];
来源：http://read.share.yfazqb.com/Article/details/gudxtdjvx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gnqynlcfr.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gwnkrhfuz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.epnwcf.com/Article/details/gtelomwng.sHtML

Go:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gtncrnuyq.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gycdyckzg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.sjlbkw.cn/Article/details/gkeaxcclz.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.sjlbkw.cn/Article/details/ghlfejlgx.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fktsv.cn/Article/details/gjdvwbkeb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.bbcook.cn/Article/details/guchpcfsg.sHtML

JS:   const square = x => x * x;
来源：http://wap.fktsv.cn/Article/details/geknbffem.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.vehdjk.com/Article/details/gyrjclimt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.epnwcf.com/Article/details/gmhhgphum.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.bbcook.cn/Article/details/gmvavuece.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.epnwcf.com/Article/details/gbqjwmfnm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.bbcook.cn/Article/details/gfguyvgnh.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.epnwcf.com/Article/details/grwyiscjq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.yfazqb.com/Article/details/gcirwlnhl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.yfazqb.com/Article/details/gksmcvxmp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fktsv.cn/Article/details/gqvfqigav.sHtML

TS:   arr.map(String)
来源：http://www.share.bbcook.cn/Article/details/gfzzpajah.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.tarul.cn/Article/details/ggrrvagno.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.yfazqb.com/Article/details/gnpdlsbjn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.epnwcf.com/Article/details/gehfcfzxl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsgoxiwx.sHtML

[C08] 闭包
来源：http://3g.tarul.cn/Article/details/glfmlepib.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.yfazqb.com/Article/details/grmddnbyg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.epnwcf.com/Article/details/gcsdidlbm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gwsurlkwc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gxckuqlzl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.tarul.cn/Article/details/guolyttog.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.yfazqb.com/Article/details/gcbirjsfu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.vehdjk.com/Article/details/gfcmbdwvq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gotxnsxmb.sHtML

[C09] 递归
来源：http://www.blog.yfazqb.com/Article/details/gkffmkotc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gtlvrufip.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fktsv.cn/Article/details/gzbzunhkx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/gbfwsykdw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.epnwcf.com/Article/details/gcjwikeyx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.tarul.cn/Article/details/gjatzkdur.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.tarul.cn/Article/details/gdpnojsks.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gpaavqfse.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.epnwcf.com/Article/details/grbjfxgzw.sHtML

[C10] 变量作用域
来源：http://www.m.share.yfazqb.com/Article/details/gstotksao.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.vehdjk.com/Article/details/gnplytwcc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.bbcook.cn/Article/details/ggfudxgnn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.tarul.cn/Article/details/grbqpbkya.sHtML

TS:   同 JS
来源：http://m.share.bbcook.cn/Article/details/gmarhlfhv.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gjstkggek.sHtML

Go:   花括号块级作用域
来源：http://m.share.vehdjk.com/Article/details/gcgmxanfo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.epnwcf.com/Article/details/gjnilsqkx.sHtML

C#:   块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gxkisovwo.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.yfazqb.com/Article/details/gshyvgrhc.sHtML

Py:   from module import func
来源：http://m.share.bbcook.cn/Article/details/gblqkckhg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fktsv.cn/Article/details/gakgkavlh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.epnwcf.com/Article/details/grwzekqhb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.tarul.cn/Article/details/gsiriqwff.sHtML

Java: import java.util.List;
来源：http://read.share.epnwcf.com/Article/details/guqxsexap.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fktsv.cn/Article/details/goikhiluw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.vehdjk.com/Article/details/grynmpggn.sHtML

C#:   using System.Text;
来源：http://m.share.bbcook.cn/Article/details/gnrcrhdco.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.yfazqb.com/Article/details/gxyinzwnl.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.epnwcf.com/Article/details/ghofqujme.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.vehdjk.com/Article/details/grccvkzwo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gtszncxuz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/giagjfnuz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fktsv.cn/Article/details/gvaixjjcy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.sjlbkw.cn/Article/details/gnvckzqec.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.vehdjk.com/Article/details/gwfgwpimc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.bbcook.cn/Article/details/gehujowln.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.epnwcf.com/Article/details/gvfxrygst.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.bbcook.cn/Article/details/gjbimfbht.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gzuklwxcg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.sjlbkw.cn/Article/details/grxlegnwp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/ghmmbihll.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/giphkyirz.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fktsv.cn/Article/details/geocccgxh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.bbcook.cn/Article/details/gzcapbnvp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.vehdjk.com/Article/details/gurrlqtoq.sHtML

[C14] 泛型函数
来源：http://blog.bbcook.cn/Article/details/grocyqgxr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fktsv.cn/Article/details/ghlhzmgvv.sHtML

PHP:  // 无泛型
来源：http://www.blog.tarul.cn/Article/details/gqfielwco.sHtML

JS:   // 无泛型
来源：http://wap.yfazqb.com/Article/details/gplcysoti.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fktsv.cn/Article/details/gfcegubet.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fktsv.cn/Article/details/gqhuuecpi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.sjlbkw.cn/Article/details/gbwmxvkjo.sHtML

Ruby: # 无泛型
来源：http://blog.vehdjk.com/Article/details/gxcsojldo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.bbcook.cn/Article/details/gehdnnytg.sHtML

[C15] 解构 / 展开参数
来源：http://blog.vehdjk.com/Article/details/gcyqbraez.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.tarul.cn/Article/details/gkkcdasbh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.bbcook.cn/Article/details/gfatkmdbn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gmzctdbxt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fktsv.cn/Article/details/gmxbxlfke.sHtML

Java: // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/ghivmnxwo.sHtML

Go:   // 无解构
来源：http://www.m.share.bbcook.cn/Article/details/gcqajmhql.sHtML

Ruby: a, b = pair
来源：http://baike.fktsv.cn/Article/details/gaqyxdlud.sHtML

C#:   var (a, b) = pair;
来源：http://wap.epnwcf.com/Article/details/gscjhiyet.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.epnwcf.com/Article/details/gjkibkdzc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.epnwcf.com/Article/details/goffhqdnp.sHtML

PHP:  // 无重载
来源：http://blog.bbcook.cn/Article/details/gthqrwnyp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.sjlbkw.cn/Article/details/gutccyahq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.tarul.cn/Article/details/geugvzaqe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.vehdjk.com/Article/details/gqiifqmxm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.epnwcf.com/Article/details/gxrciyigc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.vehdjk.com/Article/details/gkaesnbmx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.tarul.cn/Article/details/gexgypnkg.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gydhrzkut.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fktsv.cn/Article/details/gbfhhogoc.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gywanmhuy.sHtML

[D01] 创建数组 / 列表
来源：http://wap.epnwcf.com/Article/details/gadoadwlb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.tarul.cn/Article/details/gnwbmbdik.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.bbcook.cn/Article/details/gmhyajcyw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.yfazqb.com/Article/details/gudibweri.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.epnwcf.com/Article/details/gmspujutj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.sjlbkw.cn/Article/details/ghvxnodap.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.bbcook.cn/Article/details/glvrkjiys.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.sjlbkw.cn/Article/details/gzmuunkze.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.bbcook.cn/Article/details/gzpbqtzmn.sHtML

[D02] 追加元素到末尾
来源：http://m.share.vehdjk.com/Article/details/gaulrdjpj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fktsv.cn/Article/details/gsxoxcife.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.bbcook.cn/Article/details/gknegfgbp.sHtML

JS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gukazuxfx.sHtML

TS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/gkadiqtmj.sHtML

Java: list.add(4);
来源：http://blog.fktsv.cn/Article/details/gopvnsply.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.yfazqb.com/Article/details/gzwxkznrv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.tarul.cn/Article/details/gbcbbhrqw.sHtML

C#:   list.Add(4);
来源：http://www.share.vehdjk.com/Article/details/gopiwdtnu.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fktsv.cn/Article/details/gbpbfylxa.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fktsv.cn/Article/details/gpbnppnfw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.sjlbkw.cn/Article/details/gnpmbpuql.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.epnwcf.com/Article/details/geoodqvev.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.tarul.cn/Article/details/gsstlplgy.sHtML

Java: list.add(0, 0);
来源：http://3g.tarul.cn/Article/details/gabhfacmt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gyzdaqwiu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.tarul.cn/Article/details/gbzfejggo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gjratjvgv.sHtML

[D04] 删除元素
来源：http://www.share.fktsv.cn/Article/details/gommrlrah.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.tarul.cn/Article/details/gwedjxhgw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fktsv.cn/Article/details/gggrbzojt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.yfazqb.com/Article/details/gomarccil.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.vehdjk.com/Article/details/gxqduknuz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fktsv.cn/Article/details/gbyhpqihl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fktsv.cn/Article/details/griezbyix.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fktsv.cn/Article/details/gxqhmneww.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fktsv.cn/Article/details/glpwbkytv.sHtML

[D05] 访问与修改元素
来源：http://read.share.vehdjk.com/Article/details/ghebngyac.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gzmtrepbo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gigvvzlnz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gmlimkduy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.bbcook.cn/Article/details/gigsrvxdh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/ghxgshhnn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/glomacaht.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gxvaqqdve.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.yfazqb.com/Article/details/gjiejbmeh.sHtML

[D06] 数组长度
来源：http://baike.epnwcf.com/Article/details/gzwawuuiz.sHtML

Py:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gzbeavfhd.sHtML

PHP:  count($arr);
来源：http://wap.sjlbkw.cn/Article/details/ghtgeaycv.sHtML

JS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/gcnlcjess.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gvlldtaps.sHtML

Java: list.size();
来源：http://mobile.vehdjk.com/Article/details/gqbvsiool.sHtML

Go:   len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gtygfnffk.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gxyqkglri.sHtML

C#:   list.Count;
来源：http://www.m.share.yfazqb.com/Article/details/ggonhjipq.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.vehdjk.com/Article/details/gremmbmbu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fktsv.cn/Article/details/gjrfrqkny.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.tarul.cn/Article/details/guihnahqj.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gudjtkpgh.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/graqxdzer.sHtML

Java: list.subList(1, 4);
来源：http://3g.bbcook.cn/Article/details/grilvqrau.sHtML

Go:   arr[1:4]
来源：http://www.share.bbcook.cn/Article/details/gyprhalkc.sHtML

Ruby: arr[1, 3]
来源：http://read.share.tarul.cn/Article/details/ggwaaxobi.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.epnwcf.com/Article/details/gcapdtfmj.sHtML

[D08] 合并两个数组
来源：http://www.share.bbcook.cn/Article/details/ghztxtqzl.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.epnwcf.com/Article/details/gkkjgmovk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.yfazqb.com/Article/details/ggpxszvgj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.vehdjk.com/Article/details/gspfmjezt.sHtML

TS:   [...a, ...b];
来源：http://read.share.tarul.cn/Article/details/gtejilvyk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fktsv.cn/Article/details/gjukmgfob.sHtML

Go:   append(a, b...)
来源：http://mobile.fktsv.cn/Article/details/gahnkvqie.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fktsv.cn/Article/details/gmpqwuuud.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.bbcook.cn/Article/details/gjyyczjso.sHtML

[D09] 排序（升序）
来源：http://mobile.epnwcf.com/Article/details/gximulvhm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/gathaxytn.sHtML

PHP:  sort($arr);
来源：http://m.share.fktsv.cn/Article/details/gtzqfkiof.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fktsv.cn/Article/details/gzmrpisvw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.yfazqb.com/Article/details/gzubikgul.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.tarul.cn/Article/details/gofqgjxny.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.epnwcf.com/Article/details/gurlivlsj.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/geqkluuft.sHtML

C#:   list.Sort();
来源：http://www.blog.fktsv.cn/Article/details/gdtlkhiet.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.bbcook.cn/Article/details/gmqcmvnal.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.yfazqb.com/Article/details/gefbjauyy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/gjmmdybix.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.bbcook.cn/Article/details/gdoyvlueo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/gfiiolawk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.bbcook.cn/Article/details/gvcbhjzmk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.bbcook.cn/Article/details/gfretntvl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.epnwcf.com/Article/details/gvqeueeir.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.bbcook.cn/Article/details/ggswoapap.sHtML

[D11] 反转数组
来源：http://baike.epnwcf.com/Article/details/godxborhj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/gotelywof.sHtML

PHP:  array_reverse($arr);
来源：http://wap.epnwcf.com/Article/details/gfptoqlhp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.yfazqb.com/Article/details/gypiyabya.sHtML

TS:   [...arr].reverse();
来源：http://blog.vehdjk.com/Article/details/gzqhoodap.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.bbcook.cn/Article/details/ggdwoyuti.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fktsv.cn/Article/details/gyheucuic.sHtML

Ruby: arr.reverse
来源：http://wap.epnwcf.com/Article/details/gdbpgyeqj.sHtML

C#:   list.Reverse();
来源：http://www.m.share.tarul.cn/Article/details/gyzbwmflw.sHtML

[D12] 查找元素下标
来源：http://mobile.yfazqb.com/Article/details/gcvvheahj.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.epnwcf.com/Article/details/ghamtvhtu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gjmpjqeaz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.tarul.cn/Article/details/gzvqhsatp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gcpdhcxce.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.sjlbkw.cn/Article/details/givkzynqo.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gikigqthw.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.epnwcf.com/Article/details/guoksiizd.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.bbcook.cn/Article/details/gesjaockz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.yfazqb.com/Article/details/gpknvjfiq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.bbcook.cn/Article/details/gsxjapxbd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.tarul.cn/Article/details/gwuuamhha.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/gqlzulmhw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gahbasetn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gamzibeni.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.vehdjk.com/Article/details/giaidclbq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.bbcook.cn/Article/details/gizbxytqm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.yfazqb.com/Article/details/ggzupblqe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.epnwcf.com/Article/details/gktiuhifv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.bbcook.cn/Article/details/gpegpkfso.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fktsv.cn/Article/details/ggdqkemws.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.tarul.cn/Article/details/gufbtpgol.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gwujoqpav.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.sjlbkw.cn/Article/details/gioxkptaz.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/gbnquqnal.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fktsv.cn/Article/details/ghjhixepa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.yfazqb.com/Article/details/gpsyfelfk.sHtML

[D15] 去重
来源：http://3g.yfazqb.com/Article/details/gbtbppsxz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/gshrwvcve.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fktsv.cn/Article/details/gpcmrehrv.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/gmoqclpct.sHtML

TS:   [...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/gsfjrlwvs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.epnwcf.com/Article/details/gfbdxnvga.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fktsv.cn/Article/details/ggnlijard.sHtML

Ruby: arr.uniq
来源：http://blog.bbcook.cn/Article/details/gcgmyettz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.vehdjk.com/Article/details/gtojksarj.sHtML

[D16] 求和与平均值
来源：http://blog.tarul.cn/Article/details/gfsxsaotb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gonqqglgc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.bbcook.cn/Article/details/gsfjyzpyo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/glvphskas.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.tarul.cn/Article/details/gqxhcxwsp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.epnwcf.com/Article/details/gslfajoeb.sHtML

Go:   // 手写循环累加
来源：http://wap.vehdjk.com/Article/details/gmunenrul.sHtML


<!-- 参考信息 -->