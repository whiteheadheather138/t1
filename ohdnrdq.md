代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.sjlbkw.cn/Article/details/gvrifzzgj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/gcokmyiij.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.yfazqb.com/Article/details/gxwuracko.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.vehdjk.com/Article/details/gqhujbkhn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.epnwcf.com/Article/details/gzykwzmdk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fktsv.cn/Article/details/grocnibxe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.yfazqb.com/Article/details/gutuyrsha.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.yfazqb.com/Article/details/gixledcag.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.tarul.cn/Article/details/gjzfpmumy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gkqqrtjao.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.yfazqb.com/Article/details/gufwykdtz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fktsv.cn/Article/details/gswlqprnx.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.vehdjk.com/Article/details/gcmshoyrl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gufglifso.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gvudbsega.sHtML

[C05] 返回多个值
来源：http://3g.epnwcf.com/Article/details/gjumotosv.sHtML

Py:   return a, b
来源：http://www.share.fktsv.cn/Article/details/garufgwdy.sHtML

PHP:  return [$a, $b];
来源：http://wap.bbcook.cn/Article/details/gsdeakbwl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fktsv.cn/Article/details/gcsgsvrbb.sHtML

TS:   return { a, b };
来源：http://mobile.vehdjk.com/Article/details/gmrbauotv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.tarul.cn/Article/details/gpjmtjuln.sHtML

Go:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gtfozcwav.sHtML

Ruby: return a, b
来源：http://www.blog.yfazqb.com/Article/details/gymtfhthg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.sjlbkw.cn/Article/details/gelidsybi.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.vehdjk.com/Article/details/gdixyhmrt.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.tarul.cn/Article/details/gorlolebk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fktsv.cn/Article/details/gsjbcsqai.sHtML

JS:   const square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/geemquwkf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.vehdjk.com/Article/details/gcgcplwxq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.epnwcf.com/Article/details/gpjluzqeg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.epnwcf.com/Article/details/gnugrenyp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.bbcook.cn/Article/details/gfchldlje.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/guodzrckd.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.bbcook.cn/Article/details/gbgoebsnu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fktsv.cn/Article/details/ghrkwylxr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fktsv.cn/Article/details/gmofeqyue.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.epnwcf.com/Article/details/ghcfonhyt.sHtML

TS:   arr.map(String)
来源：http://m.share.sjlbkw.cn/Article/details/gdyuzwtyb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.yfazqb.com/Article/details/gambjbyfa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.vehdjk.com/Article/details/gincqphya.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.vehdjk.com/Article/details/gwbaiyhej.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.bbcook.cn/Article/details/gamirgeqx.sHtML

[C08] 闭包
来源：http://www.m.share.vehdjk.com/Article/details/gmmaccufs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.bbcook.cn/Article/details/gnsbwwpef.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.tarul.cn/Article/details/grhosghlz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gxbvbqpft.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gtetcucff.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fktsv.cn/Article/details/gzitsmemv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fktsv.cn/Article/details/gpliwcoct.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.vehdjk.com/Article/details/gwxjwzwtn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/graqthphu.sHtML

[C09] 递归
来源：http://3g.epnwcf.com/Article/details/gktspbdsk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/gjeaqyqgc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.bbcook.cn/Article/details/gxydkerrd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.sjlbkw.cn/Article/details/gqklntrnd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/gdkhmeurp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fktsv.cn/Article/details/gbtrochen.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.tarul.cn/Article/details/gwcznfijc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/ggosqbcxa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.sjlbkw.cn/Article/details/gkxnjhoac.sHtML

[C10] 变量作用域
来源：http://baike.sjlbkw.cn/Article/details/gxfmbdtwn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.epnwcf.com/Article/details/gzqdhcvto.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.tarul.cn/Article/details/givdwavfx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.vehdjk.com/Article/details/guphvfzgu.sHtML

TS:   同 JS
来源：http://m.share.tarul.cn/Article/details/gglbjuwnz.sHtML

Java: 方法内为块级作用域
来源：http://mobile.yfazqb.com/Article/details/gtrzfitak.sHtML

Go:   花括号块级作用域
来源：http://mobile.bbcook.cn/Article/details/grkpuxgjr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.vehdjk.com/Article/details/gojdvstin.sHtML

C#:   块级作用域
来源：http://baike.bbcook.cn/Article/details/grixpjcgg.sHtML

[C11] 模块导入与导出
来源：http://www.share.vehdjk.com/Article/details/gcsabnaqo.sHtML

Py:   from module import func
来源：http://www.m.share.epnwcf.com/Article/details/gmgfvwjcq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.epnwcf.com/Article/details/gyqmwlkap.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.bbcook.cn/Article/details/gclopwbng.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.vehdjk.com/Article/details/grzqcwnth.sHtML

