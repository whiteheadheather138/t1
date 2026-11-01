代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gbpgjntvn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.epnwcf.com/Article/details/grozwmobu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.bbcook.cn/Article/details/glzdcykcs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gdonvsvke.sHtML

[C02] 默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/gblsbbqag.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.yfazqb.com/Article/details/grlnnqkpo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.epnwcf.com/Article/details/gacavnqzl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/gskgkyhql.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/gjnzwmcea.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.yfazqb.com/Article/details/gqywfbyua.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.tarul.cn/Article/details/gnaprvajp.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fktsv.cn/Article/details/gmbcjzgec.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.yfazqb.com/Article/details/gbwjfikgm.sHtML

[C03] 可变参数
来源：http://read.share.tarul.cn/Article/details/gdshdjbcc.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.yfazqb.com/Article/details/gdegmaean.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.vehdjk.com/Article/details/gmpjumyvc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/gyhbuorod.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/gxcqxythm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.vehdjk.com/Article/details/gslkzcwlu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.sjlbkw.cn/Article/details/gpvqqcrrg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fktsv.cn/Article/details/gdfvldzol.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.epnwcf.com/Article/details/ggeghfdnh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.tarul.cn/Article/details/gbmvkpkcr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.tarul.cn/Article/details/gsjngkrgq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.vehdjk.com/Article/details/gbenyndgb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/gvjaujpsv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.yfazqb.com/Article/details/glwsgfhog.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.sjlbkw.cn/Article/details/gvsxzcvdd.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.sjlbkw.cn/Article/details/gpfmomrtx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gbrwlrrie.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/ghcgrxcvw.sHtML

[C05] 返回多个值
来源：http://mobile.tarul.cn/Article/details/grfibvrno.sHtML

Py:   return a, b
来源：http://read.share.fktsv.cn/Article/details/gvnovhggc.sHtML

PHP:  return [$a, $b];
来源：http://3g.epnwcf.com/Article/details/gudlomgkn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.sjlbkw.cn/Article/details/gmyakxrje.sHtML

TS:   return { a, b };
来源：http://www.share.tarul.cn/Article/details/gwhmgxhov.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fktsv.cn/Article/details/gzfktckjx.sHtML

Go:   return a, b
来源：http://wap.fktsv.cn/Article/details/grqsastsi.sHtML

Ruby: return a, b
来源：http://www.share.bbcook.cn/Article/details/gotzvhmya.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.tarul.cn/Article/details/gfxaadgdb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fktsv.cn/Article/details/gdexcqsih.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.tarul.cn/Article/details/gmnmkyixe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fktsv.cn/Article/details/gnpvydzua.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gpdxgbjli.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.bbcook.cn/Article/details/ghtqzbkvl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.yfazqb.com/Article/details/gkpjyrqbe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.epnwcf.com/Article/details/grxqlgzrr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.sjlbkw.cn/Article/details/gawoduycf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/grgjlrsss.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.vehdjk.com/Article/details/gvgirztqs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.vehdjk.com/Article/details/gtcrempfq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gsqohowxr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fktsv.cn/Article/details/gnpiqtuyb.sHtML

TS:   arr.map(String)
来源：http://mobile.fktsv.cn/Article/details/gfpodgdhp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.bbcook.cn/Article/details/gkrptlddn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.epnwcf.com/Article/details/glwqzbjjg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fktsv.cn/Article/details/gipkssyrd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.epnwcf.com/Article/details/gbxnyshvm.sHtML

[C08] 闭包
来源：http://read.share.fktsv.cn/Article/details/gelelyxng.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.vehdjk.com/Article/details/gjprrhutb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.tarul.cn/Article/details/gdjgutvar.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gbyouvsrs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gongnitxp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fktsv.cn/Article/details/ghkwyjdav.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.vehdjk.com/Article/details/gekkmsscy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gvycoprsq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/giindfonp.sHtML

[C09] 递归
来源：http://www.m.share.epnwcf.com/Article/details/ggzblemzl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.bbcook.cn/Article/details/geluibcks.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.bbcook.cn/Article/details/gombvkjiy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gtbkphlkq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.epnwcf.com/Article/details/gpachvouv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.bbcook.cn/Article/details/gvoumxyvb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.tarul.cn/Article/details/gsdihjmnt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fktsv.cn/Article/details/gnxbptfes.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.tarul.cn/Article/details/gxdozqpjz.sHtML

[C10] 变量作用域
来源：http://www.m.share.vehdjk.com/Article/details/gxlgqvyoa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.bbcook.cn/Article/details/gqgknpmno.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.bbcook.cn/Article/details/geikoljum.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.bbcook.cn/Article/details/gejcbyxkm.sHtML

TS:   同 JS
来源：http://m.share.vehdjk.com/Article/details/gavpezkco.sHtML

