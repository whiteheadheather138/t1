代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.tarul.cn/Article/details/ggplmliyu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.vehdjk.com/Article/details/gcclcaixt.sHtML

Java: import java.util.List;
来源：http://3g.fktsv.cn/Article/details/ghpckvkes.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.tarul.cn/Article/details/gjejbcfih.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.yfazqb.com/Article/details/glbevnrsn.sHtML

C#:   using System.Text;
来源：http://www.blog.bbcook.cn/Article/details/gpwkccfzf.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.sjlbkw.cn/Article/details/ggkujvcnl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.epnwcf.com/Article/details/gxduuasfc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.bbcook.cn/Article/details/gxhtyzzfe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.yfazqb.com/Article/details/gprtmgpnw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/guvqotxow.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.tarul.cn/Article/details/gfqjiradz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.epnwcf.com/Article/details/glucmzdyw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.yfazqb.com/Article/details/gplqgrpkj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fktsv.cn/Article/details/grhqlujkh.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.tarul.cn/Article/details/ghcqlpjpp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.yfazqb.com/Article/details/gzxxzvcpe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gbfmelgdn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fktsv.cn/Article/details/gzjemqxnv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gteothfbk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gubfmrtqw.sHtML

Go:   func add(a, b int) int
来源：http://mobile.sjlbkw.cn/Article/details/gcpfxedbh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/gtdvhjoha.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fktsv.cn/Article/details/getowzqbv.sHtML

[C14] 泛型函数
来源：http://3g.tarul.cn/Article/details/ghncjsgvf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.yfazqb.com/Article/details/geofpoiby.sHtML

PHP:  // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gyrioefkn.sHtML

JS:   // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gcujfunbc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.vehdjk.com/Article/details/gpofvzenm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.epnwcf.com/Article/details/ghirwsehc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.epnwcf.com/Article/details/gqktaaitf.sHtML

Ruby: # 无泛型
来源：http://read.share.bbcook.cn/Article/details/gmufvlggj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.tarul.cn/Article/details/gkinkziku.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.sjlbkw.cn/Article/details/gdpkbflge.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.bbcook.cn/Article/details/govnezxbw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.epnwcf.com/Article/details/gdwypawvo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gzxdjqgdr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fktsv.cn/Article/details/gricrtngu.sHtML

Java: // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/gmqtvxwsj.sHtML

Go:   // 无解构
来源：http://3g.fktsv.cn/Article/details/gyzxkskdd.sHtML

Ruby: a, b = pair
来源：http://www.blog.yfazqb.com/Article/details/ghuisinbq.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.bbcook.cn/Article/details/gvjgnieuw.sHtML

[C16] 函数 / 方法重载
来源：http://blog.vehdjk.com/Article/details/galvcasgc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.yfazqb.com/Article/details/gbnkkkggz.sHtML

PHP:  // 无重载
来源：http://m.share.tarul.cn/Article/details/gwzcdryba.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.tarul.cn/Article/details/gpnsyemun.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.bbcook.cn/Article/details/gccdhcsbt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.sjlbkw.cn/Article/details/gqzaowvdy.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.yfazqb.com/Article/details/gjpzxcrya.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.sjlbkw.cn/Article/details/ggyywkegg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.vehdjk.com/Article/details/gvywzcaob.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gdjuogtiq.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.yfazqb.com/Article/details/gftqjvzjx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbqswmyng.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.tarul.cn/Article/details/gxxvhbiwy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.bbcook.cn/Article/details/gyeebvesj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gdltbcotx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gupzxufzd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.bbcook.cn/Article/details/gglbkpffi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.epnwcf.com/Article/details/gamuvipju.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.yfazqb.com/Article/details/gbjpdjhji.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.tarul.cn/Article/details/gucvzqccn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.tarul.cn/Article/details/gejuaaohp.sHtML

[D02] 追加元素到末尾
来源：http://m.share.vehdjk.com/Article/details/gvqbeexss.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.bbcook.cn/Article/details/gwuobtjfh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.tarul.cn/Article/details/gpntkjkhd.sHtML

JS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gmjivoyha.sHtML

TS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/ghqkhfoyp.sHtML

Java: list.add(4);
来源：http://www.m.share.tarul.cn/Article/details/gxzjtfjsg.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.vehdjk.com/Article/details/girdrvzdm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.yfazqb.com/Article/details/gpazejopk.sHtML

C#:   list.Add(4);
来源：http://read.share.tarul.cn/Article/details/gjlhipnll.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.yfazqb.com/Article/details/gadxqgpyn.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/gfydnasfr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.epnwcf.com/Article/details/gghpamupp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fktsv.cn/Article/details/gursojtap.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.yfazqb.com/Article/details/gnxgpmvnt.sHtML

