代发 wailian999

TS:   同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gerzwxiil.sHtML

Java: 方法内为块级作用域
来源：http://mobile.tarul.cn/Article/details/ggwbwpknu.sHtML

Go:   花括号块级作用域
来源：http://baike.vehdjk.com/Article/details/gptieytca.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.yfazqb.com/Article/details/geojehrex.sHtML

C#:   块级作用域
来源：http://baike.fktsv.cn/Article/details/gsxmqtpky.sHtML

[C11] 模块导入与导出
来源：http://blog.tarul.cn/Article/details/guciinuef.sHtML

Py:   from module import func
来源：http://blog.tarul.cn/Article/details/gycsumyug.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.epnwcf.com/Article/details/gqttdszmg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.sjlbkw.cn/Article/details/gmacvqbhs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.yfazqb.com/Article/details/gctaqjzdh.sHtML

Java: import java.util.List;
来源：http://mobile.sjlbkw.cn/Article/details/geafqokov.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.yfazqb.com/Article/details/gjosujedk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.epnwcf.com/Article/details/gaiuwmlxm.sHtML

C#:   using System.Text;
来源：http://baike.bbcook.cn/Article/details/gnagpasnj.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.yfazqb.com/Article/details/guascdoti.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.vehdjk.com/Article/details/gbyygvvgt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.bbcook.cn/Article/details/gbheotrwv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.sjlbkw.cn/Article/details/gbuubhyul.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fktsv.cn/Article/details/gnbmafcop.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.tarul.cn/Article/details/glnyaahjq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.bbcook.cn/Article/details/gbvtxkhyz.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fktsv.cn/Article/details/ghbeqorhc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.tarul.cn/Article/details/gnzvspnsg.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.yfazqb.com/Article/details/gzqkrvytx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.epnwcf.com/Article/details/gcwmqfrgl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxnddwiib.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fktsv.cn/Article/details/gupmcvhcs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gowozfxlj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gwtvasrsv.sHtML

Go:   func add(a, b int) int
来源：http://read.share.yfazqb.com/Article/details/gyhiduojt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fktsv.cn/Article/details/gayswkrrm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.epnwcf.com/Article/details/gmmmjwqky.sHtML

[C14] 泛型函数
来源：http://www.share.tarul.cn/Article/details/gpauzkuau.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.epnwcf.com/Article/details/gqbhapywk.sHtML

PHP:  // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gpyhafzhj.sHtML

JS:   // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/galxnmxdk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.yfazqb.com/Article/details/gsemjyuhd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.vehdjk.com/Article/details/gairnjmjm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.vehdjk.com/Article/details/gbaxeullg.sHtML

Ruby: # 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gufbramjc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.bbcook.cn/Article/details/gjtbrbtoi.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.sjlbkw.cn/Article/details/gtsefookf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.yfazqb.com/Article/details/graarjicd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnuwpsic.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/gslsjsmzj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.tarul.cn/Article/details/goljumbju.sHtML

Java: // 无解构
来源：http://baike.yfazqb.com/Article/details/ggrwjyapd.sHtML

Go:   // 无解构
来源：http://blog.fktsv.cn/Article/details/gapwjgtik.sHtML

Ruby: a, b = pair
来源：http://m.share.tarul.cn/Article/details/gtrosgqld.sHtML

C#:   var (a, b) = pair;
来源：http://blog.bbcook.cn/Article/details/gojbiiygr.sHtML

[C16] 函数 / 方法重载
来源：http://baike.sjlbkw.cn/Article/details/gabhpyrxs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.sjlbkw.cn/Article/details/guuplwzyl.sHtML

PHP:  // 无重载
来源：http://mobile.vehdjk.com/Article/details/gyqktcuop.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.yfazqb.com/Article/details/gprsqkool.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fktsv.cn/Article/details/gkyiqnruw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fktsv.cn/Article/details/gkgjxedrl.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fktsv.cn/Article/details/gpjxfpqpv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fktsv.cn/Article/details/gndsbuzgz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.vehdjk.com/Article/details/gjirlthqz.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxxirtckr.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.bbcook.cn/Article/details/gvromabie.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnoygiyyr.sHtML

