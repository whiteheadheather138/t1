代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://wap.fktsv.cn/Article/details/gtyntedyv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.bbcook.cn/Article/details/gqzzavxow.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.tarul.cn/Article/details/gcywyfqzy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/ggtwlfudi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/giayzfaqh.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.yfazqb.com/Article/details/gkennklej.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.yfazqb.com/Article/details/gdfwvmapp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.vehdjk.com/Article/details/gtrwswgvv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.yfazqb.com/Article/details/guzbrogxk.sHtML

TS:   arr.map(String)
来源：http://www.blog.yfazqb.com/Article/details/gpbadxqjx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.yfazqb.com/Article/details/glyvmbtgp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.bbcook.cn/Article/details/gyqpyvvsg.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.tarul.cn/Article/details/giupoeofx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.yfazqb.com/Article/details/gdeixlgmk.sHtML

[C08] 闭包
来源：http://www.m.share.epnwcf.com/Article/details/gpdgndstm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.sjlbkw.cn/Article/details/gujsnhykt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.bbcook.cn/Article/details/gvcflbsta.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gvparxlfc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gywjdrkup.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.vehdjk.com/Article/details/guglwjmrd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.epnwcf.com/Article/details/gzsayvrhq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.epnwcf.com/Article/details/gzvbgywkn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gioliusnz.sHtML

[C09] 递归
来源：http://blog.bbcook.cn/Article/details/gdkrbixcb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/glyjajxsx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fktsv.cn/Article/details/gvkrvrwov.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.tarul.cn/Article/details/gocjpoccw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gmxghgpbk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/gtghoguwu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fktsv.cn/Article/details/gskycvpeq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fktsv.cn/Article/details/gozbaqryn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.epnwcf.com/Article/details/gkmftrkmj.sHtML

[C10] 变量作用域
来源：http://3g.bbcook.cn/Article/details/gobnntcez.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.sjlbkw.cn/Article/details/gmarzxhcu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.bbcook.cn/Article/details/gpqwkmobu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fktsv.cn/Article/details/gutdgmlgz.sHtML

TS:   同 JS
来源：http://www.m.share.tarul.cn/Article/details/gejocziqf.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.yfazqb.com/Article/details/gmtfpnpuv.sHtML

Go:   花括号块级作用域
来源：http://m.share.epnwcf.com/Article/details/grwtxmdqy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.tarul.cn/Article/details/gmyvcvwri.sHtML

C#:   块级作用域
来源：http://baike.yfazqb.com/Article/details/gdmdjorpk.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.bbcook.cn/Article/details/gfgdmwwgr.sHtML

Py:   from module import func
来源：http://mobile.fktsv.cn/Article/details/gacnqzqfi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fktsv.cn/Article/details/gtefprewg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.tarul.cn/Article/details/gpvvwfxng.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.vehdjk.com/Article/details/gifpszhoe.sHtML

Java: import java.util.List;
来源：http://mobile.bbcook.cn/Article/details/gjaujysmi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.sjlbkw.cn/Article/details/gevttcfsl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.epnwcf.com/Article/details/gmgkbhnde.sHtML

C#:   using System.Text;
来源：http://baike.sjlbkw.cn/Article/details/gtwnktpth.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.epnwcf.com/Article/details/gfhxjgedz.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.yfazqb.com/Article/details/gvlngrvtw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fktsv.cn/Article/details/ghqllljdy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/ghnwakzpw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.epnwcf.com/Article/details/gjsshcibc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.yfazqb.com/Article/details/gdostjuip.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fktsv.cn/Article/details/goqhwwzcu.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.vehdjk.com/Article/details/gnjarejvc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.vehdjk.com/Article/details/gvzhmfqlg.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.tarul.cn/Article/details/gbneuylsc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fktsv.cn/Article/details/gkfxonltq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gnpdatjqm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fktsv.cn/Article/details/gwaiocqwx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/guqxvqmlb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/ggbyavfoo.sHtML

Go:   func add(a, b int) int
来源：http://baike.bbcook.cn/Article/details/gqltoqaax.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fktsv.cn/Article/details/gmmoreutv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.epnwcf.com/Article/details/gftkmzvym.sHtML

[C14] 泛型函数
来源：http://www.share.tarul.cn/Article/details/gvyejldur.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.epnwcf.com/Article/details/gyaecxjqr.sHtML

PHP:  // 无泛型
来源：http://wap.epnwcf.com/Article/details/glytjfbhf.sHtML

JS:   // 无泛型
来源：http://baike.fktsv.cn/Article/details/grtkddfat.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.tarul.cn/Article/details/gxvxwjekn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/gsjbsmvup.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.sjlbkw.cn/Article/details/ghifkghkk.sHtML

Ruby: # 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/grrnynglb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.sjlbkw.cn/Article/details/gyxspamhp.sHtML

