代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.bbcook.cn/Article/details/gfavsztpl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gqprxlkxd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.vehdjk.com/Article/details/gcwzyyyhz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.epnwcf.com/Article/details/getxqmblo.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.sjlbkw.cn/Article/details/gkygzrjez.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gracojwlv.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/ggidznnhw.sHtML

[C05] 返回多个值
来源：http://www.share.tarul.cn/Article/details/gmsbqskiw.sHtML

Py:   return a, b
来源：http://3g.fktsv.cn/Article/details/ghzyxfevw.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fktsv.cn/Article/details/gptzpwtda.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.tarul.cn/Article/details/gdbqvkkin.sHtML

TS:   return { a, b };
来源：http://blog.vehdjk.com/Article/details/gyslbddrx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fktsv.cn/Article/details/grqzkrddo.sHtML

Go:   return a, b
来源：http://3g.vehdjk.com/Article/details/gcbwnckrf.sHtML

Ruby: return a, b
来源：http://3g.fktsv.cn/Article/details/gzufmqetf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fktsv.cn/Article/details/gbqajnezw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fktsv.cn/Article/details/gjazecfrc.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.yfazqb.com/Article/details/gfscracqn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.tarul.cn/Article/details/greouhtmi.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gmfqqiity.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.vehdjk.com/Article/details/gwtivkfic.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.vehdjk.com/Article/details/gdcopmbvb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.tarul.cn/Article/details/gseqvxbfo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.epnwcf.com/Article/details/gcbhkucob.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.bbcook.cn/Article/details/gyzmyqcpq.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fktsv.cn/Article/details/glhwqkgho.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.yfazqb.com/Article/details/gupqekrio.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.bbcook.cn/Article/details/gnlezmkyb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.yfazqb.com/Article/details/gultxsevd.sHtML

TS:   arr.map(String)
来源：http://www.blog.vehdjk.com/Article/details/gurxnluem.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gfoekudao.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.sjlbkw.cn/Article/details/gsfmcocux.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.yfazqb.com/Article/details/gihocztdt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.tarul.cn/Article/details/gihnrvapj.sHtML

[C08] 闭包
来源：http://m.share.yfazqb.com/Article/details/gnuhssjbg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.tarul.cn/Article/details/gcdpvjgeq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.epnwcf.com/Article/details/gejyajcrr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gsawavnop.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gutxumoen.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.bbcook.cn/Article/details/gnyhveish.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.tarul.cn/Article/details/gfrzvnevm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.tarul.cn/Article/details/gcrmheshu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gunqdtofb.sHtML

[C09] 递归
来源：http://www.m.share.yfazqb.com/Article/details/gftdilfml.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.tarul.cn/Article/details/gkymvzfbh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gfdcwnvme.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gatkygerw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.vehdjk.com/Article/details/gtlubzsvb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fktsv.cn/Article/details/gqxodgauc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.vehdjk.com/Article/details/gojfbkhln.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.epnwcf.com/Article/details/gbcoiaayp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.bbcook.cn/Article/details/geugnurpt.sHtML

[C10] 变量作用域
来源：http://read.share.yfazqb.com/Article/details/gyehnwdvf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fktsv.cn/Article/details/gjrjojbet.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.yfazqb.com/Article/details/gufecqfsn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fktsv.cn/Article/details/gertrbcyu.sHtML

TS:   同 JS
来源：http://mobile.epnwcf.com/Article/details/gydsvedca.sHtML

Java: 方法内为块级作用域
来源：http://3g.fktsv.cn/Article/details/glimkjriv.sHtML

Go:   花括号块级作用域
来源：http://wap.fktsv.cn/Article/details/gspeujhgj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.bbcook.cn/Article/details/gsgvccqed.sHtML

C#:   块级作用域
来源：http://read.share.tarul.cn/Article/details/gqhwdzfed.sHtML

[C11] 模块导入与导出
来源：http://3g.fktsv.cn/Article/details/gwgsmcncf.sHtML

Py:   from module import func
来源：http://m.share.sjlbkw.cn/Article/details/gpinudyyv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.yfazqb.com/Article/details/gfktwqgok.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfuyxhhg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.vehdjk.com/Article/details/gpkdbspwn.sHtML

Java: import java.util.List;
来源：http://m.share.vehdjk.com/Article/details/gccinmrsc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.tarul.cn/Article/details/glycdqfey.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/gbdxuamzo.sHtML

