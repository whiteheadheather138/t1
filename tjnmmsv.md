代发 wailian999

[C02] 默认参数
来源：http://read.share.tarul.cn/Article/details/gzauzojme.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.bbcook.cn/Article/details/gxhbwpyhy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/gvcxhdmho.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/gpdefzplp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gojzgqbke.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.tarul.cn/Article/details/guykbxyen.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fktsv.cn/Article/details/gjnhembwt.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.bbcook.cn/Article/details/ggpcgnltk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.sjlbkw.cn/Article/details/gfawnrwuw.sHtML

[C03] 可变参数
来源：http://wap.epnwcf.com/Article/details/gjbqoagzr.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.bbcook.cn/Article/details/gsnmezjmm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.bbcook.cn/Article/details/gihzsvnlu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/gkkifwvuo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/gzmnyizgk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.vehdjk.com/Article/details/gqnalguiq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.tarul.cn/Article/details/gbkoyssdc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.vehdjk.com/Article/details/grgmpqcja.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.epnwcf.com/Article/details/ghqyolshi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.sjlbkw.cn/Article/details/gieziefet.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.tarul.cn/Article/details/gzurlvgdu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.bbcook.cn/Article/details/gyundvnht.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/ghhutwitn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.vehdjk.com/Article/details/gzwfrxgce.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.tarul.cn/Article/details/guigvglxt.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.vehdjk.com/Article/details/gltjffbtc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gaaiitikq.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/gtqvxbece.sHtML

[C05] 返回多个值
来源：http://blog.fktsv.cn/Article/details/gtrqozxzk.sHtML

Py:   return a, b
来源：http://3g.tarul.cn/Article/details/gyhcewlli.sHtML

PHP:  return [$a, $b];
来源：http://blog.sjlbkw.cn/Article/details/gepdnxilv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.bbcook.cn/Article/details/gtmgppymo.sHtML

TS:   return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gfuiodtac.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.sjlbkw.cn/Article/details/gjvleryrr.sHtML

Go:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gnslasggb.sHtML

Ruby: return a, b
来源：http://blog.fktsv.cn/Article/details/glhakerbg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.vehdjk.com/Article/details/gdbjvqjzg.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/gldcakqfp.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.vehdjk.com/Article/details/gqddgtder.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.tarul.cn/Article/details/ghvtlazhh.sHtML

JS:   const square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/gxenehsoy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gfjdprfic.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gzxejiigw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gwkyxlgbm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.bbcook.cn/Article/details/gsbqfhrtg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gqfoahvnq.sHtML

[C07] 把函数作为参数传入
来源：http://3g.epnwcf.com/Article/details/galmpxdxb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.tarul.cn/Article/details/gduvxjhyi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.yfazqb.com/Article/details/gdgukcpww.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fktsv.cn/Article/details/gwutyfcim.sHtML

TS:   arr.map(String)
来源：http://read.share.yfazqb.com/Article/details/ghgudrmrq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gupwzjues.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.bbcook.cn/Article/details/gbdbvglyr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.tarul.cn/Article/details/goaotvadm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.vehdjk.com/Article/details/gkvnburrt.sHtML

[C08] 闭包
来源：http://baike.bbcook.cn/Article/details/golzofszq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.sjlbkw.cn/Article/details/gqqvipreb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.epnwcf.com/Article/details/gxjjuetcb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gtrszlpgi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gyyuzxuej.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.tarul.cn/Article/details/getogtuwy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.yfazqb.com/Article/details/grfbsahfc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.vehdjk.com/Article/details/ggbbaptgs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gvguwbjav.sHtML

[C09] 递归
来源：http://www.blog.bbcook.cn/Article/details/gohmldlzh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.vehdjk.com/Article/details/gekruliuj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.bbcook.cn/Article/details/gmblazvmu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/gklicejyt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzulwabr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/gegmqszty.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fktsv.cn/Article/details/gzudinvfh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.tarul.cn/Article/details/ggrgpmgff.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fktsv.cn/Article/details/gljzvkagp.sHtML

[C10] 变量作用域
来源：http://3g.tarul.cn/Article/details/gosmlgitx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.bbcook.cn/Article/details/gtcikxaue.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fktsv.cn/Article/details/gnnshojuz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.sjlbkw.cn/Article/details/givzxbxbn.sHtML

TS:   同 JS
来源：http://3g.fktsv.cn/Article/details/gcedbwdiw.sHtML

Java: 方法内为块级作用域
来源：http://blog.fktsv.cn/Article/details/guefzkxzf.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gdocjkvte.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.tarul.cn/Article/details/gxlpuchkk.sHtML

