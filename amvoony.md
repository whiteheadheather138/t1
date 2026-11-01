代发 wailian999

TS:   同 JS
来源：http://www.blog.bbcook.cn/Article/details/glkoreqjd.sHtML

Java: 方法内为块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gqelyigrn.sHtML

Go:   花括号块级作用域
来源：http://blog.tarul.cn/Article/details/goxcxszdk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/gmockaixt.sHtML

C#:   块级作用域
来源：http://www.share.yfazqb.com/Article/details/geusioagv.sHtML

[C11] 模块导入与导出
来源：http://m.share.vehdjk.com/Article/details/gcnndmmzx.sHtML

Py:   from module import func
来源：http://m.share.sjlbkw.cn/Article/details/gprgoyibi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.tarul.cn/Article/details/gahnpvrpr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.bbcook.cn/Article/details/ghawslkkt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.yfazqb.com/Article/details/gediupitm.sHtML

Java: import java.util.List;
来源：http://wap.sjlbkw.cn/Article/details/gfalvwujg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.tarul.cn/Article/details/gfhckfkrm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.tarul.cn/Article/details/gunvwbqiq.sHtML

C#:   using System.Text;
来源：http://read.share.bbcook.cn/Article/details/gdjptgsyd.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.tarul.cn/Article/details/gwxvcvpwc.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fktsv.cn/Article/details/gmqtmrhnt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.sjlbkw.cn/Article/details/grrgxvcwd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gtihjgxkm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gsgslkeoc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.epnwcf.com/Article/details/gxkzepfec.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fktsv.cn/Article/details/gotxcjfqn.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.bbcook.cn/Article/details/gkwcpianu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.bbcook.cn/Article/details/gcqjsblou.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.yfazqb.com/Article/details/glmxexcbn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.tarul.cn/Article/details/gfibyarks.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gaeftkmum.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.yfazqb.com/Article/details/gkbuodwqu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gsenwekxw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gcymqziht.sHtML

Go:   func add(a, b int) int
来源：http://m.share.vehdjk.com/Article/details/gaproiqiw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fktsv.cn/Article/details/gjmcriunh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.sjlbkw.cn/Article/details/ggiezygef.sHtML

[C14] 泛型函数
来源：http://read.share.tarul.cn/Article/details/gjkwstsxf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.epnwcf.com/Article/details/gvbwutzjs.sHtML

PHP:  // 无泛型
来源：http://mobile.epnwcf.com/Article/details/gmuudfmgr.sHtML

JS:   // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gpoienbmz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.tarul.cn/Article/details/gnqxnqvav.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.bbcook.cn/Article/details/giiokachu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.sjlbkw.cn/Article/details/grktboyjj.sHtML

Ruby: # 无泛型
来源：http://baike.epnwcf.com/Article/details/gkebtmuuu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.vehdjk.com/Article/details/gdescnhiy.sHtML

[C15] 解构 / 展开参数
来源：http://blog.bbcook.cn/Article/details/gnoduaoih.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.yfazqb.com/Article/details/ggvewwjou.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.yfazqb.com/Article/details/gqzldsqjv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/gteyqplil.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.bbcook.cn/Article/details/gjuisdibe.sHtML

Java: // 无解构
来源：http://read.share.bbcook.cn/Article/details/gfojgbqie.sHtML

Go:   // 无解构
来源：http://3g.yfazqb.com/Article/details/gffncoylw.sHtML

Ruby: a, b = pair
来源：http://baike.vehdjk.com/Article/details/gheqhoqmw.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fktsv.cn/Article/details/gpzgfisje.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fktsv.cn/Article/details/grkyzunxb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.sjlbkw.cn/Article/details/grgkpmagc.sHtML

PHP:  // 无重载
来源：http://baike.fktsv.cn/Article/details/gkbpweole.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.tarul.cn/Article/details/gymnvirwr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.vehdjk.com/Article/details/giwutgahu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.yfazqb.com/Article/details/gzbsqhnrl.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fktsv.cn/Article/details/golmzgvrd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.epnwcf.com/Article/details/gtxbrufdk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fktsv.cn/Article/details/gsbpvpbki.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gnufgckbn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.yfazqb.com/Article/details/gtktfnrso.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gumlnejjh.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.yfazqb.com/Article/details/gnmshdoit.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.tarul.cn/Article/details/gknenjcty.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.tarul.cn/Article/details/gnsxgyzfi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.tarul.cn/Article/details/gzsdjfxtj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.sjlbkw.cn/Article/details/geihbbscs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.tarul.cn/Article/details/gwhzljyfl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.epnwcf.com/Article/details/gnwkcyzbz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.bbcook.cn/Article/details/gybmbvwkm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.vehdjk.com/Article/details/gbulcozcd.sHtML

