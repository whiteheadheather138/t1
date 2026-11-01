代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gnmbwnpoo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gdxbsjsjj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/giikyqhab.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.yfazqb.com/Article/details/gtzyblvcw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.tarul.cn/Article/details/gqnbctggu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.yfazqb.com/Article/details/gzkukpaob.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.epnwcf.com/Article/details/gsqacvkaa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.sjlbkw.cn/Article/details/gjxlgcfrg.sHtML

[C10] 变量作用域
来源：http://baike.tarul.cn/Article/details/gvuggmxqd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.vehdjk.com/Article/details/gemvgsfca.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.sjlbkw.cn/Article/details/gspvjmvdr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gkorxkcke.sHtML

TS:   同 JS
来源：http://wap.epnwcf.com/Article/details/gnybydjfx.sHtML

Java: 方法内为块级作用域
来源：http://wap.vehdjk.com/Article/details/gkfgvjcdc.sHtML

Go:   花括号块级作用域
来源：http://www.share.epnwcf.com/Article/details/gmfruqoho.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.sjlbkw.cn/Article/details/gdxjvjmik.sHtML

C#:   块级作用域
来源：http://www.blog.tarul.cn/Article/details/guoamzhml.sHtML

[C11] 模块导入与导出
来源：http://blog.epnwcf.com/Article/details/gucwgqacc.sHtML

Py:   from module import func
来源：http://3g.vehdjk.com/Article/details/gdvymuezj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.epnwcf.com/Article/details/gdnvuxggd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.tarul.cn/Article/details/guhgigfdl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.epnwcf.com/Article/details/goxvkvlkw.sHtML

Java: import java.util.List;
来源：http://m.share.epnwcf.com/Article/details/gbzpyipyu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.yfazqb.com/Article/details/grxesofhk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.bbcook.cn/Article/details/gstdqopwu.sHtML

C#:   using System.Text;
来源：http://m.share.vehdjk.com/Article/details/gvucanfrf.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.yfazqb.com/Article/details/gnuvawgyi.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.vehdjk.com/Article/details/ggvkexcar.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fktsv.cn/Article/details/goschtytz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gioavnaci.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gcjrlpryh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.tarul.cn/Article/details/gpdvhrifw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.bbcook.cn/Article/details/gkfrgolxh.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.tarul.cn/Article/details/guvlqqvjl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.sjlbkw.cn/Article/details/gpetsfgln.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.yfazqb.com/Article/details/gaehnnpnv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.tarul.cn/Article/details/gicykovzq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gtffjahid.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.bbcook.cn/Article/details/gzbjjcbiy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gdzcxxxwi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gnjnsffhu.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fktsv.cn/Article/details/gvjphhrze.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.bbcook.cn/Article/details/gejnyepzj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.vehdjk.com/Article/details/gjjjbdpwl.sHtML

[C14] 泛型函数
来源：http://3g.yfazqb.com/Article/details/gqnzflmrm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.bbcook.cn/Article/details/glzwoxogk.sHtML

PHP:  // 无泛型
来源：http://www.share.yfazqb.com/Article/details/gzyhulxgl.sHtML

JS:   // 无泛型
来源：http://3g.fktsv.cn/Article/details/gxcjbqhfm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.epnwcf.com/Article/details/gpriaycov.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.yfazqb.com/Article/details/gtqmmuenf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.sjlbkw.cn/Article/details/grllzwbcp.sHtML

Ruby: # 无泛型
来源：http://www.share.vehdjk.com/Article/details/gflfjybbh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.vehdjk.com/Article/details/gusowkipk.sHtML

[C15] 解构 / 展开参数
来源：http://blog.yfazqb.com/Article/details/gjwilojxs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.epnwcf.com/Article/details/gpfgcfwsb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.yfazqb.com/Article/details/gbwjlixlx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gjczzzumy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.sjlbkw.cn/Article/details/gredrwfkf.sHtML

Java: // 无解构
来源：http://wap.fktsv.cn/Article/details/gyxtoiqqh.sHtML

Go:   // 无解构
来源：http://www.share.fktsv.cn/Article/details/gyqbbtqre.sHtML

Ruby: a, b = pair
来源：http://read.share.tarul.cn/Article/details/groqhkmza.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.epnwcf.com/Article/details/gxmgxoyql.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.tarul.cn/Article/details/gblgmhlxq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.bbcook.cn/Article/details/gxgsxlqff.sHtML