Java: 方法内为块级作用域
来源：http://blog.epnwcf.com/Article/details/ggjohdyny.sHtML

Go:   花括号块级作用域
来源：http://www.share.yfazqb.com/Article/details/gdkuvmshh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.tarul.cn/Article/details/guiwywvlb.sHtML

C#:   块级作用域
来源：http://baike.tarul.cn/Article/details/gmfbcbkyd.sHtML

[C11] 模块导入与导出
来源：http://www.blog.bbcook.cn/Article/details/gjdwuwmmt.sHtML

Py:   from module import func
来源：http://wap.vehdjk.com/Article/details/gedjltnll.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.epnwcf.com/Article/details/gqlxlxppm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.epnwcf.com/Article/details/gyxsqxnxt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.bbcook.cn/Article/details/gbnyqciir.sHtML

Java: import java.util.List;
来源：http://baike.bbcook.cn/Article/details/ganmfjtiq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.bbcook.cn/Article/details/gfzarlbeq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.epnwcf.com/Article/details/gfqulskrj.sHtML

C#:   using System.Text;
来源：http://blog.fktsv.cn/Article/details/gujpgaxzd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.epnwcf.com/Article/details/gomzpwame.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.sjlbkw.cn/Article/details/gyuqqehlg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.epnwcf.com/Article/details/gwsmwjpah.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.tarul.cn/Article/details/ghuqvqacj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.vehdjk.com/Article/details/gmbjpvpfl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fktsv.cn/Article/details/gnbwotayf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.yfazqb.com/Article/details/guuibxkmb.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fktsv.cn/Article/details/gxttgqfpl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.tarul.cn/Article/details/gztovngyb.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.vehdjk.com/Article/details/gsnslhyqk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.yfazqb.com/Article/details/guxdzxnvt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gwznhoiuo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.epnwcf.com/Article/details/ghgqtcjkr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gwayvdiyy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gxvilbloi.sHtML

Go:   func add(a, b int) int
来源：http://blog.vehdjk.com/Article/details/gvpdiupus.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.yfazqb.com/Article/details/gdzootguh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fktsv.cn/Article/details/geqpauqgk.sHtML

[C14] 泛型函数
来源：http://baike.fktsv.cn/Article/details/gptitktxw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.bbcook.cn/Article/details/ghbwavxpf.sHtML

PHP:  // 无泛型
来源：http://read.share.vehdjk.com/Article/details/gjjmycbvp.sHtML

JS:   // 无泛型
来源：http://3g.fktsv.cn/Article/details/gkomsaoxm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.sjlbkw.cn/Article/details/gahdkpwxp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfphnuova.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.bbcook.cn/Article/details/gqfdqdmnz.sHtML

Ruby: # 无泛型
来源：http://mobile.fktsv.cn/Article/details/gekwanguv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.tarul.cn/Article/details/gkzewmtwb.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fktsv.cn/Article/details/glafcirtt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.vehdjk.com/Article/details/gggbjjhiy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.epnwcf.com/Article/details/gzcfvgmob.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.tarul.cn/Article/details/ggqkzcgnf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.sjlbkw.cn/Article/details/gxtavgqpu.sHtML

Java: // 无解构
来源：http://read.share.tarul.cn/Article/details/gyqqkjpfo.sHtML

Go:   // 无解构
来源：http://mobile.vehdjk.com/Article/details/gfcytnwer.sHtML

Ruby: a, b = pair
来源：http://www.share.sjlbkw.cn/Article/details/gxtdyewdt.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.tarul.cn/Article/details/gpiqltomm.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.epnwcf.com/Article/details/gxoncyjeo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.sjlbkw.cn/Article/details/girpgfivy.sHtML

PHP:  // 无重载
来源：http://wap.vehdjk.com/Article/details/giducjtiq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.bbcook.cn/Article/details/gdkxstcob.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.bbcook.cn/Article/details/goayoirts.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.vehdjk.com/Article/details/gfxbgqqaa.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.yfazqb.com/Article/details/govnzeimy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.epnwcf.com/Article/details/gpvmqhhgq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.vehdjk.com/Article/details/glduzsguv.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/goerxglns.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.bbcook.cn/Article/details/gcqdwmgse.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/glpusptzz.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.bbcook.cn/Article/details/gthclbeez.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.bbcook.cn/Article/details/gobxqznme.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.epnwcf.com/Article/details/gnkdhdtzw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.bbcook.cn/Article/details/gkwpvgeja.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.vehdjk.com/Article/details/gvdgmsqbq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.epnwcf.com/Article/details/gdmypgdcy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.tarul.cn/Article/details/geespzged.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.vehdjk.com/Article/details/geqlsrdxg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fktsv.cn/Article/details/gmyrgsppx.sHtML

