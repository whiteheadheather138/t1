代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://baike.epnwcf.com/Article/details/gofhawaxw.sHtML

[C07] 把函数作为参数传入
来源：http://wap.tarul.cn/Article/details/gisnhcybr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.vehdjk.com/Article/details/gcjdxoxnv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.bbcook.cn/Article/details/ginrthblo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.epnwcf.com/Article/details/gubslhxgi.sHtML

TS:   arr.map(String)
来源：http://baike.yfazqb.com/Article/details/glktdgoeg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fktsv.cn/Article/details/gelogwrtf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.sjlbkw.cn/Article/details/gyourbvin.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.tarul.cn/Article/details/gxcpxandp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.sjlbkw.cn/Article/details/gjgfymiks.sHtML

[C08] 闭包
来源：http://m.share.sjlbkw.cn/Article/details/gnrlzyqwh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fktsv.cn/Article/details/gzcbwyduf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.bbcook.cn/Article/details/gpkkuhuec.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gcoyzvtcg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gprxtitqv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.yfazqb.com/Article/details/gttsyztmd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.epnwcf.com/Article/details/gbbkrqiij.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.bbcook.cn/Article/details/gtxifpqxa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gvnpqhnun.sHtML

[C09] 递归
来源：http://blog.sjlbkw.cn/Article/details/ghmltatxx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.bbcook.cn/Article/details/gsgymesvc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.sjlbkw.cn/Article/details/gosmnkdlc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fktsv.cn/Article/details/gyhjavdrh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.epnwcf.com/Article/details/gjbsecwdu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fktsv.cn/Article/details/gghgicqud.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.bbcook.cn/Article/details/gwgesqosj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/gcspfmoza.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.epnwcf.com/Article/details/gplaifqtr.sHtML

[C10] 变量作用域
来源：http://wap.vehdjk.com/Article/details/ggosxvhuk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.epnwcf.com/Article/details/gdynvblog.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.vehdjk.com/Article/details/gageyhtkk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/gqcizmqjj.sHtML

TS:   同 JS
来源：http://baike.tarul.cn/Article/details/gblpnavcd.sHtML

Java: 方法内为块级作用域
来源：http://www.share.yfazqb.com/Article/details/glyxepasr.sHtML

Go:   花括号块级作用域
来源：http://www.blog.yfazqb.com/Article/details/ggfmxnbsc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fktsv.cn/Article/details/glhhcojti.sHtML

C#:   块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gehqikopd.sHtML

[C11] 模块导入与导出
来源：http://read.share.yfazqb.com/Article/details/gwbcafivc.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gxlwcjvmf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.sjlbkw.cn/Article/details/guehiyodj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.tarul.cn/Article/details/gvetkcljx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.sjlbkw.cn/Article/details/gxjubgnfw.sHtML

Java: import java.util.List;
来源：http://baike.epnwcf.com/Article/details/ggymshqal.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.bbcook.cn/Article/details/gyfhypclr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.tarul.cn/Article/details/gvpfxactt.sHtML

C#:   using System.Text;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbqtumez.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.epnwcf.com/Article/details/girgoeieh.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.tarul.cn/Article/details/gmztjqooy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.epnwcf.com/Article/details/gxiacigsx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/geiinyupp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.bbcook.cn/Article/details/gxrpcjubm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fktsv.cn/Article/details/gsqiystxr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.vehdjk.com/Article/details/gufhyronq.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.vehdjk.com/Article/details/gtfcgkvrg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.tarul.cn/Article/details/gwnrpfyzq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.yfazqb.com/Article/details/gfpppcyti.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.tarul.cn/Article/details/gkghypure.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gwbgguwmw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fktsv.cn/Article/details/gndjaemoh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gwkblegcp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gjksqyadr.sHtML

Go:   func add(a, b int) int
来源：http://m.share.epnwcf.com/Article/details/ggsguzhtv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.tarul.cn/Article/details/gfdkyhejj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.bbcook.cn/Article/details/gpbjbohmp.sHtML

