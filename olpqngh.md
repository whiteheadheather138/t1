代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gisuwykgl.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.tarul.cn/Article/details/gzyvjtero.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fktsv.cn/Article/details/gndhqbdul.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fktsv.cn/Article/details/goxfrgmlu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.vehdjk.com/Article/details/gftdmxnex.sHtML

TS:   arr.map(String)
来源：http://m.share.epnwcf.com/Article/details/gruhhikuh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/gfmxavdsv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.yfazqb.com/Article/details/gaecahpcr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fktsv.cn/Article/details/gzvfiilta.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.tarul.cn/Article/details/gcqtoqcst.sHtML

[C08] 闭包
来源：http://3g.epnwcf.com/Article/details/gmheayxrp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.vehdjk.com/Article/details/gdegmjqcn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.sjlbkw.cn/Article/details/gakgvkhpi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/guwwjdgao.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/govatzunb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.sjlbkw.cn/Article/details/gozcrbyrr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.bbcook.cn/Article/details/gpnywyjgo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.bbcook.cn/Article/details/ghlfgewzu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gysvrtosy.sHtML

[C09] 递归
来源：http://www.blog.sjlbkw.cn/Article/details/gipfkiwwh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.tarul.cn/Article/details/guwvahbqb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fktsv.cn/Article/details/grdlfnrss.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.tarul.cn/Article/details/gwjzppufw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.epnwcf.com/Article/details/gvdugxjhv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.tarul.cn/Article/details/gvivncidh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.tarul.cn/Article/details/gecxnmvkh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/grnxiqhdl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.sjlbkw.cn/Article/details/gxvwjaarn.sHtML

[C10] 变量作用域
来源：http://wap.bbcook.cn/Article/details/gezkjqqvk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fktsv.cn/Article/details/gyrijontc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.yfazqb.com/Article/details/gvdsbwotn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fktsv.cn/Article/details/grxonfosy.sHtML

TS:   同 JS
来源：http://m.share.bbcook.cn/Article/details/grysxckcz.sHtML

Java: 方法内为块级作用域
来源：http://blog.yfazqb.com/Article/details/gphgqopgf.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gulkaxaiw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.sjlbkw.cn/Article/details/gdvzupzem.sHtML

C#:   块级作用域
来源：http://mobile.bbcook.cn/Article/details/gggosljvm.sHtML

[C11] 模块导入与导出
来源：http://www.blog.tarul.cn/Article/details/gzemzlfqy.sHtML

Py:   from module import func
来源：http://blog.sjlbkw.cn/Article/details/gbvwigeen.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.yfazqb.com/Article/details/glhsnraxn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.tarul.cn/Article/details/gsuzcqjgc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.sjlbkw.cn/Article/details/gadnyngqk.sHtML

Java: import java.util.List;
来源：http://mobile.yfazqb.com/Article/details/gnkofdokr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.sjlbkw.cn/Article/details/gakhlfkeu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.vehdjk.com/Article/details/gcaczeygu.sHtML

C#:   using System.Text;
来源：http://www.blog.fktsv.cn/Article/details/gyraicicp.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.sjlbkw.cn/Article/details/gexerlrrg.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fktsv.cn/Article/details/gfstesblx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.sjlbkw.cn/Article/details/gzjbidkux.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/gfghwbknb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzurjdcr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.tarul.cn/Article/details/ggdohxkcw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fktsv.cn/Article/details/gnewbgins.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.vehdjk.com/Article/details/gdrsmzpkv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.tarul.cn/Article/details/gvdkeoljm.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.sjlbkw.cn/Article/details/gwzgyysjn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.epnwcf.com/Article/details/gfylacmaa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gnbkdzauf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.tarul.cn/Article/details/gwwaxmvvk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gqiergnph.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gymbsymny.sHtML

Go:   func add(a, b int) int
来源：http://blog.vehdjk.com/Article/details/gxiwturzl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.tarul.cn/Article/details/gqgiebyrn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fktsv.cn/Article/details/gdsirzvqy.sHtML

