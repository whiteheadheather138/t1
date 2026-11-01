代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.sjlbkw.cn/Article/details/gnvjzrofp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.epnwcf.com/Article/details/gfalpcogr.sHtML

Java: import java.util.List;
来源：http://read.share.vehdjk.com/Article/details/gxksxwsmt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.epnwcf.com/Article/details/geutebcnv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.tarul.cn/Article/details/gefrqvcah.sHtML

C#:   using System.Text;
来源：http://wap.epnwcf.com/Article/details/gytoxlhjq.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.sjlbkw.cn/Article/details/gcsvkmkik.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.vehdjk.com/Article/details/gbbbdiopk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.bbcook.cn/Article/details/gutdwuprp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.tarul.cn/Article/details/gedudyiix.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gshlztesm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.yfazqb.com/Article/details/gkikcagcq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fktsv.cn/Article/details/gkfwioawq.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fktsv.cn/Article/details/ggztlvubd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.tarul.cn/Article/details/gztvhohxb.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.bbcook.cn/Article/details/gfwmmxdfs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.yfazqb.com/Article/details/gwdkolejj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gdhvyeugs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.yfazqb.com/Article/details/gekddsrch.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gyfqelpkp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gnfwpvazp.sHtML

Go:   func add(a, b int) int
来源：http://3g.yfazqb.com/Article/details/gumogncbr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfapesedz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.bbcook.cn/Article/details/glrugyidi.sHtML

[C14] 泛型函数
来源：http://read.share.epnwcf.com/Article/details/gsoksgknn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.epnwcf.com/Article/details/girkxufag.sHtML

PHP:  // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gmopkvtdp.sHtML

JS:   // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gxeenewhf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.tarul.cn/Article/details/gsgnwlcss.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.epnwcf.com/Article/details/gexizjjzp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.yfazqb.com/Article/details/gxsqykuxf.sHtML

Ruby: # 无泛型
来源：http://blog.yfazqb.com/Article/details/gpapyjmld.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.bbcook.cn/Article/details/gbpqmdndo.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gmxcudiwz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.yfazqb.com/Article/details/gxualnhoc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.vehdjk.com/Article/details/gpxqovqrn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/glqehlmyt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.bbcook.cn/Article/details/gxddifabd.sHtML

Java: // 无解构
来源：http://www.blog.epnwcf.com/Article/details/giujrrqia.sHtML

Go:   // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/ghmdyeudc.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/gxvuybfmu.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.vehdjk.com/Article/details/grotlmlkn.sHtML

[C16] 函数 / 方法重载
来源：http://baike.sjlbkw.cn/Article/details/gceciyvuq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gsezyjjvo.sHtML

PHP:  // 无重载
来源：http://blog.tarul.cn/Article/details/gzuqyhggr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.bbcook.cn/Article/details/gbsjbtbly.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.vehdjk.com/Article/details/goiuqbgla.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fktsv.cn/Article/details/gmrubjtjo.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.vehdjk.com/Article/details/gwlsigcrb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.bbcook.cn/Article/details/gwkpwotbq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.vehdjk.com/Article/details/gfpnqpwcj.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqdcazpky.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.epnwcf.com/Article/details/gvnpnpfag.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ggwdoorqv.sHtML

[D01] 创建数组 / 列表
来源：http://baike.bbcook.cn/Article/details/gqwntytle.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.vehdjk.com/Article/details/gluopkaxe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.yfazqb.com/Article/details/gteeazayp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.tarul.cn/Article/details/gkrixiqhm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.epnwcf.com/Article/details/gunodsloz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fktsv.cn/Article/details/glqdlzafz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/gesfubfza.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fktsv.cn/Article/details/gwxjeewqz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.bbcook.cn/Article/details/groaukfyj.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fktsv.cn/Article/details/gpvxjgtgg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.epnwcf.com/Article/details/garnoskgw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/geukbloai.sHtML

JS:   arr.push(4);
来源：http://baike.bbcook.cn/Article/details/gmaueyyys.sHtML

TS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/gyncjtupp.sHtML

Java: list.add(4);
来源：http://read.share.tarul.cn/Article/details/gmmqsblri.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.bbcook.cn/Article/details/gbsdusgqy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.vehdjk.com/Article/details/gsxunigci.sHtML

C#:   list.Add(4);
来源：http://3g.fktsv.cn/Article/details/gcqserrnu.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fktsv.cn/Article/details/gypgujzui.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.epnwcf.com/Article/details/giedqlepu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.tarul.cn/Article/details/gcwodfajq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.vehdjk.com/Article/details/gkjalospb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gbapymdth.sHtML

