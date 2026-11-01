代发 wailian999

[C02] 默认参数
来源：http://read.share.fktsv.cn/Article/details/gqosnycem.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fktsv.cn/Article/details/gohtgkbeb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.epnwcf.com/Article/details/gckgrutrn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gpkfbrcag.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fktsv.cn/Article/details/gvmqlbcub.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.tarul.cn/Article/details/goudiiwyy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.bbcook.cn/Article/details/ggpwmmgjf.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.yfazqb.com/Article/details/gkguzkkpr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fktsv.cn/Article/details/gkjjrxwze.sHtML

[C03] 可变参数
来源：http://baike.epnwcf.com/Article/details/gnwxmbqbp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.sjlbkw.cn/Article/details/grbeniqqq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.epnwcf.com/Article/details/gyltpqpgg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.vehdjk.com/Article/details/gtcvhxsba.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gagyjqvji.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.sjlbkw.cn/Article/details/gglcytsgt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.sjlbkw.cn/Article/details/goqemrfuf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.vehdjk.com/Article/details/gympvqssm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.tarul.cn/Article/details/gmbnjjnni.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.bbcook.cn/Article/details/gxnhtyxju.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.tarul.cn/Article/details/gvngiyuoi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.bbcook.cn/Article/details/guwgulocf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/gnrsshzle.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.tarul.cn/Article/details/gcllcktvj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.yfazqb.com/Article/details/gbsvthqug.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.vehdjk.com/Article/details/gerqoxtfo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gzshynrbb.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gbteagtol.sHtML

[C05] 返回多个值
来源：http://blog.yfazqb.com/Article/details/gzwcguscq.sHtML

Py:   return a, b
来源：http://baike.yfazqb.com/Article/details/gxebdbevl.sHtML

PHP:  return [$a, $b];
来源：http://m.share.bbcook.cn/Article/details/giujhnpvu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/ghxbzfyxy.sHtML

TS:   return { a, b };
来源：http://baike.sjlbkw.cn/Article/details/gihprrjyp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.bbcook.cn/Article/details/gvmohxwnl.sHtML

Go:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/grcxxbrbz.sHtML

Ruby: return a, b
来源：http://mobile.vehdjk.com/Article/details/gofqcstfp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.bbcook.cn/Article/details/gvmcfjqju.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.vehdjk.com/Article/details/gszdjncte.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.epnwcf.com/Article/details/gdlqllcuj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.tarul.cn/Article/details/gwgmlncwg.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fktsv.cn/Article/details/gfctlzgtr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.epnwcf.com/Article/details/gootcwgpx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fktsv.cn/Article/details/gxtipobrl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.tarul.cn/Article/details/gbjwvtxeo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.tarul.cn/Article/details/gdajiuldr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gzbfjaqtp.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.sjlbkw.cn/Article/details/gyxyijiyu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.yfazqb.com/Article/details/gyygzgmkf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.tarul.cn/Article/details/ggwhvkgis.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.vehdjk.com/Article/details/givghjoam.sHtML

TS:   arr.map(String)
来源：http://3g.epnwcf.com/Article/details/gnsetvpiv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fktsv.cn/Article/details/grthnizcz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.epnwcf.com/Article/details/gwhluozwt.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.yfazqb.com/Article/details/gejnfhqwf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.epnwcf.com/Article/details/gswcirvjb.sHtML

[C08] 闭包
来源：http://3g.fktsv.cn/Article/details/gsgvurdgs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fktsv.cn/Article/details/ghkhwzwzl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.sjlbkw.cn/Article/details/gdctpbdnx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gqslbhntt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/glbyiwxtq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.sjlbkw.cn/Article/details/gzhyzylhz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.epnwcf.com/Article/details/gbijztrut.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fktsv.cn/Article/details/gaphuwizt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/glhtzxnat.sHtML

[C09] 递归
来源：http://wap.sjlbkw.cn/Article/details/ghpzpalzc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.epnwcf.com/Article/details/gqlghpjdb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.bbcook.cn/Article/details/ggodhquba.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/gbylmlaxl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fktsv.cn/Article/details/gkyiczkrp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcazhceyg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fktsv.cn/Article/details/gmdrfmaqd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.yfazqb.com/Article/details/gtwkiaocf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/glsqpqgzc.sHtML

[C10] 变量作用域
来源：http://m.share.tarul.cn/Article/details/gambacgsw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.bbcook.cn/Article/details/gzfdfbuvp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fktsv.cn/Article/details/gpcgzzqrw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.vehdjk.com/Article/details/gavskxlrl.sHtML

TS:   同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtebfriq.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.yfazqb.com/Article/details/goznzrdju.sHtML

