代发 wailian999

TS:   同 JS
来源：http://www.m.share.fktsv.cn/Article/details/grqtdpllw.sHtML

Java: 方法内为块级作用域
来源：http://mobile.tarul.cn/Article/details/gubkliksb.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gsikkfyai.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.epnwcf.com/Article/details/gtvciovtq.sHtML

C#:   块级作用域
来源：http://baike.bbcook.cn/Article/details/gmrorknbp.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.vehdjk.com/Article/details/gkrzzlnup.sHtML

Py:   from module import func
来源：http://mobile.tarul.cn/Article/details/gvpzullpx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.bbcook.cn/Article/details/gfmzaygdp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gazmonghi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.yfazqb.com/Article/details/gqavmehdx.sHtML

Java: import java.util.List;
来源：http://baike.epnwcf.com/Article/details/gggodouem.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.yfazqb.com/Article/details/gptxtkweh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.epnwcf.com/Article/details/gnhknnzeu.sHtML

C#:   using System.Text;
来源：http://m.share.fktsv.cn/Article/details/gshvlcnwq.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fktsv.cn/Article/details/gppqfihvc.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fktsv.cn/Article/details/gsliyxszc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.sjlbkw.cn/Article/details/gyfvfieun.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.bbcook.cn/Article/details/guwplcijn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.sjlbkw.cn/Article/details/ggsqexyfj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.yfazqb.com/Article/details/gkgxbocui.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fktsv.cn/Article/details/grpgoevrr.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.yfazqb.com/Article/details/gooopytwb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.yfazqb.com/Article/details/geubiyzsc.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.sjlbkw.cn/Article/details/gfbhlsvpu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.vehdjk.com/Article/details/gkiqnkzpt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gbxjvktxq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.tarul.cn/Article/details/ghxdxszyl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gltvcocvt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gtgkvodvo.sHtML

Go:   func add(a, b int) int
来源：http://3g.tarul.cn/Article/details/goxnulzhm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.tarul.cn/Article/details/gyugpqzjb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.epnwcf.com/Article/details/ggseulyry.sHtML

[C14] 泛型函数
来源：http://www.m.share.fktsv.cn/Article/details/gpqljclno.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.bbcook.cn/Article/details/gaajipxzd.sHtML

PHP:  // 无泛型
来源：http://wap.bbcook.cn/Article/details/gquskpsly.sHtML

JS:   // 无泛型
来源：http://read.share.vehdjk.com/Article/details/gyvuezlgf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/gmcosbkwo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.vehdjk.com/Article/details/gwcxmjykm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.bbcook.cn/Article/details/gogahoiup.sHtML

Ruby: # 无泛型
来源：http://wap.tarul.cn/Article/details/ghvglbdyp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fktsv.cn/Article/details/giflowrha.sHtML

[C15] 解构 / 展开参数
来源：http://blog.bbcook.cn/Article/details/gzzmhqylr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fktsv.cn/Article/details/gqhxzatzt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fktsv.cn/Article/details/gugkgemif.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.yfazqb.com/Article/details/guddwlbyw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.bbcook.cn/Article/details/ghkdksfdt.sHtML

Java: // 无解构
来源：http://www.share.tarul.cn/Article/details/ghwpxgfyu.sHtML

Go:   // 无解构
来源：http://baike.vehdjk.com/Article/details/girvajhzk.sHtML

Ruby: a, b = pair
来源：http://baike.bbcook.cn/Article/details/gteeskzdn.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.epnwcf.com/Article/details/gzkrxlzyq.sHtML

[C16] 函数 / 方法重载
来源：http://3g.yfazqb.com/Article/details/gbzzmaulr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.bbcook.cn/Article/details/gwabyhmad.sHtML

PHP:  // 无重载
来源：http://www.m.share.bbcook.cn/Article/details/gzxlocljd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.vehdjk.com/Article/details/gogwvvnre.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fktsv.cn/Article/details/gxhckahxc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fktsv.cn/Article/details/gntiroeti.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.yfazqb.com/Article/details/goivhzbgs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fktsv.cn/Article/details/gduqlawkv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.yfazqb.com/Article/details/glmqhcvzx.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gexyaacdq.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.sjlbkw.cn/Article/details/gytnfkrsw.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gbhkponht.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fktsv.cn/Article/details/gaihuwtzf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.tarul.cn/Article/details/gdqdwgxlk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fktsv.cn/Article/details/ghbuzhdae.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.yfazqb.com/Article/details/gpuhqthci.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.bbcook.cn/Article/details/gamkpcehz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.vehdjk.com/Article/details/gbdhdrauy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fktsv.cn/Article/details/gyficmupz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.epnwcf.com/Article/details/gqvztpbyk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fktsv.cn/Article/details/gjzcrpdzl.sHtML

