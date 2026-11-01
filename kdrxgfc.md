代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.sjlbkw.cn/Article/details/gotcvywxl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.tarul.cn/Article/details/gzurmpwvi.sHtML

Java: import java.util.List;
来源：http://www.m.share.epnwcf.com/Article/details/gqajseejd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.yfazqb.com/Article/details/gbnentoxz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.vehdjk.com/Article/details/gqysqporw.sHtML

C#:   using System.Text;
来源：http://www.share.yfazqb.com/Article/details/gnaedaltx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.tarul.cn/Article/details/gfwbntygj.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.yfazqb.com/Article/details/gqvsyzvzy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.bbcook.cn/Article/details/gftrsrhna.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/gtjtmerjn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fktsv.cn/Article/details/gxopshijg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fktsv.cn/Article/details/gkxgudwbv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.tarul.cn/Article/details/gsxbvilsv.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.vehdjk.com/Article/details/gfrfavmpp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.sjlbkw.cn/Article/details/gvjbrsjft.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fktsv.cn/Article/details/gtqdttjtz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.vehdjk.com/Article/details/ganniulot.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gofdyfyto.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fktsv.cn/Article/details/glahpmzdg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gtbweysjn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gyaeahyka.sHtML

Go:   func add(a, b int) int
来源：http://wap.bbcook.cn/Article/details/gazhlapyd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.epnwcf.com/Article/details/gngdoyftg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fktsv.cn/Article/details/gkkzhqonc.sHtML

[C14] 泛型函数
来源：http://baike.epnwcf.com/Article/details/gohcjdpvn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.epnwcf.com/Article/details/gamhpszow.sHtML

PHP:  // 无泛型
来源：http://baike.bbcook.cn/Article/details/gqjrcbucb.sHtML

JS:   // 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gomhacakk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.sjlbkw.cn/Article/details/gndtnudpx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.epnwcf.com/Article/details/gczanidlk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.yfazqb.com/Article/details/gflbxdgvy.sHtML

Ruby: # 无泛型
来源：http://3g.tarul.cn/Article/details/gmknzqryv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.yfazqb.com/Article/details/ggcagfsez.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.yfazqb.com/Article/details/gmotppqxj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fktsv.cn/Article/details/gmqofkebb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.vehdjk.com/Article/details/gwrzgkijt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/gqsayqcec.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.vehdjk.com/Article/details/garrqsfzk.sHtML

Java: // 无解构
来源：http://www.m.share.tarul.cn/Article/details/gcqlkvozq.sHtML

Go:   // 无解构
来源：http://blog.yfazqb.com/Article/details/gnkchpzjx.sHtML

Ruby: a, b = pair
来源：http://m.share.epnwcf.com/Article/details/gubdtpycz.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.bbcook.cn/Article/details/gvgfeqcyp.sHtML

[C16] 函数 / 方法重载
来源：http://wap.tarul.cn/Article/details/gtjmpjsmj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.yfazqb.com/Article/details/gvbgqmmnz.sHtML

PHP:  // 无重载
来源：http://www.m.share.epnwcf.com/Article/details/gguuwywmq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.bbcook.cn/Article/details/gjfalsuck.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.epnwcf.com/Article/details/gdeaszklu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.sjlbkw.cn/Article/details/gcxbqfsvu.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.tarul.cn/Article/details/gankbdlsn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.yfazqb.com/Article/details/gsagpcajz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.bbcook.cn/Article/details/ggdqbeqai.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzvqrpwlx.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.tarul.cn/Article/details/ggouoqnha.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxzmezqon.sHtML

[D01] 创建数组 / 列表
来源：http://wap.yfazqb.com/Article/details/guasotxkr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.bbcook.cn/Article/details/gkmjdbusi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fktsv.cn/Article/details/gxbsnreuf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gkfvwtwln.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.vehdjk.com/Article/details/gkgzbixmr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.bbcook.cn/Article/details/goikhfwsb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.bbcook.cn/Article/details/gqjtlnjcy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fktsv.cn/Article/details/gspyrdopy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.epnwcf.com/Article/details/gvkqwvfxo.sHtML

[D02] 追加元素到末尾
来源：http://blog.fktsv.cn/Article/details/gujrnizsa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.yfazqb.com/Article/details/gbhuttjkp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.epnwcf.com/Article/details/gwarhktlu.sHtML

JS:   arr.push(4);
来源：http://read.share.epnwcf.com/Article/details/gtdnlssyu.sHtML

TS:   arr.push(4);
来源：http://blog.epnwcf.com/Article/details/grjrttodn.sHtML