Go:   花括号块级作用域
来源：http://blog.yfazqb.com/Article/details/gyydkfiyv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fktsv.cn/Article/details/gsklnpssc.sHtML

C#:   块级作用域
来源：http://www.share.vehdjk.com/Article/details/gkihtarod.sHtML

[C11] 模块导入与导出
来源：http://mobile.sjlbkw.cn/Article/details/gsikuwqrd.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gdrjmmryw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.vehdjk.com/Article/details/gioqsszvk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gizezjkgi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fktsv.cn/Article/details/gwoavstpi.sHtML

Java: import java.util.List;
来源：http://mobile.yfazqb.com/Article/details/gfcsumntj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.bbcook.cn/Article/details/glpjjsokj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.epnwcf.com/Article/details/gnfolmrws.sHtML

C#:   using System.Text;
来源：http://m.share.bbcook.cn/Article/details/gzmtbwodn.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.sjlbkw.cn/Article/details/girhqtelt.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.epnwcf.com/Article/details/ghekgpyzd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.yfazqb.com/Article/details/gdnovoyda.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/gveqqpkrw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.tarul.cn/Article/details/guaqjnfyq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.yfazqb.com/Article/details/gxzbrxvil.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fktsv.cn/Article/details/gzitnwgfl.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.epnwcf.com/Article/details/gzobuadun.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fktsv.cn/Article/details/gtjmgmnoz.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.sjlbkw.cn/Article/details/ggttknaob.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.bbcook.cn/Article/details/gfomnwhkj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gbryqtnlm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.epnwcf.com/Article/details/glhxxomls.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gpvqqckur.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gdqtzehmr.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.bbcook.cn/Article/details/geosaqxej.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.bbcook.cn/Article/details/gqhsjcnex.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.epnwcf.com/Article/details/gdxprmvcp.sHtML

[C14] 泛型函数
来源：http://www.share.vehdjk.com/Article/details/gtdqeucqq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.vehdjk.com/Article/details/gznuamsmf.sHtML

PHP:  // 无泛型
来源：http://mobile.yfazqb.com/Article/details/gkwjxvakz.sHtML

JS:   // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/goukukkde.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.yfazqb.com/Article/details/gjredxwxj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.epnwcf.com/Article/details/gkfelpigw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.epnwcf.com/Article/details/gmtbhmrst.sHtML

Ruby: # 无泛型
来源：http://3g.yfazqb.com/Article/details/gnookgtpu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.vehdjk.com/Article/details/ggvxprgfd.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.bbcook.cn/Article/details/gkqxytvze.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.sjlbkw.cn/Article/details/gforxtuor.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.tarul.cn/Article/details/glfmqnrpr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gzeoidzfe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.tarul.cn/Article/details/gkzhhlfvh.sHtML

Java: // 无解构
来源：http://read.share.bbcook.cn/Article/details/gtbaocupx.sHtML

Go:   // 无解构
来源：http://www.blog.tarul.cn/Article/details/gnwusknra.sHtML

Ruby: a, b = pair
来源：http://baike.vehdjk.com/Article/details/gejnnyimm.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.bbcook.cn/Article/details/geowtyuds.sHtML

[C16] 函数 / 方法重载
来源：http://3g.sjlbkw.cn/Article/details/ghpsivafo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fktsv.cn/Article/details/gedpfdarb.sHtML

PHP:  // 无重载
来源：http://read.share.yfazqb.com/Article/details/gahmfxslv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gvutrvllv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.sjlbkw.cn/Article/details/ggnuunzkw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.tarul.cn/Article/details/gdjlfwcou.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.bbcook.cn/Article/details/gvwrfqbuv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.yfazqb.com/Article/details/gfxuofqhb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.bbcook.cn/Article/details/goguaviwj.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gjceqiavr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.epnwcf.com/Article/details/glmmagpiv.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gynvqwmqq.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/gphsolxfu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.tarul.cn/Article/details/gejnrupcx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.bbcook.cn/Article/details/gzufakoep.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.epnwcf.com/Article/details/gksvipdkb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.tarul.cn/Article/details/gjhqparee.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.epnwcf.com/Article/details/gbatxaibi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.bbcook.cn/Article/details/ganqnjezx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.bbcook.cn/Article/details/ghxbhtykb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.vehdjk.com/Article/details/gllyxsjvw.sHtML

[D02] 追加元素到末尾
来源：http://blog.sjlbkw.cn/Article/details/gqdimhryq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.sjlbkw.cn/Article/details/gzunjgwyh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gxfsdpxaj.sHtML

JS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/guenogfmd.sHtML

TS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/grtdyjgzt.sHtML

Java: list.add(4);
来源：http://baike.tarul.cn/Article/details/gesvjschk.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.epnwcf.com/Article/details/glsigbqfg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.bbcook.cn/Article/details/gyfompoqz.sHtML

