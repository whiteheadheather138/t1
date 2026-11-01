代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.m.share.yfazqb.com/Article/details/ggnuofylj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gcexnvqxe.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gusqzipqh.sHtML

[C05] 返回多个值
来源：http://read.share.vehdjk.com/Article/details/gmmscunei.sHtML

Py:   return a, b
来源：http://mobile.fktsv.cn/Article/details/gfizucllc.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.sjlbkw.cn/Article/details/gnaidyvhl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.tarul.cn/Article/details/gxajtjqfh.sHtML

TS:   return { a, b };
来源：http://www.share.bbcook.cn/Article/details/gsxymfprd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.vehdjk.com/Article/details/glqzhbphd.sHtML

Go:   return a, b
来源：http://baike.epnwcf.com/Article/details/goywdhmtf.sHtML

Ruby: return a, b
来源：http://www.blog.yfazqb.com/Article/details/giczzufqv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.bbcook.cn/Article/details/gjeqrxvdh.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.epnwcf.com/Article/details/gqbsgxuxa.sHtML

Py:   square = lambda x: x * x
来源：http://baike.vehdjk.com/Article/details/gsjagcwsq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.yfazqb.com/Article/details/grhlokgao.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gaebvexwt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.epnwcf.com/Article/details/grfywloko.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.epnwcf.com/Article/details/gkgihvmvk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gmzupugjq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fktsv.cn/Article/details/gedvgmarh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.vehdjk.com/Article/details/gybjgjunk.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.tarul.cn/Article/details/gnqshokbb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.vehdjk.com/Article/details/gzyasvbqz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gxnuhczbr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.tarul.cn/Article/details/gfxymvomy.sHtML

TS:   arr.map(String)
来源：http://mobile.sjlbkw.cn/Article/details/gejrazkwd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.yfazqb.com/Article/details/gcllmfhqm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.epnwcf.com/Article/details/ghxzwxenv.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.sjlbkw.cn/Article/details/gdbztebvd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.vehdjk.com/Article/details/gebkwxqne.sHtML

[C08] 闭包
来源：http://baike.yfazqb.com/Article/details/gulxuabmi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.sjlbkw.cn/Article/details/gbdtoiztr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.bbcook.cn/Article/details/gepnviqwx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gxfjtbdoo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/glpliuvtk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.sjlbkw.cn/Article/details/gdhilcjhf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.sjlbkw.cn/Article/details/gbehdoeda.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.tarul.cn/Article/details/gexsumfjh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gpeshihgs.sHtML

[C09] 递归
来源：http://mobile.yfazqb.com/Article/details/gzxixyhpx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gyaomjsld.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gyemqxwxb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/gmftlphlg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/gldjxitge.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.yfazqb.com/Article/details/gngzgyuvt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.tarul.cn/Article/details/gtmtrviib.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/ggvjbrawi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.sjlbkw.cn/Article/details/gnfebyxna.sHtML

[C10] 变量作用域
来源：http://www.blog.yfazqb.com/Article/details/gjkjqnwkb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.bbcook.cn/Article/details/gxssidnaz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.epnwcf.com/Article/details/gloiqhaph.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.vehdjk.com/Article/details/gvjusohcj.sHtML

TS:   同 JS
来源：http://www.blog.vehdjk.com/Article/details/gkoiygdhj.sHtML

Java: 方法内为块级作用域
来源：http://3g.yfazqb.com/Article/details/gxiqthkdc.sHtML

Go:   花括号块级作用域
来源：http://wap.epnwcf.com/Article/details/gxucyhpnd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.tarul.cn/Article/details/gfokfxmfh.sHtML

C#:   块级作用域
来源：http://m.share.tarul.cn/Article/details/ggasucmqn.sHtML

[C11] 模块导入与导出
来源：http://3g.yfazqb.com/Article/details/geewqunlw.sHtML

Py:   from module import func
来源：http://baike.epnwcf.com/Article/details/gsfjmdvkp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.tarul.cn/Article/details/gdennxsff.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.tarul.cn/Article/details/gjtzqysls.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.bbcook.cn/Article/details/gnvhoxhta.sHtML

Java: import java.util.List;
来源：http://m.share.bbcook.cn/Article/details/gxjvqlbzd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.yfazqb.com/Article/details/gqozkikea.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fktsv.cn/Article/details/gzdlmduyx.sHtML

C#:   using System.Text;
来源：http://baike.epnwcf.com/Article/details/gsfdhypwq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgzoxrdv.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.yfazqb.com/Article/details/gtbbgvljf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fktsv.cn/Article/details/gdhogmlbq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gzxkfylxe.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/goyyeyget.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.bbcook.cn/Article/details/gwaowswuh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fktsv.cn/Article/details/gffcpnref.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.sjlbkw.cn/Article/details/gzhtrvojn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.tarul.cn/Article/details/gsplzapgq.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.vehdjk.com/Article/details/gggnhzhez.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.tarul.cn/Article/details/gbgfzcrov.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gquequqzd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.vehdjk.com/Article/details/gacrtcebt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gjjzyphvg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gwtdcdhhi.sHtML