Java: list.add(4);
来源：http://3g.epnwcf.com/Article/details/gjoktsjpy.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.vehdjk.com/Article/details/gxinkyzyb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.bbcook.cn/Article/details/ghnxhuhyo.sHtML

C#:   list.Add(4);
来源：http://read.share.sjlbkw.cn/Article/details/gwaqyaszg.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.yfazqb.com/Article/details/gqbvfnwve.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gaocfmmtv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fktsv.cn/Article/details/gjdzvnarv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.vehdjk.com/Article/details/gtnceliba.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.sjlbkw.cn/Article/details/giuffmbeh.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gkqghakij.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.yfazqb.com/Article/details/glkymzwfz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.vehdjk.com/Article/details/gkvamljjr.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.tarul.cn/Article/details/gggjopneo.sHtML

[D04] 删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gytgouadx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.tarul.cn/Article/details/glwsoefqm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.tarul.cn/Article/details/gfvjsvckm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.epnwcf.com/Article/details/gjsjsazso.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fktsv.cn/Article/details/gmhmtbgia.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.epnwcf.com/Article/details/gmxkcjzks.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.sjlbkw.cn/Article/details/ggwbffpmn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/ggynmevrb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.epnwcf.com/Article/details/gscpszzod.sHtML

[D05] 访问与修改元素
来源：http://blog.sjlbkw.cn/Article/details/gofxyxhro.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gwscijykl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.tarul.cn/Article/details/gwrgijirs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gkrxtzdbk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.vehdjk.com/Article/details/gdwxxzydc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.tarul.cn/Article/details/gqjvjqrta.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/ghcwfeikb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gxogugsxe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/gpbufppuk.sHtML

[D06] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gypwnbrlu.sHtML

Py:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/geexoidbc.sHtML

PHP:  count($arr);
来源：http://m.share.vehdjk.com/Article/details/gwjckidnb.sHtML

JS:   arr.length
来源：http://m.share.fktsv.cn/Article/details/grmhhrist.sHtML

TS:   arr.length
来源：http://baike.yfazqb.com/Article/details/ghzfmncyz.sHtML

Java: list.size();
来源：http://wap.epnwcf.com/Article/details/gcdoeteip.sHtML

Go:   len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gverripms.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gxkwmvoqb.sHtML

C#:   list.Count;
来源：http://read.share.tarul.cn/Article/details/gpyptsedr.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.epnwcf.com/Article/details/gpkagyvdg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.yfazqb.com/Article/details/gwgufubwi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.sjlbkw.cn/Article/details/gxavgmcim.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.bbcook.cn/Article/details/ggbtyxrpb.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gedcvmwpa.sHtML

Java: list.subList(1, 4);
来源：http://3g.vehdjk.com/Article/details/glzvinqhs.sHtML

Go:   arr[1:4]
来源：http://www.share.tarul.cn/Article/details/goqgkudow.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fktsv.cn/Article/details/gfcizweur.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fktsv.cn/Article/details/gnutdlkwm.sHtML

[D08] 合并两个数组
来源：http://www.share.yfazqb.com/Article/details/gephzvtlv.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.sjlbkw.cn/Article/details/gicfebxsv.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.sjlbkw.cn/Article/details/gdrpjyctx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.tarul.cn/Article/details/gjnkjwrnf.sHtML

TS:   [...a, ...b];
来源：http://3g.bbcook.cn/Article/details/gugugigbb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.tarul.cn/Article/details/gpzyxuwjb.sHtML

Go:   append(a, b...)
来源：http://blog.tarul.cn/Article/details/gycovhjth.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.epnwcf.com/Article/details/gebolvgfa.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fktsv.cn/Article/details/guyeoxkog.sHtML

[D09] 排序（升序）
来源：http://blog.fktsv.cn/Article/details/gqjtyaphj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/ghemidquu.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gmjnzlvng.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.tarul.cn/Article/details/gnlztclxf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.epnwcf.com/Article/details/gmuoduzcx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.tarul.cn/Article/details/gzixaefml.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gnjfgljqf.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gzaofogds.sHtML

C#:   list.Sort();
来源：http://blog.tarul.cn/Article/details/ggyadqhfa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.sjlbkw.cn/Article/details/gchetnywo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.tarul.cn/Article/details/gkbwycrzy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.epnwcf.com/Article/details/ghlbcvspa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fktsv.cn/Article/details/gdnifucxg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gmcpdgbmu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.vehdjk.com/Article/details/gaobvizwn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.tarul.cn/Article/details/gespobrrq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.sjlbkw.cn/Article/details/ghrtgyrvm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.tarul.cn/Article/details/gcirquibo.sHtML