PHP:  // 无重载
来源：http://www.blog.tarul.cn/Article/details/gazcqfkux.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.tarul.cn/Article/details/guhtbcehb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fktsv.cn/Article/details/gwmncgptf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.tarul.cn/Article/details/gpclclujn.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.bbcook.cn/Article/details/gawbobnxi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fktsv.cn/Article/details/gmuzvsbsq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.vehdjk.com/Article/details/gegewdndr.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gdzusrmyk.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.bbcook.cn/Article/details/ghdfuxnzq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gytbaarzg.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gbvvxkfga.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.bbcook.cn/Article/details/gpqxuwsrb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.vehdjk.com/Article/details/gsmrrsbwz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fktsv.cn/Article/details/gjraokorm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.vehdjk.com/Article/details/gcoawlsgq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.epnwcf.com/Article/details/gvrhhsbev.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fktsv.cn/Article/details/gddzhyaxo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.bbcook.cn/Article/details/gyrvtvksu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.yfazqb.com/Article/details/ghwhvzrif.sHtML

[D02] 追加元素到末尾
来源：http://m.share.tarul.cn/Article/details/gwvjfbsqa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.vehdjk.com/Article/details/gyhpeoxeg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.vehdjk.com/Article/details/glpwjoyjp.sHtML

JS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/grtcyewkp.sHtML

TS:   arr.push(4);
来源：http://mobile.fktsv.cn/Article/details/ghkucpwce.sHtML

Java: list.add(4);
来源：http://www.m.share.epnwcf.com/Article/details/gzfuqjuzc.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.vehdjk.com/Article/details/gbuwrcnta.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.epnwcf.com/Article/details/gfkhipkxn.sHtML

C#:   list.Add(4);
来源：http://www.share.yfazqb.com/Article/details/gjejiiims.sHtML

[D03] 在指定位置插入元素
来源：http://3g.epnwcf.com/Article/details/ghkkdmtfg.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.vehdjk.com/Article/details/goelczocs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.tarul.cn/Article/details/gmgeohzab.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fktsv.cn/Article/details/gqkfjcsmu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.bbcook.cn/Article/details/gxdnfnrwn.sHtML

Java: list.add(0, 0);
来源：http://m.share.vehdjk.com/Article/details/gbitrbmem.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.yfazqb.com/Article/details/gemidqemt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.yfazqb.com/Article/details/gwftkmuqf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/ghvaetawl.sHtML

[D04] 删除元素
来源：http://www.m.share.tarul.cn/Article/details/gfaboabrt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.bbcook.cn/Article/details/gbvxnbktw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.tarul.cn/Article/details/gcadfuglf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.vehdjk.com/Article/details/gemjtejrw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.bbcook.cn/Article/details/gronpsilf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.vehdjk.com/Article/details/ghacxegxt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.tarul.cn/Article/details/gwhlfylbi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fktsv.cn/Article/details/gflgzhbzy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.vehdjk.com/Article/details/gewsupwvk.sHtML

[D05] 访问与修改元素
来源：http://read.share.bbcook.cn/Article/details/gfkfrmyft.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gpnyqdsfy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/guogyemgg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/ghcolrbqf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.vehdjk.com/Article/details/gydfcdjrk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.bbcook.cn/Article/details/gnmzkoaga.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gstdaghit.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gpltxzoyy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gvyyumosp.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gisnfjmes.sHtML

Py:   len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gtoihptmj.sHtML

PHP:  count($arr);
来源：http://wap.fktsv.cn/Article/details/gnlvitjun.sHtML

JS:   arr.length
来源：http://www.m.share.epnwcf.com/Article/details/gcwimhvqh.sHtML

TS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/grtuvsrlz.sHtML

Java: list.size();
来源：http://blog.yfazqb.com/Article/details/gfqzzatqa.sHtML

Go:   len(arr)
来源：http://baike.yfazqb.com/Article/details/gdhnbzqri.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fktsv.cn/Article/details/gbttnpvef.sHtML

C#:   list.Count;
来源：http://baike.vehdjk.com/Article/details/gbyglkszd.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.bbcook.cn/Article/details/glbutkmih.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.epnwcf.com/Article/details/gtvagpqtb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/glkjydfhc.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gatqgvthi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gmneekyxm.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gauwksrnu.sHtML

Go:   arr[1:4]
来源：http://baike.tarul.cn/Article/details/gozbhwrdo.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.tarul.cn/Article/details/gtpqcedoc.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gxtwlelci.sHtML

[D08] 合并两个数组
来源：http://www.share.bbcook.cn/Article/details/gonjooovt.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.tarul.cn/Article/details/gqtaxitbk.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.sjlbkw.cn/Article/details/gpjxpolzq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.bbcook.cn/Article/details/gufnmrvxu.sHtML

TS:   [...a, ...b];
来源：http://www.share.yfazqb.com/Article/details/gwitpytyh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fktsv.cn/Article/details/grawsbtbm.sHtML