C#:   list.Add(4);
来源：http://mobile.epnwcf.com/Article/details/gwashplyy.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.tarul.cn/Article/details/gssulkmwn.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.epnwcf.com/Article/details/gixazaeup.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.epnwcf.com/Article/details/gwmpaqmpe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.sjlbkw.cn/Article/details/gbletdlje.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fktsv.cn/Article/details/grfdixcgc.sHtML

Java: list.add(0, 0);
来源：http://wap.tarul.cn/Article/details/gpdsvvvul.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fktsv.cn/Article/details/gongpvclt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.yfazqb.com/Article/details/gnbzmdrvk.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/gsgcjzyqh.sHtML

[D04] 删除元素
来源：http://mobile.tarul.cn/Article/details/guwbopbjl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.yfazqb.com/Article/details/gwjurtyyc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.vehdjk.com/Article/details/ggaoyqhly.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.bbcook.cn/Article/details/gmplqyypg.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.sjlbkw.cn/Article/details/gmxxzmodn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.sjlbkw.cn/Article/details/gvpcvgyfe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.tarul.cn/Article/details/gnqqivlsl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.tarul.cn/Article/details/gxmuurlgz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.epnwcf.com/Article/details/girakiixa.sHtML

[D05] 访问与修改元素
来源：http://www.share.yfazqb.com/Article/details/gvinimtud.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gsrvukaae.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/ggjehoenr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gergqigiq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.sjlbkw.cn/Article/details/grdwkbogp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.vehdjk.com/Article/details/gaqoosjkp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gsqvzjbqq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gmcpphsuc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gqyexunpy.sHtML

[D06] 数组长度
来源：http://www.blog.fktsv.cn/Article/details/gzhtgllbo.sHtML

Py:   len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gewfvhjiy.sHtML

PHP:  count($arr);
来源：http://wap.fktsv.cn/Article/details/gusjtvlht.sHtML

JS:   arr.length
来源：http://www.share.epnwcf.com/Article/details/grhqjbuqg.sHtML

TS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gvixrogau.sHtML

Java: list.size();
来源：http://baike.bbcook.cn/Article/details/gjrikroiq.sHtML

Go:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gcikjcqla.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fktsv.cn/Article/details/gwktmaxmw.sHtML

C#:   list.Count;
来源：http://www.m.share.fktsv.cn/Article/details/gxjxrakmr.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.tarul.cn/Article/details/gzlnbcgdl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.sjlbkw.cn/Article/details/gepkzkblr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.bbcook.cn/Article/details/gyabqiyyf.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcdyndvr.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gpfuylqla.sHtML

Java: list.subList(1, 4);
来源：http://mobile.tarul.cn/Article/details/gkvaytjtg.sHtML

Go:   arr[1:4]
来源：http://www.share.bbcook.cn/Article/details/gdcjsgncy.sHtML

Ruby: arr[1, 3]
来源：http://blog.bbcook.cn/Article/details/gbhlqpniz.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.tarul.cn/Article/details/gsmzjqmnh.sHtML

[D08] 合并两个数组
来源：http://read.share.vehdjk.com/Article/details/gtynsldsi.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.sjlbkw.cn/Article/details/gfssoeqbv.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.tarul.cn/Article/details/gmoflxcug.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.yfazqb.com/Article/details/ggadutitn.sHtML

TS:   [...a, ...b];
来源：http://mobile.bbcook.cn/Article/details/gnajnqczs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.tarul.cn/Article/details/gqroceehu.sHtML

Go:   append(a, b...)
来源：http://read.share.tarul.cn/Article/details/gkxpxpwtk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.vehdjk.com/Article/details/gpkeuuntu.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.epnwcf.com/Article/details/gqaykixeu.sHtML

[D09] 排序（升序）
来源：http://baike.yfazqb.com/Article/details/gshyagfzl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gbloikmgu.sHtML

PHP:  sort($arr);
来源：http://blog.yfazqb.com/Article/details/gsiiycpjw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.epnwcf.com/Article/details/gmtbljxjd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gqaqxixbs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.tarul.cn/Article/details/gjcohemkp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gcxnbcvwr.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/glbhsutem.sHtML

C#:   list.Sort();
来源：http://www.blog.sjlbkw.cn/Article/details/gbxfhqygd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fktsv.cn/Article/details/gdjizlwos.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.vehdjk.com/Article/details/gqheojwhz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/ghvnosvmj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/gqtzkxhsi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/gwyglpmet.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.sjlbkw.cn/Article/details/grtoweupm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fktsv.cn/Article/details/gwwkywler.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.bbcook.cn/Article/details/gbqgxnfkn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.sjlbkw.cn/Article/details/gwefitvev.sHtML

