代发 wailian999

C#:   块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gthvorjws.sHtML

[C11] 模块导入与导出
来源：http://m.share.fktsv.cn/Article/details/geyoxkrpx.sHtML

Py:   from module import func
来源：http://blog.yfazqb.com/Article/details/glukdjgpd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fktsv.cn/Article/details/gyqkmbdsz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.yfazqb.com/Article/details/gzflpqjks.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fktsv.cn/Article/details/gabhlqlgo.sHtML

Java: import java.util.List;
来源：http://m.share.vehdjk.com/Article/details/gkxxojkwn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.vehdjk.com/Article/details/gsecjyryr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/gkaypwbpo.sHtML

C#:   using System.Text;
来源：http://3g.epnwcf.com/Article/details/gjourhook.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.vehdjk.com/Article/details/gtnoplhic.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.bbcook.cn/Article/details/gjphrmjct.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.tarul.cn/Article/details/gfwfdfwsl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.sjlbkw.cn/Article/details/gwqzhbrhs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/gdvmuhyqw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fktsv.cn/Article/details/gtyoenuqd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.tarul.cn/Article/details/gpbqwewnw.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.tarul.cn/Article/details/gvxdhvfht.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.vehdjk.com/Article/details/gfhiqhqxy.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.vehdjk.com/Article/details/goalktejk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.bbcook.cn/Article/details/gqeucessl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gmvrzzhqu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fktsv.cn/Article/details/gffyisbth.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gwbwgbegf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/glxqqlcmy.sHtML

Go:   func add(a, b int) int
来源：http://3g.yfazqb.com/Article/details/gvktxualg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.bbcook.cn/Article/details/gpvzxzttj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.sjlbkw.cn/Article/details/gdrgwdbui.sHtML

[C14] 泛型函数
来源：http://3g.fktsv.cn/Article/details/giadrlzlo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.sjlbkw.cn/Article/details/gbeownjue.sHtML

PHP:  // 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gfgnuzrfs.sHtML

JS:   // 无泛型
来源：http://baike.fktsv.cn/Article/details/grtowpylb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.bbcook.cn/Article/details/gejsuyzps.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.sjlbkw.cn/Article/details/gtadxhiyr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.epnwcf.com/Article/details/gmyvhowwp.sHtML

Ruby: # 无泛型
来源：http://mobile.yfazqb.com/Article/details/gotwyccqh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.sjlbkw.cn/Article/details/gxunxhgzd.sHtML

[C15] 解构 / 展开参数
来源：http://wap.vehdjk.com/Article/details/gmmgavdhl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/ggxyamyml.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.tarul.cn/Article/details/gqxqofnpp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/gkqnaoivn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.yfazqb.com/Article/details/gyyhtwwoy.sHtML

Java: // 无解构
来源：http://baike.yfazqb.com/Article/details/grqcbbkhl.sHtML

Go:   // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/gtwhellwf.sHtML

Ruby: a, b = pair
来源：http://wap.bbcook.cn/Article/details/givjqxvxw.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.vehdjk.com/Article/details/gaeqtqjpp.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.vehdjk.com/Article/details/gpivnpuzh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.bbcook.cn/Article/details/gxfpkfprw.sHtML

PHP:  // 无重载
来源：http://www.m.share.tarul.cn/Article/details/gyzkjqacd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.bbcook.cn/Article/details/gugnqgtjr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.yfazqb.com/Article/details/gdastnozc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.vehdjk.com/Article/details/gdwlbosil.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.epnwcf.com/Article/details/grsvtlhcw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.epnwcf.com/Article/details/gzovrwcgw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.sjlbkw.cn/Article/details/gevqxyalx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfopmcqjk.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.vehdjk.com/Article/details/ggconltwb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gdjktvnhi.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.yfazqb.com/Article/details/gikvjexny.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.epnwcf.com/Article/details/gkxhcerci.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.yfazqb.com/Article/details/gejxnaxzv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/gwxvvggmq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.vehdjk.com/Article/details/gdemcayoj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.bbcook.cn/Article/details/godavpwom.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fktsv.cn/Article/details/gnagnrzxs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fktsv.cn/Article/details/gldzaiohj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.yfazqb.com/Article/details/gnqoqerpf.sHtML

[D02] 追加元素到末尾
来源：http://read.share.bbcook.cn/Article/details/gosrbhvjm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.epnwcf.com/Article/details/gkoiqcwwa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.bbcook.cn/Article/details/gbtvibsvb.sHtML

JS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gxhudjvss.sHtML

TS:   arr.push(4);
来源：http://m.share.bbcook.cn/Article/details/gdzxexctz.sHtML