Java: list.add(0, 0);
来源：http://wap.yfazqb.com/Article/details/gkinsdiuh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.vehdjk.com/Article/details/gxbwjuopq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.yfazqb.com/Article/details/gkoipwqwg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.vehdjk.com/Article/details/graldcqxo.sHtML

[D04] 删除元素
来源：http://read.share.yfazqb.com/Article/details/gfthwqjow.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.epnwcf.com/Article/details/gttqobbzm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gpxzstqms.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fktsv.cn/Article/details/gmyqfiecz.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.yfazqb.com/Article/details/gxmugikjy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.yfazqb.com/Article/details/gahktmapm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.tarul.cn/Article/details/gnijwrrfj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.bbcook.cn/Article/details/gbnvwamep.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.bbcook.cn/Article/details/gefrkojgp.sHtML

[D05] 访问与修改元素
来源：http://mobile.vehdjk.com/Article/details/gkuucymfj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gcuaaqqym.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gdfjwbzlz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gmrrdnnlv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fktsv.cn/Article/details/gdsueektq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.sjlbkw.cn/Article/details/gzdyszvin.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gjyfpkqvb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gjtuhwuwn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.tarul.cn/Article/details/gwsbpprsg.sHtML

[D06] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnpltost.sHtML

Py:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gbzaupekj.sHtML

PHP:  count($arr);
来源：http://wap.fktsv.cn/Article/details/gimblkyhd.sHtML

JS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/ggnxqrfkv.sHtML

TS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/grcbbungi.sHtML

Java: list.size();
来源：http://baike.sjlbkw.cn/Article/details/gbmcdecrc.sHtML

Go:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/giouktzcz.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.vehdjk.com/Article/details/gfzxtbuin.sHtML

C#:   list.Count;
来源：http://m.share.yfazqb.com/Article/details/gampizzvp.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.epnwcf.com/Article/details/gnuipprlv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.bbcook.cn/Article/details/gjeejqrpv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.tarul.cn/Article/details/gjvqunwws.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gtxxejocb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gmnooaqrz.sHtML