[D11] 反转数组
来源：http://mobile.vehdjk.com/Article/details/glmzczghx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.vehdjk.com/Article/details/gdjhvnpop.sHtML

PHP:  array_reverse($arr);
来源：http://wap.vehdjk.com/Article/details/gulpmcgju.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.epnwcf.com/Article/details/giwdfmgbi.sHtML

TS:   [...arr].reverse();
来源：http://blog.sjlbkw.cn/Article/details/guqionwbh.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fktsv.cn/Article/details/geaggtxtk.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.sjlbkw.cn/Article/details/gvikmlbjj.sHtML

Ruby: arr.reverse
来源：http://baike.fktsv.cn/Article/details/ggjfynnmt.sHtML

C#:   list.Reverse();
来源：http://mobile.vehdjk.com/Article/details/ghgnyieob.sHtML

[D12] 查找元素下标
来源：http://m.share.vehdjk.com/Article/details/gctqbjsxm.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.epnwcf.com/Article/details/gfmvmtris.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gutfnhofs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.tarul.cn/Article/details/gotjtjvxm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.yfazqb.com/Article/details/gjjwujtez.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.bbcook.cn/Article/details/goesqmhlg.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gwjrmtszt.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.yfazqb.com/Article/details/gwlsjntxf.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.tarul.cn/Article/details/gxypmijzs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.yfazqb.com/Article/details/garevrqvl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.sjlbkw.cn/Article/details/gaenycpci.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.yfazqb.com/Article/details/gqvuxripa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gsapmxujy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fktsv.cn/Article/details/gbkoqxejh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.vehdjk.com/Article/details/gnfxdwnzt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.tarul.cn/Article/details/gwnytuvaq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.tarul.cn/Article/details/gfgjkpous.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.tarul.cn/Article/details/gfceopizw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.vehdjk.com/Article/details/geowwvmzn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fktsv.cn/Article/details/gjekvogvl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/ghwxkpdmj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gaahywreo.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/goyuqnape.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fktsv.cn/Article/details/glggqprve.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gyzxhhgbq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.epnwcf.com/Article/details/gadxuatsg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.epnwcf.com/Article/details/gkmbdfwlg.sHtML

[D15] 去重
来源：http://m.share.bbcook.cn/Article/details/gzpnphbhk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gaefazxdn.sHtML

PHP:  array_unique($arr);
来源：http://read.share.vehdjk.com/Article/details/gjjnsvwyt.sHtML

JS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gvuqrcejs.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gtretpdgn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.bbcook.cn/Article/details/ghthpzarw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.bbcook.cn/Article/details/ggsjojcvv.sHtML

Ruby: arr.uniq
来源：http://blog.yfazqb.com/Article/details/gwetvhxjg.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.tarul.cn/Article/details/gogjyavii.sHtML

[D16] 求和与平均值
来源：http://3g.epnwcf.com/Article/details/gueazepuu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.epnwcf.com/Article/details/ggsyaiqps.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.epnwcf.com/Article/details/gdzuxeldo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.yfazqb.com/Article/details/gnphoixvo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.epnwcf.com/Article/details/glosevanp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.bbcook.cn/Article/details/gxpnebcjd.sHtML

Go:   // 手写循环累加
来源：http://3g.tarul.cn/Article/details/gfnqjeebc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/gceqlwtgb.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.epnwcf.com/Article/details/gybrsvjlt.sHtML

[D17] 最大值与最小值
来源：http://m.share.yfazqb.com/Article/details/gcoabwrgt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.epnwcf.com/Article/details/gektljhqc.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/gklayqjsh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.tarul.cn/Article/details/gtdvefkfv.sHtML

TS:   Math.max(...arr);
来源：http://mobile.bbcook.cn/Article/details/gtbuoemfr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fktsv.cn/Article/details/gtkogbtnf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.bbcook.cn/Article/details/gfojptwns.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.sjlbkw.cn/Article/details/gowpjplsr.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fktsv.cn/Article/details/gkuxffkph.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.bbcook.cn/Article/details/gojbguhla.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/gqjmitfkw.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.tarul.cn/Article/details/gtxokpyho.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.tarul.cn/Article/details/gucpokqhy.sHtML

TS:   nested.flat();
来源：http://mobile.bbcook.cn/Article/details/garvmbhij.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fktsv.cn/Article/details/gopytqhga.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.tarul.cn/Article/details/gbwsqysai.sHtML

Ruby: nested.flatten
来源：http://mobile.yfazqb.com/Article/details/gssjrijni.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.tarul.cn/Article/details/gmdqdivdr.sHtML