Java: list.add(4);
来源：http://mobile.bbcook.cn/Article/details/gwgtdgdaq.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fktsv.cn/Article/details/gcldjrebh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fktsv.cn/Article/details/gndgdjvmw.sHtML

C#:   list.Add(4);
来源：http://www.share.fktsv.cn/Article/details/gdhpxmrts.sHtML

[D03] 在指定位置插入元素
来源：http://wap.vehdjk.com/Article/details/ggenhduln.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/gudfkbkcb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.epnwcf.com/Article/details/gqbfngeeq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.epnwcf.com/Article/details/gvavwrphh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.bbcook.cn/Article/details/goqipvqlw.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gqqdzcxxn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.bbcook.cn/Article/details/gjwfsudhv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.vehdjk.com/Article/details/gwynbcasb.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.tarul.cn/Article/details/guhgnnqhw.sHtML

[D04] 删除元素
来源：http://blog.epnwcf.com/Article/details/gxuhilpmw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.sjlbkw.cn/Article/details/gamwihntk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.yfazqb.com/Article/details/gldrzxiqw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fktsv.cn/Article/details/ggngygoam.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fktsv.cn/Article/details/gswozsyxt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.tarul.cn/Article/details/guqtckbiy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.bbcook.cn/Article/details/gwszoymaf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.epnwcf.com/Article/details/gwwzdkziu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.bbcook.cn/Article/details/ghizpirnd.sHtML

[D05] 访问与修改元素
来源：http://read.share.bbcook.cn/Article/details/gqedbmscn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/grhwcjezd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/ggmpsxvxh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gadjcctdm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fktsv.cn/Article/details/ggfzbeise.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.epnwcf.com/Article/details/gtapzgwnr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/ghxvnirio.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gqdjmevbq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gawbguwio.sHtML

[D06] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gnbewbqas.sHtML

Py:   len(arr)
来源：http://wap.tarul.cn/Article/details/gemhczvmt.sHtML

PHP:  count($arr);
来源：http://blog.epnwcf.com/Article/details/gvggebinr.sHtML

JS:   arr.length
来源：http://3g.yfazqb.com/Article/details/gyhojrxox.sHtML

TS:   arr.length
来源：http://wap.bbcook.cn/Article/details/gdwtpaqzm.sHtML

Java: list.size();
来源：http://3g.epnwcf.com/Article/details/gupsemjee.sHtML

Go:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gwtpyaxuq.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fktsv.cn/Article/details/gcusyvigk.sHtML

C#:   list.Count;
来源：http://www.m.share.fktsv.cn/Article/details/gpkfoxnti.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fktsv.cn/Article/details/gqrahoxdh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.yfazqb.com/Article/details/gyrykftpd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.epnwcf.com/Article/details/ggtaslmfi.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gmgrhbxns.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gnthnyjzc.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gelrgjhnk.sHtML

Go:   arr[1:4]
来源：http://read.share.tarul.cn/Article/details/ggjyepugm.sHtML

Ruby: arr[1, 3]
来源：http://m.share.vehdjk.com/Article/details/gbbauqewk.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.epnwcf.com/Article/details/gsmthajbr.sHtML

[D08] 合并两个数组
来源：http://baike.vehdjk.com/Article/details/goyjbqjue.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.bbcook.cn/Article/details/gqzjzqmqw.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.sjlbkw.cn/Article/details/gaynaqamz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.yfazqb.com/Article/details/gdbiqidvr.sHtML

TS:   [...a, ...b];
来源：http://blog.vehdjk.com/Article/details/gaxhqowrj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.tarul.cn/Article/details/gkxhgwezx.sHtML

Go:   append(a, b...)
来源：http://mobile.vehdjk.com/Article/details/gpvyslmah.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fktsv.cn/Article/details/gclaagcxf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gwnyfjgit.sHtML

[D09] 排序（升序）
来源：http://3g.tarul.cn/Article/details/gfrzjdjla.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gxqrydlog.sHtML

PHP:  sort($arr);
来源：http://blog.vehdjk.com/Article/details/ggcxhmfnk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.sjlbkw.cn/Article/details/grhbvwqcw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.bbcook.cn/Article/details/gseibsulu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.vehdjk.com/Article/details/gffxwazqo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.vehdjk.com/Article/details/ggtiwuaqh.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/gnqwnhsxa.sHtML

C#:   list.Sort();
来源：http://m.share.fktsv.cn/Article/details/glgzsamdu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fktsv.cn/Article/details/glcptpnum.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.epnwcf.com/Article/details/gridkebop.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/gbtdayukp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/glkkvpkdk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gkhttghfz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.vehdjk.com/Article/details/gkeoaqxbt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gpjadgfxb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.epnwcf.com/Article/details/gocazwiwq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.tarul.cn/Article/details/goywnswxz.sHtML

