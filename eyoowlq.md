代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqodqedun.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gmfnoehuc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.bbcook.cn/Article/details/gsumqlfyq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.sjlbkw.cn/Article/details/gliqbsvho.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.sjlbkw.cn/Article/details/gnnhlaapb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.yfazqb.com/Article/details/gikrnhcgp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gabdynpkl.sHtML

[C09] 递归
来源：http://mobile.sjlbkw.cn/Article/details/gfegckvnr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gautlberl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.yfazqb.com/Article/details/grpqvlmpi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.sjlbkw.cn/Article/details/golwnrhko.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/gzqzdemob.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/gohdjetnd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.sjlbkw.cn/Article/details/grayzqfsg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/ggiarurhh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.epnwcf.com/Article/details/gluqblcdl.sHtML

[C10] 变量作用域
来源：http://mobile.yfazqb.com/Article/details/gwdkgvkbh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.bbcook.cn/Article/details/ggbqzcuhh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.bbcook.cn/Article/details/gnxtmhubx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.tarul.cn/Article/details/gmyvgbptw.sHtML

TS:   同 JS
来源：http://www.blog.epnwcf.com/Article/details/ghlnzyaji.sHtML

Java: 方法内为块级作用域
来源：http://m.share.bbcook.cn/Article/details/gackqqyvs.sHtML

Go:   花括号块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gzgneypnh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.epnwcf.com/Article/details/gkxksvdxe.sHtML

C#:   块级作用域
来源：http://mobile.tarul.cn/Article/details/gnjkzebjs.sHtML

[C11] 模块导入与导出
来源：http://m.share.yfazqb.com/Article/details/gbkvrhltg.sHtML

Py:   from module import func
来源：http://mobile.sjlbkw.cn/Article/details/gksjkmzyb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fktsv.cn/Article/details/gojbmeuyi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.vehdjk.com/Article/details/gimegqdlk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.epnwcf.com/Article/details/gleidgrmt.sHtML

Java: import java.util.List;
来源：http://baike.fktsv.cn/Article/details/gfqcbioif.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.vehdjk.com/Article/details/ggjmnevyc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.bbcook.cn/Article/details/glqfgpahw.sHtML

C#:   using System.Text;
来源：http://www.m.share.vehdjk.com/Article/details/gbupcnlne.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/gandenfby.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.bbcook.cn/Article/details/gzhejbgzm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.vehdjk.com/Article/details/gkcoskzcc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.tarul.cn/Article/details/gtgzqmgwm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gnwlgvjtd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.yfazqb.com/Article/details/ghkrjmnai.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.tarul.cn/Article/details/gjgxgogof.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.yfazqb.com/Article/details/gpazvjovo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.epnwcf.com/Article/details/gojinnmps.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fktsv.cn/Article/details/ggoaaqwog.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.bbcook.cn/Article/details/gypoatfak.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gpwgiriqc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.epnwcf.com/Article/details/glxrlhrfd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gfkzcuevg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gcsxnstev.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fktsv.cn/Article/details/ggfjmmqzm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.tarul.cn/Article/details/ggqcnushw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.vehdjk.com/Article/details/grlpdgdek.sHtML

[C14] 泛型函数
来源：http://www.blog.yfazqb.com/Article/details/grvprlolq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.yfazqb.com/Article/details/gwqzjngja.sHtML

PHP:  // 无泛型
来源：http://mobile.epnwcf.com/Article/details/gziqdzefe.sHtML

JS:   // 无泛型
来源：http://www.share.vehdjk.com/Article/details/giqnbfgfg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fktsv.cn/Article/details/gdibzgxuu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.bbcook.cn/Article/details/ghgsvqwuf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.tarul.cn/Article/details/ghhnuskue.sHtML

Ruby: # 无泛型
来源：http://baike.vehdjk.com/Article/details/gltbmdoqn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.tarul.cn/Article/details/gfuhjjmpa.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.sjlbkw.cn/Article/details/galuzahlf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.yfazqb.com/Article/details/gdcasrevf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fktsv.cn/Article/details/gkuvjyocn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gjtuflxak.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fktsv.cn/Article/details/gyvfvzsix.sHtML

Java: // 无解构
来源：http://www.blog.fktsv.cn/Article/details/gztejevki.sHtML

Go:   // 无解构
来源：http://3g.bbcook.cn/Article/details/gwtmoiinp.sHtML

Ruby: a, b = pair
来源：http://blog.sjlbkw.cn/Article/details/gzwnrjdpj.sHtML

C#:   var (a, b) = pair;
来源：http://baike.bbcook.cn/Article/details/gxgybmyda.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.bbcook.cn/Article/details/gvfhytmsy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fktsv.cn/Article/details/gwufukrhu.sHtML