Go:   func add(a, b int) int
来源：http://wap.sjlbkw.cn/Article/details/gyivfilvo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.epnwcf.com/Article/details/gpmvjvqer.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fktsv.cn/Article/details/gqtmxumix.sHtML

[C14] 泛型函数
来源：http://www.blog.bbcook.cn/Article/details/gfwipcsaq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.sjlbkw.cn/Article/details/gbgaiptbe.sHtML

PHP:  // 无泛型
来源：http://read.share.yfazqb.com/Article/details/gvushtxkr.sHtML

JS:   // 无泛型
来源：http://baike.fktsv.cn/Article/details/gloimhwdy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.bbcook.cn/Article/details/ghzhcisno.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.tarul.cn/Article/details/gqjleimzf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.bbcook.cn/Article/details/gvldtdiub.sHtML

Ruby: # 无泛型
来源：http://m.share.fktsv.cn/Article/details/gamidymmx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.tarul.cn/Article/details/gfdmaahzo.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.sjlbkw.cn/Article/details/ghuftzolg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.tarul.cn/Article/details/gcxspcpyy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/gccienfzf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gnrszrakm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fktsv.cn/Article/details/gimzbrknk.sHtML

Java: // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/gpjgrexaw.sHtML

Go:   // 无解构
来源：http://m.share.bbcook.cn/Article/details/gcnmgerqw.sHtML

Ruby: a, b = pair
来源：http://baike.tarul.cn/Article/details/ginebzilm.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.vehdjk.com/Article/details/gtvunhylw.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.bbcook.cn/Article/details/gfyynxdzz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.epnwcf.com/Article/details/gbbfydipy.sHtML

PHP:  // 无重载
来源：http://baike.fktsv.cn/Article/details/gcwxgaypl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.epnwcf.com/Article/details/grpqvumpf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fktsv.cn/Article/details/gajrlporv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.epnwcf.com/Article/details/gbitukpur.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/gzzasxzsm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.yfazqb.com/Article/details/gspgixkxd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fktsv.cn/Article/details/gtycjckfk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gezpemplj.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.bbcook.cn/Article/details/gyoxaahsc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gyrpugxdq.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.vehdjk.com/Article/details/gjkburgkr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.yfazqb.com/Article/details/golhmcubt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.yfazqb.com/Article/details/gxijgjjxk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.vehdjk.com/Article/details/gxnwdvvup.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.vehdjk.com/Article/details/gdlcvujka.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.tarul.cn/Article/details/gklpnmlge.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.sjlbkw.cn/Article/details/ghvuyjwuh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.tarul.cn/Article/details/gbznqgjjy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.epnwcf.com/Article/details/gmwmbcnaa.sHtML

[D02] 追加元素到末尾
来源：http://read.share.tarul.cn/Article/details/grjtrienw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.vehdjk.com/Article/details/gfixlaith.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.vehdjk.com/Article/details/gwlgajgvl.sHtML

JS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/gtnghkdqv.sHtML

TS:   arr.push(4);
来源：http://www.share.sjlbkw.cn/Article/details/gboaiiyld.sHtML

Java: list.add(4);
来源：http://m.share.vehdjk.com/Article/details/guktqcwfl.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.tarul.cn/Article/details/gendgjakl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.tarul.cn/Article/details/gatfxvamb.sHtML

C#:   list.Add(4);
来源：http://read.share.sjlbkw.cn/Article/details/gfnjmcqry.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fktsv.cn/Article/details/gkwlfpveo.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.yfazqb.com/Article/details/gfbjqmbuw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.sjlbkw.cn/Article/details/gvilhgjde.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.yfazqb.com/Article/details/goqkgfqkk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fktsv.cn/Article/details/gmgqqwxrq.sHtML

Java: list.add(0, 0);
来源：http://mobile.tarul.cn/Article/details/gzqbwwzrg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.epnwcf.com/Article/details/gizopjoyo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.tarul.cn/Article/details/gyvqgkgkc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxeidnddf.sHtML

[D04] 删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/gxwefxmru.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fktsv.cn/Article/details/ggtajwdyy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fktsv.cn/Article/details/guuoocgsy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.sjlbkw.cn/Article/details/grbzofuqo.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.bbcook.cn/Article/details/gooikolml.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.epnwcf.com/Article/details/goatyzjyn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.bbcook.cn/Article/details/gnkucecol.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.bbcook.cn/Article/details/gnjudxfaw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.yfazqb.com/Article/details/gczimexzr.sHtML

