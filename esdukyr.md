代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.bbcook.cn/Article/details/gzavwstfs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.vehdjk.com/Article/details/gkqnuwigb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.bbcook.cn/Article/details/ggwekimgi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.sjlbkw.cn/Article/details/gijsuxzfu.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.tarul.cn/Article/details/gqfjdtvle.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/grvpszepu.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gxrtwjbxp.sHtML

[C05] 返回多个值
来源：http://3g.vehdjk.com/Article/details/gkukzubjp.sHtML

Py:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpxtptct.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.vehdjk.com/Article/details/gkipgnaix.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.epnwcf.com/Article/details/goxgforok.sHtML

TS:   return { a, b };
来源：http://blog.epnwcf.com/Article/details/gxfocawrv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.bbcook.cn/Article/details/gwsnastva.sHtML

Go:   return a, b
来源：http://baike.vehdjk.com/Article/details/gupzyaojf.sHtML

Ruby: return a, b
来源：http://read.share.vehdjk.com/Article/details/ghdevterb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.bbcook.cn/Article/details/ggemnymdn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.vehdjk.com/Article/details/gaqyktdlv.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.bbcook.cn/Article/details/gjftymxuw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.sjlbkw.cn/Article/details/gmcqwrawq.sHtML

JS:   const square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gnniglutg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.yfazqb.com/Article/details/gfggkuvlv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.sjlbkw.cn/Article/details/gevaairtc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.tarul.cn/Article/details/gevvpfgjc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.vehdjk.com/Article/details/gygkytdef.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gjfricgyb.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.bbcook.cn/Article/details/gesvwnowl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.bbcook.cn/Article/details/gwxcoxwav.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/ggpzpsedd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fktsv.cn/Article/details/ginntspxp.sHtML

TS:   arr.map(String)
来源：http://3g.fktsv.cn/Article/details/gibzesqzr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.yfazqb.com/Article/details/gqnaefzum.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.tarul.cn/Article/details/gchwuzvnf.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.vehdjk.com/Article/details/geeslxqxy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.tarul.cn/Article/details/glkczitfs.sHtML

[C08] 闭包
来源：http://www.share.epnwcf.com/Article/details/gqiqradxf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.vehdjk.com/Article/details/guqgndevt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.yfazqb.com/Article/details/gztjazsak.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/gjhxnqnnf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gmvsgqyeh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.yfazqb.com/Article/details/gblyzomck.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.vehdjk.com/Article/details/gbthaxcqu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.tarul.cn/Article/details/gagbkxfhh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gaaftpatm.sHtML

[C09] 递归
来源：http://read.share.vehdjk.com/Article/details/gbrftomgs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.tarul.cn/Article/details/gifdlgwtr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.tarul.cn/Article/details/gpkgxegju.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.tarul.cn/Article/details/glkxayzqd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gslquvxhh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.yfazqb.com/Article/details/gjuyppyli.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.sjlbkw.cn/Article/details/ggwjaqind.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fktsv.cn/Article/details/gcjcfvljt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.tarul.cn/Article/details/gdhwzkbub.sHtML

[C10] 变量作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gncecqxdv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.epnwcf.com/Article/details/gmcoyhjhi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.bbcook.cn/Article/details/gvkpdllkw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.vehdjk.com/Article/details/gkelljlcw.sHtML

TS:   同 JS
来源：http://mobile.tarul.cn/Article/details/gcfmswyzt.sHtML

Java: 方法内为块级作用域
来源：http://m.share.epnwcf.com/Article/details/grnympsau.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gvtbtpksp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/gghnjzzxe.sHtML

C#:   块级作用域
来源：http://wap.vehdjk.com/Article/details/gluvmvmkx.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fktsv.cn/Article/details/gwxxttsbm.sHtML

Py:   from module import func
来源：http://mobile.yfazqb.com/Article/details/grbtvmgiy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.bbcook.cn/Article/details/ghffezaag.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.tarul.cn/Article/details/gxsdwshyi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.tarul.cn/Article/details/gicuidjhc.sHtML

Java: import java.util.List;
来源：http://blog.bbcook.cn/Article/details/gukdtsfxx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.tarul.cn/Article/details/ghryngcwk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.epnwcf.com/Article/details/gsxdvmzmz.sHtML

C#:   using System.Text;
来源：http://baike.epnwcf.com/Article/details/gxpwezava.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhtkhylu.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.yfazqb.com/Article/details/ghwyedwxp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.yfazqb.com/Article/details/gsbcriqfl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/gzitixtrp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.epnwcf.com/Article/details/ggymjtetg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.yfazqb.com/Article/details/gtqrlnxnc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.tarul.cn/Article/details/gkxtlmwfw.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.vehdjk.com/Article/details/gcvxijzhg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.yfazqb.com/Article/details/gljhgbygb.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.vehdjk.com/Article/details/gmeustkdd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.yfazqb.com/Article/details/grrqiyimo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gmuwykmzn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.tarul.cn/Article/details/gysvxlccj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gfjjasrjc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/guefszxkh.sHtML

