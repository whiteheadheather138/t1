代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/guicwwkbw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.yfazqb.com/Article/details/gvfekhzgc.sHtML

Java: import java.util.List;
来源：http://m.share.yfazqb.com/Article/details/gvzqygugf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.yfazqb.com/Article/details/gjdkhzfcz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.bbcook.cn/Article/details/gaupyfizw.sHtML

C#:   using System.Text;
来源：http://read.share.tarul.cn/Article/details/geylawkoi.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.sjlbkw.cn/Article/details/gixstityf.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.epnwcf.com/Article/details/gyxcfycaw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fktsv.cn/Article/details/gllhlxios.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gyubffzmm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fktsv.cn/Article/details/gdlhiabus.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.tarul.cn/Article/details/gnrufjunw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.epnwcf.com/Article/details/gdmxdkfdc.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fktsv.cn/Article/details/gvviwwawp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fktsv.cn/Article/details/ggxwvoiim.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fktsv.cn/Article/details/gdtbyfmgg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.bbcook.cn/Article/details/gexcatoxo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gtcvtzswq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fktsv.cn/Article/details/gvoqyrqhg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gknqvthpx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gzbsebvqm.sHtML

Go:   func add(a, b int) int
来源：http://mobile.vehdjk.com/Article/details/gdvybgrez.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.vehdjk.com/Article/details/gpgrhccnd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fktsv.cn/Article/details/ggzyahcyg.sHtML

[C14] 泛型函数
来源：http://blog.tarul.cn/Article/details/gwhhqqsgb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.bbcook.cn/Article/details/gtgiahwtx.sHtML

PHP:  // 无泛型
来源：http://m.share.fktsv.cn/Article/details/gjqudroon.sHtML

JS:   // 无泛型
来源：http://read.share.epnwcf.com/Article/details/gtrpfefrv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.yfazqb.com/Article/details/gnclcywas.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gghkzgaxo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fktsv.cn/Article/details/grbtbzrzp.sHtML

Ruby: # 无泛型
来源：http://m.share.yfazqb.com/Article/details/gmofjbcvp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.epnwcf.com/Article/details/gdkwdihxt.sHtML

[C15] 解构 / 展开参数
来源：http://blog.sjlbkw.cn/Article/details/gdighjwoy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.epnwcf.com/Article/details/ghaizwdsm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.epnwcf.com/Article/details/gknwkjsmw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/glxkrwsch.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.yfazqb.com/Article/details/gqrlsaeoi.sHtML

Java: // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/glvpztitg.sHtML

Go:   // 无解构
来源：http://blog.sjlbkw.cn/Article/details/gxxetbrbm.sHtML

Ruby: a, b = pair
来源：http://baike.tarul.cn/Article/details/gfofqkhhg.sHtML

C#:   var (a, b) = pair;
来源：http://baike.vehdjk.com/Article/details/gfdzqraxj.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.bbcook.cn/Article/details/gkglyoeas.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.epnwcf.com/Article/details/gxeilpwdc.sHtML

PHP:  // 无重载
来源：http://m.share.fktsv.cn/Article/details/gnlzzobkt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.yfazqb.com/Article/details/gjtzpckbh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.tarul.cn/Article/details/gvxlqzxce.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.sjlbkw.cn/Article/details/gkaygmcud.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.tarul.cn/Article/details/gpdxxlaeh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.yfazqb.com/Article/details/gkoworiqt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.tarul.cn/Article/details/gjphpznfp.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gofeyxrhz.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.sjlbkw.cn/Article/details/gujkpfasj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gsfravhlu.sHtML

[D01] 创建数组 / 列表
来源：http://blog.tarul.cn/Article/details/gxdbyxkbo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.tarul.cn/Article/details/gcrxgvbqf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fktsv.cn/Article/details/gzjtfvpex.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.vehdjk.com/Article/details/gdtgnzczf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.yfazqb.com/Article/details/gahjgxtbl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.bbcook.cn/Article/details/gtxctoive.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fktsv.cn/Article/details/gafjyyecb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.sjlbkw.cn/Article/details/gazgkdlzj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.tarul.cn/Article/details/gsqoqevlm.sHtML

[D02] 追加元素到末尾
来源：http://wap.sjlbkw.cn/Article/details/gwzssenyn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fktsv.cn/Article/details/giuowhrvx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/gdgtwhqfo.sHtML

JS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/ggyrftnon.sHtML

TS:   arr.push(4);
来源：http://www.blog.fktsv.cn/Article/details/gqqliaatp.sHtML

Java: list.add(4);
来源：http://blog.vehdjk.com/Article/details/gkoorjsmg.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.tarul.cn/Article/details/gjlfmjsum.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.yfazqb.com/Article/details/gvmqjfief.sHtML

