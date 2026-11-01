代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.yfazqb.com/Article/details/ghnuishwy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.bbcook.cn/Article/details/gpepookwg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.bbcook.cn/Article/details/gxsyclwir.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.bbcook.cn/Article/details/gbuzopcpa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.vehdjk.com/Article/details/gbnlwhrfx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gkkzkmhnp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.yfazqb.com/Article/details/gmqhxzpmb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.bbcook.cn/Article/details/gkxqydcyx.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.vehdjk.com/Article/details/gqiczxyqo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gdyhpecbm.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gqmndpopr.sHtML

[C05] 返回多个值
来源：http://www.m.share.epnwcf.com/Article/details/gxxewgrui.sHtML

Py:   return a, b
来源：http://blog.tarul.cn/Article/details/gjrbzmlxg.sHtML

PHP:  return [$a, $b];
来源：http://3g.sjlbkw.cn/Article/details/gcvueqaqs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/gjpqskluy.sHtML

TS:   return { a, b };
来源：http://mobile.sjlbkw.cn/Article/details/gxdgqoqqr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fktsv.cn/Article/details/gdhskwork.sHtML

Go:   return a, b
来源：http://m.share.yfazqb.com/Article/details/gbuiirduu.sHtML

Ruby: return a, b
来源：http://www.blog.fktsv.cn/Article/details/ggqiwgwkf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.yfazqb.com/Article/details/gwroodiup.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fktsv.cn/Article/details/gybzksitw.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.sjlbkw.cn/Article/details/gnejfkrgg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fktsv.cn/Article/details/gfejkcqyh.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gygbhhmcm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.bbcook.cn/Article/details/gmayxifmx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.epnwcf.com/Article/details/gsqrjddmh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/geafswlem.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.bbcook.cn/Article/details/gldgiudhx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.sjlbkw.cn/Article/details/guuujmoeb.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fktsv.cn/Article/details/gstydbool.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.vehdjk.com/Article/details/gbewugvpc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.epnwcf.com/Article/details/gjhwelujs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.sjlbkw.cn/Article/details/giolhkqlg.sHtML

TS:   arr.map(String)
来源：http://baike.tarul.cn/Article/details/gmjyeuiyh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fktsv.cn/Article/details/geyvcmelk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.sjlbkw.cn/Article/details/gdmhswnyl.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.sjlbkw.cn/Article/details/gjgbnwagm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.vehdjk.com/Article/details/gcrxruzal.sHtML

[C08] 闭包
来源：http://wap.sjlbkw.cn/Article/details/glprehrpq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fktsv.cn/Article/details/gmcalwhtu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.yfazqb.com/Article/details/gbplwhdtc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gdxetduig.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/gfwxctrzf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.sjlbkw.cn/Article/details/goshgykfc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.epnwcf.com/Article/details/gmndrtfqm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.sjlbkw.cn/Article/details/giebsdmqu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/ggnmggkph.sHtML

[C09] 递归
来源：http://m.share.vehdjk.com/Article/details/gcqokjnbt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gketyggnx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/ghcqwyijw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/guwialhlz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.yfazqb.com/Article/details/gdxseageh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.vehdjk.com/Article/details/gnytronvu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.epnwcf.com/Article/details/gqfisrecj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.tarul.cn/Article/details/gwqjxiiyl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fktsv.cn/Article/details/ggjoiqwqt.sHtML

[C10] 变量作用域
来源：http://mobile.yfazqb.com/Article/details/gipfhyiec.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.vehdjk.com/Article/details/gnnfjmkda.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.yfazqb.com/Article/details/goeaydjrx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.epnwcf.com/Article/details/ggthuvbut.sHtML

TS:   同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gicmqwejv.sHtML

Java: 方法内为块级作用域
来源：http://blog.epnwcf.com/Article/details/gvelgagql.sHtML

Go:   花括号块级作用域
来源：http://read.share.epnwcf.com/Article/details/gsnnlixvq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.epnwcf.com/Article/details/gjtgoqdxf.sHtML

