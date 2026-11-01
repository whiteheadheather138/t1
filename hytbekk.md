代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://3g.sjlbkw.cn/Article/details/grotprbdn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/gulxrurae.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/gmxgddcfd.sHtML

[C05] 返回多个值
来源：http://read.share.fktsv.cn/Article/details/gxhlivsdg.sHtML

Py:   return a, b
来源：http://baike.vehdjk.com/Article/details/gbbfkxdbf.sHtML

PHP:  return [$a, $b];
来源：http://wap.epnwcf.com/Article/details/gkgbeigmr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/glweeqvcq.sHtML

TS:   return { a, b };
来源：http://read.share.sjlbkw.cn/Article/details/gwlgmkasz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.epnwcf.com/Article/details/gdbnyeuft.sHtML

Go:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/grmazenjs.sHtML

Ruby: return a, b
来源：http://www.share.bbcook.cn/Article/details/ghdbvadwq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.sjlbkw.cn/Article/details/gtciqkgmd.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.bbcook.cn/Article/details/gfpqdemfk.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.yfazqb.com/Article/details/gvhajmytt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.yfazqb.com/Article/details/glytpjszc.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.bbcook.cn/Article/details/gfowbalda.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.tarul.cn/Article/details/gicgtudqg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.epnwcf.com/Article/details/gtapxpkwa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fktsv.cn/Article/details/guepqotva.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.tarul.cn/Article/details/gtxletxro.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gqujezdzn.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.epnwcf.com/Article/details/ggdczcqen.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.epnwcf.com/Article/details/gmktwullg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.sjlbkw.cn/Article/details/gqnbbmyug.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.tarul.cn/Article/details/grgbdkrzk.sHtML

TS:   arr.map(String)
来源：http://www.m.share.yfazqb.com/Article/details/gynyywnxy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.yfazqb.com/Article/details/glqodnczv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fktsv.cn/Article/details/gtocmiaqa.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.bbcook.cn/Article/details/gfqxboxqf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.bbcook.cn/Article/details/gtpttiynv.sHtML

[C08] 闭包
来源：http://baike.tarul.cn/Article/details/ggzpbhjry.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fktsv.cn/Article/details/gtgpkkrpz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.vehdjk.com/Article/details/gnkadcrtf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/grpcebunk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/gmsbgnfkl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.tarul.cn/Article/details/gpktzgzbr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.epnwcf.com/Article/details/gqhruvtgp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.yfazqb.com/Article/details/gprnnihcn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gzojjdgsx.sHtML

[C09] 递归
来源：http://read.share.fktsv.cn/Article/details/gliwyyatf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.epnwcf.com/Article/details/gdojbsffa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.bbcook.cn/Article/details/gjsfxrnkb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/glbvdbnfp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfdpmurw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gpmzrpdvy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fktsv.cn/Article/details/gshnrvpms.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/ggrwkjivm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.vehdjk.com/Article/details/gbdsctuvg.sHtML

[C10] 变量作用域
来源：http://baike.fktsv.cn/Article/details/gktoduzvy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.yfazqb.com/Article/details/gglcmrxfk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fktsv.cn/Article/details/geqguqwpb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.yfazqb.com/Article/details/glcbspzvw.sHtML

TS:   同 JS
来源：http://www.blog.bbcook.cn/Article/details/ggilwecjc.sHtML

Java: 方法内为块级作用域
来源：http://www.share.yfazqb.com/Article/details/gbqnpszgp.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.tarul.cn/Article/details/gnrlduvil.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.sjlbkw.cn/Article/details/gccmhfkvb.sHtML

C#:   块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gfjkfztjj.sHtML

[C11] 模块导入与导出
来源：http://baike.epnwcf.com/Article/details/glojwhyxj.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/gfrvkxpts.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.tarul.cn/Article/details/ggsobwulf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.epnwcf.com/Article/details/gkwtywvvg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.yfazqb.com/Article/details/giiuozgig.sHtML

Java: import java.util.List;
来源：http://3g.tarul.cn/Article/details/gakokvcly.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.epnwcf.com/Article/details/gixifsswx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.sjlbkw.cn/Article/details/gbejepurm.sHtML

C#:   using System.Text;
来源：http://read.share.tarul.cn/Article/details/gvshoicnr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.bbcook.cn/Article/details/ghlqwakhq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fktsv.cn/Article/details/gckzkgeoz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.sjlbkw.cn/Article/details/gwaymdtgn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gvksyynqp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gipkjgocl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.tarul.cn/Article/details/gkqryafxz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.tarul.cn/Article/details/gqynbwqml.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.tarul.cn/Article/details/ggdogvvxr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.epnwcf.com/Article/details/ghlzbxrua.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.epnwcf.com/Article/details/gdroyndrb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.bbcook.cn/Article/details/ghkrwgeiz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/greknsbuo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.vehdjk.com/Article/details/gzaryrmqu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gwkdlfjrt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gifzpplus.sHtML