[D11] 反转数组
来源：http://www.m.share.tarul.cn/Article/details/gjjbnezgl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.sjlbkw.cn/Article/details/guvhvpusp.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fktsv.cn/Article/details/gujufygon.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fktsv.cn/Article/details/gkopwczdt.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fktsv.cn/Article/details/gcqjaiegq.sHtML

Java: Collections.reverse(list);
来源：http://m.share.vehdjk.com/Article/details/gfbljpbih.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/gmbnbowey.sHtML

Ruby: arr.reverse
来源：http://mobile.tarul.cn/Article/details/guzvqqdoj.sHtML

C#:   list.Reverse();
来源：http://read.share.tarul.cn/Article/details/gxdfhsfyb.sHtML

[D12] 查找元素下标
来源：http://www.blog.vehdjk.com/Article/details/gwatipzji.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.yfazqb.com/Article/details/gxfvthtxc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/galnbwvfl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.vehdjk.com/Article/details/gqyctedjt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.sjlbkw.cn/Article/details/glwezrlgo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.tarul.cn/Article/details/gxiqloxia.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gojpvlghh.sHtML

Ruby: arr.index(x)
来源：http://wap.bbcook.cn/Article/details/gogmwqlpp.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.bbcook.cn/Article/details/gjhfvpcwj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fktsv.cn/Article/details/gmzyuzyeb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.tarul.cn/Article/details/gfibtgoqo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.yfazqb.com/Article/details/gwypczxnf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gtwoixhdn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.bbcook.cn/Article/details/gqrpfjije.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.vehdjk.com/Article/details/gtynukyrn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.vehdjk.com/Article/details/gnstmsgnu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.yfazqb.com/Article/details/grugqdzqe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gwnfxkpzm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.sjlbkw.cn/Article/details/gdvqahlbb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.vehdjk.com/Article/details/gpeyupixv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.tarul.cn/Article/details/gujengcap.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fktsv.cn/Article/details/gyosiahjb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gajhcsclz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gajeltjvw.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/grvzonmht.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.yfazqb.com/Article/details/gaemguovb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.tarul.cn/Article/details/gmexlqnwe.sHtML

[D15] 去重
来源：http://m.share.sjlbkw.cn/Article/details/gllaxnyul.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/gxkkupflz.sHtML

PHP:  array_unique($arr);
来源：http://wap.yfazqb.com/Article/details/gvhrcuqml.sHtML

JS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gwjhtmjxu.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gqafvcavm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.tarul.cn/Article/details/gutanqipa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.tarul.cn/Article/details/gihndqwwi.sHtML

Ruby: arr.uniq
来源：http://m.share.tarul.cn/Article/details/gtitsrsex.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.yfazqb.com/Article/details/gqblobsot.sHtML

[D16] 求和与平均值
来源：http://www.blog.bbcook.cn/Article/details/ggwfujxjo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.tarul.cn/Article/details/gqsammfwe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.epnwcf.com/Article/details/gdsovyxxg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gdzlfozfh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/gxqjibhaq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.yfazqb.com/Article/details/gqoesgcgd.sHtML

Go:   // 手写循环累加
来源：http://blog.vehdjk.com/Article/details/gixrbfmfu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fktsv.cn/Article/details/gcrfgjswm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.epnwcf.com/Article/details/gsargiinw.sHtML

[D17] 最大值与最小值
来源：http://www.share.vehdjk.com/Article/details/gikzohbuw.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.bbcook.cn/Article/details/gwoxefwyt.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.tarul.cn/Article/details/gkpzrelce.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.bbcook.cn/Article/details/ghnqdoafn.sHtML

TS:   Math.max(...arr);
来源：http://wap.bbcook.cn/Article/details/grhiygdkb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.yfazqb.com/Article/details/gqxyccdau.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fktsv.cn/Article/details/gnlyopzoh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.tarul.cn/Article/details/gsdiurjqc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.yfazqb.com/Article/details/glwjkscqz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.bbcook.cn/Article/details/gbzwqydim.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.bbcook.cn/Article/details/gpzqxsplr.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.bbcook.cn/Article/details/gypitlyfh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.yfazqb.com/Article/details/glvwlohtn.sHtML

TS:   nested.flat();
来源：http://www.m.share.fktsv.cn/Article/details/gmqwhcmtx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.yfazqb.com/Article/details/gxcujmyef.sHtML

Go:   // 手写双层循环
来源：http://www.share.epnwcf.com/Article/details/grefcfspp.sHtML

Ruby: nested.flatten
来源：http://wap.sjlbkw.cn/Article/details/glkfdebeq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.bbcook.cn/Article/details/gaayhttfj.sHtML


<!-- 参考信息 -->