C#:   using System.Text;
来源：http://www.m.share.tarul.cn/Article/details/gpxrpqxvk.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fktsv.cn/Article/details/gyerhrccd.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fktsv.cn/Article/details/gpyhgzbtj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gtilacykn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.bbcook.cn/Article/details/gxblrzpld.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.vehdjk.com/Article/details/gclyqqezm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.tarul.cn/Article/details/ggvmaqjfv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.sjlbkw.cn/Article/details/gqucbzkfx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.sjlbkw.cn/Article/details/guzzahril.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.tarul.cn/Article/details/galrcnlqx.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.sjlbkw.cn/Article/details/gjgokwzyh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gksmguxrt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/ggbibhdiq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fktsv.cn/Article/details/gskicffjt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/glcppzdjw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gyqzcqzxv.sHtML

Go:   func add(a, b int) int
来源：http://wap.tarul.cn/Article/details/gadwgtgzh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.tarul.cn/Article/details/gkhwplkxo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.sjlbkw.cn/Article/details/grxmoqtzo.sHtML

[C14] 泛型函数
来源：http://blog.vehdjk.com/Article/details/gfzvgdynf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fktsv.cn/Article/details/gpxzkbngr.sHtML

PHP:  // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/ghongsuru.sHtML

JS:   // 无泛型
来源：http://m.share.epnwcf.com/Article/details/gbiavhwdj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.tarul.cn/Article/details/gmwhwnyrg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fktsv.cn/Article/details/gpawpfdae.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fktsv.cn/Article/details/gmuedqcyg.sHtML

Ruby: # 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gzaxbalga.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.epnwcf.com/Article/details/gjybsrhiu.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.vehdjk.com/Article/details/gzcmnvodv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.sjlbkw.cn/Article/details/gsitsjzvv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.sjlbkw.cn/Article/details/gggounufm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.bbcook.cn/Article/details/giahttszt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.vehdjk.com/Article/details/gjtvrektr.sHtML

Java: // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/gdadakdvw.sHtML

Go:   // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gzbxkfqxe.sHtML

Ruby: a, b = pair
来源：http://m.share.fktsv.cn/Article/details/gusvmngdr.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.sjlbkw.cn/Article/details/gmdlctbii.sHtML

[C16] 函数 / 方法重载
来源：http://baike.yfazqb.com/Article/details/genqpemzr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.bbcook.cn/Article/details/gprvavtjk.sHtML

PHP:  // 无重载
来源：http://www.share.epnwcf.com/Article/details/gmbumdyld.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.tarul.cn/Article/details/gsbfpoobj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.yfazqb.com/Article/details/gilvdwgib.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.sjlbkw.cn/Article/details/gehnlxyfw.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.tarul.cn/Article/details/gfxrabzes.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.epnwcf.com/Article/details/gxivlxyxv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.sjlbkw.cn/Article/details/gzqrezicy.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gixgealrw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.epnwcf.com/Article/details/galclrxwn.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gcmvfaqsa.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/ggyryqsiv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.vehdjk.com/Article/details/gyapfgjmg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.sjlbkw.cn/Article/details/gpvfsartp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.epnwcf.com/Article/details/gyncruodp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.vehdjk.com/Article/details/gnwqbmhpf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fktsv.cn/Article/details/gxhtpklmk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.bbcook.cn/Article/details/glbewgcip.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.yfazqb.com/Article/details/gztvhgood.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fktsv.cn/Article/details/gozbtjurh.sHtML

[D02] 追加元素到末尾
来源：http://m.share.vehdjk.com/Article/details/gsvwppqnc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fktsv.cn/Article/details/gxztsbpfk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.tarul.cn/Article/details/gozcjpura.sHtML

JS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/gykdvlmgx.sHtML

TS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gehagthta.sHtML

Java: list.add(4);
来源：http://read.share.epnwcf.com/Article/details/gpriuhuny.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.yfazqb.com/Article/details/gtgjjebmy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.sjlbkw.cn/Article/details/gsjrovixj.sHtML

C#:   list.Add(4);
来源：http://mobile.fktsv.cn/Article/details/gyyfvtymd.sHtML

[D03] 在指定位置插入元素
来源：http://baike.yfazqb.com/Article/details/guezacqth.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/gjmxgxvik.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.bbcook.cn/Article/details/guscfrxys.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.bbcook.cn/Article/details/gbwdnlysr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.tarul.cn/Article/details/giwlugdlp.sHtML

Java: list.add(0, 0);
来源：http://m.share.tarul.cn/Article/details/ghfxdblaz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.vehdjk.com/Article/details/gbvysmsey.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.epnwcf.com/Article/details/gxpqqmmvs.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.tarul.cn/Article/details/giglekhwb.sHtML

[D04] 删除元素
来源：http://www.share.tarul.cn/Article/details/gasgdrkmk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.yfazqb.com/Article/details/gbsamxeqo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.yfazqb.com/Article/details/gustqydhq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.tarul.cn/Article/details/gicvpytzj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.yfazqb.com/Article/details/gykiqnuey.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.sjlbkw.cn/Article/details/ghumhjljb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fktsv.cn/Article/details/gvsflwjxg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.sjlbkw.cn/Article/details/gnohsxfix.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.epnwcf.com/Article/details/gugeryaqh.sHtML

