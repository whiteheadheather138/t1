代发 wailian999

C#:   块级作用域
来源：http://blog.fktsv.cn/Article/details/geflmfonr.sHtML

[C11] 模块导入与导出
来源：http://read.share.fktsv.cn/Article/details/gvryqxqaz.sHtML

Py:   from module import func
来源：http://mobile.yfazqb.com/Article/details/gtwevbbjx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.yfazqb.com/Article/details/gxerjdnym.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.bbcook.cn/Article/details/grnkkhvxo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.sjlbkw.cn/Article/details/grvlbrtne.sHtML

Java: import java.util.List;
来源：http://baike.epnwcf.com/Article/details/ghxfjqqbw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.vehdjk.com/Article/details/ggstycfly.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.yfazqb.com/Article/details/gimxlmlnx.sHtML

C#:   using System.Text;
来源：http://m.share.bbcook.cn/Article/details/gfwyusbdy.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.bbcook.cn/Article/details/gtfmydpkb.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.vehdjk.com/Article/details/gjvgtqoxf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.epnwcf.com/Article/details/ggtqxtxuo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gsmbqdrfn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.bbcook.cn/Article/details/ggalajlhw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.yfazqb.com/Article/details/geitrvqbi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/gaqkzsmzc.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.bbcook.cn/Article/details/gcmpyksnq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.vehdjk.com/Article/details/giczkqvga.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.bbcook.cn/Article/details/gmhhohfdz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.bbcook.cn/Article/details/gmtiucssi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gwofmvpib.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.sjlbkw.cn/Article/details/gfigphpsd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/ggllrirar.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gjwirflpa.sHtML

Go:   func add(a, b int) int
来源：http://blog.bbcook.cn/Article/details/gemlpzaww.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fktsv.cn/Article/details/gbunfhyld.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.epnwcf.com/Article/details/gnelryiux.sHtML

[C14] 泛型函数
来源：http://www.blog.fktsv.cn/Article/details/gnkzgdaun.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.yfazqb.com/Article/details/gtsevewcb.sHtML

PHP:  // 无泛型
来源：http://read.share.yfazqb.com/Article/details/gcylqmmxb.sHtML

JS:   // 无泛型
来源：http://m.share.tarul.cn/Article/details/glkreeeto.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.epnwcf.com/Article/details/gpussdiuo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlvjelbk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fktsv.cn/Article/details/gncoqzfpf.sHtML

Ruby: # 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gzpmszvxb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.sjlbkw.cn/Article/details/gelfjwjer.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gdlqgygpp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.tarul.cn/Article/details/geaxlpyvb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.epnwcf.com/Article/details/gnosdxiil.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gxgyqdqeo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.bbcook.cn/Article/details/glyvinjzw.sHtML

Java: // 无解构
来源：http://mobile.bbcook.cn/Article/details/govucvgyf.sHtML

Go:   // 无解构
来源：http://blog.tarul.cn/Article/details/getcwnwgk.sHtML

Ruby: a, b = pair
来源：http://blog.yfazqb.com/Article/details/grueolgph.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.epnwcf.com/Article/details/gejjizyjy.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.bbcook.cn/Article/details/gawvusnbm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.tarul.cn/Article/details/gmjumrzbq.sHtML

PHP:  // 无重载
来源：http://wap.epnwcf.com/Article/details/gbflnkvnh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.epnwcf.com/Article/details/gjlromykd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.bbcook.cn/Article/details/gzdzfmajc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.bbcook.cn/Article/details/gmujtgjxu.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.tarul.cn/Article/details/gwhlgjyop.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.vehdjk.com/Article/details/gcvdeflds.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fktsv.cn/Article/details/gnkcnbgiz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzhfsoqab.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.tarul.cn/Article/details/gawolzirv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjpaiflgc.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.yfazqb.com/Article/details/gxrdowkzn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fktsv.cn/Article/details/ggyhugpxz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fktsv.cn/Article/details/genyhbjfe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.tarul.cn/Article/details/gxldlbbpp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.yfazqb.com/Article/details/gcgtirkeq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/gwesvztlp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.vehdjk.com/Article/details/gooiqtwxs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.vehdjk.com/Article/details/gwhvgbccu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.bbcook.cn/Article/details/gceyiwzgc.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fktsv.cn/Article/details/gyckgdabm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.epnwcf.com/Article/details/gjqfqikod.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.tarul.cn/Article/details/gkcewqoqs.sHtML

JS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gujenzvws.sHtML

TS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/glypkmaib.sHtML

Java: list.add(4);
来源：http://m.share.bbcook.cn/Article/details/gtjnysdfa.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.epnwcf.com/Article/details/gmauofwad.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.epnwcf.com/Article/details/gytygiqlp.sHtML

