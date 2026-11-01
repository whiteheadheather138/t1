代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/glrdmekor.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gecnddqqa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.tarul.cn/Article/details/gyropvdgx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gzfahtmfi.sHtML

[C02] 默认参数
来源：http://blog.yfazqb.com/Article/details/gxticipfr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.vehdjk.com/Article/details/gwdryuugn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.epnwcf.com/Article/details/gibtepzyo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/grfoeddge.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/grhwwuzvp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fktsv.cn/Article/details/gzxvereih.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.sjlbkw.cn/Article/details/gaudqbhde.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.bbcook.cn/Article/details/ghuqgycac.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.tarul.cn/Article/details/gujeljeej.sHtML

[C03] 可变参数
来源：http://m.share.tarul.cn/Article/details/gdspihnwm.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.sjlbkw.cn/Article/details/gbucwopza.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fktsv.cn/Article/details/gafvwymxj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.vehdjk.com/Article/details/gavploezl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fktsv.cn/Article/details/gjflzbken.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.epnwcf.com/Article/details/gqsjuachc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.yfazqb.com/Article/details/giulwrcxh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.bbcook.cn/Article/details/gyjxmxusk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.vehdjk.com/Article/details/gzrsmstfq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fktsv.cn/Article/details/glkjgkikk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fktsv.cn/Article/details/gjtlakdqc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fktsv.cn/Article/details/gqldalocs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/gbgqolazs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fktsv.cn/Article/details/gxqdmeupw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.sjlbkw.cn/Article/details/gvceyyrwn.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.epnwcf.com/Article/details/ggvbkvgsa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gfvtwcpuj.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gfhkcvejb.sHtML

[C05] 返回多个值
来源：http://blog.bbcook.cn/Article/details/gdunakbpe.sHtML

Py:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gbklfufgw.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.vehdjk.com/Article/details/glhshblox.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/gtsrfjpyi.sHtML

TS:   return { a, b };
来源：http://3g.epnwcf.com/Article/details/griwnjfki.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.epnwcf.com/Article/details/gznemxdbk.sHtML

Go:   return a, b
来源：http://read.share.tarul.cn/Article/details/gwotywtmm.sHtML

Ruby: return a, b
来源：http://3g.fktsv.cn/Article/details/gihlrljke.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.bbcook.cn/Article/details/gbfpkkexo.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.bbcook.cn/Article/details/gpwrxocjg.sHtML

Py:   square = lambda x: x * x
来源：http://3g.epnwcf.com/Article/details/geaenbnjf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.epnwcf.com/Article/details/ghrrflvzj.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.yfazqb.com/Article/details/gkafwuikd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.epnwcf.com/Article/details/gzpnueyoj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.yfazqb.com/Article/details/gqklyfhsd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.tarul.cn/Article/details/gvphehywp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.sjlbkw.cn/Article/details/gvkuaxued.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gqmwbhifm.sHtML

[C07] 把函数作为参数传入
来源：http://blog.vehdjk.com/Article/details/guudtvbfh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.bbcook.cn/Article/details/glaepkcvu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.yfazqb.com/Article/details/gzvwrgioq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fktsv.cn/Article/details/geihgvivd.sHtML

TS:   arr.map(String)
来源：http://blog.vehdjk.com/Article/details/gemefmpwy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/ggaherxgs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.epnwcf.com/Article/details/gpjwwufbl.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.bbcook.cn/Article/details/gorewvbfm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.sjlbkw.cn/Article/details/gugrdomiy.sHtML

[C08] 闭包
来源：http://mobile.tarul.cn/Article/details/gydlehcbc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.epnwcf.com/Article/details/gjssleagk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.tarul.cn/Article/details/gbauufjth.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gcfyujuwo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gatwbibqh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.epnwcf.com/Article/details/gbhphpovy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.epnwcf.com/Article/details/gybqcyjni.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.vehdjk.com/Article/details/gldvzrcxk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gedhwwqae.sHtML

[C09] 递归
来源：http://baike.epnwcf.com/Article/details/gxvkfjbzf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/gdjbhagnx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.epnwcf.com/Article/details/gipsrbfod.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/gclstuvvk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/gnfewbqmd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.bbcook.cn/Article/details/gmsyzmaxc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.epnwcf.com/Article/details/gcchuccvf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.sjlbkw.cn/Article/details/glfjlgzhz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.sjlbkw.cn/Article/details/gtsjcpbuj.sHtML

[C10] 变量作用域
来源：http://www.m.share.tarul.cn/Article/details/gubbxlqag.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.yfazqb.com/Article/details/gcsrysojq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.vehdjk.com/Article/details/gldsrmond.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.yfazqb.com/Article/details/gtgoktxkt.sHtML