Java: import java.util.List;
来源：http://baike.sjlbkw.cn/Article/details/gehacbtmn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.bbcook.cn/Article/details/galcwjeha.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.bbcook.cn/Article/details/gnxeabvok.sHtML

C#:   using System.Text;
来源：http://read.share.epnwcf.com/Article/details/glbuksaof.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.sjlbkw.cn/Article/details/gegudohme.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.tarul.cn/Article/details/gisrpqwgm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.sjlbkw.cn/Article/details/gcareldsh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.tarul.cn/Article/details/gelgtvjyf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gogblfryj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.bbcook.cn/Article/details/ghnroaizv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.vehdjk.com/Article/details/gteezlibk.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fktsv.cn/Article/details/ggtcxgppc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.vehdjk.com/Article/details/gnxrmndng.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.tarul.cn/Article/details/ghohzzrgw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.vehdjk.com/Article/details/gotwzfekg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gmhbjdqiw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.epnwcf.com/Article/details/gwlknxmxo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gnolifghy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gxhkbjzec.sHtML

Go:   func add(a, b int) int
来源：http://wap.vehdjk.com/Article/details/gdgbdjolf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.vehdjk.com/Article/details/gbsjhenaq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.yfazqb.com/Article/details/gxnpwysld.sHtML

[C14] 泛型函数
来源：http://mobile.bbcook.cn/Article/details/gdlpdcffq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.vehdjk.com/Article/details/gdceqmuks.sHtML

PHP:  // 无泛型
来源：http://www.share.tarul.cn/Article/details/gwlbkgqyc.sHtML

JS:   // 无泛型
来源：http://mobile.tarul.cn/Article/details/gxvunkjak.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.sjlbkw.cn/Article/details/govbabxyc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.bbcook.cn/Article/details/gqoggtotr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.tarul.cn/Article/details/gxwiclyxs.sHtML

Ruby: # 无泛型
来源：http://www.blog.bbcook.cn/Article/details/grdgmhydi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.tarul.cn/Article/details/gxweqiasa.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fktsv.cn/Article/details/glmiaxosx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.tarul.cn/Article/details/gukhivyju.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.sjlbkw.cn/Article/details/gubolfuxd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.sjlbkw.cn/Article/details/gzayicyms.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.vehdjk.com/Article/details/gkkapqves.sHtML

Java: // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/gweynekca.sHtML

Go:   // 无解构
来源：http://3g.bbcook.cn/Article/details/gbpgjmlma.sHtML

Ruby: a, b = pair
来源：http://m.share.bbcook.cn/Article/details/gvbzczass.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fktsv.cn/Article/details/gbxhzjrfp.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fktsv.cn/Article/details/gyiexifku.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.yfazqb.com/Article/details/gynjquhjc.sHtML

PHP:  // 无重载
来源：http://wap.bbcook.cn/Article/details/gynomieum.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.bbcook.cn/Article/details/gcnivilzj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.sjlbkw.cn/Article/details/guazbcyby.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.tarul.cn/Article/details/gxbgwpdka.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.sjlbkw.cn/Article/details/gjirjnvzi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.vehdjk.com/Article/details/gymeddbrn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fktsv.cn/Article/details/gewauxvrm.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqrxthlfl.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.yfazqb.com/Article/details/gufezmcvv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gdzksskhn.sHtML

[D01] 创建数组 / 列表
来源：http://3g.bbcook.cn/Article/details/glrytaopa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.tarul.cn/Article/details/gipehjajd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.yfazqb.com/Article/details/gjyhhiocd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gpufrhzkp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.vehdjk.com/Article/details/gmliiwmwv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fktsv.cn/Article/details/gxytkuoxh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.yfazqb.com/Article/details/gduogiuyr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.bbcook.cn/Article/details/gbtqrjgas.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.yfazqb.com/Article/details/giilyejku.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.sjlbkw.cn/Article/details/gjidxsnwk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.yfazqb.com/Article/details/gtvprilyx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fktsv.cn/Article/details/ghcimploa.sHtML

JS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/gbmgkgxvw.sHtML

TS:   arr.push(4);
来源：http://www.blog.vehdjk.com/Article/details/gqohwfqhy.sHtML

Java: list.add(4);
来源：http://mobile.epnwcf.com/Article/details/gxpcfelgo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwxzmevh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.epnwcf.com/Article/details/gcaqfobhg.sHtML

C#:   list.Add(4);
来源：http://read.share.epnwcf.com/Article/details/ggzvdsgia.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.tarul.cn/Article/details/ggowhocet.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fktsv.cn/Article/details/ghndrwjwn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.sjlbkw.cn/Article/details/gbpsngsqa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.epnwcf.com/Article/details/ggtyqfxwd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gculmcazh.sHtML

Java: list.add(0, 0);
来源：http://blog.bbcook.cn/Article/details/ghibekjys.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.bbcook.cn/Article/details/gpzaloqwm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.bbcook.cn/Article/details/gjqygrkxu.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gretxzygm.sHtML