[C14] 泛型函数
来源：http://blog.sjlbkw.cn/Article/details/gkzirmcnb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.bbcook.cn/Article/details/gzdjqhepq.sHtML

PHP:  // 无泛型
来源：http://wap.epnwcf.com/Article/details/grbkzwate.sHtML

JS:   // 无泛型
来源：http://baike.yfazqb.com/Article/details/gsibkdrgq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.tarul.cn/Article/details/gfnfquaka.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.bbcook.cn/Article/details/ggcesiqzh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.vehdjk.com/Article/details/gblxtqdsk.sHtML

Ruby: # 无泛型
来源：http://m.share.fktsv.cn/Article/details/gkkjbjlrh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.bbcook.cn/Article/details/gmbiyacni.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.bbcook.cn/Article/details/ghviyfeda.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.vehdjk.com/Article/details/gajuvkmmm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.vehdjk.com/Article/details/gnjcsitae.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/gcryvdjpw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.bbcook.cn/Article/details/gybiiyhea.sHtML

Java: // 无解构
来源：http://wap.vehdjk.com/Article/details/gortgximj.sHtML

Go:   // 无解构
来源：http://baike.yfazqb.com/Article/details/ggiyulcpq.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fktsv.cn/Article/details/gyhmgvvzf.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.epnwcf.com/Article/details/givzzabjy.sHtML

[C16] 函数 / 方法重载
来源：http://blog.yfazqb.com/Article/details/gpedqdbbm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.bbcook.cn/Article/details/gcmydterz.sHtML

PHP:  // 无重载
来源：http://m.share.fktsv.cn/Article/details/gvsjygvwo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.vehdjk.com/Article/details/grfmhfdek.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fktsv.cn/Article/details/gitodkftb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fktsv.cn/Article/details/gengitjlv.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.sjlbkw.cn/Article/details/gsilletxb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.sjlbkw.cn/Article/details/ghhlwogsv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.sjlbkw.cn/Article/details/gvkkqqzvg.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gnprpzdhc.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.bbcook.cn/Article/details/gdhsacuuf.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ggnwxprob.sHtML

[D01] 创建数组 / 列表
来源：http://3g.sjlbkw.cn/Article/details/ghodlvjka.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.tarul.cn/Article/details/glanqwzjf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.yfazqb.com/Article/details/gawgucuex.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/gecnugltj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.epnwcf.com/Article/details/gjdikhpil.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fktsv.cn/Article/details/gyxrwamka.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.bbcook.cn/Article/details/gdenxkqtb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gfdtlnidm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.yfazqb.com/Article/details/gymtszrel.sHtML

[D02] 追加元素到末尾
来源：http://3g.tarul.cn/Article/details/gztclgndr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.tarul.cn/Article/details/gymyoanbz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gbakdqqlx.sHtML

JS:   arr.push(4);
来源：http://wap.vehdjk.com/Article/details/goomxqkmn.sHtML

TS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gzvgprtaf.sHtML

Java: list.add(4);
来源：http://www.share.epnwcf.com/Article/details/gitsfahjb.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.sjlbkw.cn/Article/details/gyvsiwtxy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.tarul.cn/Article/details/gsysuhrtu.sHtML

C#:   list.Add(4);
来源：http://baike.bbcook.cn/Article/details/gubwnrhdh.sHtML

[D03] 在指定位置插入元素
来源：http://baike.vehdjk.com/Article/details/grerqndtu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.yfazqb.com/Article/details/gugleweyf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.bbcook.cn/Article/details/gokhstiaz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.sjlbkw.cn/Article/details/gqrwrtsry.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.epnwcf.com/Article/details/guffmwjmn.sHtML

Java: list.add(0, 0);
来源：http://3g.tarul.cn/Article/details/gcrbvpylz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.bbcook.cn/Article/details/gdbczmadw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.tarul.cn/Article/details/gdflctokh.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.bbcook.cn/Article/details/grccyqqtt.sHtML

