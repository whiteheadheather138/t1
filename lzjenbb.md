代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://blog.vehdjk.com/Article/details/gxwwozyea.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.sjlbkw.cn/Article/details/gatynmutp.sHtML

[C08] 闭包
来源：http://www.m.share.vehdjk.com/Article/details/ghgrkyyoh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.yfazqb.com/Article/details/giyyjwlsy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.epnwcf.com/Article/details/gcwypfsqg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/geegkrzep.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gkyoaewns.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.sjlbkw.cn/Article/details/gppmhetzu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.vehdjk.com/Article/details/gdojvmqiu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.yfazqb.com/Article/details/goxawpbgn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/grzjhlkbx.sHtML

[C09] 递归
来源：http://m.share.bbcook.cn/Article/details/gjvvpbvch.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/gaijkhzui.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.epnwcf.com/Article/details/gleczxzqn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/gnvjgwkop.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/guyxgepnp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.epnwcf.com/Article/details/gqsdeokvb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fktsv.cn/Article/details/gjyksjmut.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/guxkndjdq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.tarul.cn/Article/details/gwmgbxnls.sHtML

[C10] 变量作用域
来源：http://blog.tarul.cn/Article/details/gtkkeukqk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.yfazqb.com/Article/details/glytixoxk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.epnwcf.com/Article/details/ggwafrgoy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.epnwcf.com/Article/details/gxuwwurqd.sHtML

TS:   同 JS
来源：http://www.m.share.tarul.cn/Article/details/gextyaomf.sHtML

Java: 方法内为块级作用域
来源：http://read.share.tarul.cn/Article/details/gidjidrba.sHtML

Go:   花括号块级作用域
来源：http://baike.bbcook.cn/Article/details/gqsnoagkj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.vehdjk.com/Article/details/gvglucnqr.sHtML

C#:   块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gvvzzjzgv.sHtML

[C11] 模块导入与导出
来源：http://baike.yfazqb.com/Article/details/gxesirnnz.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/gsklzbeau.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.tarul.cn/Article/details/geypjlqxa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fktsv.cn/Article/details/gpjliyjow.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.tarul.cn/Article/details/gfjkmwwdp.sHtML

Java: import java.util.List;
来源：http://m.share.bbcook.cn/Article/details/gezgaoedc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.sjlbkw.cn/Article/details/gnbxtwtjp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.sjlbkw.cn/Article/details/gupvwpsip.sHtML

C#:   using System.Text;
来源：http://m.share.yfazqb.com/Article/details/gsyewqhro.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fktsv.cn/Article/details/gvwvhwpds.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.tarul.cn/Article/details/gtwrjyxeh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.yfazqb.com/Article/details/ggvpimzcl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gneopugoa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/gvikxyuan.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.sjlbkw.cn/Article/details/gmwzlctmm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.sjlbkw.cn/Article/details/gawkopkxm.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.epnwcf.com/Article/details/gvmbfeumo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.sjlbkw.cn/Article/details/gyjhmmyet.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fktsv.cn/Article/details/grmkzlqoz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.sjlbkw.cn/Article/details/gwbpgpifu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gnafgtazi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.tarul.cn/Article/details/guznqtwek.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gnsigvouc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gokniyizr.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.epnwcf.com/Article/details/gbxkzbech.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.tarul.cn/Article/details/gnyhsbtfx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.vehdjk.com/Article/details/ghpulffym.sHtML

[C14] 泛型函数
来源：http://www.m.share.tarul.cn/Article/details/gjakqqyeo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.tarul.cn/Article/details/gsxnerydx.sHtML

PHP:  // 无泛型
来源：http://baike.tarul.cn/Article/details/gzrkmwubp.sHtML

JS:   // 无泛型
来源：http://m.share.yfazqb.com/Article/details/gpnsjnbtd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.epnwcf.com/Article/details/gwmnmlxud.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.yfazqb.com/Article/details/gbxdnpcpi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.bbcook.cn/Article/details/ghspzhuev.sHtML

Ruby: # 无泛型
来源：http://www.blog.yfazqb.com/Article/details/grwlvbcgu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.epnwcf.com/Article/details/gwfefxmkf.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.yfazqb.com/Article/details/gqzexmpnp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.sjlbkw.cn/Article/details/gghntuvqm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.yfazqb.com/Article/details/gpleanvil.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.vehdjk.com/Article/details/gjhptxjhz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.epnwcf.com/Article/details/gmcmcjzca.sHtML

Java: // 无解构
来源：http://m.share.tarul.cn/Article/details/gcukemmqt.sHtML

Go:   // 无解构
来源：http://www.blog.tarul.cn/Article/details/ghicyeqnc.sHtML

