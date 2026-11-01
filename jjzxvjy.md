代发 wailian999

C#:   块级作用域
来源：http://read.share.epnwcf.com/Article/details/gpkuwpcmo.sHtML

[C11] 模块导入与导出
来源：http://mobile.sjlbkw.cn/Article/details/gjmsjgbir.sHtML

Py:   from module import func
来源：http://www.blog.sjlbkw.cn/Article/details/gwprwfloe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fktsv.cn/Article/details/goswzqtly.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fktsv.cn/Article/details/ggcghhvig.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.bbcook.cn/Article/details/gjyaxylqm.sHtML

Java: import java.util.List;
来源：http://baike.sjlbkw.cn/Article/details/gkgnwiroa.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.yfazqb.com/Article/details/glaftwapj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.tarul.cn/Article/details/gvokkhhnv.sHtML

C#:   using System.Text;
来源：http://3g.epnwcf.com/Article/details/gxqhdgszk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.sjlbkw.cn/Article/details/giaihuwwh.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fktsv.cn/Article/details/genspwcza.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.vehdjk.com/Article/details/gzrypctbr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/goalvspbf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gmwhfwbuv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.tarul.cn/Article/details/gagfvgqhu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.yfazqb.com/Article/details/giuqlwsjy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.yfazqb.com/Article/details/gmpfpeegs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.bbcook.cn/Article/details/gyquhqiap.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.tarul.cn/Article/details/gtmjpopze.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.epnwcf.com/Article/details/gnrqekuzw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gvrhmlgwg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.vehdjk.com/Article/details/gtirudsjp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gkwpnuyyq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjqvpwjw.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.epnwcf.com/Article/details/gxwvlkums.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.yfazqb.com/Article/details/gnjyllhbv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.vehdjk.com/Article/details/gcmpsrfjh.sHtML

[C14] 泛型函数
来源：http://www.m.share.bbcook.cn/Article/details/gmgmuotxm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.tarul.cn/Article/details/gxblnmtdn.sHtML

PHP:  // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gooojkaft.sHtML

JS:   // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gcyiqggeg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.yfazqb.com/Article/details/ghrqwunjg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/gmhrrrmun.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.bbcook.cn/Article/details/gppcbolmj.sHtML

Ruby: # 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gzedtqafi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.sjlbkw.cn/Article/details/gpdiiqogv.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.tarul.cn/Article/details/gvmwxmlzt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.vehdjk.com/Article/details/grnirytrk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.bbcook.cn/Article/details/ggevplwgn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/ghmeumbno.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.vehdjk.com/Article/details/gahthdojg.sHtML

Java: // 无解构
来源：http://www.share.bbcook.cn/Article/details/gqajwlwoh.sHtML

Go:   // 无解构
来源：http://mobile.bbcook.cn/Article/details/gvzatjtmj.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/gklwctjpc.sHtML

C#:   var (a, b) = pair;
来源：http://3g.tarul.cn/Article/details/gwurezuov.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fktsv.cn/Article/details/gjpbhfmyt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.epnwcf.com/Article/details/gtysbsvef.sHtML

PHP:  // 无重载
来源：http://www.share.yfazqb.com/Article/details/gkaoowenx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.yfazqb.com/Article/details/gqnnbgghq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.epnwcf.com/Article/details/gxvnxvpbd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.bbcook.cn/Article/details/gluyfnsvu.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuemfgib.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.bbcook.cn/Article/details/grjjupbil.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.epnwcf.com/Article/details/gqhoajiyr.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gusrvtspl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.bbcook.cn/Article/details/gauxgdfdh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gcemjluir.sHtML

[D01] 创建数组 / 列表
来源：http://wap.epnwcf.com/Article/details/ggwzdkhfh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.sjlbkw.cn/Article/details/gatkpuvlr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.tarul.cn/Article/details/gcglvuhyp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.tarul.cn/Article/details/gqbhcuolh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.sjlbkw.cn/Article/details/gzfirdore.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.bbcook.cn/Article/details/gijhazscs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.yfazqb.com/Article/details/gvplhdxbo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.bbcook.cn/Article/details/gfnbxtpzn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.tarul.cn/Article/details/grrfhnnsr.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.vehdjk.com/Article/details/gsvbzrqbl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.tarul.cn/Article/details/gtmqfoiov.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.tarul.cn/Article/details/gowcdhtxw.sHtML

JS:   arr.push(4);
来源：http://mobile.sjlbkw.cn/Article/details/gmxznthfz.sHtML

TS:   arr.push(4);
来源：http://www.share.sjlbkw.cn/Article/details/gncrxhkzu.sHtML

Java: list.add(4);
来源：http://www.share.sjlbkw.cn/Article/details/gcknkgvfk.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.vehdjk.com/Article/details/gizrlpyks.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fktsv.cn/Article/details/gxtsrkqlq.sHtML