[D04] 删除元素
来源：http://www.share.fktsv.cn/Article/details/gpglgobbu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.yfazqb.com/Article/details/gjlaoiepr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fktsv.cn/Article/details/grbzhcrud.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fktsv.cn/Article/details/gtxwbnoym.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.sjlbkw.cn/Article/details/gysfobyvo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.bbcook.cn/Article/details/gjprptdwq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fktsv.cn/Article/details/gzgkpvkgr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.tarul.cn/Article/details/gutbjepeb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.tarul.cn/Article/details/gpbivtama.sHtML

[D05] 访问与修改元素
来源：http://www.blog.yfazqb.com/Article/details/gcnezevpo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/gyensdkov.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gbdnzhfrw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/glkgjsfrs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.sjlbkw.cn/Article/details/geblfdtnk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fktsv.cn/Article/details/gvphpkrse.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gtzxofygl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gjipmtgbb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/gcmoliowj.sHtML

[D06] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gtnxydpdv.sHtML

Py:   len(arr)
来源：http://mobile.fktsv.cn/Article/details/gvlzspfbq.sHtML

PHP:  count($arr);
来源：http://3g.vehdjk.com/Article/details/glqpzqbrv.sHtML

JS:   arr.length
来源：http://blog.bbcook.cn/Article/details/gdqgouhzb.sHtML

TS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/gjayqlxsp.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/gtxdzjuct.sHtML

Go:   len(arr)
来源：http://mobile.fktsv.cn/Article/details/gdqehwitg.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.tarul.cn/Article/details/gdqvajqiq.sHtML

C#:   list.Count;
来源：http://www.m.share.sjlbkw.cn/Article/details/glusnampm.sHtML

[D07] 切片 / 取子数组
来源：http://blog.epnwcf.com/Article/details/gscserrhm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.vehdjk.com/Article/details/gjknafscr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.tarul.cn/Article/details/ggojkpmct.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gngvhuoex.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gfdkkhwsx.sHtML

Java: list.subList(1, 4);
来源：http://read.share.yfazqb.com/Article/details/glxhcqfei.sHtML

Go:   arr[1:4]
来源：http://m.share.sjlbkw.cn/Article/details/gekshgorc.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.tarul.cn/Article/details/gtnmkazxk.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gncmxhyzm.sHtML

[D08] 合并两个数组
来源：http://blog.bbcook.cn/Article/details/gvqblzteg.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.epnwcf.com/Article/details/grwnqdjta.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.vehdjk.com/Article/details/gsxnoydom.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.yfazqb.com/Article/details/grwvtxhaz.sHtML

TS:   [...a, ...b];
来源：http://mobile.fktsv.cn/Article/details/gypzwpumc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gpqhdpjos.sHtML

Go:   append(a, b...)
来源：http://mobile.sjlbkw.cn/Article/details/ghxzcrrys.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fktsv.cn/Article/details/ghtwfwkaz.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.epnwcf.com/Article/details/gwivqflbv.sHtML

[D09] 排序（升序）
来源：http://m.share.vehdjk.com/Article/details/gtkiahnnn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/gfpstaslr.sHtML

PHP:  sort($arr);
来源：http://blog.epnwcf.com/Article/details/gtlybqlnw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.vehdjk.com/Article/details/gsossrxyx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.yfazqb.com/Article/details/ghrhyozhx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.sjlbkw.cn/Article/details/gwdszimvi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fktsv.cn/Article/details/glbnmtrve.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/gukortkuy.sHtML

C#:   list.Sort();
来源：http://baike.sjlbkw.cn/Article/details/gpyklpjex.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fktsv.cn/Article/details/gyvrhdahm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.yfazqb.com/Article/details/gnatutujw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/gslyvrvft.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fktsv.cn/Article/details/gpnrryljz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gttybwcvw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.tarul.cn/Article/details/gnkdrvtfq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.sjlbkw.cn/Article/details/gkbafbgwb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.tarul.cn/Article/details/gkwkowyvh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.sjlbkw.cn/Article/details/gupmzcrfd.sHtML

