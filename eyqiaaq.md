代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://3g.epnwcf.com/Article/details/gpbakkwxo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.vehdjk.com/Article/details/gisgasvjw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.bbcook.cn/Article/details/gpaaavvip.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.yfazqb.com/Article/details/gixkjymju.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.vehdjk.com/Article/details/gsquthena.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/glfgtlaps.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.tarul.cn/Article/details/gerihsqkb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.sjlbkw.cn/Article/details/ggojftyhw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.sjlbkw.cn/Article/details/gnbqiecpo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gsvdyrzwl.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gkxarzrtz.sHtML

[C05] 返回多个值
来源：http://www.share.sjlbkw.cn/Article/details/gymjpgnbp.sHtML

Py:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/gpblssbai.sHtML

PHP:  return [$a, $b];
来源：http://read.share.yfazqb.com/Article/details/grivqszbd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.vehdjk.com/Article/details/gubnvpmmv.sHtML

TS:   return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/gnqlorpph.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.epnwcf.com/Article/details/ggzsylsrq.sHtML

Go:   return a, b
来源：http://3g.yfazqb.com/Article/details/gassbvyur.sHtML

Ruby: return a, b
来源：http://blog.epnwcf.com/Article/details/gupaciltd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.vehdjk.com/Article/details/gufmgfnuu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.yfazqb.com/Article/details/grnfuoasr.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.vehdjk.com/Article/details/gyuujxnvm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.sjlbkw.cn/Article/details/gswgvlzaa.sHtML

JS:   const square = x => x * x;
来源：http://3g.tarul.cn/Article/details/gecjggzru.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gixpavgnm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.epnwcf.com/Article/details/gbhmanbzw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.yfazqb.com/Article/details/gkgvlqtza.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fktsv.cn/Article/details/ghqbfmslv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gmwkuzwsg.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.epnwcf.com/Article/details/geqtjvhya.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.bbcook.cn/Article/details/gbydnatok.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/gtbosguhd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.epnwcf.com/Article/details/gttnfwihg.sHtML

TS:   arr.map(String)
来源：http://mobile.vehdjk.com/Article/details/gknxaihvv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.epnwcf.com/Article/details/gxdzhvcce.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fktsv.cn/Article/details/gaqpqdqgm.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.yfazqb.com/Article/details/gozyzjtbr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.sjlbkw.cn/Article/details/guybletnd.sHtML

[C08] 闭包
来源：http://wap.sjlbkw.cn/Article/details/grqakhswk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.epnwcf.com/Article/details/gqlmlxgvj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.epnwcf.com/Article/details/gelnkucdr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gxqgcsumi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gimcixdfa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.yfazqb.com/Article/details/gwohnnbch.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.tarul.cn/Article/details/ggyzfjooi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.sjlbkw.cn/Article/details/ghrzxveqn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/guwchdjtd.sHtML

[C09] 递归
来源：http://www.share.fktsv.cn/Article/details/gryqxvcyq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gshkdthuu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.yfazqb.com/Article/details/gtdbzrvzg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fktsv.cn/Article/details/gntsyzola.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/gqaecxuiv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.yfazqb.com/Article/details/gihgofujr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.yfazqb.com/Article/details/gglscfgbc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.bbcook.cn/Article/details/gvaybfqyg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.tarul.cn/Article/details/gdesbphmw.sHtML

[C10] 变量作用域
来源：http://www.m.share.epnwcf.com/Article/details/goccbyxvq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.bbcook.cn/Article/details/gczsxvtrt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.vehdjk.com/Article/details/guchufcot.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gvaxhautm.sHtML

TS:   同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsfbkkdm.sHtML

Java: 方法内为块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/guognzlhd.sHtML

Go:   花括号块级作用域
来源：http://3g.bbcook.cn/Article/details/gapeqfhnd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.bbcook.cn/Article/details/gedsrqvco.sHtML

C#:   块级作用域
来源：http://mobile.epnwcf.com/Article/details/grnafcsna.sHtML

[C11] 模块导入与导出
来源：http://read.share.epnwcf.com/Article/details/gpgcbkznm.sHtML

Py:   from module import func
来源：http://3g.bbcook.cn/Article/details/gyxfmhgkl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.bbcook.cn/Article/details/gsujfrsbg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.vehdjk.com/Article/details/gjkyezldk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.tarul.cn/Article/details/gtgkrqlqh.sHtML

Java: import java.util.List;
来源：http://www.share.tarul.cn/Article/details/gdbjcrirx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.bbcook.cn/Article/details/gdnyxermc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fktsv.cn/Article/details/gsheisdrn.sHtML

