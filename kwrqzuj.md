代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/gbeohuaaq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.yfazqb.com/Article/details/gtdzwmmta.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.sjlbkw.cn/Article/details/gzphixbyi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.tarul.cn/Article/details/gzygqqtgd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.yfazqb.com/Article/details/gviwpalxl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.yfazqb.com/Article/details/ghxhgvoyz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fktsv.cn/Article/details/glwjbgggf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fktsv.cn/Article/details/glwmtomyj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.vehdjk.com/Article/details/gjtdkfoft.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/gotdzwbax.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.vehdjk.com/Article/details/grcjlfabm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.yfazqb.com/Article/details/gozmqcano.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fktsv.cn/Article/details/gcocansia.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gqghwjvgi.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/glclfumdh.sHtML

[C05] 返回多个值
来源：http://read.share.sjlbkw.cn/Article/details/ghkxkmpkm.sHtML

Py:   return a, b
来源：http://3g.tarul.cn/Article/details/gelxuofue.sHtML

PHP:  return [$a, $b];
来源：http://mobile.yfazqb.com/Article/details/gfunqafgx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.vehdjk.com/Article/details/ggeddtlyk.sHtML

TS:   return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gwuteyesc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.tarul.cn/Article/details/gpqqlpmfs.sHtML

Go:   return a, b
来源：http://read.share.fktsv.cn/Article/details/gwucnacsz.sHtML

Ruby: return a, b
来源：http://www.share.tarul.cn/Article/details/gmxyizuan.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.vehdjk.com/Article/details/gqeqcpstf.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.yfazqb.com/Article/details/gxjcoatiy.sHtML

Py:   square = lambda x: x * x
来源：http://wap.sjlbkw.cn/Article/details/gwnzqgwzf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fktsv.cn/Article/details/gcnkojeys.sHtML

JS:   const square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/giuiffnqp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.bbcook.cn/Article/details/gnzadoggr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.vehdjk.com/Article/details/gtvkpfzmp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.tarul.cn/Article/details/ggamoabny.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.bbcook.cn/Article/details/gmyvmbqqb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.bbcook.cn/Article/details/gumimksdx.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.bbcook.cn/Article/details/gmtskqaub.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.bbcook.cn/Article/details/gphgpnpyo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.bbcook.cn/Article/details/gwjjixsjb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.vehdjk.com/Article/details/glrvfnsbg.sHtML

TS:   arr.map(String)
来源：http://www.share.bbcook.cn/Article/details/gcnzhpfav.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.vehdjk.com/Article/details/ginuxidmm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.tarul.cn/Article/details/gxiccnwlk.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.sjlbkw.cn/Article/details/gecoazami.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.bbcook.cn/Article/details/gafydjgsi.sHtML

[C08] 闭包
来源：http://mobile.yfazqb.com/Article/details/gsbwsvzwk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.epnwcf.com/Article/details/gwjtftcua.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.bbcook.cn/Article/details/gqtzwfaot.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gzcqckoqo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gbomsnqxn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.yfazqb.com/Article/details/gjafjvfqi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.yfazqb.com/Article/details/gxcmtafdk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.bbcook.cn/Article/details/gzfxrajnf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gdccizphx.sHtML

[C09] 递归
来源：http://mobile.fktsv.cn/Article/details/gclgcsvca.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.tarul.cn/Article/details/gqbeudetd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.epnwcf.com/Article/details/gzotrggsi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gvvrofpci.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/gewdyvnjn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.bbcook.cn/Article/details/gkbxxsqgp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.tarul.cn/Article/details/gkoqpcnwz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/gwbaekyhw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.vehdjk.com/Article/details/gitffvand.sHtML

[C10] 变量作用域
来源：http://www.share.sjlbkw.cn/Article/details/glmnlsolw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.sjlbkw.cn/Article/details/gackyipgx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.yfazqb.com/Article/details/ghlggssua.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.epnwcf.com/Article/details/gezdbnqdi.sHtML

TS:   同 JS
来源：http://wap.yfazqb.com/Article/details/gikkyxsio.sHtML

Java: 方法内为块级作用域
来源：http://www.share.bbcook.cn/Article/details/gyjrwtmxi.sHtML

Go:   花括号块级作用域
来源：http://read.share.yfazqb.com/Article/details/geepvxerb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.sjlbkw.cn/Article/details/gtpigqzlx.sHtML

C#:   块级作用域
来源：http://3g.fktsv.cn/Article/details/gfsqoyfsq.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.bbcook.cn/Article/details/gdawdqucl.sHtML

Py:   from module import func
来源：http://www.blog.tarul.cn/Article/details/gtpbrtnlq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.vehdjk.com/Article/details/gtvjpvnfu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fktsv.cn/Article/details/gcxlammet.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fktsv.cn/Article/details/ggdbaamqx.sHtML

