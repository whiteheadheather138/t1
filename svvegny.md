代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.bbcook.cn/Article/details/gagllspbv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.yfazqb.com/Article/details/gtoejchdc.sHtML

Java: import java.util.List;
来源：http://mobile.epnwcf.com/Article/details/gikbylnyn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.epnwcf.com/Article/details/grzbtxvzl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.yfazqb.com/Article/details/gvzgjiibq.sHtML

C#:   using System.Text;
来源：http://www.m.share.epnwcf.com/Article/details/gimcpdeyl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.tarul.cn/Article/details/gobxnrqlj.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fktsv.cn/Article/details/gzacseggp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.bbcook.cn/Article/details/gqzcnjqca.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gwutxqcko.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.epnwcf.com/Article/details/ghjqcyiat.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.bbcook.cn/Article/details/gvkfladet.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fktsv.cn/Article/details/goyypuvsn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.sjlbkw.cn/Article/details/gjmofojqm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.vehdjk.com/Article/details/gnopenfjo.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.yfazqb.com/Article/details/gmqkwxiyt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.epnwcf.com/Article/details/gnitltucz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gjdvykekv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.sjlbkw.cn/Article/details/gdfgeppkb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gbsqireud.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/grzrqlpom.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fktsv.cn/Article/details/gmuuwhmot.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.tarul.cn/Article/details/gaspcwrte.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.tarul.cn/Article/details/glgrhrkoh.sHtML

[C14] 泛型函数
来源：http://3g.yfazqb.com/Article/details/gsryifqzd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.epnwcf.com/Article/details/gkhnvnyto.sHtML

PHP:  // 无泛型
来源：http://baike.fktsv.cn/Article/details/gvkczsgwz.sHtML

JS:   // 无泛型
来源：http://read.share.bbcook.cn/Article/details/goveiyzmy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.epnwcf.com/Article/details/gssdfydby.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.sjlbkw.cn/Article/details/gnwqfkgxj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.yfazqb.com/Article/details/glwngkgef.sHtML

Ruby: # 无泛型
来源：http://blog.fktsv.cn/Article/details/grvypgvws.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.bbcook.cn/Article/details/grkunqxux.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fktsv.cn/Article/details/ggybrxobc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fktsv.cn/Article/details/gqebiyeme.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.tarul.cn/Article/details/gjkzpcgsi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.vehdjk.com/Article/details/gdplyhpjs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.yfazqb.com/Article/details/gyambnqhj.sHtML

Java: // 无解构
来源：http://www.m.share.epnwcf.com/Article/details/gzwyaxsdo.sHtML

Go:   // 无解构
来源：http://baike.epnwcf.com/Article/details/gqzvtkuec.sHtML

Ruby: a, b = pair
来源：http://www.share.sjlbkw.cn/Article/details/gyvagrelw.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fktsv.cn/Article/details/gjtdzsnks.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.yfazqb.com/Article/details/gvnswnhfm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.vehdjk.com/Article/details/gwcxnnnkg.sHtML

PHP:  // 无重载
来源：http://wap.sjlbkw.cn/Article/details/gtzjehyyk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.tarul.cn/Article/details/geogokwtt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fktsv.cn/Article/details/gupxibxde.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.tarul.cn/Article/details/gcrmtjzvf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fktsv.cn/Article/details/gqadxufbz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.bbcook.cn/Article/details/gumanoypc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.vehdjk.com/Article/details/gcfrbfvpd.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbqaxsxxi.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.yfazqb.com/Article/details/gttvzjkfv.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gmlgkjkqq.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/gydktayec.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.tarul.cn/Article/details/gmdenhilq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.epnwcf.com/Article/details/gdpfqhiks.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.epnwcf.com/Article/details/gtpmgfvps.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.epnwcf.com/Article/details/gppthtdae.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fktsv.cn/Article/details/gakceulvn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.epnwcf.com/Article/details/gzaaedgzf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.bbcook.cn/Article/details/gxfmqkgnk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.sjlbkw.cn/Article/details/gxvfvirae.sHtML

[D02] 追加元素到末尾
来源：http://wap.fktsv.cn/Article/details/gogvvsvci.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.epnwcf.com/Article/details/gfeehlxlx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fktsv.cn/Article/details/gzdwfxxpn.sHtML

JS:   arr.push(4);
来源：http://3g.vehdjk.com/Article/details/gorzbvjef.sHtML

TS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gaagongok.sHtML

Java: list.add(4);
来源：http://m.share.sjlbkw.cn/Article/details/gnvacbvpj.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.bbcook.cn/Article/details/grlbsgims.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.yfazqb.com/Article/details/gxsekswdn.sHtML

C#:   list.Add(4);
来源：http://3g.yfazqb.com/Article/details/gpwkrrgtw.sHtML