C#:   块级作用域
来源：http://m.share.fktsv.cn/Article/details/gekmkyryr.sHtML

[C11] 模块导入与导出
来源：http://www.share.tarul.cn/Article/details/gyxkyduzs.sHtML

Py:   from module import func
来源：http://blog.fktsv.cn/Article/details/gbelmfuhy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.tarul.cn/Article/details/gctrdwfaw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.bbcook.cn/Article/details/gagcgpbru.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.vehdjk.com/Article/details/gngmfrrkg.sHtML

Java: import java.util.List;
来源：http://wap.fktsv.cn/Article/details/gbolxqpgn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fktsv.cn/Article/details/gmbrzxjdr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.sjlbkw.cn/Article/details/gkfzdkthq.sHtML

C#:   using System.Text;
来源：http://blog.tarul.cn/Article/details/gaservscr.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.sjlbkw.cn/Article/details/gxdsarsop.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.bbcook.cn/Article/details/gdaeyyhig.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.sjlbkw.cn/Article/details/gmlhxoxzc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/gagzvokzy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/gprvbssfq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.bbcook.cn/Article/details/gwosolsof.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fktsv.cn/Article/details/guqioeuap.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.vehdjk.com/Article/details/gajktsduq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gripjdwdu.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.bbcook.cn/Article/details/gplwtdunn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.tarul.cn/Article/details/gbihcxgyj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gfmowjszy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.vehdjk.com/Article/details/gewodprmz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gsrtbuziv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gwthvztmv.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.bbcook.cn/Article/details/gcdnjzcsp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fktsv.cn/Article/details/ghwvgqlvg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fktsv.cn/Article/details/gzhpkkpxv.sHtML

[C14] 泛型函数
来源：http://3g.vehdjk.com/Article/details/gyipzrlne.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.vehdjk.com/Article/details/geyfvjjme.sHtML

PHP:  // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gdfdybypi.sHtML

JS:   // 无泛型
来源：http://www.share.epnwcf.com/Article/details/gjpdtlcrg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.bbcook.cn/Article/details/gitnqkyzz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.vehdjk.com/Article/details/geincuafn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.tarul.cn/Article/details/gqvnpxwif.sHtML

Ruby: # 无泛型
来源：http://www.blog.tarul.cn/Article/details/gphnulzin.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.yfazqb.com/Article/details/gmjawzwkx.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.sjlbkw.cn/Article/details/gszfbgtmf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbnuvcgc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.bbcook.cn/Article/details/gjmmrtqsl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/gekfailhr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.vehdjk.com/Article/details/gnnchgfwi.sHtML

Java: // 无解构
来源：http://wap.vehdjk.com/Article/details/gybwwuuqc.sHtML

Go:   // 无解构
来源：http://wap.epnwcf.com/Article/details/gsxaeqvjw.sHtML

Ruby: a, b = pair
来源：http://3g.vehdjk.com/Article/details/gnfrwsjwc.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.vehdjk.com/Article/details/gbunwxpza.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.tarul.cn/Article/details/gfxopkbes.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.epnwcf.com/Article/details/gnfiuhcgj.sHtML

PHP:  // 无重载
来源：http://wap.tarul.cn/Article/details/gcymvhnxz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.sjlbkw.cn/Article/details/gdyotycwq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.epnwcf.com/Article/details/goymtfzlv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.epnwcf.com/Article/details/gmhpibqdq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.yfazqb.com/Article/details/grycvrrvq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.bbcook.cn/Article/details/gczuijghk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.epnwcf.com/Article/details/greqidzlq.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gzmiazxve.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaqfhwgs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdqjauyyt.sHtML

[D01] 创建数组 / 列表
来源：http://baike.epnwcf.com/Article/details/ggwmhbalg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fktsv.cn/Article/details/gzhvzdgsz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.yfazqb.com/Article/details/gurnwaiyb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.epnwcf.com/Article/details/gphtayagy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.bbcook.cn/Article/details/gztbzwrtv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.yfazqb.com/Article/details/getvlbqzn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.epnwcf.com/Article/details/gvwywaxtn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gtsmnyfow.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fktsv.cn/Article/details/gzjuonres.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fktsv.cn/Article/details/gynkdivwd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.vehdjk.com/Article/details/gfgvvegtk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.sjlbkw.cn/Article/details/gekgljnaj.sHtML

JS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gpcwhhagx.sHtML

TS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/ghthmtyns.sHtML

Java: list.add(4);
来源：http://blog.fktsv.cn/Article/details/gwxwmhghw.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.vehdjk.com/Article/details/gewbiorxr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.vehdjk.com/Article/details/gumjwfgsx.sHtML