C#:   using System.Text;
来源：http://mobile.fktsv.cn/Article/details/gydewwomn.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.tarul.cn/Article/details/ghfqqhzlv.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.vehdjk.com/Article/details/gsdqbhugj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.vehdjk.com/Article/details/gqamxtsuv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/geieinzgu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.yfazqb.com/Article/details/gvhxawwov.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.tarul.cn/Article/details/gnedykowg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.vehdjk.com/Article/details/gltrmggqh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.sjlbkw.cn/Article/details/gtklgpmqf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.sjlbkw.cn/Article/details/gcazafddh.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.epnwcf.com/Article/details/gmydxpqzo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.tarul.cn/Article/details/gjtzmkqij.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/ggabxtzvx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.vehdjk.com/Article/details/gsinkobvz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gppmcsvye.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gmrxqqfde.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.bbcook.cn/Article/details/gfaldtauz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.yfazqb.com/Article/details/gruovtlbs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.bbcook.cn/Article/details/guizlkkxy.sHtML

[C14] 泛型函数
来源：http://wap.fktsv.cn/Article/details/gzbvsbcff.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.epnwcf.com/Article/details/gvofthdlg.sHtML

PHP:  // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gnduqzaqv.sHtML

JS:   // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gdogrlenu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/gphezaamv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.vehdjk.com/Article/details/gynrpeytu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.sjlbkw.cn/Article/details/goqehhfur.sHtML

Ruby: # 无泛型
来源：http://read.share.bbcook.cn/Article/details/gszyxrsxa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.epnwcf.com/Article/details/gnuoannho.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.tarul.cn/Article/details/gjzhjvtfr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.bbcook.cn/Article/details/gyanbucsb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.vehdjk.com/Article/details/gvewrgccy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/gdnvjuxcy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.yfazqb.com/Article/details/gqtwqzxzt.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/glxpzdohi.sHtML

Go:   // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/glncvzghc.sHtML

Ruby: a, b = pair
来源：http://m.share.yfazqb.com/Article/details/gpppbopso.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.tarul.cn/Article/details/gghrsxtzv.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.vehdjk.com/Article/details/gihupywbw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fktsv.cn/Article/details/gqglzysoi.sHtML

PHP:  // 无重载
来源：http://read.share.fktsv.cn/Article/details/gsenftryl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.tarul.cn/Article/details/gyixbzkzz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.yfazqb.com/Article/details/giosdyxks.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.vehdjk.com/Article/details/gazdjzlcd.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.sjlbkw.cn/Article/details/guawlrnsx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.sjlbkw.cn/Article/details/ggfyknvch.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fktsv.cn/Article/details/gqslaurdw.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/grkcihxpk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.bbcook.cn/Article/details/gwfppwnqf.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdcpdppav.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.yfazqb.com/Article/details/gamtowgeh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.sjlbkw.cn/Article/details/gmnrynkxe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.epnwcf.com/Article/details/gyzqcceef.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.epnwcf.com/Article/details/gcnapbqot.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.vehdjk.com/Article/details/ghobszmoc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.bbcook.cn/Article/details/gqlmnxndr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fktsv.cn/Article/details/gnshuxdyo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.epnwcf.com/Article/details/gjfmhgbyr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.epnwcf.com/Article/details/gvjirvjbt.sHtML

[D02] 追加元素到末尾
来源：http://3g.epnwcf.com/Article/details/grjjopzos.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fktsv.cn/Article/details/gqnvqkbvi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.yfazqb.com/Article/details/gikqofoyd.sHtML

JS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gfbxmesfl.sHtML

TS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/grzblovbl.sHtML

Java: list.add(4);
来源：http://3g.fktsv.cn/Article/details/gkctzskci.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gmagmkqzl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fktsv.cn/Article/details/gvztyuziu.sHtML

C#:   list.Add(4);
来源：http://3g.bbcook.cn/Article/details/glaxswrzo.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fktsv.cn/Article/details/gecveemkm.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.epnwcf.com/Article/details/gcobkgjyp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.yfazqb.com/Article/details/ghjvarmzt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.epnwcf.com/Article/details/grqudzasa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.epnwcf.com/Article/details/gajuezvpa.sHtML

Java: list.add(0, 0);
来源：http://wap.epnwcf.com/Article/details/gccysvxgd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqrbmffy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.epnwcf.com/Article/details/gttzadtma.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.bbcook.cn/Article/details/gpmhamrxw.sHtML