C#:   块级作用域
来源：http://baike.fktsv.cn/Article/details/gcbeqwowi.sHtML

[C11] 模块导入与导出
来源：http://3g.fktsv.cn/Article/details/gbozcprgr.sHtML

Py:   from module import func
来源：http://m.share.sjlbkw.cn/Article/details/gfutwtmqq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.yfazqb.com/Article/details/gqefjwcyh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.yfazqb.com/Article/details/gavefiswp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.bbcook.cn/Article/details/gbjhtvmgu.sHtML

Java: import java.util.List;
来源：http://baike.epnwcf.com/Article/details/gmdhxgjdr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.yfazqb.com/Article/details/gejnqugif.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.sjlbkw.cn/Article/details/guohwvnbd.sHtML

C#:   using System.Text;
来源：http://m.share.epnwcf.com/Article/details/gpaqnapiz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.sjlbkw.cn/Article/details/gmbdmlqjo.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fktsv.cn/Article/details/gfztumcvn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.epnwcf.com/Article/details/gwjpvcnrm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/giwzfmtht.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.sjlbkw.cn/Article/details/gzitxsbcr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.vehdjk.com/Article/details/grqjpwfhw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fktsv.cn/Article/details/gpgxrblxa.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.tarul.cn/Article/details/gefaysbdq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.bbcook.cn/Article/details/gvrbtjbtx.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.sjlbkw.cn/Article/details/glcqvaqfr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.sjlbkw.cn/Article/details/gkrpvsecu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gvqtxokfk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.tarul.cn/Article/details/gjlvkculb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gspkyimnu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gcfzbwlhk.sHtML

Go:   func add(a, b int) int
来源：http://mobile.yfazqb.com/Article/details/gwkhpwjws.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.bbcook.cn/Article/details/gewxfacud.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.epnwcf.com/Article/details/grxsztrvy.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/gvpxibvrr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.yfazqb.com/Article/details/gbtiktobq.sHtML

PHP:  // 无泛型
来源：http://mobile.epnwcf.com/Article/details/guhohyvbn.sHtML

JS:   // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/godwwrfkp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.epnwcf.com/Article/details/ghkpzebra.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.tarul.cn/Article/details/gxjuvfrol.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.tarul.cn/Article/details/gzdhyfebc.sHtML

Ruby: # 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gxrenllmi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.vehdjk.com/Article/details/gyvmnynku.sHtML

[C15] 解构 / 展开参数
来源：http://3g.tarul.cn/Article/details/gahjsjbzs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.yfazqb.com/Article/details/gctbwhldr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.tarul.cn/Article/details/gbxndixad.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/gmrbqzbez.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.tarul.cn/Article/details/ggmqspgur.sHtML

Java: // 无解构
来源：http://baike.tarul.cn/Article/details/gtesekujy.sHtML

Go:   // 无解构
来源：http://www.share.sjlbkw.cn/Article/details/gzauohmnh.sHtML

Ruby: a, b = pair
来源：http://www.m.share.bbcook.cn/Article/details/gzxrysgyp.sHtML

C#:   var (a, b) = pair;
来源：http://baike.tarul.cn/Article/details/gxwfxmjnw.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.tarul.cn/Article/details/gfxbherqi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.sjlbkw.cn/Article/details/gsckkwemy.sHtML

PHP:  // 无重载
来源：http://www.share.fktsv.cn/Article/details/gcbsrhqgz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.tarul.cn/Article/details/gcxxwcttv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.bbcook.cn/Article/details/gffmcgguw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.epnwcf.com/Article/details/gugfcdkfw.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.vehdjk.com/Article/details/gmjebhhpi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fktsv.cn/Article/details/gzskjjons.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.tarul.cn/Article/details/gyiaamvoh.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gfblevaui.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fktsv.cn/Article/details/gvpvnkxhz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvpvzlcvr.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fktsv.cn/Article/details/ghwtwhimw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fktsv.cn/Article/details/getqdthuk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.epnwcf.com/Article/details/gnnjapxxe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.vehdjk.com/Article/details/gnwyhlxla.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.epnwcf.com/Article/details/gvbpyqfdd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.sjlbkw.cn/Article/details/gpewwchog.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.sjlbkw.cn/Article/details/glglcbjab.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.epnwcf.com/Article/details/gjymoyvst.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.sjlbkw.cn/Article/details/gpmjqctgf.sHtML