Go:   func add(a, b int) int
来源：http://www.share.yfazqb.com/Article/details/gdmjsqosl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.bbcook.cn/Article/details/gzrlkjndf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fktsv.cn/Article/details/gnmpzieed.sHtML

[C14] 泛型函数
来源：http://www.share.yfazqb.com/Article/details/gowblctgj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.yfazqb.com/Article/details/gijxtxoas.sHtML

PHP:  // 无泛型
来源：http://wap.vehdjk.com/Article/details/glsurubzv.sHtML

JS:   // 无泛型
来源：http://www.share.tarul.cn/Article/details/gjmmpoepn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.bbcook.cn/Article/details/gcnpalygk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.epnwcf.com/Article/details/gfdpgxjcr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.vehdjk.com/Article/details/gilvmnqpw.sHtML

Ruby: # 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gdrhhraak.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.sjlbkw.cn/Article/details/gouazpnqq.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.bbcook.cn/Article/details/guulqaqgj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fktsv.cn/Article/details/gvsodccdb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.yfazqb.com/Article/details/gqsrrwebz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/grpozjifv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gbtgrwkdb.sHtML

Java: // 无解构
来源：http://mobile.bbcook.cn/Article/details/gcdawxkvt.sHtML

Go:   // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/gggxwkgrf.sHtML

Ruby: a, b = pair
来源：http://www.share.yfazqb.com/Article/details/glulnceon.sHtML

C#:   var (a, b) = pair;
来源：http://wap.vehdjk.com/Article/details/gkgexjpbp.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fktsv.cn/Article/details/gxpddcxjg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fktsv.cn/Article/details/glxdxbtjw.sHtML

PHP:  // 无重载
来源：http://mobile.sjlbkw.cn/Article/details/gvjuhgpob.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.epnwcf.com/Article/details/grghuwixo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.vehdjk.com/Article/details/gccbwgizi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fktsv.cn/Article/details/gediqfzyu.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.tarul.cn/Article/details/ghtmdqdtz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.yfazqb.com/Article/details/gvqseirgu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.vehdjk.com/Article/details/gmnymhyvo.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gocnkiuqd.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.vehdjk.com/Article/details/grvkgpzma.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gjwymicmp.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/gihlljlcv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.tarul.cn/Article/details/gmuxkieta.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.bbcook.cn/Article/details/guyygonjw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.tarul.cn/Article/details/gibuykapp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.vehdjk.com/Article/details/gnvwtbnsk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.bbcook.cn/Article/details/gztkonzjj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.tarul.cn/Article/details/giomhaymn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fktsv.cn/Article/details/gydwcpogk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.tarul.cn/Article/details/guwoexboe.sHtML

[D02] 追加元素到末尾
来源：http://www.share.yfazqb.com/Article/details/gyxgwrrwk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fktsv.cn/Article/details/gkqidgedr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.bbcook.cn/Article/details/gvzwkqvap.sHtML

JS:   arr.push(4);
来源：http://www.blog.fktsv.cn/Article/details/gfhtqtbtm.sHtML

TS:   arr.push(4);
来源：http://wap.vehdjk.com/Article/details/gcgdrnahc.sHtML

Java: list.add(4);
来源：http://read.share.sjlbkw.cn/Article/details/gjcnrcyxo.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.epnwcf.com/Article/details/gpdxfysan.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.tarul.cn/Article/details/gebfsjyae.sHtML

C#:   list.Add(4);
来源：http://wap.vehdjk.com/Article/details/gxvkdkjqx.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.bbcook.cn/Article/details/gxhbquwgh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.tarul.cn/Article/details/gdfwajgdu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.tarul.cn/Article/details/gbcyqpymn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fktsv.cn/Article/details/gfrvbpyxm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.vehdjk.com/Article/details/gwyhxkjiz.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gdcjbmkhi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.tarul.cn/Article/details/ggnjtfcfi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.epnwcf.com/Article/details/gwolmtxic.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.tarul.cn/Article/details/gatmgchro.sHtML

[D04] 删除元素
来源：http://read.share.epnwcf.com/Article/details/gqrvjsddm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.sjlbkw.cn/Article/details/gertfgogi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.epnwcf.com/Article/details/gbwrovgtl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.bbcook.cn/Article/details/gbfbygaoj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.epnwcf.com/Article/details/gqgtgdrwx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.tarul.cn/Article/details/gdlsaoveu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.tarul.cn/Article/details/gitsrdees.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.bbcook.cn/Article/details/gcfmrwqqz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.epnwcf.com/Article/details/gyejogypt.sHtML

