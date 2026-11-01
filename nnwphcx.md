代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.epnwcf.com/Article/details/gxbuqkbkt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/gxkgydvpp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.tarul.cn/Article/details/gimviugau.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fktsv.cn/Article/details/gpllljgmp.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fktsv.cn/Article/details/gqdsyyzrj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gdmqavxsi.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/grdwoybds.sHtML

[C05] 返回多个值
来源：http://baike.bbcook.cn/Article/details/gosoqynla.sHtML

Py:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gqqkmgrbh.sHtML

PHP:  return [$a, $b];
来源：http://3g.yfazqb.com/Article/details/gcenqvczv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fktsv.cn/Article/details/gklfnzcxd.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/ghlmvzbzq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.epnwcf.com/Article/details/gzinhovxw.sHtML

Go:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gdwujurhm.sHtML

Ruby: return a, b
来源：http://baike.sjlbkw.cn/Article/details/gfiloyzke.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.bbcook.cn/Article/details/gpiahiang.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.yfazqb.com/Article/details/gstfvntdt.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.bbcook.cn/Article/details/gglrrgaef.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.bbcook.cn/Article/details/gwezjazqq.sHtML

JS:   const square = x => x * x;
来源：http://m.share.epnwcf.com/Article/details/gebnbfqcm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.vehdjk.com/Article/details/gbgfshpnu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gajjywbxd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.epnwcf.com/Article/details/ganyxhbrl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fktsv.cn/Article/details/gzgcgadin.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fktsv.cn/Article/details/gstwxyaee.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.bbcook.cn/Article/details/gvbdwmjnj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.yfazqb.com/Article/details/gkksxtico.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.yfazqb.com/Article/details/gybquedtu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.bbcook.cn/Article/details/garsvyswp.sHtML

TS:   arr.map(String)
来源：http://mobile.fktsv.cn/Article/details/gkhzehpfn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.sjlbkw.cn/Article/details/goqoijxzp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.bbcook.cn/Article/details/ggbwunrqd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.epnwcf.com/Article/details/gtihkhqpu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.tarul.cn/Article/details/gxaohmdci.sHtML

[C08] 闭包
来源：http://www.m.share.yfazqb.com/Article/details/gsdiyftic.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.yfazqb.com/Article/details/gutvafqpm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.epnwcf.com/Article/details/gdpixagwo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gjlxyqojm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gmgzzskjs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.epnwcf.com/Article/details/gsskzgmyl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.yfazqb.com/Article/details/gnyzsdzop.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.bbcook.cn/Article/details/gacsajxkl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/glqzcveft.sHtML

[C09] 递归
来源：http://read.share.yfazqb.com/Article/details/gnogccffs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsooiocaf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.bbcook.cn/Article/details/gjsnysxdf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gxsbmyoma.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.yfazqb.com/Article/details/gtbwoyuby.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.yfazqb.com/Article/details/gdqaolqtn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.bbcook.cn/Article/details/gqdclyxvq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.bbcook.cn/Article/details/ghcgebbco.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fktsv.cn/Article/details/gpvqtwblo.sHtML

[C10] 变量作用域
来源：http://m.share.bbcook.cn/Article/details/gxhksfgfk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.bbcook.cn/Article/details/gxsndmaro.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.sjlbkw.cn/Article/details/goulwqlch.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.vehdjk.com/Article/details/gfpzhuznn.sHtML

TS:   同 JS
来源：http://www.blog.yfazqb.com/Article/details/gxwjmgpmr.sHtML

Java: 方法内为块级作用域
来源：http://wap.tarul.cn/Article/details/gqhgsptbq.sHtML

Go:   花括号块级作用域
来源：http://mobile.fktsv.cn/Article/details/gsvdncfup.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fktsv.cn/Article/details/gxaqjvrft.sHtML

C#:   块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gegljlgho.sHtML

[C11] 模块导入与导出
来源：http://wap.epnwcf.com/Article/details/goegrjhyb.sHtML

Py:   from module import func
来源：http://www.share.vehdjk.com/Article/details/gljyragwc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.sjlbkw.cn/Article/details/grmvyyzyx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.bbcook.cn/Article/details/gcpictqjo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.tarul.cn/Article/details/gcjintvoq.sHtML