[D19] 按字段分组
来源：http://mobile.sjlbkw.cn/Article/details/gzrlnsgdj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fktsv.cn/Article/details/geyzuknci.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.yfazqb.com/Article/details/gdsybzbyg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.epnwcf.com/Article/details/gyyspiglv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.vehdjk.com/Article/details/ghuuhzxru.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.yfazqb.com/Article/details/gpgfsrtfl.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.bbcook.cn/Article/details/gtrscwalh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.vehdjk.com/Article/details/gxcbhkomk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.epnwcf.com/Article/details/gfqeaxbqs.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.vehdjk.com/Article/details/glmpfjfdn.sHtML

Py:   Counter(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gxousbcpz.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.epnwcf.com/Article/details/gwaivwkkx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gdgsclmdw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/gpvlfjijx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.bbcook.cn/Article/details/gknlweerr.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.sjlbkw.cn/Article/details/gjmiynriu.sHtML

Ruby: arr.tally
来源：http://baike.fktsv.cn/Article/details/gfzizqtfp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fktsv.cn/Article/details/godxlzqlz.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.vehdjk.com/Article/details/gerguafoy.sHtML

Py:   x in arr
来源：http://blog.vehdjk.com/Article/details/gmtlbgpoo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/giiorcaao.sHtML

JS:   arr.includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gyvjbkaey.sHtML

TS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/galobcxkr.sHtML

Java: list.contains(x)
来源：http://wap.epnwcf.com/Article/details/gdvaywwcv.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gbvapbuyt.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gjnfiqmbg.sHtML

C#:   list.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/grulksote.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.epnwcf.com/Article/details/grjxkfxmv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.vehdjk.com/Article/details/grubfghzg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.bbcook.cn/Article/details/gytzrihhb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gkffisxxk.sHtML

TS:   [...arr];
来源：http://wap.fktsv.cn/Article/details/gfjedzakk.sHtML

Java: new ArrayList<>(list);
来源：http://blog.vehdjk.com/Article/details/gzajvuyht.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.yfazqb.com/Article/details/grrkmrhkv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlebedqm.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fktsv.cn/Article/details/grgrozpkl.sHtML

[D23] reduce 累积计算
来源：http://www.share.tarul.cn/Article/details/gwmgkzrhv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gnhafskcr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.yfazqb.com/Article/details/gzlyraxfo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.bbcook.cn/Article/details/gvjchsgpj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/gdvkmlbvl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.sjlbkw.cn/Article/details/gfzadeuqy.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/gjreszyrf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.vehdjk.com/Article/details/gesnbnrvs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.epnwcf.com/Article/details/grdemagkw.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fktsv.cn/Article/details/gqgnixgog.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.yfazqb.com/Article/details/gfruhkabx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.tarul.cn/Article/details/galakswfz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.tarul.cn/Article/details/gfapfvird.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.epnwcf.com/Article/details/gsahyvdax.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.tarul.cn/Article/details/gmnvpnffh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.vehdjk.com/Article/details/gfhugpcut.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwklvrcfp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fktsv.cn/Article/details/gitbyisaq.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.epnwcf.com/Article/details/gdjthrfnm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.sjlbkw.cn/Article/details/goshqjgup.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fktsv.cn/Article/details/gfpipdvay.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.sjlbkw.cn/Article/details/gkdlxcozc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.tarul.cn/Article/details/gndlexkry.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/geabzlzxq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.yfazqb.com/Article/details/galiyhajw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.bbcook.cn/Article/details/gruywkiqa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/gjjgapmba.sHtML

[D26] 数组转字符串
来源：http://baike.sjlbkw.cn/Article/details/ggriehlzx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fktsv.cn/Article/details/gxeligojg.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.yfazqb.com/Article/details/gcfmffaha.sHtML

JS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gfgissitq.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gzgsprjuw.sHtML

Java: String.join(", ", list)
来源：http://read.share.epnwcf.com/Article/details/grqzihrsv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.vehdjk.com/Article/details/gadupjlmi.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/guvemhaeu.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/guvjhpyaz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxobditnr.sHtML

E. 字符串处理
来源：http://mobile.vehdjk.com/Article/details/gyduopepe.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdtacmtzt.sHtML

[E01] 拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/glgxmtxix.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.yfazqb.com/Article/details/gvlbrqtcz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fktsv.cn/Article/details/gwezfubyq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.sjlbkw.cn/Article/details/ghbbtsrwl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gidmxpggj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.vehdjk.com/Article/details/gmfyzqecs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.epnwcf.com/Article/details/gljlxwadq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.yfazqb.com/Article/details/gbjaviyuv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.tarul.cn/Article/details/gosopqozd.sHtML


<!-- 参考信息 -->