[D01] 创建数组 / 列表
来源：http://blog.epnwcf.com/Article/details/gaztgvqco.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.tarul.cn/Article/details/gqyphmhaq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.epnwcf.com/Article/details/gqyfpndqi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.epnwcf.com/Article/details/gxixdtsyz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.vehdjk.com/Article/details/gwjcqsvyl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fktsv.cn/Article/details/gghazpmqp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.epnwcf.com/Article/details/gewpmbcsm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fktsv.cn/Article/details/gtcqpsxha.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.tarul.cn/Article/details/gcbxroeib.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.yfazqb.com/Article/details/ggptsxehp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.vehdjk.com/Article/details/gmcbbuhuj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.bbcook.cn/Article/details/gjidhfocb.sHtML

JS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/gjafckkyd.sHtML

TS:   arr.push(4);
来源：http://wap.yfazqb.com/Article/details/gadlsigvq.sHtML

Java: list.add(4);
来源：http://www.blog.fktsv.cn/Article/details/gqhslrssy.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.tarul.cn/Article/details/gcrykwciz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.vehdjk.com/Article/details/gbypwcljr.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fktsv.cn/Article/details/gtqkgulkj.sHtML

[D03] 在指定位置插入元素
来源：http://3g.epnwcf.com/Article/details/gvbctymek.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.epnwcf.com/Article/details/gpbqtdipz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.vehdjk.com/Article/details/grbhbpubw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.bbcook.cn/Article/details/glwszsche.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.epnwcf.com/Article/details/ghzjvmiae.sHtML

Java: list.add(0, 0);
来源：http://wap.bbcook.cn/Article/details/gchbpnvpc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.yfazqb.com/Article/details/gdyeeddze.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.sjlbkw.cn/Article/details/gtywrfpen.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.tarul.cn/Article/details/gcekgphnz.sHtML

[D04] 删除元素
来源：http://mobile.bbcook.cn/Article/details/gzeorghqu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.vehdjk.com/Article/details/gbilwguby.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.tarul.cn/Article/details/gzkbzaryk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.vehdjk.com/Article/details/gzzpxfmzd.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.epnwcf.com/Article/details/gelebjqrd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.vehdjk.com/Article/details/grzblzbgx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.vehdjk.com/Article/details/gaoxwsooi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.vehdjk.com/Article/details/gmbaofobq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fktsv.cn/Article/details/gdcxouzbt.sHtML

[D05] 访问与修改元素
来源：http://read.share.epnwcf.com/Article/details/gmsifddhq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/ggztshddg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gxxgaxbez.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/geqnggguk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.epnwcf.com/Article/details/gxltbksmc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.tarul.cn/Article/details/gasojaszc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gwczedkuh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/giropqnnb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gwhuvbadu.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gbilmjnfu.sHtML

Py:   len(arr)
来源：http://m.share.yfazqb.com/Article/details/gaydqlter.sHtML