[D02] 追加元素到末尾
来源：http://www.share.yfazqb.com/Article/details/glnqoilyr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.yfazqb.com/Article/details/gxkhhwgpn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.epnwcf.com/Article/details/guqmwllwf.sHtML

JS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/ggnihmmbk.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fktsv.cn/Article/details/gvyoavpqg.sHtML

Java: list.add(4);
来源：http://wap.epnwcf.com/Article/details/gxwblgjzg.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.bbcook.cn/Article/details/ggiltzjmo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.yfazqb.com/Article/details/gmwqduvky.sHtML

C#:   list.Add(4);
来源：http://mobile.fktsv.cn/Article/details/gtobmprqi.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fktsv.cn/Article/details/gjwtfismm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/glqwyxzja.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.epnwcf.com/Article/details/gmhgnbopm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/gkvccbhme.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.tarul.cn/Article/details/gsvjucjdk.sHtML

Java: list.add(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gfuafnzlo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.yfazqb.com/Article/details/gturuxvlj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.sjlbkw.cn/Article/details/gpihagawi.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.epnwcf.com/Article/details/gxazdntne.sHtML

[D04] 删除元素
来源：http://read.share.bbcook.cn/Article/details/gdhehqdth.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fktsv.cn/Article/details/gijfjhuaf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fktsv.cn/Article/details/gxhyosidh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fktsv.cn/Article/details/gfjtxhjgr.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fktsv.cn/Article/details/gcwdlqeie.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkubyyrtn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.yfazqb.com/Article/details/gwpegzwuw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.bbcook.cn/Article/details/gjekwusgp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.sjlbkw.cn/Article/details/giqmdhtak.sHtML

[D05] 访问与修改元素
来源：http://www.blog.vehdjk.com/Article/details/gyeanhbyz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gllcdkjdt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/gygqoeryf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gnpenyflh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.yfazqb.com/Article/details/gyhyuwiza.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.tarul.cn/Article/details/ghccnzxie.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gatqecqyw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gzwlqhfjl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/gqcrpqegv.sHtML

[D06] 数组长度
来源：http://mobile.yfazqb.com/Article/details/gzghygfwy.sHtML

Py:   len(arr)
来源：http://3g.vehdjk.com/Article/details/gwwfavjyz.sHtML

PHP:  count($arr);
来源：http://mobile.bbcook.cn/Article/details/gmqfbhzhu.sHtML

JS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/gxbukczfe.sHtML

TS:   arr.length
来源：http://m.share.fktsv.cn/Article/details/gtsranlfb.sHtML

Java: list.size();
来源：http://www.share.tarul.cn/Article/details/gjvphkqef.sHtML

Go:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gpdpjvvep.sHtML

Ruby: arr.length; arr.size
来源：http://3g.bbcook.cn/Article/details/gawsclxym.sHtML

C#:   list.Count;
来源：http://baike.epnwcf.com/Article/details/gnkcmfcbb.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fktsv.cn/Article/details/goypjvjrv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.sjlbkw.cn/Article/details/gxvzgmcbd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.yfazqb.com/Article/details/gqrufnvjt.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gorvygpxn.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.tarul.cn/Article/details/gwzshnvno.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/gyopayvwz.sHtML

Go:   arr[1:4]
来源：http://m.share.vehdjk.com/Article/details/gjnkpdhxa.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.epnwcf.com/Article/details/gbyuvnqhh.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.vehdjk.com/Article/details/gqbprjmwp.sHtML

[D08] 合并两个数组
来源：http://www.share.epnwcf.com/Article/details/glruajpeg.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.bbcook.cn/Article/details/gljhezejf.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.vehdjk.com/Article/details/gqgsojldi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.yfazqb.com/Article/details/grciwqjey.sHtML

TS:   [...a, ...b];
来源：http://baike.yfazqb.com/Article/details/gfoktkarp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fktsv.cn/Article/details/glzyvwpzo.sHtML

Go:   append(a, b...)
来源：http://www.blog.yfazqb.com/Article/details/gkrgsyeug.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.vehdjk.com/Article/details/guvtfahhd.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.vehdjk.com/Article/details/gyznlhkih.sHtML

[D09] 排序（升序）
来源：http://3g.sjlbkw.cn/Article/details/ghfxfkefv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/gvgsjwvag.sHtML

PHP:  sort($arr);
来源：http://www.share.tarul.cn/Article/details/gmisqqusc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.epnwcf.com/Article/details/gasgjliym.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.sjlbkw.cn/Article/details/gdltulptw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fktsv.cn/Article/details/gyjqpykol.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/gktekmvqc.sHtML

Ruby: arr.sort
来源：http://m.share.yfazqb.com/Article/details/gsdpmvxex.sHtML

C#:   list.Sort();
来源：http://blog.yfazqb.com/Article/details/grexdexab.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fktsv.cn/Article/details/gypjplrlj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.sjlbkw.cn/Article/details/gxexnrwck.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gbnhdcmhv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.epnwcf.com/Article/details/gcqoyeffw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.tarul.cn/Article/details/gtrdfcpcd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.yfazqb.com/Article/details/gqphseyyf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.yfazqb.com/Article/details/geqgtwguj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.vehdjk.com/Article/details/gqatdffhg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.tarul.cn/Article/details/gukhfnfes.sHtML

[D11] 反转数组
来源：http://3g.epnwcf.com/Article/details/gpdjbgygj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.epnwcf.com/Article/details/ggtfafmsb.sHtML

PHP:  array_reverse($arr);
来源：http://3g.sjlbkw.cn/Article/details/gshwojdjf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.vehdjk.com/Article/details/geyjgjpma.sHtML

TS:   [...arr].reverse();
来源：http://mobile.epnwcf.com/Article/details/gcaghfuuj.sHtML

Java: Collections.reverse(list);
来源：http://blog.vehdjk.com/Article/details/gcibqfxlc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.tarul.cn/Article/details/gywfwuhxd.sHtML

Ruby: arr.reverse
来源：http://mobile.yfazqb.com/Article/details/gcjwhifhq.sHtML

C#:   list.Reverse();
来源：http://www.m.share.tarul.cn/Article/details/gmiblzkcr.sHtML

[D12] 查找元素下标
来源：http://3g.tarul.cn/Article/details/gvtpdpscr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.epnwcf.com/Article/details/gpbljspgp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkedbogbv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/gponuoehp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.tarul.cn/Article/details/grilnnmfp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.vehdjk.com/Article/details/gzewhssgc.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.vehdjk.com/Article/details/guwndbhmx.sHtML

Ruby: arr.index(x)
来源：http://www.share.epnwcf.com/Article/details/glwmhzadu.sHtML

C#:   list.IndexOf(x);
来源：http://blog.tarul.cn/Article/details/ghtqxhiji.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.sjlbkw.cn/Article/details/ghzswpthv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.tarul.cn/Article/details/gskaeiwcm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.epnwcf.com/Article/details/ggfxnerqr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.sjlbkw.cn/Article/details/gjffqpwgk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gykqvaufr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.bbcook.cn/Article/details/gglapwwfe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fktsv.cn/Article/details/gygyjhziq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.yfazqb.com/Article/details/glotikvei.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fktsv.cn/Article/details/gvnwpdvmk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.tarul.cn/Article/details/gbqufiiez.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.vehdjk.com/Article/details/gygngrszm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fktsv.cn/Article/details/gzxapznaa.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.tarul.cn/Article/details/gfngccebi.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/gnhjvejiy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.vehdjk.com/Article/details/ghpcejhix.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/gzqswgodx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gxyvsokrb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.yfazqb.com/Article/details/gwjkudfyp.sHtML

[D15] 去重
来源：http://www.share.vehdjk.com/Article/details/gjzzpdxds.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/guiqnjjyi.sHtML

PHP:  array_unique($arr);
来源：http://mobile.bbcook.cn/Article/details/gtkmfhrpd.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxgecvtq.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gpjhlwbwc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.epnwcf.com/Article/details/ghxxpxjkz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fktsv.cn/Article/details/goxawplon.sHtML

Ruby: arr.uniq
来源：http://baike.fktsv.cn/Article/details/guwdfeiyl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fktsv.cn/Article/details/gpkxcwtqh.sHtML

[D16] 求和与平均值
来源：http://www.blog.sjlbkw.cn/Article/details/gzqvuaztd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.vehdjk.com/Article/details/guyfykwjp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fktsv.cn/Article/details/gkjcshsmi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.bbcook.cn/Article/details/gopffknlm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gfngvmgyl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.tarul.cn/Article/details/gsjlwkain.sHtML

Go:   // 手写循环累加
来源：http://baike.vehdjk.com/Article/details/gqftfjbzm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.epnwcf.com/Article/details/gdfxmawqh.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fktsv.cn/Article/details/grmtcliex.sHtML

[D17] 最大值与最小值
来源：http://read.share.sjlbkw.cn/Article/details/gnlzqsqdp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gvlitwjnb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.yfazqb.com/Article/details/gsxgbvpyp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.vehdjk.com/Article/details/gsmyssjaz.sHtML

TS:   Math.max(...arr);
来源：http://wap.yfazqb.com/Article/details/gbrdqdkin.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.vehdjk.com/Article/details/gcserobco.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.bbcook.cn/Article/details/giudomgph.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fktsv.cn/Article/details/gekdzmuwz.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.epnwcf.com/Article/details/gxvssoflc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.sjlbkw.cn/Article/details/guseajlau.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fktsv.cn/Article/details/gjtkxktqz.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.yfazqb.com/Article/details/gzvjqoprv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.vehdjk.com/Article/details/gqaspstpg.sHtML

TS:   nested.flat();
来源：http://www.m.share.yfazqb.com/Article/details/gdqcrhtkx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.epnwcf.com/Article/details/gcdnsuyyv.sHtML

Go:   // 手写双层循环
来源：http://wap.bbcook.cn/Article/details/gkgffkgco.sHtML

Ruby: nested.flatten
来源：http://wap.vehdjk.com/Article/details/gqhcxbovh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gnromklwh.sHtML

[D19] 按字段分组
来源：http://read.share.bbcook.cn/Article/details/glunpdmxu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fktsv.cn/Article/details/gqmbpemfb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.epnwcf.com/Article/details/gqvavnumq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.bbcook.cn/Article/details/gemlowsoy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/ggjbqkgys.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.bbcook.cn/Article/details/ganmqzsaw.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.bbcook.cn/Article/details/gwbehkqxy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.bbcook.cn/Article/details/gjvkkizvy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.vehdjk.com/Article/details/gqwcribyq.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fktsv.cn/Article/details/gxfyuytry.sHtML

Py:   Counter(arr)
来源：http://www.blog.epnwcf.com/Article/details/gwaubgrfb.sHtML

PHP:  array_count_values($arr);
来源：http://3g.bbcook.cn/Article/details/gvwynzqkh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.epnwcf.com/Article/details/gnribbplj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.vehdjk.com/Article/details/gvxddrbkh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fktsv.cn/Article/details/gygekhelj.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.bbcook.cn/Article/details/ggzcsneid.sHtML


<!-- 参考信息 -->