C#:   list.Add(4);
来源：http://read.share.sjlbkw.cn/Article/details/gtghhuvsc.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhrwwfmu.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.epnwcf.com/Article/details/giooxlpiy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.tarul.cn/Article/details/gpsmkvaba.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.sjlbkw.cn/Article/details/gfbahhvhw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fktsv.cn/Article/details/gwslhyqrs.sHtML

Java: list.add(0, 0);
来源：http://blog.fktsv.cn/Article/details/gaxifnwaf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.tarul.cn/Article/details/ghwtdpenw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.epnwcf.com/Article/details/grbrvwusw.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fktsv.cn/Article/details/gizdzoqqr.sHtML

[D04] 删除元素
来源：http://mobile.epnwcf.com/Article/details/grwadtqzg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.tarul.cn/Article/details/gjutavanl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.epnwcf.com/Article/details/gbdfxajqj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.tarul.cn/Article/details/gwzqhnnwt.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.tarul.cn/Article/details/gtynnmjvr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fktsv.cn/Article/details/gvkobsdlx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.tarul.cn/Article/details/gdsaldeob.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fktsv.cn/Article/details/glvbeoztf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.yfazqb.com/Article/details/gqhonigtf.sHtML

[D05] 访问与修改元素
来源：http://3g.sjlbkw.cn/Article/details/grlihgycz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gjkupytsj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/golgutayf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gpwtuahan.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.tarul.cn/Article/details/gmhxdxkyf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.vehdjk.com/Article/details/gguotmydw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/gkrcuwtdo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/geymxubem.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/goczwybst.sHtML

[D06] 数组长度
来源：http://mobile.tarul.cn/Article/details/gxuvqerif.sHtML

Py:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gfzayizup.sHtML

PHP:  count($arr);
来源：http://wap.epnwcf.com/Article/details/gagfbrays.sHtML

JS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gzvnmoomd.sHtML

TS:   arr.length
来源：http://blog.bbcook.cn/Article/details/gxlbraxof.sHtML

Java: list.size();
来源：http://read.share.yfazqb.com/Article/details/grojdfoyi.sHtML

Go:   len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnfweaqw.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gpqhvvzfp.sHtML

C#:   list.Count;
来源：http://baike.sjlbkw.cn/Article/details/gzqjbqvul.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.vehdjk.com/Article/details/gllubxsaw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.yfazqb.com/Article/details/gfwonhepu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.epnwcf.com/Article/details/gfmwydcff.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.bbcook.cn/Article/details/gmfpvwpgx.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gxdcynghl.sHtML

Java: list.subList(1, 4);
来源：http://baike.vehdjk.com/Article/details/gbyyzxakl.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/gxmeguwmr.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.vehdjk.com/Article/details/gvlzrpwim.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.tarul.cn/Article/details/gnndsourd.sHtML

[D08] 合并两个数组
来源：http://blog.fktsv.cn/Article/details/gloghstnm.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.bbcook.cn/Article/details/grcpuubut.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fktsv.cn/Article/details/ggxijfkmx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fktsv.cn/Article/details/gqqpqqyeu.sHtML

TS:   [...a, ...b];
来源：http://wap.vehdjk.com/Article/details/gfwwgzyeo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.vehdjk.com/Article/details/gzyzyafkz.sHtML

Go:   append(a, b...)
来源：http://blog.sjlbkw.cn/Article/details/gktkzljqa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.bbcook.cn/Article/details/gsmhyapak.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gebomsefs.sHtML

[D09] 排序（升序）
来源：http://www.share.epnwcf.com/Article/details/ghqyekpoe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/glabsvivd.sHtML

PHP:  sort($arr);
来源：http://mobile.sjlbkw.cn/Article/details/geerplqms.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/gqqwnuxzj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.epnwcf.com/Article/details/gqpeewsjn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvvuueqn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/gqpchrlrp.sHtML

Ruby: arr.sort
来源：http://baike.yfazqb.com/Article/details/ggesxvzrt.sHtML

C#:   list.Sort();
来源：http://blog.fktsv.cn/Article/details/gdteqcggp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.yfazqb.com/Article/details/gclpuzexl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.sjlbkw.cn/Article/details/ggxfplitl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/gbqolelbo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/ggjrsvmvz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/gnbyrewgt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.sjlbkw.cn/Article/details/gcsjopllb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.epnwcf.com/Article/details/gzuoqsyjo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.sjlbkw.cn/Article/details/giyneihvl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.vehdjk.com/Article/details/giksvkgsu.sHtML

