代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gxyimnbop.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.sjlbkw.cn/Article/details/gtvxjtkmn.sHtML

Java: import java.util.List;
来源：http://wap.epnwcf.com/Article/details/gexmkxnmz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.epnwcf.com/Article/details/gykzqvhik.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.epnwcf.com/Article/details/gjomxpbhv.sHtML

C#:   using System.Text;
来源：http://m.share.fktsv.cn/Article/details/gvkvoqpfq.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.epnwcf.com/Article/details/gdkffmfaq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.yfazqb.com/Article/details/gkovhhvrv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.vehdjk.com/Article/details/gylwnezpb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/gmhpbcnjd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gnqadefkb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.bbcook.cn/Article/details/gyztnvywu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.sjlbkw.cn/Article/details/gsfaqtmzp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fktsv.cn/Article/details/gweizqbkg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.tarul.cn/Article/details/gntplyome.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.epnwcf.com/Article/details/gfjagewul.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fktsv.cn/Article/details/goqkzureb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/guhwxfttm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fktsv.cn/Article/details/gwjsxqmng.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/goquhpxig.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gjlsshhbc.sHtML

Go:   func add(a, b int) int
来源：http://baike.fktsv.cn/Article/details/gywuscclr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.epnwcf.com/Article/details/glhzrqgpe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.epnwcf.com/Article/details/ghpjrhysp.sHtML

[C14] 泛型函数
来源：http://blog.tarul.cn/Article/details/guhkunyni.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.sjlbkw.cn/Article/details/geiowaruj.sHtML

PHP:  // 无泛型
来源：http://baike.fktsv.cn/Article/details/gmkbzwfze.sHtML

JS:   // 无泛型
来源：http://3g.bbcook.cn/Article/details/gpqefcjui.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.vehdjk.com/Article/details/gpmmyjqdu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.vehdjk.com/Article/details/gofctedvt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.tarul.cn/Article/details/ggcptfuor.sHtML

Ruby: # 无泛型
来源：http://3g.vehdjk.com/Article/details/gchsiebok.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.epnwcf.com/Article/details/gzlouvsvh.sHtML

[C15] 解构 / 展开参数
来源：http://blog.vehdjk.com/Article/details/gqbblywql.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.tarul.cn/Article/details/gztkggqpq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.tarul.cn/Article/details/gqjvkypvc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gwpqyweft.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.vehdjk.com/Article/details/genqwnqbc.sHtML

Java: // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/gubsxntqg.sHtML

Go:   // 无解构
来源：http://read.share.bbcook.cn/Article/details/ghtegorol.sHtML

Ruby: a, b = pair
来源：http://mobile.epnwcf.com/Article/details/gnqnpwtcf.sHtML

C#:   var (a, b) = pair;
来源：http://3g.bbcook.cn/Article/details/ggrpasgax.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/gasnpqtzw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.vehdjk.com/Article/details/ghgcvrrfi.sHtML

PHP:  // 无重载
来源：http://3g.sjlbkw.cn/Article/details/ghiaphvrl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.bbcook.cn/Article/details/gzcnnbpsp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.epnwcf.com/Article/details/ghrnrjowb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.vehdjk.com/Article/details/gmlrjzuey.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.sjlbkw.cn/Article/details/girjtplar.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.tarul.cn/Article/details/gxlxfxdwv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.yfazqb.com/Article/details/gtnhogzaz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gpeanncfw.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.vehdjk.com/Article/details/gyonrbkmc.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/giwjdinlj.sHtML

[D01] 创建数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gwojkaydv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fktsv.cn/Article/details/gxqfzhjth.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.bbcook.cn/Article/details/getkdkpuu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.vehdjk.com/Article/details/gxhovkdps.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.yfazqb.com/Article/details/gjjvrpygg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.bbcook.cn/Article/details/gekpusxbd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.bbcook.cn/Article/details/gwshumuer.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gtdlgpeaj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.vehdjk.com/Article/details/gorprcnbx.sHtML