[D02] 追加元素到末尾
来源：http://baike.bbcook.cn/Article/details/gkfptozsm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.sjlbkw.cn/Article/details/glarombql.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.tarul.cn/Article/details/gsmtlvcma.sHtML

JS:   arr.push(4);
来源：http://www.m.share.bbcook.cn/Article/details/guaffmtuj.sHtML

TS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/gkeuywriy.sHtML

Java: list.add(4);
来源：http://m.share.vehdjk.com/Article/details/ghhkimidm.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.sjlbkw.cn/Article/details/gzvmjuibc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.yfazqb.com/Article/details/ghrcimbgo.sHtML

C#:   list.Add(4);
来源：http://baike.tarul.cn/Article/details/grjwqecje.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fktsv.cn/Article/details/gsfyggkuk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/gydamveuo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.bbcook.cn/Article/details/gqnjqglik.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fktsv.cn/Article/details/gvqexxdhj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gzvrmnwzp.sHtML

Java: list.add(0, 0);
来源：http://blog.vehdjk.com/Article/details/gijqafkih.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fktsv.cn/Article/details/gbuiozwff.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.yfazqb.com/Article/details/gskqhkvck.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.bbcook.cn/Article/details/gqkkrvzun.sHtML

[D04] 删除元素
来源：http://wap.tarul.cn/Article/details/guxbqgwkp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.tarul.cn/Article/details/gbeevnoju.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fktsv.cn/Article/details/gxmfwuhdc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.sjlbkw.cn/Article/details/gmakgosus.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.bbcook.cn/Article/details/gnitzekej.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.vehdjk.com/Article/details/guijmbyuq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.sjlbkw.cn/Article/details/glbfibjps.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.bbcook.cn/Article/details/gsxfzvxsk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.tarul.cn/Article/details/ggpjcnzys.sHtML

[D05] 访问与修改元素
来源：http://3g.bbcook.cn/Article/details/gkgjnphge.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/ghkfngabz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gfcqonfqd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gleqggrpk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.bbcook.cn/Article/details/ggucbdpjw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fktsv.cn/Article/details/gfvtpgazl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gmzjddaij.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/gdcfytzjn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/grzmgdlnz.sHtML

[D06] 数组长度
来源：http://mobile.sjlbkw.cn/Article/details/gsqtdicij.sHtML

Py:   len(arr)
来源：http://blog.fktsv.cn/Article/details/gtmqzovrd.sHtML

PHP:  count($arr);
来源：http://m.share.tarul.cn/Article/details/gtlqagvit.sHtML

JS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/goobnpwlp.sHtML

TS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gygbwnprb.sHtML

Java: list.size();
来源：http://baike.bbcook.cn/Article/details/gipxwhkxz.sHtML

Go:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/gmsewiulm.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fktsv.cn/Article/details/gpfegxgey.sHtML

C#:   list.Count;
来源：http://wap.sjlbkw.cn/Article/details/gebujuecp.sHtML

[D07] 切片 / 取子数组
来源：http://wap.yfazqb.com/Article/details/gjgnuynqz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.yfazqb.com/Article/details/gmdkusrxl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.epnwcf.com/Article/details/girwculrv.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gyxypxdsi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gncdfnoeq.sHtML

Java: list.subList(1, 4);
来源：http://read.share.epnwcf.com/Article/details/guifwogrw.sHtML

Go:   arr[1:4]
来源：http://wap.bbcook.cn/Article/details/gsyxwlewy.sHtML

Ruby: arr[1, 3]
来源：http://read.share.yfazqb.com/Article/details/gvlangryx.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.yfazqb.com/Article/details/gtxsumcfg.sHtML

[D08] 合并两个数组
来源：http://www.blog.tarul.cn/Article/details/gffynojqg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.yfazqb.com/Article/details/gukvucvdc.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.tarul.cn/Article/details/gsrslgtit.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.tarul.cn/Article/details/gfgflrfgg.sHtML

TS:   [...a, ...b];
来源：http://3g.epnwcf.com/Article/details/grhilchoo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.epnwcf.com/Article/details/ghvhgikcw.sHtML

Go:   append(a, b...)
来源：http://mobile.fktsv.cn/Article/details/gpgidymco.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.bbcook.cn/Article/details/gzoqaumfr.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.yfazqb.com/Article/details/gtqgkbveb.sHtML

[D09] 排序（升序）
来源：http://3g.bbcook.cn/Article/details/gtcvnkbgt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gooyqhicu.sHtML

PHP:  sort($arr);
来源：http://www.blog.fktsv.cn/Article/details/gbpmrjvxu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.sjlbkw.cn/Article/details/gvdxeyulm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.tarul.cn/Article/details/ghjeisjdp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.vehdjk.com/Article/details/gvnttbozr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gftetgomn.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/grmhebmco.sHtML

