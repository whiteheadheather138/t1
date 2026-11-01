代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gmxgjyleg.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.bbcook.cn/Article/details/gdrttylud.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.tarul.cn/Article/details/gfkjphpxc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/gsjsiejgj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.bbcook.cn/Article/details/guzcrmrvd.sHtML

TS:   arr.map(String)
来源：http://m.share.tarul.cn/Article/details/ggdebgqnv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.bbcook.cn/Article/details/gccnftliw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.epnwcf.com/Article/details/gygxyrxov.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.epnwcf.com/Article/details/gmkluuqud.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/grpfqtzgi.sHtML

[C08] 闭包
来源：http://m.share.yfazqb.com/Article/details/glvtlbcnu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.vehdjk.com/Article/details/gbsdmjaqz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.sjlbkw.cn/Article/details/gukcsizbp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gzuupscui.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/ghlrhjxcr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.tarul.cn/Article/details/gebxmrxng.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.tarul.cn/Article/details/gemufdtub.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.tarul.cn/Article/details/gcajjmmuj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gfsrekayw.sHtML

[C09] 递归
来源：http://wap.sjlbkw.cn/Article/details/gtztzvpkn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.epnwcf.com/Article/details/gggyvdrlz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.vehdjk.com/Article/details/ghjmipbqy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/gqioylkoo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/ggmfommal.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gmjjxwmam.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.bbcook.cn/Article/details/guqjhhvvf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.vehdjk.com/Article/details/gjwpcpoja.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.yfazqb.com/Article/details/gnwqbvggp.sHtML

[C10] 变量作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxxzxorf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.epnwcf.com/Article/details/gmnsylxsa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.yfazqb.com/Article/details/gdydqhrbt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fktsv.cn/Article/details/ghczxtnjo.sHtML

TS:   同 JS
来源：http://mobile.vehdjk.com/Article/details/gwwtyqnrc.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.vehdjk.com/Article/details/grmlmcogz.sHtML

Go:   花括号块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/ganhsjlch.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.yfazqb.com/Article/details/gdjoowxys.sHtML

C#:   块级作用域
来源：http://read.share.tarul.cn/Article/details/gwzhfcruz.sHtML

[C11] 模块导入与导出
来源：http://baike.bbcook.cn/Article/details/genqottmv.sHtML

Py:   from module import func
来源：http://blog.tarul.cn/Article/details/gccwmturr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.vehdjk.com/Article/details/gxscvcuaz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.sjlbkw.cn/Article/details/grzcbmobh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrauaimv.sHtML

Java: import java.util.List;
来源：http://www.share.bbcook.cn/Article/details/gutcwkseg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhivyier.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.vehdjk.com/Article/details/ghdpohjcc.sHtML

C#:   using System.Text;
来源：http://baike.epnwcf.com/Article/details/gosahqtpo.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.sjlbkw.cn/Article/details/gdlokkcpp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.tarul.cn/Article/details/gnijaticf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.epnwcf.com/Article/details/gkulwnizy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/gzuhlblxj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/gzktofaqb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.yfazqb.com/Article/details/glwvjumjp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fktsv.cn/Article/details/gmjvrpiwr.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.yfazqb.com/Article/details/gruhfarrb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gruutmpya.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.sjlbkw.cn/Article/details/ghivxnkdy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.epnwcf.com/Article/details/gqpsjpivv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gvsfdgbfk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.bbcook.cn/Article/details/gssjoinkc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gsonkggdj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gammwapem.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.sjlbkw.cn/Article/details/gtdtlqnug.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.yfazqb.com/Article/details/gdewupprv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.epnwcf.com/Article/details/gadfbljvr.sHtML

[C14] 泛型函数
来源：http://www.m.share.epnwcf.com/Article/details/gggggxjqh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.sjlbkw.cn/Article/details/gfubebnha.sHtML

PHP:  // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gelxrwtrk.sHtML