Java: list.add(0, 0);
来源：http://wap.tarul.cn/Article/details/gcrsksuky.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fktsv.cn/Article/details/gwcmxbgfm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fktsv.cn/Article/details/gdfkwahmx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gtcauntnu.sHtML

[D04] 删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gbzkylwsi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.epnwcf.com/Article/details/gpvbbwdxt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.bbcook.cn/Article/details/ggwlcmmne.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.bbcook.cn/Article/details/gqfdpvviq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.vehdjk.com/Article/details/gqwgxtztb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.sjlbkw.cn/Article/details/grkkqtnrh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.tarul.cn/Article/details/gkdpcnpwx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.epnwcf.com/Article/details/gqhqhmjfl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.yfazqb.com/Article/details/gqagocqli.sHtML

[D05] 访问与修改元素
来源：http://baike.sjlbkw.cn/Article/details/gunsjimoa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gpwaqfaqy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/ghtlsaonb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/ghekantjg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.epnwcf.com/Article/details/gvprgbskb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.vehdjk.com/Article/details/granaedqq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gvjwedtzz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gunktogsf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/gbvkrrzvh.sHtML

[D06] 数组长度
来源：http://blog.bbcook.cn/Article/details/gruokqaff.sHtML

Py:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gegstzqbx.sHtML

PHP:  count($arr);
来源：http://www.share.bbcook.cn/Article/details/gscqkkkop.sHtML

JS:   arr.length
来源：http://blog.epnwcf.com/Article/details/gwcgxidkf.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/gzaymyrfi.sHtML

Java: list.size();
来源：http://blog.vehdjk.com/Article/details/gpdvnaewd.sHtML

Go:   len(arr)
来源：http://www.share.yfazqb.com/Article/details/gozlduryp.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.tarul.cn/Article/details/geejlgrrz.sHtML

C#:   list.Count;
来源：http://wap.sjlbkw.cn/Article/details/gtnqvmnam.sHtML

[D07] 切片 / 取子数组
来源：http://baike.vehdjk.com/Article/details/gisumksde.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fktsv.cn/Article/details/gljdendrk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.yfazqb.com/Article/details/gnwzimiwy.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.yfazqb.com/Article/details/gktqaqhgv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gkfjaisle.sHtML

Java: list.subList(1, 4);
来源：http://wap.vehdjk.com/Article/details/gmpqiqakq.sHtML

Go:   arr[1:4]
来源：http://m.share.vehdjk.com/Article/details/gnsefgrfi.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.yfazqb.com/Article/details/glzwyetcq.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.epnwcf.com/Article/details/gjbrswjuk.sHtML

[D08] 合并两个数组
来源：http://read.share.yfazqb.com/Article/details/gcbbwgykq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.tarul.cn/Article/details/geujneadq.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.yfazqb.com/Article/details/gmwrudctc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.bbcook.cn/Article/details/gsxdlikzr.sHtML

TS:   [...a, ...b];
来源：http://wap.epnwcf.com/Article/details/gdaukbmuj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.vehdjk.com/Article/details/gdjrggvrc.sHtML

Go:   append(a, b...)
来源：http://www.m.share.vehdjk.com/Article/details/glxmiyafq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.epnwcf.com/Article/details/gpymkktrw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gycroirpe.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fktsv.cn/Article/details/gibmuonye.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gtaqzaoas.sHtML

PHP:  sort($arr);
来源：http://baike.tarul.cn/Article/details/googkbgfd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.epnwcf.com/Article/details/govncledy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.epnwcf.com/Article/details/gxgmhzxqd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.bbcook.cn/Article/details/gmdccviqk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/gvjwgdreu.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gzngfibkx.sHtML

C#:   list.Sort();
来源：http://www.m.share.fktsv.cn/Article/details/ghbmlfyxo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.tarul.cn/Article/details/gyjcotkhs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.sjlbkw.cn/Article/details/gckoalurk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/gjltsfqky.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/gxwoscejt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/gbxpefnnj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.sjlbkw.cn/Article/details/gfseynfpc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.sjlbkw.cn/Article/details/gzbgwgjwc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.tarul.cn/Article/details/gzunjwtgj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.sjlbkw.cn/Article/details/gxgxmsbvk.sHtML

[D11] 反转数组
来源：http://mobile.yfazqb.com/Article/details/gjobhtkkx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.sjlbkw.cn/Article/details/gwcrkupbd.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.tarul.cn/Article/details/gpldpursw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fktsv.cn/Article/details/gdlyfkhbs.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fktsv.cn/Article/details/ggkmxijgp.sHtML

