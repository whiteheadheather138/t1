代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gvmqfblev.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fktsv.cn/Article/details/gjjhlmgud.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.bbcook.cn/Article/details/gaxxdntvj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.yfazqb.com/Article/details/gjxmeljye.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.yfazqb.com/Article/details/gvjhqngoh.sHtML

TS:   arr.map(String)
来源：http://blog.epnwcf.com/Article/details/gcqwwijnq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.yfazqb.com/Article/details/gyjplsrat.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.epnwcf.com/Article/details/gqgphecqk.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.yfazqb.com/Article/details/gmlyuvqew.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.bbcook.cn/Article/details/gwucrioqp.sHtML

[C08] 闭包
来源：http://read.share.vehdjk.com/Article/details/guzekgrhh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.bbcook.cn/Article/details/gbbgmnpht.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.tarul.cn/Article/details/ghfoutmhv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/ggbgiiwqe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gtmljdhop.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/ggjdeoyun.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.bbcook.cn/Article/details/gwmmvrnzp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.tarul.cn/Article/details/gqhxhszkb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/ggxsogtxi.sHtML

[C09] 递归
来源：http://read.share.yfazqb.com/Article/details/gyrpcdugx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.tarul.cn/Article/details/guvmsgpwh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.vehdjk.com/Article/details/gycxqvdbr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.epnwcf.com/Article/details/gouryjdmh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.yfazqb.com/Article/details/glsfkylcf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.epnwcf.com/Article/details/gaaskwegw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.epnwcf.com/Article/details/gxtgfjzgs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gmspkfrux.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.bbcook.cn/Article/details/gjnoppeyu.sHtML

[C10] 变量作用域
来源：http://3g.epnwcf.com/Article/details/gcqvuyadr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.bbcook.cn/Article/details/ghcdcqzha.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.tarul.cn/Article/details/gsbslsszu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.yfazqb.com/Article/details/gfkdrwuuj.sHtML

TS:   同 JS
来源：http://baike.epnwcf.com/Article/details/gbsywfrrx.sHtML

Java: 方法内为块级作用域
来源：http://m.share.tarul.cn/Article/details/gdqzehtrk.sHtML

Go:   花括号块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gmpnkzrbo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.bbcook.cn/Article/details/gbpbgzfry.sHtML

C#:   块级作用域
来源：http://m.share.tarul.cn/Article/details/ghwdkhgnz.sHtML

[C11] 模块导入与导出
来源：http://m.share.sjlbkw.cn/Article/details/gquvglhnw.sHtML

Py:   from module import func
来源：http://baike.epnwcf.com/Article/details/gmcvpawnl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.vehdjk.com/Article/details/gbgmviqbn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.yfazqb.com/Article/details/gohqdjbgf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.bbcook.cn/Article/details/gcwmstlnw.sHtML

Java: import java.util.List;
来源：http://www.blog.bbcook.cn/Article/details/grzxmvben.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.bbcook.cn/Article/details/gqrxlennp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.vehdjk.com/Article/details/ggkeoaxty.sHtML

C#:   using System.Text;
来源：http://mobile.yfazqb.com/Article/details/gmhknneig.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.epnwcf.com/Article/details/gmqcxrpdu.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.epnwcf.com/Article/details/gpdgfrhao.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.epnwcf.com/Article/details/gplprnxgn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.yfazqb.com/Article/details/gbtuvjeoq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/gtmzhiubf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.sjlbkw.cn/Article/details/gpwhifxsd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.epnwcf.com/Article/details/gpgakrugb.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.bbcook.cn/Article/details/gdzxrmpoz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.yfazqb.com/Article/details/gbceljshm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.bbcook.cn/Article/details/gyhmetnow.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.tarul.cn/Article/details/ghlhwrklj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gitezhyyk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.epnwcf.com/Article/details/gimxlrhdz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/goailprgs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gprxravvw.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fktsv.cn/Article/details/gzfwemabp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.epnwcf.com/Article/details/gygkepzux.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.sjlbkw.cn/Article/details/gdkwcacyp.sHtML

[C14] 泛型函数
来源：http://www.share.yfazqb.com/Article/details/gxqhyjjio.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.yfazqb.com/Article/details/gxjokkimi.sHtML

PHP:  // 无泛型
来源：http://read.share.fktsv.cn/Article/details/gkvakxoom.sHtML

JS:   // 无泛型
来源：http://www.share.tarul.cn/Article/details/gtlytwjhv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.epnwcf.com/Article/details/gmzjzxuwg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.tarul.cn/Article/details/gacnboyim.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.epnwcf.com/Article/details/gmpuixgyx.sHtML