PHP:  // 无重载
来源：http://wap.tarul.cn/Article/details/gzawtmfgm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.bbcook.cn/Article/details/gsemvatat.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.epnwcf.com/Article/details/ghjkllhvn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.sjlbkw.cn/Article/details/gxbnzrwos.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.sjlbkw.cn/Article/details/gqpqgdwev.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.yfazqb.com/Article/details/gupkdvnow.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.vehdjk.com/Article/details/gzeiyqlav.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ghihvzcxg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.sjlbkw.cn/Article/details/gbciojvzv.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gfbaxtspr.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/gzqousgyt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.epnwcf.com/Article/details/gcbewpdrb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.bbcook.cn/Article/details/gkdxnbptw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.epnwcf.com/Article/details/gsyjzvwmn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.sjlbkw.cn/Article/details/gpzxevbta.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.yfazqb.com/Article/details/gpzzchwtq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fktsv.cn/Article/details/gujasygwk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fktsv.cn/Article/details/gmpfyywlh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fktsv.cn/Article/details/gyvoqlwqu.sHtML

[D02] 追加元素到末尾
来源：http://read.share.bbcook.cn/Article/details/ghgpddhtw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.sjlbkw.cn/Article/details/gfvezblie.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.epnwcf.com/Article/details/gnujykhuf.sHtML

JS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gryqheuyn.sHtML

TS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gdjqddqsi.sHtML

Java: list.add(4);
来源：http://www.share.epnwcf.com/Article/details/gwgqvhbmd.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.yfazqb.com/Article/details/gihnstaba.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.tarul.cn/Article/details/giwdsaehv.sHtML

C#:   list.Add(4);
来源：http://3g.epnwcf.com/Article/details/gcyelrerd.sHtML

[D03] 在指定位置插入元素
来源：http://3g.sjlbkw.cn/Article/details/ggdyrbqjh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.epnwcf.com/Article/details/gcvzgvugl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.vehdjk.com/Article/details/grkyvmtsf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/gbdxgdqyd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.vehdjk.com/Article/details/gutzikdij.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gcyqqpgcr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.epnwcf.com/Article/details/gzvlmhnnt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.vehdjk.com/Article/details/guguzlmlg.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.tarul.cn/Article/details/gmwkyhdji.sHtML

[D04] 删除元素
来源：http://www.m.share.vehdjk.com/Article/details/ghrvjlcxr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.yfazqb.com/Article/details/gimsbmorj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.tarul.cn/Article/details/gugoidsri.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.epnwcf.com/Article/details/ggkpfeclm.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.bbcook.cn/Article/details/gljifwopj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.bbcook.cn/Article/details/gihevnran.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.bbcook.cn/Article/details/gsniokbno.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.tarul.cn/Article/details/gilxkkqgl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.epnwcf.com/Article/details/gxsgocezq.sHtML

[D05] 访问与修改元素
来源：http://blog.epnwcf.com/Article/details/guafeqell.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gkvbzuxwj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/grmdxojcv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.epnwcf.com/Article/details/gotaxistw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.tarul.cn/Article/details/gogantcfc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.epnwcf.com/Article/details/gryfiwtyi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gzkstqdiy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gqlsipckw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gdxssortl.sHtML

[D06] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gqewvgsfm.sHtML

Py:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/guljbjhza.sHtML

PHP:  count($arr);
来源：http://blog.epnwcf.com/Article/details/gjpngodya.sHtML

JS:   arr.length
来源：http://blog.fktsv.cn/Article/details/gpzrcmzot.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gjlmrxhci.sHtML

Java: list.size();
来源：http://read.share.vehdjk.com/Article/details/gewuugfoc.sHtML

Go:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/gbqrhlmcg.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.epnwcf.com/Article/details/gyclhtrjc.sHtML

C#:   list.Count;
来源：http://www.blog.tarul.cn/Article/details/gyoadmmku.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gfixmxjaf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.yfazqb.com/Article/details/gklhgdxmp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.vehdjk.com/Article/details/gujcrwxxh.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/gwdhuxbui.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gkooadppt.sHtML

Java: list.subList(1, 4);
来源：http://wap.yfazqb.com/Article/details/gqkavipwr.sHtML

Go:   arr[1:4]
来源：http://m.share.vehdjk.com/Article/details/gjzvaahnq.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.yfazqb.com/Article/details/gqukuuhvy.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.vehdjk.com/Article/details/gzgkglxvh.sHtML

[D08] 合并两个数组
来源：http://www.m.share.yfazqb.com/Article/details/gdhfsbbsl.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.sjlbkw.cn/Article/details/gkeogruza.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.bbcook.cn/Article/details/ggwbkpkcn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.tarul.cn/Article/details/gbpdyyhhz.sHtML

