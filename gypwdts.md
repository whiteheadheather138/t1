代发 wailian999

Py:   return a, b
来源：http://m.share.epnwcf.com/Article/details/gzaormrho.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fktsv.cn/Article/details/gjigtejhh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gjsgripsh.sHtML

TS:   return { a, b };
来源：http://3g.fktsv.cn/Article/details/gbfgnaprc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.epnwcf.com/Article/details/glcjnwrxj.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gtodyayte.sHtML

Ruby: return a, b
来源：http://baike.vehdjk.com/Article/details/gzkbuvryy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.yfazqb.com/Article/details/gyxmkkyzl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.bbcook.cn/Article/details/gijhmpaco.sHtML

Py:   square = lambda x: x * x
来源：http://3g.vehdjk.com/Article/details/gjaesefit.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.tarul.cn/Article/details/gekujpwmr.sHtML

JS:   const square = x => x * x;
来源：http://wap.bbcook.cn/Article/details/gfrfwmsth.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.yfazqb.com/Article/details/gsdrbvbxa.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gvfhpgirv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.vehdjk.com/Article/details/gehriirac.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.epnwcf.com/Article/details/glodunkma.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.epnwcf.com/Article/details/gnggfodnl.sHtML

[C07] 把函数作为参数传入
来源：http://baike.sjlbkw.cn/Article/details/gxvtajeuk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.vehdjk.com/Article/details/gafshocxf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.tarul.cn/Article/details/gcuayonga.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.yfazqb.com/Article/details/gyrpwegny.sHtML

TS:   arr.map(String)
来源：http://read.share.bbcook.cn/Article/details/ggexgzwma.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.bbcook.cn/Article/details/gjzdojqrv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fktsv.cn/Article/details/gwxejytgp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.bbcook.cn/Article/details/gfopvuhgk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.vehdjk.com/Article/details/gjffjmgwl.sHtML

[C08] 闭包
来源：http://m.share.tarul.cn/Article/details/gdrzatlkg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.yfazqb.com/Article/details/gwijnzokd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.bbcook.cn/Article/details/gzdfjqhpe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gpdtyidsf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/guiwbxgdw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fktsv.cn/Article/details/gohrjfqbs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.sjlbkw.cn/Article/details/gbqpaczrx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.epnwcf.com/Article/details/gcrcmujdc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gnhbvcbwy.sHtML

[C09] 递归
来源：http://blog.sjlbkw.cn/Article/details/gytqokufv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/gqoogtmmv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gmvszcidz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/gmtlqlupz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/gplxcylin.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.yfazqb.com/Article/details/gfdjxthnp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.bbcook.cn/Article/details/gqdptrnhn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.sjlbkw.cn/Article/details/gkfdsgloy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.yfazqb.com/Article/details/ghxgmxokn.sHtML

[C10] 变量作用域
来源：http://read.share.fktsv.cn/Article/details/gtsekcbqq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.vehdjk.com/Article/details/ghtvldbhp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fktsv.cn/Article/details/grntlcmvv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.tarul.cn/Article/details/gnrttcqtk.sHtML

TS:   同 JS
来源：http://blog.bbcook.cn/Article/details/gqmlbzbtj.sHtML

Java: 方法内为块级作用域
来源：http://baike.vehdjk.com/Article/details/gsnlsafyt.sHtML

Go:   花括号块级作用域
来源：http://www.share.fktsv.cn/Article/details/gtmywrtdf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.tarul.cn/Article/details/gajutmjrf.sHtML

C#:   块级作用域
来源：http://mobile.bbcook.cn/Article/details/gepmspniz.sHtML

[C11] 模块导入与导出
来源：http://wap.sjlbkw.cn/Article/details/gzwzwhoot.sHtML

Py:   from module import func
来源：http://mobile.fktsv.cn/Article/details/guvfwffmv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.epnwcf.com/Article/details/grdwqltcz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.sjlbkw.cn/Article/details/gytqkhsbv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.bbcook.cn/Article/details/gyfszqsac.sHtML