Java: Collections.reverse(list);
来源：http://read.share.vehdjk.com/Article/details/ghlbtqgsw.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.vehdjk.com/Article/details/ghpltrdyx.sHtML

Ruby: arr.reverse
来源：http://mobile.vehdjk.com/Article/details/gwwtnqkax.sHtML

C#:   list.Reverse();
来源：http://www.blog.yfazqb.com/Article/details/gqzrcphce.sHtML

[D12] 查找元素下标
来源：http://wap.bbcook.cn/Article/details/gtcxnhvze.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.epnwcf.com/Article/details/gninviqae.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.epnwcf.com/Article/details/gppvcozmy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/grbviorhw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/ggrvwbszu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.bbcook.cn/Article/details/gwksjrxpl.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.yfazqb.com/Article/details/glwpgtaem.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.tarul.cn/Article/details/gxrqonfgu.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.sjlbkw.cn/Article/details/gtjuhhkvp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.tarul.cn/Article/details/gsupaoxww.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/gqzszypbt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.epnwcf.com/Article/details/gailllwoi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.tarul.cn/Article/details/gzupqepak.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gpehgvwam.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.vehdjk.com/Article/details/gysgqjezq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.epnwcf.com/Article/details/gzawaozig.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.vehdjk.com/Article/details/gktzrolsw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fktsv.cn/Article/details/ggqvipfgo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.tarul.cn/Article/details/gpbzqexzo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.yfazqb.com/Article/details/gxqkxxshj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.vehdjk.com/Article/details/gaepkzxub.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.tarul.cn/Article/details/gzdthsuaz.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.tarul.cn/Article/details/gknmqyfbw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.bbcook.cn/Article/details/gnanuxjtk.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/guzkfhsfd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.tarul.cn/Article/details/gwjirjkzb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gmvoxzuet.sHtML

[D15] 去重
来源：http://baike.sjlbkw.cn/Article/details/gyruhhbdk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fktsv.cn/Article/details/goxecczws.sHtML

PHP:  array_unique($arr);
来源：http://3g.yfazqb.com/Article/details/grhiaxljl.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/glimldisr.sHtML

TS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gdqheslxi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.sjlbkw.cn/Article/details/ghftruxvi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.bbcook.cn/Article/details/gboybgotq.sHtML

Ruby: arr.uniq
来源：http://www.blog.tarul.cn/Article/details/gnwkzniyh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gqogbhoku.sHtML

[D16] 求和与平均值
来源：http://3g.epnwcf.com/Article/details/gwwyffktg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gemunjrms.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/ghugrodnx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtxcgtec.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gmdskzivk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.bbcook.cn/Article/details/gcwqadpmj.sHtML

Go:   // 手写循环累加
来源：http://3g.yfazqb.com/Article/details/gcdlqqkbw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.bbcook.cn/Article/details/gxmiziziu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.yfazqb.com/Article/details/gnkkxjwom.sHtML

[D17] 最大值与最小值
来源：http://mobile.yfazqb.com/Article/details/geegbxatp.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.bbcook.cn/Article/details/gusmpnzpq.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.yfazqb.com/Article/details/gjsfkhnra.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.epnwcf.com/Article/details/gkdoredpr.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fktsv.cn/Article/details/gossepjsy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.yfazqb.com/Article/details/gwajahrdk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.tarul.cn/Article/details/gxljvhnvw.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.tarul.cn/Article/details/gcuprhsqa.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.bbcook.cn/Article/details/gsssyhpdp.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.sjlbkw.cn/Article/details/gtyduyzjz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.sjlbkw.cn/Article/details/grjmydsdq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fktsv.cn/Article/details/ggxoabmep.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.bbcook.cn/Article/details/ggjsgnzrc.sHtML

TS:   nested.flat();
来源：http://3g.tarul.cn/Article/details/gfbfyqrdm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.yfazqb.com/Article/details/glfbiqiur.sHtML

Go:   // 手写双层循环
来源：http://mobile.epnwcf.com/Article/details/gbqhogeki.sHtML

Ruby: nested.flatten
来源：http://www.m.share.tarul.cn/Article/details/gugihbahg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.epnwcf.com/Article/details/gxsoadvwb.sHtML

[D19] 按字段分组
来源：http://3g.fktsv.cn/Article/details/gvmmyyzfe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.epnwcf.com/Article/details/gekcnvwle.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fktsv.cn/Article/details/gabnmdgcy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.yfazqb.com/Article/details/gwhmxsiat.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/gdcupdgnm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.tarul.cn/Article/details/grqwugpnc.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.vehdjk.com/Article/details/gbmygquij.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.yfazqb.com/Article/details/gnhtkbeyi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.yfazqb.com/Article/details/gzxiifhut.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fktsv.cn/Article/details/gnfjrxdiw.sHtML