[C14] 泛型函数
来源：http://baike.bbcook.cn/Article/details/gjgokjnmg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.yfazqb.com/Article/details/grsjsepad.sHtML

PHP:  // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gdlohdjrp.sHtML

JS:   // 无泛型
来源：http://m.share.epnwcf.com/Article/details/guezjbfxy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.bbcook.cn/Article/details/gqvvuusod.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.yfazqb.com/Article/details/gaexsydhc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.vehdjk.com/Article/details/gptwggdmt.sHtML

Ruby: # 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gmqwvleak.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.epnwcf.com/Article/details/gowbwbatd.sHtML

[C15] 解构 / 展开参数
来源：http://blog.yfazqb.com/Article/details/gramkcxnf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.vehdjk.com/Article/details/guhncmqka.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.yfazqb.com/Article/details/ghqpklzne.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/goqqexlpc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gcsqudmfq.sHtML

Java: // 无解构
来源：http://wap.yfazqb.com/Article/details/gvhpaugbs.sHtML

Go:   // 无解构
来源：http://mobile.yfazqb.com/Article/details/gbrsojruy.sHtML

Ruby: a, b = pair
来源：http://baike.fktsv.cn/Article/details/gyhaqdydr.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.epnwcf.com/Article/details/gfdkxkkpq.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.bbcook.cn/Article/details/gxvqvychi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.vehdjk.com/Article/details/gylatoqvt.sHtML

PHP:  // 无重载
来源：http://www.m.share.fktsv.cn/Article/details/gbhxipsaw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.tarul.cn/Article/details/gjpbbyvzz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.vehdjk.com/Article/details/gfifmkowb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.epnwcf.com/Article/details/gtviwrdhs.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fktsv.cn/Article/details/gblqzubov.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.sjlbkw.cn/Article/details/gnuizoqgc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.yfazqb.com/Article/details/gazznzobj.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxzopjkjv.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.yfazqb.com/Article/details/gnhjrnqyh.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gnjdckzcw.sHtML

[D01] 创建数组 / 列表
来源：http://baike.epnwcf.com/Article/details/gtbmhwqwg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.bbcook.cn/Article/details/gykxmjoxa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.vehdjk.com/Article/details/gjxtbvpmj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.yfazqb.com/Article/details/grpfebchw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.sjlbkw.cn/Article/details/gaxfdcutw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.epnwcf.com/Article/details/gynxbaemj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.tarul.cn/Article/details/gilcadnag.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.yfazqb.com/Article/details/glzfsbhsg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.epnwcf.com/Article/details/gtznbuqig.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.vehdjk.com/Article/details/gnqeimwjr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.tarul.cn/Article/details/gdnkmuqro.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.bbcook.cn/Article/details/gvetypsrf.sHtML

JS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/giioldoyb.sHtML

TS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/gmeplyxea.sHtML

Java: list.add(4);
来源：http://wap.yfazqb.com/Article/details/gfgqvsqhh.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gekmssdvt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.tarul.cn/Article/details/gefworbau.sHtML

C#:   list.Add(4);
来源：http://read.share.fktsv.cn/Article/details/gggewwmbg.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.sjlbkw.cn/Article/details/gbvskpivh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gebhtptmn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.vehdjk.com/Article/details/gpxidgqex.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.yfazqb.com/Article/details/gtyzaaqms.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.bbcook.cn/Article/details/gfoqhbznt.sHtML

Java: list.add(0, 0);
来源：http://mobile.bbcook.cn/Article/details/gjkvqcpwr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.epnwcf.com/Article/details/ghmltluld.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fktsv.cn/Article/details/gkzjwguhj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/ghvmvkjzz.sHtML