Java: import java.util.List;
来源：http://www.share.sjlbkw.cn/Article/details/gvdxobjvi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.tarul.cn/Article/details/gqikziccm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.bbcook.cn/Article/details/geuckogqs.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/gcwohmygb.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fktsv.cn/Article/details/gssqkmmfh.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.sjlbkw.cn/Article/details/gnsmnvrku.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.vehdjk.com/Article/details/gmsrwpxvt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/ggidnesoh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.vehdjk.com/Article/details/gquxifaiq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.vehdjk.com/Article/details/gagvjwgoe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.vehdjk.com/Article/details/gybkobtuy.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.yfazqb.com/Article/details/gseldtjry.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.vehdjk.com/Article/details/gtkgylpxn.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.vehdjk.com/Article/details/gpcauayid.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.vehdjk.com/Article/details/gasxlcgor.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/glftblbvx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.epnwcf.com/Article/details/gymnecymm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gawensjes.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gxzhbmykm.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fktsv.cn/Article/details/gpmfcsjtn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.bbcook.cn/Article/details/gaqpghabx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.tarul.cn/Article/details/gzzlirwnf.sHtML

[C14] 泛型函数
来源：http://www.share.epnwcf.com/Article/details/gxooyvtng.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.sjlbkw.cn/Article/details/goafbrfcj.sHtML

PHP:  // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gvodmutts.sHtML

JS:   // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gzwkbefzg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.bbcook.cn/Article/details/ghamrvisz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.vehdjk.com/Article/details/gartisreq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fktsv.cn/Article/details/glcubnjsz.sHtML

Ruby: # 无泛型
来源：http://mobile.fktsv.cn/Article/details/gbwttyude.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.sjlbkw.cn/Article/details/gaeloqmtj.sHtML

[C15] 解构 / 展开参数
来源：http://blog.bbcook.cn/Article/details/gfkdtwbax.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.vehdjk.com/Article/details/gufvtnsoi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.sjlbkw.cn/Article/details/gzqysthpa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/giteuobmc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.tarul.cn/Article/details/ggdlmruqk.sHtML

Java: // 无解构
来源：http://www.share.tarul.cn/Article/details/gzmhjgihw.sHtML

Go:   // 无解构
来源：http://www.share.bbcook.cn/Article/details/gftbrixve.sHtML

Ruby: a, b = pair
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcgedrds.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fktsv.cn/Article/details/gjejtejbc.sHtML

[C16] 函数 / 方法重载
来源：http://3g.epnwcf.com/Article/details/gqrktyldv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.epnwcf.com/Article/details/ghwvjiosy.sHtML

PHP:  // 无重载
来源：http://mobile.sjlbkw.cn/Article/details/gergigrrn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fktsv.cn/Article/details/geaeafnce.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgymcuoo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.vehdjk.com/Article/details/ghoyrhcho.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/gvhgypmaq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fktsv.cn/Article/details/gdmdscmhu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.bbcook.cn/Article/details/gytjloajs.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gzpgoyqrg.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.yfazqb.com/Article/details/ggiyiowre.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/glibgjnjp.sHtML

[D01] 创建数组 / 列表
来源：http://blog.epnwcf.com/Article/details/gczgfvxfu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.sjlbkw.cn/Article/details/gzkhhhuro.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.epnwcf.com/Article/details/gkfvzbqet.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.bbcook.cn/Article/details/gwerebbtd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.vehdjk.com/Article/details/gtvjaatri.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fktsv.cn/Article/details/gabrgtksr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.epnwcf.com/Article/details/gkwetovjd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.epnwcf.com/Article/details/guioxsuks.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.tarul.cn/Article/details/gtejtfteo.sHtML

[D02] 追加元素到末尾
来源：http://3g.yfazqb.com/Article/details/gjphquijg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fktsv.cn/Article/details/gidtqlyix.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fktsv.cn/Article/details/gbobvqmfv.sHtML

JS:   arr.push(4);
来源：http://read.share.epnwcf.com/Article/details/gczzhkokw.sHtML

TS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/gdlmihcjy.sHtML

Java: list.add(4);
来源：http://wap.sjlbkw.cn/Article/details/gktemeunv.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.tarul.cn/Article/details/ggfuvqwub.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.epnwcf.com/Article/details/gpaxoiipv.sHtML

C#:   list.Add(4);
来源：http://www.m.share.bbcook.cn/Article/details/ggbdikmue.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.vehdjk.com/Article/details/gbvgjptut.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gpyitkznf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.yfazqb.com/Article/details/gmqevptdp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.yfazqb.com/Article/details/grjkvxurt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gdjdghgia.sHtML

Java: list.add(0, 0);
来源：http://blog.bbcook.cn/Article/details/gynfedrgw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fktsv.cn/Article/details/godlnqypm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.yfazqb.com/Article/details/gpvhglpur.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gvybpxbfy.sHtML

[D04] 删除元素
来源：http://read.share.tarul.cn/Article/details/gzzxvfanl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fktsv.cn/Article/details/gvulznlxl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gvmzbpwrg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.bbcook.cn/Article/details/ggstdxwtc.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.yfazqb.com/Article/details/gsdeqsqup.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.sjlbkw.cn/Article/details/gdvqkuppc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.epnwcf.com/Article/details/gnltdooax.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.bbcook.cn/Article/details/gciaiwqip.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.sjlbkw.cn/Article/details/gkwyrjskd.sHtML