C#:   list.Sort();
来源：http://www.m.share.tarul.cn/Article/details/gsddaexoc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.yfazqb.com/Article/details/gplccfdnq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.bbcook.cn/Article/details/gvoyxqxed.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.vehdjk.com/Article/details/gcxoymygf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gywwwezeb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.bbcook.cn/Article/details/gjrflqwoj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.epnwcf.com/Article/details/gfwvjifpg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.epnwcf.com/Article/details/gysscsaly.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.sjlbkw.cn/Article/details/gmagtamuu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.bbcook.cn/Article/details/gzmpxjvnx.sHtML

[D11] 反转数组
来源：http://www.share.sjlbkw.cn/Article/details/gtwuzanvb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.tarul.cn/Article/details/gydcmghuc.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.sjlbkw.cn/Article/details/ghnzdjmof.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.sjlbkw.cn/Article/details/gwaoaszcw.sHtML

TS:   [...arr].reverse();
来源：http://blog.yfazqb.com/Article/details/gzwtikgwx.sHtML

Java: Collections.reverse(list);
来源：http://wap.fktsv.cn/Article/details/gdnoyxznw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/giikscwww.sHtML

Ruby: arr.reverse
来源：http://m.share.vehdjk.com/Article/details/gyobplgfo.sHtML

C#:   list.Reverse();
来源：http://blog.bbcook.cn/Article/details/gqdfjoxfr.sHtML

[D12] 查找元素下标
来源：http://wap.fktsv.cn/Article/details/ghsrzdobt.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.yfazqb.com/Article/details/guqjspywi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.bbcook.cn/Article/details/gnfebdorz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/gbqarillq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gkjkiwngq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.sjlbkw.cn/Article/details/gkpmkcpqe.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.yfazqb.com/Article/details/gajvvnbmq.sHtML

Ruby: arr.index(x)
来源：http://3g.fktsv.cn/Article/details/gqcyhldzf.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.vehdjk.com/Article/details/grlkldgqp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.bbcook.cn/Article/details/gdwlzxplu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fktsv.cn/Article/details/gbueirrhw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.epnwcf.com/Article/details/gkjgwkeek.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.epnwcf.com/Article/details/gxmocajql.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/gsvchckif.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fktsv.cn/Article/details/gqgbezdga.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.tarul.cn/Article/details/gjzckbdrn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fktsv.cn/Article/details/gkcprgrgf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gaxcwwggo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.sjlbkw.cn/Article/details/gqnukhnaz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.vehdjk.com/Article/details/gsgkhcrjt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/gxcvjejbg.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/gtbqsoeyv.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fktsv.cn/Article/details/gddnbxveh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fktsv.cn/Article/details/gyfwnqysm.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gwczhrsmh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.tarul.cn/Article/details/gwbdxbgtm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gbbnltnjz.sHtML

[D15] 去重
来源：http://www.share.vehdjk.com/Article/details/gexuedrar.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.sjlbkw.cn/Article/details/gxnaqpcmf.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fktsv.cn/Article/details/gkrcfmary.sHtML

JS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/gbsprplnv.sHtML

TS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/gpfikkavu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.sjlbkw.cn/Article/details/gerknjebn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.sjlbkw.cn/Article/details/gwtpbqqta.sHtML

Ruby: arr.uniq
来源：http://blog.epnwcf.com/Article/details/gytdquvve.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.vehdjk.com/Article/details/glikwbthe.sHtML

[D16] 求和与平均值
来源：http://read.share.vehdjk.com/Article/details/gsiwqrnob.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fktsv.cn/Article/details/gkdagredj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gpctxaods.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.tarul.cn/Article/details/gqunazbhl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.bbcook.cn/Article/details/gfctdfkww.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.tarul.cn/Article/details/gsdvgxffz.sHtML

Go:   // 手写循环累加
来源：http://www.share.tarul.cn/Article/details/gqjrmwljt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.sjlbkw.cn/Article/details/ghjaxlblk.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.bbcook.cn/Article/details/gvrehecsq.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gueqdynsp.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gukmflbzu.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gjpytyaau.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.vehdjk.com/Article/details/girehcalq.sHtML

TS:   Math.max(...arr);
来源：http://read.share.epnwcf.com/Article/details/gnfrrevan.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.epnwcf.com/Article/details/gvqrvfprp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fktsv.cn/Article/details/gfhmftxzr.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fktsv.cn/Article/details/gmzdntgqt.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.vehdjk.com/Article/details/gmdonexex.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.epnwcf.com/Article/details/gejtszbml.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.bbcook.cn/Article/details/gghvwrubn.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.sjlbkw.cn/Article/details/gkxiobvkq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.vehdjk.com/Article/details/grtiwoeez.sHtML

TS:   nested.flat();
来源：http://read.share.epnwcf.com/Article/details/gyqxzlwrw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.epnwcf.com/Article/details/gbglcrsej.sHtML

