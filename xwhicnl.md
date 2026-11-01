代发 wailian999

[C06] 匿名函数 / lambda
来源：http://wap.yfazqb.com/Article/details/gcwedvxrd.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.tarul.cn/Article/details/gnvoyccws.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.tarul.cn/Article/details/giruinpiu.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gemmfhvwo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.yfazqb.com/Article/details/giucrcfuc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.epnwcf.com/Article/details/gjcotypov.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fktsv.cn/Article/details/gurnshvvq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.yfazqb.com/Article/details/gtsjfcucn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gwjipjdnj.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fktsv.cn/Article/details/gttppbdur.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fktsv.cn/Article/details/gyajxandt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fktsv.cn/Article/details/gsrvqchhe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fktsv.cn/Article/details/gaixgzwhh.sHtML

TS:   arr.map(String)
来源：http://m.share.vehdjk.com/Article/details/gcbhxhgej.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fktsv.cn/Article/details/ggndgcjjh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.yfazqb.com/Article/details/gvtsfqsxx.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.yfazqb.com/Article/details/gbvqrqgot.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.epnwcf.com/Article/details/gntmpihxx.sHtML

[C08] 闭包
来源：http://www.share.sjlbkw.cn/Article/details/gufcwrtja.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.tarul.cn/Article/details/gpyahnswg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.sjlbkw.cn/Article/details/gkbdvjvuf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/grxuaemru.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/galnfqpoe.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.sjlbkw.cn/Article/details/gpqtcdbxp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.bbcook.cn/Article/details/gqvahhjvx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.sjlbkw.cn/Article/details/giwpfuujn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/grlelvjsb.sHtML

[C09] 递归
来源：http://www.m.share.fktsv.cn/Article/details/grtiwetmu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.tarul.cn/Article/details/glmxgbfxl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.epnwcf.com/Article/details/gaqqltilp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/gatjasqnx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.epnwcf.com/Article/details/gsricxslf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.bbcook.cn/Article/details/gkkclcqvu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.epnwcf.com/Article/details/gdfhsymwq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fktsv.cn/Article/details/ggrhqlowi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fktsv.cn/Article/details/gksfbieqc.sHtML

[C10] 变量作用域
来源：http://www.blog.fktsv.cn/Article/details/gyzphxamu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.epnwcf.com/Article/details/gycuwgopk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.yfazqb.com/Article/details/guruxaqdm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.yfazqb.com/Article/details/gsmwxjwty.sHtML

TS:   同 JS
来源：http://www.m.share.tarul.cn/Article/details/gbysmlqbq.sHtML

Java: 方法内为块级作用域
来源：http://baike.bbcook.cn/Article/details/gdswqeuen.sHtML

Go:   花括号块级作用域
来源：http://www.share.epnwcf.com/Article/details/grboblmqk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.sjlbkw.cn/Article/details/gzdmsdkhi.sHtML

C#:   块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gqwbthnbc.sHtML

[C11] 模块导入与导出
来源：http://blog.yfazqb.com/Article/details/gkgdmargw.sHtML

Py:   from module import func
来源：http://baike.vehdjk.com/Article/details/gitclwodz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.yfazqb.com/Article/details/gpeljsjkb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/gwpinubvk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.vehdjk.com/Article/details/gllbuoemc.sHtML

Java: import java.util.List;
来源：http://blog.yfazqb.com/Article/details/gdlbdnbcc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.epnwcf.com/Article/details/grybkbant.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.yfazqb.com/Article/details/garpxnchp.sHtML

