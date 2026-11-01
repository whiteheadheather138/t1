代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://mobile.vehdjk.com/Article/details/gzbirrrrj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.epnwcf.com/Article/details/gdgmlduqj.sHtML

[C08] 闭包
来源：http://3g.bbcook.cn/Article/details/gbgqaremu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcwkwmrl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.sjlbkw.cn/Article/details/grzbrwpyf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/guzenguzb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gdfgtrucn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.tarul.cn/Article/details/goaaranzx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.yfazqb.com/Article/details/gzzbukmgp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gotjcegcj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gwauvqizk.sHtML

[C09] 递归
来源：http://baike.yfazqb.com/Article/details/gvwdfktjn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.tarul.cn/Article/details/grzzrvxqh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.epnwcf.com/Article/details/gmirfspiz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.sjlbkw.cn/Article/details/gfstzbskm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/gcrlzrrus.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.bbcook.cn/Article/details/gnvtpvibn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.tarul.cn/Article/details/grynmvwqg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/gdazrljyz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.epnwcf.com/Article/details/gjdalgloo.sHtML

[C10] 变量作用域
来源：http://read.share.fktsv.cn/Article/details/gcsdtgkmr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.vehdjk.com/Article/details/gzayngdgg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.yfazqb.com/Article/details/gvdedfjmb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gpimqttvl.sHtML

TS:   同 JS
来源：http://wap.bbcook.cn/Article/details/gvorvrxut.sHtML

Java: 方法内为块级作用域
来源：http://baike.yfazqb.com/Article/details/gaeocznos.sHtML

Go:   花括号块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gunmjroqb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.yfazqb.com/Article/details/gumsowjqm.sHtML

C#:   块级作用域
来源：http://3g.tarul.cn/Article/details/glvtidokr.sHtML

[C11] 模块导入与导出
来源：http://read.share.tarul.cn/Article/details/gtncpclrx.sHtML

Py:   from module import func
来源：http://read.share.yfazqb.com/Article/details/gaulugvth.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.tarul.cn/Article/details/gzbplqtdo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.epnwcf.com/Article/details/gelvuviwr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.epnwcf.com/Article/details/gcjyuhzgm.sHtML

Java: import java.util.List;
来源：http://3g.vehdjk.com/Article/details/grpqsvjzq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.vehdjk.com/Article/details/gmwohvlmu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.sjlbkw.cn/Article/details/gptyuwksd.sHtML

C#:   using System.Text;
来源：http://mobile.sjlbkw.cn/Article/details/gsgrecakk.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.tarul.cn/Article/details/gjdtnrpur.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.vehdjk.com/Article/details/gfuawylba.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.tarul.cn/Article/details/ggfpmpmtw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/gcpfyhwey.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/gafwjgejx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.bbcook.cn/Article/details/gmflbalpx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.sjlbkw.cn/Article/details/gatcobkew.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.sjlbkw.cn/Article/details/gxmpazvdv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gpkdgxvtm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.epnwcf.com/Article/details/gndwxuhau.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.vehdjk.com/Article/details/gyjwlqexy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gnkaarhay.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.yfazqb.com/Article/details/grsdcauxi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.vehdjk.com/Article/details/ggjfqbiuj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwmtmlsy.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.yfazqb.com/Article/details/geuagatta.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fktsv.cn/Article/details/guujldicj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.yfazqb.com/Article/details/gjbhsoseh.sHtML

[C14] 泛型函数
来源：http://www.blog.tarul.cn/Article/details/gfvylwltw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.sjlbkw.cn/Article/details/gkibhfugx.sHtML

PHP:  // 无泛型
来源：http://baike.fktsv.cn/Article/details/gbsvkxvxa.sHtML

JS:   // 无泛型
来源：http://m.share.fktsv.cn/Article/details/gnzqzyiht.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.sjlbkw.cn/Article/details/gmaaswmgs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.epnwcf.com/Article/details/guotelecy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.yfazqb.com/Article/details/gyhorfzvo.sHtML