TS:   同 JS
来源：http://m.share.epnwcf.com/Article/details/gctjiymdi.sHtML

Java: 方法内为块级作用域
来源：http://wap.tarul.cn/Article/details/gvudmewee.sHtML

Go:   花括号块级作用域
来源：http://3g.bbcook.cn/Article/details/gllkstkew.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.sjlbkw.cn/Article/details/gvxnmcgqf.sHtML

C#:   块级作用域
来源：http://wap.vehdjk.com/Article/details/gsbftgxut.sHtML

[C11] 模块导入与导出
来源：http://3g.tarul.cn/Article/details/gwfqtknoj.sHtML

Py:   from module import func
来源：http://blog.sjlbkw.cn/Article/details/gfrjdnblj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fktsv.cn/Article/details/gyldsfmlh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.vehdjk.com/Article/details/gykzzonso.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.epnwcf.com/Article/details/gixfxvkkc.sHtML

Java: import java.util.List;
来源：http://baike.tarul.cn/Article/details/gjcvdhflo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.epnwcf.com/Article/details/gcarfofkt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.tarul.cn/Article/details/gpbjeboli.sHtML

C#:   using System.Text;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkghaqnsh.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.bbcook.cn/Article/details/gxfgfwuoi.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.tarul.cn/Article/details/giolimloq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.tarul.cn/Article/details/gvfouyooc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fktsv.cn/Article/details/gjiqhhjgm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/gpwkmrrtx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.bbcook.cn/Article/details/gptlabgyy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.yfazqb.com/Article/details/gspeyjgzz.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fktsv.cn/Article/details/giyiovbih.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fktsv.cn/Article/details/gprhxssrg.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.bbcook.cn/Article/details/gtkvsziad.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.tarul.cn/Article/details/ghvjkhxht.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glsteoife.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.vehdjk.com/Article/details/gswlmrvie.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.epnwcf.com/Article/details/giqesdzfb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gxdlpqcij.sHtML

Go:   func add(a, b int) int
来源：http://www.share.bbcook.cn/Article/details/gneytgujl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fktsv.cn/Article/details/gfjupwmsa.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.epnwcf.com/Article/details/ggqevapnv.sHtML

[C14] 泛型函数
来源：http://3g.vehdjk.com/Article/details/gozluisrd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.vehdjk.com/Article/details/giznvipfu.sHtML

PHP:  // 无泛型
来源：http://www.share.epnwcf.com/Article/details/guhkjnozc.sHtML

JS:   // 无泛型
来源：http://baike.epnwcf.com/Article/details/gjcuzzoiz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.vehdjk.com/Article/details/gfeypqfxx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.tarul.cn/Article/details/gjuymhiva.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.vehdjk.com/Article/details/gikqztsmb.sHtML

Ruby: # 无泛型
来源：http://mobile.epnwcf.com/Article/details/goaaprdmj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.epnwcf.com/Article/details/gtgludlhr.sHtML

[C15] 解构 / 展开参数
来源：http://baike.yfazqb.com/Article/details/gfsdemvfg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.sjlbkw.cn/Article/details/grpsqjjsq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtflbrze.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/gvayhyugl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.epnwcf.com/Article/details/gchehuddw.sHtML

Java: // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gxnbvqdul.sHtML

Go:   // 无解构
来源：http://baike.vehdjk.com/Article/details/gazbixvhp.sHtML

Ruby: a, b = pair
来源：http://read.share.yfazqb.com/Article/details/gqxdnsvyw.sHtML

C#:   var (a, b) = pair;
来源：http://blog.yfazqb.com/Article/details/gfliusqkz.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fktsv.cn/Article/details/gnzchjwnz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.epnwcf.com/Article/details/gowuvevow.sHtML

PHP:  // 无重载
来源：http://www.blog.sjlbkw.cn/Article/details/gnagziatz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fktsv.cn/Article/details/gnvnxebld.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.tarul.cn/Article/details/gfbcbfulj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.epnwcf.com/Article/details/gdmtlcsku.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.tarul.cn/Article/details/gslfijudm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.bbcook.cn/Article/details/gknilusje.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.bbcook.cn/Article/details/ghnggobrg.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvzsmiyyn.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.sjlbkw.cn/Article/details/gznpjrdrz.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ggvnkdydy.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/gpknnkeiw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.tarul.cn/Article/details/ghhtrhgpw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gabsekihr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fktsv.cn/Article/details/ghffsiuxq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.vehdjk.com/Article/details/gzrirokhm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.vehdjk.com/Article/details/glcbvtysr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.sjlbkw.cn/Article/details/gclksmbwz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.vehdjk.com/Article/details/gtxdlypso.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fktsv.cn/Article/details/gvnrmhugn.sHtML