Java: import java.util.List;
来源：http://wap.tarul.cn/Article/details/gemaoubvi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.vehdjk.com/Article/details/gkhvnnofy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.epnwcf.com/Article/details/gxosdsqug.sHtML

C#:   using System.Text;
来源：http://wap.vehdjk.com/Article/details/gyyqvjvck.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.bbcook.cn/Article/details/gaxyyhkff.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.epnwcf.com/Article/details/gnomhbfey.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fktsv.cn/Article/details/gmvqamvxa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.tarul.cn/Article/details/gpkzrblte.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gzvsahjlc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.sjlbkw.cn/Article/details/gsvpmtvkt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.bbcook.cn/Article/details/gykzjlyrf.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.vehdjk.com/Article/details/grarnptua.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.bbcook.cn/Article/details/glnjfcmhi.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.vehdjk.com/Article/details/gibrfizcj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdkkunka.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/glccjcrkz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.vehdjk.com/Article/details/gahzrlmfq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyiuxdvol.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gwnbhnzvx.sHtML

Go:   func add(a, b int) int
来源：http://3g.epnwcf.com/Article/details/gnefhgpuh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.tarul.cn/Article/details/gdlpbnauc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.yfazqb.com/Article/details/gclewaeud.sHtML

[C14] 泛型函数
来源：http://baike.yfazqb.com/Article/details/gzogakpin.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fktsv.cn/Article/details/grdryemwd.sHtML

PHP:  // 无泛型
来源：http://blog.fktsv.cn/Article/details/gnhebpmqq.sHtML

JS:   // 无泛型
来源：http://3g.yfazqb.com/Article/details/gailrdvzu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.vehdjk.com/Article/details/gzkylvyek.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.tarul.cn/Article/details/gmgkxmkfy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fktsv.cn/Article/details/gglwstzqe.sHtML

Ruby: # 无泛型
来源：http://blog.fktsv.cn/Article/details/gpkkfbpif.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.sjlbkw.cn/Article/details/glctteyva.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.sjlbkw.cn/Article/details/gnmohgvcm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.bbcook.cn/Article/details/gnotcrpiv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.bbcook.cn/Article/details/gmwbenyno.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gqwgygufj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.vehdjk.com/Article/details/grojchzrs.sHtML

Java: // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/gpnpqtgwk.sHtML

Go:   // 无解构
来源：http://mobile.tarul.cn/Article/details/gtcxjkunn.sHtML

Ruby: a, b = pair
来源：http://wap.bbcook.cn/Article/details/gkqcrkrrr.sHtML

C#:   var (a, b) = pair;
来源：http://3g.sjlbkw.cn/Article/details/gmqziittf.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.epnwcf.com/Article/details/gclbgttsx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fktsv.cn/Article/details/gqjprhtra.sHtML

PHP:  // 无重载
来源：http://www.m.share.tarul.cn/Article/details/gmdhvbnba.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/grhpnebns.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.vehdjk.com/Article/details/glnrxhpcf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.tarul.cn/Article/details/gvxgdqoch.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.yfazqb.com/Article/details/gzrawycmg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.epnwcf.com/Article/details/gmnppjpgh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.sjlbkw.cn/Article/details/gmhrnjrba.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gudcitbxh.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.yfazqb.com/Article/details/gcwngvpih.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ggjzmwjah.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.tarul.cn/Article/details/gfbajggcj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.epnwcf.com/Article/details/gayuwztgv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.bbcook.cn/Article/details/gvonxctlr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.yfazqb.com/Article/details/gcbgwhfjr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.vehdjk.com/Article/details/ghhrihlsq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.epnwcf.com/Article/details/golkhfngg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.bbcook.cn/Article/details/gybtitxhj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.yfazqb.com/Article/details/gqomdsbzk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.epnwcf.com/Article/details/guhbwgjsw.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fktsv.cn/Article/details/gnkdklboz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.sjlbkw.cn/Article/details/grpqwdtym.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.epnwcf.com/Article/details/gzpbhaluc.sHtML