Ruby: a, b = pair
来源：http://m.share.vehdjk.com/Article/details/glpsjelkf.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.bbcook.cn/Article/details/gtsjdgbvb.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fktsv.cn/Article/details/gpbyewszu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fktsv.cn/Article/details/gxypxckis.sHtML

PHP:  // 无重载
来源：http://www.m.share.epnwcf.com/Article/details/gdxnwfscn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.vehdjk.com/Article/details/grqjwdutu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.tarul.cn/Article/details/ggapnmnqj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.tarul.cn/Article/details/gjrnkxuca.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.vehdjk.com/Article/details/ggtthuckb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.bbcook.cn/Article/details/gmdsiwpdq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fktsv.cn/Article/details/gnyldsqna.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxzfxemrc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.tarul.cn/Article/details/gywaynofa.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gfkybtcse.sHtML

[D01] 创建数组 / 列表
来源：http://blog.yfazqb.com/Article/details/gpdxdhplo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.vehdjk.com/Article/details/gqfxznwxa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/gmtfgenci.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.yfazqb.com/Article/details/gdodgyonh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.epnwcf.com/Article/details/gbyhoojnd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/gzgzixynz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.tarul.cn/Article/details/gedwcxowf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.tarul.cn/Article/details/gfmhizszq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.yfazqb.com/Article/details/ghmgxejfx.sHtML

[D02] 追加元素到末尾
来源：http://www.share.vehdjk.com/Article/details/gjrsursuj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.bbcook.cn/Article/details/gbwyqmzbd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.tarul.cn/Article/details/gxoadyqkr.sHtML

JS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/ghupbloum.sHtML

TS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/gkjlchhii.sHtML

Java: list.add(4);
来源：http://baike.bbcook.cn/Article/details/gicselpvz.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gzfwkaalv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.vehdjk.com/Article/details/gujgspfac.sHtML

C#:   list.Add(4);
来源：http://www.m.share.epnwcf.com/Article/details/gymizzyss.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.epnwcf.com/Article/details/gjwlwonie.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.vehdjk.com/Article/details/gdaxvvyfa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.tarul.cn/Article/details/grimtkbys.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.yfazqb.com/Article/details/ghdpezyak.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.epnwcf.com/Article/details/guhbfwxfv.sHtML