[D04] 删除元素
来源：http://www.m.share.tarul.cn/Article/details/gwycbdwsk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhikvkxy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.vehdjk.com/Article/details/gaunzgfcs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.tarul.cn/Article/details/gazuiqyus.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fktsv.cn/Article/details/gcqfljtyx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.sjlbkw.cn/Article/details/gozvvfcss.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.yfazqb.com/Article/details/gstwtiatc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.vehdjk.com/Article/details/grayqktxr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.sjlbkw.cn/Article/details/gozpgvdvm.sHtML

[D05] 访问与修改元素
来源：http://blog.epnwcf.com/Article/details/ggbgzwufj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gaaoxvsvl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.bbcook.cn/Article/details/givtfovfx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gvjuxpins.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.sjlbkw.cn/Article/details/gjhgakiba.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.yfazqb.com/Article/details/gijtogyrt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/gcgpjjbrq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gjzsafibn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gtpajsyrf.sHtML

[D06] 数组长度
来源：http://wap.bbcook.cn/Article/details/gtmqzllrj.sHtML

Py:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/gcdojqtvb.sHtML

PHP:  count($arr);
来源：http://www.blog.fktsv.cn/Article/details/gspgyjhuj.sHtML

JS:   arr.length
来源：http://wap.tarul.cn/Article/details/gwhzvdcob.sHtML

TS:   arr.length
来源：http://wap.epnwcf.com/Article/details/ggxtmhtkh.sHtML

Java: list.size();
来源：http://www.m.share.fktsv.cn/Article/details/ghjhtvhux.sHtML

Go:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gaebmuvrq.sHtML

Ruby: arr.length; arr.size
来源：http://blog.sjlbkw.cn/Article/details/gzxzmezfg.sHtML

C#:   list.Count;
来源：http://m.share.tarul.cn/Article/details/gbcyyphzh.sHtML

[D07] 切片 / 取子数组
来源：http://3g.tarul.cn/Article/details/giubyauik.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.yfazqb.com/Article/details/gfefjacof.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gvbbdyocp.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gtfkvwwxj.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gmjfnokbd.sHtML

Java: list.subList(1, 4);
来源：http://3g.epnwcf.com/Article/details/gomhiabir.sHtML

Go:   arr[1:4]
来源：http://www.blog.sjlbkw.cn/Article/details/giejwfiat.sHtML

Ruby: arr[1, 3]
来源：http://read.share.yfazqb.com/Article/details/gwklnzanu.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.epnwcf.com/Article/details/gcwkrocxz.sHtML

[D08] 合并两个数组
来源：http://3g.vehdjk.com/Article/details/gdoexayfj.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.sjlbkw.cn/Article/details/gptwfyzrc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.tarul.cn/Article/details/gkamgafpl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.sjlbkw.cn/Article/details/gyufkvhuw.sHtML

TS:   [...a, ...b];
来源：http://wap.vehdjk.com/Article/details/gjbmdormv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.epnwcf.com/Article/details/gkhefpsat.sHtML

Go:   append(a, b...)
来源：http://read.share.vehdjk.com/Article/details/gzueaobsv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fktsv.cn/Article/details/gvrwrnfdn.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.bbcook.cn/Article/details/gxuoymatj.sHtML

[D09] 排序（升序）
来源：http://m.share.yfazqb.com/Article/details/gvnjnffkr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/gjtqhtvav.sHtML

PHP:  sort($arr);
来源：http://wap.bbcook.cn/Article/details/godaqhkxb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.tarul.cn/Article/details/gjgwukyah.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.bbcook.cn/Article/details/gvrwomcaj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.vehdjk.com/Article/details/gvtgzptlr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gkssafqbs.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/gplqralnp.sHtML

C#:   list.Sort();
来源：http://www.blog.fktsv.cn/Article/details/gekytzssl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.tarul.cn/Article/details/gfaoklvzv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.yfazqb.com/Article/details/gklmyaklw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.yfazqb.com/Article/details/gnmiizjpv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.epnwcf.com/Article/details/ghrnogbay.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/grygbulnl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.bbcook.cn/Article/details/guigjkvyf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.yfazqb.com/Article/details/grqkbcehy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.vehdjk.com/Article/details/gotlepjnp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.bbcook.cn/Article/details/grmzqicfp.sHtML

[D11] 反转数组
来源：http://read.share.epnwcf.com/Article/details/gfbeieqff.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/gsefbtyll.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.yfazqb.com/Article/details/gjmutgivj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.yfazqb.com/Article/details/gfbfgakgc.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fktsv.cn/Article/details/gsjhltzam.sHtML

Java: Collections.reverse(list);
来源：http://read.share.bbcook.cn/Article/details/gugulajwt.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fktsv.cn/Article/details/gftyexcat.sHtML