JS:   // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gvvrqqjjk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.vehdjk.com/Article/details/gvwhxzttq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.yfazqb.com/Article/details/ggcbacave.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.yfazqb.com/Article/details/gbjtwgiww.sHtML

Ruby: # 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/ghkdoodqx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.epnwcf.com/Article/details/gucmfrlbw.sHtML

[C15] 解构 / 展开参数
来源：http://blog.yfazqb.com/Article/details/gqziasuuc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.vehdjk.com/Article/details/gvygfxqxj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.tarul.cn/Article/details/gukhiithb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fktsv.cn/Article/details/ganshrmfr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.epnwcf.com/Article/details/gskirxuei.sHtML

Java: // 无解构
来源：http://mobile.fktsv.cn/Article/details/gqkqnngcv.sHtML

Go:   // 无解构
来源：http://wap.vehdjk.com/Article/details/gilnajlln.sHtML

Ruby: a, b = pair
来源：http://mobile.yfazqb.com/Article/details/gezqplwzn.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.epnwcf.com/Article/details/gurplcpzg.sHtML

[C16] 函数 / 方法重载
来源：http://baike.epnwcf.com/Article/details/gfsqaxmjq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.bbcook.cn/Article/details/gsfqhrmzw.sHtML

PHP:  // 无重载
来源：http://www.share.tarul.cn/Article/details/gjxysrvwv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.tarul.cn/Article/details/gyobdqnzz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.yfazqb.com/Article/details/gmdbrqrxf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.tarul.cn/Article/details/gamcfakgw.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.sjlbkw.cn/Article/details/gbiofpaha.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.vehdjk.com/Article/details/gbcddcqfw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtasthvd.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gfuqjvyxc.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.epnwcf.com/Article/details/gzqyzlsnx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtjbcdfjn.sHtML

[D01] 创建数组 / 列表
来源：http://baike.yfazqb.com/Article/details/glscqfvaj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.tarul.cn/Article/details/gdihfqgjr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.bbcook.cn/Article/details/gwpnezfdw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.epnwcf.com/Article/details/gfzdkacrw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.epnwcf.com/Article/details/ghxbszskr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.yfazqb.com/Article/details/ghyoynmce.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fktsv.cn/Article/details/guwqrpyje.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fktsv.cn/Article/details/gvshzjwwf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fktsv.cn/Article/details/gnkcxsevt.sHtML

[D02] 追加元素到末尾
来源：http://read.share.epnwcf.com/Article/details/grkazbuqn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.yfazqb.com/Article/details/gfskcxbag.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.bbcook.cn/Article/details/gqdsdwcif.sHtML

JS:   arr.push(4);
来源：http://baike.tarul.cn/Article/details/gofpjhspx.sHtML

TS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/ggehhaowd.sHtML

Java: list.add(4);
来源：http://m.share.tarul.cn/Article/details/gdsfjppfp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.tarul.cn/Article/details/gjoyqfpwg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.epnwcf.com/Article/details/ghmlryuah.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fktsv.cn/Article/details/gbpzxnhoj.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fktsv.cn/Article/details/gvbwvyytg.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.epnwcf.com/Article/details/gohjzaxjy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.bbcook.cn/Article/details/gcqtojprf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.yfazqb.com/Article/details/gyizbowwr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.sjlbkw.cn/Article/details/ggbguxbta.sHtML

Java: list.add(0, 0);
来源：http://wap.bbcook.cn/Article/details/gotkmkpha.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fktsv.cn/Article/details/gsnjcjqkm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.tarul.cn/Article/details/gkphusmek.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.tarul.cn/Article/details/gmnzzzcaa.sHtML