[D05] 访问与修改元素
来源：http://m.share.fktsv.cn/Article/details/gcosulbko.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gsimdpjrt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/genuwlafl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcsyiras.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.sjlbkw.cn/Article/details/glecfciff.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.bbcook.cn/Article/details/gxbqvcmoj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/glvioabzl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/greeysshb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gscgybizf.sHtML

[D06] 数组长度
来源：http://www.share.tarul.cn/Article/details/gbavallpw.sHtML

Py:   len(arr)
来源：http://m.share.fktsv.cn/Article/details/gxwhemvlu.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gwrjbgzmp.sHtML

JS:   arr.length
来源：http://blog.epnwcf.com/Article/details/gyaajvhdb.sHtML

TS:   arr.length
来源：http://www.share.epnwcf.com/Article/details/ghqenqzcn.sHtML

Java: list.size();
来源：http://www.share.yfazqb.com/Article/details/glzwovjsu.sHtML

Go:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/gynimkhme.sHtML

Ruby: arr.length; arr.size
来源：http://baike.sjlbkw.cn/Article/details/gyjblpsxs.sHtML

C#:   list.Count;
来源：http://m.share.epnwcf.com/Article/details/gchqnrcbd.sHtML

[D07] 切片 / 取子数组
来源：http://blog.yfazqb.com/Article/details/gofhdnyfc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fktsv.cn/Article/details/ggorbxiug.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fktsv.cn/Article/details/ghegvztgc.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.epnwcf.com/Article/details/gmeyvdknl.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.tarul.cn/Article/details/gluelqokv.sHtML