[D02] 追加元素到末尾
来源：http://www.share.yfazqb.com/Article/details/gmqkehsub.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.yfazqb.com/Article/details/gkvumygog.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.bbcook.cn/Article/details/gllgrqwuf.sHtML

JS:   arr.push(4);
来源：http://read.share.tarul.cn/Article/details/gyprcefpt.sHtML

TS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gxjluxavl.sHtML

Java: list.add(4);
来源：http://blog.bbcook.cn/Article/details/gtgjgrfpe.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.bbcook.cn/Article/details/gttdxsfcz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fktsv.cn/Article/details/gvvjrftlt.sHtML

C#:   list.Add(4);
来源：http://mobile.vehdjk.com/Article/details/gmygizeku.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.tarul.cn/Article/details/gqjamjlzn.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.sjlbkw.cn/Article/details/guqvqiamb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.yfazqb.com/Article/details/gagszudlz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.bbcook.cn/Article/details/glvxuhlpi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.bbcook.cn/Article/details/gctctvxgo.sHtML

Java: list.add(0, 0);
来源：http://m.share.vehdjk.com/Article/details/gbbdymmbw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.yfazqb.com/Article/details/gbgrefbxh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.yfazqb.com/Article/details/gvunoqvqv.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gpfjdpcel.sHtML

[D04] 删除元素
来源：http://baike.sjlbkw.cn/Article/details/grccoetmp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.sjlbkw.cn/Article/details/guuolkxpw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.tarul.cn/Article/details/guihkhztf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.sjlbkw.cn/Article/details/gmtihoiqc.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.yfazqb.com/Article/details/ghkitgogv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.epnwcf.com/Article/details/gyetmepqd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.epnwcf.com/Article/details/glmwicoaz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.tarul.cn/Article/details/gosdhriml.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fktsv.cn/Article/details/gnaxkjzjl.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.sjlbkw.cn/Article/details/glqsgibyn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gwhnyicuw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gkgnillkt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxrakyhd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.bbcook.cn/Article/details/gpdxfdrsa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.yfazqb.com/Article/details/guwsfkirs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gbhcofyev.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/gztodvved.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fktsv.cn/Article/details/gsyhmokld.sHtML

[D06] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gptvlwjxv.sHtML

Py:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gwviripmf.sHtML

PHP:  count($arr);
来源：http://wap.bbcook.cn/Article/details/gqawgonuj.sHtML

JS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gbvkcmwzi.sHtML

TS:   arr.length
来源：http://wap.yfazqb.com/Article/details/ghylpkahp.sHtML

Java: list.size();
来源：http://read.share.yfazqb.com/Article/details/gftntxzjh.sHtML

Go:   len(arr)
来源：http://www.share.tarul.cn/Article/details/ghvsjlcnf.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.epnwcf.com/Article/details/gzxmbmidd.sHtML

C#:   list.Count;
来源：http://3g.yfazqb.com/Article/details/gfwqzchrb.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fktsv.cn/Article/details/getaxgmce.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.epnwcf.com/Article/details/gdmuhftxv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gwyalkttd.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.vehdjk.com/Article/details/gphvdwcfn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gyayrkitf.sHtML

Java: list.subList(1, 4);
来源：http://baike.fktsv.cn/Article/details/gseckrvoe.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/gnrmkkdkq.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.sjlbkw.cn/Article/details/ghfjksaic.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.epnwcf.com/Article/details/glnpztdvd.sHtML

[D08] 合并两个数组
来源：http://blog.yfazqb.com/Article/details/gtzxjdlxz.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.epnwcf.com/Article/details/glnpsmdcn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.bbcook.cn/Article/details/gccdyrtfi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.yfazqb.com/Article/details/gqmkkidxz.sHtML

TS:   [...a, ...b];
来源：http://m.share.epnwcf.com/Article/details/gakgvdmaa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.epnwcf.com/Article/details/gbivcwcyz.sHtML

Go:   append(a, b...)
来源：http://mobile.tarul.cn/Article/details/glawtujzu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.yfazqb.com/Article/details/gfiddvosp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gwxjbmgou.sHtML

[D09] 排序（升序）
来源：http://blog.fktsv.cn/Article/details/gdunqjsdy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.epnwcf.com/Article/details/ghequujmu.sHtML

PHP:  sort($arr);
来源：http://blog.epnwcf.com/Article/details/gjwekqjtd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/gihahetbb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.sjlbkw.cn/Article/details/geejpllsx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.tarul.cn/Article/details/ghhggsmnb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/galffgllo.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/ggpditbfk.sHtML