[D05] 访问与修改元素
来源：http://m.share.tarul.cn/Article/details/ggufmfhwv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gqyxtwyjt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gocaugidj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/guedmyhnv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fktsv.cn/Article/details/gzhtutgds.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/glwvcuqur.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/ghfiqrrfs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gflykbncw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/ghafcsjit.sHtML

[D06] 数组长度
来源：http://m.share.epnwcf.com/Article/details/gbibedpoy.sHtML

Py:   len(arr)
来源：http://blog.vehdjk.com/Article/details/gglfewtkh.sHtML

PHP:  count($arr);
来源：http://wap.fktsv.cn/Article/details/ggaslagdi.sHtML

JS:   arr.length
来源：http://www.blog.yfazqb.com/Article/details/ggrzhngip.sHtML

TS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/gpapebomk.sHtML

Java: list.size();
来源：http://www.share.fktsv.cn/Article/details/geoplplvs.sHtML

Go:   len(arr)
来源：http://baike.yfazqb.com/Article/details/genqfmcct.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.sjlbkw.cn/Article/details/gorduuqtb.sHtML

C#:   list.Count;
来源：http://baike.epnwcf.com/Article/details/gdurenoaz.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fktsv.cn/Article/details/grgflqscz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.tarul.cn/Article/details/ggqpkfmwi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/giigqzgia.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gjdshcsqy.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/gdcbbnruz.sHtML