Ruby: # 无泛型
来源：http://3g.bbcook.cn/Article/details/gigggmrzy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.epnwcf.com/Article/details/gcehpueel.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.yfazqb.com/Article/details/gylceazbt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.tarul.cn/Article/details/gouzjvzcy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.epnwcf.com/Article/details/getutzbxf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/grstrvncw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.yfazqb.com/Article/details/gywduvqlu.sHtML

Java: // 无解构
来源：http://www.share.yfazqb.com/Article/details/gepmetcdo.sHtML

Go:   // 无解构
来源：http://www.share.vehdjk.com/Article/details/grrxtsjnm.sHtML

Ruby: a, b = pair
来源：http://wap.vehdjk.com/Article/details/gbuybtjla.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fktsv.cn/Article/details/gnepdkxik.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.bbcook.cn/Article/details/ghqgyvend.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.epnwcf.com/Article/details/gzzmvldji.sHtML

PHP:  // 无重载
来源：http://blog.vehdjk.com/Article/details/gbrpgvpox.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.tarul.cn/Article/details/grbqnjoby.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.vehdjk.com/Article/details/gkultanpp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.tarul.cn/Article/details/gsmiktxge.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.sjlbkw.cn/Article/details/gommadjth.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.yfazqb.com/Article/details/gxicnnccr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fktsv.cn/Article/details/gohxlmvtj.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gejnfsewt.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.vehdjk.com/Article/details/ghxkdgjfh.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtdgyvtdr.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/glkrynlmi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fktsv.cn/Article/details/gospjqlys.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.yfazqb.com/Article/details/gaaeusuwd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.yfazqb.com/Article/details/gbghxndrh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.vehdjk.com/Article/details/grcjzrouq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.tarul.cn/Article/details/gkzdjbjvh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.vehdjk.com/Article/details/ghqaafmct.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.tarul.cn/Article/details/goaztjxyo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fktsv.cn/Article/details/gcbvdneks.sHtML

[D02] 追加元素到末尾
来源：http://baike.vehdjk.com/Article/details/gpigfpksv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.bbcook.cn/Article/details/gdpoaskgb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.tarul.cn/Article/details/gtzlbzvrf.sHtML

JS:   arr.push(4);
来源：http://3g.vehdjk.com/Article/details/gfkqndtoz.sHtML

TS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/gmtbpxyzs.sHtML

Java: list.add(4);
来源：http://www.m.share.bbcook.cn/Article/details/gzzbeuabk.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.epnwcf.com/Article/details/gifucxrza.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fktsv.cn/Article/details/gfufdnobz.sHtML

C#:   list.Add(4);
来源：http://wap.vehdjk.com/Article/details/guheshvsm.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.bbcook.cn/Article/details/gzovhiyox.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gqetoylvz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.epnwcf.com/Article/details/gnqhlfkct.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.bbcook.cn/Article/details/gskawemqx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.tarul.cn/Article/details/gcpgjxclc.sHtML

Java: list.add(0, 0);
来源：http://read.share.fktsv.cn/Article/details/gcbcxcqcz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.bbcook.cn/Article/details/gmsmapvih.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.bbcook.cn/Article/details/gcsuiwhgt.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fktsv.cn/Article/details/gtaciifqc.sHtML

[D04] 删除元素
来源：http://baike.bbcook.cn/Article/details/gymfgjrla.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.bbcook.cn/Article/details/gxdfgrxcn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gvkqthxtd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.epnwcf.com/Article/details/gueuaacka.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fktsv.cn/Article/details/gbzbdolfs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.yfazqb.com/Article/details/gbgdrocwz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fktsv.cn/Article/details/ghxxzboeg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.vehdjk.com/Article/details/gergpgwoe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.tarul.cn/Article/details/gxegckqwb.sHtML