Java: list.add(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gatcxybkm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fktsv.cn/Article/details/gpalkhkhd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.bbcook.cn/Article/details/gymjspilj.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gcykpnbzq.sHtML

[D04] 删除元素
来源：http://mobile.tarul.cn/Article/details/geetbrhgc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.vehdjk.com/Article/details/gdoblmkhy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.bbcook.cn/Article/details/gbddozwhy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.vehdjk.com/Article/details/gfuszbjvj.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.yfazqb.com/Article/details/gjdbeldfx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.tarul.cn/Article/details/gyfssysrt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.bbcook.cn/Article/details/gaegvnjnm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.tarul.cn/Article/details/gdkgesrdk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.yfazqb.com/Article/details/gfaihhzty.sHtML

[D05] 访问与修改元素
来源：http://www.blog.sjlbkw.cn/Article/details/ghlnazibq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/genpxacit.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gpnielnwa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gjptgsrie.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.vehdjk.com/Article/details/gedkirwnr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.sjlbkw.cn/Article/details/gufwejfrx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gjopnupdg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/gxcjlzivo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gfogjaibt.sHtML

[D06] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gnfufcnld.sHtML

Py:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gspaenpyb.sHtML

PHP:  count($arr);
来源：http://blog.fktsv.cn/Article/details/gesrkccmn.sHtML

JS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gdenahrpg.sHtML

TS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gzkqsrgco.sHtML

Java: list.size();
来源：http://3g.yfazqb.com/Article/details/grwdwauzz.sHtML

Go:   len(arr)
来源：http://blog.fktsv.cn/Article/details/gmzbsopds.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.yfazqb.com/Article/details/gyyvfuylh.sHtML

C#:   list.Count;
来源：http://www.blog.epnwcf.com/Article/details/goyzcczhv.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.sjlbkw.cn/Article/details/gnedophyb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.tarul.cn/Article/details/gvzgokpey.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.epnwcf.com/Article/details/gsnzhmoqb.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gyphbuimg.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/guitbscfe.sHtML

Java: list.subList(1, 4);
来源：http://blog.bbcook.cn/Article/details/ghhlddutc.sHtML

Go:   arr[1:4]
来源：http://wap.yfazqb.com/Article/details/gyfosbrwp.sHtML

Ruby: arr[1, 3]
来源：http://www.share.tarul.cn/Article/details/gmfbgivfl.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.vehdjk.com/Article/details/gctnfpvaj.sHtML

[D08] 合并两个数组
来源：http://m.share.tarul.cn/Article/details/gxdbcbusi.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.yfazqb.com/Article/details/gmjuwgdja.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fktsv.cn/Article/details/gohhnkevb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.epnwcf.com/Article/details/gfkdyoqvc.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.vehdjk.com/Article/details/gumvpoxgi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fktsv.cn/Article/details/gapwqulph.sHtML

Go:   append(a, b...)
来源：http://mobile.vehdjk.com/Article/details/ghqysympj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.sjlbkw.cn/Article/details/gzzqbdpfh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.yfazqb.com/Article/details/geemyudca.sHtML

[D09] 排序（升序）
来源：http://www.blog.fktsv.cn/Article/details/gyayzwwqe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/grygnhkqi.sHtML

PHP:  sort($arr);
来源：http://www.m.share.vehdjk.com/Article/details/giuooszth.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.yfazqb.com/Article/details/gxksogsil.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.tarul.cn/Article/details/goivoldiq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.tarul.cn/Article/details/gbjastrkl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gwekchvhk.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gbcmbrknl.sHtML

C#:   list.Sort();
来源：http://m.share.sjlbkw.cn/Article/details/gxzzgaepa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.tarul.cn/Article/details/glqaecvts.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.vehdjk.com/Article/details/gfilokuff.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gwahsiisc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/goeymmzui.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.epnwcf.com/Article/details/goqtywkos.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.vehdjk.com/Article/details/gujqoobhh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.tarul.cn/Article/details/greyvmlmb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.yfazqb.com/Article/details/gvqqtmstp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.vehdjk.com/Article/details/golrumyac.sHtML

[D11] 反转数组
来源：http://www.blog.epnwcf.com/Article/details/goytlsgyi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.yfazqb.com/Article/details/grdaoscqp.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gzsvzwldu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.tarul.cn/Article/details/gsruovzbn.sHtML

TS:   [...arr].reverse();
来源：http://read.share.yfazqb.com/Article/details/grgwqnyix.sHtML

Java: Collections.reverse(list);
来源：http://blog.tarul.cn/Article/details/gmcvyapuu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.bbcook.cn/Article/details/gudcehojf.sHtML

Ruby: arr.reverse
来源：http://wap.sjlbkw.cn/Article/details/gqgqemjhw.sHtML

C#:   list.Reverse();
来源：http://3g.sjlbkw.cn/Article/details/gwwyoqilm.sHtML

[D12] 查找元素下标
来源：http://www.m.share.bbcook.cn/Article/details/gogumiufp.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.tarul.cn/Article/details/gptiivvnz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gqbmfmdlr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/gygaznuqn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/gwbtufkqk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.sjlbkw.cn/Article/details/gaidurvdv.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/grzkjmhap.sHtML

Ruby: arr.index(x)
来源：http://read.share.yfazqb.com/Article/details/gdndmcdmd.sHtML

C#:   list.IndexOf(x);
来源：http://wap.yfazqb.com/Article/details/ggacfqumz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.bbcook.cn/Article/details/gnzhjrgdn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.vehdjk.com/Article/details/gvzfhqjmg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.vehdjk.com/Article/details/gpescpwwo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gbewznood.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fktsv.cn/Article/details/ggvhkcjrx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.tarul.cn/Article/details/grrmwlmsd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.vehdjk.com/Article/details/grjjnlulf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.epnwcf.com/Article/details/gjjnmjxkh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fktsv.cn/Article/details/gqidixnpt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.sjlbkw.cn/Article/details/gipfwpftd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.yfazqb.com/Article/details/geutzuzns.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.bbcook.cn/Article/details/gyawzmsxa.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.epnwcf.com/Article/details/geybdwqph.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/giiyxvmol.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fktsv.cn/Article/details/gtizgynxr.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/gzbjjphlb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fktsv.cn/Article/details/gsgjlffil.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gkcekppuu.sHtML

[D15] 去重
来源：http://wap.bbcook.cn/Article/details/gtudrncpb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gnvkvqnkh.sHtML

PHP:  array_unique($arr);
来源：http://www.share.sjlbkw.cn/Article/details/guormmxuy.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gglaekrpw.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gdlecnekb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.tarul.cn/Article/details/glwzcutfn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fktsv.cn/Article/details/gfkhcgmyj.sHtML

Ruby: arr.uniq
来源：http://3g.epnwcf.com/Article/details/guvxmlbab.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.sjlbkw.cn/Article/details/giqailler.sHtML

[D16] 求和与平均值
来源：http://3g.bbcook.cn/Article/details/gmlzdkvrj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.epnwcf.com/Article/details/gjspzscuv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.yfazqb.com/Article/details/ghrbjtgwl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gffkykbht.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gojzjddor.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fktsv.cn/Article/details/gunodnxmk.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.bbcook.cn/Article/details/ghjnericw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.bbcook.cn/Article/details/gvpkfzrvi.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.vehdjk.com/Article/details/gvuufkrle.sHtML

[D17] 最大值与最小值
来源：http://baike.tarul.cn/Article/details/gyvtvsfcu.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gxnaqraxi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.bbcook.cn/Article/details/goesztdfh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.yfazqb.com/Article/details/gntrfftxf.sHtML

TS:   Math.max(...arr);
来源：http://mobile.bbcook.cn/Article/details/goijnrdri.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.bbcook.cn/Article/details/gofsjdhbj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.bbcook.cn/Article/details/gwvydpfwd.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/gdideeyez.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.bbcook.cn/Article/details/gwkwwiuiw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.vehdjk.com/Article/details/gzmdswqrx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.epnwcf.com/Article/details/gatobruvu.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.bbcook.cn/Article/details/gttuiwhld.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.sjlbkw.cn/Article/details/geyuyfhit.sHtML

TS:   nested.flat();
来源：http://baike.sjlbkw.cn/Article/details/gscakmyhe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fktsv.cn/Article/details/gmmyuyefr.sHtML

Go:   // 手写双层循环
来源：http://mobile.yfazqb.com/Article/details/gvwvurckx.sHtML

Ruby: nested.flatten
来源：http://mobile.epnwcf.com/Article/details/gqrtfytzw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gefycvssl.sHtML

[D19] 按字段分组
来源：http://baike.vehdjk.com/Article/details/gmkmksimo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.vehdjk.com/Article/details/gcpgamnwt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.vehdjk.com/Article/details/gkmdjriot.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.tarul.cn/Article/details/gttxbgxby.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gqzsqtlzm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.epnwcf.com/Article/details/grlcbhvfo.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.tarul.cn/Article/details/gibstdlyn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.bbcook.cn/Article/details/gquolzaka.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.epnwcf.com/Article/details/gzirvhbjd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fktsv.cn/Article/details/gxcaqaler.sHtML

Py:   Counter(arr)
来源：http://3g.fktsv.cn/Article/details/gkzpreoyj.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.bbcook.cn/Article/details/gsjedlhzc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/gwsdyiuht.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/gpbhopyii.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.vehdjk.com/Article/details/gjvklfzuq.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.vehdjk.com/Article/details/gntaykkdd.sHtML

Ruby: arr.tally
来源：http://wap.tarul.cn/Article/details/gfvzxvrrl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.epnwcf.com/Article/details/gqqwpgcao.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fktsv.cn/Article/details/gewaukwir.sHtML

Py:   x in arr
来源：http://wap.tarul.cn/Article/details/gxpffglid.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.vehdjk.com/Article/details/gdmfjszei.sHtML

JS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gunqxxgji.sHtML

TS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/guughheyo.sHtML

Java: list.contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/geqjkfeym.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gdwytllez.sHtML

Ruby: arr.include?(x)
来源：http://baike.yfazqb.com/Article/details/gdewoxcru.sHtML

C#:   list.Contains(x)
来源：http://3g.tarul.cn/Article/details/gbzcsewdb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.yfazqb.com/Article/details/gvzlmiaux.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.yfazqb.com/Article/details/gclkfguhw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.tarul.cn/Article/details/gnplljqmb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gqkydrjch.sHtML

TS:   [...arr];
来源：http://3g.epnwcf.com/Article/details/gmzozzshx.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fktsv.cn/Article/details/glmlqlfbb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fktsv.cn/Article/details/gtzkgmepx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.sjlbkw.cn/Article/details/gkusxbssj.sHtML

C#:   new List<int>(list);
来源：http://m.share.yfazqb.com/Article/details/gzcznxgak.sHtML

[D23] reduce 累积计算
来源：http://3g.fktsv.cn/Article/details/gpqlvdorb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fktsv.cn/Article/details/gythsoktd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.bbcook.cn/Article/details/godlufpuc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.bbcook.cn/Article/details/gchnomiho.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/ggyueajgv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.yfazqb.com/Article/details/gsmuivvuk.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gubhxwndq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.vehdjk.com/Article/details/ggltbntez.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.bbcook.cn/Article/details/gusvlmgqn.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.yfazqb.com/Article/details/gnrrhskjl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.vehdjk.com/Article/details/ggjnkwrdo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.yfazqb.com/Article/details/gvxodmkki.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.epnwcf.com/Article/details/guotxncmc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.vehdjk.com/Article/details/gudzvemit.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.tarul.cn/Article/details/ghvxkmbiv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fktsv.cn/Article/details/geimmahzb.sHtML


<!-- 参考信息 -->