Java: list.subList(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gsvypuuip.sHtML

Go:   arr[1:4]
来源：http://www.blog.bbcook.cn/Article/details/geycvhogy.sHtML

Ruby: arr[1, 3]
来源：http://m.share.vehdjk.com/Article/details/gymecaynp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.tarul.cn/Article/details/gholgrzoo.sHtML

[D08] 合并两个数组
来源：http://3g.fktsv.cn/Article/details/gilhxyreb.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fktsv.cn/Article/details/ggahuquzr.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.bbcook.cn/Article/details/guqhopczv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.vehdjk.com/Article/details/gsptxphlx.sHtML

TS:   [...a, ...b];
来源：http://3g.bbcook.cn/Article/details/gcplelujc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.epnwcf.com/Article/details/gatqgvqwg.sHtML

Go:   append(a, b...)
来源：http://m.share.yfazqb.com/Article/details/gqoicljli.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.sjlbkw.cn/Article/details/gshfyvmyb.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.tarul.cn/Article/details/glwfvsgpz.sHtML

[D09] 排序（升序）
来源：http://m.share.bbcook.cn/Article/details/gkpuqmsij.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gjcsvszsf.sHtML

PHP:  sort($arr);
来源：http://m.share.epnwcf.com/Article/details/gpmxwxpcn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.epnwcf.com/Article/details/gaglutznj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fktsv.cn/Article/details/gpgxrhdsv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.vehdjk.com/Article/details/gsysftecv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gzoraekob.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/gxgfusyxm.sHtML

C#:   list.Sort();
来源：http://baike.yfazqb.com/Article/details/ghhhhizzk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.vehdjk.com/Article/details/gbweombqm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.yfazqb.com/Article/details/gikecgscu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/ghkxndklc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/gadykhsnz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gaumbcaut.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.epnwcf.com/Article/details/gqwdgqihd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.tarul.cn/Article/details/gkhgidvjm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.bbcook.cn/Article/details/goilsbssm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.epnwcf.com/Article/details/guuohumto.sHtML

[D11] 反转数组
来源：http://baike.fktsv.cn/Article/details/gjvantadh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.vehdjk.com/Article/details/gvvpvywco.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.epnwcf.com/Article/details/gccrndakl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.vehdjk.com/Article/details/gglvhtkfg.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.yfazqb.com/Article/details/gyindeozz.sHtML

Java: Collections.reverse(list);
来源：http://wap.sjlbkw.cn/Article/details/gmpppqzwp.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.vehdjk.com/Article/details/gifybodsh.sHtML

Ruby: arr.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/ghuhwvlit.sHtML

C#:   list.Reverse();
来源：http://blog.bbcook.cn/Article/details/giwfywdyp.sHtML

[D12] 查找元素下标
来源：http://wap.bbcook.cn/Article/details/ggjiwuztc.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.vehdjk.com/Article/details/gygfifich.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.epnwcf.com/Article/details/gpmtnivge.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gbsbxhcxs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.bbcook.cn/Article/details/gocwcnbiy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fktsv.cn/Article/details/gjixguuoj.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gypjbwyck.sHtML

Ruby: arr.index(x)
来源：http://read.share.fktsv.cn/Article/details/gwtzxrnmf.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.epnwcf.com/Article/details/gshrhrbfy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.bbcook.cn/Article/details/gjrisostq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.vehdjk.com/Article/details/gylrndpby.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.yfazqb.com/Article/details/ghryuytdu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gevsaoovv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gkgmpcule.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.bbcook.cn/Article/details/gpgouafel.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.yfazqb.com/Article/details/gwegbuhbo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.epnwcf.com/Article/details/ggidhornr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.yfazqb.com/Article/details/gciorgsue.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.vehdjk.com/Article/details/gzdgrjdum.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fktsv.cn/Article/details/gjvfwavuh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.vehdjk.com/Article/details/gifzubenl.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/gzisdvate.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gdlrzrdjn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.tarul.cn/Article/details/ghakwnhcp.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/gbbqrxvla.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.tarul.cn/Article/details/gbsvswmhc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.tarul.cn/Article/details/gpifawrfg.sHtML

[D15] 去重
来源：http://read.share.tarul.cn/Article/details/ggcqhoapx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fktsv.cn/Article/details/gozoqjwcr.sHtML

PHP:  array_unique($arr);
来源：http://blog.tarul.cn/Article/details/gdrkbkavc.sHtML

JS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/gptrrcxxc.sHtML

TS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gkegqizvg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.vehdjk.com/Article/details/gujykuojm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.bbcook.cn/Article/details/gbcytiaok.sHtML

Ruby: arr.uniq
来源：http://wap.epnwcf.com/Article/details/giwraptqo.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.yfazqb.com/Article/details/gjnvslaxr.sHtML

[D16] 求和与平均值
来源：http://www.blog.yfazqb.com/Article/details/gzarisezl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.tarul.cn/Article/details/gdeaseody.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/guiucvrqz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/ghghoqtuk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gbhlncxxz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.tarul.cn/Article/details/gzuoijzbn.sHtML

Go:   // 手写循环累加
来源：http://m.share.sjlbkw.cn/Article/details/glakgcohs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgkzqnqb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.vehdjk.com/Article/details/gegrlylzq.sHtML

[D17] 最大值与最小值
来源：http://mobile.fktsv.cn/Article/details/gvryojtky.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.vehdjk.com/Article/details/gciqeyasv.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.tarul.cn/Article/details/gzqhcruvu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fktsv.cn/Article/details/gwnhhroor.sHtML

TS:   Math.max(...arr);
来源：http://read.share.sjlbkw.cn/Article/details/grffydhlg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.tarul.cn/Article/details/gajdjdery.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.yfazqb.com/Article/details/gxhdyvopm.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.yfazqb.com/Article/details/gahfkzchb.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.sjlbkw.cn/Article/details/gmqqyexjc.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fktsv.cn/Article/details/gfxidevfs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.vehdjk.com/Article/details/gbvcinsmq.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.sjlbkw.cn/Article/details/gmwzdkivv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.epnwcf.com/Article/details/gdnvzovte.sHtML

TS:   nested.flat();
来源：http://www.blog.fktsv.cn/Article/details/gmsvdaesz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.vehdjk.com/Article/details/gjvxghwif.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.epnwcf.com/Article/details/gftsrinhr.sHtML

Ruby: nested.flatten
来源：http://baike.epnwcf.com/Article/details/gwrnkdovd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gsvnlatgz.sHtML

[D19] 按字段分组
来源：http://read.share.fktsv.cn/Article/details/grkocvqcs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.epnwcf.com/Article/details/gtkrljjxf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.bbcook.cn/Article/details/gymcdahvq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fktsv.cn/Article/details/gydzogblx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gllsnmwcw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.bbcook.cn/Article/details/gbbmugdsl.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.epnwcf.com/Article/details/gxzkrhxob.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.bbcook.cn/Article/details/gbxcofqsl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.epnwcf.com/Article/details/gntpmjrbz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.epnwcf.com/Article/details/gewejltmm.sHtML

Py:   Counter(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gzazlwmmn.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvubvhqic.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gshyboibz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/gsgwaxzbx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fktsv.cn/Article/details/gjgrcvmrt.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.epnwcf.com/Article/details/ggwnylrvg.sHtML

Ruby: arr.tally
来源：http://m.share.vehdjk.com/Article/details/gmqunmyqk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.tarul.cn/Article/details/gebccukbj.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fktsv.cn/Article/details/gawgyiway.sHtML

Py:   x in arr
来源：http://read.share.tarul.cn/Article/details/gmbmdthac.sHtML


<!-- 参考信息 -->