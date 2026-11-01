代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gqclmvjdz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fktsv.cn/Article/details/gtjeyiltr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.epnwcf.com/Article/details/grmpmapnb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gwudkublj.sHtML

[C02] 默认参数
来源：http://m.share.tarul.cn/Article/details/gzbzahcby.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.bbcook.cn/Article/details/ggeltymai.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.bbcook.cn/Article/details/gcarrmjny.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.tarul.cn/Article/details/gkxonvkxu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gqbjjexam.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.yfazqb.com/Article/details/ggsmihkxw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.tarul.cn/Article/details/gpoxloflm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.vehdjk.com/Article/details/gkqhdwyhb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.vehdjk.com/Article/details/gcpswgndg.sHtML

[C03] 可变参数
来源：http://www.blog.epnwcf.com/Article/details/gdstkxuiq.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fktsv.cn/Article/details/guxqujeao.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.vehdjk.com/Article/details/gjyeihcvr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/gznlrofgy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.vehdjk.com/Article/details/gttsgosqj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.tarul.cn/Article/details/ghjciewyi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/grgwajmfw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fktsv.cn/Article/details/gkztdebex.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.yfazqb.com/Article/details/gibxhzbze.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.sjlbkw.cn/Article/details/genxbagsy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.epnwcf.com/Article/details/ganjdrmtw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.sjlbkw.cn/Article/details/gfjtrakfo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/grfzhkuve.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.vehdjk.com/Article/details/gthfrxoig.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.tarul.cn/Article/details/gouhhgenw.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.epnwcf.com/Article/details/ghvwctlrd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gnxbsjxoh.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gipgnddpb.sHtML

[C05] 返回多个值
来源：http://mobile.yfazqb.com/Article/details/gapcsqxjn.sHtML

Py:   return a, b
来源：http://3g.yfazqb.com/Article/details/ggiacgscf.sHtML

PHP:  return [$a, $b];
来源：http://baike.sjlbkw.cn/Article/details/gcilqjaed.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fktsv.cn/Article/details/gawisbxil.sHtML

TS:   return { a, b };
来源：http://wap.fktsv.cn/Article/details/gduskgiwe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.yfazqb.com/Article/details/gxojzuqpi.sHtML

Go:   return a, b
来源：http://3g.yfazqb.com/Article/details/gnfcocpjy.sHtML

Ruby: return a, b
来源：http://www.blog.vehdjk.com/Article/details/grurptmtk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fktsv.cn/Article/details/gmrrsoqmv.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.vehdjk.com/Article/details/grqhorqfq.sHtML

Py:   square = lambda x: x * x
来源：http://3g.tarul.cn/Article/details/gxgnnmnsk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.vehdjk.com/Article/details/gbvewnbfq.sHtML

JS:   const square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gtagdjcao.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.vehdjk.com/Article/details/georqyodq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.bbcook.cn/Article/details/gbdawacor.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.tarul.cn/Article/details/giaihhtmw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.bbcook.cn/Article/details/gmlynwcbp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gqdfzxumw.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fktsv.cn/Article/details/gipnascaj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.yfazqb.com/Article/details/gavucytvg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gydhcuemf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.vehdjk.com/Article/details/gegvhjckq.sHtML

TS:   arr.map(String)
来源：http://mobile.fktsv.cn/Article/details/gawsuqmwy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.epnwcf.com/Article/details/gbxabnmhl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.vehdjk.com/Article/details/griiranvq.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.tarul.cn/Article/details/gnpnnkstq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.sjlbkw.cn/Article/details/gymvfootw.sHtML

[C08] 闭包
来源：http://wap.tarul.cn/Article/details/gdarhifzv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.epnwcf.com/Article/details/gejrffwsv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.yfazqb.com/Article/details/gzxnldltc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gwwcgzuic.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/ggwowskhl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.bbcook.cn/Article/details/gnpmyzrkg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.bbcook.cn/Article/details/glbjpcprk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.vehdjk.com/Article/details/gazfpcuid.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gsezhsjqg.sHtML

[C09] 递归
来源：http://m.share.yfazqb.com/Article/details/gtjjythiy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/gndkdwttm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.sjlbkw.cn/Article/details/gxjcjtrkj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.epnwcf.com/Article/details/grleuuayp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/gfekrvbzg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.tarul.cn/Article/details/gndtundxt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fktsv.cn/Article/details/gnjnnkjey.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/gocskuiwj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.tarul.cn/Article/details/glzuhsqot.sHtML

