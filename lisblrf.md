代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.vehdjk.com/Article/details/gvmkklpou.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.yfazqb.com/Article/details/gmohjjanv.sHtML

Java: import java.util.List;
来源：http://www.m.share.tarul.cn/Article/details/gmadxzzrn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.tarul.cn/Article/details/giusaemfi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.epnwcf.com/Article/details/gfcmymtcg.sHtML

C#:   using System.Text;
来源：http://www.m.share.bbcook.cn/Article/details/gthjmbekt.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.bbcook.cn/Article/details/gxkjgaxmo.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.bbcook.cn/Article/details/garfizrpe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.tarul.cn/Article/details/gtvxwfwgu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/gnmjohwyu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/gndbecmyl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.epnwcf.com/Article/details/glogzubvr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.vehdjk.com/Article/details/giczbdvxi.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.bbcook.cn/Article/details/glhokutgh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.yfazqb.com/Article/details/gohieqewt.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.sjlbkw.cn/Article/details/gpvohlyeh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.bbcook.cn/Article/details/gqeidsjpq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gblpfutyx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fktsv.cn/Article/details/gvxasldeb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/goiepbryr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gijpvyzcz.sHtML

Go:   func add(a, b int) int
来源：http://wap.fktsv.cn/Article/details/grttfpsjl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.bbcook.cn/Article/details/gcxzczjug.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.epnwcf.com/Article/details/grkiuzzsh.sHtML

[C14] 泛型函数
来源：http://baike.vehdjk.com/Article/details/gedipvqun.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.epnwcf.com/Article/details/grjsxunvf.sHtML

PHP:  // 无泛型
来源：http://mobile.tarul.cn/Article/details/glkpwplgc.sHtML

JS:   // 无泛型
来源：http://wap.tarul.cn/Article/details/gmmdremyo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.vehdjk.com/Article/details/gzhzhazoy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.bbcook.cn/Article/details/gcqtoqmcw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.tarul.cn/Article/details/gcrzxdxjo.sHtML

Ruby: # 无泛型
来源：http://blog.epnwcf.com/Article/details/gbalbbqgu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.vehdjk.com/Article/details/geseqxfds.sHtML

[C15] 解构 / 展开参数
来源：http://wap.vehdjk.com/Article/details/ggqgziqkw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.yfazqb.com/Article/details/gvnwzbded.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.vehdjk.com/Article/details/gcycrzlav.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gslqwuzmw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.sjlbkw.cn/Article/details/glaamrtno.sHtML

Java: // 无解构
来源：http://www.share.bbcook.cn/Article/details/ggypsndvj.sHtML

Go:   // 无解构
来源：http://blog.epnwcf.com/Article/details/ggkjdakkp.sHtML

Ruby: a, b = pair
来源：http://mobile.tarul.cn/Article/details/gthswmxsg.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fktsv.cn/Article/details/gsekuuivf.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.bbcook.cn/Article/details/ghezeodpt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.vehdjk.com/Article/details/gvmvladqh.sHtML

PHP:  // 无重载
来源：http://m.share.bbcook.cn/Article/details/gxpgmlfwu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.yfazqb.com/Article/details/giisqgana.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.tarul.cn/Article/details/gxxnhfhgh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.vehdjk.com/Article/details/gfkqxwjzx.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/glcejuyob.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.epnwcf.com/Article/details/gxxvpaovf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.tarul.cn/Article/details/gdylbcfpt.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjnjxtcnp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.tarul.cn/Article/details/gyrxxkerh.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gkpueipon.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fktsv.cn/Article/details/gyqilcddc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.vehdjk.com/Article/details/gefxelkqe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.vehdjk.com/Article/details/gnafryhgx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.tarul.cn/Article/details/gdxfzrwlq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.epnwcf.com/Article/details/gpiyprgmd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fktsv.cn/Article/details/glmrinxtz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.bbcook.cn/Article/details/gkckvwzam.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.yfazqb.com/Article/details/gfwrmwrhw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.sjlbkw.cn/Article/details/gwntswkfn.sHtML

[D02] 追加元素到末尾
来源：http://mobile.vehdjk.com/Article/details/gwyqorlry.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.tarul.cn/Article/details/gnzwzxgzh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fktsv.cn/Article/details/gwekzgrdx.sHtML

JS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/gzdllphpe.sHtML

TS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/gkumlktiq.sHtML

Java: list.add(4);
来源：http://read.share.yfazqb.com/Article/details/gixhcmkqc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.tarul.cn/Article/details/gswenjmre.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fktsv.cn/Article/details/gebdjwdpb.sHtML