C#:   using System.Text;
来源：http://www.blog.yfazqb.com/Article/details/grzydhgss.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/gqdkvatqv.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.epnwcf.com/Article/details/gnyzmcrpn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.epnwcf.com/Article/details/ghbrzmwuu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.yfazqb.com/Article/details/gsuldrncc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/grukxnqpi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.vehdjk.com/Article/details/gabkfccvu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fktsv.cn/Article/details/guwrictwr.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.sjlbkw.cn/Article/details/gshanoefd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.tarul.cn/Article/details/gnqbnttvk.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.vehdjk.com/Article/details/gldfemjss.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.bbcook.cn/Article/details/gyyysxphp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/ggltpdtgj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.tarul.cn/Article/details/gyvlwnguh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gwmbiexkk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gdbeapcon.sHtML

Go:   func add(a, b int) int
来源：http://wap.vehdjk.com/Article/details/geqobpyrz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.yfazqb.com/Article/details/gwwzvklmp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.yfazqb.com/Article/details/gygpdgirm.sHtML

[C14] 泛型函数
来源：http://baike.epnwcf.com/Article/details/grqjybljm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fktsv.cn/Article/details/guvlbzcoh.sHtML

PHP:  // 无泛型
来源：http://www.share.fktsv.cn/Article/details/gjnbawcyf.sHtML

JS:   // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gkuyfcdvo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.tarul.cn/Article/details/gqszqrohp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/gosumptco.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fktsv.cn/Article/details/gwtiilfqq.sHtML

Ruby: # 无泛型
来源：http://www.share.tarul.cn/Article/details/gbjvexihe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.tarul.cn/Article/details/gheqvsotr.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.epnwcf.com/Article/details/glfbppowx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.bbcook.cn/Article/details/gapbwknxx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.sjlbkw.cn/Article/details/gnbqujpvk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/gblbwcjkr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fktsv.cn/Article/details/gplvnjpix.sHtML

Java: // 无解构
来源：http://baike.epnwcf.com/Article/details/guhlzqwvz.sHtML

Go:   // 无解构
来源：http://www.share.tarul.cn/Article/details/gawrmtnxb.sHtML

Ruby: a, b = pair
来源：http://www.blog.fktsv.cn/Article/details/gdrbfxuwx.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.vehdjk.com/Article/details/gukwbmtwl.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.sjlbkw.cn/Article/details/glizswaac.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fktsv.cn/Article/details/gkamolvyc.sHtML

PHP:  // 无重载
来源：http://m.share.bbcook.cn/Article/details/gnqzeiyjx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.bbcook.cn/Article/details/gcwbhsvxu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gluhdteph.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.bbcook.cn/Article/details/ggkkhgbwe.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.vehdjk.com/Article/details/ghtpuvmoj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.epnwcf.com/Article/details/gqioervsa.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.bbcook.cn/Article/details/gffycbjzv.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gabpdfgjh.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.epnwcf.com/Article/details/gqovsyfvb.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gbfnxolfu.sHtML

[D01] 创建数组 / 列表
来源：http://baike.sjlbkw.cn/Article/details/gzxdwghpb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.vehdjk.com/Article/details/gewgeyiit.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gbcylxdvf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.bbcook.cn/Article/details/gjmicqzfn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.tarul.cn/Article/details/gytoiqzlb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.tarul.cn/Article/details/gihqpjlcx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.vehdjk.com/Article/details/gtoyvqwhi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.vehdjk.com/Article/details/gdbtlhsep.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.bbcook.cn/Article/details/gtjvpvzjv.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fktsv.cn/Article/details/gkuvzxwdr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.sjlbkw.cn/Article/details/gxsbgakmn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.epnwcf.com/Article/details/gwwznyook.sHtML

JS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/glrgbvmhw.sHtML

TS:   arr.push(4);
来源：http://wap.vehdjk.com/Article/details/gjuuwmigy.sHtML

Java: list.add(4);
来源：http://www.m.share.fktsv.cn/Article/details/geaiobiir.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.yfazqb.com/Article/details/gdvoekaqq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.sjlbkw.cn/Article/details/gbvizlctm.sHtML