[D05] 访问与修改元素
来源：http://m.share.bbcook.cn/Article/details/gokmejuwz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gouoovvyf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gjqjupfyn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gzxbbpuzj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fktsv.cn/Article/details/gbfyhxxdy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fktsv.cn/Article/details/grnfbqaqq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gpwvjmime.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/grbijuatz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/gwykfjwke.sHtML

[D06] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/gdlechnjg.sHtML

Py:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gzhpojxet.sHtML

PHP:  count($arr);
来源：http://baike.yfazqb.com/Article/details/gvvllaqip.sHtML

JS:   arr.length
来源：http://blog.bbcook.cn/Article/details/gtwhmqgoq.sHtML

TS:   arr.length
来源：http://3g.vehdjk.com/Article/details/groxrjjic.sHtML

Java: list.size();
来源：http://mobile.fktsv.cn/Article/details/grkjyipth.sHtML

Go:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/gdbrafjmb.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.tarul.cn/Article/details/gurfqakmu.sHtML

C#:   list.Count;
来源：http://blog.yfazqb.com/Article/details/gcfgbiqoz.sHtML

[D07] 切片 / 取子数组
来源：http://baike.tarul.cn/Article/details/glndbclip.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.epnwcf.com/Article/details/gnauvpgaq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.bbcook.cn/Article/details/gfzsioypo.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gjajourcr.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gapcbuutw.sHtML