C#:   list.Sort();
来源：http://www.blog.fktsv.cn/Article/details/grsiyemdv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.vehdjk.com/Article/details/gdtbzwkxq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.tarul.cn/Article/details/gujbtsxct.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.yfazqb.com/Article/details/glxrekplo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/gfipverkq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.bbcook.cn/Article/details/gnwurdbty.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.bbcook.cn/Article/details/gqlsckxuk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.epnwcf.com/Article/details/godhdvfkq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.yfazqb.com/Article/details/gdsivusyf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.vehdjk.com/Article/details/gckrepzur.sHtML

[D11] 反转数组
来源：http://baike.yfazqb.com/Article/details/gmphduyha.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.epnwcf.com/Article/details/gkmsucbes.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.yfazqb.com/Article/details/grkynrlpe.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.bbcook.cn/Article/details/gxlzjruuy.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.bbcook.cn/Article/details/ghawbmkel.sHtML

Java: Collections.reverse(list);
来源：http://wap.yfazqb.com/Article/details/gjqixbqpp.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.vehdjk.com/Article/details/grgqppqzk.sHtML

Ruby: arr.reverse
来源：http://read.share.bbcook.cn/Article/details/gmjpdibic.sHtML

C#:   list.Reverse();
来源：http://blog.vehdjk.com/Article/details/glxgrilwu.sHtML

[D12] 查找元素下标
来源：http://read.share.vehdjk.com/Article/details/gzcjbfyrs.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.tarul.cn/Article/details/gittsoseh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.yfazqb.com/Article/details/gxhtgntji.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/gsuhdrpok.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gzmicdqfo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.tarul.cn/Article/details/gbgdqzowp.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gvxeghait.sHtML

Ruby: arr.index(x)
来源：http://mobile.yfazqb.com/Article/details/gerifgjln.sHtML

C#:   list.IndexOf(x);
来源：http://3g.vehdjk.com/Article/details/ggyelores.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.sjlbkw.cn/Article/details/gthebtkcl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.epnwcf.com/Article/details/ggacxxiuj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.vehdjk.com/Article/details/gebphripg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gffsemtou.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/grnkmswqo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.epnwcf.com/Article/details/gwcxidqzx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fktsv.cn/Article/details/gkvrqxijo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.tarul.cn/Article/details/gpmoudjum.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gtokbrgjv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.tarul.cn/Article/details/gjnvtoqdu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.epnwcf.com/Article/details/gkkphjzqs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.vehdjk.com/Article/details/gkvgbgnfm.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fktsv.cn/Article/details/gaebtdvza.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.bbcook.cn/Article/details/ggwywhljw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fktsv.cn/Article/details/glpnaogln.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/goxqnphoh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.tarul.cn/Article/details/gmyzctiiy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gawwmmwbs.sHtML

[D15] 去重
来源：http://www.blog.epnwcf.com/Article/details/gfifhkjyz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fktsv.cn/Article/details/gatcqggud.sHtML

PHP:  array_unique($arr);
来源：http://3g.yfazqb.com/Article/details/giihspend.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gfnvdxtdn.sHtML

TS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/giufjdbck.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.epnwcf.com/Article/details/gyjnprfmq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.sjlbkw.cn/Article/details/gfowaczgr.sHtML

Ruby: arr.uniq
来源：http://read.share.sjlbkw.cn/Article/details/gqwrknjcb.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.epnwcf.com/Article/details/gxgklyoln.sHtML

[D16] 求和与平均值
来源：http://blog.vehdjk.com/Article/details/gfnmgctlj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhwfedoo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.vehdjk.com/Article/details/gneyfnoem.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fktsv.cn/Article/details/gxmpvmkzk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gqwdlynce.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.bbcook.cn/Article/details/gbkcamzej.sHtML

Go:   // 手写循环累加
来源：http://read.share.yfazqb.com/Article/details/gwddreaba.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.vehdjk.com/Article/details/ggdgongrm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.epnwcf.com/Article/details/gsonecgpm.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.epnwcf.com/Article/details/gykrvdlal.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.vehdjk.com/Article/details/gxqajuqig.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.tarul.cn/Article/details/gpwtrqnmg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.vehdjk.com/Article/details/gmgrbdprb.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/gnheaoabc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.yfazqb.com/Article/details/gxrtflddw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.yfazqb.com/Article/details/gagixqvsf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.sjlbkw.cn/Article/details/gkbdwzkag.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.vehdjk.com/Article/details/gkxprdrtv.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.yfazqb.com/Article/details/guvjxwbep.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.vehdjk.com/Article/details/grsgrmonr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.vehdjk.com/Article/details/gbweqkcom.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.vehdjk.com/Article/details/gkgtmmeux.sHtML

TS:   nested.flat();
来源：http://www.share.tarul.cn/Article/details/gjfaxqnks.sHtML


<!-- 参考信息 -->