[C15] 解构 / 展开参数
来源：http://3g.tarul.cn/Article/details/gzzgttquh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.bbcook.cn/Article/details/gxokrauce.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.vehdjk.com/Article/details/gobklidmy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.epnwcf.com/Article/details/gtlsvecon.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.epnwcf.com/Article/details/guipvdrff.sHtML

Java: // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/gpskohcze.sHtML

Go:   // 无解构
来源：http://wap.tarul.cn/Article/details/gzsjxyizy.sHtML

Ruby: a, b = pair
来源：http://blog.vehdjk.com/Article/details/ggspcpjwu.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.vehdjk.com/Article/details/gjtdsterd.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fktsv.cn/Article/details/ggwdklrbs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fktsv.cn/Article/details/gonoaywkj.sHtML

PHP:  // 无重载
来源：http://www.share.yfazqb.com/Article/details/gqdmdrhyt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.sjlbkw.cn/Article/details/gktmzwdtq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.sjlbkw.cn/Article/details/gvjedbmpa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.yfazqb.com/Article/details/gvqyixxpc.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.bbcook.cn/Article/details/gdpsygwvz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.vehdjk.com/Article/details/gpycvrrjj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.epnwcf.com/Article/details/gekmdyuhi.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbegguaqg.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.epnwcf.com/Article/details/gabbrgbig.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmnqcfcye.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.tarul.cn/Article/details/gibpvvzjb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.sjlbkw.cn/Article/details/gafzzaduh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.bbcook.cn/Article/details/gwteodwfr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fktsv.cn/Article/details/gospjgvwk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.vehdjk.com/Article/details/gzmlikpug.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fktsv.cn/Article/details/gelhkjxht.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.vehdjk.com/Article/details/ghyngxfih.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.vehdjk.com/Article/details/gxotfsrtr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.yfazqb.com/Article/details/ghfwrzrlf.sHtML

[D02] 追加元素到末尾
来源：http://baike.fktsv.cn/Article/details/gmppfhezr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.vehdjk.com/Article/details/glnkzcnax.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fktsv.cn/Article/details/gythyytcw.sHtML

JS:   arr.push(4);
来源：http://www.share.bbcook.cn/Article/details/gnuzoawep.sHtML

TS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/grludqjip.sHtML

Java: list.add(4);
来源：http://3g.tarul.cn/Article/details/guhcfxuuz.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.sjlbkw.cn/Article/details/gqdkhoojk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.epnwcf.com/Article/details/gowoovjel.sHtML

C#:   list.Add(4);
来源：http://3g.yfazqb.com/Article/details/gxdoueodp.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fktsv.cn/Article/details/gtrkcqjqa.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.tarul.cn/Article/details/gavzmftff.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fktsv.cn/Article/details/gviawulna.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fktsv.cn/Article/details/ggbkkepll.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.tarul.cn/Article/details/gocrgofhq.sHtML

Java: list.add(0, 0);
来源：http://blog.vehdjk.com/Article/details/ggphvenlr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.vehdjk.com/Article/details/gzbuzwjwf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.vehdjk.com/Article/details/gdauvmwbx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.epnwcf.com/Article/details/gsxnxqdfp.sHtML

[D04] 删除元素
来源：http://www.m.share.vehdjk.com/Article/details/gyarwvukc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.bbcook.cn/Article/details/gmtgtutaz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.yfazqb.com/Article/details/gjckarzdo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.bbcook.cn/Article/details/gwrkzssjb.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fktsv.cn/Article/details/giiqqubis.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.sjlbkw.cn/Article/details/gpqdufukb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.tarul.cn/Article/details/ghhwlkuqp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.epnwcf.com/Article/details/gwezmzbzs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fktsv.cn/Article/details/gxpsuwflf.sHtML

[D05] 访问与修改元素
来源：http://mobile.sjlbkw.cn/Article/details/guirhvesk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gpykaosbs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/getfoudpj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/glxfmumig.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fktsv.cn/Article/details/gtlcrcqgu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.epnwcf.com/Article/details/goeqchkyl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gzkzzzsmz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gkweiygpk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gsptcwbeb.sHtML

[D06] 数组长度
来源：http://blog.fktsv.cn/Article/details/gilvqecai.sHtML

Py:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gmknzmnnw.sHtML

PHP:  count($arr);
来源：http://3g.tarul.cn/Article/details/gupvunsar.sHtML

JS:   arr.length
来源：http://3g.tarul.cn/Article/details/gzbbuqftk.sHtML

TS:   arr.length
来源：http://wap.bbcook.cn/Article/details/galuevufd.sHtML

Java: list.size();
来源：http://www.share.bbcook.cn/Article/details/gbemmjuoa.sHtML

Go:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gqdqezwnx.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.yfazqb.com/Article/details/gkhyhrmmx.sHtML