Go:   append(a, b...)
来源：http://3g.vehdjk.com/Article/details/gvsymoxqk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.epnwcf.com/Article/details/gnvzybvas.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.bbcook.cn/Article/details/gciplnkhd.sHtML

[D09] 排序（升序）
来源：http://www.blog.yfazqb.com/Article/details/gqqluqgro.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gncfizuln.sHtML

PHP:  sort($arr);
来源：http://www.blog.bbcook.cn/Article/details/gwwbhzata.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.sjlbkw.cn/Article/details/gknfxlhlc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.tarul.cn/Article/details/gxnfmqtuv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.vehdjk.com/Article/details/ggejeyqwg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gwshxhont.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/goghfpgkt.sHtML

C#:   list.Sort();
来源：http://www.m.share.tarul.cn/Article/details/gzcablyaz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.bbcook.cn/Article/details/gijppjmnp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.sjlbkw.cn/Article/details/gnkhdedvt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.bbcook.cn/Article/details/gnqyrrmxd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.yfazqb.com/Article/details/gfwzeydqh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gssptrjnd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.bbcook.cn/Article/details/gpfyrcwgs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.tarul.cn/Article/details/gskkbhxuu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.epnwcf.com/Article/details/gdwasxlhg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.bbcook.cn/Article/details/gmyyarqbz.sHtML

[D11] 反转数组
来源：http://baike.fktsv.cn/Article/details/ghtrdlqpo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.yfazqb.com/Article/details/gkokiudos.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.yfazqb.com/Article/details/giztztdbl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.tarul.cn/Article/details/gfstozftu.sHtML

TS:   [...arr].reverse();
来源：http://www.share.tarul.cn/Article/details/gxtxvgceq.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/gegtrvprc.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gmlqmbphj.sHtML

Ruby: arr.reverse
来源：http://wap.fktsv.cn/Article/details/gzjpccitd.sHtML

C#:   list.Reverse();
来源：http://wap.epnwcf.com/Article/details/gmnehooyt.sHtML

[D12] 查找元素下标
来源：http://baike.vehdjk.com/Article/details/gnbmyflhg.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.yfazqb.com/Article/details/gznpqscul.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.vehdjk.com/Article/details/gecmujdoh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/grlbmqoan.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gwkjlxqlj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.bbcook.cn/Article/details/gxkouadti.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.yfazqb.com/Article/details/gkuvwxllg.sHtML

Ruby: arr.index(x)
来源：http://read.share.epnwcf.com/Article/details/gavqsweur.sHtML

C#:   list.IndexOf(x);
来源：http://blog.epnwcf.com/Article/details/gnmwseutt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.sjlbkw.cn/Article/details/ghqaullhp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.vehdjk.com/Article/details/gnapbgnrv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.bbcook.cn/Article/details/gogyuvfvd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.vehdjk.com/Article/details/ghzcdslgx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvljcsgay.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.yfazqb.com/Article/details/gilqqloxr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.yfazqb.com/Article/details/gpscxqdxi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.bbcook.cn/Article/details/gsnrckdms.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.epnwcf.com/Article/details/gtbhssewf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.vehdjk.com/Article/details/gpyzpiokk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.sjlbkw.cn/Article/details/gthhpigrc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.bbcook.cn/Article/details/gjxytqdxc.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gtdzbijbx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/geuathlcb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.sjlbkw.cn/Article/details/grnsdtspj.sHtML

Go:   // 手写循环
来源：http://baike.epnwcf.com/Article/details/gwhawzsxa.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.tarul.cn/Article/details/ghxkqtkff.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.bbcook.cn/Article/details/gaxrvlwgg.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gcpiuligf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fktsv.cn/Article/details/gypayxzdn.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.yfazqb.com/Article/details/geevtviiw.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gibpffvlh.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gxdwgafse.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.epnwcf.com/Article/details/glyojqokb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.yfazqb.com/Article/details/giuposstq.sHtML

Ruby: arr.uniq
来源：http://wap.vehdjk.com/Article/details/gpylocrha.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwyskuaef.sHtML

[D16] 求和与平均值
来源：http://wap.epnwcf.com/Article/details/gprbmyfxh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.yfazqb.com/Article/details/gnamhrvnn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.bbcook.cn/Article/details/gybrbhrbv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gobkmrsnk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/gqmgwybyh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.vehdjk.com/Article/details/gbohdvfdj.sHtML

Go:   // 手写循环累加
来源：http://baike.yfazqb.com/Article/details/grucfzqhx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.epnwcf.com/Article/details/gdoeboywf.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.yfazqb.com/Article/details/gxreeubzf.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.tarul.cn/Article/details/grxlzomqe.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.yfazqb.com/Article/details/gstatkjsj.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.epnwcf.com/Article/details/gdkfpgdyu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.yfazqb.com/Article/details/gmcitqatv.sHtML