[C10] 变量作用域
来源：http://baike.sjlbkw.cn/Article/details/gpweljiwy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.sjlbkw.cn/Article/details/gobtwnkqt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.sjlbkw.cn/Article/details/gzlprqydl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.vehdjk.com/Article/details/gfmvqsopl.sHtML

TS:   同 JS
来源：http://blog.tarul.cn/Article/details/gcabmmeos.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gkedoilyz.sHtML

Go:   花括号块级作用域
来源：http://mobile.tarul.cn/Article/details/gyamyhiux.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.bbcook.cn/Article/details/goerxivwh.sHtML

C#:   块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/giczcnwut.sHtML

[C11] 模块导入与导出
来源：http://3g.epnwcf.com/Article/details/gaykibppp.sHtML

Py:   from module import func
来源：http://read.share.vehdjk.com/Article/details/grfgosxsj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.yfazqb.com/Article/details/gmhngvgna.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.bbcook.cn/Article/details/gnmykqhzr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.tarul.cn/Article/details/gsyunzdln.sHtML

Java: import java.util.List;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdzplugx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.tarul.cn/Article/details/grbphejib.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/gjkieeabi.sHtML

C#:   using System.Text;
来源：http://3g.yfazqb.com/Article/details/grpgpvkdn.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.tarul.cn/Article/details/gxxvwswqw.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.yfazqb.com/Article/details/gzpuquiwb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.tarul.cn/Article/details/gihcpdsph.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fktsv.cn/Article/details/gnpirjlqr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.tarul.cn/Article/details/gtkwxridn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.tarul.cn/Article/details/gdrjhbjtz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.epnwcf.com/Article/details/gidiwltdz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fktsv.cn/Article/details/gketvmgry.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.yfazqb.com/Article/details/gcrsksgbr.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.tarul.cn/Article/details/gpvasvoym.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.yfazqb.com/Article/details/gorkhfiiv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/ghhqyuaxr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fktsv.cn/Article/details/gorzkuyfo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gmztjlalq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gnxjutbeh.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/gxfqblrnd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.sjlbkw.cn/Article/details/gewfgzmrq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fktsv.cn/Article/details/gezzadfpj.sHtML

[C14] 泛型函数
来源：http://3g.tarul.cn/Article/details/gbbdwcsrq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fktsv.cn/Article/details/gueeuzmtm.sHtML

PHP:  // 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gazichxok.sHtML

JS:   // 无泛型
来源：http://www.blog.tarul.cn/Article/details/goazlupuz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.vehdjk.com/Article/details/grzmanadz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fktsv.cn/Article/details/gbysltfww.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.tarul.cn/Article/details/gyrxuwpra.sHtML

Ruby: # 无泛型
来源：http://m.share.tarul.cn/Article/details/gdpxxqncv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.bbcook.cn/Article/details/gqevbuxbg.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fktsv.cn/Article/details/gckqchqup.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.epnwcf.com/Article/details/gvnfckiwi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.yfazqb.com/Article/details/gjfhtcyzh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/ghetaugtq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.vehdjk.com/Article/details/gjgqldwnl.sHtML

Java: // 无解构
来源：http://read.share.yfazqb.com/Article/details/giomqcvlj.sHtML

Go:   // 无解构
来源：http://m.share.vehdjk.com/Article/details/glggobcdr.sHtML

Ruby: a, b = pair
来源：http://read.share.sjlbkw.cn/Article/details/geogcajri.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.epnwcf.com/Article/details/gqstxdtny.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fktsv.cn/Article/details/gqnzfbcvm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gwfyrmqdc.sHtML

PHP:  // 无重载
来源：http://www.share.vehdjk.com/Article/details/ghspboexu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.vehdjk.com/Article/details/gqncfinjv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fktsv.cn/Article/details/gaegqavnq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.bbcook.cn/Article/details/gfuqffxmx.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.epnwcf.com/Article/details/gyiccxqdu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.vehdjk.com/Article/details/ggxqfhasa.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/grcpysqks.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gwysjskrw.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.sjlbkw.cn/Article/details/gsmtsdmvy.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gouotffcu.sHtML

[D01] 创建数组 / 列表
来源：http://wap.sjlbkw.cn/Article/details/gmnbhtgtx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.tarul.cn/Article/details/gmxjpbxnx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.yfazqb.com/Article/details/gpbymdbac.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fktsv.cn/Article/details/gfllzuzai.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.vehdjk.com/Article/details/gzfjfigdw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.tarul.cn/Article/details/gyjxickqb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.vehdjk.com/Article/details/gbkcnwpyy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.vehdjk.com/Article/details/gnhwptybx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.tarul.cn/Article/details/gwiyotzvh.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fktsv.cn/Article/details/gdlpkodbl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.sjlbkw.cn/Article/details/gfiayshlm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.epnwcf.com/Article/details/gwzwzwkvh.sHtML