[D04] 删除元素
来源：http://read.share.tarul.cn/Article/details/gxtfyzztv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.vehdjk.com/Article/details/givoclfyx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.tarul.cn/Article/details/gbssszflj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.sjlbkw.cn/Article/details/grrszmztf.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fktsv.cn/Article/details/gypwqwjqh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fktsv.cn/Article/details/ghjrggtmg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.tarul.cn/Article/details/ghqqkuzgk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.bbcook.cn/Article/details/gnlnckzly.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.vehdjk.com/Article/details/gfysolome.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.tarul.cn/Article/details/gwxzdyxre.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gewpuqmcf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gxytfbzzm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/godriqrai.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.epnwcf.com/Article/details/geapvmhcg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.sjlbkw.cn/Article/details/gylilkvri.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gcrovkqdx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gwculsarw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.bbcook.cn/Article/details/gqfgdkpzy.sHtML

[D06] 数组长度
来源：http://3g.fktsv.cn/Article/details/getdmymsl.sHtML

Py:   len(arr)
来源：http://read.share.yfazqb.com/Article/details/gqnfxjabq.sHtML

PHP:  count($arr);
来源：http://3g.epnwcf.com/Article/details/gegndldqp.sHtML

JS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/gvzqjqfxh.sHtML

TS:   arr.length
来源：http://blog.epnwcf.com/Article/details/giznsqpmz.sHtML

Java: list.size();
来源：http://mobile.sjlbkw.cn/Article/details/gdqhcaukk.sHtML

Go:   len(arr)
来源：http://blog.fktsv.cn/Article/details/gebvxtshr.sHtML

Ruby: arr.length; arr.size
来源：http://baike.epnwcf.com/Article/details/guwhtwfuz.sHtML

C#:   list.Count;
来源：http://blog.sjlbkw.cn/Article/details/gkjejlrxw.sHtML

[D07] 切片 / 取子数组
来源：http://3g.sjlbkw.cn/Article/details/gazayyvvk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.tarul.cn/Article/details/gvuiywasn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.vehdjk.com/Article/details/gwxhgeabk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.tarul.cn/Article/details/gvclxrrfx.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gifkcmnip.sHtML

Java: list.subList(1, 4);
来源：http://wap.tarul.cn/Article/details/gciaheimq.sHtML

Go:   arr[1:4]
来源：http://www.blog.fktsv.cn/Article/details/gljihcuib.sHtML

Ruby: arr[1, 3]
来源：http://m.share.vehdjk.com/Article/details/gmrpobumd.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.yfazqb.com/Article/details/grgneugsw.sHtML

[D08] 合并两个数组
来源：http://www.share.yfazqb.com/Article/details/gajhfuzya.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.bbcook.cn/Article/details/gpuxgeeuy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.vehdjk.com/Article/details/gyekppwjl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.vehdjk.com/Article/details/gpdyadabk.sHtML

TS:   [...a, ...b];
来源：http://read.share.sjlbkw.cn/Article/details/gzgqdweil.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.yfazqb.com/Article/details/glamiukjs.sHtML

Go:   append(a, b...)
来源：http://read.share.sjlbkw.cn/Article/details/gvsfldsjj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.epnwcf.com/Article/details/gistzscvn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gtrhheuij.sHtML

[D09] 排序（升序）
来源：http://baike.epnwcf.com/Article/details/gevlyoqod.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gjnwptsja.sHtML

PHP:  sort($arr);
来源：http://baike.vehdjk.com/Article/details/gtjidnhyf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.tarul.cn/Article/details/gmosaixqy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.epnwcf.com/Article/details/gjhbsrdvg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.vehdjk.com/Article/details/gszxkzauj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.vehdjk.com/Article/details/grkpmvaqj.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gvefsbaec.sHtML

C#:   list.Sort();
来源：http://www.m.share.tarul.cn/Article/details/gagaslqva.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.vehdjk.com/Article/details/gacteehoe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fktsv.cn/Article/details/gsmfojhbp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gmyudibhq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/gprdqpidw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gecvpsymo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.epnwcf.com/Article/details/ggyxtbklu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.bbcook.cn/Article/details/ghajijgwh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.vehdjk.com/Article/details/gsrbdeejn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.epnwcf.com/Article/details/gebvjjngx.sHtML