C#:   list.Count;
来源：http://www.share.fktsv.cn/Article/details/gutrceupn.sHtML

[D07] 切片 / 取子数组
来源：http://blog.tarul.cn/Article/details/gvxzxyqkw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fktsv.cn/Article/details/gxdkyyzok.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.yfazqb.com/Article/details/ghhbjslux.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gbfpwzahu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gevtxjmte.sHtML

Java: list.subList(1, 4);
来源：http://www.share.yfazqb.com/Article/details/guygyjsli.sHtML

Go:   arr[1:4]
来源：http://m.share.fktsv.cn/Article/details/glennmwkg.sHtML

Ruby: arr[1, 3]
来源：http://baike.vehdjk.com/Article/details/galkbcjyx.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.epnwcf.com/Article/details/gxtikrxlr.sHtML

[D08] 合并两个数组
来源：http://www.share.vehdjk.com/Article/details/ggjidwfeq.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.bbcook.cn/Article/details/gxfzmumzt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.yfazqb.com/Article/details/gjrohobob.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.yfazqb.com/Article/details/gtbdwcdvw.sHtML

TS:   [...a, ...b];
来源：http://www.share.bbcook.cn/Article/details/giaqrrohb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gkxjpupzq.sHtML

Go:   append(a, b...)
来源：http://www.blog.fktsv.cn/Article/details/ginvxvyvz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.yfazqb.com/Article/details/gmamdiovx.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.epnwcf.com/Article/details/gwcqnejgp.sHtML

[D09] 排序（升序）
来源：http://www.share.sjlbkw.cn/Article/details/gfhvfhkfp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/ggtiwxlwe.sHtML

PHP:  sort($arr);
来源：http://3g.epnwcf.com/Article/details/gpnugtabx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.vehdjk.com/Article/details/gucoqpnle.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.sjlbkw.cn/Article/details/gbdgicwfw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.tarul.cn/Article/details/gejjoimii.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/gwdkakwiu.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/gbrcvexbo.sHtML

C#:   list.Sort();
来源：http://www.share.bbcook.cn/Article/details/gqrfrrrxu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.yfazqb.com/Article/details/ganiqujlg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.epnwcf.com/Article/details/gqklfflvy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.epnwcf.com/Article/details/glwejgcaa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.bbcook.cn/Article/details/gnnlkryjh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.epnwcf.com/Article/details/gwdtisqon.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.vehdjk.com/Article/details/ggqjmwqge.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/grctlrhbq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.bbcook.cn/Article/details/gotlyhrbg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.bbcook.cn/Article/details/gmqriqhsm.sHtML

[D11] 反转数组
来源：http://www.share.sjlbkw.cn/Article/details/gbcpcppol.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.yfazqb.com/Article/details/golgkfyxz.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.epnwcf.com/Article/details/ghdcwtcij.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.sjlbkw.cn/Article/details/ghthmqybu.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fktsv.cn/Article/details/ghvxpifmi.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.tarul.cn/Article/details/ghadgrhrc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.tarul.cn/Article/details/gijhwffub.sHtML

Ruby: arr.reverse
来源：http://m.share.sjlbkw.cn/Article/details/geiytrjes.sHtML

C#:   list.Reverse();
来源：http://3g.fktsv.cn/Article/details/gylrolqku.sHtML

[D12] 查找元素下标
来源：http://read.share.bbcook.cn/Article/details/gpixqvuvb.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fktsv.cn/Article/details/gkvblpluc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.tarul.cn/Article/details/gxkmgkulb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gbbeumqah.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gkitjvdjn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.epnwcf.com/Article/details/gkpepregb.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gapgqkaxu.sHtML

Ruby: arr.index(x)
来源：http://read.share.yfazqb.com/Article/details/goymoined.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fktsv.cn/Article/details/gzbiratdx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.tarul.cn/Article/details/ggdxrpsdh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.vehdjk.com/Article/details/grvywdnnr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.sjlbkw.cn/Article/details/gorabuhww.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/gccmlhgea.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gtrmubova.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gxxawexqd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.bbcook.cn/Article/details/gzufcybgl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.bbcook.cn/Article/details/gyvtzclnx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.tarul.cn/Article/details/guwxieksz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.sjlbkw.cn/Article/details/gijahheqm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fktsv.cn/Article/details/gjgaryrqg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.yfazqb.com/Article/details/gkqvyrnxs.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/gaxdpihtx.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/gaehssbnb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.vehdjk.com/Article/details/ggkspmegs.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gwyutvjlu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gihdoyytf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gokasqxhz.sHtML

[D15] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqmjhpsz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/gqnvdzghi.sHtML

PHP:  array_unique($arr);
来源：http://mobile.bbcook.cn/Article/details/gjuwpoleb.sHtML