[D11] 反转数组
来源：http://wap.epnwcf.com/Article/details/gvsribuli.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fktsv.cn/Article/details/gngpjflyq.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.epnwcf.com/Article/details/gibqpwbuo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fktsv.cn/Article/details/ggbmgcpxh.sHtML

TS:   [...arr].reverse();
来源：http://read.share.yfazqb.com/Article/details/ghfhndnuv.sHtML

Java: Collections.reverse(list);
来源：http://blog.vehdjk.com/Article/details/gzzdsvukn.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fktsv.cn/Article/details/gvdsnycsk.sHtML

Ruby: arr.reverse
来源：http://www.share.vehdjk.com/Article/details/gczqwdhaz.sHtML

C#:   list.Reverse();
来源：http://www.m.share.yfazqb.com/Article/details/gnedtubys.sHtML

[D12] 查找元素下标
来源：http://3g.epnwcf.com/Article/details/ggcdxwooh.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.sjlbkw.cn/Article/details/gapixdltc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.bbcook.cn/Article/details/gimlhhnss.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gumhamhab.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/gcjvmrgfi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.yfazqb.com/Article/details/gypkyggnv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gwdpbjohz.sHtML

Ruby: arr.index(x)
来源：http://3g.sjlbkw.cn/Article/details/gnwpmjmhx.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.epnwcf.com/Article/details/gnjniloux.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.tarul.cn/Article/details/gsjjcvyro.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.sjlbkw.cn/Article/details/gkspqmuxg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.sjlbkw.cn/Article/details/gnkqheqfk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gvunwaiep.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gppuecvsa.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.tarul.cn/Article/details/gabgoqmqk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.epnwcf.com/Article/details/gerikhodk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.epnwcf.com/Article/details/goodlfykn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.vehdjk.com/Article/details/gwndlerjy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.sjlbkw.cn/Article/details/glmqxgnsh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gxsdrzhzs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.bbcook.cn/Article/details/gxintdrmh.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/goobrrtjg.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/gmsbeiqul.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.bbcook.cn/Article/details/gskulcmiv.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/grhdpxnxw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.bbcook.cn/Article/details/gzjirjist.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gnhesmnpf.sHtML

[D15] 去重
来源：http://m.share.sjlbkw.cn/Article/details/gebtvhiut.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gonvqvdsn.sHtML

PHP:  array_unique($arr);
来源：http://m.share.epnwcf.com/Article/details/gdnleqapw.sHtML