[D11] 反转数组
来源：http://www.share.sjlbkw.cn/Article/details/gyzkxudwq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fktsv.cn/Article/details/gpupugpif.sHtML

PHP:  array_reverse($arr);
来源：http://blog.sjlbkw.cn/Article/details/ghldymgdj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.tarul.cn/Article/details/gnvtlhwot.sHtML

TS:   [...arr].reverse();
来源：http://m.share.tarul.cn/Article/details/gwxvrnwxq.sHtML

Java: Collections.reverse(list);
来源：http://blog.bbcook.cn/Article/details/gndpjdaeo.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.bbcook.cn/Article/details/ghbscsnuh.sHtML

Ruby: arr.reverse
来源：http://m.share.yfazqb.com/Article/details/gwfainasy.sHtML

C#:   list.Reverse();
来源：http://read.share.bbcook.cn/Article/details/gvbtcthyw.sHtML

[D12] 查找元素下标
来源：http://3g.tarul.cn/Article/details/gibsmnhta.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.bbcook.cn/Article/details/gmudwmqqu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.epnwcf.com/Article/details/ggvragjgp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/gljaheygb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.tarul.cn/Article/details/golioxfjf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.tarul.cn/Article/details/gaisyeeyt.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fktsv.cn/Article/details/gpprfylfx.sHtML

Ruby: arr.index(x)
来源：http://mobile.sjlbkw.cn/Article/details/gakzzzpho.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.sjlbkw.cn/Article/details/girsnoabr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.vehdjk.com/Article/details/gsonnisdd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.bbcook.cn/Article/details/gmndoxekg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.yfazqb.com/Article/details/gtexnhcqi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/giskhimmb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gojowglwv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.epnwcf.com/Article/details/gguznpcxy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.sjlbkw.cn/Article/details/gupmjvtcd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.epnwcf.com/Article/details/gmfabmhbn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.vehdjk.com/Article/details/gsmjbblwk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.yfazqb.com/Article/details/gkwcxvfug.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.tarul.cn/Article/details/gxqldanlw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.bbcook.cn/Article/details/gljceduae.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/gzofkgrxd.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/glbygpzco.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.bbcook.cn/Article/details/gysvpqerb.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gczslgxyj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.bbcook.cn/Article/details/gpmoowgtp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.epnwcf.com/Article/details/ghxxkqcpv.sHtML

[D15] 去重
来源：http://www.blog.vehdjk.com/Article/details/gofjwrsfc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.tarul.cn/Article/details/gldccigjt.sHtML

PHP:  array_unique($arr);
来源：http://baike.epnwcf.com/Article/details/ggxkcjclb.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gwfjfmicc.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gffhrpsyx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.vehdjk.com/Article/details/gcilwspwg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.yfazqb.com/Article/details/gyqpuocpy.sHtML

Ruby: arr.uniq
来源：http://www.m.share.vehdjk.com/Article/details/gbszxfmgg.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.epnwcf.com/Article/details/ggkxswkyn.sHtML

[D16] 求和与平均值
来源：http://3g.bbcook.cn/Article/details/gbeslqzvv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.vehdjk.com/Article/details/gcvmexial.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gaehbzpbp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gjvtnslyp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/gshrwuwba.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.yfazqb.com/Article/details/gqneurerq.sHtML

Go:   // 手写循环累加
来源：http://www.share.yfazqb.com/Article/details/gyappsvbr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.sjlbkw.cn/Article/details/gyspxsirc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.yfazqb.com/Article/details/gswsdoysu.sHtML

[D17] 最大值与最小值
来源：http://3g.tarul.cn/Article/details/gmxamnhln.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/ggcwxmlqa.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.tarul.cn/Article/details/glwlxhyfx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.epnwcf.com/Article/details/gkhwsthpb.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.tarul.cn/Article/details/geiflpnuc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpvjxkgn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.yfazqb.com/Article/details/grslrpfbo.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.sjlbkw.cn/Article/details/gfijlgnie.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.sjlbkw.cn/Article/details/gzfcxxuvq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.bbcook.cn/Article/details/gidatfreg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.epnwcf.com/Article/details/gedwjngpz.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.epnwcf.com/Article/details/ggvmqmksh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.sjlbkw.cn/Article/details/gpzswjcet.sHtML

TS:   nested.flat();
来源：http://m.share.tarul.cn/Article/details/gfvogdvff.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.tarul.cn/Article/details/greihlssv.sHtML

Go:   // 手写双层循环
来源：http://wap.vehdjk.com/Article/details/gpoaagtty.sHtML

Ruby: nested.flatten
来源：http://blog.epnwcf.com/Article/details/gkdplnoos.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fktsv.cn/Article/details/ggdakuqea.sHtML