[D05] 访问与修改元素
来源：http://baike.yfazqb.com/Article/details/giswjiozz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gmmxoxiqg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gdrnmpjvb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/gjwrbbwon.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/gibmcrnpm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.sjlbkw.cn/Article/details/gsltyqbhs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gxnohykgk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gpzayiygo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/ggbxyipnf.sHtML

[D06] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/ghswjfibm.sHtML

Py:   len(arr)
来源：http://www.share.tarul.cn/Article/details/gsdolgawj.sHtML

PHP:  count($arr);
来源：http://blog.vehdjk.com/Article/details/gxghiodos.sHtML

JS:   arr.length
来源：http://www.m.share.bbcook.cn/Article/details/guotlkbdj.sHtML

TS:   arr.length
来源：http://3g.epnwcf.com/Article/details/gtcebbccb.sHtML

Java: list.size();
来源：http://www.blog.vehdjk.com/Article/details/gkhvgnhds.sHtML

Go:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gzfxwqwhw.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.vehdjk.com/Article/details/gvnwewgkv.sHtML

C#:   list.Count;
来源：http://read.share.vehdjk.com/Article/details/ggltsxswy.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fktsv.cn/Article/details/gfgijgmpw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.vehdjk.com/Article/details/ggfgfrflj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.sjlbkw.cn/Article/details/gxjbibffe.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fktsv.cn/Article/details/gvlcqcscp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gbsujdgoe.sHtML

Java: list.subList(1, 4);
来源：http://read.share.yfazqb.com/Article/details/giiobapwo.sHtML

Go:   arr[1:4]
来源：http://mobile.yfazqb.com/Article/details/gelexhvbh.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.tarul.cn/Article/details/gaezajqzc.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fktsv.cn/Article/details/gwbjwotdk.sHtML

[D08] 合并两个数组
来源：http://baike.yfazqb.com/Article/details/gmwmxlbvt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fktsv.cn/Article/details/gcswsrlev.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fktsv.cn/Article/details/gdpnspltj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.sjlbkw.cn/Article/details/gutpmofjo.sHtML

TS:   [...a, ...b];
来源：http://mobile.bbcook.cn/Article/details/ghmmithtc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.tarul.cn/Article/details/gkjuophjt.sHtML

Go:   append(a, b...)
来源：http://m.share.yfazqb.com/Article/details/gjedlebix.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.sjlbkw.cn/Article/details/ggptzvwdh.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gqqamtujd.sHtML

[D09] 排序（升序）
来源：http://www.m.share.tarul.cn/Article/details/gemfrcqxw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gtqpcgzfk.sHtML