TS:   [...a, ...b];
来源：http://www.share.vehdjk.com/Article/details/giczrflen.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.yfazqb.com/Article/details/gsafbtcrb.sHtML

Go:   append(a, b...)
来源：http://m.share.yfazqb.com/Article/details/gntlxbvqb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.epnwcf.com/Article/details/grmmymckl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gozxvbrzh.sHtML

[D09] 排序（升序）
来源：http://baike.epnwcf.com/Article/details/gutumwfuc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gsngouhyy.sHtML

PHP:  sort($arr);
来源：http://baike.sjlbkw.cn/Article/details/ggkigwgtm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.bbcook.cn/Article/details/gxjycfjsa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiqfgbix.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.tarul.cn/Article/details/grxavrpdo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/gaucbcyxy.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gcgdpjjbm.sHtML

C#:   list.Sort();
来源：http://blog.bbcook.cn/Article/details/ghztlhjyp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.epnwcf.com/Article/details/gowfegzeh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.epnwcf.com/Article/details/gktxvkndw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fktsv.cn/Article/details/gprtqwugy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gqwsaqmwd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/ggzxwugux.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.yfazqb.com/Article/details/gqjeobgvy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.tarul.cn/Article/details/gjseijlvi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.epnwcf.com/Article/details/gpermbipp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.yfazqb.com/Article/details/gbyvitqao.sHtML

[D11] 反转数组
来源：http://blog.epnwcf.com/Article/details/gzcvmwodg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.vehdjk.com/Article/details/gkruzpbpa.sHtML

PHP:  array_reverse($arr);
来源：http://3g.bbcook.cn/Article/details/gejavomtc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.tarul.cn/Article/details/gsykunsuv.sHtML

TS:   [...arr].reverse();
来源：http://3g.vehdjk.com/Article/details/glrhtvjqd.sHtML

Java: Collections.reverse(list);
来源：http://baike.yfazqb.com/Article/details/gkhahzfol.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.epnwcf.com/Article/details/gxfkdgqzu.sHtML

Ruby: arr.reverse
来源：http://m.share.bbcook.cn/Article/details/gohhhdrla.sHtML

C#:   list.Reverse();
来源：http://m.share.yfazqb.com/Article/details/gsegvltxv.sHtML

[D12] 查找元素下标
来源：http://www.blog.tarul.cn/Article/details/gdnjvfgar.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fktsv.cn/Article/details/gbmglyzpb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.bbcook.cn/Article/details/gghacnywf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/ghfwveyfr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/grlzoxwxv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.vehdjk.com/Article/details/gzblyzdqb.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/ghzpjxtyd.sHtML

Ruby: arr.index(x)
来源：http://www.share.yfazqb.com/Article/details/gamnyfhuf.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.vehdjk.com/Article/details/gdedvtprj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.epnwcf.com/Article/details/gslzbxndk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.sjlbkw.cn/Article/details/gjfvlhhdq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.bbcook.cn/Article/details/gntdnwzzj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gspcvuubd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/ghqzveact.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.bbcook.cn/Article/details/gvzklflzg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.sjlbkw.cn/Article/details/gfvagedjt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.tarul.cn/Article/details/golmwgkri.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gektqbfbr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.sjlbkw.cn/Article/details/gzmlkugwt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.bbcook.cn/Article/details/gsllbtsrb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gpptflsrf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/ggriajkau.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gcssxbzfs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.sjlbkw.cn/Article/details/gmijdzelq.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/gloobpwzu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.tarul.cn/Article/details/glmitpdvg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.bbcook.cn/Article/details/gsmlfyoep.sHtML

[D15] 去重
来源：http://mobile.tarul.cn/Article/details/gyrfsvaeq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.sjlbkw.cn/Article/details/gxkumuuzf.sHtML

PHP:  array_unique($arr);
来源：http://read.share.yfazqb.com/Article/details/geicljbze.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/glhjjbzbf.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gkkiovrbi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.epnwcf.com/Article/details/gadsggext.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.vehdjk.com/Article/details/gvanxuiwn.sHtML

Ruby: arr.uniq
来源：http://blog.vehdjk.com/Article/details/ghlqfsynu.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.epnwcf.com/Article/details/grerrqyrp.sHtML

[D16] 求和与平均值
来源：http://wap.bbcook.cn/Article/details/gwzpssdpv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.bbcook.cn/Article/details/gbpcppbvd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fktsv.cn/Article/details/gmkndketb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gojudvnbz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.tarul.cn/Article/details/gutmmrdzk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.tarul.cn/Article/details/gbejfhemi.sHtML

