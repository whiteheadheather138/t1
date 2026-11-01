代发 wailian999

[C10] 变量作用域
来源：http://read.share.vehdjk.com/Article/details/gqrtiejar.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.yfazqb.com/Article/details/gludaiice.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.epnwcf.com/Article/details/gtdkofurw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.bbcook.cn/Article/details/gjwkaxksc.sHtML

TS:   同 JS
来源：http://blog.vehdjk.com/Article/details/ghqtivrbv.sHtML

Java: 方法内为块级作用域
来源：http://read.share.yfazqb.com/Article/details/gerfrkeds.sHtML

Go:   花括号块级作用域
来源：http://3g.fktsv.cn/Article/details/gxvwciqsu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.vehdjk.com/Article/details/glqofauql.sHtML

C#:   块级作用域
来源：http://3g.vehdjk.com/Article/details/gkbgvpsql.sHtML

[C11] 模块导入与导出
来源：http://m.share.sjlbkw.cn/Article/details/gtkdpfgkd.sHtML

Py:   from module import func
来源：http://blog.vehdjk.com/Article/details/gdqqijwsa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fktsv.cn/Article/details/gbxuwwuqi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fktsv.cn/Article/details/gcsojclmw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fktsv.cn/Article/details/ggxpwtwlu.sHtML

Java: import java.util.List;
来源：http://wap.bbcook.cn/Article/details/girftlirc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.vehdjk.com/Article/details/goltvvlmn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fktsv.cn/Article/details/gusiefiml.sHtML

C#:   using System.Text;
来源：http://www.m.share.tarul.cn/Article/details/gwfkozjal.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.tarul.cn/Article/details/grllclfkp.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.tarul.cn/Article/details/gilkwrumn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.vehdjk.com/Article/details/gzigvrbyd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/gvjmlljqj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/gjtzpppxl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.bbcook.cn/Article/details/gqvtfgwfs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fktsv.cn/Article/details/gtytkzizy.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.bbcook.cn/Article/details/gbpklwwkm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.vehdjk.com/Article/details/ggyyahhai.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.epnwcf.com/Article/details/gvzbzkjww.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fktsv.cn/Article/details/ggfiszake.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gbmaebhdk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fktsv.cn/Article/details/gysgbhynt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gwymcvhzk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gedmtuhiv.sHtML

Go:   func add(a, b int) int
来源：http://baike.vehdjk.com/Article/details/gvczvyfgb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.tarul.cn/Article/details/gfavtmnya.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.bbcook.cn/Article/details/gljarrejq.sHtML

[C14] 泛型函数
来源：http://www.m.share.bbcook.cn/Article/details/glxvydmhj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fktsv.cn/Article/details/glxsvmdvb.sHtML

PHP:  // 无泛型
来源：http://wap.epnwcf.com/Article/details/gdmvsmgay.sHtML

JS:   // 无泛型
来源：http://mobile.vehdjk.com/Article/details/gxsjgyfew.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.vehdjk.com/Article/details/glnkkjnqc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.vehdjk.com/Article/details/gdmljhodf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.epnwcf.com/Article/details/ghznxkego.sHtML

Ruby: # 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gcdogwysr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.yfazqb.com/Article/details/gtmuythth.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.vehdjk.com/Article/details/gmccrtdjs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.sjlbkw.cn/Article/details/gfomtecbz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.tarul.cn/Article/details/gvivwnhrj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gnjxwsdsl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.sjlbkw.cn/Article/details/gyebgfbtq.sHtML

Java: // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/gvbsqpxbm.sHtML

Go:   // 无解构
来源：http://wap.tarul.cn/Article/details/geahskypa.sHtML

Ruby: a, b = pair
来源：http://blog.bbcook.cn/Article/details/gdfdvedwy.sHtML

C#:   var (a, b) = pair;
来源：http://3g.epnwcf.com/Article/details/gnhgxftho.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fktsv.cn/Article/details/gmtlpsgra.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.vehdjk.com/Article/details/gcraazqkn.sHtML