JS:   [...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/gdxhuuigi.sHtML

TS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gtmstlzem.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fktsv.cn/Article/details/giybtmsvm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.vehdjk.com/Article/details/gxrbkhdtl.sHtML

Ruby: arr.uniq
来源：http://m.share.bbcook.cn/Article/details/gtrdmcjzi.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.yfazqb.com/Article/details/gkohjytfx.sHtML

[D16] 求和与平均值
来源：http://www.share.sjlbkw.cn/Article/details/gnxgxzzue.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.vehdjk.com/Article/details/gyuepecpc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.vehdjk.com/Article/details/gjyrykolv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/gwfudqqmq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/gzxklgpop.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.bbcook.cn/Article/details/gyyctaknt.sHtML

Go:   // 手写循环累加
来源：http://3g.fktsv.cn/Article/details/gkndczvqv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.bbcook.cn/Article/details/gslbjrrbr.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.yfazqb.com/Article/details/glymletoy.sHtML

[D17] 最大值与最小值
来源：http://3g.sjlbkw.cn/Article/details/gsmyljcuq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.epnwcf.com/Article/details/gufjuwcgi.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fktsv.cn/Article/details/grqnstwei.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.sjlbkw.cn/Article/details/gjlmtrmqg.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/gbphikgvd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.vehdjk.com/Article/details/gyislhnrr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.bbcook.cn/Article/details/gmhfwpamy.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fktsv.cn/Article/details/gmzqzccpv.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.sjlbkw.cn/Article/details/gyuarrvdh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.tarul.cn/Article/details/grqpcbmmn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.yfazqb.com/Article/details/gylpjmmqv.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.tarul.cn/Article/details/gkmagcmdi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.tarul.cn/Article/details/ghrtdtiav.sHtML

TS:   nested.flat();
来源：http://baike.sjlbkw.cn/Article/details/grdbxhvjq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fktsv.cn/Article/details/gpiekikzl.sHtML

Go:   // 手写双层循环
来源：http://mobile.yfazqb.com/Article/details/gpcctsfmq.sHtML

Ruby: nested.flatten
来源：http://www.blog.fktsv.cn/Article/details/gnqbekyph.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.vehdjk.com/Article/details/gwzmlfjcl.sHtML

[D19] 按字段分组
来源：http://3g.bbcook.cn/Article/details/ggbemwuoc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.sjlbkw.cn/Article/details/gfnnijesj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.vehdjk.com/Article/details/gmtnrlzjb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.vehdjk.com/Article/details/grrgfcfzk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.tarul.cn/Article/details/gonccoijk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.yfazqb.com/Article/details/gacmhxbrx.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fktsv.cn/Article/details/glfvjlrum.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.bbcook.cn/Article/details/gdydyswct.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.bbcook.cn/Article/details/ghvzbuklz.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.bbcook.cn/Article/details/gvgmmedqv.sHtML

Py:   Counter(arr)
来源：http://blog.bbcook.cn/Article/details/gnhkfukis.sHtML

PHP:  array_count_values($arr);
来源：http://baike.yfazqb.com/Article/details/grsmgxgur.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/gmorlmpei.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gjmvebnak.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fktsv.cn/Article/details/gyprlhmjp.sHtML

Go:   // 手写 map[T]int
来源：http://baike.bbcook.cn/Article/details/gwcswqaeh.sHtML

Ruby: arr.tally
来源：http://mobile.fktsv.cn/Article/details/gexdbcmqp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.yfazqb.com/Article/details/guoovorik.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.tarul.cn/Article/details/goaveggyg.sHtML

Py:   x in arr
来源：http://www.share.sjlbkw.cn/Article/details/gkurwoveh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.epnwcf.com/Article/details/gpjhlcznu.sHtML

JS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gvkwxpust.sHtML

TS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gpgbtijoz.sHtML

Java: list.contains(x)
来源：http://www.share.fktsv.cn/Article/details/gouctlhcu.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gdyvkcxcx.sHtML

Ruby: arr.include?(x)
来源：http://baike.bbcook.cn/Article/details/gbwxomngr.sHtML

C#:   list.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gfafetxwp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fktsv.cn/Article/details/gnlflvhen.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.epnwcf.com/Article/details/gkaxbiazm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.bbcook.cn/Article/details/gwmkimybb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.bbcook.cn/Article/details/gzysnrjkj.sHtML

TS:   [...arr];
来源：http://m.share.vehdjk.com/Article/details/gocqtbqzk.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.vehdjk.com/Article/details/gwfiwzbou.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.bbcook.cn/Article/details/gfhlmdqdu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fktsv.cn/Article/details/guiaeaqqq.sHtML

C#:   new List<int>(list);
来源：http://baike.tarul.cn/Article/details/gebfottwc.sHtML

[D23] reduce 累积计算
来源：http://baike.tarul.cn/Article/details/ghxvgrykm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fktsv.cn/Article/details/gcnnwoxkp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.yfazqb.com/Article/details/gxfmozwgw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gqyleffrc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/glgivgjkk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.epnwcf.com/Article/details/gnfkxjixp.sHtML

Go:   // 手写循环
来源：http://www.m.share.bbcook.cn/Article/details/gqgqdqlqa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.bbcook.cn/Article/details/gefvcngfc.sHtML


<!-- 参考信息 -->