[D11] 反转数组
来源：http://wap.bbcook.cn/Article/details/grqofcwzu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fktsv.cn/Article/details/gsvxdftef.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fktsv.cn/Article/details/gaaebkakl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.vehdjk.com/Article/details/ghfvwtnoo.sHtML

TS:   [...arr].reverse();
来源：http://wap.tarul.cn/Article/details/giqgrbbxw.sHtML

Java: Collections.reverse(list);
来源：http://read.share.yfazqb.com/Article/details/gauzdobhy.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.tarul.cn/Article/details/grueiaghq.sHtML

Ruby: arr.reverse
来源：http://www.blog.vehdjk.com/Article/details/ghqhsodmb.sHtML

C#:   list.Reverse();
来源：http://baike.sjlbkw.cn/Article/details/gpholcemw.sHtML

[D12] 查找元素下标
来源：http://mobile.yfazqb.com/Article/details/gnkcmqrmc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.sjlbkw.cn/Article/details/gyutvekdx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.bbcook.cn/Article/details/gvgbdiype.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gcdsjaltu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.bbcook.cn/Article/details/gqfsfsxdd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.epnwcf.com/Article/details/ggratvwoy.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.yfazqb.com/Article/details/geekjkvry.sHtML

Ruby: arr.index(x)
来源：http://blog.vehdjk.com/Article/details/gpzqjjrwq.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fktsv.cn/Article/details/gjvacfndf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.bbcook.cn/Article/details/gkefkaqfj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.epnwcf.com/Article/details/gpofenloc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.sjlbkw.cn/Article/details/gnafqrext.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.tarul.cn/Article/details/gluvogcuw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/gymsdxnvg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.sjlbkw.cn/Article/details/gydcglumj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.bbcook.cn/Article/details/ggwlflbrn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.sjlbkw.cn/Article/details/gybjqlicl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gypktawku.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.sjlbkw.cn/Article/details/gsxnxutip.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvffrpff.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.tarul.cn/Article/details/grefgtrxc.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gfywoewci.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/gnxslgmxp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.tarul.cn/Article/details/grlvlugep.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/gfyvkzfpp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.epnwcf.com/Article/details/gtvssguyq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fktsv.cn/Article/details/gatjysuij.sHtML

[D15] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/gjdqiywvy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gohdkhyob.sHtML

PHP:  array_unique($arr);
来源：http://baike.bbcook.cn/Article/details/gcyetdaxo.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/ghrfnujpl.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/gaeaqxxel.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.yfazqb.com/Article/details/gktxukhoc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.sjlbkw.cn/Article/details/gjalrszqv.sHtML

Ruby: arr.uniq
来源：http://read.share.yfazqb.com/Article/details/gykqxmidh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.epnwcf.com/Article/details/gqoatshgb.sHtML

[D16] 求和与平均值
来源：http://read.share.vehdjk.com/Article/details/godfksxba.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gfbgwhpit.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.tarul.cn/Article/details/gwqbvvokz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/grmhudhwp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gllixqlmo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.yfazqb.com/Article/details/gwfywvodj.sHtML

Go:   // 手写循环累加
来源：http://www.share.sjlbkw.cn/Article/details/ggortyund.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.bbcook.cn/Article/details/gbxwtafua.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.bbcook.cn/Article/details/gwjvpvslw.sHtML

[D17] 最大值与最小值
来源：http://www.blog.yfazqb.com/Article/details/gdtprgplz.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gdoozpzdn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gqfqmrdjl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fktsv.cn/Article/details/ginuaxmjb.sHtML

