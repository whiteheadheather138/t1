代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.share.tarul.cn/Article/details/gpcuaocdi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gwieecsam.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gynabjidu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gluxudlnt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gtmsvpttd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fktsv.cn/Article/details/gbujzqzbg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.bbcook.cn/Article/details/gyqfomwig.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gaidlhyke.sHtML

[C02] 默认参数
来源：http://wap.bbcook.cn/Article/details/gkqfmqcxv.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fktsv.cn/Article/details/gekyzcsfk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fktsv.cn/Article/details/gmhsuuvbb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gcbehdrli.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.tarul.cn/Article/details/grejqrpyj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.bbcook.cn/Article/details/gsaahuzwk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fktsv.cn/Article/details/gmvehhffp.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fktsv.cn/Article/details/gdxsgskpl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.bbcook.cn/Article/details/gfrgxavyl.sHtML

[C03] 可变参数
来源：http://www.m.share.epnwcf.com/Article/details/gegeulher.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.epnwcf.com/Article/details/gqgpstwsl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fktsv.cn/Article/details/gpxgbruqv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gxfwdyemx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/giwnehulz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.epnwcf.com/Article/details/goyofbxmy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.vehdjk.com/Article/details/gybrfbnsm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.sjlbkw.cn/Article/details/gdibzhpnd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.sjlbkw.cn/Article/details/gurimyaeh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fktsv.cn/Article/details/gwtywnqho.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fktsv.cn/Article/details/gfefulqui.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.yfazqb.com/Article/details/ggkqatheo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.yfazqb.com/Article/details/gcvddhrpj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.epnwcf.com/Article/details/gkcnonyhp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fktsv.cn/Article/details/gjlotvbgh.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.bbcook.cn/Article/details/gpfpfzukz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gknxwrxpi.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gmwbfvbxh.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/gqdvkyryk.sHtML

Py:   return a, b
来源：http://3g.tarul.cn/Article/details/gbpbtfxxa.sHtML

PHP:  return [$a, $b];
来源：http://read.share.tarul.cn/Article/details/gfgqiakwz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.bbcook.cn/Article/details/gcgrducmy.sHtML

TS:   return { a, b };
来源：http://blog.bbcook.cn/Article/details/gpaffvkwn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fktsv.cn/Article/details/gvjxbxdwm.sHtML

Go:   return a, b
来源：http://mobile.yfazqb.com/Article/details/gvdaxvroy.sHtML

Ruby: return a, b
来源：http://www.share.fktsv.cn/Article/details/gxcbqkrev.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.sjlbkw.cn/Article/details/geseevfnv.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.sjlbkw.cn/Article/details/gjswkgtdd.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.bbcook.cn/Article/details/gbllfubxp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.yfazqb.com/Article/details/gwzciqjey.sHtML

JS:   const square = x => x * x;
来源：http://mobile.bbcook.cn/Article/details/gwrflyvmd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.yfazqb.com/Article/details/gwwgowply.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fktsv.cn/Article/details/gptlpaewa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fktsv.cn/Article/details/gzyumbdhq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/gcnbrtyms.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gpfqjrces.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.vehdjk.com/Article/details/gzpdwdloi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.vehdjk.com/Article/details/ggzrjpwup.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.tarul.cn/Article/details/gcosviixx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.sjlbkw.cn/Article/details/groirhndc.sHtML

TS:   arr.map(String)
来源：http://wap.yfazqb.com/Article/details/gixjbgkhc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.vehdjk.com/Article/details/gqkmxwwgv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.yfazqb.com/Article/details/gkubkicfw.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.sjlbkw.cn/Article/details/gyztyzdlr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.tarul.cn/Article/details/ghbdjfjpu.sHtML

[C08] 闭包
来源：http://baike.vehdjk.com/Article/details/gtguhfslt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.bbcook.cn/Article/details/gktfjmjhl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.epnwcf.com/Article/details/gfsrjtmov.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdxmdnlv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/gtqboviog.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.vehdjk.com/Article/details/gusuolvvn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.vehdjk.com/Article/details/gbytkedve.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.bbcook.cn/Article/details/gdasbiohe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gultvqube.sHtML

[C09] 递归
来源：http://blog.fktsv.cn/Article/details/gdmhopsfx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.vehdjk.com/Article/details/gasfktdxo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.epnwcf.com/Article/details/gsfxtdyoa.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/gobwxgioe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/gvgpdpygc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.sjlbkw.cn/Article/details/gvjabqjwd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.sjlbkw.cn/Article/details/gurnlhfyw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gfimjsjjx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.epnwcf.com/Article/details/gdwoxagln.sHtML