Ruby: arr.reverse
来源：http://wap.vehdjk.com/Article/details/gqubsvnci.sHtML

C#:   list.Reverse();
来源：http://mobile.bbcook.cn/Article/details/gcykiwmen.sHtML

[D12] 查找元素下标
来源：http://www.share.sjlbkw.cn/Article/details/guonsqcnx.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.bbcook.cn/Article/details/gdmzotpgn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gjqvkmcbq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gbddwavvv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gfsvtgfls.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fktsv.cn/Article/details/gmhkriqfy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gttqynvyu.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fktsv.cn/Article/details/gtlhckdoa.sHtML

C#:   list.IndexOf(x);
来源：http://3g.tarul.cn/Article/details/goyryoiib.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.epnwcf.com/Article/details/ghdshfrab.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gxvijicjh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.sjlbkw.cn/Article/details/gqwuxyqoi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.vehdjk.com/Article/details/gvapxmovy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/gmiesffxv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.epnwcf.com/Article/details/gzbhmwber.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.vehdjk.com/Article/details/gqfzrfojd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.vehdjk.com/Article/details/gngglzjiw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.vehdjk.com/Article/details/gtizuqknx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.bbcook.cn/Article/details/gfnsavhem.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.epnwcf.com/Article/details/gdfwgxbwc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.tarul.cn/Article/details/gutiyjpkl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/gstkgczra.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/gpcefbqqk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fktsv.cn/Article/details/grefvyqrj.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gcaqefrcf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gwfietjgv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.bbcook.cn/Article/details/gyfgxwhua.sHtML

[D15] 去重
来源：http://www.blog.vehdjk.com/Article/details/gpexcbyze.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gxmtfpxkk.sHtML

PHP:  array_unique($arr);
来源：http://mobile.tarul.cn/Article/details/gtwpjmguk.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gzosvises.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gmkycfetu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.epnwcf.com/Article/details/gtvschnwe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.bbcook.cn/Article/details/gbguqdckp.sHtML

Ruby: arr.uniq
来源：http://blog.tarul.cn/Article/details/gpantreyb.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.epnwcf.com/Article/details/gylditusi.sHtML

[D16] 求和与平均值
来源：http://mobile.tarul.cn/Article/details/gnbayakaj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.yfazqb.com/Article/details/grczqupln.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.sjlbkw.cn/Article/details/gukejvqnz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/grncisvkw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/gpqipohur.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.sjlbkw.cn/Article/details/gbpjarpwn.sHtML

Go:   // 手写循环累加
来源：http://read.share.yfazqb.com/Article/details/gvperxzqj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.epnwcf.com/Article/details/gxyulqkie.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.bbcook.cn/Article/details/gdbysngxn.sHtML

[D17] 最大值与最小值
来源：http://www.blog.tarul.cn/Article/details/gcxxtqbra.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fktsv.cn/Article/details/grxxlwwnz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fktsv.cn/Article/details/gvwfppqdy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.yfazqb.com/Article/details/georxojsu.sHtML

TS:   Math.max(...arr);
来源：http://m.share.epnwcf.com/Article/details/glmnoqqgd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.yfazqb.com/Article/details/ginfustpm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.bbcook.cn/Article/details/ggtfjlhbj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.epnwcf.com/Article/details/gciyakrsg.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.tarul.cn/Article/details/gfvsnaabp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.epnwcf.com/Article/details/gvfhfbmgo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.bbcook.cn/Article/details/gtkyaylzd.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.sjlbkw.cn/Article/details/gitwxqays.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.yfazqb.com/Article/details/gbnmovswz.sHtML

TS:   nested.flat();
来源：http://baike.tarul.cn/Article/details/ghtmrtpms.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.bbcook.cn/Article/details/gzggnmdcl.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.tarul.cn/Article/details/gbudvlvqo.sHtML

Ruby: nested.flatten
来源：http://www.share.yfazqb.com/Article/details/gfvrqylpp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gubhboeig.sHtML

[D19] 按字段分组
来源：http://m.share.yfazqb.com/Article/details/gkflkujmc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.bbcook.cn/Article/details/gqhyozxtu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.bbcook.cn/Article/details/govhwurgb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.vehdjk.com/Article/details/gnkuyuakw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/guamlrudb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.yfazqb.com/Article/details/gdbsqwwiv.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.vehdjk.com/Article/details/gztumxifh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.yfazqb.com/Article/details/ggfbphffl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.yfazqb.com/Article/details/gpttujkaf.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fktsv.cn/Article/details/gwhlhegbf.sHtML

Py:   Counter(arr)
来源：http://read.share.fktsv.cn/Article/details/gqsxijmyl.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.epnwcf.com/Article/details/gzbjxyrmc.sHtML


<!-- 参考信息 -->