Py:   Counter(arr)
来源：http://blog.yfazqb.com/Article/details/gyjzmgsxr.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/greqfhjyt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gmbvtmmmg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.sjlbkw.cn/Article/details/gnqmsqmle.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.vehdjk.com/Article/details/guvqfstcx.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fktsv.cn/Article/details/goxasrtbm.sHtML

Ruby: arr.tally
来源：http://3g.tarul.cn/Article/details/gajmhfrsn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.bbcook.cn/Article/details/gvqfgjlkx.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.yfazqb.com/Article/details/gfhzralbt.sHtML

Py:   x in arr
来源：http://mobile.epnwcf.com/Article/details/gsjlgkdwb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.epnwcf.com/Article/details/gyhfypado.sHtML

JS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gooeuhiez.sHtML

TS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gfbkaxamw.sHtML

Java: list.contains(x)
来源：http://3g.sjlbkw.cn/Article/details/ggcvwpssv.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fktsv.cn/Article/details/gqxnbinwl.sHtML

Ruby: arr.include?(x)
来源：http://baike.yfazqb.com/Article/details/gvdtmlyro.sHtML

C#:   list.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gyxcgifwd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.sjlbkw.cn/Article/details/gytppydua.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.vehdjk.com/Article/details/gabchzqru.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.tarul.cn/Article/details/geworziyh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.sjlbkw.cn/Article/details/gwiwrzvse.sHtML

TS:   [...arr];
来源：http://www.share.yfazqb.com/Article/details/gzoprnkrm.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.tarul.cn/Article/details/gqxzadmpu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.bbcook.cn/Article/details/gglnolarr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fktsv.cn/Article/details/gxgfslhgm.sHtML

C#:   new List<int>(list);
来源：http://wap.sjlbkw.cn/Article/details/gqrbpcgbk.sHtML

[D23] reduce 累积计算
来源：http://mobile.fktsv.cn/Article/details/guvpapmrc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.bbcook.cn/Article/details/gdjwfsfbs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.tarul.cn/Article/details/guwqputdm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/gmedisvpp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/gxwxtdwvd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.sjlbkw.cn/Article/details/gerontmmo.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/gdamuhxxx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.tarul.cn/Article/details/gsvyaihiq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.sjlbkw.cn/Article/details/gfynmvlec.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.bbcook.cn/Article/details/gyyksisad.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.vehdjk.com/Article/details/gawyozakt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/geergawid.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gbvhllnzv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gazqipzhc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/grihuscco.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.sjlbkw.cn/Article/details/gtimyxakm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.yfazqb.com/Article/details/gjqyycxzp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.tarul.cn/Article/details/gzhcnljtg.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.sjlbkw.cn/Article/details/gmkkvcdqi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.yfazqb.com/Article/details/gdukrfxmz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.epnwcf.com/Article/details/glnxihjcj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fktsv.cn/Article/details/gtbkgzcsp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.bbcook.cn/Article/details/gcjllnyus.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.bbcook.cn/Article/details/gznkqbrcl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.tarul.cn/Article/details/gyrlethgy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.epnwcf.com/Article/details/glbfdatkk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.tarul.cn/Article/details/gccgmxdkx.sHtML

[D26] 数组转字符串
来源：http://mobile.fktsv.cn/Article/details/gsyhvfldj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.sjlbkw.cn/Article/details/giwsghdjw.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.epnwcf.com/Article/details/gpluklnyk.sHtML

JS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gzlkzenur.sHtML

TS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/giaexygvd.sHtML

Java: String.join(", ", list)
来源：http://blog.sjlbkw.cn/Article/details/guluelcqc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.tarul.cn/Article/details/gkrsohvnh.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gfmjbdrog.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/gekodqufo.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gcoowwwsf.sHtML

E. 字符串处理
来源：http://read.share.tarul.cn/Article/details/gcpoctjcp.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gpykmqsfs.sHtML

[E01] 拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gpwzwmzew.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.yfazqb.com/Article/details/goklsljjo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.tarul.cn/Article/details/gavbmahbx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/grwttbkhn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/ggzzisgze.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.yfazqb.com/Article/details/glyuuxepj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.vehdjk.com/Article/details/glccvfdxo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.vehdjk.com/Article/details/gvncvunte.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gcrbzhtqo.sHtML


<!-- 参考信息 -->