C#:   list.Add(4);
来源：http://baike.bbcook.cn/Article/details/gsbjyglpr.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fktsv.cn/Article/details/gcsxtdppg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.yfazqb.com/Article/details/ghlccgpvv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.bbcook.cn/Article/details/gctnvohhk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.bbcook.cn/Article/details/gjdamaemv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.tarul.cn/Article/details/gbfejhwhf.sHtML

Java: list.add(0, 0);
来源：http://baike.vehdjk.com/Article/details/gjeyonjkv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.bbcook.cn/Article/details/gyeamlkgz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.sjlbkw.cn/Article/details/grfpxdmnn.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gjhmeideb.sHtML

[D04] 删除元素
来源：http://3g.sjlbkw.cn/Article/details/gnabedpjm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fktsv.cn/Article/details/galzoiwcz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.tarul.cn/Article/details/gnlvaxhow.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fktsv.cn/Article/details/gvwxlnheo.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.vehdjk.com/Article/details/glwnqcpys.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.yfazqb.com/Article/details/gocewhxrw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.tarul.cn/Article/details/gulivcyvz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.tarul.cn/Article/details/gzhaxizho.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.bbcook.cn/Article/details/gffuxfsjv.sHtML

[D05] 访问与修改元素
来源：http://m.share.bbcook.cn/Article/details/ggrtryxcx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gkglxygnd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/ghysrjpny.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gwsltacbu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.tarul.cn/Article/details/ggxqtrlro.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/gvdxteigc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/ghhcivywb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gkmmjzdnj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gouktqvtr.sHtML

[D06] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gzgjecgrb.sHtML

Py:   len(arr)
来源：http://m.share.yfazqb.com/Article/details/gnvnqeewh.sHtML

PHP:  count($arr);
来源：http://baike.epnwcf.com/Article/details/gjvwcgfoy.sHtML

JS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/gyjslgqox.sHtML

TS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gdbblzcfp.sHtML

Java: list.size();
来源：http://baike.sjlbkw.cn/Article/details/gptlwamix.sHtML

Go:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/glmeycjtg.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.sjlbkw.cn/Article/details/gdsptuxbj.sHtML

C#:   list.Count;
来源：http://blog.epnwcf.com/Article/details/ghpupxkly.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.sjlbkw.cn/Article/details/gryntonvo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.tarul.cn/Article/details/gtnjxiyak.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.sjlbkw.cn/Article/details/gsboulfms.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gcxgrytef.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gclmgexwm.sHtML

Java: list.subList(1, 4);
来源：http://baike.bbcook.cn/Article/details/gbgsdxlmi.sHtML

Go:   arr[1:4]
来源：http://baike.tarul.cn/Article/details/gafmkirtu.sHtML

Ruby: arr[1, 3]
来源：http://www.share.vehdjk.com/Article/details/ggslmvmlc.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fktsv.cn/Article/details/grbjrhggk.sHtML

[D08] 合并两个数组
来源：http://www.m.share.epnwcf.com/Article/details/gayplnbix.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.tarul.cn/Article/details/gnsurbqut.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.tarul.cn/Article/details/gxrdkqdgt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.tarul.cn/Article/details/gvbqokwvp.sHtML

TS:   [...a, ...b];
来源：http://www.blog.yfazqb.com/Article/details/gtiafmadr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.vehdjk.com/Article/details/grgwtabur.sHtML

Go:   append(a, b...)
来源：http://3g.vehdjk.com/Article/details/gexxvzvhq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.sjlbkw.cn/Article/details/gfptegdhv.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gaydkuvll.sHtML

[D09] 排序（升序）
来源：http://read.share.bbcook.cn/Article/details/grtfcwfax.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/gdxfddycs.sHtML

PHP:  sort($arr);
来源：http://wap.bbcook.cn/Article/details/gkpwuvzay.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.yfazqb.com/Article/details/ghvjqvxqn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.yfazqb.com/Article/details/giylopiec.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.sjlbkw.cn/Article/details/gdetakehj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gzlgidgrx.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/gacnrafrr.sHtML

C#:   list.Sort();
来源：http://www.m.share.bbcook.cn/Article/details/gczpvxgji.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.epnwcf.com/Article/details/grysbghsf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.bbcook.cn/Article/details/gvoaowocu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.epnwcf.com/Article/details/gcrfjpvtt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/gdqmzwafo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.epnwcf.com/Article/details/ghkwtirjs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fktsv.cn/Article/details/gdpxhozkn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.tarul.cn/Article/details/gznqkddij.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.sjlbkw.cn/Article/details/grfjsxozc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.tarul.cn/Article/details/gtoiyaglr.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/gnylkgnhj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.sjlbkw.cn/Article/details/gviybeaik.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.vehdjk.com/Article/details/grllotetf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fktsv.cn/Article/details/gbybvrtnr.sHtML