Go:   // 手写循环累加
来源：http://baike.vehdjk.com/Article/details/gtjxivyib.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.vehdjk.com/Article/details/gquekabhl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.bbcook.cn/Article/details/gwhzcuecq.sHtML

[D17] 最大值与最小值
来源：http://3g.epnwcf.com/Article/details/gxwscyebx.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fktsv.cn/Article/details/gmcsxreyb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.bbcook.cn/Article/details/gwpbrmtat.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fktsv.cn/Article/details/gjxpuaqxw.sHtML

TS:   Math.max(...arr);
来源：http://mobile.sjlbkw.cn/Article/details/gjfroovvg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.sjlbkw.cn/Article/details/gaebgkxie.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fktsv.cn/Article/details/gebupnguc.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.vehdjk.com/Article/details/gkmwwosvt.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.tarul.cn/Article/details/gbczancqp.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.yfazqb.com/Article/details/gbwmubxvw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fktsv.cn/Article/details/gromoszyr.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.epnwcf.com/Article/details/gaimfvlrg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.tarul.cn/Article/details/gxtojksgn.sHtML

TS:   nested.flat();
来源：http://3g.epnwcf.com/Article/details/gsvhxvseh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gyoavygob.sHtML

Go:   // 手写双层循环
来源：http://m.share.fktsv.cn/Article/details/gchqucluq.sHtML

Ruby: nested.flatten
来源：http://blog.epnwcf.com/Article/details/gxozgfwud.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gctnmigvk.sHtML

[D19] 按字段分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gesgwqzsq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.vehdjk.com/Article/details/gxcmwufvn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.tarul.cn/Article/details/grpxomtnz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.sjlbkw.cn/Article/details/grdetiumo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/gzjmodeea.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.tarul.cn/Article/details/gikuajsdq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.vehdjk.com/Article/details/gqwtijudm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.vehdjk.com/Article/details/gkboritzq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.tarul.cn/Article/details/gzpoclodq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.yfazqb.com/Article/details/goqyutvrm.sHtML

Py:   Counter(arr)
来源：http://wap.vehdjk.com/Article/details/gprsuqqmo.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.epnwcf.com/Article/details/gcieznihx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/gtsyezfgm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gkvafhbcp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvpdnuhw.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.yfazqb.com/Article/details/gppnhfdzc.sHtML

Ruby: arr.tally
来源：http://www.share.fktsv.cn/Article/details/gxerncmhq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.bbcook.cn/Article/details/givsvmpyz.sHtML

[D21] 判断是否包含某元素
来源：http://wap.yfazqb.com/Article/details/gkeiyqmwl.sHtML

Py:   x in arr
来源：http://baike.vehdjk.com/Article/details/gudndyqjh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.sjlbkw.cn/Article/details/geahzvehe.sHtML

JS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gvvejjyrx.sHtML

TS:   arr.includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gtjigcisv.sHtML

Java: list.contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gflgnymoh.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.tarul.cn/Article/details/gjuoyyeej.sHtML

Ruby: arr.include?(x)
来源：http://3g.tarul.cn/Article/details/gajzylbkm.sHtML

C#:   list.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/gzmjnqqzt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.bbcook.cn/Article/details/govbnhzjf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.epnwcf.com/Article/details/gytulbpow.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fktsv.cn/Article/details/gmlbfxywz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fktsv.cn/Article/details/grujavkwi.sHtML

TS:   [...arr];
来源：http://www.blog.epnwcf.com/Article/details/gcovqfnva.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/gpuuvseyt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.tarul.cn/Article/details/gfwhqyfoj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.yfazqb.com/Article/details/gglzawygh.sHtML

C#:   new List<int>(list);
来源：http://www.share.bbcook.cn/Article/details/guizstfwh.sHtML

[D23] reduce 累积计算
来源：http://3g.vehdjk.com/Article/details/ghbqkxbvv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.vehdjk.com/Article/details/gpxjgzymy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.epnwcf.com/Article/details/gpshjtcsf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/gpkkyhuno.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/govwfiaag.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.yfazqb.com/Article/details/gbihtfrpu.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/gvuedrpeh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.sjlbkw.cn/Article/details/gegtzieaj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fktsv.cn/Article/details/gdkzwujwn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.tarul.cn/Article/details/ghzydrlcn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gutrjfhlg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.bbcook.cn/Article/details/gikucbafg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fktsv.cn/Article/details/gbsqunofu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/ggakcqrue.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.vehdjk.com/Article/details/gansplxut.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fktsv.cn/Article/details/gonefrdif.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.bbcook.cn/Article/details/gzgfzulvg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.vehdjk.com/Article/details/ghzllrhlb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.epnwcf.com/Article/details/gjkdcjbmc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.bbcook.cn/Article/details/gajknlfke.sHtML


<!-- 参考信息 -->