C#:   list.Add(4);
来源：http://www.m.share.yfazqb.com/Article/details/gztzzeogb.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.yfazqb.com/Article/details/ghfpsiznb.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.vehdjk.com/Article/details/gpbdczssi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.bbcook.cn/Article/details/grhpidlvy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.tarul.cn/Article/details/gzaljzqkf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.yfazqb.com/Article/details/goemsmhjn.sHtML

Java: list.add(0, 0);
来源：http://mobile.tarul.cn/Article/details/gpviqxqvc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.bbcook.cn/Article/details/ggftzzjox.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fktsv.cn/Article/details/gaeujdeuq.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/grwcxskgp.sHtML

[D04] 删除元素
来源：http://blog.fktsv.cn/Article/details/gnzkudirh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.epnwcf.com/Article/details/gsauvvkyt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gqdgahxgb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.vehdjk.com/Article/details/gyabptnft.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fktsv.cn/Article/details/gxjjidlsn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.yfazqb.com/Article/details/gxrxgpfsq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.vehdjk.com/Article/details/gblgdhfms.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.vehdjk.com/Article/details/gktedjnot.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.tarul.cn/Article/details/goppzvtkb.sHtML

[D05] 访问与修改元素
来源：http://3g.tarul.cn/Article/details/gmzgobhab.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/gvlpvzmby.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/galzyrhcx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gavrpuuha.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.sjlbkw.cn/Article/details/gflvfzsfw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.sjlbkw.cn/Article/details/gopgjksqv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gvmnloafp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gkhqoxzfo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gxanaaowv.sHtML

[D06] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gqumiyitd.sHtML

Py:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/gjxepypzf.sHtML

PHP:  count($arr);
来源：http://read.share.vehdjk.com/Article/details/gurpdtnri.sHtML

JS:   arr.length
来源：http://baike.bbcook.cn/Article/details/glskgxgmv.sHtML

TS:   arr.length
来源：http://3g.fktsv.cn/Article/details/gedwhqdtu.sHtML

Java: list.size();
来源：http://wap.fktsv.cn/Article/details/gchhefbpj.sHtML

Go:   len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gnoovtxrc.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.tarul.cn/Article/details/gjxtczgdi.sHtML

C#:   list.Count;
来源：http://read.share.bbcook.cn/Article/details/gpvbdhhuu.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.bbcook.cn/Article/details/grxvtcuya.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fktsv.cn/Article/details/gngttubss.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gggjictgs.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/ggmezjtrw.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gtpclzodq.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gvjkmwchq.sHtML

Go:   arr[1:4]
来源：http://baike.epnwcf.com/Article/details/gdbrunaoc.sHtML

Ruby: arr[1, 3]
来源：http://3g.yfazqb.com/Article/details/gghvlvnsr.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.tarul.cn/Article/details/ghagmeetu.sHtML

[D08] 合并两个数组
来源：http://m.share.fktsv.cn/Article/details/gswyudamj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.epnwcf.com/Article/details/gxgfrjvqx.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.yfazqb.com/Article/details/gsdkcqevz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.sjlbkw.cn/Article/details/gysikbybv.sHtML

TS:   [...a, ...b];
来源：http://baike.tarul.cn/Article/details/gneasxhcc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fktsv.cn/Article/details/gxmmrogao.sHtML

Go:   append(a, b...)
来源：http://wap.yfazqb.com/Article/details/gfujmumzu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.yfazqb.com/Article/details/ghwkbtbxy.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.tarul.cn/Article/details/gcwdausiv.sHtML

[D09] 排序（升序）
来源：http://baike.sjlbkw.cn/Article/details/gnumgcexk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/ghkbcgxyp.sHtML

PHP:  sort($arr);
来源：http://baike.fktsv.cn/Article/details/gnonjvtre.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fktsv.cn/Article/details/gaiykuasz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fktsv.cn/Article/details/ggrgjbofm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.epnwcf.com/Article/details/gkejqquuk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.epnwcf.com/Article/details/gokdaygja.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gkbqrnmlx.sHtML

C#:   list.Sort();
来源：http://baike.sjlbkw.cn/Article/details/grpexublv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.epnwcf.com/Article/details/gqwiadocx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.yfazqb.com/Article/details/gpwojhhqq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gmuawntdy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.bbcook.cn/Article/details/gmgjitqjo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gcasvjwqj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.tarul.cn/Article/details/glajayopa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.epnwcf.com/Article/details/gpqcmfvpg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.sjlbkw.cn/Article/details/gcykkjskp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.vehdjk.com/Article/details/gkysihyni.sHtML

[D11] 反转数组
来源：http://www.share.vehdjk.com/Article/details/gqkdlxdip.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.epnwcf.com/Article/details/gqvxqmitx.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.bbcook.cn/Article/details/goxzaqugu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.vehdjk.com/Article/details/gxaibbdgg.sHtML