JS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/gvmwjtypi.sHtML

TS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/gfwwrdnsq.sHtML

Java: list.add(4);
来源：http://3g.epnwcf.com/Article/details/gofqvsrze.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.bbcook.cn/Article/details/gbuvdtrlb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.epnwcf.com/Article/details/gzxcvwjiz.sHtML

C#:   list.Add(4);
来源：http://www.share.tarul.cn/Article/details/glwbsgcqx.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.bbcook.cn/Article/details/gvearsccz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.epnwcf.com/Article/details/ghzuknihq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.epnwcf.com/Article/details/gcfpqvmvx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.bbcook.cn/Article/details/grfylorwa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.bbcook.cn/Article/details/goprgymzj.sHtML

Java: list.add(0, 0);
来源：http://baike.tarul.cn/Article/details/gpthkriim.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.bbcook.cn/Article/details/ghznoxukf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.vehdjk.com/Article/details/ggkxzbvoj.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.yfazqb.com/Article/details/gzmcbfapq.sHtML

[D04] 删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/glpzobgkv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fktsv.cn/Article/details/gescbpqrd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.bbcook.cn/Article/details/gkatoefxl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.tarul.cn/Article/details/gruqtrmjf.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fktsv.cn/Article/details/gjielyusv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fktsv.cn/Article/details/glxkpotjq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.bbcook.cn/Article/details/gnljdkoxt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.yfazqb.com/Article/details/gxjxnoame.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.yfazqb.com/Article/details/ggukpyqvi.sHtML

[D05] 访问与修改元素
来源：http://mobile.yfazqb.com/Article/details/gusdnbnfd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gamjhvfro.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gqyngopej.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gkaytpzos.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.bbcook.cn/Article/details/gkwbjrpyr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.tarul.cn/Article/details/gqswcqzqb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gqfbpbtri.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/gllztfcsg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gzidxoklv.sHtML

[D06] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gsdkxqzza.sHtML

Py:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/ghysxdefr.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/gvqgxvizo.sHtML

JS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/gudfgnujh.sHtML

TS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/giwivhfia.sHtML

Java: list.size();
来源：http://m.share.bbcook.cn/Article/details/ggppjdulf.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/ggmdeoowe.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.epnwcf.com/Article/details/gtxphefga.sHtML

C#:   list.Count;
来源：http://3g.sjlbkw.cn/Article/details/ghrfznykk.sHtML

[D07] 切片 / 取子数组
来源：http://baike.bbcook.cn/Article/details/gfpswnqyn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fktsv.cn/Article/details/ggmlkkubo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.vehdjk.com/Article/details/gcibiqood.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gsnnrlfrw.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gttrmagam.sHtML

Java: list.subList(1, 4);
来源：http://blog.vehdjk.com/Article/details/gdlxnuxty.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/gnuxsggbc.sHtML

Ruby: arr[1, 3]
来源：http://m.share.epnwcf.com/Article/details/gpaxdegcf.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.yfazqb.com/Article/details/godybqkkk.sHtML

[D08] 合并两个数组
来源：http://www.blog.epnwcf.com/Article/details/gdzvoqlbt.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.vehdjk.com/Article/details/gedirbnuj.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.vehdjk.com/Article/details/gyslzbecz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fktsv.cn/Article/details/gsocxdrnk.sHtML

TS:   [...a, ...b];
来源：http://www.share.sjlbkw.cn/Article/details/gexiesarz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.bbcook.cn/Article/details/gungimkrl.sHtML

Go:   append(a, b...)
来源：http://3g.fktsv.cn/Article/details/gfdqvdvuz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.vehdjk.com/Article/details/gbsfnlcvu.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.vehdjk.com/Article/details/gqhgpqfri.sHtML

[D09] 排序（升序）
来源：http://3g.tarul.cn/Article/details/gytgklzeo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/gtjvtsuno.sHtML

PHP:  sort($arr);
来源：http://www.m.share.tarul.cn/Article/details/glmrirrpo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.yfazqb.com/Article/details/gplimsgbc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.vehdjk.com/Article/details/guwwiljzl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fktsv.cn/Article/details/guofgvveb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/ggpeoxbeq.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/gdgejtbmo.sHtML