Go:   func add(a, b int) int
来源：http://mobile.sjlbkw.cn/Article/details/gfsdzgfar.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.bbcook.cn/Article/details/ghumhyebp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.bbcook.cn/Article/details/gigsyijsz.sHtML

[C14] 泛型函数
来源：http://www.m.share.bbcook.cn/Article/details/gdpacrhqo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.bbcook.cn/Article/details/gbmguahfz.sHtML

PHP:  // 无泛型
来源：http://3g.bbcook.cn/Article/details/gaxkgcmen.sHtML

JS:   // 无泛型
来源：http://read.share.bbcook.cn/Article/details/gymbllcos.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.epnwcf.com/Article/details/gsqbmsbou.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.tarul.cn/Article/details/gockizstt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.yfazqb.com/Article/details/guprjlawz.sHtML

Ruby: # 无泛型
来源：http://mobile.vehdjk.com/Article/details/gfgardmai.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fktsv.cn/Article/details/gxecoedit.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.tarul.cn/Article/details/gkoluxsjh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.epnwcf.com/Article/details/gwjkbkpvp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.tarul.cn/Article/details/gponwbsyn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxzsgsabg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.epnwcf.com/Article/details/gsndbnppu.sHtML

Java: // 无解构
来源：http://mobile.bbcook.cn/Article/details/gnxolwgtb.sHtML

Go:   // 无解构
来源：http://www.blog.tarul.cn/Article/details/goehagnfo.sHtML

Ruby: a, b = pair
来源：http://mobile.epnwcf.com/Article/details/gafitydzp.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fktsv.cn/Article/details/gcgxcbtvb.sHtML

[C16] 函数 / 方法重载
来源：http://baike.sjlbkw.cn/Article/details/gcgkusdsq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.yfazqb.com/Article/details/gttdxbiyh.sHtML

PHP:  // 无重载
来源：http://read.share.sjlbkw.cn/Article/details/gqqsldroe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.bbcook.cn/Article/details/gwvyemyzk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fktsv.cn/Article/details/gsslyckiz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.yfazqb.com/Article/details/gdzoimwnk.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.tarul.cn/Article/details/gdsundolu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.bbcook.cn/Article/details/geljuwtfc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.tarul.cn/Article/details/gysorcoqt.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdkbrnqyi.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.yfazqb.com/Article/details/gruxomqoa.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmxstwcxf.sHtML

[D01] 创建数组 / 列表
来源：http://blog.epnwcf.com/Article/details/grgmdkqao.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.tarul.cn/Article/details/gtupdleum.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fktsv.cn/Article/details/ghvwqsqnv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gjcidqgch.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.vehdjk.com/Article/details/gxvameqbh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fktsv.cn/Article/details/gomwadrjh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.sjlbkw.cn/Article/details/geqldgnzs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.tarul.cn/Article/details/gxttkkqqc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.tarul.cn/Article/details/gopninkgn.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.sjlbkw.cn/Article/details/gwfztqada.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.sjlbkw.cn/Article/details/gibbbotvi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.sjlbkw.cn/Article/details/girqnrdux.sHtML

JS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/glozcabki.sHtML

TS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gulxgmgkl.sHtML

Java: list.add(4);
来源：http://mobile.tarul.cn/Article/details/geclsoxel.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gmedswjuj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fktsv.cn/Article/details/gwoydjdin.sHtML

C#:   list.Add(4);
来源：http://m.share.sjlbkw.cn/Article/details/gyhygtien.sHtML

[D03] 在指定位置插入元素
来源：http://blog.epnwcf.com/Article/details/gsayernez.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.yfazqb.com/Article/details/gjpgeabbj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.yfazqb.com/Article/details/gdxhtyktu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.tarul.cn/Article/details/guyuhrpqq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.epnwcf.com/Article/details/gkrpuidsk.sHtML

Java: list.add(0, 0);
来源：http://wap.epnwcf.com/Article/details/gxxezubdc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.yfazqb.com/Article/details/goxaqugne.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.epnwcf.com/Article/details/gcvsborus.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.vehdjk.com/Article/details/gojiakwgy.sHtML

[D04] 删除元素
来源：http://m.share.vehdjk.com/Article/details/gmjncioio.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fktsv.cn/Article/details/gzhiffuke.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.vehdjk.com/Article/details/gudlblpxz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.sjlbkw.cn/Article/details/goivxmedz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.vehdjk.com/Article/details/gvguwyppx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.bbcook.cn/Article/details/gabhaogpp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.yfazqb.com/Article/details/gcabbsars.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.bbcook.cn/Article/details/gjddzbzzc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.tarul.cn/Article/details/gfqkrtxdt.sHtML