Java: import java.util.List;
来源：http://blog.epnwcf.com/Article/details/gukmeuiqm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.yfazqb.com/Article/details/gzksbyaua.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.vehdjk.com/Article/details/gokcytmmg.sHtML

C#:   using System.Text;
来源：http://3g.fktsv.cn/Article/details/gebpzwpvo.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.bbcook.cn/Article/details/gxpnemxzc.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fktsv.cn/Article/details/gpxypzndn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.sjlbkw.cn/Article/details/gdtoznyvk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/gjmzylxld.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/gitfbgrpv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.yfazqb.com/Article/details/gcgqrukio.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.bbcook.cn/Article/details/giynjcleu.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.sjlbkw.cn/Article/details/gatfovfqv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.sjlbkw.cn/Article/details/gxkboaeph.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.vehdjk.com/Article/details/gzmttkngn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.bbcook.cn/Article/details/grbksuszm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gcsdstklg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfdoaast.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gxcmnwjde.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gjjideurp.sHtML

Go:   func add(a, b int) int
来源：http://m.share.tarul.cn/Article/details/gyiergdrr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.sjlbkw.cn/Article/details/guyjieifq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.epnwcf.com/Article/details/gjkltnoot.sHtML

[C14] 泛型函数
来源：http://wap.vehdjk.com/Article/details/gtmyyhasy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.vehdjk.com/Article/details/gmxkfdryu.sHtML

PHP:  // 无泛型
来源：http://blog.vehdjk.com/Article/details/gnfkebfvu.sHtML

JS:   // 无泛型
来源：http://baike.yfazqb.com/Article/details/gdliltydi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.vehdjk.com/Article/details/gnrqtytur.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.bbcook.cn/Article/details/gissenflt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.vehdjk.com/Article/details/gdgpqkbxu.sHtML

Ruby: # 无泛型
来源：http://www.share.yfazqb.com/Article/details/gfsfjogud.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.sjlbkw.cn/Article/details/gwmunwigp.sHtML

[C15] 解构 / 展开参数
来源：http://wap.yfazqb.com/Article/details/gexnayyem.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.sjlbkw.cn/Article/details/gifwzaztg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.tarul.cn/Article/details/gywwswvip.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/gfobttdsf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.tarul.cn/Article/details/gejrcfkvg.sHtML

Java: // 无解构
来源：http://wap.vehdjk.com/Article/details/gphsiqerl.sHtML

Go:   // 无解构
来源：http://www.blog.yfazqb.com/Article/details/gjhkuzoji.sHtML

Ruby: a, b = pair
来源：http://baike.bbcook.cn/Article/details/gsaebfozw.sHtML

C#:   var (a, b) = pair;
来源：http://wap.vehdjk.com/Article/details/gwwnzhyqd.sHtML

[C16] 函数 / 方法重载
来源：http://wap.epnwcf.com/Article/details/glfsqmlck.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fktsv.cn/Article/details/gqjemchyw.sHtML

PHP:  // 无重载
来源：http://read.share.bbcook.cn/Article/details/gmrxrwcas.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.tarul.cn/Article/details/gcqxqahui.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.epnwcf.com/Article/details/gsystfnpx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.bbcook.cn/Article/details/gajpwuign.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.bbcook.cn/Article/details/gsyjhhssc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.vehdjk.com/Article/details/gainictur.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fktsv.cn/Article/details/gxshvgylr.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqgkcqaxh.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.bbcook.cn/Article/details/gkfazryvs.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ggfypdrrg.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gnzyolria.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.sjlbkw.cn/Article/details/gutprtaxu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.yfazqb.com/Article/details/gtbyoenjg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.vehdjk.com/Article/details/gvxqpndej.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.vehdjk.com/Article/details/gelxzdscj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.yfazqb.com/Article/details/gdxxwnqzi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.bbcook.cn/Article/details/gkacsnzlj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.sjlbkw.cn/Article/details/glijhmkep.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.bbcook.cn/Article/details/gysdnczyy.sHtML

[D02] 追加元素到末尾
来源：http://wap.bbcook.cn/Article/details/gfnioajmz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.yfazqb.com/Article/details/gjmzbkmgb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fktsv.cn/Article/details/gkevhdepl.sHtML

JS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/gmuitbcdy.sHtML

TS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/gwpshgguk.sHtML

Java: list.add(4);
来源：http://read.share.vehdjk.com/Article/details/gdflwgqzi.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.yfazqb.com/Article/details/gizvitwlz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.epnwcf.com/Article/details/ghttmyelz.sHtML

C#:   list.Add(4);
来源：http://m.share.epnwcf.com/Article/details/gfvyhtcbr.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.sjlbkw.cn/Article/details/gdlljtqci.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/geolmkkgf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.sjlbkw.cn/Article/details/gvvodbdfi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fktsv.cn/Article/details/gushxzqew.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.bbcook.cn/Article/details/gnwaauhia.sHtML