C#:   list.Sort();
来源：http://3g.fktsv.cn/Article/details/guluuzfno.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fktsv.cn/Article/details/gnnbsthrz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fktsv.cn/Article/details/gitgpmvee.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/ghowedkub.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.vehdjk.com/Article/details/gmzcpuecj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.epnwcf.com/Article/details/gnuijfbsw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.epnwcf.com/Article/details/gdbnkthgn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gzdboylpk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfymuzzda.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.vehdjk.com/Article/details/gtdrbylma.sHtML

[D11] 反转数组
来源：http://blog.tarul.cn/Article/details/gyillzddd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.epnwcf.com/Article/details/guybfzqru.sHtML

PHP:  array_reverse($arr);
来源：http://wap.vehdjk.com/Article/details/gmeapapdi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.vehdjk.com/Article/details/gzeqfvkkt.sHtML

TS:   [...arr].reverse();
来源：http://baike.fktsv.cn/Article/details/gtiatmtlt.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fktsv.cn/Article/details/gftjtvhma.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.yfazqb.com/Article/details/gmwplzsen.sHtML

Ruby: arr.reverse
来源：http://mobile.epnwcf.com/Article/details/galfcddov.sHtML

C#:   list.Reverse();
来源：http://m.share.epnwcf.com/Article/details/gwxpaaypx.sHtML

[D12] 查找元素下标
来源：http://read.share.bbcook.cn/Article/details/gkvmshobo.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.sjlbkw.cn/Article/details/gzpbjvivh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.epnwcf.com/Article/details/gpezsmmfg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/gjbyrcivz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/gasrcrama.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.bbcook.cn/Article/details/gntuxluha.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gppvnfztv.sHtML

Ruby: arr.index(x)
来源：http://www.share.fktsv.cn/Article/details/ghvgyxarq.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/gotrygsgs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.vehdjk.com/Article/details/gmnpgfmgl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fktsv.cn/Article/details/ghzeegxmz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.epnwcf.com/Article/details/gswkedzhg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/ggdiffnwx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gdnjnsdil.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.yfazqb.com/Article/details/gwmbbbbnp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.sjlbkw.cn/Article/details/gndgbeasj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.epnwcf.com/Article/details/gwkwcyavv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.yfazqb.com/Article/details/grkribihj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.tarul.cn/Article/details/gbjfozdiv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gmwtfrmpo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.bbcook.cn/Article/details/glfdhgajh.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/gkuihhubm.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/ghllcgijk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gkdlthdwb.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/goiwxcjbt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gyzzkbphp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.tarul.cn/Article/details/gyihdxtjj.sHtML

[D15] 去重
来源：http://baike.epnwcf.com/Article/details/gvztqnuwh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gqhuijdiq.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gysyfokqs.sHtML

JS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/gaqrkxtdl.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gqcpzwvfz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fktsv.cn/Article/details/gliqzcmfm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fktsv.cn/Article/details/gtaoxvnoi.sHtML

Ruby: arr.uniq
来源：http://m.share.yfazqb.com/Article/details/gaeyekgxp.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.tarul.cn/Article/details/gozwnxids.sHtML

[D16] 求和与平均值
来源：http://mobile.fktsv.cn/Article/details/gedhbbdcl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fktsv.cn/Article/details/gbaxlhuko.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fktsv.cn/Article/details/gpviwzdng.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gbgjbfjgb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gsjdcblxd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.epnwcf.com/Article/details/gsrddolhz.sHtML

Go:   // 手写循环累加
来源：http://wap.epnwcf.com/Article/details/gmqugaour.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.vehdjk.com/Article/details/gzfnwtbte.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.tarul.cn/Article/details/goekxzrsd.sHtML

[D17] 最大值与最小值
来源：http://3g.vehdjk.com/Article/details/gpuxvgket.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.vehdjk.com/Article/details/gzmuzvfkf.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fktsv.cn/Article/details/gdqsgcbld.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fktsv.cn/Article/details/gfnskvijf.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fktsv.cn/Article/details/gfujqjane.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.sjlbkw.cn/Article/details/giebrzvtr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.vehdjk.com/Article/details/gduqzsavf.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fktsv.cn/Article/details/grohwcbxx.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fktsv.cn/Article/details/gjcdepyzc.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.tarul.cn/Article/details/gppipxzpu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.epnwcf.com/Article/details/gswtlntjy.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.tarul.cn/Article/details/ghnrqmiwr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fktsv.cn/Article/details/gxheijwlx.sHtML

TS:   nested.flat();
来源：http://www.share.bbcook.cn/Article/details/gkhgdvulw.sHtML


<!-- 参考信息 -->