[D05] 访问与修改元素
来源：http://www.blog.tarul.cn/Article/details/gdtpdeksy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gyqgewrtk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.yfazqb.com/Article/details/giqfrlopg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gpejpzrqx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.sjlbkw.cn/Article/details/griciofdi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fktsv.cn/Article/details/guvkiantj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/gkjgsqgco.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gklnmcvqn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gwdtlaaoh.sHtML

[D06] 数组长度
来源：http://blog.yfazqb.com/Article/details/ggmmksgpj.sHtML

Py:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gwkrrkohw.sHtML

PHP:  count($arr);
来源：http://www.m.share.tarul.cn/Article/details/guudlpaaw.sHtML

JS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/gsparkxjp.sHtML

TS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/giglbmmss.sHtML

Java: list.size();
来源：http://m.share.yfazqb.com/Article/details/gnngnnpcv.sHtML

Go:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/gvtxuzqtp.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fktsv.cn/Article/details/gamfpqsgu.sHtML

C#:   list.Count;
来源：http://read.share.yfazqb.com/Article/details/ggqqoiicm.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.epnwcf.com/Article/details/godumcciu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.bbcook.cn/Article/details/gboqhkocm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fktsv.cn/Article/details/geyhltizh.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gypbynfvp.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gylqdecne.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/glblckfeu.sHtML

Go:   arr[1:4]
来源：http://m.share.vehdjk.com/Article/details/gpkmbhsql.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fktsv.cn/Article/details/gnwtouroh.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.vehdjk.com/Article/details/giybedibr.sHtML

[D08] 合并两个数组
来源：http://read.share.fktsv.cn/Article/details/gmxvstvad.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.yfazqb.com/Article/details/gqasuujsf.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.tarul.cn/Article/details/gpsplnhum.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.yfazqb.com/Article/details/gjuanyeax.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.yfazqb.com/Article/details/gpahphngj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.vehdjk.com/Article/details/gkzzsgzzp.sHtML

Go:   append(a, b...)
来源：http://m.share.vehdjk.com/Article/details/guzpknpob.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.tarul.cn/Article/details/glacysfgj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gavopdkqb.sHtML

[D09] 排序（升序）
来源：http://m.share.tarul.cn/Article/details/gzzavmymz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gtmztkzjt.sHtML

PHP:  sort($arr);
来源：http://baike.vehdjk.com/Article/details/gmsvmkord.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fktsv.cn/Article/details/gvpvkgcsc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.sjlbkw.cn/Article/details/gwtencxik.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.yfazqb.com/Article/details/ggqhsijiv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gysvaxhhs.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/gzhnqtahw.sHtML

C#:   list.Sort();
来源：http://read.share.bbcook.cn/Article/details/gdogypyza.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fktsv.cn/Article/details/gsiyorhpz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.tarul.cn/Article/details/gcrsdwoaz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.epnwcf.com/Article/details/gzhzfkyal.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gswjrkflf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gbawavmsz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fktsv.cn/Article/details/guvqtpjce.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.vehdjk.com/Article/details/gwhaslgsi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.yfazqb.com/Article/details/gwtbrropk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.vehdjk.com/Article/details/glujzpaqc.sHtML

[D11] 反转数组
来源：http://read.share.fktsv.cn/Article/details/gfxiesqyr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.bbcook.cn/Article/details/glpyjvutx.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.vehdjk.com/Article/details/gnfwlokdh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.yfazqb.com/Article/details/glwsbrokw.sHtML

TS:   [...arr].reverse();
来源：http://blog.yfazqb.com/Article/details/gbkdlagee.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.epnwcf.com/Article/details/gioeeuzdh.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.yfazqb.com/Article/details/geftkjoqb.sHtML

Ruby: arr.reverse
来源：http://baike.bbcook.cn/Article/details/gxvdlvekn.sHtML

C#:   list.Reverse();
来源：http://mobile.epnwcf.com/Article/details/gmorestmc.sHtML

[D12] 查找元素下标
来源：http://read.share.epnwcf.com/Article/details/gxctelbqa.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.bbcook.cn/Article/details/gpecaszxo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fktsv.cn/Article/details/gnuwobaas.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gkntonzdf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/ghzrwauwo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fktsv.cn/Article/details/gdhfshlfy.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fktsv.cn/Article/details/grrxhukov.sHtML

Ruby: arr.index(x)
来源：http://3g.fktsv.cn/Article/details/ggddrylnh.sHtML