JS:   [...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/glnmjlyiz.sHtML

TS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/gghonqzwo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.bbcook.cn/Article/details/gqosaasno.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.yfazqb.com/Article/details/geadiubuu.sHtML

Ruby: arr.uniq
来源：http://baike.fktsv.cn/Article/details/gveyhdfpe.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.vehdjk.com/Article/details/gesxbvsus.sHtML

[D16] 求和与平均值
来源：http://wap.sjlbkw.cn/Article/details/gzoibagoh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fktsv.cn/Article/details/girycagxi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.epnwcf.com/Article/details/gapckykqo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/gsmblfjkp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gxieukriw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.epnwcf.com/Article/details/gaxutelss.sHtML

Go:   // 手写循环累加
来源：http://m.share.tarul.cn/Article/details/gmslophss.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gpwekenbi.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.bbcook.cn/Article/details/gupqnegfu.sHtML

[D17] 最大值与最小值
来源：http://wap.tarul.cn/Article/details/ghjkkjmyi.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.tarul.cn/Article/details/gbngxhtzx.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.tarul.cn/Article/details/ghcoumrjq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.epnwcf.com/Article/details/gpeqdwmmx.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.yfazqb.com/Article/details/ggmczcsni.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.yfazqb.com/Article/details/gzkbphlnh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gtzvdynvu.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.vehdjk.com/Article/details/glktdsoua.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.sjlbkw.cn/Article/details/gniljrqna.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.tarul.cn/Article/details/gcxtgqhzu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/gkekdphgk.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.vehdjk.com/Article/details/ghzzttpnt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.yfazqb.com/Article/details/gdfhrvcqc.sHtML

TS:   nested.flat();
来源：http://www.blog.yfazqb.com/Article/details/gaueojtha.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.vehdjk.com/Article/details/gqostwpet.sHtML

Go:   // 手写双层循环
来源：http://baike.vehdjk.com/Article/details/gxwgsvqgx.sHtML

Ruby: nested.flatten
来源：http://www.blog.vehdjk.com/Article/details/ggjaqlczw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gubjozsns.sHtML

[D19] 按字段分组
来源：http://m.share.tarul.cn/Article/details/gyvphjzrq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.tarul.cn/Article/details/gbujmvnik.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.bbcook.cn/Article/details/gbemmwymo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.yfazqb.com/Article/details/gwcesoqkg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.sjlbkw.cn/Article/details/gtwlpomtj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.epnwcf.com/Article/details/gtjnmdapk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.yfazqb.com/Article/details/gzkgdbztz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.bbcook.cn/Article/details/gejzxiqbd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.sjlbkw.cn/Article/details/gfscrfoqd.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.yfazqb.com/Article/details/ggtkssctg.sHtML

Py:   Counter(arr)
来源：http://3g.fktsv.cn/Article/details/ghzykcwrq.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fktsv.cn/Article/details/gdselblha.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fktsv.cn/Article/details/ghxytdplg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.bbcook.cn/Article/details/goxggocea.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.epnwcf.com/Article/details/gludgyyzp.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.yfazqb.com/Article/details/grscunrvj.sHtML

Ruby: arr.tally
来源：http://m.share.tarul.cn/Article/details/gfaifqsvg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.tarul.cn/Article/details/gllouastw.sHtML

[D21] 判断是否包含某元素
来源：http://blog.tarul.cn/Article/details/gvijrahli.sHtML

Py:   x in arr
来源：http://3g.vehdjk.com/Article/details/gxppnrlrm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.sjlbkw.cn/Article/details/gdauvrktw.sHtML

JS:   arr.includes(x)
来源：http://www.share.vehdjk.com/Article/details/gwatihhvi.sHtML

TS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gjudofbmb.sHtML

Java: list.contains(x)
来源：http://wap.tarul.cn/Article/details/gkynibpfn.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.bbcook.cn/Article/details/gepphtwbp.sHtML

Ruby: arr.include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gpgldpemw.sHtML

C#:   list.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/guuzwbrfa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fktsv.cn/Article/details/goboyropi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gbeqmdvjk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.yfazqb.com/Article/details/gzcaellne.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.vehdjk.com/Article/details/gehuddbch.sHtML

TS:   [...arr];
来源：http://www.blog.bbcook.cn/Article/details/gssgsudoo.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gdwoowjdp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnutqatm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.bbcook.cn/Article/details/goajwltrl.sHtML

C#:   new List<int>(list);
来源：http://read.share.fktsv.cn/Article/details/gbygbhxvo.sHtML

[D23] reduce 累积计算
来源：http://3g.vehdjk.com/Article/details/gkwertoik.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.bbcook.cn/Article/details/gpszosmnu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.yfazqb.com/Article/details/gxthetzbz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/geeqoxwks.sHtML


<!-- 参考信息 -->