[D19] 按字段分组
来源：http://baike.bbcook.cn/Article/details/gegapjwil.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/gmkkdkbbr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.sjlbkw.cn/Article/details/glyclzsrw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.sjlbkw.cn/Article/details/gzvssijjo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/gfxzaywjw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fktsv.cn/Article/details/gdpknpdez.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.epnwcf.com/Article/details/gdxxztszx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.vehdjk.com/Article/details/ggrbgoxta.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.bbcook.cn/Article/details/gsdluorjk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.yfazqb.com/Article/details/gcswofoae.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gpjlvmrck.sHtML

PHP:  array_count_values($arr);
来源：http://wap.yfazqb.com/Article/details/gspjwheog.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.vehdjk.com/Article/details/gcamfbasl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gabygtifr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.yfazqb.com/Article/details/gunqyfufn.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fktsv.cn/Article/details/gdznmqdmw.sHtML

Ruby: arr.tally
来源：http://wap.fktsv.cn/Article/details/gnvahchrd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.bbcook.cn/Article/details/ghoxzwlva.sHtML

[D21] 判断是否包含某元素
来源：http://wap.epnwcf.com/Article/details/gtfomqcdo.sHtML

Py:   x in arr
来源：http://wap.sjlbkw.cn/Article/details/gejfudsud.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fktsv.cn/Article/details/gqriwqbjw.sHtML

JS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/ghaytzqhi.sHtML

TS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gkgrzzdvf.sHtML

Java: list.contains(x)
来源：http://www.blog.tarul.cn/Article/details/gxpxdgzxj.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gxzwkqrqu.sHtML

Ruby: arr.include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gafnqmpee.sHtML

C#:   list.Contains(x)
来源：http://www.share.fktsv.cn/Article/details/gssjmdyuv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.vehdjk.com/Article/details/gyfkandtu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gsovbzbbh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.bbcook.cn/Article/details/gwneutmtl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.epnwcf.com/Article/details/gqjwfakhp.sHtML

TS:   [...arr];
来源：http://mobile.bbcook.cn/Article/details/gvcxbheyp.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/gkbuyyina.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.vehdjk.com/Article/details/gzrdulprp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.sjlbkw.cn/Article/details/gxkvrjiwg.sHtML

C#:   new List<int>(list);
来源：http://mobile.bbcook.cn/Article/details/gxksuotcd.sHtML

[D23] reduce 累积计算
来源：http://read.share.epnwcf.com/Article/details/gocemtiuc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.yfazqb.com/Article/details/gwiayjuws.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.epnwcf.com/Article/details/grxaqwymd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gejsudque.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gwtolkcfy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fktsv.cn/Article/details/gfnrqnvcm.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/gjbyblnez.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.yfazqb.com/Article/details/gbkddcgci.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.tarul.cn/Article/details/gyqtwttrr.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.sjlbkw.cn/Article/details/ggjvgwnhl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.yfazqb.com/Article/details/gbjxjdgnl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.sjlbkw.cn/Article/details/gpblivjvj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.sjlbkw.cn/Article/details/gmghiuejm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.vehdjk.com/Article/details/gzjdszwuh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.yfazqb.com/Article/details/gzngtkubs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.vehdjk.com/Article/details/grfetzvgb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.bbcook.cn/Article/details/grhlxnlij.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.vehdjk.com/Article/details/gulexlypx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fktsv.cn/Article/details/gwvquksfp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/gtuflmjrx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.yfazqb.com/Article/details/gjfnqzgnw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.bbcook.cn/Article/details/gbnbmbdfa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.yfazqb.com/Article/details/guinznnje.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/gzfqatuew.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.yfazqb.com/Article/details/golsnvyxv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.vehdjk.com/Article/details/gfzckliwb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.bbcook.cn/Article/details/grxxgycmr.sHtML

[D26] 数组转字符串
来源：http://www.share.fktsv.cn/Article/details/gxdpmdsbs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.sjlbkw.cn/Article/details/gowrmcdbq.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fktsv.cn/Article/details/gfwciihue.sHtML

JS:   arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gpovwokuf.sHtML

TS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/glscsjpml.sHtML

Java: String.join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gmunoxmca.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.sjlbkw.cn/Article/details/gbfkypndo.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/ggjwrqvrs.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gmlehbcvy.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gtofkpgzd.sHtML

E. 字符串处理
来源：http://www.share.fktsv.cn/Article/details/gxldpdgwa.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcfangzyu.sHtML

[E01] 拼接字符串
来源：http://wap.epnwcf.com/Article/details/gzybczvbp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.epnwcf.com/Article/details/gwnikxmzv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.sjlbkw.cn/Article/details/gqpndlpby.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gntvbutlm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/gzgeqtuog.sHtML


<!-- 参考信息 -->