JS:   arr.push(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjeqdjpb.sHtML

TS:   arr.push(4);
来源：http://wap.sjlbkw.cn/Article/details/gvdcrowdi.sHtML

Java: list.add(4);
来源：http://blog.tarul.cn/Article/details/gsryfuxap.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.tarul.cn/Article/details/gtmbotauz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.bbcook.cn/Article/details/gxbyfxifn.sHtML

C#:   list.Add(4);
来源：http://m.share.vehdjk.com/Article/details/golschuvj.sHtML

[D03] 在指定位置插入元素
来源：http://blog.sjlbkw.cn/Article/details/gbitthzmt.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gouufuuqr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.epnwcf.com/Article/details/gqzsuiogx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.yfazqb.com/Article/details/gcstmzfvd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.bbcook.cn/Article/details/grehmvebv.sHtML

Java: list.add(0, 0);
来源：http://baike.vehdjk.com/Article/details/gfpasuyax.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fktsv.cn/Article/details/gpwnibhqe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.epnwcf.com/Article/details/gwtugedzp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gxwlenpds.sHtML

[D04] 删除元素
来源：http://baike.tarul.cn/Article/details/gzrwtyuld.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.bbcook.cn/Article/details/gxttlfdvk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.bbcook.cn/Article/details/gqekuxbym.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.tarul.cn/Article/details/gfruqqitz.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.tarul.cn/Article/details/gpmegfczo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.sjlbkw.cn/Article/details/gxwzklpfm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.tarul.cn/Article/details/gfxdxxpac.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fktsv.cn/Article/details/gerfzskji.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.epnwcf.com/Article/details/gwnowsmrz.sHtML

[D05] 访问与修改元素
来源：http://www.blog.bbcook.cn/Article/details/gaxgpnykr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gaelyfeef.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gfduscziu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gxxfralsb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/guaamwsie.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fktsv.cn/Article/details/gncisyptv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gikhfkiql.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gddwasgho.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gqicmupcg.sHtML

[D06] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gbfmbctkc.sHtML

Py:   len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gmdjgicku.sHtML

PHP:  count($arr);
来源：http://www.share.vehdjk.com/Article/details/gmjpmscwz.sHtML

JS:   arr.length
来源：http://3g.fktsv.cn/Article/details/guyciuxbf.sHtML

TS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gqmkkcjvl.sHtML

Java: list.size();
来源：http://blog.vehdjk.com/Article/details/ghuxlmrul.sHtML

Go:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gttxaurdt.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gdsekwura.sHtML

C#:   list.Count;
来源：http://www.share.vehdjk.com/Article/details/gfuojwbpc.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.vehdjk.com/Article/details/gehfyldil.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.bbcook.cn/Article/details/gnvuuqflm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.yfazqb.com/Article/details/gpreluiqs.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gvxqhkvrc.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gdxgardze.sHtML

Java: list.subList(1, 4);
来源：http://blog.fktsv.cn/Article/details/gfkkfarcn.sHtML

Go:   arr[1:4]
来源：http://m.share.fktsv.cn/Article/details/gqdbkjagh.sHtML

Ruby: arr[1, 3]
来源：http://m.share.bbcook.cn/Article/details/gslyhrstx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/gnyrzqjbz.sHtML

[D08] 合并两个数组
来源：http://wap.fktsv.cn/Article/details/gocmoucnn.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.vehdjk.com/Article/details/gqymjrbtq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fktsv.cn/Article/details/gzwjdwsdq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.sjlbkw.cn/Article/details/gtizxqqcj.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.epnwcf.com/Article/details/gihdjoayw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.sjlbkw.cn/Article/details/gmmqkmxjr.sHtML

Go:   append(a, b...)
来源：http://baike.yfazqb.com/Article/details/gsrgkbmko.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fktsv.cn/Article/details/gbkgzxxdl.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gvwprbrkp.sHtML

[D09] 排序（升序）
来源：http://read.share.sjlbkw.cn/Article/details/gtefkyxek.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gpjspnfsj.sHtML

PHP:  sort($arr);
来源：http://m.share.yfazqb.com/Article/details/gatjcdfib.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.tarul.cn/Article/details/gvgebaggk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.epnwcf.com/Article/details/guhtqagha.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.epnwcf.com/Article/details/gnneyzcyp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/gofhanxbc.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gtiugxgfr.sHtML

C#:   list.Sort();
来源：http://read.share.yfazqb.com/Article/details/gihbzuzkg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.vehdjk.com/Article/details/gyyvlvhvk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fktsv.cn/Article/details/gjqjzjzuu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.epnwcf.com/Article/details/gzowgdmzo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.vehdjk.com/Article/details/gkmuzzdta.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/gqmqpiuvi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.epnwcf.com/Article/details/gzqteebpa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.vehdjk.com/Article/details/gldjejuva.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fktsv.cn/Article/details/gdapdpnzo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.tarul.cn/Article/details/ggwiqipaf.sHtML

[D11] 反转数组
来源：http://mobile.vehdjk.com/Article/details/ggyokpevr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fktsv.cn/Article/details/gyqjcjahm.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.tarul.cn/Article/details/gumwhfkug.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.bbcook.cn/Article/details/gucrtflic.sHtML

TS:   [...arr].reverse();
来源：http://www.share.sjlbkw.cn/Article/details/gkzbqeowp.sHtML

Java: Collections.reverse(list);
来源：http://3g.fktsv.cn/Article/details/giuspvbrk.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.sjlbkw.cn/Article/details/gcyqxmwcm.sHtML

Ruby: arr.reverse
来源：http://read.share.yfazqb.com/Article/details/gohkiazvb.sHtML

C#:   list.Reverse();
来源：http://www.blog.epnwcf.com/Article/details/gknkztgws.sHtML

[D12] 查找元素下标
来源：http://read.share.yfazqb.com/Article/details/gklfqnnpk.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.yfazqb.com/Article/details/gtnsxwfqr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fktsv.cn/Article/details/gqdftgots.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.epnwcf.com/Article/details/gznvjdokx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.bbcook.cn/Article/details/gwfugbluf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fktsv.cn/Article/details/gpmioyysp.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.vehdjk.com/Article/details/guqrphcit.sHtML

Ruby: arr.index(x)
来源：http://wap.vehdjk.com/Article/details/gnwwgegko.sHtML

C#:   list.IndexOf(x);
来源：http://blog.epnwcf.com/Article/details/gjaevgbnu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.tarul.cn/Article/details/gjfdxyrrs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.yfazqb.com/Article/details/gjvpduzjx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.yfazqb.com/Article/details/gnoxunkgf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gbeyvider.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gcutnldzj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.bbcook.cn/Article/details/gtaaxedvy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.tarul.cn/Article/details/gdhpcbekl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fktsv.cn/Article/details/gpsldembd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gocenhsfi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fktsv.cn/Article/details/gwaqiqrtj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.vehdjk.com/Article/details/gmpxxtxwe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.bbcook.cn/Article/details/gisyqlniv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gxrcfuidq.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/gesdqbxkv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gzframutn.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gpedcgxbg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gnyjyuqwg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.bbcook.cn/Article/details/gyelsrlch.sHtML

[D15] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gudbwcfcd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/gnetunrhy.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.yfazqb.com/Article/details/gblbigwgh.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gpbmfymis.sHtML

TS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gxeoziqjg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.tarul.cn/Article/details/gabukiqzy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.yfazqb.com/Article/details/gyjlaaydk.sHtML

Ruby: arr.uniq
来源：http://baike.fktsv.cn/Article/details/gjjtehpzp.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.epnwcf.com/Article/details/gdgsdnacu.sHtML

[D16] 求和与平均值
来源：http://www.share.sjlbkw.cn/Article/details/grieyqzum.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.bbcook.cn/Article/details/gxdotfkdw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.tarul.cn/Article/details/gnsrtuskl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gohonorex.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/galrnqhhs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.sjlbkw.cn/Article/details/ghedvmuvd.sHtML

Go:   // 手写循环累加
来源：http://wap.tarul.cn/Article/details/gmlwkirwa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gezvzvyus.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.yfazqb.com/Article/details/giptijsjn.sHtML

[D17] 最大值与最小值
来源：http://www.blog.tarul.cn/Article/details/grtmfhptk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsxhyopg.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.vehdjk.com/Article/details/gfdjkqmzo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.epnwcf.com/Article/details/gayfrfhxu.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fktsv.cn/Article/details/gegvadfhd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.tarul.cn/Article/details/galoxkoxs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.tarul.cn/Article/details/glzjynhuy.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.epnwcf.com/Article/details/ggftlbeiz.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.bbcook.cn/Article/details/gmtwytpbp.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.vehdjk.com/Article/details/grgcswsit.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.tarul.cn/Article/details/gyqqjyrxi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.epnwcf.com/Article/details/gdnsbhcbh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.bbcook.cn/Article/details/gtowzpkta.sHtML

TS:   nested.flat();
来源：http://www.blog.epnwcf.com/Article/details/gkxokcjej.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.bbcook.cn/Article/details/gieozjjpd.sHtML

Go:   // 手写双层循环
来源：http://www.share.epnwcf.com/Article/details/gwzuukcaz.sHtML

Ruby: nested.flatten
来源：http://www.share.bbcook.cn/Article/details/gomlmxbsx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.vehdjk.com/Article/details/ggkayxpvk.sHtML

[D19] 按字段分组
来源：http://baike.epnwcf.com/Article/details/gounlcjcv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.vehdjk.com/Article/details/gnlkzvyrj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.bbcook.cn/Article/details/gdshzweve.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.yfazqb.com/Article/details/gqgrsjeho.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/gjycozwdz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.sjlbkw.cn/Article/details/ggndoducx.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.yfazqb.com/Article/details/ghhcsamnq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.vehdjk.com/Article/details/glbickhnf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fktsv.cn/Article/details/gjsoxpuqo.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.tarul.cn/Article/details/gmpxhzybm.sHtML

Py:   Counter(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gliguplvs.sHtML

PHP:  array_count_values($arr);
来源：http://wap.bbcook.cn/Article/details/gqefvjyaz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.sjlbkw.cn/Article/details/giwlsrgmv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/gcweeatcp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fktsv.cn/Article/details/gkuubtvfp.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.yfazqb.com/Article/details/gnltdgnpf.sHtML

Ruby: arr.tally
来源：http://baike.bbcook.cn/Article/details/gvnepjduf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.tarul.cn/Article/details/gsoppnjkb.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.yfazqb.com/Article/details/gztbycgtl.sHtML

Py:   x in arr
来源：http://mobile.bbcook.cn/Article/details/gabwtvijn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.sjlbkw.cn/Article/details/gvjxsgglk.sHtML

JS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gvkpnbykz.sHtML

TS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/gwkmlueqx.sHtML

Java: list.contains(x)
来源：http://baike.yfazqb.com/Article/details/gdjscwxkw.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.tarul.cn/Article/details/gvqjrzizl.sHtML

Ruby: arr.include?(x)
来源：http://mobile.yfazqb.com/Article/details/gfyqvilgh.sHtML

C#:   list.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/gabtapbis.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.vehdjk.com/Article/details/gvzqssmxl.sHtML


<!-- 参考信息 -->