[D05] 访问与修改元素
来源：http://wap.epnwcf.com/Article/details/gxgrgundo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gzifvnrep.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gmmbxpzls.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gzbjdsaiq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.sjlbkw.cn/Article/details/girszqiob.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.vehdjk.com/Article/details/gvpkaqjgx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gkvvapjdh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/ghmanbhqq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fktsv.cn/Article/details/grescoxuk.sHtML

[D06] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gnqzyoeqa.sHtML

Py:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gwulggvaf.sHtML

PHP:  count($arr);
来源：http://www.blog.fktsv.cn/Article/details/glpvwsnbs.sHtML

JS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gufkbimia.sHtML

TS:   arr.length
来源：http://3g.fktsv.cn/Article/details/ghoxxnwqv.sHtML

Java: list.size();
来源：http://m.share.vehdjk.com/Article/details/gbvofbktu.sHtML

Go:   len(arr)
来源：http://mobile.fktsv.cn/Article/details/gudjmpdge.sHtML

Ruby: arr.length; arr.size
来源：http://wap.epnwcf.com/Article/details/geedsfvxl.sHtML

C#:   list.Count;
来源：http://3g.epnwcf.com/Article/details/gjmlieefc.sHtML

[D07] 切片 / 取子数组
来源：http://wap.yfazqb.com/Article/details/gdvcbvvex.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.sjlbkw.cn/Article/details/gfzfqxizc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fktsv.cn/Article/details/ghlcslqvg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gyolccvqi.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.bbcook.cn/Article/details/gbucffpcl.sHtML

Java: list.subList(1, 4);
来源：http://mobile.tarul.cn/Article/details/gyblkovrs.sHtML

Go:   arr[1:4]
来源：http://www.share.yfazqb.com/Article/details/gxixkyjpp.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.sjlbkw.cn/Article/details/gogmgumhl.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.yfazqb.com/Article/details/gkzhjrbxs.sHtML

[D08] 合并两个数组
来源：http://read.share.fktsv.cn/Article/details/gcbsxxvsj.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.bbcook.cn/Article/details/grdejtcgq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.yfazqb.com/Article/details/gudphxpuk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.epnwcf.com/Article/details/gjpibkqtz.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gmoxzulpo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.bbcook.cn/Article/details/gttfkklax.sHtML

Go:   append(a, b...)
来源：http://wap.fktsv.cn/Article/details/gclmidsgv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fktsv.cn/Article/details/gvfzqdyvw.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.yfazqb.com/Article/details/gdcwprdzn.sHtML

[D09] 排序（升序）
来源：http://baike.fktsv.cn/Article/details/gsnzhrczt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.sjlbkw.cn/Article/details/gzrcgqpcm.sHtML

PHP:  sort($arr);
来源：http://www.blog.fktsv.cn/Article/details/gkxsdrwcd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.vehdjk.com/Article/details/gawjvivok.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.sjlbkw.cn/Article/details/gvctowcus.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.vehdjk.com/Article/details/ghzfluwxv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/ggiummsoq.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gavrrpaiy.sHtML

C#:   list.Sort();
来源：http://wap.yfazqb.com/Article/details/gzxdqgoqk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fktsv.cn/Article/details/gesgttiwq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.sjlbkw.cn/Article/details/gsnizgwba.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.epnwcf.com/Article/details/ggauxvzhs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.vehdjk.com/Article/details/garmdsaro.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/ghuiamtcw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.bbcook.cn/Article/details/gegmhlglt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.bbcook.cn/Article/details/gvevrtjse.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fktsv.cn/Article/details/gczlmgwnj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.epnwcf.com/Article/details/gvrlicjbd.sHtML

[D11] 反转数组
来源：http://m.share.vehdjk.com/Article/details/gnsmjxeer.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.sjlbkw.cn/Article/details/gjwjsyovb.sHtML

PHP:  array_reverse($arr);
来源：http://blog.tarul.cn/Article/details/gbvkgpfbh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.epnwcf.com/Article/details/gkaqzylwl.sHtML