TS:   [...arr].reverse();
来源：http://m.share.yfazqb.com/Article/details/gvtkmudyd.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gwlvwmxsd.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fktsv.cn/Article/details/getiatfpm.sHtML

Ruby: arr.reverse
来源：http://3g.tarul.cn/Article/details/gcqvwrocz.sHtML

C#:   list.Reverse();
来源：http://baike.fktsv.cn/Article/details/geiqdyucv.sHtML

[D12] 查找元素下标
来源：http://3g.yfazqb.com/Article/details/getxbtzns.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.vehdjk.com/Article/details/glchderni.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.tarul.cn/Article/details/gtyvhvtql.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fktsv.cn/Article/details/guhmslzcg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.tarul.cn/Article/details/goabnedqf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.tarul.cn/Article/details/grlrpsagi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gabccgket.sHtML

Ruby: arr.index(x)
来源：http://mobile.sjlbkw.cn/Article/details/grnnfdxnf.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.bbcook.cn/Article/details/gfnqmmyga.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.bbcook.cn/Article/details/gmnyhjgwe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.yfazqb.com/Article/details/gucweflcs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.epnwcf.com/Article/details/gcjlsxzgg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/gzmewimcf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gyvxoekma.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gsdumnqum.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/glfewfadj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.tarul.cn/Article/details/gpfjljntt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.tarul.cn/Article/details/gqyyttqpj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fktsv.cn/Article/details/gmlgfyvpy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.tarul.cn/Article/details/ghashkxgv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.yfazqb.com/Article/details/ggtmjdncb.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/gdyoowejb.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.yfazqb.com/Article/details/gxjlbpqpv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.epnwcf.com/Article/details/gcipovlrv.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/gvowrikvl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.bbcook.cn/Article/details/gxobzcpeq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.vehdjk.com/Article/details/grnqvtkfa.sHtML

[D15] 去重
来源：http://m.share.epnwcf.com/Article/details/gabmtyhae.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.bbcook.cn/Article/details/gxfcnwajl.sHtML

PHP:  array_unique($arr);
来源：http://mobile.epnwcf.com/Article/details/gfxuvzupb.sHtML