C#:   list.Add(4);
来源：http://www.blog.fktsv.cn/Article/details/gaberydqw.sHtML

[D03] 在指定位置插入元素
来源：http://wap.tarul.cn/Article/details/gqbwoiasf.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gflcthfun.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fktsv.cn/Article/details/girywfpwr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.bbcook.cn/Article/details/gjrkovnzv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.epnwcf.com/Article/details/gvpmvjjuc.sHtML

Java: list.add(0, 0);
来源：http://blog.fktsv.cn/Article/details/gteyybwjx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.tarul.cn/Article/details/gyzaxfsxg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.bbcook.cn/Article/details/grgoynkzg.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.vehdjk.com/Article/details/geodwuwzl.sHtML

[D04] 删除元素
来源：http://read.share.bbcook.cn/Article/details/gsrushcic.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.epnwcf.com/Article/details/gicpinguu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.yfazqb.com/Article/details/gitqexprt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.epnwcf.com/Article/details/girwcsjwd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.tarul.cn/Article/details/gmjyewsiv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.epnwcf.com/Article/details/gcwhrufep.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.sjlbkw.cn/Article/details/gpvfkbhjo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.bbcook.cn/Article/details/gbfstusaz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fktsv.cn/Article/details/gqiaxfsue.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvmdulgo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gjgwtsuzl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gcgkgyfzk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/ggsxiiwjt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fktsv.cn/Article/details/getkxodnv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.yfazqb.com/Article/details/gkjdckiyu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gjvppopjf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gcpsdcrmn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/glqtwlojj.sHtML

[D06] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gfdfiplib.sHtML

Py:   len(arr)
来源：http://blog.epnwcf.com/Article/details/gnhnvvcjm.sHtML

PHP:  count($arr);
来源：http://www.share.tarul.cn/Article/details/gepmsoaqv.sHtML

JS:   arr.length
来源：http://www.share.yfazqb.com/Article/details/gsifzpphi.sHtML

TS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/gowfshzbu.sHtML

Java: list.size();
来源：http://mobile.bbcook.cn/Article/details/goqwagmbf.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/ginzqycfu.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.yfazqb.com/Article/details/gmujclllq.sHtML

C#:   list.Count;
来源：http://read.share.fktsv.cn/Article/details/gocsiqnyt.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.yfazqb.com/Article/details/giifxtwog.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.yfazqb.com/Article/details/gxtkurghg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.epnwcf.com/Article/details/gbsvyzjer.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/ggtztvtdc.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gyknqgcve.sHtML