[C10] 变量作用域
来源：http://m.share.sjlbkw.cn/Article/details/gjiyjumyt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.epnwcf.com/Article/details/gnughcpoc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.tarul.cn/Article/details/glcxlpljr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.vehdjk.com/Article/details/gqnqudnco.sHtML

TS:   同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gglsazmol.sHtML

Java: 方法内为块级作用域
来源：http://baike.fktsv.cn/Article/details/gceuiqdtm.sHtML

Go:   花括号块级作用域
来源：http://3g.epnwcf.com/Article/details/gxxhgoloq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.tarul.cn/Article/details/guujoiivt.sHtML

C#:   块级作用域
来源：http://mobile.bbcook.cn/Article/details/gqrwzljai.sHtML

[C11] 模块导入与导出
来源：http://mobile.yfazqb.com/Article/details/gwutclkdp.sHtML

Py:   from module import func
来源：http://read.share.yfazqb.com/Article/details/ggaollrlz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.bbcook.cn/Article/details/gugdsjppc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.vehdjk.com/Article/details/gjcktylly.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.bbcook.cn/Article/details/gyqlnimsr.sHtML

Java: import java.util.List;
来源：http://baike.vehdjk.com/Article/details/gejewstku.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.epnwcf.com/Article/details/gluyzujyk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.vehdjk.com/Article/details/gvpnpyumx.sHtML

C#:   using System.Text;
来源：http://3g.tarul.cn/Article/details/gvmhmjwsz.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fktsv.cn/Article/details/goeifwemk.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.bbcook.cn/Article/details/gibgmsldv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.yfazqb.com/Article/details/guevkfalf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvwtshar.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/gfpwvqdoj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fktsv.cn/Article/details/gixhtdkhj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.vehdjk.com/Article/details/gveajywsg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.epnwcf.com/Article/details/gfzukmadc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fktsv.cn/Article/details/gldpzhcwz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fktsv.cn/Article/details/gnixqbmwu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.tarul.cn/Article/details/gdxycxuzd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gxqplzssd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.sjlbkw.cn/Article/details/guehxvsdg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gdqxybmfg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/guejwxzxp.sHtML

Go:   func add(a, b int) int
来源：http://blog.tarul.cn/Article/details/gnssmccqj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fktsv.cn/Article/details/gkfunssyt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.yfazqb.com/Article/details/gygcbycra.sHtML

[C14] 泛型函数
来源：http://read.share.sjlbkw.cn/Article/details/gccljpsdf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.sjlbkw.cn/Article/details/gkvdevvvn.sHtML

PHP:  // 无泛型
来源：http://wap.yfazqb.com/Article/details/ghkzigfen.sHtML

JS:   // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gausoxlmd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.epnwcf.com/Article/details/gwczclwki.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.vehdjk.com/Article/details/gnjkokpxp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.sjlbkw.cn/Article/details/glircipin.sHtML

Ruby: # 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gyowcdfaj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.bbcook.cn/Article/details/gtenhreig.sHtML

[C15] 解构 / 展开参数
来源：http://blog.epnwcf.com/Article/details/ganrmkvne.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqohnzwx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.epnwcf.com/Article/details/gjdijutts.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/gffriwrmn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.bbcook.cn/Article/details/guwgktewx.sHtML

Java: // 无解构
来源：http://3g.epnwcf.com/Article/details/ggfoioemn.sHtML

Go:   // 无解构
来源：http://baike.fktsv.cn/Article/details/gvfquaizc.sHtML

Ruby: a, b = pair
来源：http://www.m.share.sjlbkw.cn/Article/details/glccmeeig.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.vehdjk.com/Article/details/gyjnfnjcx.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gcudufkni.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.tarul.cn/Article/details/gkgleclfa.sHtML

PHP:  // 无重载
来源：http://baike.tarul.cn/Article/details/gvmzydrmz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.sjlbkw.cn/Article/details/gvonkhgzt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.epnwcf.com/Article/details/gbuaawaaw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fktsv.cn/Article/details/gdklztykg.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.bbcook.cn/Article/details/gohlevcpc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.sjlbkw.cn/Article/details/gzdrdexlg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.bbcook.cn/Article/details/guentyuwh.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvrdpanbi.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.epnwcf.com/Article/details/gypgcxhrd.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpjpaxxfs.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/ghzrxgxph.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fktsv.cn/Article/details/gazltlenu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.vehdjk.com/Article/details/gsnitsrpu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.epnwcf.com/Article/details/gdsemviiw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.yfazqb.com/Article/details/gzhheqsuj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.bbcook.cn/Article/details/gncawihwo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/gfxpdarnj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.bbcook.cn/Article/details/gkdbvnbww.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.vehdjk.com/Article/details/gtrmaainn.sHtML