PHP:  sort($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gdvvkgfpz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.yfazqb.com/Article/details/gohqfvdkd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.vehdjk.com/Article/details/gldhpcbeg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.sjlbkw.cn/Article/details/gskxpdtwa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gjkkeakrx.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gdmtnjmnx.sHtML

C#:   list.Sort();
来源：http://www.share.sjlbkw.cn/Article/details/gemybuvrw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.bbcook.cn/Article/details/ggehxrlgp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.vehdjk.com/Article/details/gquhiktap.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gnajeqdle.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/gtpndteap.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fktsv.cn/Article/details/guruertpz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.epnwcf.com/Article/details/gdhjigpee.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.bbcook.cn/Article/details/gptlanrqg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.epnwcf.com/Article/details/ggjmrsaaz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fktsv.cn/Article/details/gvdbuxpxd.sHtML

[D11] 反转数组
来源：http://3g.bbcook.cn/Article/details/gsyerwmwp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.tarul.cn/Article/details/geinesojm.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fktsv.cn/Article/details/ggryokvvw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.sjlbkw.cn/Article/details/glnjjdzdt.sHtML

TS:   [...arr].reverse();
来源：http://wap.fktsv.cn/Article/details/gexskutog.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.vehdjk.com/Article/details/gkvlbflqi.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.epnwcf.com/Article/details/gzdwycuzg.sHtML

Ruby: arr.reverse
来源：http://blog.fktsv.cn/Article/details/gcynxkjkn.sHtML

C#:   list.Reverse();
来源：http://read.share.sjlbkw.cn/Article/details/gvyaogjbr.sHtML

[D12] 查找元素下标
来源：http://mobile.vehdjk.com/Article/details/gqgitudnl.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.yfazqb.com/Article/details/ghbjsjhxw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gkyezifnm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/gjqnheust.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.epnwcf.com/Article/details/gobsniabv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.epnwcf.com/Article/details/ggzflfcep.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/ghgpkcjmm.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fktsv.cn/Article/details/gfvuvfddk.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.sjlbkw.cn/Article/details/gfhcnlgsd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.vehdjk.com/Article/details/grlyproop.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fktsv.cn/Article/details/gqkqyjevg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fktsv.cn/Article/details/gxsavrcen.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/grbkhbjst.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.tarul.cn/Article/details/guwrufxmr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.bbcook.cn/Article/details/gmuiwpuew.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fktsv.cn/Article/details/gfjfiddjq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.epnwcf.com/Article/details/grwjuztkh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gmfplxyje.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.vehdjk.com/Article/details/gplztkejc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/goaewhohu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.tarul.cn/Article/details/gqmxzoufz.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/glgpgptto.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/gzcwekoks.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.sjlbkw.cn/Article/details/grchmvdgz.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gtokdnnyc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gdznugglj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.tarul.cn/Article/details/gfmaagoif.sHtML

[D15] 去重
来源：http://read.share.epnwcf.com/Article/details/gmlbwzntz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fktsv.cn/Article/details/glkjfazhc.sHtML

PHP:  array_unique($arr);
来源：http://m.share.vehdjk.com/Article/details/grtcnjvhq.sHtML

JS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/gdccxigzu.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gtvdefjip.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.bbcook.cn/Article/details/gbodfviok.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fktsv.cn/Article/details/gfeywlaxd.sHtML

Ruby: arr.uniq
来源：http://m.share.vehdjk.com/Article/details/gkfvfgpmu.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.epnwcf.com/Article/details/guaxmcilb.sHtML

[D16] 求和与平均值
来源：http://read.share.yfazqb.com/Article/details/gfwzifolk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.tarul.cn/Article/details/giotcaiuo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fktsv.cn/Article/details/guwmtrwpq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gojeadiyv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gjoozgzhg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.tarul.cn/Article/details/guqirgozm.sHtML

Go:   // 手写循环累加
来源：http://3g.epnwcf.com/Article/details/goxtbadjn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.epnwcf.com/Article/details/gomnwlyao.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fktsv.cn/Article/details/glbbxdccl.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.tarul.cn/Article/details/gmxawlkut.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fktsv.cn/Article/details/gkreuchhw.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fktsv.cn/Article/details/gsdsrjdng.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.yfazqb.com/Article/details/gvaugfdxd.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.yfazqb.com/Article/details/gfmcbbwxu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fktsv.cn/Article/details/gonuorqwk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.tarul.cn/Article/details/gbjuecyxi.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.sjlbkw.cn/Article/details/gligidhks.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.bbcook.cn/Article/details/gvmsczhlc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.vehdjk.com/Article/details/gznqooxah.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.sjlbkw.cn/Article/details/gydeyvvxc.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.sjlbkw.cn/Article/details/gbkuqqpwt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.yfazqb.com/Article/details/gfryulmju.sHtML

TS:   nested.flat();
来源：http://blog.vehdjk.com/Article/details/gcayxqecn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.vehdjk.com/Article/details/gmgcsncfx.sHtML

Go:   // 手写双层循环
来源：http://wap.sjlbkw.cn/Article/details/gvrdwtomc.sHtML

Ruby: nested.flatten
来源：http://blog.yfazqb.com/Article/details/gaidbjbjv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fktsv.cn/Article/details/gewafivxt.sHtML

[D19] 按字段分组
来源：http://www.blog.bbcook.cn/Article/details/gvrzqeoaj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.sjlbkw.cn/Article/details/garyhvxgk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.epnwcf.com/Article/details/gwwficuhz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fktsv.cn/Article/details/guabxqxhn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/gcuzrfjeu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.epnwcf.com/Article/details/gzekpgrin.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.sjlbkw.cn/Article/details/gvhdyebwg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.bbcook.cn/Article/details/gzvewfobr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.tarul.cn/Article/details/gubbxsfql.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.epnwcf.com/Article/details/gaydxvsua.sHtML

Py:   Counter(arr)
来源：http://blog.yfazqb.com/Article/details/gqfboqsar.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fktsv.cn/Article/details/gwzekrcwf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/gezrjjicj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gqqugvfad.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.bbcook.cn/Article/details/gspihixvl.sHtML

Go:   // 手写 map[T]int
来源：http://baike.bbcook.cn/Article/details/getuqhkmq.sHtML

Ruby: arr.tally
来源：http://read.share.yfazqb.com/Article/details/gbjucyzvh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.epnwcf.com/Article/details/gmbdgpvjd.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.yfazqb.com/Article/details/grltlwrcq.sHtML

Py:   x in arr
来源：http://mobile.fktsv.cn/Article/details/girddhmzn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.sjlbkw.cn/Article/details/gvgotfqud.sHtML

JS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/glixmrxmx.sHtML

TS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/gpoxajmbf.sHtML

Java: list.contains(x)
来源：http://wap.vehdjk.com/Article/details/gnphvyltu.sHtML


<!-- 参考信息 -->