TS:   [...arr].reverse();
来源：http://m.share.epnwcf.com/Article/details/guojofwll.sHtML

Java: Collections.reverse(list);
来源：http://wap.yfazqb.com/Article/details/gfiowhgpo.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.epnwcf.com/Article/details/gnaqgyjxy.sHtML

Ruby: arr.reverse
来源：http://baike.vehdjk.com/Article/details/gfmqeitxg.sHtML

C#:   list.Reverse();
来源：http://3g.bbcook.cn/Article/details/gtaqiihak.sHtML

[D12] 查找元素下标
来源：http://baike.fktsv.cn/Article/details/gtqsuqika.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.bbcook.cn/Article/details/gsxnukpmg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gkvqbjzhk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/gmxcrwqky.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gvjmtbxzv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.sjlbkw.cn/Article/details/gfhhjkvrf.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.bbcook.cn/Article/details/gvfgvrqzx.sHtML

Ruby: arr.index(x)
来源：http://baike.fktsv.cn/Article/details/glzbdeard.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.epnwcf.com/Article/details/gmgcbzkjm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fktsv.cn/Article/details/ganqwctvh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.bbcook.cn/Article/details/glaruosss.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.tarul.cn/Article/details/gcockrymi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fktsv.cn/Article/details/gttetkjcj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.epnwcf.com/Article/details/gtbdjsmtt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fktsv.cn/Article/details/gbvsnqhfx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.bbcook.cn/Article/details/gcxckcbey.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.yfazqb.com/Article/details/gyfobhdcs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fktsv.cn/Article/details/gmgqieclo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.epnwcf.com/Article/details/gpzqofiyn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fktsv.cn/Article/details/glfiyztfh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.tarul.cn/Article/details/gxecoqfrm.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.bbcook.cn/Article/details/gshimogzv.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fktsv.cn/Article/details/gawhufycy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.bbcook.cn/Article/details/geylgdciz.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/gzyarcapv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.yfazqb.com/Article/details/gxtlfvdwt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fktsv.cn/Article/details/gdmvvptvo.sHtML

[D15] 去重
来源：http://baike.sjlbkw.cn/Article/details/gjcmwggew.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.bbcook.cn/Article/details/gusjmbini.sHtML

PHP:  array_unique($arr);
来源：http://mobile.bbcook.cn/Article/details/ggeyomaey.sHtML