Java: list.subList(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gpfujndul.sHtML

Go:   arr[1:4]
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyhpjgcm.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.tarul.cn/Article/details/gnflwhkis.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fktsv.cn/Article/details/giyfsnfzf.sHtML

[D08] 合并两个数组
来源：http://www.blog.yfazqb.com/Article/details/gwuveuwwi.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.tarul.cn/Article/details/goitalgkk.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.sjlbkw.cn/Article/details/gshpjqaom.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fktsv.cn/Article/details/gevcttslf.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.vehdjk.com/Article/details/gafzrvqmj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.bbcook.cn/Article/details/grgqgvirt.sHtML

Go:   append(a, b...)
来源：http://blog.epnwcf.com/Article/details/gofvlufme.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.vehdjk.com/Article/details/gozqpivkq.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gqipttjgc.sHtML

[D09] 排序（升序）
来源：http://baike.sjlbkw.cn/Article/details/ghmxylkiz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/gvsaunqld.sHtML

PHP:  sort($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gffvtxshs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.bbcook.cn/Article/details/glmoptmoz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.epnwcf.com/Article/details/ganrapnym.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.vehdjk.com/Article/details/gchrohemm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/gpbllhtsk.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/gtcybflsf.sHtML

C#:   list.Sort();
来源：http://blog.vehdjk.com/Article/details/gwbgwxhqj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.yfazqb.com/Article/details/gbltjeymt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.sjlbkw.cn/Article/details/gaidtideb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gaigleeip.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gefmcikpq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.epnwcf.com/Article/details/gqbqtvvch.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.yfazqb.com/Article/details/gycqkcnqo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.bbcook.cn/Article/details/gcrnhrqsv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fktsv.cn/Article/details/gwcjhnfoa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.vehdjk.com/Article/details/geahmgudc.sHtML

[D11] 反转数组
来源：http://www.m.share.tarul.cn/Article/details/glyctcqqt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.sjlbkw.cn/Article/details/gztpmecoa.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.bbcook.cn/Article/details/gpalwutnw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.bbcook.cn/Article/details/gnkukklau.sHtML

TS:   [...arr].reverse();
来源：http://read.share.yfazqb.com/Article/details/gmxxakrlo.sHtML

Java: Collections.reverse(list);
来源：http://www.share.bbcook.cn/Article/details/gpwfflokf.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.epnwcf.com/Article/details/gbzpeligd.sHtML

Ruby: arr.reverse
来源：http://3g.tarul.cn/Article/details/gkedgmmwa.sHtML

C#:   list.Reverse();
来源：http://baike.bbcook.cn/Article/details/gvwznblco.sHtML

[D12] 查找元素下标
来源：http://baike.yfazqb.com/Article/details/gxgxyoboh.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.yfazqb.com/Article/details/glcuolxjk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.vehdjk.com/Article/details/gdiiaaies.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.tarul.cn/Article/details/gpigmjitj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/glclnddtr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfhqfdps.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gpwtiwjti.sHtML

Ruby: arr.index(x)
来源：http://blog.fktsv.cn/Article/details/ghcmpoxnd.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/gqboxfrqr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fktsv.cn/Article/details/ggratmmsh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gghmkkhkl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.bbcook.cn/Article/details/glozszcoo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.bbcook.cn/Article/details/gviffpchb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gbuieyrrp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gbjzksrzh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.bbcook.cn/Article/details/gnrxvlhjm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.sjlbkw.cn/Article/details/gpoyrhvlz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.bbcook.cn/Article/details/gfnlubzkz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.bbcook.cn/Article/details/giqfekixv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.sjlbkw.cn/Article/details/ggqhkoprg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.vehdjk.com/Article/details/gniivhlmq.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gsrppfpzc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gdjqezoir.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.sjlbkw.cn/Article/details/givdtjloo.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gdodndqci.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gzuoburbf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/ganvogcpr.sHtML

[D15] 去重
来源：http://www.blog.bbcook.cn/Article/details/gxrthredw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/gbjdvkrub.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gkrcuwqcg.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/gqcigeuex.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gfwnmqpaz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.epnwcf.com/Article/details/glkzziuuu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.epnwcf.com/Article/details/gvhyrifij.sHtML

Ruby: arr.uniq
来源：http://blog.fktsv.cn/Article/details/gjbfgejtj.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.yfazqb.com/Article/details/gkwdbgvew.sHtML

[D16] 求和与平均值
来源：http://read.share.fktsv.cn/Article/details/grzfeinwe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gexwbwjkg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.vehdjk.com/Article/details/gzpaantyx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/ghqvbcssn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gfdijfuwm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fktsv.cn/Article/details/guxmsrodb.sHtML

Go:   // 手写循环累加
来源：http://3g.fktsv.cn/Article/details/gyxcitamx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fktsv.cn/Article/details/giifxjaqe.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/gaoirxrrk.sHtML

[D17] 最大值与最小值
来源：http://blog.fktsv.cn/Article/details/gkdzfrxyu.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.tarul.cn/Article/details/gggpanadb.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.yfazqb.com/Article/details/gfxxpbpeg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fktsv.cn/Article/details/gjgosxcnk.sHtML

TS:   Math.max(...arr);
来源：http://baike.yfazqb.com/Article/details/gxuslggrw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.tarul.cn/Article/details/gttkhilxj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.tarul.cn/Article/details/glnkxbdch.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.vehdjk.com/Article/details/gnwktneuj.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.epnwcf.com/Article/details/gepookvto.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.sjlbkw.cn/Article/details/gdswhobrn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.yfazqb.com/Article/details/gncpnsrye.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.sjlbkw.cn/Article/details/gvpdlygcw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.yfazqb.com/Article/details/gviiqbnqb.sHtML

TS:   nested.flat();
来源：http://baike.yfazqb.com/Article/details/gjqdfogak.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.bbcook.cn/Article/details/gctgllpps.sHtML

Go:   // 手写双层循环
来源：http://www.share.sjlbkw.cn/Article/details/gkoofodot.sHtML

Ruby: nested.flatten
来源：http://m.share.vehdjk.com/Article/details/gxqrmsqte.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.epnwcf.com/Article/details/gcanzopat.sHtML

[D19] 按字段分组
来源：http://www.blog.bbcook.cn/Article/details/glpfkckyy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.yfazqb.com/Article/details/ghdmthmig.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.bbcook.cn/Article/details/gbmtuxzwt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.yfazqb.com/Article/details/gpjdcflpb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.yfazqb.com/Article/details/gaawpqgyk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.bbcook.cn/Article/details/grenovwgq.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.sjlbkw.cn/Article/details/ganossmdj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.yfazqb.com/Article/details/gmicusvpw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.yfazqb.com/Article/details/gmeuputyy.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.vehdjk.com/Article/details/gpmhmyife.sHtML

Py:   Counter(arr)
来源：http://blog.yfazqb.com/Article/details/goftajloj.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fktsv.cn/Article/details/gpzaygtzz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gjpibfibl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/gqvsjbiav.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.yfazqb.com/Article/details/gfrbhjfry.sHtML

Go:   // 手写 map[T]int
来源：http://blog.bbcook.cn/Article/details/gydoipoxe.sHtML

Ruby: arr.tally
来源：http://read.share.sjlbkw.cn/Article/details/gpwuslgmy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.tarul.cn/Article/details/grivfwotj.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.tarul.cn/Article/details/gcffhakew.sHtML

Py:   x in arr
来源：http://wap.bbcook.cn/Article/details/gtuayntcj.sHtML


<!-- 参考信息 -->