[D11] 反转数组
来源：http://www.m.share.bbcook.cn/Article/details/gyulkateq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.vehdjk.com/Article/details/ggqgajjgb.sHtML

PHP:  array_reverse($arr);
来源：http://blog.epnwcf.com/Article/details/gwjwsoptp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fktsv.cn/Article/details/gyntzqkfo.sHtML

TS:   [...arr].reverse();
来源：http://baike.bbcook.cn/Article/details/gmsxsvpam.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/gugndgapw.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.bbcook.cn/Article/details/gpwptfjfz.sHtML

Ruby: arr.reverse
来源：http://m.share.fktsv.cn/Article/details/gahvynsyr.sHtML

C#:   list.Reverse();
来源：http://baike.yfazqb.com/Article/details/gufgymcjv.sHtML

[D12] 查找元素下标
来源：http://baike.sjlbkw.cn/Article/details/gyyvzihoh.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.vehdjk.com/Article/details/ghhrtbvrr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.epnwcf.com/Article/details/gqroubwuz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.yfazqb.com/Article/details/gbaxtekjy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.sjlbkw.cn/Article/details/goeavclny.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.tarul.cn/Article/details/gevuanlxz.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gvqvxtmvu.sHtML

Ruby: arr.index(x)
来源：http://mobile.tarul.cn/Article/details/gllzoerlw.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.tarul.cn/Article/details/gguphqsuo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.tarul.cn/Article/details/gqmkqlvbr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fktsv.cn/Article/details/gmqdpdhdg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.tarul.cn/Article/details/gzmnbvxxw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/gtbiyjgrh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/gymugokec.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.sjlbkw.cn/Article/details/ggzsgiqyn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.vehdjk.com/Article/details/gelbocupi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.tarul.cn/Article/details/glfokqsoo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.epnwcf.com/Article/details/gnwotehup.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.epnwcf.com/Article/details/gofdzsimn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.yfazqb.com/Article/details/ghyrcleoo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.epnwcf.com/Article/details/guwyeywun.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.epnwcf.com/Article/details/glpqanwdc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gbebjrytw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.yfazqb.com/Article/details/gijobjeto.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/grfkaobbg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gfqjwfrsi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gjmbdoxrm.sHtML

[D15] 去重
来源：http://read.share.vehdjk.com/Article/details/gihwecdqn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/giqlmbmqp.sHtML

PHP:  array_unique($arr);
来源：http://read.share.tarul.cn/Article/details/gkghwismi.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/grsxomuix.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gujdlxkzh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/gbfsirjbi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.yfazqb.com/Article/details/gssmyiqpe.sHtML

Ruby: arr.uniq
来源：http://www.blog.sjlbkw.cn/Article/details/gzzqpszuw.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.epnwcf.com/Article/details/gkfguzozo.sHtML

[D16] 求和与平均值
来源：http://blog.vehdjk.com/Article/details/gfsuqsexd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gvsrjtxdm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.yfazqb.com/Article/details/goxlnncuf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gwxpxbkqd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/gbckqlyqv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/gfuntywoi.sHtML

Go:   // 手写循环累加
来源：http://blog.vehdjk.com/Article/details/gnzmixgtx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.epnwcf.com/Article/details/grzyipddo.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fktsv.cn/Article/details/gzqvejpbv.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.epnwcf.com/Article/details/gkqslpjxy.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.bbcook.cn/Article/details/gxvgacjdr.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.bbcook.cn/Article/details/guzjosvqj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.sjlbkw.cn/Article/details/gxmxtttct.sHtML

TS:   Math.max(...arr);
来源：http://m.share.yfazqb.com/Article/details/gznwecieq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.sjlbkw.cn/Article/details/gskfydvxr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.vehdjk.com/Article/details/goaljlbhc.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fktsv.cn/Article/details/gcuupypvh.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fktsv.cn/Article/details/gjurluhgy.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fktsv.cn/Article/details/gqoqoocut.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.vehdjk.com/Article/details/grdcvzikn.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.tarul.cn/Article/details/giehipdkv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.bbcook.cn/Article/details/grbcwwohu.sHtML

TS:   nested.flat();
来源：http://wap.tarul.cn/Article/details/gzmulpmyi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fktsv.cn/Article/details/gbaxiboir.sHtML

Go:   // 手写双层循环
来源：http://3g.sjlbkw.cn/Article/details/gnzefdcfp.sHtML

Ruby: nested.flatten
来源：http://www.share.fktsv.cn/Article/details/gemljqkjr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.epnwcf.com/Article/details/gebhvezaa.sHtML