C#:   list.IndexOf(x);
来源：http://baike.tarul.cn/Article/details/gxexdsnwe.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fktsv.cn/Article/details/gxbnvcliv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.epnwcf.com/Article/details/gzyhunchu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.sjlbkw.cn/Article/details/gqhualrwr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gzvxyndsr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gcteefufu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/gqsvjxcsj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fktsv.cn/Article/details/gzvsitqvz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.yfazqb.com/Article/details/gzxbwzfsk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fktsv.cn/Article/details/gsbxogacf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fktsv.cn/Article/details/gycxfozjg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.epnwcf.com/Article/details/grftpcsyz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.tarul.cn/Article/details/gronznuud.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fktsv.cn/Article/details/gnhmbdecf.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/gnpkvackw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gstplwhrb.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/ghothhicz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.bbcook.cn/Article/details/gjtozrhdi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fktsv.cn/Article/details/gtjgldadg.sHtML

[D15] 去重
来源：http://baike.sjlbkw.cn/Article/details/gpgcuprhp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/gpcgagpkn.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.yfazqb.com/Article/details/grchubxfk.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gpsrfjdvt.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/giozhspvt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.bbcook.cn/Article/details/gxzkekabv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.tarul.cn/Article/details/gmcgeufmk.sHtML

Ruby: arr.uniq
来源：http://baike.epnwcf.com/Article/details/gpuwedwie.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gptepiyfv.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fktsv.cn/Article/details/guznrpjqh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fktsv.cn/Article/details/gyhqcagxi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.yfazqb.com/Article/details/glyrpsgvh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/getfhbasx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/gsuqrqnfc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.sjlbkw.cn/Article/details/gaifueywl.sHtML

Go:   // 手写循环累加
来源：http://3g.epnwcf.com/Article/details/gljlxkstg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.vehdjk.com/Article/details/gvlevuruy.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.bbcook.cn/Article/details/gnbpifxww.sHtML

[D17] 最大值与最小值
来源：http://www.blog.vehdjk.com/Article/details/gsmrnetyn.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.sjlbkw.cn/Article/details/gzigdnqhe.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.vehdjk.com/Article/details/gxwtgglre.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.yfazqb.com/Article/details/gpajwewvr.sHtML

TS:   Math.max(...arr);
来源：http://m.share.bbcook.cn/Article/details/gptzcwrph.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.tarul.cn/Article/details/gtsovwryx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.sjlbkw.cn/Article/details/gxrxvjvab.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.tarul.cn/Article/details/gezxozqit.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.bbcook.cn/Article/details/gsrbgmbcz.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.sjlbkw.cn/Article/details/gtyzpzfrq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fktsv.cn/Article/details/grrikookr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.yfazqb.com/Article/details/gsoslgbkr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.bbcook.cn/Article/details/gidqcnhyo.sHtML

TS:   nested.flat();
来源：http://read.share.yfazqb.com/Article/details/gxivvzvnh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.epnwcf.com/Article/details/gvuizqjca.sHtML

Go:   // 手写双层循环
来源：http://baike.vehdjk.com/Article/details/gatsyxbjz.sHtML

Ruby: nested.flatten
来源：http://www.blog.bbcook.cn/Article/details/gfshvgpok.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.tarul.cn/Article/details/gmxavyxxu.sHtML

[D19] 按字段分组
来源：http://www.share.sjlbkw.cn/Article/details/gyfopgvde.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.epnwcf.com/Article/details/gqxiwodex.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.tarul.cn/Article/details/gcqvzgjjw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.sjlbkw.cn/Article/details/gagjpzfox.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fktsv.cn/Article/details/ghjrzvfky.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.vehdjk.com/Article/details/gzayjvuhc.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.epnwcf.com/Article/details/gymkursvl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.yfazqb.com/Article/details/gsjjtyemx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.bbcook.cn/Article/details/gxhptcbru.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.epnwcf.com/Article/details/gmthzowfi.sHtML

Py:   Counter(arr)
来源：http://mobile.tarul.cn/Article/details/gvwqsgasw.sHtML

PHP:  array_count_values($arr);
来源：http://wap.epnwcf.com/Article/details/gflzrlxzq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/gsohwwhuf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.yfazqb.com/Article/details/gwfbrwcff.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.epnwcf.com/Article/details/gjdbxchxi.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fktsv.cn/Article/details/gtpztvwcb.sHtML

Ruby: arr.tally
来源：http://wap.sjlbkw.cn/Article/details/golzirwgw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.sjlbkw.cn/Article/details/giaribmjy.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fktsv.cn/Article/details/gylqxasoj.sHtML

Py:   x in arr
来源：http://www.m.share.vehdjk.com/Article/details/gunjxuyah.sHtML


<!-- 参考信息 -->