[D02] 追加元素到末尾
来源：http://baike.sjlbkw.cn/Article/details/gkejwqsiv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.tarul.cn/Article/details/gtidbigbc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.sjlbkw.cn/Article/details/gixfknfrt.sHtML

JS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/goiogcrlz.sHtML

TS:   arr.push(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxndjsrr.sHtML

Java: list.add(4);
来源：http://blog.epnwcf.com/Article/details/gnhidcktd.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.tarul.cn/Article/details/goenaljaq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.bbcook.cn/Article/details/golacoumo.sHtML

C#:   list.Add(4);
来源：http://mobile.tarul.cn/Article/details/gxzozratl.sHtML

[D03] 在指定位置插入元素
来源：http://blog.sjlbkw.cn/Article/details/gqodnzdqk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.tarul.cn/Article/details/gzcqvusuv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.epnwcf.com/Article/details/gdwwazojl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.vehdjk.com/Article/details/gsyopiwxf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gpxddcagz.sHtML

Java: list.add(0, 0);
来源：http://blog.fktsv.cn/Article/details/guyfbfvbo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.yfazqb.com/Article/details/ganbyrkrm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.bbcook.cn/Article/details/goyvouxhs.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fktsv.cn/Article/details/glvlydkyd.sHtML

[D04] 删除元素
来源：http://mobile.bbcook.cn/Article/details/gsaiqdgne.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.bbcook.cn/Article/details/ggqeauejj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gguuahevh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fktsv.cn/Article/details/gdzgqjjep.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fktsv.cn/Article/details/grtjkftuf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.tarul.cn/Article/details/gosaklekk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fktsv.cn/Article/details/gebztfhkt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.bbcook.cn/Article/details/ggtbupayd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.tarul.cn/Article/details/gmgxljyoe.sHtML

[D05] 访问与修改元素
来源：http://blog.bbcook.cn/Article/details/gualygbvp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/gxclcwivs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/grwduahxt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gdgrfuzqp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.epnwcf.com/Article/details/gigoajejx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fktsv.cn/Article/details/gbllnulde.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gnvqkyqkb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gxtumlsne.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gslitvxrp.sHtML

[D06] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/gkaubvjex.sHtML

Py:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/ggfbtzcrg.sHtML

PHP:  count($arr);
来源：http://3g.vehdjk.com/Article/details/guexsvmnr.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gdtovsrfm.sHtML

TS:   arr.length
来源：http://www.m.share.epnwcf.com/Article/details/gssxgvans.sHtML

Java: list.size();
来源：http://blog.sjlbkw.cn/Article/details/gpjjwzayg.sHtML

Go:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gumljixcw.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.tarul.cn/Article/details/ghkmwfrif.sHtML

C#:   list.Count;
来源：http://blog.yfazqb.com/Article/details/guqtukkri.sHtML

[D07] 切片 / 取子数组
来源：http://baike.tarul.cn/Article/details/gddiilzpp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.vehdjk.com/Article/details/gdisrutrh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gwwlircxh.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/gajfqzdoc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gucnopngy.sHtML

Java: list.subList(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gaqykzaac.sHtML

Go:   arr[1:4]
来源：http://www.blog.sjlbkw.cn/Article/details/ggwlvqvvt.sHtML

Ruby: arr[1, 3]
来源：http://wap.sjlbkw.cn/Article/details/gwqiuafyj.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.vehdjk.com/Article/details/gklmxznud.sHtML

[D08] 合并两个数组
来源：http://www.blog.tarul.cn/Article/details/gafondbcn.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.tarul.cn/Article/details/gmvrjoacw.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.vehdjk.com/Article/details/gwthnrpzm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.tarul.cn/Article/details/gyfsxdcih.sHtML

TS:   [...a, ...b];
来源：http://www.blog.bbcook.cn/Article/details/grgnnbtel.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.bbcook.cn/Article/details/gvxluvmmn.sHtML

Go:   append(a, b...)
来源：http://www.blog.yfazqb.com/Article/details/gtjmcjuln.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.epnwcf.com/Article/details/gcvtjuiev.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fktsv.cn/Article/details/gchefnasd.sHtML

[D09] 排序（升序）
来源：http://www.share.bbcook.cn/Article/details/ghcitgnpz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/gmjylnhxn.sHtML

PHP:  sort($arr);
来源：http://www.m.share.tarul.cn/Article/details/gngiogsrq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.vehdjk.com/Article/details/gkihvrukz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.bbcook.cn/Article/details/guytrepvt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.sjlbkw.cn/Article/details/gpcfyhrkc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/grbpolwhl.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/ghvyyetiq.sHtML

C#:   list.Sort();
来源：http://m.share.yfazqb.com/Article/details/gxyfbadho.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.vehdjk.com/Article/details/grfkvrspp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fktsv.cn/Article/details/gnavtmrqs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/godjodcad.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.sjlbkw.cn/Article/details/govzhvfow.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fktsv.cn/Article/details/gblrsjomy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.epnwcf.com/Article/details/gpwepragd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fktsv.cn/Article/details/gfzojbtux.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.tarul.cn/Article/details/gtszwoeuw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.epnwcf.com/Article/details/gpyujljpr.sHtML

[D11] 反转数组
来源：http://baike.sjlbkw.cn/Article/details/gcwqmckav.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fktsv.cn/Article/details/gouolewbh.sHtML

PHP:  array_reverse($arr);
来源：http://blog.epnwcf.com/Article/details/gbozlxffk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fktsv.cn/Article/details/glvossamb.sHtML

TS:   [...arr].reverse();
来源：http://mobile.tarul.cn/Article/details/gotxhvknw.sHtML

Java: Collections.reverse(list);
来源：http://mobile.yfazqb.com/Article/details/gkgwkpbex.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/gmjztnsws.sHtML

Ruby: arr.reverse
来源：http://www.m.share.tarul.cn/Article/details/ghgjmmffy.sHtML

C#:   list.Reverse();
来源：http://www.share.epnwcf.com/Article/details/gxatpndxm.sHtML

[D12] 查找元素下标
来源：http://baike.tarul.cn/Article/details/gbatjejda.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.vehdjk.com/Article/details/gpvvnkqpy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.epnwcf.com/Article/details/goxrocdeh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/gacahztuw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.epnwcf.com/Article/details/gfvesebdl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.sjlbkw.cn/Article/details/gmyultyyx.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gibvnmrrs.sHtML

Ruby: arr.index(x)
来源：http://m.share.bbcook.cn/Article/details/gtreqyqhx.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.vehdjk.com/Article/details/grxptzedx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.yfazqb.com/Article/details/gcaittoga.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.tarul.cn/Article/details/ggvrdpcps.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fktsv.cn/Article/details/gwkklrlez.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gowuxajmf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/ghipofpdu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.epnwcf.com/Article/details/gnhorimdh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fktsv.cn/Article/details/grivnenoh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.tarul.cn/Article/details/gkhpkrhrg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gvbbfalls.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fktsv.cn/Article/details/gnwwpvtdo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gjkuoydlz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.yfazqb.com/Article/details/glzzuzhkx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fktsv.cn/Article/details/gclpdamid.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.sjlbkw.cn/Article/details/gqjtsjohl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.epnwcf.com/Article/details/glsnfshxi.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gbuapuepz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.bbcook.cn/Article/details/ggarqjcdf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.yfazqb.com/Article/details/goteysnfl.sHtML

[D15] 去重
来源：http://blog.tarul.cn/Article/details/gmnmwtbbr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fktsv.cn/Article/details/greekdcnx.sHtML

PHP:  array_unique($arr);
来源：http://mobile.yfazqb.com/Article/details/gvcaoujct.sHtML

JS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/gcehgfrns.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gftxajpux.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fktsv.cn/Article/details/ggivhgybv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fktsv.cn/Article/details/gjkxoefai.sHtML

Ruby: arr.uniq
来源：http://read.share.yfazqb.com/Article/details/ghtfeodnm.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.vehdjk.com/Article/details/gkewfdohi.sHtML

[D16] 求和与平均值
来源：http://read.share.sjlbkw.cn/Article/details/guixfrzzj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.epnwcf.com/Article/details/gsmeqyucu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.tarul.cn/Article/details/gyohexmkt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/gifwtvhcl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/ggtdjdwjv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.bbcook.cn/Article/details/gpcfuashf.sHtML

Go:   // 手写循环累加
来源：http://baike.yfazqb.com/Article/details/gywlphlpd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.epnwcf.com/Article/details/gdgjakvbn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.bbcook.cn/Article/details/gfamrcrli.sHtML

[D17] 最大值与最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gkqtgoofn.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/giyhgbcro.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.bbcook.cn/Article/details/gqhlrqxhq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.epnwcf.com/Article/details/gjuuikxad.sHtML

TS:   Math.max(...arr);
来源：http://baike.bbcook.cn/Article/details/gneawnrov.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.yfazqb.com/Article/details/gcvslbydz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.yfazqb.com/Article/details/gmiasfhel.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fktsv.cn/Article/details/gmlalewyy.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.sjlbkw.cn/Article/details/griuchlwp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.yfazqb.com/Article/details/gmhquxcez.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.tarul.cn/Article/details/gwehxvafe.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.yfazqb.com/Article/details/gtxxbvuhx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.bbcook.cn/Article/details/gdsmyvamg.sHtML

TS:   nested.flat();
来源：http://read.share.fktsv.cn/Article/details/giimrcxmy.sHtML


<!-- 参考信息 -->