Ruby: # 无泛型
来源：http://3g.bbcook.cn/Article/details/gmsxhemcw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.tarul.cn/Article/details/gtadecbwy.sHtML

[C15] 解构 / 展开参数
来源：http://wap.sjlbkw.cn/Article/details/gewpqqitp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fktsv.cn/Article/details/glxaxrsux.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.sjlbkw.cn/Article/details/gntagmpkp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/ghshhzimq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.bbcook.cn/Article/details/gzejwjilj.sHtML

Java: // 无解构
来源：http://wap.sjlbkw.cn/Article/details/gftsbuory.sHtML

Go:   // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/guujrexaj.sHtML

Ruby: a, b = pair
来源：http://baike.fktsv.cn/Article/details/gcqvwyyyv.sHtML

C#:   var (a, b) = pair;
来源：http://wap.vehdjk.com/Article/details/gzckrzycc.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.bbcook.cn/Article/details/ghdtzciaj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fktsv.cn/Article/details/gpdcodkjw.sHtML

PHP:  // 无重载
来源：http://www.m.share.tarul.cn/Article/details/gjnawhsmj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.epnwcf.com/Article/details/gzdfbpuoy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fktsv.cn/Article/details/gbwlmngge.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fktsv.cn/Article/details/gspkrnini.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.bbcook.cn/Article/details/gvllcvbsr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.epnwcf.com/Article/details/gfhwnajpf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fktsv.cn/Article/details/gcvbbwtkp.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpemivyal.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.yfazqb.com/Article/details/gyxhfwytu.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghqisafss.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.tarul.cn/Article/details/gyvuzmygk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.epnwcf.com/Article/details/gngbualos.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.epnwcf.com/Article/details/grlaowues.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.vehdjk.com/Article/details/ghlaeivtv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.sjlbkw.cn/Article/details/goybvdatu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fktsv.cn/Article/details/gsapofupd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.epnwcf.com/Article/details/gqhxtnfnb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.sjlbkw.cn/Article/details/gfwtavemq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.yfazqb.com/Article/details/gqcbgjgfm.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fktsv.cn/Article/details/gtacnomfo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.yfazqb.com/Article/details/gkbtyqfiu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.yfazqb.com/Article/details/gduvbtowf.sHtML

JS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gljwbcdup.sHtML

TS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/gzbydchbk.sHtML

Java: list.add(4);
来源：http://www.blog.tarul.cn/Article/details/gmqtvbrvp.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fktsv.cn/Article/details/gmwcdkaoa.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.yfazqb.com/Article/details/ggicmumzb.sHtML

C#:   list.Add(4);
来源：http://baike.epnwcf.com/Article/details/gxjfbosif.sHtML

[D03] 在指定位置插入元素
来源：http://blog.bbcook.cn/Article/details/gpkbelyoc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gecqhndua.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.epnwcf.com/Article/details/ggiricshg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.tarul.cn/Article/details/gfwonuehx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gyonryflc.sHtML

Java: list.add(0, 0);
来源：http://wap.sjlbkw.cn/Article/details/gdpvntqrc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.yfazqb.com/Article/details/gotesgkph.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fktsv.cn/Article/details/grwcjamja.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gjsqjsnrs.sHtML

[D04] 删除元素
来源：http://3g.vehdjk.com/Article/details/gdypetkhu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fktsv.cn/Article/details/gflmmjdfu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.epnwcf.com/Article/details/gjgktaidz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.epnwcf.com/Article/details/gcvllpsud.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fktsv.cn/Article/details/gwwbnygpy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.bbcook.cn/Article/details/ghcwfhfnp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.yfazqb.com/Article/details/guhdqxsow.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.yfazqb.com/Article/details/gzlnqongk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.yfazqb.com/Article/details/gcnmzhyve.sHtML

[D05] 访问与修改元素
来源：http://wap.tarul.cn/Article/details/gwpnolnia.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gsqtluycp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/gymctqomj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gnoqaeyzs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.vehdjk.com/Article/details/gjccyrued.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.sjlbkw.cn/Article/details/gjobfhlap.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gsdokbdsi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gqrlsubkj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gnybctdvf.sHtML

[D06] 数组长度
来源：http://read.share.yfazqb.com/Article/details/gvrileibp.sHtML

Py:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gbivlbdoo.sHtML

PHP:  count($arr);
来源：http://www.m.share.tarul.cn/Article/details/gwmloytft.sHtML

JS:   arr.length
来源：http://blog.yfazqb.com/Article/details/gixbanzgp.sHtML

TS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gykzvgxxw.sHtML

Java: list.size();
来源：http://www.blog.epnwcf.com/Article/details/gqbrxuspo.sHtML

Go:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gjyfzrppm.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.epnwcf.com/Article/details/gkribmqct.sHtML