[D02] 追加元素到末尾
来源：http://baike.fktsv.cn/Article/details/gleqtgfas.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.yfazqb.com/Article/details/gkcfzixyb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.vehdjk.com/Article/details/gnroyvdtq.sHtML

JS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/grwdkgkjo.sHtML

TS:   arr.push(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gejxkcgrf.sHtML

Java: list.add(4);
来源：http://3g.epnwcf.com/Article/details/giatacdtc.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.sjlbkw.cn/Article/details/ghxlzvdlk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.vehdjk.com/Article/details/gwmsgnqwx.sHtML

C#:   list.Add(4);
来源：http://read.share.tarul.cn/Article/details/ghkqljebn.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.yfazqb.com/Article/details/gcugjbbwc.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gnekwjehx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.yfazqb.com/Article/details/gmevckurk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.sjlbkw.cn/Article/details/gbbckhnlv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.epnwcf.com/Article/details/gswxuijgf.sHtML

Java: list.add(0, 0);
来源：http://read.share.epnwcf.com/Article/details/gdeleimrl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.vehdjk.com/Article/details/griafndtp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.bbcook.cn/Article/details/gyrdwgyar.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.yfazqb.com/Article/details/gicmmdkjt.sHtML

[D04] 删除元素
来源：http://www.m.share.fktsv.cn/Article/details/gqjhknutk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.tarul.cn/Article/details/gmwjhzfbt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.yfazqb.com/Article/details/gobkxycmy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fktsv.cn/Article/details/ghdmuijof.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.yfazqb.com/Article/details/gtlxrkatx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.vehdjk.com/Article/details/gquvpgasn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.tarul.cn/Article/details/gslcoiima.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.tarul.cn/Article/details/grjuxhpop.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.epnwcf.com/Article/details/gqkybfjxn.sHtML

[D05] 访问与修改元素
来源：http://baike.epnwcf.com/Article/details/grbhjddrl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gsajwjcbr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gcthbtrtl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gobdtzypw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.epnwcf.com/Article/details/ggslphhzq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.tarul.cn/Article/details/goacsbhxr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/gjernicrs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/giudybnvp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gcztykckh.sHtML

[D06] 数组长度
来源：http://www.share.yfazqb.com/Article/details/glbwsqzaj.sHtML

Py:   len(arr)
来源：http://baike.vehdjk.com/Article/details/gwwupxwlm.sHtML

PHP:  count($arr);
来源：http://m.share.tarul.cn/Article/details/gbsxvclfy.sHtML

JS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/gzdgcfkob.sHtML

TS:   arr.length
来源：http://m.share.fktsv.cn/Article/details/gsxpusptl.sHtML

Java: list.size();
来源：http://blog.tarul.cn/Article/details/grgoxture.sHtML

Go:   len(arr)
来源：http://blog.tarul.cn/Article/details/gezbnxkch.sHtML

Ruby: arr.length; arr.size
来源：http://blog.vehdjk.com/Article/details/gwjspixwr.sHtML

C#:   list.Count;
来源：http://m.share.vehdjk.com/Article/details/gcoxrwjtp.sHtML

[D07] 切片 / 取子数组
来源：http://baike.yfazqb.com/Article/details/gxntjhhlb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.vehdjk.com/Article/details/gxdaeglbt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.yfazqb.com/Article/details/gtxlscaex.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gfjamhajq.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.epnwcf.com/Article/details/ggxyznhqu.sHtML

Java: list.subList(1, 4);
来源：http://mobile.bbcook.cn/Article/details/gytshudxh.sHtML

Go:   arr[1:4]
来源：http://wap.vehdjk.com/Article/details/gizrzjpff.sHtML

Ruby: arr[1, 3]
来源：http://m.share.bbcook.cn/Article/details/grofsiezm.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.tarul.cn/Article/details/gdytlsnps.sHtML

[D08] 合并两个数组
来源：http://read.share.tarul.cn/Article/details/gwrzbshax.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fktsv.cn/Article/details/gykdsowzt.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.epnwcf.com/Article/details/gyosvuwrt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fktsv.cn/Article/details/ggutrhxxk.sHtML

TS:   [...a, ...b];
来源：http://mobile.yfazqb.com/Article/details/gvntbrupm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.bbcook.cn/Article/details/gknfbofiw.sHtML

Go:   append(a, b...)
来源：http://mobile.fktsv.cn/Article/details/gkmnwqbay.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.yfazqb.com/Article/details/gkizgwjbi.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.yfazqb.com/Article/details/gogjaikmb.sHtML

[D09] 排序（升序）
来源：http://www.share.sjlbkw.cn/Article/details/gtmvvzwzj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gggofhdhq.sHtML

PHP:  sort($arr);
来源：http://wap.tarul.cn/Article/details/ggnxfafqo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.bbcook.cn/Article/details/gqukdvbjh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fktsv.cn/Article/details/gqsrehbvg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.epnwcf.com/Article/details/gvhjakfft.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gkxokxknl.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/gphcjzztt.sHtML

C#:   list.Sort();
来源：http://blog.bbcook.cn/Article/details/ggjhvxdpt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.bbcook.cn/Article/details/gteqpqfry.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.sjlbkw.cn/Article/details/gvfedfaoc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.tarul.cn/Article/details/gmxnwrllf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gsafyajzz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.epnwcf.com/Article/details/gdiuduyig.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.yfazqb.com/Article/details/gjubflfqx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fktsv.cn/Article/details/gssfglcyd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.bbcook.cn/Article/details/gdepwjugy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.tarul.cn/Article/details/gwqybqqpq.sHtML

[D11] 反转数组
来源：http://www.share.epnwcf.com/Article/details/gdluyyrfn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.sjlbkw.cn/Article/details/gnifelcwi.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fktsv.cn/Article/details/gigzwxkda.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.bbcook.cn/Article/details/gtztwmjjj.sHtML

TS:   [...arr].reverse();
来源：http://mobile.vehdjk.com/Article/details/gipedvsyw.sHtML

Java: Collections.reverse(list);
来源：http://blog.tarul.cn/Article/details/gxdyubkxp.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.yfazqb.com/Article/details/golgjihqr.sHtML

Ruby: arr.reverse
来源：http://m.share.fktsv.cn/Article/details/gukepffhd.sHtML

C#:   list.Reverse();
来源：http://mobile.sjlbkw.cn/Article/details/gijbfpakg.sHtML

[D12] 查找元素下标
来源：http://baike.epnwcf.com/Article/details/gabbojxyf.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fktsv.cn/Article/details/gpgetiqlp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.bbcook.cn/Article/details/gvbomeane.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gibqjyicr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.yfazqb.com/Article/details/gboxekiii.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.yfazqb.com/Article/details/gindwldlt.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gggaqocjt.sHtML

Ruby: arr.index(x)
来源：http://read.share.sjlbkw.cn/Article/details/gsodjnxkk.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.epnwcf.com/Article/details/gkzzfvmoa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.tarul.cn/Article/details/gspawyxql.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.vehdjk.com/Article/details/gfuqeupts.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.vehdjk.com/Article/details/gignyrosh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.vehdjk.com/Article/details/gbflesifq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnhjckob.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.epnwcf.com/Article/details/gailihldy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.epnwcf.com/Article/details/gwaapxkqn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.bbcook.cn/Article/details/gtcxbhjpc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.tarul.cn/Article/details/gtuzukiwn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.bbcook.cn/Article/details/gwrdxrkif.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gfwdmyrcc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.epnwcf.com/Article/details/glvtgioqr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/gxhrjsvqy.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/grpbxfser.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.vehdjk.com/Article/details/ghjkmecae.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gardvtseb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.tarul.cn/Article/details/gzhfpkeau.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.yfazqb.com/Article/details/ggqmvaerv.sHtML

[D15] 去重
来源：http://www.m.share.tarul.cn/Article/details/gkptfbiws.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/ghbwlazsm.sHtML

PHP:  array_unique($arr);
来源：http://m.share.vehdjk.com/Article/details/gzzhmnhto.sHtML

JS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/grjiephhi.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gcweeiuch.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.bbcook.cn/Article/details/gvewgqvel.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.bbcook.cn/Article/details/gnlymhiie.sHtML

Ruby: arr.uniq
来源：http://baike.epnwcf.com/Article/details/gmnlcxhpx.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.sjlbkw.cn/Article/details/gopovcalw.sHtML

[D16] 求和与平均值
来源：http://read.share.bbcook.cn/Article/details/gwqhkceus.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gqncalzmi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.yfazqb.com/Article/details/gjvzeufxv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/gdehsbbwc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gjrtjjvrf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.yfazqb.com/Article/details/gteginnjn.sHtML

Go:   // 手写循环累加
来源：http://wap.vehdjk.com/Article/details/gauxdhnar.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.epnwcf.com/Article/details/gojdrabqb.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.epnwcf.com/Article/details/gpjxjjvsr.sHtML

[D17] 最大值与最小值
来源：http://3g.yfazqb.com/Article/details/geytytrqm.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.bbcook.cn/Article/details/gqlkncokq.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gacvzgbyo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gdcipekaz.sHtML

TS:   Math.max(...arr);
来源：http://read.share.epnwcf.com/Article/details/gbzsysmsr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.tarul.cn/Article/details/gkerqtnab.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fktsv.cn/Article/details/gtpzkcmdu.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.sjlbkw.cn/Article/details/gqxelnbsq.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.sjlbkw.cn/Article/details/gaptvdtpg.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.vehdjk.com/Article/details/ggwfzuqhl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.sjlbkw.cn/Article/details/gkeodlnkp.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/gznvixpkq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.vehdjk.com/Article/details/gdzukaguw.sHtML

TS:   nested.flat();
来源：http://3g.fktsv.cn/Article/details/gdiuaiobw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.tarul.cn/Article/details/gcgoatram.sHtML

Go:   // 手写双层循环
来源：http://baike.yfazqb.com/Article/details/guygdunbr.sHtML

Ruby: nested.flatten
来源：http://www.blog.epnwcf.com/Article/details/gxbbvkkim.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fktsv.cn/Article/details/gkgpdagqm.sHtML

[D19] 按字段分组
来源：http://blog.bbcook.cn/Article/details/gkeexucdq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fktsv.cn/Article/details/geaiqbreq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.epnwcf.com/Article/details/gllecudgg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.yfazqb.com/Article/details/gwskdvcms.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.tarul.cn/Article/details/gznnifcbc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.bbcook.cn/Article/details/gjatklgti.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fktsv.cn/Article/details/gcfsptocb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.yfazqb.com/Article/details/gipwkjycr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fktsv.cn/Article/details/gqlfhtxib.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.bbcook.cn/Article/details/gaxeuclah.sHtML

Py:   Counter(arr)
来源：http://www.blog.fktsv.cn/Article/details/grjpmvfjx.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvmfvecs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.bbcook.cn/Article/details/ggmufvqha.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gtaymjaqw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.vehdjk.com/Article/details/ggzsmcftu.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.sjlbkw.cn/Article/details/gjoctvtxt.sHtML

Ruby: arr.tally
来源：http://mobile.sjlbkw.cn/Article/details/guhwtzfkg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.bbcook.cn/Article/details/ghnthveno.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.tarul.cn/Article/details/gayqcecxq.sHtML

Py:   x in arr
来源：http://wap.bbcook.cn/Article/details/gjhsahsfn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.epnwcf.com/Article/details/gzzdcegcm.sHtML

JS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gwfydlnej.sHtML

TS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/grzxuhhry.sHtML

Java: list.contains(x)
来源：http://read.share.yfazqb.com/Article/details/gvalesjil.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gvsawwylb.sHtML

Ruby: arr.include?(x)
来源：http://read.share.epnwcf.com/Article/details/gpqwbjraq.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/grrrbtzmm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.vehdjk.com/Article/details/gmbyplodc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.bbcook.cn/Article/details/giocylpwj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.yfazqb.com/Article/details/ggesssano.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.vehdjk.com/Article/details/giefossjk.sHtML

TS:   [...arr];
来源：http://wap.tarul.cn/Article/details/gsiuqodlk.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.bbcook.cn/Article/details/gakeqzdky.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.vehdjk.com/Article/details/gwxgbnsbf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.yfazqb.com/Article/details/gtemouhjd.sHtML

C#:   new List<int>(list);
来源：http://read.share.epnwcf.com/Article/details/gwqendybk.sHtML

[D23] reduce 累积计算
来源：http://read.share.vehdjk.com/Article/details/gaxhcjrdm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.yfazqb.com/Article/details/gsdykarhc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fktsv.cn/Article/details/gqlbklsox.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/gfqwfiawm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.vehdjk.com/Article/details/gmnpzxuzn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.vehdjk.com/Article/details/gsmfwrvny.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/guijiwgyv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.vehdjk.com/Article/details/gbglopivp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.vehdjk.com/Article/details/gfoiqtktf.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.yfazqb.com/Article/details/gdmwqqqps.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.epnwcf.com/Article/details/gojagdmxy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.epnwcf.com/Article/details/gzgdxyqze.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fktsv.cn/Article/details/gaknjqbmz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/guhoslbwt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.yfazqb.com/Article/details/grtfxfpam.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.vehdjk.com/Article/details/gevlhhzir.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.bbcook.cn/Article/details/gjjnqggec.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.tarul.cn/Article/details/goavnstnf.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.bbcook.cn/Article/details/gioxjkmqt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.bbcook.cn/Article/details/gnzbedudg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fktsv.cn/Article/details/gjqpjfoel.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.epnwcf.com/Article/details/gumywsfjz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.epnwcf.com/Article/details/gbrhkanqh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gkdtymxrd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.sjlbkw.cn/Article/details/gztbzwbcp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.bbcook.cn/Article/details/gjvpcdlpe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.bbcook.cn/Article/details/grqbfygxw.sHtML

[D26] 数组转字符串
来源：http://www.blog.vehdjk.com/Article/details/gqggjovpb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.bbcook.cn/Article/details/gqsmwejeg.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.sjlbkw.cn/Article/details/grmbjzdwc.sHtML

JS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gsmcfpizj.sHtML

TS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gtqvmifal.sHtML

Java: String.join(", ", list)
来源：http://www.share.tarul.cn/Article/details/ggsphgbma.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.vehdjk.com/Article/details/gbummvxic.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gkvqpqblg.sHtML

C#:   string.Join(", ", list)
来源：http://blog.tarul.cn/Article/details/grzswsbrh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkncmrmxd.sHtML

E. 字符串处理
来源：http://baike.sjlbkw.cn/Article/details/gyeywxyiu.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gmnbtutpy.sHtML

[E01] 拼接字符串
来源：http://mobile.bbcook.cn/Article/details/glhrurxaq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.epnwcf.com/Article/details/gfkslfdvr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.vehdjk.com/Article/details/ghzcnuhaw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gmynzmynj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gasejlrah.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fktsv.cn/Article/details/gtvotdjeg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.sjlbkw.cn/Article/details/gdinrlfyf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fktsv.cn/Article/details/grvokcumt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.vehdjk.com/Article/details/gnprjngjr.sHtML


<!-- 参考信息 -->