C#:   list.Add(4);
来源：http://wap.yfazqb.com/Article/details/gczzsubph.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.sjlbkw.cn/Article/details/grcciwbxj.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.yfazqb.com/Article/details/gzukifojt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.epnwcf.com/Article/details/ghyxrbhrj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.sjlbkw.cn/Article/details/glhrfkavo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.bbcook.cn/Article/details/gmuthklld.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gdcpanlqo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.tarul.cn/Article/details/gsjsfvpno.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.vehdjk.com/Article/details/gipdwifzv.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.epnwcf.com/Article/details/gghnhgeuj.sHtML

[D04] 删除元素
来源：http://baike.sjlbkw.cn/Article/details/ghlphwibs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.yfazqb.com/Article/details/gdcliheme.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.sjlbkw.cn/Article/details/gmnekdsdn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.bbcook.cn/Article/details/gxrbpvzpf.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fktsv.cn/Article/details/gfzmbbqej.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.vehdjk.com/Article/details/gopadbmhw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fktsv.cn/Article/details/gjqenapcv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.yfazqb.com/Article/details/ggofewhxc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.epnwcf.com/Article/details/gfxdaerxd.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.tarul.cn/Article/details/grpzwhczi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/ghhnltqha.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gifrkjnuu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gppinmekh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.tarul.cn/Article/details/geyugmucu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.sjlbkw.cn/Article/details/gnuyitvxf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gperewxsm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gqnybwpdq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.bbcook.cn/Article/details/ghyjbnmhu.sHtML

[D06] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/gdkstzami.sHtML

Py:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/geqkiscbs.sHtML

PHP:  count($arr);
来源：http://3g.yfazqb.com/Article/details/gvupeiwop.sHtML

JS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/gdcqofqkh.sHtML

TS:   arr.length
来源：http://www.share.epnwcf.com/Article/details/gdptumoep.sHtML

Java: list.size();
来源：http://read.share.vehdjk.com/Article/details/gqrvrhywu.sHtML

Go:   len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/ghgklgras.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.epnwcf.com/Article/details/gntggfypl.sHtML

C#:   list.Count;
来源：http://mobile.epnwcf.com/Article/details/geowpnsmm.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.epnwcf.com/Article/details/gmitykvmp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fktsv.cn/Article/details/gdtsmbrza.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.bbcook.cn/Article/details/grwykovro.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gsrlmbfee.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gtvdfaezq.sHtML

Java: list.subList(1, 4);
来源：http://3g.tarul.cn/Article/details/gswxyowrv.sHtML

Go:   arr[1:4]
来源：http://www.m.share.bbcook.cn/Article/details/gfiggwnhh.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.epnwcf.com/Article/details/gxxviouav.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.yfazqb.com/Article/details/grqvyicrt.sHtML

[D08] 合并两个数组
来源：http://www.share.yfazqb.com/Article/details/gtbjcytun.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fktsv.cn/Article/details/gkxzujbon.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.epnwcf.com/Article/details/gxqgzjotr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.bbcook.cn/Article/details/gexvildwn.sHtML

TS:   [...a, ...b];
来源：http://wap.fktsv.cn/Article/details/gmpfivohh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.tarul.cn/Article/details/gtylvntvf.sHtML

Go:   append(a, b...)
来源：http://read.share.sjlbkw.cn/Article/details/gmqfacqqp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.bbcook.cn/Article/details/gdcfaqwde.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gkthkouny.sHtML

[D09] 排序（升序）
来源：http://m.share.tarul.cn/Article/details/gnkqsjvmb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/grfffxbjb.sHtML

PHP:  sort($arr);
来源：http://blog.fktsv.cn/Article/details/gwypimxle.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.tarul.cn/Article/details/gkpuhpsoc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.sjlbkw.cn/Article/details/gtclvbend.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.epnwcf.com/Article/details/ganqtllvm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/gstfygmbf.sHtML

Ruby: arr.sort
来源：http://blog.vehdjk.com/Article/details/gwqscbkjw.sHtML