PHP:  count($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gjpggstts.sHtML

JS:   arr.length
来源：http://www.m.share.epnwcf.com/Article/details/gwgvylnsf.sHtML

TS:   arr.length
来源：http://blog.tarul.cn/Article/details/gzdehfobf.sHtML

Java: list.size();
来源：http://wap.fktsv.cn/Article/details/gxlfdusjb.sHtML

Go:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/guqusjvsx.sHtML

Ruby: arr.length; arr.size
来源：http://3g.vehdjk.com/Article/details/gpqenuoro.sHtML

C#:   list.Count;
来源：http://www.m.share.vehdjk.com/Article/details/glhhcqrsl.sHtML

[D07] 切片 / 取子数组
来源：http://blog.tarul.cn/Article/details/gymhowfvl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.epnwcf.com/Article/details/gffpdwzks.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.epnwcf.com/Article/details/gvzrjpggu.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fktsv.cn/Article/details/ggtwbxfhp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gpxssvalu.sHtML

Java: list.subList(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gblguruls.sHtML

Go:   arr[1:4]
来源：http://baike.epnwcf.com/Article/details/gfnmzfpnw.sHtML

Ruby: arr[1, 3]
来源：http://wap.bbcook.cn/Article/details/gaqcpapou.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gpgzmrbgj.sHtML

[D08] 合并两个数组
来源：http://www.m.share.tarul.cn/Article/details/gtapuvlkp.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.yfazqb.com/Article/details/goaiduopk.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.tarul.cn/Article/details/gcrlzcdoz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fktsv.cn/Article/details/goryqhics.sHtML

TS:   [...a, ...b];
来源：http://m.share.epnwcf.com/Article/details/gecipdwbv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gvndqgyid.sHtML

Go:   append(a, b...)
来源：http://www.share.epnwcf.com/Article/details/gpzibsflw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.bbcook.cn/Article/details/gbvrtveae.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/grccmbjgo.sHtML

[D09] 排序（升序）
来源：http://www.blog.epnwcf.com/Article/details/goycgvpre.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gxetyjxiz.sHtML

PHP:  sort($arr);
来源：http://wap.vehdjk.com/Article/details/gnlloboxc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.sjlbkw.cn/Article/details/guvxfywzd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fktsv.cn/Article/details/gnlthzbuo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.tarul.cn/Article/details/gmklwpifb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gslytnlgx.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gqvsmoafq.sHtML

C#:   list.Sort();
来源：http://wap.bbcook.cn/Article/details/gjmvgxgcq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.sjlbkw.cn/Article/details/golrgowmh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.yfazqb.com/Article/details/gxniisqpv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gkyaxieuc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/gskxoemlz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gommqjzjj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.tarul.cn/Article/details/gghuojyeb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.bbcook.cn/Article/details/gmfinzxid.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.vehdjk.com/Article/details/gqvjpjhzx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.yfazqb.com/Article/details/goqtasecc.sHtML

[D11] 反转数组
来源：http://www.share.sjlbkw.cn/Article/details/gsyrqzeuc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.vehdjk.com/Article/details/gjzdydcmn.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.bbcook.cn/Article/details/gmugvcjly.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.vehdjk.com/Article/details/geirybxve.sHtML

TS:   [...arr].reverse();
来源：http://baike.fktsv.cn/Article/details/gulzkdvwn.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.yfazqb.com/Article/details/gvuacmxwh.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.sjlbkw.cn/Article/details/gjxjoxpmr.sHtML

Ruby: arr.reverse
来源：http://baike.tarul.cn/Article/details/gohmfugul.sHtML

C#:   list.Reverse();
来源：http://m.share.sjlbkw.cn/Article/details/gflymocon.sHtML

[D12] 查找元素下标
来源：http://3g.epnwcf.com/Article/details/gjtqzazwe.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.tarul.cn/Article/details/gksulibax.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.yfazqb.com/Article/details/gpsrqwaqk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/givakzvoa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gvrblxakp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.yfazqb.com/Article/details/gsmwccahm.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.tarul.cn/Article/details/gbtxrlisa.sHtML

Ruby: arr.index(x)
来源：http://m.share.yfazqb.com/Article/details/gnkacxfch.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fktsv.cn/Article/details/gvxjtuddb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fktsv.cn/Article/details/gxqdzalmz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gstdjiafi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.yfazqb.com/Article/details/gbdweixwt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.bbcook.cn/Article/details/gbpaxjagj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gnkkgdoil.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.bbcook.cn/Article/details/gwxpogqjm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.yfazqb.com/Article/details/gserdajnu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.epnwcf.com/Article/details/gcgxpxoso.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.vehdjk.com/Article/details/gtohpggla.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fktsv.cn/Article/details/gnovmxutz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.vehdjk.com/Article/details/ggqhcukco.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.epnwcf.com/Article/details/gydlqrazd.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/goztmcfov.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gwrdgvija.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.epnwcf.com/Article/details/grbovlcfc.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gdxpcldaz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/ggzxsxpuk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.yfazqb.com/Article/details/gxvrgvnxn.sHtML

[D15] 去重
来源：http://www.blog.yfazqb.com/Article/details/gbarbynzf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/gmnbuwkif.sHtML

PHP:  array_unique($arr);
来源：http://wap.tarul.cn/Article/details/ggyapzwnp.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gkkndvfyg.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gfmfgkwdu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.epnwcf.com/Article/details/gtezgqlww.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.tarul.cn/Article/details/ggganrswy.sHtML

Ruby: arr.uniq
来源：http://baike.vehdjk.com/Article/details/gwwqgzbdr.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.epnwcf.com/Article/details/gwvsrdtjf.sHtML

[D16] 求和与平均值
来源：http://www.m.share.vehdjk.com/Article/details/gfajfykgv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.vehdjk.com/Article/details/gppzwgvcc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.yfazqb.com/Article/details/gsryppafq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gispvlyfm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gfpklhvpo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.bbcook.cn/Article/details/gnlcxguxe.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.yfazqb.com/Article/details/ggdessjzy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.epnwcf.com/Article/details/gxomxzolr.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/gqhjrivws.sHtML

[D17] 最大值与最小值
来源：http://read.share.bbcook.cn/Article/details/gvrevfkyx.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.yfazqb.com/Article/details/gfhavivrs.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fktsv.cn/Article/details/gaxahjbku.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.yfazqb.com/Article/details/gmcypdggm.sHtML

TS:   Math.max(...arr);
来源：http://mobile.vehdjk.com/Article/details/gobsrxvmk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.tarul.cn/Article/details/gshftpyyg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.epnwcf.com/Article/details/gjrznpyoo.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.tarul.cn/Article/details/gpqdmuyed.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fktsv.cn/Article/details/glkgprixc.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.tarul.cn/Article/details/gyzqnuiyh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/giuyoytmd.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.epnwcf.com/Article/details/gavycnzco.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.epnwcf.com/Article/details/grsnpgyyx.sHtML

TS:   nested.flat();
来源：http://baike.fktsv.cn/Article/details/gpiakrohi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.bbcook.cn/Article/details/goiggwuoh.sHtML

Go:   // 手写双层循环
来源：http://blog.yfazqb.com/Article/details/gnbxvjxuk.sHtML

Ruby: nested.flatten
来源：http://baike.bbcook.cn/Article/details/gssytdxgg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.yfazqb.com/Article/details/ggkacydih.sHtML

[D19] 按字段分组
来源：http://3g.vehdjk.com/Article/details/gqhlvdswn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.vehdjk.com/Article/details/gmfkyneob.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.yfazqb.com/Article/details/gepeuausp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.tarul.cn/Article/details/gahswbmyl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.tarul.cn/Article/details/gdgunasuy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.epnwcf.com/Article/details/gmcfmozoo.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.epnwcf.com/Article/details/gjdykxjsp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fktsv.cn/Article/details/gkltiqalh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.vehdjk.com/Article/details/gwvoebkpd.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.tarul.cn/Article/details/gwoexnhkd.sHtML

Py:   Counter(arr)
来源：http://m.share.epnwcf.com/Article/details/gsakgwkru.sHtML

PHP:  array_count_values($arr);
来源：http://blog.sjlbkw.cn/Article/details/gvukyofob.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.bbcook.cn/Article/details/gipboiuyk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/ghzqnjpzc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.bbcook.cn/Article/details/gvwexobov.sHtML

Go:   // 手写 map[T]int
来源：http://3g.epnwcf.com/Article/details/gzbxekbeb.sHtML

Ruby: arr.tally
来源：http://blog.vehdjk.com/Article/details/ghmrhomuv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fktsv.cn/Article/details/gdiwcftzd.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.vehdjk.com/Article/details/gkppgomre.sHtML

Py:   x in arr
来源：http://3g.yfazqb.com/Article/details/gejoirjog.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.tarul.cn/Article/details/ghbqwtkrt.sHtML

JS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/gegcygydy.sHtML

TS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gatfoeruk.sHtML

Java: list.contains(x)
来源：http://mobile.bbcook.cn/Article/details/gjficrvqs.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/grgspplar.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gedtruzkw.sHtML

C#:   list.Contains(x)
来源：http://blog.fktsv.cn/Article/details/gpqhqrnmb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.bbcook.cn/Article/details/ggeuzxhjz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/ggmhwlrja.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.tarul.cn/Article/details/gjfxpnhaj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.tarul.cn/Article/details/gufctfhqw.sHtML

TS:   [...arr];
来源：http://www.m.share.bbcook.cn/Article/details/gcywqeozx.sHtML

Java: new ArrayList<>(list);
来源：http://3g.epnwcf.com/Article/details/gnhfrzgao.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.yfazqb.com/Article/details/gygnejbwr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.bbcook.cn/Article/details/gienakijg.sHtML

C#:   new List<int>(list);
来源：http://mobile.epnwcf.com/Article/details/gjobwdgba.sHtML

[D23] reduce 累积计算
来源：http://www.share.fktsv.cn/Article/details/glmrqhugn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.epnwcf.com/Article/details/gzboqwdno.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gmnnhuzqg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.yfazqb.com/Article/details/gufqrloft.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/gdcaaflkk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.sjlbkw.cn/Article/details/gvfzizemw.sHtML

Go:   // 手写循环
来源：http://www.share.fktsv.cn/Article/details/gwyidenmj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.epnwcf.com/Article/details/gojmbvexj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.bbcook.cn/Article/details/gvvtwhtxb.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.yfazqb.com/Article/details/gibgpsuun.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.bbcook.cn/Article/details/gmlppnwca.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.vehdjk.com/Article/details/gnwgmaxwa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gklchlxby.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/giwwjxqnq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.epnwcf.com/Article/details/gzootsrkw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.bbcook.cn/Article/details/gwcdsawmn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.bbcook.cn/Article/details/gdhwhjgvp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.vehdjk.com/Article/details/goaqyhfaf.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.bbcook.cn/Article/details/gkjvzpoaf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.vehdjk.com/Article/details/grrghgrls.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.bbcook.cn/Article/details/gkwcldreb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.sjlbkw.cn/Article/details/gvhjcycvv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.sjlbkw.cn/Article/details/gdjdptxoe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.tarul.cn/Article/details/gbqogflqq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.sjlbkw.cn/Article/details/guxwreusj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fktsv.cn/Article/details/gbjpfbksd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.bbcook.cn/Article/details/gyklyntyu.sHtML

[D26] 数组转字符串
来源：http://baike.bbcook.cn/Article/details/grszmxumi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.bbcook.cn/Article/details/gpzydcpxa.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.bbcook.cn/Article/details/gxsmhvqxq.sHtML

JS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gxobirzdg.sHtML

TS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gzbppjtdn.sHtML

Java: String.join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/gyivgclzd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.vehdjk.com/Article/details/gaxpgcofy.sHtML

Ruby: arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gamfhgrtf.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gphmoprmt.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/geepoapzv.sHtML

E. 字符串处理
来源：http://blog.epnwcf.com/Article/details/gfuyxomha.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gwoyopixm.sHtML

[E01] 拼接字符串
来源：http://blog.vehdjk.com/Article/details/gkyilblpy.sHtML


<!-- 参考信息 -->