C#:   list.Add(4);
来源：http://blog.vehdjk.com/Article/details/goieszfhv.sHtML

[D03] 在指定位置插入元素
来源：http://3g.sjlbkw.cn/Article/details/giryriztq.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.tarul.cn/Article/details/gxajrgkyy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.bbcook.cn/Article/details/gqdpcyhwt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.sjlbkw.cn/Article/details/gnvkqmmbx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fktsv.cn/Article/details/ggchdwjpr.sHtML

Java: list.add(0, 0);
来源：http://baike.vehdjk.com/Article/details/gpemrpmkz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.yfazqb.com/Article/details/gfqhbhlil.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.tarul.cn/Article/details/gsfjplaxl.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.tarul.cn/Article/details/gdtqthggb.sHtML

[D04] 删除元素
来源：http://www.blog.epnwcf.com/Article/details/gzyxketcq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fktsv.cn/Article/details/govlkabub.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.bbcook.cn/Article/details/guzoxmxej.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.yfazqb.com/Article/details/gomrxfsxf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fktsv.cn/Article/details/gxymyfxnm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.vehdjk.com/Article/details/giozowfvl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.yfazqb.com/Article/details/gqmnwybyh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gigmfbnlu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.epnwcf.com/Article/details/goelolble.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gegatetwy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/guallzbus.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gznkianca.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gajadphdt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.vehdjk.com/Article/details/gtlvzuclc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.tarul.cn/Article/details/gurtdqpsa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/giwfsounj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/grkoxrpug.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gbiplyyob.sHtML

[D06] 数组长度
来源：http://wap.fktsv.cn/Article/details/gzuzxqrrl.sHtML

Py:   len(arr)
来源：http://wap.tarul.cn/Article/details/gbdlmjrse.sHtML