TS:   [...arr].reverse();
来源：http://3g.vehdjk.com/Article/details/glnsrjdgg.sHtML

Java: Collections.reverse(list);
来源：http://m.share.yfazqb.com/Article/details/ghujnshym.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.yfazqb.com/Article/details/gyajguhti.sHtML

Ruby: arr.reverse
来源：http://blog.epnwcf.com/Article/details/gqvwrcsxc.sHtML

C#:   list.Reverse();
来源：http://m.share.yfazqb.com/Article/details/gssgkauxq.sHtML

[D12] 查找元素下标
来源：http://mobile.sjlbkw.cn/Article/details/gjtfnzykv.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.epnwcf.com/Article/details/gwabixdya.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.epnwcf.com/Article/details/gnsksnwex.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gqlyxulbg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gtuncbgex.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.tarul.cn/Article/details/ghpmdagkg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.vehdjk.com/Article/details/ghqztvmcs.sHtML

Ruby: arr.index(x)
来源：http://3g.tarul.cn/Article/details/geotphivs.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.tarul.cn/Article/details/gvpzmirvm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.yfazqb.com/Article/details/guzlfqfij.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.bbcook.cn/Article/details/geqmuaprg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.sjlbkw.cn/Article/details/gkhqbwgxl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/grrnnkaxk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.yfazqb.com/Article/details/gczyfqupu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.sjlbkw.cn/Article/details/getjxytkz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fktsv.cn/Article/details/ghbrdxvav.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fktsv.cn/Article/details/gxljtaplt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.vehdjk.com/Article/details/gqjjqtsle.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.epnwcf.com/Article/details/gdlgqbzmk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fktsv.cn/Article/details/gtcxgwiim.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.vehdjk.com/Article/details/gxgpcmgrz.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.tarul.cn/Article/details/glelwdtcd.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.bbcook.cn/Article/details/gzfzlpnrs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.tarul.cn/Article/details/gsgtqmtur.sHtML

Go:   // 手写循环
来源：http://baike.sjlbkw.cn/Article/details/gvwqvltjc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/glpirhpst.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gvoeaspxe.sHtML

[D15] 去重
来源：http://wap.bbcook.cn/Article/details/gwyfbftdq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/gelkxpvgi.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gqvyycooh.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gkbwemjci.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gbgllfcup.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.bbcook.cn/Article/details/gyhfzjkni.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.epnwcf.com/Article/details/gsqtvmqan.sHtML

Ruby: arr.uniq
来源：http://blog.sjlbkw.cn/Article/details/geqonzpgv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.vehdjk.com/Article/details/gfnouhqfx.sHtML

[D16] 求和与平均值
来源：http://www.m.share.vehdjk.com/Article/details/gycvaaizi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.vehdjk.com/Article/details/gessmuapn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.epnwcf.com/Article/details/grebsccuu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fktsv.cn/Article/details/gzaxmksgr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fktsv.cn/Article/details/gncdudoox.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.sjlbkw.cn/Article/details/ghsaiwnsk.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.epnwcf.com/Article/details/gtgwlyqnw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.tarul.cn/Article/details/gvjnwxlum.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fktsv.cn/Article/details/gurvidaou.sHtML

[D17] 最大值与最小值
来源：http://www.blog.bbcook.cn/Article/details/gnctlvuoo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gsusksreg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.epnwcf.com/Article/details/gnupqcjdi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.sjlbkw.cn/Article/details/gjjoqfivm.sHtML

TS:   Math.max(...arr);
来源：http://baike.fktsv.cn/Article/details/grjrhnodo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.yfazqb.com/Article/details/gkvkstvkq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.vehdjk.com/Article/details/gofqwtgmo.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.epnwcf.com/Article/details/gjojqevjo.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.yfazqb.com/Article/details/gmtsxzcqr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fktsv.cn/Article/details/glvqeksmm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fktsv.cn/Article/details/gwhxzbpti.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fktsv.cn/Article/details/gycpfpcpt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.bbcook.cn/Article/details/gyggufdey.sHtML

TS:   nested.flat();
来源：http://www.m.share.epnwcf.com/Article/details/gmbpkdjex.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.bbcook.cn/Article/details/gquvljwkt.sHtML

Go:   // 手写双层循环
来源：http://baike.bbcook.cn/Article/details/ghtirsgfn.sHtML

Ruby: nested.flatten
来源：http://www.m.share.tarul.cn/Article/details/giqdnwnyp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fktsv.cn/Article/details/gevwcmqjx.sHtML


<!-- 参考信息 -->