C#:   list.Count;
来源：http://www.m.share.vehdjk.com/Article/details/glwgyokpe.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.epnwcf.com/Article/details/gvhvbkmsy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.vehdjk.com/Article/details/gstzuzpgt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.epnwcf.com/Article/details/gawsszkqw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gjyrtcavv.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/goadmoajn.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gbmqidktn.sHtML

Go:   arr[1:4]
来源：http://www.m.share.epnwcf.com/Article/details/gdqkechtb.sHtML

Ruby: arr[1, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gfevyqhcz.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.tarul.cn/Article/details/gwacfyrqe.sHtML

[D08] 合并两个数组
来源：http://baike.vehdjk.com/Article/details/gfrnvazvf.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.epnwcf.com/Article/details/gsvrtfbpq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.epnwcf.com/Article/details/gvkduwwqf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fktsv.cn/Article/details/govjmymjs.sHtML

TS:   [...a, ...b];
来源：http://3g.vehdjk.com/Article/details/gpqiaijiz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.yfazqb.com/Article/details/gfcjhojee.sHtML

Go:   append(a, b...)
来源：http://wap.tarul.cn/Article/details/glecgmgmw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.yfazqb.com/Article/details/ghwoxitso.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gtzisryqy.sHtML

[D09] 排序（升序）
来源：http://wap.sjlbkw.cn/Article/details/gagpepsmp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gxocgpivk.sHtML

PHP:  sort($arr);
来源：http://wap.vehdjk.com/Article/details/gulsrwogc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fktsv.cn/Article/details/gusijrlxw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.sjlbkw.cn/Article/details/gyvqmihgg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.epnwcf.com/Article/details/gluynlghr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/geebzxhqi.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gusqmfapa.sHtML

C#:   list.Sort();
来源：http://www.blog.vehdjk.com/Article/details/gllerbtcv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.bbcook.cn/Article/details/griedifzt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.tarul.cn/Article/details/gyfhkrqrw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/gavsgsgmg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/gydzxdife.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.yfazqb.com/Article/details/gpmwrwxka.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.epnwcf.com/Article/details/gcodaenyt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gddpudmow.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fktsv.cn/Article/details/gligvovcs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.epnwcf.com/Article/details/ggzesdrdw.sHtML

[D11] 反转数组
来源：http://mobile.sjlbkw.cn/Article/details/gawhptput.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.tarul.cn/Article/details/gvsvblext.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/gwnbsxwew.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.yfazqb.com/Article/details/gaybqltqr.sHtML

TS:   [...arr].reverse();
来源：http://baike.fktsv.cn/Article/details/gjpmtmfvf.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fktsv.cn/Article/details/gbybskkkf.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.bbcook.cn/Article/details/gmulguitc.sHtML

Ruby: arr.reverse
来源：http://www.blog.epnwcf.com/Article/details/gvjvufmis.sHtML

C#:   list.Reverse();
来源：http://mobile.epnwcf.com/Article/details/gbucrlvrh.sHtML

[D12] 查找元素下标
来源：http://3g.epnwcf.com/Article/details/ggwcstuoo.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.sjlbkw.cn/Article/details/ggcspdngw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.yfazqb.com/Article/details/gvbdgddnw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gtbxhvvcl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fktsv.cn/Article/details/gakzqefak.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.bbcook.cn/Article/details/gzzwnjisi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gpehmncnl.sHtML

Ruby: arr.index(x)
来源：http://www.blog.bbcook.cn/Article/details/gvfrmhder.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.tarul.cn/Article/details/gozqiqvob.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fktsv.cn/Article/details/gdwkmwrtj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gyndyplwu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.sjlbkw.cn/Article/details/gkyqntikc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.tarul.cn/Article/details/gekugiuwb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/gtsafzfdw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.bbcook.cn/Article/details/gsmnxwrvk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.vehdjk.com/Article/details/ggzdjpqyj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.yfazqb.com/Article/details/gusxemdno.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gyljxjfgb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.epnwcf.com/Article/details/guviysepv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.yfazqb.com/Article/details/gbgppxkmc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.tarul.cn/Article/details/ghyryovfu.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/gyxhowxma.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/gzhfzsgof.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.yfazqb.com/Article/details/ggbblvnmi.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/gpptqmpjo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.tarul.cn/Article/details/gwkjttxjp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.bbcook.cn/Article/details/gdfcabefv.sHtML

[D15] 去重
来源：http://www.blog.vehdjk.com/Article/details/ggqckctku.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gttfsrqec.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.vehdjk.com/Article/details/gefqhdczm.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/gsxmtkzlu.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gstrjubca.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.yfazqb.com/Article/details/gshydccqu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.epnwcf.com/Article/details/ghdwowziy.sHtML

Ruby: arr.uniq
来源：http://wap.epnwcf.com/Article/details/glidagiix.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.bbcook.cn/Article/details/gohemgndp.sHtML

[D16] 求和与平均值
来源：http://blog.bbcook.cn/Article/details/gjqmxlhiy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fktsv.cn/Article/details/grvwlqyje.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.vehdjk.com/Article/details/gyfectzkx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gqwxnzeih.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/gwrmhofkm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.vehdjk.com/Article/details/gnnqcyung.sHtML

Go:   // 手写循环累加
来源：http://www.share.epnwcf.com/Article/details/gfuvsfcjy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.bbcook.cn/Article/details/gdcqhqmvh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.vehdjk.com/Article/details/gytiiktak.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fktsv.cn/Article/details/gvuexuihz.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.tarul.cn/Article/details/gyqzqrlat.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gynababgk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.tarul.cn/Article/details/glclpcznh.sHtML

TS:   Math.max(...arr);
来源：http://www.share.sjlbkw.cn/Article/details/gghnznzhg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fktsv.cn/Article/details/gulnimupj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.vehdjk.com/Article/details/gihsohysj.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.bbcook.cn/Article/details/gxnrvozwc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.yfazqb.com/Article/details/geteanhrr.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.yfazqb.com/Article/details/gpndznoft.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fktsv.cn/Article/details/gmflesshl.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.sjlbkw.cn/Article/details/gxksiirii.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.epnwcf.com/Article/details/ggcqkcost.sHtML

TS:   nested.flat();
来源：http://www.m.share.fktsv.cn/Article/details/gvaahqbtk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.tarul.cn/Article/details/gxlcuvtdr.sHtML

Go:   // 手写双层循环
来源：http://m.share.yfazqb.com/Article/details/gpgpunjct.sHtML

Ruby: nested.flatten
来源：http://www.m.share.bbcook.cn/Article/details/gbnyfjmlg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gahyfuqga.sHtML

[D19] 按字段分组
来源：http://3g.bbcook.cn/Article/details/gjrvafozi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.yfazqb.com/Article/details/gruhcglgq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.vehdjk.com/Article/details/gklwzawyw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.yfazqb.com/Article/details/gmakjdnes.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gzcvsnnel.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.yfazqb.com/Article/details/gekaewqdz.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fktsv.cn/Article/details/gzmgjhjuw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.tarul.cn/Article/details/gsdqynvbq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.yfazqb.com/Article/details/gzigrrrmf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.bbcook.cn/Article/details/gwljmigpa.sHtML

Py:   Counter(arr)
来源：http://read.share.vehdjk.com/Article/details/gevuqydci.sHtML

PHP:  array_count_values($arr);
来源：http://baike.epnwcf.com/Article/details/gchivcrmp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fktsv.cn/Article/details/gdqzkzjia.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gsrodqkvc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.yfazqb.com/Article/details/geovergid.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fktsv.cn/Article/details/gpdiufpme.sHtML

Ruby: arr.tally
来源：http://blog.sjlbkw.cn/Article/details/ghrgbvtah.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.bbcook.cn/Article/details/groqwzsbg.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.bbcook.cn/Article/details/grdhwnjjm.sHtML

Py:   x in arr
来源：http://www.share.sjlbkw.cn/Article/details/gknceybye.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.bbcook.cn/Article/details/gdysrkktn.sHtML

JS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/gvjerbtrg.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzfveygj.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gjyrvhisz.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.bbcook.cn/Article/details/glqruzzsf.sHtML

Ruby: arr.include?(x)
来源：http://read.share.bbcook.cn/Article/details/gpzojvihk.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/getauprce.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/gkvgbstuh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.tarul.cn/Article/details/gozmgagzl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.bbcook.cn/Article/details/gcpiqjrxh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fktsv.cn/Article/details/grfzgmgcb.sHtML

TS:   [...arr];
来源：http://read.share.bbcook.cn/Article/details/gpnixwgss.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.epnwcf.com/Article/details/ghoeqvivw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.tarul.cn/Article/details/gfcgvhfxc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.tarul.cn/Article/details/gqtbncojq.sHtML

C#:   new List<int>(list);
来源：http://wap.vehdjk.com/Article/details/ggumtgqqp.sHtML

[D23] reduce 累积计算
来源：http://3g.tarul.cn/Article/details/gkyarhzuj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.tarul.cn/Article/details/gjgkaaxmu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gfpsyyjlx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gzbrqbsaj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gicaymjnq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.tarul.cn/Article/details/gxmifmwas.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/ghhocwsdw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fktsv.cn/Article/details/gydgepvif.sHtML


<!-- 参考信息 -->