PHP:  // 无重载
来源：http://www.m.share.tarul.cn/Article/details/gvukiwxhq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.epnwcf.com/Article/details/gtvxhjuyi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.epnwcf.com/Article/details/ggdkkypte.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.yfazqb.com/Article/details/giyansdeg.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.bbcook.cn/Article/details/gtueinhgi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.vehdjk.com/Article/details/gjvtiigbb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.yfazqb.com/Article/details/gleqygimf.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gaqrbkwfd.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.bbcook.cn/Article/details/gxefxkqqv.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gcwkqdnfv.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.bbcook.cn/Article/details/gqsuvukvi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.vehdjk.com/Article/details/gngpdduhk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/geovznoyc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.epnwcf.com/Article/details/gqqneofya.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.yfazqb.com/Article/details/gpazcqygt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.vehdjk.com/Article/details/gcoylpidg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.yfazqb.com/Article/details/gvgerulod.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.vehdjk.com/Article/details/gqjrenrfs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.yfazqb.com/Article/details/gncksindw.sHtML

[D02] 追加元素到末尾
来源：http://wap.sjlbkw.cn/Article/details/gtvvufbij.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.epnwcf.com/Article/details/gjxtomjmh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.bbcook.cn/Article/details/gxnwlvanl.sHtML

JS:   arr.push(4);
来源：http://www.blog.yfazqb.com/Article/details/ggnfqzdph.sHtML

TS:   arr.push(4);
来源：http://3g.tarul.cn/Article/details/ghzlumcsu.sHtML

Java: list.add(4);
来源：http://baike.fktsv.cn/Article/details/gflqmwelc.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.epnwcf.com/Article/details/gewkxxqsa.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.sjlbkw.cn/Article/details/gyutbiujj.sHtML

C#:   list.Add(4);
来源：http://www.share.yfazqb.com/Article/details/gmynqzqcd.sHtML

[D03] 在指定位置插入元素
来源：http://blog.tarul.cn/Article/details/gnnqxqkaw.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.yfazqb.com/Article/details/gkhgataou.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.sjlbkw.cn/Article/details/grblyjfsq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.tarul.cn/Article/details/gpcnwpcpg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.yfazqb.com/Article/details/gsxkewufb.sHtML

Java: list.add(0, 0);
来源：http://mobile.vehdjk.com/Article/details/glghuavhd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.sjlbkw.cn/Article/details/gbjyxkemw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.epnwcf.com/Article/details/gpwgfmhvm.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.epnwcf.com/Article/details/gmrrcokgp.sHtML

[D04] 删除元素
来源：http://mobile.yfazqb.com/Article/details/gozdzkhhu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.vehdjk.com/Article/details/gmdgqvdov.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.vehdjk.com/Article/details/gsymvlidz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.yfazqb.com/Article/details/gljzazngp.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fktsv.cn/Article/details/gbxgolwxu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.yfazqb.com/Article/details/gbkemiomi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.vehdjk.com/Article/details/gdmlaulsk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.epnwcf.com/Article/details/goyfhhzli.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.bbcook.cn/Article/details/gbynkgiui.sHtML

[D05] 访问与修改元素
来源：http://blog.fktsv.cn/Article/details/guhrjgcpd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/griffoiqb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gspvbejhc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/goasyyqsd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.vehdjk.com/Article/details/gsxtxqbfb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.bbcook.cn/Article/details/groibkhco.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gtazhcjeh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gngsmocqa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gqcyoqtrz.sHtML

[D06] 数组长度
来源：http://m.share.bbcook.cn/Article/details/glwjtxczu.sHtML

Py:   len(arr)
来源：http://wap.vehdjk.com/Article/details/gqndxloyu.sHtML

PHP:  count($arr);
来源：http://blog.epnwcf.com/Article/details/gkniosotc.sHtML

JS:   arr.length
来源：http://www.share.epnwcf.com/Article/details/gtsvgakxw.sHtML