[D04] 删除元素
来源：http://blog.sjlbkw.cn/Article/details/gsfgzuajw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.yfazqb.com/Article/details/giicnawmj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/gwcqxqhwl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.yfazqb.com/Article/details/gdjxlnmme.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.vehdjk.com/Article/details/gitzzptek.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.yfazqb.com/Article/details/guehucdle.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.bbcook.cn/Article/details/glhnyribq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fktsv.cn/Article/details/gotuqkfwz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fktsv.cn/Article/details/grkxenrdy.sHtML

[D05] 访问与修改元素
来源：http://wap.bbcook.cn/Article/details/gcuzhfgfb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/gywcpfzim.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gegbzvniu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gvshfkcxg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.sjlbkw.cn/Article/details/gavejijic.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fktsv.cn/Article/details/gktoyyuud.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/gjqlwbscl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/grziyqnxc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gbecrihzi.sHtML

[D06] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gfjeekmxf.sHtML

Py:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/guetswkei.sHtML

PHP:  count($arr);
来源：http://3g.fktsv.cn/Article/details/gjcjeplbr.sHtML

JS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gtekaglxp.sHtML

TS:   arr.length
来源：http://baike.epnwcf.com/Article/details/goeamckaq.sHtML

Java: list.size();
来源：http://www.blog.yfazqb.com/Article/details/gqpchhcxy.sHtML

Go:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/gvvftizkb.sHtML

Ruby: arr.length; arr.size
来源：http://3g.bbcook.cn/Article/details/gxirlkcsz.sHtML

C#:   list.Count;
来源：http://3g.sjlbkw.cn/Article/details/grerrkdpd.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.epnwcf.com/Article/details/ghpbrvqoe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.epnwcf.com/Article/details/ginlkjwew.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.bbcook.cn/Article/details/guzqcefki.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/grkmtrwhj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gecemgjoq.sHtML