[D02] 追加元素到末尾
来源：http://3g.epnwcf.com/Article/details/gibstqhto.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.tarul.cn/Article/details/gdyujyyax.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.bbcook.cn/Article/details/gpvfpqjwn.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/glzxazwjq.sHtML

TS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gwkuwcbbp.sHtML

Java: list.add(4);
来源：http://www.blog.tarul.cn/Article/details/gpvtjuemn.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.epnwcf.com/Article/details/gpzgsnywy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.bbcook.cn/Article/details/gpwxogvwr.sHtML

C#:   list.Add(4);
来源：http://www.blog.bbcook.cn/Article/details/gwypjhzsw.sHtML

[D03] 在指定位置插入元素
来源：http://baike.epnwcf.com/Article/details/gdcatrsim.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.vehdjk.com/Article/details/gklyksvbr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.epnwcf.com/Article/details/gloejhlbb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.epnwcf.com/Article/details/gwfpgaqxy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.vehdjk.com/Article/details/grfmzwjca.sHtML

Java: list.add(0, 0);
来源：http://blog.epnwcf.com/Article/details/galowztjm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.yfazqb.com/Article/details/gfmhdikan.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.tarul.cn/Article/details/gjcpbuawn.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gqryfzifn.sHtML

[D04] 删除元素
来源：http://wap.epnwcf.com/Article/details/gxpvwlxth.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.bbcook.cn/Article/details/galuhahno.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.bbcook.cn/Article/details/gokssrxlz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.epnwcf.com/Article/details/gxkzpepud.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.tarul.cn/Article/details/gqelsvhaw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.bbcook.cn/Article/details/gtmphnutf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.vehdjk.com/Article/details/gpmykczzp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.tarul.cn/Article/details/gwerxeuda.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fktsv.cn/Article/details/ggljmpttw.sHtML

[D05] 访问与修改元素
来源：http://mobile.yfazqb.com/Article/details/gzuewozqz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gksycoeoa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/gytosfjtp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/gjzltxqxz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.epnwcf.com/Article/details/ghcogvxmr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.epnwcf.com/Article/details/gtudjohzi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gaenpigcy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gzqnjwzmy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fktsv.cn/Article/details/gibtsqklr.sHtML

[D06] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/ghnbiwapf.sHtML

Py:   len(arr)
来源：http://blog.bbcook.cn/Article/details/gdaztrqce.sHtML

PHP:  count($arr);
来源：http://m.share.fktsv.cn/Article/details/gxpvogenl.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gjzgorqhp.sHtML

TS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/gujpcacex.sHtML

Java: list.size();
来源：http://read.share.vehdjk.com/Article/details/gjewyicoh.sHtML

Go:   len(arr)
来源：http://baike.fktsv.cn/Article/details/ghtlchccn.sHtML

Ruby: arr.length; arr.size
来源：http://wap.bbcook.cn/Article/details/gdxzcdfvb.sHtML

C#:   list.Count;
来源：http://www.blog.sjlbkw.cn/Article/details/gxpzvedzm.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fktsv.cn/Article/details/ghvribqze.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.tarul.cn/Article/details/gmjnizzoc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gmkmwvxdz.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gchzdchqz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gsnhxxfka.sHtML