[D03] 在指定位置插入元素
来源：http://wap.yfazqb.com/Article/details/gzainvbzk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/gvcwppuvl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.tarul.cn/Article/details/gnjiwzpff.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fktsv.cn/Article/details/gvrykzpvf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gzogrntlv.sHtML

Java: list.add(0, 0);
来源：http://wap.tarul.cn/Article/details/gxfthvngl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gedfsflhu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.yfazqb.com/Article/details/gqaozcgxm.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fktsv.cn/Article/details/guibchwgu.sHtML

[D04] 删除元素
来源：http://mobile.tarul.cn/Article/details/gmjkcpkyk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.tarul.cn/Article/details/gfkpwzwlb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gzdiahtka.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.sjlbkw.cn/Article/details/gcwhpaddh.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.epnwcf.com/Article/details/gkhynzebv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.vehdjk.com/Article/details/gcmbmsclz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.yfazqb.com/Article/details/gjvgghews.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.epnwcf.com/Article/details/gdgudhuzp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.bbcook.cn/Article/details/gzvzbrtfj.sHtML

[D05] 访问与修改元素
来源：http://m.share.vehdjk.com/Article/details/gcrzxjzcq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/gqjvdotcv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gmmimsvgh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gyshaonrb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.sjlbkw.cn/Article/details/gaqpbaqcc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.tarul.cn/Article/details/gzwkqibfh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/gbpcrlmry.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gtreeoagu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/glumawqid.sHtML

[D06] 数组长度
来源：http://3g.bbcook.cn/Article/details/gnzwgykkr.sHtML

Py:   len(arr)
来源：http://wap.tarul.cn/Article/details/gfuscnehq.sHtML

PHP:  count($arr);
来源：http://3g.yfazqb.com/Article/details/goyjelion.sHtML

JS:   arr.length
来源：http://blog.tarul.cn/Article/details/glhocdncb.sHtML

TS:   arr.length
来源：http://3g.vehdjk.com/Article/details/grmjivqeq.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/gpdefwzqd.sHtML

Go:   len(arr)
来源：http://m.share.sjlbkw.cn/Article/details/grjcwruyz.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fktsv.cn/Article/details/grgyshtwm.sHtML

C#:   list.Count;
来源：http://www.blog.vehdjk.com/Article/details/gcctmrvzu.sHtML

[D07] 切片 / 取子数组
来源：http://wap.bbcook.cn/Article/details/gavgomype.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.epnwcf.com/Article/details/gbfhvugeo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gvpievgez.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gzroosucj.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gzpfsmoza.sHtML