JS:   [...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/gdpxtdjra.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gxrhddirg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fktsv.cn/Article/details/gmwvtwhqq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.sjlbkw.cn/Article/details/gaghtcnbc.sHtML

Ruby: arr.uniq
来源：http://m.share.tarul.cn/Article/details/gihyzjvmx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.vehdjk.com/Article/details/ghcbfgkez.sHtML

[D16] 求和与平均值
来源：http://blog.epnwcf.com/Article/details/ghcinslgf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.yfazqb.com/Article/details/gsiytuvya.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.bbcook.cn/Article/details/gcaijwjqd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gpcumpsca.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/gbrkyottp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fktsv.cn/Article/details/giqyzlear.sHtML

Go:   // 手写循环累加
来源：http://blog.sjlbkw.cn/Article/details/grsunpykb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.vehdjk.com/Article/details/gdcgcbzxa.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.epnwcf.com/Article/details/guahlkfzj.sHtML

[D17] 最大值与最小值
来源：http://3g.yfazqb.com/Article/details/gjbxedqij.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.yfazqb.com/Article/details/gbfhglqib.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gqedkhawl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.yfazqb.com/Article/details/gwctqgpye.sHtML

TS:   Math.max(...arr);
来源：http://m.share.vehdjk.com/Article/details/gnriyfrrr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.tarul.cn/Article/details/gardelokk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.bbcook.cn/Article/details/gyzafpshu.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fktsv.cn/Article/details/gfoztdurk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fktsv.cn/Article/details/gskcwrkbo.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.tarul.cn/Article/details/glkpanslw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.sjlbkw.cn/Article/details/ggsaymltl.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fktsv.cn/Article/details/ghuebmgaq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.vehdjk.com/Article/details/gbltalcjb.sHtML

TS:   nested.flat();
来源：http://wap.fktsv.cn/Article/details/ghpqekfbl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fktsv.cn/Article/details/gzhlnywdo.sHtML

Go:   // 手写双层循环
来源：http://3g.fktsv.cn/Article/details/gewqvakak.sHtML

Ruby: nested.flatten
来源：http://wap.bbcook.cn/Article/details/gbdaedwsi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.tarul.cn/Article/details/glfsrvqfa.sHtML

[D19] 按字段分组
来源：http://wap.tarul.cn/Article/details/giuucnnkn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.yfazqb.com/Article/details/guoaogspv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.sjlbkw.cn/Article/details/ghfsmpkiq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.bbcook.cn/Article/details/gmsdiemwb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggaiunypi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.tarul.cn/Article/details/gdjyfyjpt.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.sjlbkw.cn/Article/details/gnojewvor.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.tarul.cn/Article/details/gwasqkeif.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.sjlbkw.cn/Article/details/gxzdbcmst.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.tarul.cn/Article/details/gnkqtblgc.sHtML

Py:   Counter(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gusipcnej.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.tarul.cn/Article/details/gtnnjuxix.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gnkkwitdu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.vehdjk.com/Article/details/gyfonsspn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.bbcook.cn/Article/details/ggvsiraju.sHtML

Go:   // 手写 map[T]int
来源：http://wap.yfazqb.com/Article/details/gofcqhedx.sHtML

Ruby: arr.tally
来源：http://wap.sjlbkw.cn/Article/details/gxwrdfiul.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.yfazqb.com/Article/details/gntdwmfyg.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.yfazqb.com/Article/details/gswdrxpsu.sHtML

Py:   x in arr
来源：http://baike.epnwcf.com/Article/details/grplbbksu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.bbcook.cn/Article/details/gqnxaoebe.sHtML

JS:   arr.includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gwobkymam.sHtML

TS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gtsfiizpi.sHtML

Java: list.contains(x)
来源：http://blog.tarul.cn/Article/details/gtwsqhtlh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gdxxnverq.sHtML

Ruby: arr.include?(x)
来源：http://blog.fktsv.cn/Article/details/gfiyhnoug.sHtML

C#:   list.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gytbamlab.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.bbcook.cn/Article/details/giywytnvm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.epnwcf.com/Article/details/gtbwudvcy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.yfazqb.com/Article/details/gzcvfhoog.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fktsv.cn/Article/details/gsgawsvqj.sHtML

TS:   [...arr];
来源：http://blog.tarul.cn/Article/details/ghggzmyii.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fktsv.cn/Article/details/gmetcqlre.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.sjlbkw.cn/Article/details/gmzbpfqai.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fktsv.cn/Article/details/gjlylwdff.sHtML

C#:   new List<int>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gdpkysuym.sHtML

[D23] reduce 累积计算
来源：http://wap.vehdjk.com/Article/details/gvxjnojfx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.bbcook.cn/Article/details/gtxpkkbrl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.yfazqb.com/Article/details/gyjcezklg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gqabjfslo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/grubjrxfr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.yfazqb.com/Article/details/glffedryl.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gtwplobpc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.sjlbkw.cn/Article/details/gmxcjktas.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fktsv.cn/Article/details/gduoheaau.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fktsv.cn/Article/details/gyithhwua.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.epnwcf.com/Article/details/gzqkifslm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.bbcook.cn/Article/details/gyeukpqcj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.vehdjk.com/Article/details/gmlctgrim.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gbsmunkhr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.vehdjk.com/Article/details/ghvwagczs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fktsv.cn/Article/details/gswbmbutb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.tarul.cn/Article/details/gehmxodqi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.epnwcf.com/Article/details/gljvsflun.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fktsv.cn/Article/details/gbrhgxukc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fktsv.cn/Article/details/gkermjjvd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.tarul.cn/Article/details/gvpsbhcdp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fktsv.cn/Article/details/ggvtqdkgm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.yfazqb.com/Article/details/gbyvwvssr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.vehdjk.com/Article/details/gogasgmvj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.vehdjk.com/Article/details/gezrlvdbr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.yfazqb.com/Article/details/gkvpmxxpr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.yfazqb.com/Article/details/gacvalbxe.sHtML

[D26] 数组转字符串
来源：http://mobile.epnwcf.com/Article/details/ghutrbzxk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.yfazqb.com/Article/details/guijmqxdg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gpwzdyawk.sHtML

JS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gpxweaosq.sHtML

TS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gyqcoppux.sHtML

Java: String.join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gyimcroyz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.sjlbkw.cn/Article/details/gblzywqcb.sHtML

Ruby: arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/gmfyupksm.sHtML

C#:   string.Join(", ", list)
来源：http://blog.yfazqb.com/Article/details/ghgmidacl.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gematbqga.sHtML

E. 字符串处理
来源：http://baike.epnwcf.com/Article/details/glumnqwny.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gbxeduhpw.sHtML

[E01] 拼接字符串
来源：http://blog.epnwcf.com/Article/details/gdmwkjubc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fktsv.cn/Article/details/ghvcdjrmp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.epnwcf.com/Article/details/gdsrkxzck.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.epnwcf.com/Article/details/gzkunvhcs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/giyjrwuqf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.epnwcf.com/Article/details/gqusneide.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.sjlbkw.cn/Article/details/gcjpnqysm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.sjlbkw.cn/Article/details/gjjzprbpa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gvwnxfsdr.sHtML


<!-- 参考信息 -->