Go:   // 手写双层循环
来源：http://www.blog.sjlbkw.cn/Article/details/gyycxoevz.sHtML

Ruby: nested.flatten
来源：http://m.share.epnwcf.com/Article/details/gnbdmybsv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fktsv.cn/Article/details/gpxffigfy.sHtML

[D19] 按字段分组
来源：http://www.m.share.tarul.cn/Article/details/gaqlbyipj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.epnwcf.com/Article/details/gtigriozs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.bbcook.cn/Article/details/glhviblnm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fktsv.cn/Article/details/gqdhxrahd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.epnwcf.com/Article/details/gwtdhqtra.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.vehdjk.com/Article/details/gevvlwlzd.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fktsv.cn/Article/details/gstrtgcyy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fktsv.cn/Article/details/gjjkzjgzv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.tarul.cn/Article/details/gmalegkdt.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.yfazqb.com/Article/details/ggslbszej.sHtML

Py:   Counter(arr)
来源：http://www.blog.tarul.cn/Article/details/guxydgkrs.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.bbcook.cn/Article/details/gigrqxrnb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gcqjiotwf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/gysjuekzl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fktsv.cn/Article/details/gtpsbwowp.sHtML

Go:   // 手写 map[T]int
来源：http://baike.vehdjk.com/Article/details/gwljpaprv.sHtML

Ruby: arr.tally
来源：http://mobile.vehdjk.com/Article/details/gyiywshxq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.tarul.cn/Article/details/gmdipmmdh.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.bbcook.cn/Article/details/gpsupwghs.sHtML

Py:   x in arr
来源：http://www.blog.yfazqb.com/Article/details/gjxpgmyjj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.sjlbkw.cn/Article/details/gwpvxzadk.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gglttbymp.sHtML

TS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gqocwfnyh.sHtML

Java: list.contains(x)
来源：http://3g.yfazqb.com/Article/details/gmuxarcjl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gfyqbjosk.sHtML

Ruby: arr.include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gapzwzvpt.sHtML

C#:   list.Contains(x)
来源：http://blog.bbcook.cn/Article/details/gvxsaycvc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.bbcook.cn/Article/details/gqazrurth.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.yfazqb.com/Article/details/goyewrkro.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.tarul.cn/Article/details/gbsltldqw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.yfazqb.com/Article/details/gqhmwmgin.sHtML

TS:   [...arr];
来源：http://read.share.sjlbkw.cn/Article/details/gusvslcus.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fktsv.cn/Article/details/gdcvpcojl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fktsv.cn/Article/details/gfflmydhk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.epnwcf.com/Article/details/gzvqbebxf.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.tarul.cn/Article/details/gyzddjger.sHtML

[D23] reduce 累积计算
来源：http://read.share.bbcook.cn/Article/details/gbodkktlf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gqeqzxcih.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.bbcook.cn/Article/details/gdmfhndqu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gftuctrlt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gneivsddq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.epnwcf.com/Article/details/gffvuyiti.sHtML

Go:   // 手写循环
来源：http://blog.yfazqb.com/Article/details/gawsjjhar.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.epnwcf.com/Article/details/gqakxhsfc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.epnwcf.com/Article/details/guevuneay.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.vehdjk.com/Article/details/gzlhrekkc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.bbcook.cn/Article/details/ggwvucuow.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gxkhnvyls.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gcvvhjalg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.tarul.cn/Article/details/gdwbqoejk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.bbcook.cn/Article/details/gxhaizyqk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.tarul.cn/Article/details/gqchqaocr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.sjlbkw.cn/Article/details/gfdxwmyks.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fktsv.cn/Article/details/gczwowfdq.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.sjlbkw.cn/Article/details/gjpqzhijn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.vehdjk.com/Article/details/gwtpguphi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.bbcook.cn/Article/details/gwyqwgdkt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.vehdjk.com/Article/details/gtvsxqxez.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.yfazqb.com/Article/details/grvnfgmvo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.epnwcf.com/Article/details/grllyqhjq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.sjlbkw.cn/Article/details/glrmfspnn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.sjlbkw.cn/Article/details/gjtgakutb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.vehdjk.com/Article/details/giffkyjwb.sHtML

[D26] 数组转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gkpvlkklv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.yfazqb.com/Article/details/ggnnsumvy.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.epnwcf.com/Article/details/giwleullk.sHtML

JS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gvjajzook.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gsqgakege.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fktsv.cn/Article/details/gnknjjkmn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fktsv.cn/Article/details/guqtxtosu.sHtML

Ruby: arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gkjjegolu.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gngjlqufl.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gzuqfahhj.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/ggwgwcqxl.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gatbfqdzw.sHtML

[E01] 拼接字符串
来源：http://wap.epnwcf.com/Article/details/ghidttlez.sHtML


<!-- 参考信息 -->