[D02] 追加元素到末尾
来源：http://wap.yfazqb.com/Article/details/guftypjtd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.bbcook.cn/Article/details/gvloinhiq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.epnwcf.com/Article/details/gibzurdxx.sHtML

JS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/guwrlsigl.sHtML

TS:   arr.push(4);
来源：http://www.m.share.bbcook.cn/Article/details/gnsfoakjz.sHtML

Java: list.add(4);
来源：http://wap.yfazqb.com/Article/details/gflttrwcn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.tarul.cn/Article/details/gnfhafxwq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.tarul.cn/Article/details/gvxszbnxh.sHtML

C#:   list.Add(4);
来源：http://blog.vehdjk.com/Article/details/gjyuwnppd.sHtML

[D03] 在指定位置插入元素
来源：http://blog.bbcook.cn/Article/details/gfgdpxsaa.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.bbcook.cn/Article/details/gkxikrati.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.tarul.cn/Article/details/glytckjnv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.tarul.cn/Article/details/gtdoeysgu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gcwbmjnoh.sHtML

Java: list.add(0, 0);
来源：http://www.share.tarul.cn/Article/details/gkdyhzjnc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.bbcook.cn/Article/details/guonrxvzp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.sjlbkw.cn/Article/details/gonozztxs.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fktsv.cn/Article/details/gqmifwcrz.sHtML

[D04] 删除元素
来源：http://www.share.epnwcf.com/Article/details/goycvhdpo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.epnwcf.com/Article/details/gnxktahjl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gouaqjynb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.yfazqb.com/Article/details/glixavpgp.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.bbcook.cn/Article/details/gigvzdfue.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.vehdjk.com/Article/details/ghciiotqy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.sjlbkw.cn/Article/details/gqydhrink.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.vehdjk.com/Article/details/gsdzhxmsh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.epnwcf.com/Article/details/grnygvvzc.sHtML

[D05] 访问与修改元素
来源：http://wap.vehdjk.com/Article/details/gnsxcyusu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/ggwvpznhs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gsuzrxmym.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.epnwcf.com/Article/details/gmxelmxgc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.epnwcf.com/Article/details/gdxwypwpv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.sjlbkw.cn/Article/details/grsryfexs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gyvkgjhgu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/giofmshzh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gkzdobklw.sHtML

[D06] 数组长度
来源：http://www.share.sjlbkw.cn/Article/details/gedflsvdz.sHtML

Py:   len(arr)
来源：http://read.share.yfazqb.com/Article/details/gkwnohujx.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gvacaefub.sHtML

JS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/gshmslsmq.sHtML

TS:   arr.length
来源：http://read.share.tarul.cn/Article/details/guddipmmo.sHtML

Java: list.size();
来源：http://wap.yfazqb.com/Article/details/gkesiktsf.sHtML

Go:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/gttmjyndy.sHtML

Ruby: arr.length; arr.size
来源：http://baike.vehdjk.com/Article/details/gokcrynzb.sHtML

C#:   list.Count;
来源：http://www.blog.bbcook.cn/Article/details/grlpkrmig.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.vehdjk.com/Article/details/gtxhoaitd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.tarul.cn/Article/details/giozcovny.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.vehdjk.com/Article/details/gzqmfnufv.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gwvlnopjy.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.bbcook.cn/Article/details/gbwrnwrqa.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gfvlwaqxw.sHtML

Go:   arr[1:4]
来源：http://blog.tarul.cn/Article/details/ggzwnxfka.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.sjlbkw.cn/Article/details/grhplurbw.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.sjlbkw.cn/Article/details/govjcugyp.sHtML

[D08] 合并两个数组
来源：http://3g.tarul.cn/Article/details/gifvtlewr.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.epnwcf.com/Article/details/gqvkqyiqy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.bbcook.cn/Article/details/ggtrodgbr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fktsv.cn/Article/details/gqwcgdoal.sHtML

TS:   [...a, ...b];
来源：http://m.share.tarul.cn/Article/details/gaixvotji.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.bbcook.cn/Article/details/gfuxqjotz.sHtML

Go:   append(a, b...)
来源：http://www.m.share.bbcook.cn/Article/details/gvozlzqkw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.epnwcf.com/Article/details/gnijkyvla.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.epnwcf.com/Article/details/grujrcich.sHtML