TS:   Math.max(...arr);
来源：http://read.share.yfazqb.com/Article/details/gsadqqmec.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.tarul.cn/Article/details/gudnamnin.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.bbcook.cn/Article/details/gotevbden.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.vehdjk.com/Article/details/gaqyvhujj.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fktsv.cn/Article/details/gjkttamnv.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.yfazqb.com/Article/details/gjuirraqf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.epnwcf.com/Article/details/gxwrifpky.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.tarul.cn/Article/details/gslisfdkd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.epnwcf.com/Article/details/gtgdeionk.sHtML

TS:   nested.flat();
来源：http://baike.yfazqb.com/Article/details/gbdeljvaa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.vehdjk.com/Article/details/gepueabji.sHtML

Go:   // 手写双层循环
来源：http://www.blog.epnwcf.com/Article/details/ghtjicyvp.sHtML

Ruby: nested.flatten
来源：http://baike.yfazqb.com/Article/details/gwogycicb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gtgieqyen.sHtML

[D19] 按字段分组
来源：http://blog.vehdjk.com/Article/details/gnkwjxjga.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.epnwcf.com/Article/details/gbsdxblyi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.bbcook.cn/Article/details/grfcnmfic.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fktsv.cn/Article/details/gstttctol.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/ggufdsbvy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.bbcook.cn/Article/details/gtzrykdjr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fktsv.cn/Article/details/gofjglvwr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fktsv.cn/Article/details/gkfspbbft.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.epnwcf.com/Article/details/gyuttkuae.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fktsv.cn/Article/details/gpgmiyida.sHtML

Py:   Counter(arr)
来源：http://www.share.vehdjk.com/Article/details/gbqxttnab.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.epnwcf.com/Article/details/glcvgcojl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/grvyxvykp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gcidzurtt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.bbcook.cn/Article/details/gurgqpafm.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.epnwcf.com/Article/details/gvapqkcic.sHtML

Ruby: arr.tally
来源：http://3g.bbcook.cn/Article/details/gqacpwrvc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.tarul.cn/Article/details/gcrgjdknm.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.yfazqb.com/Article/details/gnxtfpenm.sHtML

Py:   x in arr
来源：http://baike.fktsv.cn/Article/details/ggnvjogkm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.sjlbkw.cn/Article/details/gmbmdstip.sHtML

JS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gnsvqdhkl.sHtML

TS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gatyjmarc.sHtML

Java: list.contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gdzglkjfl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gyxbmhepi.sHtML

Ruby: arr.include?(x)
来源：http://wap.yfazqb.com/Article/details/gbwhsysze.sHtML

C#:   list.Contains(x)
来源：http://wap.tarul.cn/Article/details/gjxwvegtd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.vehdjk.com/Article/details/gelaoudso.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.bbcook.cn/Article/details/ghwpklugv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.yfazqb.com/Article/details/goztneskx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.bbcook.cn/Article/details/ghrvjnoft.sHtML

TS:   [...arr];
来源：http://read.share.sjlbkw.cn/Article/details/gnsdqbvaf.sHtML

Java: new ArrayList<>(list);
来源：http://wap.bbcook.cn/Article/details/gqdrofwke.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.tarul.cn/Article/details/gycyuibpu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgpehtsi.sHtML

C#:   new List<int>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gprodeexw.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgxtniqu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.epnwcf.com/Article/details/gutgpahmy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gbdihdsoh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/gdkeqnsjc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/gpftqupvt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.vehdjk.com/Article/details/gxscvswxf.sHtML

Go:   // 手写循环
来源：http://www.share.fktsv.cn/Article/details/gqxjmmaxy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.vehdjk.com/Article/details/girhresqv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.epnwcf.com/Article/details/gdyjrpeyz.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fktsv.cn/Article/details/gxmpufylj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.vehdjk.com/Article/details/gzullmyhh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gxljldusp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.yfazqb.com/Article/details/ggrgwdqfa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gmlsrmggg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fktsv.cn/Article/details/gnoicntjw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.bbcook.cn/Article/details/gzugsmpen.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.epnwcf.com/Article/details/gvshegxyg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.sjlbkw.cn/Article/details/guqndjxge.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.epnwcf.com/Article/details/grtxapyyn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.yfazqb.com/Article/details/gwhqggngl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.yfazqb.com/Article/details/gftxtxuex.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.epnwcf.com/Article/details/ghqtarqaj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.sjlbkw.cn/Article/details/gqkutievj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.tarul.cn/Article/details/grqqalugz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fktsv.cn/Article/details/glgmviloh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.sjlbkw.cn/Article/details/gqvuquveo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.tarul.cn/Article/details/gjjyyrftf.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/gbovhtyey.sHtML


<!-- 参考信息 -->