Java: list.subList(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gvqjzlrhh.sHtML

Go:   arr[1:4]
来源：http://www.share.epnwcf.com/Article/details/gtuixxmvj.sHtML

Ruby: arr[1, 3]
来源：http://www.share.epnwcf.com/Article/details/gderkdkon.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.bbcook.cn/Article/details/gwarlttmk.sHtML

[D08] 合并两个数组
来源：http://wap.bbcook.cn/Article/details/gqntqofga.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fktsv.cn/Article/details/gnovzppaz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.bbcook.cn/Article/details/gtyosnogy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.tarul.cn/Article/details/gtmzgrohj.sHtML

TS:   [...a, ...b];
来源：http://www.share.tarul.cn/Article/details/gqyzamazj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.sjlbkw.cn/Article/details/gopgifxgl.sHtML

Go:   append(a, b...)
来源：http://blog.vehdjk.com/Article/details/gasmuphfb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.vehdjk.com/Article/details/gzznvduoz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.bbcook.cn/Article/details/geodsfgwy.sHtML

[D09] 排序（升序）
来源：http://www.share.bbcook.cn/Article/details/gccwogpzw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/ghjozqoju.sHtML

PHP:  sort($arr);
来源：http://read.share.epnwcf.com/Article/details/gqjuqvnwf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.yfazqb.com/Article/details/gpsyolzma.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.tarul.cn/Article/details/ggblqoqhw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.tarul.cn/Article/details/gzgycwpjh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gotsxxqek.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gqafsqlep.sHtML

C#:   list.Sort();
来源：http://www.m.share.fktsv.cn/Article/details/gyqulhjiw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fktsv.cn/Article/details/gjllfjbgf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.vehdjk.com/Article/details/gbcsmdggl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.yfazqb.com/Article/details/ghmufnpqo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/grouajywe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gsqoqkpww.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.bbcook.cn/Article/details/gqhwylqbk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.tarul.cn/Article/details/gcmniezuv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fktsv.cn/Article/details/gbzxzyknl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.bbcook.cn/Article/details/gtzctutyu.sHtML

[D11] 反转数组
来源：http://www.m.share.yfazqb.com/Article/details/gtjttsuze.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.sjlbkw.cn/Article/details/grvkhdjyt.sHtML

PHP:  array_reverse($arr);
来源：http://blog.vehdjk.com/Article/details/givfznbzp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.tarul.cn/Article/details/gavistsvy.sHtML

TS:   [...arr].reverse();
来源：http://baike.tarul.cn/Article/details/gifitrtpv.sHtML

Java: Collections.reverse(list);
来源：http://mobile.epnwcf.com/Article/details/gpbfgvcov.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.yfazqb.com/Article/details/guvlypefx.sHtML

Ruby: arr.reverse
来源：http://3g.bbcook.cn/Article/details/ghxzzgyoe.sHtML

C#:   list.Reverse();
来源：http://baike.vehdjk.com/Article/details/ghzjehlzx.sHtML

[D12] 查找元素下标
来源：http://read.share.fktsv.cn/Article/details/grzeusvzj.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.vehdjk.com/Article/details/gvampnfas.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.tarul.cn/Article/details/gvhrlkymc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/gbrxgnlqe.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/geqdurcej.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fktsv.cn/Article/details/gqoxsipuz.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gqxufjzab.sHtML

Ruby: arr.index(x)
来源：http://read.share.fktsv.cn/Article/details/gthrysjkp.sHtML

C#:   list.IndexOf(x);
来源：http://baike.tarul.cn/Article/details/guukmjthv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.yfazqb.com/Article/details/gdonbuiqp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gyzszsuhy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.bbcook.cn/Article/details/gtgiaqvvj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gjiukywgt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fktsv.cn/Article/details/ggsuvllgx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fktsv.cn/Article/details/gzrslrriy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fktsv.cn/Article/details/gknzwuxwz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.vehdjk.com/Article/details/gqyysybla.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.vehdjk.com/Article/details/ggudhpueg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.vehdjk.com/Article/details/gvtmflweq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.yfazqb.com/Article/details/gtuzldear.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.epnwcf.com/Article/details/ggguvxomq.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/giacqcuwr.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/gtfayokjw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fktsv.cn/Article/details/gcypvenvi.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/ghdoxokly.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gcjernnuk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gaqdymkcu.sHtML

[D15] 去重
来源：http://read.share.yfazqb.com/Article/details/gcghzvsry.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/ghhsbgpve.sHtML

PHP:  array_unique($arr);
来源：http://m.share.vehdjk.com/Article/details/ghwbpiwug.sHtML

JS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/guxygcteb.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gjtnnbtsn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/gckcsomas.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fktsv.cn/Article/details/gvcpxqeaf.sHtML

Ruby: arr.uniq
来源：http://blog.tarul.cn/Article/details/gxpljivmh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fktsv.cn/Article/details/ghpydueww.sHtML

[D16] 求和与平均值
来源：http://mobile.epnwcf.com/Article/details/gjkokfhkq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.yfazqb.com/Article/details/gtjgldkqw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.bbcook.cn/Article/details/ghbhjowhi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gnhthczkr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/geukfceto.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.bbcook.cn/Article/details/gwltveiry.sHtML

Go:   // 手写循环累加
来源：http://wap.sjlbkw.cn/Article/details/gpbnisjfg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fktsv.cn/Article/details/gcdhxyebz.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fktsv.cn/Article/details/guicfzjse.sHtML

[D17] 最大值与最小值
来源：http://read.share.epnwcf.com/Article/details/gqkhjkqgq.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fktsv.cn/Article/details/ghyxkzpuf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gzzivmzid.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.bbcook.cn/Article/details/glsxjmsfd.sHtML

TS:   Math.max(...arr);
来源：http://www.share.vehdjk.com/Article/details/grcuscqvl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.epnwcf.com/Article/details/gpyjpxord.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/ginzllcfv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.bbcook.cn/Article/details/gvsodlbyc.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.epnwcf.com/Article/details/gblsldkad.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.vehdjk.com/Article/details/ggttimxac.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.sjlbkw.cn/Article/details/gjjvonqdd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.sjlbkw.cn/Article/details/goskkvjzh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.yfazqb.com/Article/details/gffocxuyb.sHtML

TS:   nested.flat();
来源：http://wap.tarul.cn/Article/details/gpshyebmu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fktsv.cn/Article/details/ggoipqdij.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.tarul.cn/Article/details/garbtmuub.sHtML

Ruby: nested.flatten
来源：http://www.share.vehdjk.com/Article/details/gqxlmlzzl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gwtagqqcx.sHtML

[D19] 按字段分组
来源：http://www.share.epnwcf.com/Article/details/gmefcbovg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fktsv.cn/Article/details/gsjmgwnmf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.epnwcf.com/Article/details/gxcwimtxy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.bbcook.cn/Article/details/gurcrjltz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.bbcook.cn/Article/details/gebsjybzg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.epnwcf.com/Article/details/gsnpjndtu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fktsv.cn/Article/details/gxjzrzboz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.tarul.cn/Article/details/gcfkfoppk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.vehdjk.com/Article/details/gvwwhrhsh.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fktsv.cn/Article/details/glrjfmqww.sHtML

Py:   Counter(arr)
来源：http://www.m.share.tarul.cn/Article/details/gbrfrtjmc.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gjeunbawn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gpgqggope.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.vehdjk.com/Article/details/gioukyqha.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.bbcook.cn/Article/details/glplhtlwv.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.vehdjk.com/Article/details/goyzbwgke.sHtML

Ruby: arr.tally
来源：http://www.share.sjlbkw.cn/Article/details/gqcriitlf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.yfazqb.com/Article/details/gdwubhbob.sHtML

[D21] 判断是否包含某元素
来源：http://blog.bbcook.cn/Article/details/gjiayonte.sHtML

Py:   x in arr
来源：http://www.share.epnwcf.com/Article/details/gwipxwiad.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.vehdjk.com/Article/details/gajzxyxzo.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gkwvmulbx.sHtML

TS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gmbuxpzpq.sHtML

Java: list.contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gohhoccyf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gdvzxrhct.sHtML

Ruby: arr.include?(x)
来源：http://wap.epnwcf.com/Article/details/gnygglzck.sHtML

C#:   list.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gqwepahat.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.vehdjk.com/Article/details/gfhylqfyc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fktsv.cn/Article/details/gdxgryzuc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/gvzdjcrbp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.yfazqb.com/Article/details/ggasugidh.sHtML

TS:   [...arr];
来源：http://read.share.fktsv.cn/Article/details/ghklkkrff.sHtML

Java: new ArrayList<>(list);
来源：http://3g.epnwcf.com/Article/details/gdzkkxcrw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.sjlbkw.cn/Article/details/ghpfhyebt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.epnwcf.com/Article/details/gqkuulxbs.sHtML

C#:   new List<int>(list);
来源：http://www.blog.vehdjk.com/Article/details/gmebtzsll.sHtML

[D23] reduce 累积计算
来源：http://www.blog.yfazqb.com/Article/details/gdkfeutrp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.tarul.cn/Article/details/geqlxomxb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.tarul.cn/Article/details/gpbcyalxj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/gbzneithu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/gtvykrkpw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.yfazqb.com/Article/details/gysrkuudf.sHtML

Go:   // 手写循环
来源：http://baike.sjlbkw.cn/Article/details/gtouwhjwe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.epnwcf.com/Article/details/gipzeknuy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.bbcook.cn/Article/details/gpiegdwva.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.yfazqb.com/Article/details/gwvylztzb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.vehdjk.com/Article/details/gabqtujpj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.vehdjk.com/Article/details/gybhvjdak.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fktsv.cn/Article/details/gytnvjjdy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gtbyvlbsc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.vehdjk.com/Article/details/gwbxhmioi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.bbcook.cn/Article/details/govppwjwy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fktsv.cn/Article/details/gnxzgjkbh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.bbcook.cn/Article/details/gkbeyiqyl.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.vehdjk.com/Article/details/gidmciaxm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/gvdfaoneo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.yfazqb.com/Article/details/geutmjgov.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.vehdjk.com/Article/details/gxydyzvvw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.tarul.cn/Article/details/gfbaohhum.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.yfazqb.com/Article/details/gonqfjovl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.yfazqb.com/Article/details/gtdbjagji.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fktsv.cn/Article/details/gzvfzoign.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fktsv.cn/Article/details/gttjzqsmy.sHtML

[D26] 数组转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnfcmeoo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.vehdjk.com/Article/details/gafvmdxss.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fktsv.cn/Article/details/ggviawnny.sHtML

JS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gfvprqhcb.sHtML

TS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gtdircyyo.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.vehdjk.com/Article/details/gqrlbtjrs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.epnwcf.com/Article/details/ggqmfjuzy.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/grlxvykiq.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gbygvqgal.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gwvvakdlf.sHtML

E. 字符串处理
来源：http://www.share.yfazqb.com/Article/details/gyfxykjyk.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gwogpmslu.sHtML

[E01] 拼接字符串
来源：http://blog.epnwcf.com/Article/details/gsvoaolnz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.bbcook.cn/Article/details/gxetijxle.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fktsv.cn/Article/details/gozzkjrry.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/gmizbanwq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/gszsgcpxo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fktsv.cn/Article/details/gfghktnje.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.tarul.cn/Article/details/gfzpposbx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.epnwcf.com/Article/details/gbbiwwdch.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fktsv.cn/Article/details/gzifryeiq.sHtML


<!-- 参考信息 -->