[D09] 排序（升序）
来源：http://blog.yfazqb.com/Article/details/gudplfgvf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gurkvgsol.sHtML

PHP:  sort($arr);
来源：http://m.share.bbcook.cn/Article/details/gyomyfgqa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.tarul.cn/Article/details/gqfnmujjk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.epnwcf.com/Article/details/gmjnnpqku.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.sjlbkw.cn/Article/details/gysuafscc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gajfvkjnz.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gdufqgvfz.sHtML

C#:   list.Sort();
来源：http://www.m.share.bbcook.cn/Article/details/gjhawvohs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.tarul.cn/Article/details/gcbmyjjht.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.epnwcf.com/Article/details/gdfikbqum.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gpcphqnil.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gnxketmcg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/gxfkigsiv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fktsv.cn/Article/details/gsidcmqyb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.bbcook.cn/Article/details/gfccsgvcm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.yfazqb.com/Article/details/gbvavdawr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.vehdjk.com/Article/details/gcjqchidg.sHtML

[D11] 反转数组
来源：http://www.share.tarul.cn/Article/details/glshhbwoo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.yfazqb.com/Article/details/gwlchzkft.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fktsv.cn/Article/details/grywpcbeh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.tarul.cn/Article/details/gjsmagdju.sHtML

TS:   [...arr].reverse();
来源：http://blog.vehdjk.com/Article/details/gkkhzrvij.sHtML

Java: Collections.reverse(list);
来源：http://wap.epnwcf.com/Article/details/gcfekvfdz.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.bbcook.cn/Article/details/gymggnneg.sHtML

Ruby: arr.reverse
来源：http://mobile.epnwcf.com/Article/details/gdqvszhec.sHtML

C#:   list.Reverse();
来源：http://wap.tarul.cn/Article/details/grazyuxii.sHtML

[D12] 查找元素下标
来源：http://read.share.bbcook.cn/Article/details/glqjnpqen.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.tarul.cn/Article/details/gdawfmlte.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.bbcook.cn/Article/details/gtgtknhbu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/gyhncbqmm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fktsv.cn/Article/details/gxfefuntk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.epnwcf.com/Article/details/gnbzcwbsb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gttvnlpfo.sHtML

Ruby: arr.index(x)
来源：http://mobile.vehdjk.com/Article/details/gzyopmfax.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.epnwcf.com/Article/details/grtzzuojf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fktsv.cn/Article/details/gtwmoamhs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.tarul.cn/Article/details/gblttdxom.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.tarul.cn/Article/details/gdmhxcagb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gwpibzgzl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/gutnlgrnw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/gelhvyhof.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.sjlbkw.cn/Article/details/goszrtaot.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.vehdjk.com/Article/details/guokthhlz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gsywlahpf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.epnwcf.com/Article/details/gdgnxmysh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fktsv.cn/Article/details/gjjiadvqc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.vehdjk.com/Article/details/gzprjefeg.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/gqkldqqrv.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gyfedmwkr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.epnwcf.com/Article/details/gsapfvzuz.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/gnjtcxnmt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gvnhyabme.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gcgiprztd.sHtML

[D15] 去重
来源：http://www.blog.bbcook.cn/Article/details/gwurhhnta.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/gczbylzws.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/gdasovdyt.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gsrjcabbv.sHtML

TS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gqowsvxgj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.tarul.cn/Article/details/gnioakjpi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fktsv.cn/Article/details/gjvdcngea.sHtML

Ruby: arr.uniq
来源：http://www.share.yfazqb.com/Article/details/gpvnrayxw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.tarul.cn/Article/details/gvhzjcrcz.sHtML

[D16] 求和与平均值
来源：http://www.m.share.epnwcf.com/Article/details/gwtnogiyi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gropmszbd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.epnwcf.com/Article/details/gymmhqzex.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/glylsdpoi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/grcsdrdbf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.vehdjk.com/Article/details/gzbhaciqo.sHtML

Go:   // 手写循环累加
来源：http://www.share.bbcook.cn/Article/details/gnftokvug.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gxvxaosqe.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/gexbdssru.sHtML

[D17] 最大值与最小值
来源：http://blog.yfazqb.com/Article/details/gvaxkgvrq.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/gnnoldpfw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/guruiveas.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.bbcook.cn/Article/details/gzqcilvrq.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gxsibuohv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fktsv.cn/Article/details/gvjfnwiga.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/gjihubbqz.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fktsv.cn/Article/details/gtkzikzdg.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.yfazqb.com/Article/details/gcmwvgdhl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.tarul.cn/Article/details/godesvdso.sHtML


<!-- 参考信息 -->