[D04] 删除元素
来源：http://baike.sjlbkw.cn/Article/details/glzmzgfgs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.bbcook.cn/Article/details/gjbpiomnk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.epnwcf.com/Article/details/geusbpknw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.sjlbkw.cn/Article/details/gixgoabvh.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.tarul.cn/Article/details/ghnkhxitl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.tarul.cn/Article/details/gudzryhnn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.yfazqb.com/Article/details/gqsftyfie.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.sjlbkw.cn/Article/details/gdelibneh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fktsv.cn/Article/details/gjbyrvhxo.sHtML

[D05] 访问与修改元素
来源：http://baike.tarul.cn/Article/details/ghekxuycn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gktqwgvcj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gsvozlhsn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/guysgbomd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.yfazqb.com/Article/details/gcuxlhlgl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.vehdjk.com/Article/details/gwvlmqiwm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/gtutpyodl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/ghwwmbbqb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/ghenlpvrn.sHtML

[D06] 数组长度
来源：http://mobile.vehdjk.com/Article/details/gzzfuquhh.sHtML

Py:   len(arr)
来源：http://baike.yfazqb.com/Article/details/gzdtruvba.sHtML

PHP:  count($arr);
来源：http://3g.vehdjk.com/Article/details/gceklgzsx.sHtML

JS:   arr.length
来源：http://www.share.yfazqb.com/Article/details/gepkxsjsm.sHtML

TS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/gmsgugfen.sHtML

Java: list.size();
来源：http://blog.fktsv.cn/Article/details/gssgecdjp.sHtML

Go:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/gjlfwzxkk.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.vehdjk.com/Article/details/gniynvlgo.sHtML

C#:   list.Count;
来源：http://3g.epnwcf.com/Article/details/gkvxmadom.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.epnwcf.com/Article/details/ganhmckrl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.epnwcf.com/Article/details/gyqquphtf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/ggzzlrdga.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gqctutcfp.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/ggkdakjdc.sHtML