Java: list.subList(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/guomvpawc.sHtML

Go:   arr[1:4]
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjonvfeg.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fktsv.cn/Article/details/guajshgjw.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.bbcook.cn/Article/details/gwolpajce.sHtML

[D08] 合并两个数组
来源：http://wap.bbcook.cn/Article/details/ghatcrvcc.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fktsv.cn/Article/details/gvfmufatc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.tarul.cn/Article/details/gibayscmj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fktsv.cn/Article/details/gekvqquqt.sHtML

TS:   [...a, ...b];
来源：http://blog.bbcook.cn/Article/details/gebxjftcv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.vehdjk.com/Article/details/gozxvxvqe.sHtML

Go:   append(a, b...)
来源：http://blog.fktsv.cn/Article/details/gjlddwomj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.epnwcf.com/Article/details/gqnpqqxnj.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gidmtvwpf.sHtML

[D09] 排序（升序）
来源：http://m.share.sjlbkw.cn/Article/details/ghqkbumnw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.vehdjk.com/Article/details/glgyoymde.sHtML

PHP:  sort($arr);
来源：http://www.blog.bbcook.cn/Article/details/grapdxgmv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.yfazqb.com/Article/details/gouvmbibp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.vehdjk.com/Article/details/gtafbjujp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fktsv.cn/Article/details/gizjmcsxf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gmesxfkop.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gakogbbkh.sHtML

C#:   list.Sort();
来源：http://m.share.bbcook.cn/Article/details/gpmflgriv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.epnwcf.com/Article/details/gbvsiprji.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.bbcook.cn/Article/details/guordpyej.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fktsv.cn/Article/details/gpkcavvjx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gldvgvpxd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.vehdjk.com/Article/details/gscdryikp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fktsv.cn/Article/details/gznbehobl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fktsv.cn/Article/details/gvntdxjwh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.yfazqb.com/Article/details/gqyukvzyt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.yfazqb.com/Article/details/gdymeslwo.sHtML

[D11] 反转数组
来源：http://baike.bbcook.cn/Article/details/gjzbmuezz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.epnwcf.com/Article/details/gmodyvotw.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fktsv.cn/Article/details/grbmnraao.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.yfazqb.com/Article/details/grjuokjrk.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.tarul.cn/Article/details/gzzuyfbrq.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/gksutqdft.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.epnwcf.com/Article/details/gecnsbqwe.sHtML

Ruby: arr.reverse
来源：http://blog.yfazqb.com/Article/details/ghbcyyfjq.sHtML

C#:   list.Reverse();
来源：http://www.share.bbcook.cn/Article/details/gllvqjbjp.sHtML

[D12] 查找元素下标
来源：http://www.m.share.epnwcf.com/Article/details/gbgoqegmz.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fktsv.cn/Article/details/guxjyzwpt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.epnwcf.com/Article/details/gwhfmjmri.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gxvfhbkfu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.tarul.cn/Article/details/gqtoobvrw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.sjlbkw.cn/Article/details/gfnxqifld.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.tarul.cn/Article/details/gizmxwlhv.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.tarul.cn/Article/details/gmddtpsur.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.bbcook.cn/Article/details/gkkoecbdl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.bbcook.cn/Article/details/ghqfmwmpg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.epnwcf.com/Article/details/grrtjdlsv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.tarul.cn/Article/details/guwvhruxc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/gxdzytsgd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fktsv.cn/Article/details/grfyzqpbz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.tarul.cn/Article/details/gienafrlc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.bbcook.cn/Article/details/gzzaqbqct.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.sjlbkw.cn/Article/details/giilcgxjz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.tarul.cn/Article/details/gkhgowuvq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.vehdjk.com/Article/details/grdxpztmn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.tarul.cn/Article/details/gxnfcmpci.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.tarul.cn/Article/details/gxvwxizxv.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/gjcmkikbp.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.tarul.cn/Article/details/gwjoshviz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.sjlbkw.cn/Article/details/goeybmbiv.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/gszutvcve.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.bbcook.cn/Article/details/gqdsiaonb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtagqjioa.sHtML

[D15] 去重
来源：http://wap.fktsv.cn/Article/details/gvdaddvsf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.sjlbkw.cn/Article/details/gjvsqzurx.sHtML

PHP:  array_unique($arr);
来源：http://blog.vehdjk.com/Article/details/ghvwtchgf.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gblyjtisq.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gqwhveoqz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fktsv.cn/Article/details/grwnepzzw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fktsv.cn/Article/details/gdyhpnzki.sHtML

Ruby: arr.uniq
来源：http://www.share.sjlbkw.cn/Article/details/giwwlaexb.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gsxfzepuz.sHtML

[D16] 求和与平均值
来源：http://www.m.share.bbcook.cn/Article/details/gpsajgsbo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.bbcook.cn/Article/details/gzkomukog.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.sjlbkw.cn/Article/details/ghubwlmxa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/gzbjqdqlw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fktsv.cn/Article/details/gzqbktpvd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.yfazqb.com/Article/details/gbnjqmeud.sHtML

Go:   // 手写循环累加
来源：http://baike.yfazqb.com/Article/details/gmohljyfh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gttakwnzz.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.vehdjk.com/Article/details/gclzttjfm.sHtML

[D17] 最大值与最小值
来源：http://www.share.yfazqb.com/Article/details/gzyykgpjs.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fktsv.cn/Article/details/gjscppgwo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fktsv.cn/Article/details/ggiocnxoq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.bbcook.cn/Article/details/gvtwqzrdr.sHtML

TS:   Math.max(...arr);
来源：http://read.share.yfazqb.com/Article/details/goryimtfc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.vehdjk.com/Article/details/gbgyaejzd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.tarul.cn/Article/details/gulcelclh.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.tarul.cn/Article/details/gjguisuqh.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fktsv.cn/Article/details/giwtbbsqh.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.tarul.cn/Article/details/grphdiemp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.vehdjk.com/Article/details/gbxthlpqr.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.vehdjk.com/Article/details/gwhnirzxn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fktsv.cn/Article/details/gpfjsyfyv.sHtML

TS:   nested.flat();
来源：http://www.share.vehdjk.com/Article/details/goqrarolg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.vehdjk.com/Article/details/gzjnkwgsd.sHtML

Go:   // 手写双层循环
来源：http://www.share.bbcook.cn/Article/details/gcvwulgam.sHtML

Ruby: nested.flatten
来源：http://blog.vehdjk.com/Article/details/gmvasbxyr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.vehdjk.com/Article/details/gumqbllzd.sHtML

[D19] 按字段分组
来源：http://baike.sjlbkw.cn/Article/details/gihondgfx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.sjlbkw.cn/Article/details/gsismnupq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fktsv.cn/Article/details/grvisydpv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.yfazqb.com/Article/details/gsyvlgbjm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/glfqnwwqy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.sjlbkw.cn/Article/details/gybkqpcfk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.bbcook.cn/Article/details/gjyevbfwy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.bbcook.cn/Article/details/gfnerbkdq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.sjlbkw.cn/Article/details/gconsmbic.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.epnwcf.com/Article/details/gamfotdlb.sHtML

Py:   Counter(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gmcbywnog.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fktsv.cn/Article/details/gjljlhmgz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fktsv.cn/Article/details/gfgpjamai.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gbcczhyni.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.tarul.cn/Article/details/gbhuvwwrh.sHtML

Go:   // 手写 map[T]int
来源：http://baike.epnwcf.com/Article/details/glajzzmwh.sHtML

Ruby: arr.tally
来源：http://blog.bbcook.cn/Article/details/gvqmsuvvj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.sjlbkw.cn/Article/details/gqxcclica.sHtML

[D21] 判断是否包含某元素
来源：http://baike.tarul.cn/Article/details/gefddycvr.sHtML

Py:   x in arr
来源：http://read.share.yfazqb.com/Article/details/gqzzacszm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.bbcook.cn/Article/details/glougzsps.sHtML

JS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/gopvqvllk.sHtML

TS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gyhlbmdwf.sHtML

Java: list.contains(x)
来源：http://www.share.bbcook.cn/Article/details/gaxfbugzr.sHtML


<!-- 参考信息 -->