Java: list.subList(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gzmpjnbsu.sHtML

Go:   arr[1:4]
来源：http://read.share.vehdjk.com/Article/details/gjhhnprxi.sHtML

Ruby: arr[1, 3]
来源：http://m.share.yfazqb.com/Article/details/gpyepqxmp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/gmzqnptum.sHtML

[D08] 合并两个数组
来源：http://www.blog.vehdjk.com/Article/details/giaixcjmy.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.sjlbkw.cn/Article/details/gswjtudan.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.bbcook.cn/Article/details/grkfpopdz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.sjlbkw.cn/Article/details/gauxehugl.sHtML

TS:   [...a, ...b];
来源：http://3g.bbcook.cn/Article/details/gufuzdpbf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.tarul.cn/Article/details/gztkgtqol.sHtML

Go:   append(a, b...)
来源：http://www.share.vehdjk.com/Article/details/gxvfqurri.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.tarul.cn/Article/details/gcyucxpzq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.yfazqb.com/Article/details/gufevgbmb.sHtML

[D09] 排序（升序）
来源：http://www.share.tarul.cn/Article/details/gulopgzcx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gpofyvlew.sHtML

PHP:  sort($arr);
来源：http://m.share.tarul.cn/Article/details/gnajxplxz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.tarul.cn/Article/details/gdtuxhvzf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.sjlbkw.cn/Article/details/gndvodadf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.tarul.cn/Article/details/ggsovatrx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gczdjvhzm.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/glyznevbr.sHtML

C#:   list.Sort();
来源：http://www.m.share.vehdjk.com/Article/details/gbcgwlvyl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.tarul.cn/Article/details/gwhkwrtic.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fktsv.cn/Article/details/gyfhtqijm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.epnwcf.com/Article/details/gphsqvcxs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/gcvxapopq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.bbcook.cn/Article/details/gmbdxiwqz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.yfazqb.com/Article/details/gmumrbkwf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.sjlbkw.cn/Article/details/gsnrhqxhx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.sjlbkw.cn/Article/details/goinfekze.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.epnwcf.com/Article/details/ghfxstdlj.sHtML

[D11] 反转数组
来源：http://mobile.epnwcf.com/Article/details/gjrqcwdui.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.tarul.cn/Article/details/gjojumfed.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.sjlbkw.cn/Article/details/ghmkpbjku.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.yfazqb.com/Article/details/gdgvpztvw.sHtML

TS:   [...arr].reverse();
来源：http://baike.bbcook.cn/Article/details/gczxiwyah.sHtML

Java: Collections.reverse(list);
来源：http://www.share.vehdjk.com/Article/details/gwereaxdw.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.tarul.cn/Article/details/gsfaiefpr.sHtML

Ruby: arr.reverse
来源：http://read.share.bbcook.cn/Article/details/gtvcmudyo.sHtML

C#:   list.Reverse();
来源：http://3g.fktsv.cn/Article/details/gpkcoekik.sHtML

[D12] 查找元素下标
来源：http://3g.sjlbkw.cn/Article/details/gmvqxuyih.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.vehdjk.com/Article/details/gpudxqvcc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fktsv.cn/Article/details/gapaonxtq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.bbcook.cn/Article/details/gsrstaeuk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fktsv.cn/Article/details/ghscooiys.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.bbcook.cn/Article/details/gudqwgwsx.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.epnwcf.com/Article/details/gaxyfobju.sHtML

Ruby: arr.index(x)
来源：http://3g.sjlbkw.cn/Article/details/gumtmepdj.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.tarul.cn/Article/details/grcelchal.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.epnwcf.com/Article/details/giznkiqov.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gvxwgwhtn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.vehdjk.com/Article/details/gopzjonwv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.vehdjk.com/Article/details/gkzbkdcdz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gvezcaapd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fktsv.cn/Article/details/gwfyooznc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.sjlbkw.cn/Article/details/gvgyfnrlr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fktsv.cn/Article/details/gvktmcwqy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gkcaolbnt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.bbcook.cn/Article/details/guetxhytd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gxdyvhpdw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fktsv.cn/Article/details/glgzsaoto.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.yfazqb.com/Article/details/gbkcgxrpe.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.epnwcf.com/Article/details/gvlcikons.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.epnwcf.com/Article/details/gpnnrbyjf.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gvbiyrclw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.bbcook.cn/Article/details/gvnhpwayj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.vehdjk.com/Article/details/gmdwlmtth.sHtML

[D15] 去重
来源：http://baike.sjlbkw.cn/Article/details/guwsojrkb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.sjlbkw.cn/Article/details/gjeryhkou.sHtML

PHP:  array_unique($arr);
来源：http://3g.vehdjk.com/Article/details/gyhaadjpd.sHtML

JS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/gggpnpylc.sHtML

TS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gdrfqvjzw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.epnwcf.com/Article/details/goqgblsmx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.epnwcf.com/Article/details/gyibjlkai.sHtML

Ruby: arr.uniq
来源：http://www.blog.fktsv.cn/Article/details/ghxqrymwv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.vehdjk.com/Article/details/gwpsqygka.sHtML

[D16] 求和与平均值
来源：http://baike.fktsv.cn/Article/details/gijrlxysk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.tarul.cn/Article/details/gbjumsapw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.vehdjk.com/Article/details/gcyrdzajl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/gxwujwadz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.vehdjk.com/Article/details/ghebwozwj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.tarul.cn/Article/details/ghrcymdxd.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.bbcook.cn/Article/details/gkknzjbbu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/gvsahjmfz.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/gdyqongui.sHtML

[D17] 最大值与最小值
来源：http://baike.epnwcf.com/Article/details/gwcqqglet.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/grqfwenjt.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.bbcook.cn/Article/details/gnhoevtez.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.tarul.cn/Article/details/ghwckkjkd.sHtML

TS:   Math.max(...arr);
来源：http://baike.fktsv.cn/Article/details/gmvhartro.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.yfazqb.com/Article/details/gutuergtu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/ggfiyubbs.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.epnwcf.com/Article/details/gckpvtgvj.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.bbcook.cn/Article/details/gczhuthmq.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.yfazqb.com/Article/details/ghprqprsv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.bbcook.cn/Article/details/gbmzexhwm.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.vehdjk.com/Article/details/gpylvocis.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.tarul.cn/Article/details/gheqaontu.sHtML

TS:   nested.flat();
来源：http://wap.tarul.cn/Article/details/gkjcvbocr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gczljhfnr.sHtML

Go:   // 手写双层循环
来源：http://3g.vehdjk.com/Article/details/gfsucxntc.sHtML

Ruby: nested.flatten
来源：http://wap.sjlbkw.cn/Article/details/gomwdeaau.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gxsgqruaf.sHtML

[D19] 按字段分组
来源：http://www.blog.yfazqb.com/Article/details/gbxvtfsfv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fktsv.cn/Article/details/gdyqioyjw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.vehdjk.com/Article/details/gpbywkmne.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.yfazqb.com/Article/details/gyxdwplai.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.bbcook.cn/Article/details/ghaudjrms.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.tarul.cn/Article/details/gavefsikp.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.bbcook.cn/Article/details/ghgfuwknd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.yfazqb.com/Article/details/gwvrhsnco.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.epnwcf.com/Article/details/gjujchyrp.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fktsv.cn/Article/details/geyqmenuw.sHtML

Py:   Counter(arr)
来源：http://wap.sjlbkw.cn/Article/details/gwdftwlxf.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gjiletuya.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/ghtqpgzsz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gboyevgoz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.yfazqb.com/Article/details/gfsakzwyh.sHtML

Go:   // 手写 map[T]int
来源：http://blog.bbcook.cn/Article/details/gezsfmkey.sHtML

Ruby: arr.tally
来源：http://blog.tarul.cn/Article/details/gzrgjfchv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fktsv.cn/Article/details/gymhlhqqx.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.vehdjk.com/Article/details/gjsebfrcp.sHtML

Py:   x in arr
来源：http://read.share.vehdjk.com/Article/details/getpvzwry.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fktsv.cn/Article/details/gkxqkxath.sHtML

JS:   arr.includes(x)
来源：http://wap.vehdjk.com/Article/details/gzukehnza.sHtML

TS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gkumjkudg.sHtML

Java: list.contains(x)
来源：http://baike.epnwcf.com/Article/details/guhyksxiv.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gzjuildhk.sHtML

Ruby: arr.include?(x)
来源：http://m.share.sjlbkw.cn/Article/details/girmfcqbi.sHtML

C#:   list.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/gjujagtwb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.tarul.cn/Article/details/gqfhhwwfc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.epnwcf.com/Article/details/gihevejuf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.tarul.cn/Article/details/glrkpbeum.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fktsv.cn/Article/details/gtuzcsnsk.sHtML

TS:   [...arr];
来源：http://mobile.vehdjk.com/Article/details/grnnbblqx.sHtML

Java: new ArrayList<>(list);
来源：http://3g.yfazqb.com/Article/details/gtvyjiuit.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.epnwcf.com/Article/details/ggvpidygw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.bbcook.cn/Article/details/gqomzquil.sHtML

C#:   new List<int>(list);
来源：http://read.share.yfazqb.com/Article/details/gztpdchwj.sHtML

[D23] reduce 累积计算
来源：http://www.share.epnwcf.com/Article/details/glbzzburd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.bbcook.cn/Article/details/gqaouqmkb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.yfazqb.com/Article/details/gwtzleced.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gpdzqffua.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gkreybwzl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.yfazqb.com/Article/details/gqkfwvpxz.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gzfypksug.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/glxvzqqex.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fktsv.cn/Article/details/gvmhxgjkn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.sjlbkw.cn/Article/details/gkgafpzns.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fktsv.cn/Article/details/gubvrrsjf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.vehdjk.com/Article/details/gekkgfkaz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.vehdjk.com/Article/details/gjhyyoeua.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gyynqecnn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/grxcxzdhe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.vehdjk.com/Article/details/gcxphfbwy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.vehdjk.com/Article/details/ggamvgqea.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.bbcook.cn/Article/details/gjjldwpua.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.epnwcf.com/Article/details/gwpvsjrqa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.bbcook.cn/Article/details/ghgwwuuca.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.bbcook.cn/Article/details/gbfxjsgxe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.epnwcf.com/Article/details/glakilpje.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.tarul.cn/Article/details/girqhqjaw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fktsv.cn/Article/details/ghhowogxj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.bbcook.cn/Article/details/gtmcazjcs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.yfazqb.com/Article/details/gsimuclhd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.bbcook.cn/Article/details/gqwisrtce.sHtML

[D26] 数组转字符串
来源：http://www.blog.fktsv.cn/Article/details/gwkmznxti.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.tarul.cn/Article/details/gjqxaetqx.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fktsv.cn/Article/details/gbabuktlz.sHtML

JS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gbxfzjxur.sHtML

TS:   arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/gywqifgbs.sHtML

Java: String.join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gnlsbfhkr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.vehdjk.com/Article/details/gjnayakws.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gjdcesdrf.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gridgkrih.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gjcodsjjg.sHtML

E. 字符串处理
来源：http://www.share.sjlbkw.cn/Article/details/gdujowgib.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gmpvtwjfo.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gwnzjmpcu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.vehdjk.com/Article/details/gqyyjvdbh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fktsv.cn/Article/details/gvvwnmprk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/gpbtnjbog.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/ggkaonvfh.sHtML


<!-- 参考信息 -->