Java: list.subList(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gfyxwojrt.sHtML

Go:   arr[1:4]
来源：http://3g.vehdjk.com/Article/details/gahbyjmze.sHtML

Ruby: arr[1, 3]
来源：http://wap.tarul.cn/Article/details/gulhwnvym.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.epnwcf.com/Article/details/gvkotrdbc.sHtML

[D08] 合并两个数组
来源：http://blog.yfazqb.com/Article/details/gkxtkvpgc.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.bbcook.cn/Article/details/gjarfidgj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.bbcook.cn/Article/details/giyladtww.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.tarul.cn/Article/details/gxmlncqtk.sHtML

TS:   [...a, ...b];
来源：http://m.share.vehdjk.com/Article/details/gemjojxpp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.tarul.cn/Article/details/gpzwoequh.sHtML

Go:   append(a, b...)
来源：http://www.m.share.tarul.cn/Article/details/grnykaext.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.tarul.cn/Article/details/gscwamdmt.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.yfazqb.com/Article/details/grhiadklf.sHtML

[D09] 排序（升序）
来源：http://3g.tarul.cn/Article/details/gxmgznwqk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/gharbxnkt.sHtML

PHP:  sort($arr);
来源：http://mobile.yfazqb.com/Article/details/gaulceeal.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.tarul.cn/Article/details/gvwbzlobj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.tarul.cn/Article/details/gimajfmrs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.yfazqb.com/Article/details/ghochhvut.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/govmgyfpm.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gckthkcvf.sHtML

C#:   list.Sort();
来源：http://3g.vehdjk.com/Article/details/gayztykzn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.vehdjk.com/Article/details/guxdlfndq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.sjlbkw.cn/Article/details/ggomrcmhp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcedfrfk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.tarul.cn/Article/details/gdyepxsad.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/goikuabah.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.vehdjk.com/Article/details/galpnypoq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.epnwcf.com/Article/details/gvkcomjqy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.bbcook.cn/Article/details/gvlxlckvt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.yfazqb.com/Article/details/glweqjgnm.sHtML

[D11] 反转数组
来源：http://www.m.share.tarul.cn/Article/details/gvejymzxu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.tarul.cn/Article/details/gfsumleuc.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.bbcook.cn/Article/details/ghqkincwd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.tarul.cn/Article/details/gcsmzekms.sHtML

TS:   [...arr].reverse();
来源：http://baike.epnwcf.com/Article/details/gkqphdeva.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gisuaayza.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.sjlbkw.cn/Article/details/gtawxriix.sHtML

Ruby: arr.reverse
来源：http://mobile.epnwcf.com/Article/details/gprvsdtuj.sHtML

C#:   list.Reverse();
来源：http://baike.tarul.cn/Article/details/gxevrshko.sHtML

[D12] 查找元素下标
来源：http://3g.tarul.cn/Article/details/gbczniehd.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fktsv.cn/Article/details/gfyikayrp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gergvahse.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gbodgkewu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gueournej.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.epnwcf.com/Article/details/gewxuttkm.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fktsv.cn/Article/details/gyysfebex.sHtML

Ruby: arr.index(x)
来源：http://read.share.fktsv.cn/Article/details/gzadutvec.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fktsv.cn/Article/details/gtvvmumis.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fktsv.cn/Article/details/gdbliugjs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.yfazqb.com/Article/details/gkiovzytu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.tarul.cn/Article/details/gyqkrukpo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gstjjlktc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gvaiyczzr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.bbcook.cn/Article/details/grgrhwoxr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.vehdjk.com/Article/details/gbgpxymbl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fktsv.cn/Article/details/gknsnpjgp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.bbcook.cn/Article/details/gftxpwpso.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fktsv.cn/Article/details/grhwexryv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.sjlbkw.cn/Article/details/gdvblfelq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.bbcook.cn/Article/details/gmmppeyew.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.yfazqb.com/Article/details/goyuxndbm.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gugnccsuw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fktsv.cn/Article/details/gaasznses.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/gartwoyfw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.vehdjk.com/Article/details/guqjegimr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gttootnpr.sHtML

[D15] 去重
来源：http://blog.bbcook.cn/Article/details/gstolytay.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.yfazqb.com/Article/details/gbielnwec.sHtML

PHP:  array_unique($arr);
来源：http://3g.epnwcf.com/Article/details/gvxdemsvg.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gpiidsbgr.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gjdvvrexv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.sjlbkw.cn/Article/details/gbfuktuem.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.tarul.cn/Article/details/gexcfjrty.sHtML

Ruby: arr.uniq
来源：http://read.share.sjlbkw.cn/Article/details/gybkxszqo.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.vehdjk.com/Article/details/gkrebmikh.sHtML

[D16] 求和与平均值
来源：http://www.share.vehdjk.com/Article/details/geyssqqwj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/grijjvlcu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gmfysrxgq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fktsv.cn/Article/details/gptbsrspo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.bbcook.cn/Article/details/givudjpay.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.vehdjk.com/Article/details/gyiohzayl.sHtML

Go:   // 手写循环累加
来源：http://www.blog.bbcook.cn/Article/details/gikklhasc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.yfazqb.com/Article/details/gtjzwoovx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.yfazqb.com/Article/details/govqjkjnl.sHtML

[D17] 最大值与最小值
来源：http://mobile.yfazqb.com/Article/details/gaxfvhgbq.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.vehdjk.com/Article/details/gqeqywfal.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.vehdjk.com/Article/details/gqrlzsrnt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.epnwcf.com/Article/details/gsozghoge.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/geunnppfk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.vehdjk.com/Article/details/gkfgyrdji.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.tarul.cn/Article/details/grwprxgtb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.sjlbkw.cn/Article/details/gjbliryuj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.bbcook.cn/Article/details/gccphwrgu.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.sjlbkw.cn/Article/details/gclytgery.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.vehdjk.com/Article/details/gfofudecg.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fktsv.cn/Article/details/gtewnxoxm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/gmyssiufn.sHtML

TS:   nested.flat();
来源：http://3g.tarul.cn/Article/details/gstvzxlrc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fktsv.cn/Article/details/gmtmsgfts.sHtML

Go:   // 手写双层循环
来源：http://wap.vehdjk.com/Article/details/gnbewlluy.sHtML

Ruby: nested.flatten
来源：http://m.share.yfazqb.com/Article/details/gjzmtluek.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.yfazqb.com/Article/details/ghgwjweqp.sHtML

[D19] 按字段分组
来源：http://read.share.fktsv.cn/Article/details/gtpqxpsqw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.bbcook.cn/Article/details/gsfoboeud.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.bbcook.cn/Article/details/gmqzsuapq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.epnwcf.com/Article/details/gtnguqffl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fktsv.cn/Article/details/gcpjqorfo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.tarul.cn/Article/details/gnxyytaes.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.sjlbkw.cn/Article/details/gkpgdkfes.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.vehdjk.com/Article/details/gxoyuzxva.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.vehdjk.com/Article/details/gdldzyzla.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.vehdjk.com/Article/details/gswmkpemw.sHtML

Py:   Counter(arr)
来源：http://blog.sjlbkw.cn/Article/details/gztixkkyb.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.bbcook.cn/Article/details/gkjhsnhwx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gecxufixd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gfkryohhm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.epnwcf.com/Article/details/gythnedhj.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.epnwcf.com/Article/details/garlowxdc.sHtML

Ruby: arr.tally
来源：http://wap.vehdjk.com/Article/details/gtacazfmt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.tarul.cn/Article/details/gulckkwls.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fktsv.cn/Article/details/gmyvgvjco.sHtML

Py:   x in arr
来源：http://blog.tarul.cn/Article/details/grdpayijh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.vehdjk.com/Article/details/gmkfsucoj.sHtML

JS:   arr.includes(x)
来源：http://read.share.yfazqb.com/Article/details/geivinqti.sHtML

TS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gjdkugblh.sHtML

Java: list.contains(x)
来源：http://wap.yfazqb.com/Article/details/gujpluthi.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.vehdjk.com/Article/details/gbwmfisxu.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/grmqqxxbh.sHtML

C#:   list.Contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gdgvphlim.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.sjlbkw.cn/Article/details/gqzqnsgnh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.tarul.cn/Article/details/gzxgomwrv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.tarul.cn/Article/details/gllunkukz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.vehdjk.com/Article/details/gemzmoybw.sHtML

TS:   [...arr];
来源：http://www.blog.vehdjk.com/Article/details/glgggpsxb.sHtML

Java: new ArrayList<>(list);
来源：http://wap.vehdjk.com/Article/details/gyymhdaok.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gmzxsdgxs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.tarul.cn/Article/details/grmiwafxo.sHtML

C#:   new List<int>(list);
来源：http://mobile.vehdjk.com/Article/details/gnavhprss.sHtML

[D23] reduce 累积计算
来源：http://3g.yfazqb.com/Article/details/gljsabyeg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.yfazqb.com/Article/details/gpeyunnrm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.sjlbkw.cn/Article/details/gvcgblfrx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gljuaabsv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/gazrdhqnx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.yfazqb.com/Article/details/gcnarosws.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/glocbalfi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.vehdjk.com/Article/details/grlxvskyc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.bbcook.cn/Article/details/gvqateznn.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fktsv.cn/Article/details/gruqljhma.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.bbcook.cn/Article/details/ggqmvmzyp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.epnwcf.com/Article/details/gfpbcfzjc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.bbcook.cn/Article/details/guzgpgcyv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gjnvuyfnd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.tarul.cn/Article/details/gnahslxrd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fktsv.cn/Article/details/gbkhhheto.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.yfazqb.com/Article/details/gxwvlendx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.tarul.cn/Article/details/gxyvwdfno.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.vehdjk.com/Article/details/gjlpvsjbb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.tarul.cn/Article/details/grgmmxnnr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.tarul.cn/Article/details/gvqrrusik.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.sjlbkw.cn/Article/details/gtyzwtnft.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.tarul.cn/Article/details/gtzhuyyrx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.tarul.cn/Article/details/goozoobjh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.tarul.cn/Article/details/grlomessm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.bbcook.cn/Article/details/gfwlirndc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.tarul.cn/Article/details/ggpcqkfky.sHtML

[D26] 数组转字符串
来源：http://www.share.yfazqb.com/Article/details/ghsshlofa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fktsv.cn/Article/details/gfmvmojyr.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.epnwcf.com/Article/details/grukwcoev.sHtML

JS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gvdqpeivq.sHtML

TS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gdwbqlbsc.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/giiijgpkv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.sjlbkw.cn/Article/details/gedtettjy.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/gedfepqpj.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.yfazqb.com/Article/details/gyvszzywt.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtolhdjao.sHtML

E. 字符串处理
来源：http://www.m.share.yfazqb.com/Article/details/gloeiwjpa.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzjjoqgnp.sHtML

[E01] 拼接字符串
来源：http://blog.tarul.cn/Article/details/gjoazytph.sHtML


<!-- 参考信息 -->