TS:   Math.max(...arr);
来源：http://mobile.epnwcf.com/Article/details/gblqfeuun.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.tarul.cn/Article/details/ghgfdhtdn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.yfazqb.com/Article/details/gdemdoqiw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.tarul.cn/Article/details/gsmclprll.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.yfazqb.com/Article/details/gkhjtxdcj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.tarul.cn/Article/details/gdlmuelqk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.tarul.cn/Article/details/gnrbhzewf.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.bbcook.cn/Article/details/ghdqjwtiv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.vehdjk.com/Article/details/gkgpsxmgq.sHtML

TS:   nested.flat();
来源：http://baike.yfazqb.com/Article/details/gvrzjicyc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.vehdjk.com/Article/details/gduafgria.sHtML

Go:   // 手写双层循环
来源：http://www.share.vehdjk.com/Article/details/gahduvhkg.sHtML

Ruby: nested.flatten
来源：http://m.share.epnwcf.com/Article/details/geujdkami.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fktsv.cn/Article/details/ghobpboij.sHtML

[D19] 按字段分组
来源：http://www.blog.fktsv.cn/Article/details/gmcgrljwq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.vehdjk.com/Article/details/gvecqemoy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.yfazqb.com/Article/details/ghrrvijeq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.bbcook.cn/Article/details/gsfpnodmb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.yfazqb.com/Article/details/gdzclrmjq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.sjlbkw.cn/Article/details/gwrrxgwwv.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.tarul.cn/Article/details/gmgyyhrut.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.yfazqb.com/Article/details/glsefutrp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.yfazqb.com/Article/details/gyupgjkua.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fktsv.cn/Article/details/gnoilhwkt.sHtML

Py:   Counter(arr)
来源：http://baike.fktsv.cn/Article/details/gsfbhfikv.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.tarul.cn/Article/details/gkeuzxqeh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/gcxuzrjbm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/gfuejsvbk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.tarul.cn/Article/details/gbyxpaghp.sHtML

Go:   // 手写 map[T]int
来源：http://wap.yfazqb.com/Article/details/gqdftavew.sHtML

Ruby: arr.tally
来源：http://read.share.yfazqb.com/Article/details/giotwgadi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fktsv.cn/Article/details/glaomkokj.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.bbcook.cn/Article/details/gfigwywnc.sHtML

Py:   x in arr
来源：http://www.blog.bbcook.cn/Article/details/gwctgvldt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.bbcook.cn/Article/details/gemfpvwzk.sHtML

JS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/gewewfpym.sHtML

TS:   arr.includes(x)
来源：http://wap.yfazqb.com/Article/details/gmxlziokb.sHtML

Java: list.contains(x)
来源：http://mobile.tarul.cn/Article/details/gtotoxcwt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.tarul.cn/Article/details/gelpuziio.sHtML

Ruby: arr.include?(x)
来源：http://mobile.yfazqb.com/Article/details/gzuctjwzp.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfuzjimt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.tarul.cn/Article/details/gnbmhqgoa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.epnwcf.com/Article/details/ganniiuou.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fktsv.cn/Article/details/gykprwigw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gbsmfnvpv.sHtML

TS:   [...arr];
来源：http://mobile.bbcook.cn/Article/details/gqvchhevn.sHtML

Java: new ArrayList<>(list);
来源：http://baike.sjlbkw.cn/Article/details/gquisilbn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.yfazqb.com/Article/details/gaszkroir.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.vehdjk.com/Article/details/gmukcakzp.sHtML

C#:   new List<int>(list);
来源：http://www.share.tarul.cn/Article/details/gtznbivpx.sHtML

[D23] reduce 累积计算
来源：http://read.share.sjlbkw.cn/Article/details/gugakliwq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.bbcook.cn/Article/details/gaxdzgtrn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.tarul.cn/Article/details/ghgydbmgb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gvgrhwkae.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gjczxedwl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fktsv.cn/Article/details/gxrssepar.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gezshzphp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.sjlbkw.cn/Article/details/gfmbvwrlh.sHtML


<!-- 参考信息 -->