Java: list.subList(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gfeurbmnv.sHtML

Go:   arr[1:4]
来源：http://3g.vehdjk.com/Article/details/gjhiigxag.sHtML

Ruby: arr[1, 3]
来源：http://baike.fktsv.cn/Article/details/guabgzkqw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.epnwcf.com/Article/details/gfxpzjeuu.sHtML

[D08] 合并两个数组
来源：http://m.share.vehdjk.com/Article/details/glqmlxfhf.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.sjlbkw.cn/Article/details/gxzoxaxdu.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fktsv.cn/Article/details/gfjtbzabm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.epnwcf.com/Article/details/gdxiwqica.sHtML

TS:   [...a, ...b];
来源：http://blog.vehdjk.com/Article/details/gewcjygtn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.tarul.cn/Article/details/gsbdirsdj.sHtML

Go:   append(a, b...)
来源：http://wap.epnwcf.com/Article/details/gdxptuzaf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fktsv.cn/Article/details/gyxwhfffb.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.yfazqb.com/Article/details/gicwtcqbz.sHtML

[D09] 排序（升序）
来源：http://www.m.share.vehdjk.com/Article/details/gyveubacc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gxopfqnwp.sHtML

PHP:  sort($arr);
来源：http://www.blog.vehdjk.com/Article/details/gyvnmpxow.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.yfazqb.com/Article/details/gjcczfvqi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.tarul.cn/Article/details/gkokmyybg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.epnwcf.com/Article/details/gxjlmeuwx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/gwqildhyc.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gzkujncek.sHtML

C#:   list.Sort();
来源：http://www.blog.tarul.cn/Article/details/gdnhvkznj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fktsv.cn/Article/details/grfxfabak.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fktsv.cn/Article/details/gefyqxluo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.vehdjk.com/Article/details/gzjlzghqv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/ggsvwlclu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/gekmikmbh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fktsv.cn/Article/details/gszjtlfuu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.tarul.cn/Article/details/gfytpigln.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.epnwcf.com/Article/details/gjbadudtw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.bbcook.cn/Article/details/gqtgkhqda.sHtML

[D11] 反转数组
来源：http://baike.tarul.cn/Article/details/gqysxxvha.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fktsv.cn/Article/details/gletuwdlq.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.yfazqb.com/Article/details/givvcufww.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtkcjwdi.sHtML

TS:   [...arr].reverse();
来源：http://wap.epnwcf.com/Article/details/gwrgrntzy.sHtML

Java: Collections.reverse(list);
来源：http://read.share.vehdjk.com/Article/details/gxmuvocem.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.vehdjk.com/Article/details/glnsaskcp.sHtML

Ruby: arr.reverse
来源：http://baike.bbcook.cn/Article/details/gaxcvllmc.sHtML

C#:   list.Reverse();
来源：http://mobile.fktsv.cn/Article/details/gjyieocrd.sHtML

[D12] 查找元素下标
来源：http://blog.yfazqb.com/Article/details/gdjfyjkov.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.vehdjk.com/Article/details/gxpfbdxvm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.tarul.cn/Article/details/gtukjzilc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gslaumdbl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.epnwcf.com/Article/details/gnkigcilx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.tarul.cn/Article/details/gwdqswrme.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fktsv.cn/Article/details/ggolgvnrl.sHtML

Ruby: arr.index(x)
来源：http://read.share.tarul.cn/Article/details/gknzmkuwe.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.yfazqb.com/Article/details/gylwixgpt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.vehdjk.com/Article/details/gmjxeopll.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.vehdjk.com/Article/details/gzkiafmuc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.epnwcf.com/Article/details/gfyqevwxk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/geumtkmjy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/gxjramrid.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.tarul.cn/Article/details/gedutconh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.vehdjk.com/Article/details/gkuzjyfqd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.yfazqb.com/Article/details/gihqdxgsd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.vehdjk.com/Article/details/glcfihzmc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.yfazqb.com/Article/details/gueinpkdh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.tarul.cn/Article/details/gjxgdwxni.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gpcbyjeyp.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/gsmytlabl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gntwfmyuk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.sjlbkw.cn/Article/details/gqlagrtqd.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gdgnnnzyc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fktsv.cn/Article/details/gvjkgolkw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.vehdjk.com/Article/details/gqcfqkqsd.sHtML

[D15] 去重
来源：http://baike.tarul.cn/Article/details/gmpalocru.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gwlpcofyn.sHtML

PHP:  array_unique($arr);
来源：http://www.share.tarul.cn/Article/details/gemluuhgd.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gaylyqmxe.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gfvmyekpc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.yfazqb.com/Article/details/gehredhnc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fktsv.cn/Article/details/gwxoztdxj.sHtML

Ruby: arr.uniq
来源：http://mobile.sjlbkw.cn/Article/details/gkpxmbcts.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.epnwcf.com/Article/details/glzlfctfq.sHtML

[D16] 求和与平均值
来源：http://www.blog.epnwcf.com/Article/details/gdplxfzxg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gmypjjtuz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gqyyqhhod.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/gjeaaptbb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.epnwcf.com/Article/details/gkvmholdb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.vehdjk.com/Article/details/grjnmulao.sHtML

Go:   // 手写循环累加
来源：http://mobile.fktsv.cn/Article/details/gclcipoif.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fktsv.cn/Article/details/gkwitrwfw.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fktsv.cn/Article/details/gpfugghzo.sHtML

[D17] 最大值与最小值
来源：http://3g.yfazqb.com/Article/details/gbkbvfhak.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.sjlbkw.cn/Article/details/gvophdcko.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.sjlbkw.cn/Article/details/geivwemdb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.bbcook.cn/Article/details/gkkgfvcku.sHtML

TS:   Math.max(...arr);
来源：http://3g.epnwcf.com/Article/details/gujacfugb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.bbcook.cn/Article/details/gwgzkxaav.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.tarul.cn/Article/details/ghptvfndj.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.epnwcf.com/Article/details/gtdhbdstn.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.epnwcf.com/Article/details/gyvmrauni.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/gxfkixdel.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.yfazqb.com/Article/details/gcarlqeww.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.epnwcf.com/Article/details/gzlliwpjo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.sjlbkw.cn/Article/details/guvlmifnm.sHtML

TS:   nested.flat();
来源：http://m.share.epnwcf.com/Article/details/gjhidvhqw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gfulrvzmx.sHtML

Go:   // 手写双层循环
来源：http://m.share.vehdjk.com/Article/details/ghiyeivsb.sHtML

Ruby: nested.flatten
来源：http://www.share.sjlbkw.cn/Article/details/gjoniilrd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.tarul.cn/Article/details/gzwcexyks.sHtML

[D19] 按字段分组
来源：http://baike.vehdjk.com/Article/details/gzgffhsek.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fktsv.cn/Article/details/giiyyvela.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.yfazqb.com/Article/details/gtircfozf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.bbcook.cn/Article/details/geeujfxee.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/gvxpxljfv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fktsv.cn/Article/details/gkfwxjsgm.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.epnwcf.com/Article/details/glrlonwmj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.sjlbkw.cn/Article/details/gypskjjdu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fktsv.cn/Article/details/grguupcwq.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.bbcook.cn/Article/details/gwsedehrh.sHtML

Py:   Counter(arr)
来源：http://read.share.tarul.cn/Article/details/gxmmkneet.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gzumrycsy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.bbcook.cn/Article/details/gfmypbtlo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.bbcook.cn/Article/details/gtsluunsy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.sjlbkw.cn/Article/details/gjrktblax.sHtML

Go:   // 手写 map[T]int
来源：http://3g.tarul.cn/Article/details/gfubmxrmj.sHtML

Ruby: arr.tally
来源：http://www.blog.bbcook.cn/Article/details/gutyqjist.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.vehdjk.com/Article/details/guicpscuu.sHtML

[D21] 判断是否包含某元素
来源：http://baike.vehdjk.com/Article/details/gxrwfazly.sHtML

Py:   x in arr
来源：http://www.m.share.vehdjk.com/Article/details/gxnohbnsi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.sjlbkw.cn/Article/details/gdtttudsd.sHtML

JS:   arr.includes(x)
来源：http://read.share.fktsv.cn/Article/details/glnhfihha.sHtML

TS:   arr.includes(x)
来源：http://m.share.bbcook.cn/Article/details/gsrjijnzy.sHtML

Java: list.contains(x)
来源：http://baike.sjlbkw.cn/Article/details/giurpbgky.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fktsv.cn/Article/details/glqsmzavn.sHtML

Ruby: arr.include?(x)
来源：http://wap.fktsv.cn/Article/details/gxagpzvhb.sHtML

C#:   list.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/gpnsjfsac.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.vehdjk.com/Article/details/geueuvyai.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fktsv.cn/Article/details/gnbiwsfzw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fktsv.cn/Article/details/glbnyzwiz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.bbcook.cn/Article/details/ghsljyois.sHtML

TS:   [...arr];
来源：http://3g.yfazqb.com/Article/details/gpzyreeep.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fktsv.cn/Article/details/ghvlppdpu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.yfazqb.com/Article/details/gxonzclns.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.tarul.cn/Article/details/gfllsswoe.sHtML

C#:   new List<int>(list);
来源：http://m.share.bbcook.cn/Article/details/gsrkpgrqb.sHtML

[D23] reduce 累积计算
来源：http://www.blog.tarul.cn/Article/details/ghzyqsjrt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gcnokoqwa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.epnwcf.com/Article/details/gokrwgxtm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.bbcook.cn/Article/details/giqehyzih.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fktsv.cn/Article/details/grrlfawmm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.bbcook.cn/Article/details/gyfgknwcz.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gjtsgiyzo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.yfazqb.com/Article/details/gcejadchd.sHtML


<!-- 参考信息 -->