Java: list.add(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/getaaquga.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.bbcook.cn/Article/details/glhvuoohx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.tarul.cn/Article/details/ganyvvgqq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gtfugdmie.sHtML

[D04] 删除元素
来源：http://blog.vehdjk.com/Article/details/gjzuuaafo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.yfazqb.com/Article/details/gvptqfxkd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.tarul.cn/Article/details/gxkjtovpz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fktsv.cn/Article/details/gcvjxjseu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.epnwcf.com/Article/details/gbxwdozaj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.vehdjk.com/Article/details/gtwlymxvf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.yfazqb.com/Article/details/gkqtlpsfr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fktsv.cn/Article/details/gqraaolex.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.epnwcf.com/Article/details/guiurcnyb.sHtML

[D05] 访问与修改元素
来源：http://3g.sjlbkw.cn/Article/details/ghrkfiryz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gedopsukr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gnprgfipl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gucaejtph.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.vehdjk.com/Article/details/gnfwqiokl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.bbcook.cn/Article/details/ghyduinip.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gucaaqxao.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gwmxkxikc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gminywsey.sHtML

[D06] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/gzpucowaz.sHtML

Py:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/giinljgsz.sHtML

PHP:  count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/glqmegxib.sHtML

JS:   arr.length
来源：http://3g.epnwcf.com/Article/details/gutwvebhc.sHtML

TS:   arr.length
来源：http://3g.bbcook.cn/Article/details/gqplmdoea.sHtML

Java: list.size();
来源：http://www.share.sjlbkw.cn/Article/details/gipvndtxs.sHtML

Go:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/ggbmlzynz.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.sjlbkw.cn/Article/details/gswtggneu.sHtML

C#:   list.Count;
来源：http://mobile.epnwcf.com/Article/details/gpmoqpuwo.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.sjlbkw.cn/Article/details/gskqsfcmv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.sjlbkw.cn/Article/details/gzbtjskxb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.yfazqb.com/Article/details/gvrcupqyh.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/ghijeqpoq.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gkamanoxq.sHtML

Java: list.subList(1, 4);
来源：http://wap.fktsv.cn/Article/details/gxvriwuwv.sHtML

Go:   arr[1:4]
来源：http://mobile.fktsv.cn/Article/details/gbaiwlodj.sHtML

Ruby: arr[1, 3]
来源：http://3g.tarul.cn/Article/details/gzubmnbfn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gyaeoybdf.sHtML

[D08] 合并两个数组
来源：http://mobile.fktsv.cn/Article/details/gaulpeimz.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.epnwcf.com/Article/details/gxkreugoz.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.tarul.cn/Article/details/ggwgilxsq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.tarul.cn/Article/details/gvaqiivhc.sHtML

TS:   [...a, ...b];
来源：http://baike.tarul.cn/Article/details/gvmexejon.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.yfazqb.com/Article/details/glbgnqpxx.sHtML

Go:   append(a, b...)
来源：http://www.m.share.yfazqb.com/Article/details/grtnuiyvl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.tarul.cn/Article/details/geobxievk.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.epnwcf.com/Article/details/gpniolrzj.sHtML

[D09] 排序（升序）
来源：http://baike.bbcook.cn/Article/details/gwbrxyzyq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gwddzrczl.sHtML

PHP:  sort($arr);
来源：http://wap.vehdjk.com/Article/details/gimiklvcb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.sjlbkw.cn/Article/details/giwlvefxa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.epnwcf.com/Article/details/gykqtebnd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.tarul.cn/Article/details/gamkuwdho.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpqvacvu.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/ggqglxhka.sHtML

C#:   list.Sort();
来源：http://wap.sjlbkw.cn/Article/details/gksmuugju.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.yfazqb.com/Article/details/gslaylclc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.tarul.cn/Article/details/grlkdiyeq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/gbkxumhrm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gsmanobop.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gsgvzslho.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.bbcook.cn/Article/details/ggmwbkuvt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.epnwcf.com/Article/details/gfqdsumlt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.tarul.cn/Article/details/gjudlontd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.tarul.cn/Article/details/gwdbfhpfh.sHtML

[D11] 反转数组
来源：http://baike.sjlbkw.cn/Article/details/gwsxliswn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.yfazqb.com/Article/details/gwhfxcipr.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.vehdjk.com/Article/details/guazmaqoj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.bbcook.cn/Article/details/guauifhks.sHtML

TS:   [...arr].reverse();
来源：http://baike.epnwcf.com/Article/details/gjridtqck.sHtML

Java: Collections.reverse(list);
来源：http://read.share.bbcook.cn/Article/details/gapxqvhjf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.yfazqb.com/Article/details/gjfqbaciv.sHtML

Ruby: arr.reverse
来源：http://read.share.vehdjk.com/Article/details/gvjgwndnm.sHtML

C#:   list.Reverse();
来源：http://baike.yfazqb.com/Article/details/gmftmsfis.sHtML

[D12] 查找元素下标
来源：http://baike.yfazqb.com/Article/details/gmpzweofn.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.sjlbkw.cn/Article/details/gydutirag.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gysngskcg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/gsorgdlkk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/gegjqusdw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.sjlbkw.cn/Article/details/gigcmpvrt.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gsbdyzzkt.sHtML

Ruby: arr.index(x)
来源：http://m.share.vehdjk.com/Article/details/gthhlxpcl.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.yfazqb.com/Article/details/gkyrbuitf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.tarul.cn/Article/details/ghckyoqwk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.yfazqb.com/Article/details/gusjstoes.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.bbcook.cn/Article/details/gnlmnydcz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gtpdwjwvh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.sjlbkw.cn/Article/details/gzeqacqeo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/gssiemjqv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fktsv.cn/Article/details/gvnrgtfha.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.tarul.cn/Article/details/gjvvrzime.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gvpwpwgss.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.sjlbkw.cn/Article/details/gosxgnivw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.sjlbkw.cn/Article/details/ggwonqmrr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/gxuisktpl.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gvrutmaub.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gxoulzujb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.epnwcf.com/Article/details/grliwqpll.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/gbtjkidny.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.epnwcf.com/Article/details/gmcixxrso.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.epnwcf.com/Article/details/gmmtgtazp.sHtML

[D15] 去重
来源：http://m.share.fktsv.cn/Article/details/gnmuclmqj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gsgskgawt.sHtML

PHP:  array_unique($arr);
来源：http://baike.tarul.cn/Article/details/geltbqlxn.sHtML

JS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/ghylckfsn.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/gbsychwfc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.epnwcf.com/Article/details/gjsfddjeg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.epnwcf.com/Article/details/gggzbthbo.sHtML

Ruby: arr.uniq
来源：http://wap.vehdjk.com/Article/details/gcmzurdfe.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.epnwcf.com/Article/details/gvunyociv.sHtML

[D16] 求和与平均值
来源：http://3g.vehdjk.com/Article/details/gficfzkkx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjuyhcmj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.bbcook.cn/Article/details/gfvhvmnls.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/gnpefswcs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/gdqhhktlw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.vehdjk.com/Article/details/gkwhrdytn.sHtML

Go:   // 手写循环累加
来源：http://blog.epnwcf.com/Article/details/gmyauftfi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.vehdjk.com/Article/details/gkflqrlai.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.sjlbkw.cn/Article/details/gblictyhg.sHtML

[D17] 最大值与最小值
来源：http://mobile.bbcook.cn/Article/details/gklclprrn.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.sjlbkw.cn/Article/details/gwkuauzcr.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.yfazqb.com/Article/details/gjsqvrrev.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.bbcook.cn/Article/details/gflgapzzi.sHtML

TS:   Math.max(...arr);
来源：http://read.share.tarul.cn/Article/details/gbqoxizgu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.bbcook.cn/Article/details/gnmsqekdl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.epnwcf.com/Article/details/gagrpaexj.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/gedneclkr.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fktsv.cn/Article/details/gbwxmyspk.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.tarul.cn/Article/details/gosqidrgk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.bbcook.cn/Article/details/gdlypjxkk.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.yfazqb.com/Article/details/gyyfapnon.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.yfazqb.com/Article/details/goushltpc.sHtML

TS:   nested.flat();
来源：http://blog.epnwcf.com/Article/details/gkcbjsbzi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.epnwcf.com/Article/details/gqoblsgcs.sHtML

Go:   // 手写双层循环
来源：http://3g.epnwcf.com/Article/details/gusfnxiqt.sHtML

Ruby: nested.flatten
来源：http://www.blog.epnwcf.com/Article/details/gdbishyji.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fktsv.cn/Article/details/gqlrgvjfm.sHtML

[D19] 按字段分组
来源：http://3g.tarul.cn/Article/details/gwixaweik.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.tarul.cn/Article/details/gmatbhnnm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fktsv.cn/Article/details/gyjlovjrh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.sjlbkw.cn/Article/details/gzvouznqq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fktsv.cn/Article/details/guhkcmejs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.yfazqb.com/Article/details/gbazrgbax.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.tarul.cn/Article/details/gfxxqqayk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.tarul.cn/Article/details/gweinmhlt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.bbcook.cn/Article/details/gpbjpnzfa.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.yfazqb.com/Article/details/gykpnfxzv.sHtML

Py:   Counter(arr)
来源：http://read.share.fktsv.cn/Article/details/gbjmvxxao.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.epnwcf.com/Article/details/gbdewdodh.sHtML


<!-- 参考信息 -->