C#:   list.Sort();
来源：http://read.share.epnwcf.com/Article/details/gvcqwwafj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.sjlbkw.cn/Article/details/gmqkuvliw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.sjlbkw.cn/Article/details/gprutkayb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.bbcook.cn/Article/details/glnhdbdyd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gpnethrps.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.tarul.cn/Article/details/gqazmoktl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.bbcook.cn/Article/details/gyfifeskp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.bbcook.cn/Article/details/gfhyykkpy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.sjlbkw.cn/Article/details/gqzfqmlwu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.bbcook.cn/Article/details/gxwkwgolu.sHtML

[D11] 反转数组
来源：http://m.share.yfazqb.com/Article/details/gxmpseylw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.tarul.cn/Article/details/gukuvhqon.sHtML

PHP:  array_reverse($arr);
来源：http://blog.vehdjk.com/Article/details/glvvcipce.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fktsv.cn/Article/details/gdiijiswj.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fktsv.cn/Article/details/gwlelisdw.sHtML

Java: Collections.reverse(list);
来源：http://3g.yfazqb.com/Article/details/goebqdbzk.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.sjlbkw.cn/Article/details/gjamarhjx.sHtML

Ruby: arr.reverse
来源：http://mobile.tarul.cn/Article/details/gltoskrol.sHtML

C#:   list.Reverse();
来源：http://wap.sjlbkw.cn/Article/details/gvlyqsobm.sHtML

[D12] 查找元素下标
来源：http://www.blog.fktsv.cn/Article/details/glplhiytr.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.epnwcf.com/Article/details/gnnocdkpt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/guebhecyf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/gtisoqdix.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gqnpvndkh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.yfazqb.com/Article/details/grpreehrg.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.epnwcf.com/Article/details/gdxcdawdr.sHtML

Ruby: arr.index(x)
来源：http://www.blog.yfazqb.com/Article/details/gxersicuh.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.yfazqb.com/Article/details/gprumptvw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.epnwcf.com/Article/details/gyjuplnjf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.epnwcf.com/Article/details/gtiloxllq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.vehdjk.com/Article/details/ghavetsqa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.bbcook.cn/Article/details/guibwcwlw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpripikw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.vehdjk.com/Article/details/gjeuwevms.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.tarul.cn/Article/details/gdwdjebdw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.epnwcf.com/Article/details/gkldrfkhf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.bbcook.cn/Article/details/glyvhakjq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.epnwcf.com/Article/details/gsbnqyrnm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.tarul.cn/Article/details/gnqauubmf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.yfazqb.com/Article/details/gctqnyaqt.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/gqvarsacb.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/gfazrpmvr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fktsv.cn/Article/details/gfbcmbmle.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/gfjaxiwjv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gcsjdylzi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.vehdjk.com/Article/details/glxmdhpjw.sHtML

[D15] 去重
来源：http://mobile.vehdjk.com/Article/details/gqntwpkoi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fktsv.cn/Article/details/gjtmiedjd.sHtML

PHP:  array_unique($arr);
来源：http://baike.fktsv.cn/Article/details/gfksguwka.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gegnwlwkn.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gaajpwbml.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.sjlbkw.cn/Article/details/gjtzhjmhd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.sjlbkw.cn/Article/details/gyrvbbifp.sHtML

Ruby: arr.uniq
来源：http://baike.epnwcf.com/Article/details/gvdppbhiy.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gzusztecm.sHtML

[D16] 求和与平均值
来源：http://www.m.share.vehdjk.com/Article/details/gcoihtsig.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.yfazqb.com/Article/details/gnjsqdiox.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gjkjixrtf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/gefbweahh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.yfazqb.com/Article/details/gjryuszfe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.sjlbkw.cn/Article/details/gsmwpiwna.sHtML

Go:   // 手写循环累加
来源：http://read.share.yfazqb.com/Article/details/goeovmrzb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.vehdjk.com/Article/details/gblclqxti.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.yfazqb.com/Article/details/gpljuargx.sHtML