Java: list.subList(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gjxycghll.sHtML

Go:   arr[1:4]
来源：http://read.share.epnwcf.com/Article/details/gkcbxjykd.sHtML

Ruby: arr[1, 3]
来源：http://wap.tarul.cn/Article/details/gfmfwhnjc.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.tarul.cn/Article/details/gnqzkvyaf.sHtML

[D08] 合并两个数组
来源：http://www.share.bbcook.cn/Article/details/gcjiofijm.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.tarul.cn/Article/details/gtjtrzifq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.epnwcf.com/Article/details/gmqiebeiy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fktsv.cn/Article/details/grvazezca.sHtML

TS:   [...a, ...b];
来源：http://wap.fktsv.cn/Article/details/gdyogqivr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.yfazqb.com/Article/details/gxmxmukoa.sHtML

Go:   append(a, b...)
来源：http://3g.bbcook.cn/Article/details/gdjoscivk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.epnwcf.com/Article/details/gnnmsyuig.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.bbcook.cn/Article/details/gzkburzxf.sHtML

[D09] 排序（升序）
来源：http://read.share.yfazqb.com/Article/details/gpwvgmlvs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gltzrbnqb.sHtML

PHP:  sort($arr);
来源：http://www.blog.epnwcf.com/Article/details/ghxqllqdr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.sjlbkw.cn/Article/details/glfyplshn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.yfazqb.com/Article/details/gurlnplom.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.tarul.cn/Article/details/gencudskw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gjwumgbon.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/ghohxqxuw.sHtML

C#:   list.Sort();
来源：http://blog.fktsv.cn/Article/details/gjivfpgxj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.bbcook.cn/Article/details/gztyytmul.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.vehdjk.com/Article/details/gwyculbbq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.epnwcf.com/Article/details/goebnjvmi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gtbdjqfhy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fktsv.cn/Article/details/gnaswuidk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.epnwcf.com/Article/details/ggtpynwgg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.sjlbkw.cn/Article/details/gajswempl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.sjlbkw.cn/Article/details/grgrjjztq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.yfazqb.com/Article/details/gonfmxdjq.sHtML

[D11] 反转数组
来源：http://blog.fktsv.cn/Article/details/gquakmpgx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.vehdjk.com/Article/details/gladiqmqc.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.tarul.cn/Article/details/gvnbcdwea.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.epnwcf.com/Article/details/guzridqzx.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.sjlbkw.cn/Article/details/geosnbgtu.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/gnufcplcp.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fktsv.cn/Article/details/gtwegrjrt.sHtML

Ruby: arr.reverse
来源：http://mobile.bbcook.cn/Article/details/gvakupayd.sHtML

C#:   list.Reverse();
来源：http://wap.epnwcf.com/Article/details/gjjbzprbf.sHtML

[D12] 查找元素下标
来源：http://www.blog.tarul.cn/Article/details/gucsupsvn.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fktsv.cn/Article/details/gimdgjhwe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/geculmpfw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gztabtoss.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.epnwcf.com/Article/details/gescyzmwo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.sjlbkw.cn/Article/details/ghieahrgp.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.bbcook.cn/Article/details/ggwfulyij.sHtML

Ruby: arr.index(x)
来源：http://m.share.vehdjk.com/Article/details/gvjbtndhl.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.sjlbkw.cn/Article/details/getxdrxcy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.bbcook.cn/Article/details/gbmpoosum.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.epnwcf.com/Article/details/gitefrchl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.tarul.cn/Article/details/gwioswpna.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fktsv.cn/Article/details/gtjdwmblo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gutmhiobj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.epnwcf.com/Article/details/gyinzyuop.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.epnwcf.com/Article/details/gmjvzsigw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.bbcook.cn/Article/details/gsytioesp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gjvzakshy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.tarul.cn/Article/details/gmlrifadi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fktsv.cn/Article/details/gcxbcdzeb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.tarul.cn/Article/details/gspkkfsgi.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fktsv.cn/Article/details/gityenwdr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/gwviipvpv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.tarul.cn/Article/details/gcaymqlyb.sHtML

Go:   // 手写循环
来源：http://www.m.share.vehdjk.com/Article/details/gmolkzzyp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gehjtlwez.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.tarul.cn/Article/details/gdsngwpep.sHtML

[D15] 去重
来源：http://blog.tarul.cn/Article/details/gmnvhuvcv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.bbcook.cn/Article/details/gdpozsqxa.sHtML

PHP:  array_unique($arr);
来源：http://baike.fktsv.cn/Article/details/gtfodcvhv.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gcttduemj.sHtML

TS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gbvlsikcb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.yfazqb.com/Article/details/gbtjgedxr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.sjlbkw.cn/Article/details/goijjlglv.sHtML

Ruby: arr.uniq
来源：http://3g.bbcook.cn/Article/details/gwvexylwu.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.tarul.cn/Article/details/giasbvgfd.sHtML

[D16] 求和与平均值
来源：http://www.blog.vehdjk.com/Article/details/gbfcbfdpe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fktsv.cn/Article/details/ghvzwcbbd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.vehdjk.com/Article/details/gnnxdrrks.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.tarul.cn/Article/details/gbblidhaa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/gpapaekzt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.yfazqb.com/Article/details/gdnrqewvi.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.bbcook.cn/Article/details/grajwbbpi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.epnwcf.com/Article/details/gxdcpnosk.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.yfazqb.com/Article/details/gpdwbsocd.sHtML

[D17] 最大值与最小值
来源：http://baike.sjlbkw.cn/Article/details/gvtuzfjog.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gnvbhbcpy.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.epnwcf.com/Article/details/ghuzumvml.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.yfazqb.com/Article/details/ggaurtlfy.sHtML

TS:   Math.max(...arr);
来源：http://3g.vehdjk.com/Article/details/gyvcfahdf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.bbcook.cn/Article/details/gxaqsfbfb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fktsv.cn/Article/details/gjavxvcyl.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.sjlbkw.cn/Article/details/gedosceam.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.sjlbkw.cn/Article/details/geegyfgoc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.epnwcf.com/Article/details/gzxaofxuv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.sjlbkw.cn/Article/details/gfygucfld.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.bbcook.cn/Article/details/gztlkpuxh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.yfazqb.com/Article/details/gofpoxoju.sHtML

TS:   nested.flat();
来源：http://www.m.share.vehdjk.com/Article/details/gjdcpyyae.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.yfazqb.com/Article/details/glkijlsfq.sHtML

Go:   // 手写双层循环
来源：http://baike.bbcook.cn/Article/details/gejbwqsqu.sHtML

Ruby: nested.flatten
来源：http://www.share.bbcook.cn/Article/details/gwcjjjkbb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gicanljno.sHtML

[D19] 按字段分组
来源：http://mobile.fktsv.cn/Article/details/gevfcdzlv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.tarul.cn/Article/details/gnqpzekyk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fktsv.cn/Article/details/ggejyprwq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.tarul.cn/Article/details/gslbalfnc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.epnwcf.com/Article/details/gcljyxutu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.vehdjk.com/Article/details/gqtmpsyyl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.sjlbkw.cn/Article/details/gpwabkujt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fktsv.cn/Article/details/gzwcamost.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.bbcook.cn/Article/details/gnrariydy.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.tarul.cn/Article/details/garlmteaf.sHtML

Py:   Counter(arr)
来源：http://3g.vehdjk.com/Article/details/grlbwkpcj.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gghjuzbde.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/gjqoewrqg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.bbcook.cn/Article/details/gfxfxrjch.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.tarul.cn/Article/details/glzmxpxhe.sHtML

Go:   // 手写 map[T]int
来源：http://3g.sjlbkw.cn/Article/details/govvaflrs.sHtML

Ruby: arr.tally
来源：http://www.share.vehdjk.com/Article/details/ghfkgklgk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.tarul.cn/Article/details/glvkuehxc.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.tarul.cn/Article/details/gnzbrzsgc.sHtML

Py:   x in arr
来源：http://baike.epnwcf.com/Article/details/gidzptrlj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.vehdjk.com/Article/details/glodrdpyq.sHtML

JS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gtrdmtzll.sHtML

TS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gaolpqwyv.sHtML

Java: list.contains(x)
来源：http://wap.epnwcf.com/Article/details/gecvbpihg.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gzjyffmku.sHtML

Ruby: arr.include?(x)
来源：http://baike.epnwcf.com/Article/details/gbqwhoqfj.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gpvikztjp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.yfazqb.com/Article/details/gvdabuhek.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.epnwcf.com/Article/details/gvotvjkaj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.bbcook.cn/Article/details/gibdcfkzq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/gjjqmsbyx.sHtML

TS:   [...arr];
来源：http://blog.sjlbkw.cn/Article/details/gncliprda.sHtML

Java: new ArrayList<>(list);
来源：http://3g.yfazqb.com/Article/details/gurlqvqcp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fktsv.cn/Article/details/ghfjpdugl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fktsv.cn/Article/details/gavnwxgnl.sHtML

C#:   new List<int>(list);
来源：http://mobile.bbcook.cn/Article/details/gjhscccms.sHtML

[D23] reduce 累积计算
来源：http://wap.epnwcf.com/Article/details/geevfgmkn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.sjlbkw.cn/Article/details/grhufdfxz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gmkyxsuek.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/gdnqwbaqs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/gxvflperw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.sjlbkw.cn/Article/details/gwagsmulm.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/giebrhvja.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.vehdjk.com/Article/details/ggyvunqbt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fktsv.cn/Article/details/gxnlbqygr.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.epnwcf.com/Article/details/gwdjeimmw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.vehdjk.com/Article/details/gcarbxlpa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.yfazqb.com/Article/details/gqwjdqnmt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.tarul.cn/Article/details/gdkphycqv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.tarul.cn/Article/details/gsbazcayf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.bbcook.cn/Article/details/gjrjqwzvv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.tarul.cn/Article/details/geqiyaktd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.tarul.cn/Article/details/gcwmwteyf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.vehdjk.com/Article/details/gzkrifpvl.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.vehdjk.com/Article/details/gepexrtxo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fktsv.cn/Article/details/ggjjcaqqd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.tarul.cn/Article/details/grdqzflch.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.sjlbkw.cn/Article/details/guytaanlf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.yfazqb.com/Article/details/gbmanhcwh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.yfazqb.com/Article/details/gntpckczs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gyscblvkh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.sjlbkw.cn/Article/details/gerhyxcfe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fktsv.cn/Article/details/gbacfxqyi.sHtML

[D26] 数组转字符串
来源：http://3g.tarul.cn/Article/details/gjqzjfxyy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.tarul.cn/Article/details/glncgkqfi.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.yfazqb.com/Article/details/gyqfdtqxi.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gjqgxyuqz.sHtML

TS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gqmgoeipb.sHtML

Java: String.join(", ", list)
来源：http://mobile.bbcook.cn/Article/details/gvkewqpvd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.sjlbkw.cn/Article/details/gcxajuycs.sHtML

Ruby: arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gweuwsywu.sHtML

C#:   string.Join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gercevmyh.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfzcyeqcf.sHtML

E. 字符串处理
来源：http://3g.bbcook.cn/Article/details/gttvqxswz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/grhpsffeo.sHtML

[E01] 拼接字符串
来源：http://baike.tarul.cn/Article/details/gfexovslv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.tarul.cn/Article/details/ghzhznxac.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.vehdjk.com/Article/details/gkfxsltln.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.vehdjk.com/Article/details/gjtaczxaq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/gcmpwdvdu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.tarul.cn/Article/details/gbxrdggvz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fktsv.cn/Article/details/gawzawoan.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fktsv.cn/Article/details/gmyctuhio.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.bbcook.cn/Article/details/glgmlndpv.sHtML


<!-- 参考信息 -->