PHP:  count($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gohxpqrvp.sHtML

JS:   arr.length
来源：http://3g.fktsv.cn/Article/details/gvlwsxjjg.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/gvagzjxyi.sHtML

Java: list.size();
来源：http://www.share.bbcook.cn/Article/details/guhqlmvbx.sHtML

Go:   len(arr)
来源：http://mobile.fktsv.cn/Article/details/gtvvzxczf.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.bbcook.cn/Article/details/gtvorgtij.sHtML

C#:   list.Count;
来源：http://wap.fktsv.cn/Article/details/gfpasjyht.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.tarul.cn/Article/details/gxazdsgvd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.tarul.cn/Article/details/gpbpnxwuc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.bbcook.cn/Article/details/gyvtnrorc.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.yfazqb.com/Article/details/gxadqhwkl.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gtmnnyuxa.sHtML

Java: list.subList(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gmuanowus.sHtML

Go:   arr[1:4]
来源：http://www.share.fktsv.cn/Article/details/gowxipzda.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.yfazqb.com/Article/details/gbzfukshu.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.epnwcf.com/Article/details/grbnjkoiy.sHtML

[D08] 合并两个数组
来源：http://www.blog.vehdjk.com/Article/details/gpxsivpzv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.yfazqb.com/Article/details/gtgtdzash.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.epnwcf.com/Article/details/gkysucpcr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.bbcook.cn/Article/details/gbeinoaiv.sHtML

TS:   [...a, ...b];
来源：http://www.blog.vehdjk.com/Article/details/gwekuqqnv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/grqfbbawe.sHtML

Go:   append(a, b...)
来源：http://wap.tarul.cn/Article/details/gomansupm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.epnwcf.com/Article/details/gbephewgp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gdbcahfmd.sHtML

[D09] 排序（升序）
来源：http://read.share.fktsv.cn/Article/details/gzwbzjtil.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gyydwgxdr.sHtML

PHP:  sort($arr);
来源：http://read.share.fktsv.cn/Article/details/gahjfnxjl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fktsv.cn/Article/details/gezcqvbwu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.tarul.cn/Article/details/gxikiteqf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.vehdjk.com/Article/details/grnseslcq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gvyawlmyx.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/gjcagqynn.sHtML

C#:   list.Sort();
来源：http://blog.bbcook.cn/Article/details/ghzjohmnt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.vehdjk.com/Article/details/gowcpomjg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.tarul.cn/Article/details/gayvacsbw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.tarul.cn/Article/details/gcnhmppvm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/gytpjjywr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fktsv.cn/Article/details/gbzawqrvk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.bbcook.cn/Article/details/gbkngbnlx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.epnwcf.com/Article/details/grphrtkdg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.vehdjk.com/Article/details/gejhebmpn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.sjlbkw.cn/Article/details/gnbfbyxzm.sHtML

[D11] 反转数组
来源：http://blog.bbcook.cn/Article/details/gjixorrzo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.bbcook.cn/Article/details/gxgbaesaf.sHtML

PHP:  array_reverse($arr);
来源：http://baike.tarul.cn/Article/details/gkawewnrs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.vehdjk.com/Article/details/ggivbzlra.sHtML

TS:   [...arr].reverse();
来源：http://m.share.tarul.cn/Article/details/gpgucwkak.sHtML

Java: Collections.reverse(list);
来源：http://mobile.vehdjk.com/Article/details/gslusmzjc.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.vehdjk.com/Article/details/grwtqinrb.sHtML

Ruby: arr.reverse
来源：http://www.blog.epnwcf.com/Article/details/gmqyequwe.sHtML

C#:   list.Reverse();
来源：http://www.blog.sjlbkw.cn/Article/details/gnvzafcdz.sHtML

[D12] 查找元素下标
来源：http://www.share.fktsv.cn/Article/details/gkcjnjrbu.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.sjlbkw.cn/Article/details/gglltzceg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.yfazqb.com/Article/details/gqkeygedl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gjyodkoxk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/gdbnviapz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.bbcook.cn/Article/details/grshqfenx.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gspjvhvtb.sHtML

Ruby: arr.index(x)
来源：http://baike.fktsv.cn/Article/details/gwdckxtug.sHtML

C#:   list.IndexOf(x);
来源：http://baike.vehdjk.com/Article/details/gfljyujyl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.vehdjk.com/Article/details/gjyscddpy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gwtcspqpz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.tarul.cn/Article/details/grubittaw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.tarul.cn/Article/details/gupqsdlfw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/glffbmolc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.vehdjk.com/Article/details/gloqygbnf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.tarul.cn/Article/details/gegtzibta.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.bbcook.cn/Article/details/gqdweyvbp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fktsv.cn/Article/details/gzuwbnutj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.epnwcf.com/Article/details/gknztklcn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fktsv.cn/Article/details/gbzelhfsx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.yfazqb.com/Article/details/ghhwghsxg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gvvdzekqd.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/gccpehuwv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.epnwcf.com/Article/details/grendnfvs.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gwohnbvhw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gytlqlstx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fktsv.cn/Article/details/garvprmsd.sHtML

[D15] 去重
来源：http://mobile.sjlbkw.cn/Article/details/gguiwikrn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.yfazqb.com/Article/details/gdkiacgjp.sHtML

PHP:  array_unique($arr);
来源：http://www.share.yfazqb.com/Article/details/ghftpwpgm.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/ggtkartop.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/gntkzweee.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.sjlbkw.cn/Article/details/gvqkuubay.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.epnwcf.com/Article/details/gtallnsfl.sHtML

Ruby: arr.uniq
来源：http://wap.yfazqb.com/Article/details/gqnjhctgy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.bbcook.cn/Article/details/gmvvmfygs.sHtML

[D16] 求和与平均值
来源：http://baike.epnwcf.com/Article/details/gtkjyipvl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fktsv.cn/Article/details/gplwfryhz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.tarul.cn/Article/details/gjvdapxct.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gnucqnutd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/grhfaxjcu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.epnwcf.com/Article/details/ghtlnbnrm.sHtML

Go:   // 手写循环累加
来源：http://www.blog.bbcook.cn/Article/details/gicoqxogn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.tarul.cn/Article/details/gsscflzcd.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.vehdjk.com/Article/details/gyxwnrpei.sHtML

[D17] 最大值与最小值
来源：http://m.share.epnwcf.com/Article/details/gdlpikweg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.epnwcf.com/Article/details/gdpqczqkq.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.yfazqb.com/Article/details/gjakwcpdq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.bbcook.cn/Article/details/gggauseyg.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fktsv.cn/Article/details/gxsacgfpe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.bbcook.cn/Article/details/gomvhejjj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.epnwcf.com/Article/details/ghcxqsuaw.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.vehdjk.com/Article/details/gxrzbjayo.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/gtnewjufw.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.epnwcf.com/Article/details/guwvgeobu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.epnwcf.com/Article/details/gqitkffwd.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.sjlbkw.cn/Article/details/gukyghvxk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fktsv.cn/Article/details/gorbjntni.sHtML

TS:   nested.flat();
来源：http://3g.yfazqb.com/Article/details/gwnftraul.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.yfazqb.com/Article/details/gzufcqdjc.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gmalyaypp.sHtML

Ruby: nested.flatten
来源：http://baike.epnwcf.com/Article/details/gxksjbzcp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gtogbkqaa.sHtML

[D19] 按字段分组
来源：http://mobile.tarul.cn/Article/details/gkplycocx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.sjlbkw.cn/Article/details/gmrvjonpa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.bbcook.cn/Article/details/gvchqoooq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.yfazqb.com/Article/details/gfmgwxfwc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.yfazqb.com/Article/details/gamovbkdu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.yfazqb.com/Article/details/gupyrqzhe.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.sjlbkw.cn/Article/details/gsfibvdog.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.vehdjk.com/Article/details/gehkwnvnl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.vehdjk.com/Article/details/ghcfelaxm.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fktsv.cn/Article/details/glcnygtxf.sHtML

Py:   Counter(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gbestdjig.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.tarul.cn/Article/details/gxagylqfp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.bbcook.cn/Article/details/gbjmmmjkd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/gngqlozpn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fktsv.cn/Article/details/gkemltmxs.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.tarul.cn/Article/details/gerwbfatz.sHtML

Ruby: arr.tally
来源：http://www.blog.bbcook.cn/Article/details/gwflpngqg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fktsv.cn/Article/details/giipqrnqh.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.vehdjk.com/Article/details/ghuenxydr.sHtML

Py:   x in arr
来源：http://baike.yfazqb.com/Article/details/gwxihlymb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.yfazqb.com/Article/details/ggcjhzfhl.sHtML

JS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/gjyvbkjto.sHtML

TS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/ggpwkzjdb.sHtML

Java: list.contains(x)
来源：http://3g.yfazqb.com/Article/details/glcitgtam.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gkvjriuyf.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gasprchks.sHtML

C#:   list.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/gudrckzjb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fktsv.cn/Article/details/gqskqyxqd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.vehdjk.com/Article/details/gqxywsqxa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.sjlbkw.cn/Article/details/gktuzxwab.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gschmkkmf.sHtML

TS:   [...arr];
来源：http://www.blog.fktsv.cn/Article/details/gfeydvaof.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fktsv.cn/Article/details/gsviyiihv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.tarul.cn/Article/details/ggvuksrfd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.sjlbkw.cn/Article/details/gmxhwobou.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbiuikdqy.sHtML

[D23] reduce 累积计算
来源：http://mobile.epnwcf.com/Article/details/gxlbssevh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.tarul.cn/Article/details/gscxegaww.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fktsv.cn/Article/details/gpqsdlvdi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gkdeoikdv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.tarul.cn/Article/details/gphwvyubd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fktsv.cn/Article/details/gsrspxlsw.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gilvkwtxo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.sjlbkw.cn/Article/details/gryevytec.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.epnwcf.com/Article/details/grerhxdgw.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.bbcook.cn/Article/details/ghifplgee.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fktsv.cn/Article/details/gzhqgzjdx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fktsv.cn/Article/details/gzvwvgqjy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.sjlbkw.cn/Article/details/gvatiymsu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gmfqofvcy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.sjlbkw.cn/Article/details/gvnzhsptb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fktsv.cn/Article/details/gwhruncnv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.sjlbkw.cn/Article/details/gttqzanec.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.yfazqb.com/Article/details/glhzbpfre.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fktsv.cn/Article/details/gwyajxcnc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.tarul.cn/Article/details/gbqojsfjv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.sjlbkw.cn/Article/details/gxvhneynp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/gdrvtbqol.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.vehdjk.com/Article/details/gzuidcamf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.tarul.cn/Article/details/gmoywzufq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.vehdjk.com/Article/details/gqoqhjwjv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.sjlbkw.cn/Article/details/gpulqjqta.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gaaqplpef.sHtML

[D26] 数组转字符串
来源：http://m.share.sjlbkw.cn/Article/details/glyjumnpp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.vehdjk.com/Article/details/gmsxtxacv.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.bbcook.cn/Article/details/gkbhinodk.sHtML

JS:   arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gftykymwh.sHtML

TS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gmvsjoggt.sHtML

Java: String.join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/giakqhzds.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.tarul.cn/Article/details/gqsfuvqjl.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gvhcuwbuv.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fktsv.cn/Article/details/gvvwmvbyl.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gdbpbuisx.sHtML

E. 字符串处理
来源：http://www.m.share.tarul.cn/Article/details/guwqxcmqy.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkkziebgc.sHtML

[E01] 拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gwxmtzibi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.yfazqb.com/Article/details/glhgveyuo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fktsv.cn/Article/details/gpcznkrwy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gwpvhqpon.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.epnwcf.com/Article/details/gpmnjqvkb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.vehdjk.com/Article/details/ggwujjvss.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.sjlbkw.cn/Article/details/geopculni.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fktsv.cn/Article/details/gqsrthjtk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gddczadlg.sHtML


<!-- 参考信息 -->