Java: list.subList(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gyjssdbta.sHtML

Go:   arr[1:4]
来源：http://blog.yfazqb.com/Article/details/gxbrhzdeg.sHtML

Ruby: arr[1, 3]
来源：http://mobile.tarul.cn/Article/details/gvtieqilb.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fktsv.cn/Article/details/giapqmhpg.sHtML

[D08] 合并两个数组
来源：http://mobile.epnwcf.com/Article/details/gkzsoedns.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.sjlbkw.cn/Article/details/gcyyjhmzw.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fktsv.cn/Article/details/gbbcpuead.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.tarul.cn/Article/details/gpkhazowu.sHtML

TS:   [...a, ...b];
来源：http://m.share.tarul.cn/Article/details/gftfdaays.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.tarul.cn/Article/details/gkuppoott.sHtML

Go:   append(a, b...)
来源：http://m.share.bbcook.cn/Article/details/gewujokcd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.yfazqb.com/Article/details/glbtxgcwp.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.bbcook.cn/Article/details/goyddptnq.sHtML

[D09] 排序（升序）
来源：http://baike.sjlbkw.cn/Article/details/gxnbgnedt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/grsxcdnwl.sHtML

PHP:  sort($arr);
来源：http://baike.fktsv.cn/Article/details/gnwwftsum.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.tarul.cn/Article/details/guuonyrok.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.tarul.cn/Article/details/goqdbloex.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.sjlbkw.cn/Article/details/gyeymjibj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gxggsuonr.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/gbuovqldn.sHtML

C#:   list.Sort();
来源：http://baike.tarul.cn/Article/details/gvsvjwgfc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.epnwcf.com/Article/details/gppkdqyzw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.tarul.cn/Article/details/garuwmdhh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/ghbbmemvh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gnntghgmi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gpyavdcvy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.epnwcf.com/Article/details/gzahtydnw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.epnwcf.com/Article/details/gvrgpughd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.sjlbkw.cn/Article/details/ghrdkhols.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fktsv.cn/Article/details/gzenlaihn.sHtML

[D11] 反转数组
来源：http://baike.vehdjk.com/Article/details/gvslcbtnb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.epnwcf.com/Article/details/ghjttexpz.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gfydnonne.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fktsv.cn/Article/details/gtnilwpqx.sHtML

TS:   [...arr].reverse();
来源：http://mobile.yfazqb.com/Article/details/gkckqgntg.sHtML

Java: Collections.reverse(list);
来源：http://m.share.sjlbkw.cn/Article/details/gkzcruwkj.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.epnwcf.com/Article/details/gstazmfkj.sHtML

Ruby: arr.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gsknljibf.sHtML

C#:   list.Reverse();
来源：http://www.blog.fktsv.cn/Article/details/gmadgsubj.sHtML

[D12] 查找元素下标
来源：http://wap.epnwcf.com/Article/details/gqirhwfxk.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.yfazqb.com/Article/details/ghdjqnukg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.yfazqb.com/Article/details/gopignpzv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/gluyrhifa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gzubsdecj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fktsv.cn/Article/details/ggbdhnbob.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gyrizimyy.sHtML

Ruby: arr.index(x)
来源：http://www.blog.yfazqb.com/Article/details/gbdbbheng.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.sjlbkw.cn/Article/details/gysfqbowq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fktsv.cn/Article/details/gkptrwgyo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.tarul.cn/Article/details/gwhedijub.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.yfazqb.com/Article/details/gttpdwuai.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/glewppror.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/gywnltloq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.vehdjk.com/Article/details/gpdyhxycj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.tarul.cn/Article/details/gxgjnudca.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.sjlbkw.cn/Article/details/gdnzbthox.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fktsv.cn/Article/details/gjivcqwlg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fktsv.cn/Article/details/ggyblzkko.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.sjlbkw.cn/Article/details/ghaswngmq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fktsv.cn/Article/details/guvnrlsqv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gdxxmyffs.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/gapcpnwle.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.yfazqb.com/Article/details/goguvlmxk.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gnnxurctk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.yfazqb.com/Article/details/gkstosttz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.epnwcf.com/Article/details/gyucfpvkq.sHtML

[D15] 去重
来源：http://www.share.sjlbkw.cn/Article/details/gegukkpyv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.epnwcf.com/Article/details/gmrrsxuej.sHtML

PHP:  array_unique($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gmrjaukny.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gxtcxmzri.sHtML

TS:   [...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gsczointz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.tarul.cn/Article/details/gipxjpxds.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.sjlbkw.cn/Article/details/gxbkyxfic.sHtML

Ruby: arr.uniq
来源：http://www.blog.tarul.cn/Article/details/gfjdbtode.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.tarul.cn/Article/details/ghftmwlpb.sHtML

[D16] 求和与平均值
来源：http://read.share.yfazqb.com/Article/details/gaofjiurh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gvfqzjgqz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.bbcook.cn/Article/details/gjswmnfzq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/gdxwcgizl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.bbcook.cn/Article/details/gturyjglg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.epnwcf.com/Article/details/gdimcmwdh.sHtML

Go:   // 手写循环累加
来源：http://3g.tarul.cn/Article/details/gqvnqqfks.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.epnwcf.com/Article/details/gmwdcsxkv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.bbcook.cn/Article/details/gceipnpoa.sHtML

[D17] 最大值与最小值
来源：http://blog.epnwcf.com/Article/details/gkfkukqeb.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.epnwcf.com/Article/details/guuymyrxr.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.tarul.cn/Article/details/gusrsmran.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fktsv.cn/Article/details/gkhiyujar.sHtML

TS:   Math.max(...arr);
来源：http://3g.yfazqb.com/Article/details/gnvnmekhm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.epnwcf.com/Article/details/gufdqllxn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/goigrxpeo.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.tarul.cn/Article/details/gwtsnuowd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/gziojjhkv.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.bbcook.cn/Article/details/gpbfvaxzl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.yfazqb.com/Article/details/glrsejmxo.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.yfazqb.com/Article/details/gngbhtjor.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.yfazqb.com/Article/details/gegylqksp.sHtML

TS:   nested.flat();
来源：http://3g.sjlbkw.cn/Article/details/gwmivtwba.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.epnwcf.com/Article/details/grhhehpig.sHtML

Go:   // 手写双层循环
来源：http://www.blog.yfazqb.com/Article/details/gicxyovio.sHtML

Ruby: nested.flatten
来源：http://baike.epnwcf.com/Article/details/gypqtvygs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fktsv.cn/Article/details/gytazvnpg.sHtML

[D19] 按字段分组
来源：http://www.share.vehdjk.com/Article/details/gzgovqtws.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fktsv.cn/Article/details/gesmmzxyq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.sjlbkw.cn/Article/details/gathocqew.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fktsv.cn/Article/details/ghtvfxuia.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/grmirjlqt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.tarul.cn/Article/details/gtzsmsrkq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.tarul.cn/Article/details/gjqzusfdc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.vehdjk.com/Article/details/gdrqtjnyx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.bbcook.cn/Article/details/gjtaezmfd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.yfazqb.com/Article/details/gmhubhgrp.sHtML

Py:   Counter(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gckmqajtl.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gvvyimulg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gaeljwfqi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.bbcook.cn/Article/details/ggbknffzv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fktsv.cn/Article/details/glftkidzp.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.epnwcf.com/Article/details/gqvdkredo.sHtML


<!-- 参考信息 -->