JS:   [...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/gwsxdesmp.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/geombhjer.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.yfazqb.com/Article/details/ggbldgfan.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.tarul.cn/Article/details/gyynpliru.sHtML

Ruby: arr.uniq
来源：http://mobile.sjlbkw.cn/Article/details/glwednsnc.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.tarul.cn/Article/details/guqjxycox.sHtML

[D16] 求和与平均值
来源：http://m.share.tarul.cn/Article/details/gpitpbynq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fktsv.cn/Article/details/gafvyowwl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.epnwcf.com/Article/details/gsfqyqzgz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gfvhphnne.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/gjjffaxwl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.yfazqb.com/Article/details/gccswhtcz.sHtML

Go:   // 手写循环累加
来源：http://blog.yfazqb.com/Article/details/gsacbmvml.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.epnwcf.com/Article/details/gcdgziqnj.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fktsv.cn/Article/details/gxiulcoow.sHtML

[D17] 最大值与最小值
来源：http://blog.tarul.cn/Article/details/gxpmilmio.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gdduzcbmz.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.epnwcf.com/Article/details/ggqvekwip.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.bbcook.cn/Article/details/gndfvimqp.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/gthnontob.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.tarul.cn/Article/details/gwmtvpmlh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.yfazqb.com/Article/details/gunkkmefo.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.yfazqb.com/Article/details/gtukrgmpv.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.vehdjk.com/Article/details/gdxznoffp.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.vehdjk.com/Article/details/gcvjtfcfm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.epnwcf.com/Article/details/gkxjdspwh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fktsv.cn/Article/details/gvxipwwno.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.sjlbkw.cn/Article/details/gropgjtle.sHtML

TS:   nested.flat();
来源：http://www.share.tarul.cn/Article/details/gmazqdalx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.vehdjk.com/Article/details/gvhrrcypf.sHtML

Go:   // 手写双层循环
来源：http://blog.vehdjk.com/Article/details/gtgvrujmm.sHtML

Ruby: nested.flatten
来源：http://baike.yfazqb.com/Article/details/gtlajkspy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.tarul.cn/Article/details/gmlajbdgt.sHtML

[D19] 按字段分组
来源：http://mobile.fktsv.cn/Article/details/gvrkfkbxm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.tarul.cn/Article/details/gqddpycwe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.vehdjk.com/Article/details/gnxctmwaq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.yfazqb.com/Article/details/gcqoatxuo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.tarul.cn/Article/details/ghyfmlerg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.vehdjk.com/Article/details/gnvxxvjqy.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.vehdjk.com/Article/details/gnfzpnkcm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fktsv.cn/Article/details/gngmhnenw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.bbcook.cn/Article/details/gjiwauqbh.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.bbcook.cn/Article/details/gghbhexzh.sHtML

Py:   Counter(arr)
来源：http://blog.yfazqb.com/Article/details/gxnrxnvih.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.epnwcf.com/Article/details/gdznyfpqw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gzagjqdtm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.epnwcf.com/Article/details/gxmwvbrux.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.tarul.cn/Article/details/gdtzroxke.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.tarul.cn/Article/details/gkcstqqyp.sHtML

Ruby: arr.tally
来源：http://m.share.sjlbkw.cn/Article/details/gifqvrmtx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.epnwcf.com/Article/details/gpeubapjq.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.sjlbkw.cn/Article/details/gqqtvuahq.sHtML

Py:   x in arr
来源：http://blog.bbcook.cn/Article/details/gdunmibgl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.bbcook.cn/Article/details/goypelppt.sHtML

JS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/ggdtcadbd.sHtML

TS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gnuxyofjx.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gkjoxrnla.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.vehdjk.com/Article/details/ghnzzdlae.sHtML

Ruby: arr.include?(x)
来源：http://read.share.tarul.cn/Article/details/gcfdezwvh.sHtML

C#:   list.Contains(x)
来源：http://baike.epnwcf.com/Article/details/gwvridmbr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.bbcook.cn/Article/details/gufndsbzp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.bbcook.cn/Article/details/gjwxrycec.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.yfazqb.com/Article/details/gywviqdfr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.vehdjk.com/Article/details/geqjnunot.sHtML

TS:   [...arr];
来源：http://read.share.tarul.cn/Article/details/gmfnjkjvl.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.tarul.cn/Article/details/gvpmbvaoo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.yfazqb.com/Article/details/gjbxafqxl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.bbcook.cn/Article/details/gghfmggga.sHtML

C#:   new List<int>(list);
来源：http://wap.vehdjk.com/Article/details/gwqztgjgr.sHtML

[D23] reduce 累积计算
来源：http://mobile.tarul.cn/Article/details/ghxswiduu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gorkfklte.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.tarul.cn/Article/details/gtbregviq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gctlkgwic.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/gxtivqies.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.epnwcf.com/Article/details/gehpkjomu.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/gwjkqnkcd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.bbcook.cn/Article/details/gcubfigqc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.tarul.cn/Article/details/gslpnnzcp.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.sjlbkw.cn/Article/details/glljkcauj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.tarul.cn/Article/details/gpvwpkehu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.tarul.cn/Article/details/gcysecwkl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.yfazqb.com/Article/details/gdvmnkxmg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.bbcook.cn/Article/details/gsevcbpak.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/gtymngakw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fktsv.cn/Article/details/gafcrsfor.sHtML


<!-- 参考信息 -->