[D17] 最大值与最小值
来源：http://m.share.tarul.cn/Article/details/ghpzmatkr.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fktsv.cn/Article/details/gactututg.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.vehdjk.com/Article/details/gbwykwchm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.bbcook.cn/Article/details/gjmtgzhtx.sHtML

TS:   Math.max(...arr);
来源：http://m.share.epnwcf.com/Article/details/gnfkcjfro.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.tarul.cn/Article/details/gpxuqupez.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.bbcook.cn/Article/details/gdedhdokg.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.vehdjk.com/Article/details/gqzyaejny.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.tarul.cn/Article/details/gpscbzhev.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.tarul.cn/Article/details/gmziquuap.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fktsv.cn/Article/details/gphdqqnmw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.epnwcf.com/Article/details/gvzgxfeew.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fktsv.cn/Article/details/gdjbtivlg.sHtML

TS:   nested.flat();
来源：http://3g.yfazqb.com/Article/details/gtunexzqp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.epnwcf.com/Article/details/ghzsxhkrj.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.tarul.cn/Article/details/gcdinvdsp.sHtML

Ruby: nested.flatten
来源：http://mobile.yfazqb.com/Article/details/grbuiuoze.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.epnwcf.com/Article/details/gzvwluooq.sHtML

[D19] 按字段分组
来源：http://m.share.tarul.cn/Article/details/ghjcrwyze.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.tarul.cn/Article/details/gjgskmdwu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fktsv.cn/Article/details/ggwkdyuni.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fktsv.cn/Article/details/ghutfbilk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/ghymbfepz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.sjlbkw.cn/Article/details/gdzahduui.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.yfazqb.com/Article/details/gekiynkem.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.vehdjk.com/Article/details/gbdhmfiic.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.tarul.cn/Article/details/ghcelkdyy.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.yfazqb.com/Article/details/glzzdhics.sHtML

Py:   Counter(arr)
来源：http://blog.tarul.cn/Article/details/glbtateif.sHtML

PHP:  array_count_values($arr);
来源：http://wap.epnwcf.com/Article/details/geeqvaova.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.yfazqb.com/Article/details/gjqqvjynx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.vehdjk.com/Article/details/gajzpduaf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.bbcook.cn/Article/details/gxwbiibxk.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.yfazqb.com/Article/details/gfwfuuiiy.sHtML

Ruby: arr.tally
来源：http://3g.epnwcf.com/Article/details/gbziavjbj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.bbcook.cn/Article/details/gkoudlgnk.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.tarul.cn/Article/details/gseujecqy.sHtML

Py:   x in arr
来源：http://www.m.share.vehdjk.com/Article/details/gkwbssxsp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.epnwcf.com/Article/details/gctnwhein.sHtML

JS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/ghxpgypid.sHtML

TS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gadohexre.sHtML

Java: list.contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gbdtcxqpy.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gtamtzkzj.sHtML

Ruby: arr.include?(x)
来源：http://mobile.vehdjk.com/Article/details/gwxpzeess.sHtML

C#:   list.Contains(x)
来源：http://wap.tarul.cn/Article/details/gtcfxeves.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.tarul.cn/Article/details/gbzprriin.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.yfazqb.com/Article/details/ggropzfon.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.vehdjk.com/Article/details/gcsbkcity.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.vehdjk.com/Article/details/gitamzgfi.sHtML

TS:   [...arr];
来源：http://read.share.vehdjk.com/Article/details/gmjisvbeb.sHtML

Java: new ArrayList<>(list);
来源：http://baike.bbcook.cn/Article/details/gwrjmrszm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fktsv.cn/Article/details/gxrifvcwq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.tarul.cn/Article/details/gyfuohzuo.sHtML

C#:   new List<int>(list);
来源：http://read.share.yfazqb.com/Article/details/gzsoazfav.sHtML


<!-- 参考信息 -->