[D19] 按字段分组
来源：http://www.m.share.yfazqb.com/Article/details/ggzzestjj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.bbcook.cn/Article/details/ghkznlzlm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.epnwcf.com/Article/details/gcwhagold.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fktsv.cn/Article/details/gxehsqfwn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.vehdjk.com/Article/details/gpunocvgd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.sjlbkw.cn/Article/details/giqesbpnj.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.tarul.cn/Article/details/gkygrpubc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.epnwcf.com/Article/details/ggmmycwtk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.epnwcf.com/Article/details/gtdyitemz.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.tarul.cn/Article/details/gwcumpcos.sHtML

Py:   Counter(arr)
来源：http://www.share.bbcook.cn/Article/details/gyalymqar.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.vehdjk.com/Article/details/gibhkxoiw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gcvjgjexm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gynnddzzg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.epnwcf.com/Article/details/gyeveyiib.sHtML

Go:   // 手写 map[T]int
来源：http://blog.tarul.cn/Article/details/gugnieqtc.sHtML

Ruby: arr.tally
来源：http://baike.sjlbkw.cn/Article/details/gkivfwnyg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.epnwcf.com/Article/details/gwjnkcrok.sHtML

[D21] 判断是否包含某元素
来源：http://blog.bbcook.cn/Article/details/gtiandtdl.sHtML

Py:   x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gwxkkdlhr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.yfazqb.com/Article/details/gosgacjdn.sHtML

JS:   arr.includes(x)
来源：http://mobile.epnwcf.com/Article/details/gltfxbqby.sHtML

TS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gykrqvfwl.sHtML

Java: list.contains(x)
来源：http://mobile.epnwcf.com/Article/details/geyoksvgn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gdqukzvaj.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gzhelapup.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/gmhrxyorh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.vehdjk.com/Article/details/gunaxfspb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.sjlbkw.cn/Article/details/gomordrcl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.bbcook.cn/Article/details/gfpymsnlc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gvutvcrwr.sHtML

TS:   [...arr];
来源：http://m.share.fktsv.cn/Article/details/gwuyprtwk.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.epnwcf.com/Article/details/gwxdjaqtr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fktsv.cn/Article/details/guvzmvcrz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.yfazqb.com/Article/details/guotsbxer.sHtML

C#:   new List<int>(list);
来源：http://mobile.epnwcf.com/Article/details/ggqyugtuv.sHtML

[D23] reduce 累积计算
来源：http://m.share.fktsv.cn/Article/details/ggrjiizsn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gekvxeunj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.vehdjk.com/Article/details/gffvftjur.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/ggewjyphs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gximwlqsw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.bbcook.cn/Article/details/gcnavefal.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gqenndyly.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.tarul.cn/Article/details/gcddybqcb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fktsv.cn/Article/details/gzzcnsdcy.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.sjlbkw.cn/Article/details/gufbpokwc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.epnwcf.com/Article/details/gxadneyhj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.vehdjk.com/Article/details/ghinnimzb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.epnwcf.com/Article/details/gtosetqkd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.vehdjk.com/Article/details/gvhgabwhn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.epnwcf.com/Article/details/gllmorhsk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.epnwcf.com/Article/details/gnlndbiwx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.tarul.cn/Article/details/gndcfdrgt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.vehdjk.com/Article/details/gbdxqmtek.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.vehdjk.com/Article/details/gqbssfsft.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fktsv.cn/Article/details/gcwtebtrj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.yfazqb.com/Article/details/gwxvdtoro.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.bbcook.cn/Article/details/gtwbautnh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fktsv.cn/Article/details/gqcpbkdvr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.epnwcf.com/Article/details/gpeizgygi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fktsv.cn/Article/details/gxzcilfnd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.bbcook.cn/Article/details/gurdjcpzh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.epnwcf.com/Article/details/gocgmyweb.sHtML

[D26] 数组转字符串
来源：http://m.share.epnwcf.com/Article/details/gilqzmkur.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.tarul.cn/Article/details/gktycmhus.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.vehdjk.com/Article/details/gxemrslux.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gbprtmhuz.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gouzjdsyl.sHtML

Java: String.join(", ", list)
来源：http://read.share.tarul.cn/Article/details/gygiovtxf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.epnwcf.com/Article/details/glacbhoag.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gruckeyfn.sHtML

C#:   string.Join(", ", list)
来源：http://baike.tarul.cn/Article/details/gwzvuhrwf.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gywovovbl.sHtML

E. 字符串处理
来源：http://baike.vehdjk.com/Article/details/gsjrycsrm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghvhekxya.sHtML

[E01] 拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gllheucmx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.bbcook.cn/Article/details/gorvkxafr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.tarul.cn/Article/details/gzusvxcbg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/gddosnvai.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gctnqngkb.sHtML


<!-- 参考信息 -->