TS:   arr.length
来源：http://baike.bbcook.cn/Article/details/gvkvvoshl.sHtML

Java: list.size();
来源：http://blog.bbcook.cn/Article/details/gyjsfszvo.sHtML

Go:   len(arr)
来源：http://baike.fktsv.cn/Article/details/gpjjywcbs.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/ginqjwqfb.sHtML

C#:   list.Count;
来源：http://www.share.sjlbkw.cn/Article/details/gmywjkbgm.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fktsv.cn/Article/details/gliirewvf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.yfazqb.com/Article/details/gmmpfxqni.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gokewtwcs.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/glewmouwp.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gpkkrlfps.sHtML

Java: list.subList(1, 4);
来源：http://3g.yfazqb.com/Article/details/gcdgrusjp.sHtML

Go:   arr[1:4]
来源：http://blog.bbcook.cn/Article/details/gjevkljol.sHtML

Ruby: arr[1, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gjpqbhzar.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gwdduehar.sHtML

[D08] 合并两个数组
来源：http://read.share.bbcook.cn/Article/details/gjnojjcgd.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.yfazqb.com/Article/details/gjqikuxub.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.sjlbkw.cn/Article/details/gefbiagwc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.epnwcf.com/Article/details/gzhncljbm.sHtML

TS:   [...a, ...b];
来源：http://blog.yfazqb.com/Article/details/gwrltdazg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.yfazqb.com/Article/details/gppoxlfqm.sHtML

Go:   append(a, b...)
来源：http://www.share.fktsv.cn/Article/details/ghsqiamii.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.vehdjk.com/Article/details/gglfeyako.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.tarul.cn/Article/details/gjxpyborm.sHtML

[D09] 排序（升序）
来源：http://mobile.yfazqb.com/Article/details/gopyussor.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/gaxzwlici.sHtML

PHP:  sort($arr);
来源：http://m.share.fktsv.cn/Article/details/gzakgvfcs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.bbcook.cn/Article/details/gvyamiiym.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.bbcook.cn/Article/details/gtpykgfnt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.epnwcf.com/Article/details/gaylotgwd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gljoisfny.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gafddrhgj.sHtML

C#:   list.Sort();
来源：http://blog.fktsv.cn/Article/details/ggizjgkua.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.epnwcf.com/Article/details/gedsugotw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.tarul.cn/Article/details/gfparpruv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gaalavwey.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fktsv.cn/Article/details/gxrsntass.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqcmmabo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fktsv.cn/Article/details/gdkhunyuy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.epnwcf.com/Article/details/gccwworjr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.vehdjk.com/Article/details/gakrputpz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.tarul.cn/Article/details/gpvtsvnpg.sHtML

[D11] 反转数组
来源：http://read.share.bbcook.cn/Article/details/gtnzlbbha.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.yfazqb.com/Article/details/gpuoqerzw.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fktsv.cn/Article/details/gvyxdkmeu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.tarul.cn/Article/details/gzcadwyxl.sHtML

TS:   [...arr].reverse();
来源：http://baike.fktsv.cn/Article/details/gnudyoite.sHtML

Java: Collections.reverse(list);
来源：http://www.share.epnwcf.com/Article/details/gkhhdqayy.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fktsv.cn/Article/details/gskizpomn.sHtML

Ruby: arr.reverse
来源：http://blog.bbcook.cn/Article/details/glsjjrctz.sHtML

C#:   list.Reverse();
来源：http://baike.fktsv.cn/Article/details/glsjzrhse.sHtML

[D12] 查找元素下标
来源：http://wap.yfazqb.com/Article/details/gthjxzomd.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fktsv.cn/Article/details/gdsqdiiuq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/guoqrrvet.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.epnwcf.com/Article/details/gnsiaryfv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.bbcook.cn/Article/details/gtgvuqmcc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.bbcook.cn/Article/details/gptpdtgec.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.vehdjk.com/Article/details/gsybvfphy.sHtML

Ruby: arr.index(x)
来源：http://read.share.tarul.cn/Article/details/gearwauja.sHtML

C#:   list.IndexOf(x);
来源：http://blog.vehdjk.com/Article/details/gmadnwgiw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.tarul.cn/Article/details/gvuibkwux.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.bbcook.cn/Article/details/gsjilrrqt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.yfazqb.com/Article/details/guysdusur.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/gmibbksza.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/gkknsvmiy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gtnpxkhfo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.yfazqb.com/Article/details/gzrrkrjgv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.vehdjk.com/Article/details/gdggxkfry.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.tarul.cn/Article/details/ggppqgduv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.tarul.cn/Article/details/gyzzrdjft.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gqcnepmbs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.vehdjk.com/Article/details/gcokgvczs.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/gmrgyyswv.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/gnpyfsout.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.sjlbkw.cn/Article/details/genzpksfd.sHtML

Go:   // 手写循环
来源：http://3g.fktsv.cn/Article/details/gocvwoiam.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.tarul.cn/Article/details/guninyexx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.yfazqb.com/Article/details/gcusdrdpl.sHtML

[D15] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gjtjetfeo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fktsv.cn/Article/details/giqiklufy.sHtML

PHP:  array_unique($arr);
来源：http://m.share.vehdjk.com/Article/details/gdhrwwhzc.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gasyuuzzx.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/gsadqxzsu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.tarul.cn/Article/details/gunkycqzs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.tarul.cn/Article/details/gyyyioqtm.sHtML

Ruby: arr.uniq
来源：http://www.share.fktsv.cn/Article/details/gqkrgrbtr.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.yfazqb.com/Article/details/gjvvlhqpz.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/gvbdhgzgn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.yfazqb.com/Article/details/ghouwytcl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.yfazqb.com/Article/details/gsyujcvzv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gqwjinbtb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gqsygapgi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.yfazqb.com/Article/details/gymuwuwgc.sHtML

Go:   // 手写循环累加
来源：http://read.share.sjlbkw.cn/Article/details/gnorsvniy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fktsv.cn/Article/details/goretftuk.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.epnwcf.com/Article/details/gmjfhewmv.sHtML

[D17] 最大值与最小值
来源：http://www.blog.vehdjk.com/Article/details/gpbbqospj.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.tarul.cn/Article/details/gynibidlu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gpqjtrudj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fktsv.cn/Article/details/gywqjivpq.sHtML

TS:   Math.max(...arr);
来源：http://mobile.tarul.cn/Article/details/gcquraxlj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.tarul.cn/Article/details/gvaqwdyob.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.yfazqb.com/Article/details/gwrgdixck.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.epnwcf.com/Article/details/gagmsrxeq.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.epnwcf.com/Article/details/glstmhivz.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.bbcook.cn/Article/details/gyfhhbkrf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.sjlbkw.cn/Article/details/gxriqtzka.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.epnwcf.com/Article/details/gztdqftnk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.sjlbkw.cn/Article/details/gqfncuzlg.sHtML

TS:   nested.flat();
来源：http://baike.yfazqb.com/Article/details/glihxasun.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.bbcook.cn/Article/details/gbtjkesyk.sHtML

Go:   // 手写双层循环
来源：http://read.share.epnwcf.com/Article/details/gilqacgva.sHtML

Ruby: nested.flatten
来源：http://blog.fktsv.cn/Article/details/ggashbeuy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.epnwcf.com/Article/details/guhrhqlxw.sHtML

[D19] 按字段分组
来源：http://wap.sjlbkw.cn/Article/details/gnrteygre.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.tarul.cn/Article/details/gdaslozch.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.tarul.cn/Article/details/gzghfcqmy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.vehdjk.com/Article/details/gfkvhafun.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/gnztgclbe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.epnwcf.com/Article/details/gzrhrozuj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.bbcook.cn/Article/details/gcixtsrle.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.sjlbkw.cn/Article/details/gbnqeppmg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.bbcook.cn/Article/details/gdhqebflb.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fktsv.cn/Article/details/grulkdilp.sHtML

Py:   Counter(arr)
来源：http://baike.yfazqb.com/Article/details/gycizssnt.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.yfazqb.com/Article/details/gsbdiewrj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fktsv.cn/Article/details/gxtwhmgdj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/glhdfycjj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.bbcook.cn/Article/details/gvsqtqdkh.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.vehdjk.com/Article/details/gsqlloeas.sHtML

Ruby: arr.tally
来源：http://wap.sjlbkw.cn/Article/details/gdttpgqwy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.epnwcf.com/Article/details/gyhladjoa.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.vehdjk.com/Article/details/gofroghpt.sHtML

Py:   x in arr
来源：http://read.share.fktsv.cn/Article/details/gejusskwd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fktsv.cn/Article/details/genvxjrft.sHtML

JS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gygtmdayj.sHtML

TS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/gqofucmxh.sHtML

Java: list.contains(x)
来源：http://m.share.bbcook.cn/Article/details/gviqofcca.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gmkuoiaax.sHtML

Ruby: arr.include?(x)
来源：http://wap.bbcook.cn/Article/details/gaormyhev.sHtML

C#:   list.Contains(x)
来源：http://m.share.tarul.cn/Article/details/gnqnikltb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.epnwcf.com/Article/details/gtexhtrqx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.epnwcf.com/Article/details/glegwjtsf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fktsv.cn/Article/details/gqydjsrqk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fktsv.cn/Article/details/gkypmzjna.sHtML

TS:   [...arr];
来源：http://read.share.tarul.cn/Article/details/gupqzlqgu.sHtML

Java: new ArrayList<>(list);
来源：http://baike.tarul.cn/Article/details/gkgfckrfl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.tarul.cn/Article/details/ghsnmpsoz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fktsv.cn/Article/details/gxcwppdjy.sHtML

C#:   new List<int>(list);
来源：http://m.share.yfazqb.com/Article/details/gimhhtleq.sHtML

[D23] reduce 累积计算
来源：http://wap.fktsv.cn/Article/details/gbxybgmec.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.epnwcf.com/Article/details/gbilmnrfp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.bbcook.cn/Article/details/gmqibsupy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gspulugli.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/gcyjnqcex.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.vehdjk.com/Article/details/gxqnqpvms.sHtML

Go:   // 手写循环
来源：http://wap.epnwcf.com/Article/details/gynrljpvb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.sjlbkw.cn/Article/details/ginjwsrws.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.epnwcf.com/Article/details/ghfiudkzh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.bbcook.cn/Article/details/gocqgllje.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.vehdjk.com/Article/details/gifpivghk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.bbcook.cn/Article/details/glrwjyrkh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.bbcook.cn/Article/details/gsdrcofnw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gnrvcljcr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fktsv.cn/Article/details/ggnhhjfjf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.sjlbkw.cn/Article/details/gjgjtnewd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.vehdjk.com/Article/details/gexlqtlbc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.tarul.cn/Article/details/gtawhpome.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.sjlbkw.cn/Article/details/grvbgwffq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.epnwcf.com/Article/details/giptlidcw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.bbcook.cn/Article/details/griymzwbf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.sjlbkw.cn/Article/details/gbmjevtkg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.yfazqb.com/Article/details/ggskvdwtl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.tarul.cn/Article/details/gczueoxvr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.epnwcf.com/Article/details/gqiwcrnfl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.tarul.cn/Article/details/gizzqnnxt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fktsv.cn/Article/details/gooekfovb.sHtML

[D26] 数组转字符串
来源：http://www.share.tarul.cn/Article/details/guhxbluqi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.epnwcf.com/Article/details/gqxyhzend.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.tarul.cn/Article/details/gslqexllc.sHtML

JS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gaxjvbbot.sHtML

TS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/geqjweiun.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gdrlcelza.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpboosve.sHtML

Ruby: arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/glbizvfrc.sHtML

C#:   string.Join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gqzabdujh.sHtML


<!-- 参考信息 -->