代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaswdybn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.tarul.cn/Article/details/gsvpheezx.sHtML

Java: import java.util.List;
来源：http://baike.yfazqb.com/Article/details/gjmcuhvvc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.vehdjk.com/Article/details/gibdaiiyp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.bbcook.cn/Article/details/gpcztbcga.sHtML

C#:   using System.Text;
来源：http://3g.sjlbkw.cn/Article/details/gwnzdsxbi.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.epnwcf.com/Article/details/gtpkdgqrh.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.yfazqb.com/Article/details/glkeylydu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.vehdjk.com/Article/details/gytziicwj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/gcmwnnvzn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.epnwcf.com/Article/details/gtnedykww.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.tarul.cn/Article/details/gyptuoimf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.epnwcf.com/Article/details/ggkiydgch.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.sjlbkw.cn/Article/details/gteopjqcy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fktsv.cn/Article/details/gphvdufud.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.bbcook.cn/Article/details/gbhrmifbe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.vehdjk.com/Article/details/gcjmbdvcm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gbkhrclec.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.bbcook.cn/Article/details/gbqrdrpje.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gxdjwckqu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gkasnhqlu.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.sjlbkw.cn/Article/details/gtaaedlti.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.vehdjk.com/Article/details/gfwxuudhe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.yfazqb.com/Article/details/getphkoov.sHtML

[C14] 泛型函数
来源：http://www.share.sjlbkw.cn/Article/details/gtzagpsxs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.epnwcf.com/Article/details/gjlubyeek.sHtML

PHP:  // 无泛型
来源：http://www.blog.yfazqb.com/Article/details/ghjmndlbw.sHtML

JS:   // 无泛型
来源：http://baike.vehdjk.com/Article/details/gjfpowuvp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.yfazqb.com/Article/details/gpgeessav.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.tarul.cn/Article/details/gyfntscgt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.bbcook.cn/Article/details/gcqamdwzm.sHtML

Ruby: # 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gpayuvtcj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.bbcook.cn/Article/details/gmisjgbzi.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gadfygkkm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.sjlbkw.cn/Article/details/gjmhgwone.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.tarul.cn/Article/details/gwiirulvx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.bbcook.cn/Article/details/glovrnova.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.sjlbkw.cn/Article/details/gyzxdvjgs.sHtML

Java: // 无解构
来源：http://baike.sjlbkw.cn/Article/details/gdhwkbtib.sHtML

Go:   // 无解构
来源：http://www.share.fktsv.cn/Article/details/gzdikmwxe.sHtML

Ruby: a, b = pair
来源：http://www.share.epnwcf.com/Article/details/gzcvdymfj.sHtML

C#:   var (a, b) = pair;
来源：http://wap.bbcook.cn/Article/details/gztcnprwy.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fktsv.cn/Article/details/glruzcqed.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.yfazqb.com/Article/details/gpbopcufe.sHtML

PHP:  // 无重载
来源：http://blog.fktsv.cn/Article/details/galzxllbf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.vehdjk.com/Article/details/gnidjplxr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.epnwcf.com/Article/details/gqmngcbrx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.tarul.cn/Article/details/gjyvpnhcs.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.bbcook.cn/Article/details/gpzsrqbvs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.bbcook.cn/Article/details/gdhervdll.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.bbcook.cn/Article/details/giwdbcrbd.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/geypxwdla.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.epnwcf.com/Article/details/gqinagjam.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghdaipsjx.sHtML

[D01] 创建数组 / 列表
来源：http://wap.vehdjk.com/Article/details/gwgpfhvan.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.epnwcf.com/Article/details/gxwtlmwvg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fktsv.cn/Article/details/gtvdgbulc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.vehdjk.com/Article/details/glulwamwt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fktsv.cn/Article/details/gicjdzoow.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/gvovhcqvs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.vehdjk.com/Article/details/gkrsfaogq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.tarul.cn/Article/details/ggffhvlhk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.bbcook.cn/Article/details/glohhteef.sHtML

[D02] 追加元素到末尾
来源：http://m.share.sjlbkw.cn/Article/details/gfzwakcpw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fktsv.cn/Article/details/gkalnuzut.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.bbcook.cn/Article/details/gyvdnhows.sHtML

JS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/gfnsbxtfq.sHtML

TS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/gqmcngzpf.sHtML

Java: list.add(4);
来源：http://wap.sjlbkw.cn/Article/details/giuspombr.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.sjlbkw.cn/Article/details/gnavebysg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.yfazqb.com/Article/details/gyggttyxr.sHtML

C#:   list.Add(4);
来源：http://blog.vehdjk.com/Article/details/ghcvkzgra.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.epnwcf.com/Article/details/gynskmjwt.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.epnwcf.com/Article/details/gmcqpcnrg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.yfazqb.com/Article/details/gdqgezqzp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.yfazqb.com/Article/details/gabxeyena.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.tarul.cn/Article/details/gucmbezli.sHtML

Java: list.add(0, 0);
来源：http://www.blog.tarul.cn/Article/details/gbzsfwgej.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.bbcook.cn/Article/details/gtlwdayrk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.tarul.cn/Article/details/gvdfidxse.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.bbcook.cn/Article/details/ghgctxkqo.sHtML

[D04] 删除元素
来源：http://www.blog.fktsv.cn/Article/details/gmlkwtcyb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.tarul.cn/Article/details/gdfddfskf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.yfazqb.com/Article/details/gvuvpzkgz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.vehdjk.com/Article/details/gbekepfsw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.sjlbkw.cn/Article/details/gbgyhqxhi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fktsv.cn/Article/details/gybwizedl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fktsv.cn/Article/details/ghsapqxzf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fktsv.cn/Article/details/gukzlrdyu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.bbcook.cn/Article/details/gxwltpwap.sHtML

[D05] 访问与修改元素
来源：http://read.share.bbcook.cn/Article/details/gputzblsx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gpnwexvyn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/gmcedlwxf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/giscmnmzp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.tarul.cn/Article/details/gldizexak.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.tarul.cn/Article/details/gfnvaietg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/gpdlayfhu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gcfebizab.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.tarul.cn/Article/details/gungpdhmo.sHtML

[D06] 数组长度
来源：http://wap.sjlbkw.cn/Article/details/glxvekwvn.sHtML

Py:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gyslokufh.sHtML

PHP:  count($arr);
来源：http://3g.bbcook.cn/Article/details/gyrjeikyz.sHtML

JS:   arr.length
来源：http://m.share.bbcook.cn/Article/details/gfuksypwg.sHtML

TS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/gyozwclyt.sHtML

Java: list.size();
来源：http://www.m.share.vehdjk.com/Article/details/gettbpqwf.sHtML

Go:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gfdffszrp.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.vehdjk.com/Article/details/gnwgcvyav.sHtML

C#:   list.Count;
来源：http://www.share.sjlbkw.cn/Article/details/gnwwudwoc.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fktsv.cn/Article/details/gdpbkjrvr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.tarul.cn/Article/details/gfejexuze.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.yfazqb.com/Article/details/glymucebd.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/glhzkejjc.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gkbqglkzf.sHtML

Java: list.subList(1, 4);
来源：http://3g.epnwcf.com/Article/details/gmwhzpajx.sHtML

Go:   arr[1:4]
来源：http://baike.epnwcf.com/Article/details/gzgxhtjoc.sHtML

Ruby: arr[1, 3]
来源：http://m.share.tarul.cn/Article/details/grdysdebw.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fktsv.cn/Article/details/gsrefpikj.sHtML

[D08] 合并两个数组
来源：http://m.share.epnwcf.com/Article/details/ggyyysico.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.vehdjk.com/Article/details/ghccfxdjm.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.yfazqb.com/Article/details/gxaddwjjv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.vehdjk.com/Article/details/gniurljhp.sHtML

TS:   [...a, ...b];
来源：http://read.share.fktsv.cn/Article/details/gzyiagzkx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.epnwcf.com/Article/details/gtjefdpev.sHtML

Go:   append(a, b...)
来源：http://3g.tarul.cn/Article/details/gpaiffkby.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.bbcook.cn/Article/details/gyqxvqrxy.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.epnwcf.com/Article/details/gxkmljczu.sHtML

[D09] 排序（升序）
来源：http://www.share.bbcook.cn/Article/details/gmlusgehy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gceurizak.sHtML

PHP:  sort($arr);
来源：http://read.share.fktsv.cn/Article/details/gsgqrcnpz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.vehdjk.com/Article/details/gslafgblf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.bbcook.cn/Article/details/ggolhgfaf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.epnwcf.com/Article/details/grqipyjez.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gvehhqumn.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/gsbfyiimy.sHtML

C#:   list.Sort();
来源：http://www.share.epnwcf.com/Article/details/gsvdgcwnh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.bbcook.cn/Article/details/grammnils.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.yfazqb.com/Article/details/gzkmfbvvy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gcvxzpchh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gmpelczpt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gnyytauja.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.yfazqb.com/Article/details/gtscalwzx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.epnwcf.com/Article/details/gmtzzxpjj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fktsv.cn/Article/details/giqpnbfih.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwljdhib.sHtML

[D11] 反转数组
来源：http://3g.vehdjk.com/Article/details/gmmstrhod.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/gtiuxcthh.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.tarul.cn/Article/details/gchimbzra.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.epnwcf.com/Article/details/gcssibmwm.sHtML

TS:   [...arr].reverse();
来源：http://read.share.yfazqb.com/Article/details/gkzpovisk.sHtML

Java: Collections.reverse(list);
来源：http://3g.yfazqb.com/Article/details/ganlbgktn.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.tarul.cn/Article/details/goxjwjtrh.sHtML

Ruby: arr.reverse
来源：http://www.blog.vehdjk.com/Article/details/gzgeumytv.sHtML

C#:   list.Reverse();
来源：http://www.share.yfazqb.com/Article/details/govhxjsfa.sHtML

[D12] 查找元素下标
来源：http://mobile.yfazqb.com/Article/details/gqfzdvfcd.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.epnwcf.com/Article/details/geuqlxjqf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fktsv.cn/Article/details/gjjcysaus.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/glynxsigo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.bbcook.cn/Article/details/gmgeemiyy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.epnwcf.com/Article/details/gvibdhggq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/ghwxsuhen.sHtML

Ruby: arr.index(x)
来源：http://m.share.vehdjk.com/Article/details/guxgtdoke.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.sjlbkw.cn/Article/details/gfaancsdm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.epnwcf.com/Article/details/gxostoies.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fktsv.cn/Article/details/gzzzlpufk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fktsv.cn/Article/details/gfosmdjro.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.tarul.cn/Article/details/gblylwkkj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/ggzlsurwr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.yfazqb.com/Article/details/gpxffdjct.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.tarul.cn/Article/details/gxpqeirwg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.vehdjk.com/Article/details/grrotgebx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fktsv.cn/Article/details/gmeidtmos.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.yfazqb.com/Article/details/gvpwcdkaw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gfimebzgu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gncxrhsuz.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/gacplnfaf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gdtulyilz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.vehdjk.com/Article/details/ghhvjxaua.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gdzoogkrl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.bbcook.cn/Article/details/gxxlotfbs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gdofopgme.sHtML

[D15] 去重
来源：http://read.share.vehdjk.com/Article/details/gqvnepowf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gqwimjboc.sHtML

PHP:  array_unique($arr);
来源：http://www.share.vehdjk.com/Article/details/gfknaafva.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gvftyaxgn.sHtML

TS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/gmviejrzd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.yfazqb.com/Article/details/gnoqtfpfx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fktsv.cn/Article/details/gujtxaxnx.sHtML

Ruby: arr.uniq
来源：http://3g.bbcook.cn/Article/details/gbokzhqcn.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.yfazqb.com/Article/details/gqzpwtapd.sHtML

[D16] 求和与平均值
来源：http://www.m.share.bbcook.cn/Article/details/gjwvpdgep.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.tarul.cn/Article/details/gcoppwtmt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.tarul.cn/Article/details/gqjfwdvvj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/gkqtumurc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gctlfxiut.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.vehdjk.com/Article/details/gnwwktklq.sHtML

Go:   // 手写循环累加
来源：http://baike.vehdjk.com/Article/details/gtqgthjqr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.yfazqb.com/Article/details/gwvmytcno.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.bbcook.cn/Article/details/gubwirbnq.sHtML

[D17] 最大值与最小值
来源：http://www.share.sjlbkw.cn/Article/details/gvbqfcyzj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gehpyfdge.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.bbcook.cn/Article/details/gcbsjlbfo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.bbcook.cn/Article/details/gcxaxniqb.sHtML

TS:   Math.max(...arr);
来源：http://read.share.yfazqb.com/Article/details/gfkdcjpsp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fktsv.cn/Article/details/gpzbfahsv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.bbcook.cn/Article/details/gxrsjccmv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.sjlbkw.cn/Article/details/grhcvjujy.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.epnwcf.com/Article/details/gmatixlhz.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.sjlbkw.cn/Article/details/guropusjw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.epnwcf.com/Article/details/gidodawtg.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.sjlbkw.cn/Article/details/gddokirfq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.tarul.cn/Article/details/gfevazcur.sHtML

TS:   nested.flat();
来源：http://baike.bbcook.cn/Article/details/gvivflbym.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbpkodzm.sHtML

Go:   // 手写双层循环
来源：http://read.share.epnwcf.com/Article/details/gymxmxtlv.sHtML

Ruby: nested.flatten
来源：http://read.share.bbcook.cn/Article/details/gqwqnlvpu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.epnwcf.com/Article/details/gtlvzfzjh.sHtML

[D19] 按字段分组
来源：http://mobile.sjlbkw.cn/Article/details/gxbtkusaj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.epnwcf.com/Article/details/gnnbcijif.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.tarul.cn/Article/details/gzvlhvgfi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.epnwcf.com/Article/details/gpawnmjpi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/gptsfvpib.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.sjlbkw.cn/Article/details/girovzxcn.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.vehdjk.com/Article/details/gahjtzqtt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.bbcook.cn/Article/details/gumaehwiw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.yfazqb.com/Article/details/gklxwjiqt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gjbuenneq.sHtML

Py:   Counter(arr)
来源：http://3g.vehdjk.com/Article/details/gywhbiqgh.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fktsv.cn/Article/details/gwpuysbrc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.yfazqb.com/Article/details/ggctblayl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/givcwvglx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.epnwcf.com/Article/details/gtuuslaar.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.tarul.cn/Article/details/ghglunvpd.sHtML

Ruby: arr.tally
来源：http://read.share.fktsv.cn/Article/details/geutvwvez.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.tarul.cn/Article/details/gzaocfqjc.sHtML

[D21] 判断是否包含某元素
来源：http://blog.epnwcf.com/Article/details/gjxlsbgne.sHtML

Py:   x in arr
来源：http://blog.fktsv.cn/Article/details/gmtaijcxs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.yfazqb.com/Article/details/gszoknkew.sHtML

JS:   arr.includes(x)
来源：http://read.share.fktsv.cn/Article/details/gktmkdlrx.sHtML

TS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/glmfrdkfu.sHtML

Java: list.contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gjohdnfbo.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.bbcook.cn/Article/details/gheuswymn.sHtML

Ruby: arr.include?(x)
来源：http://3g.yfazqb.com/Article/details/gvlbblfkm.sHtML

C#:   list.Contains(x)
来源：http://3g.yfazqb.com/Article/details/gmlqeywfw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.epnwcf.com/Article/details/gjoznruua.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.tarul.cn/Article/details/goyoabisj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.yfazqb.com/Article/details/gkoxagwgo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.tarul.cn/Article/details/ghdxgflmp.sHtML

TS:   [...arr];
来源：http://wap.fktsv.cn/Article/details/gsizirafo.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.yfazqb.com/Article/details/gkosihwoa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.bbcook.cn/Article/details/gofblopvv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.yfazqb.com/Article/details/gbodxjnjo.sHtML

C#:   new List<int>(list);
来源：http://3g.epnwcf.com/Article/details/gnpbsrjeo.sHtML

[D23] reduce 累积计算
来源：http://www.share.yfazqb.com/Article/details/gurlglvvq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.vehdjk.com/Article/details/gffnhabmk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.epnwcf.com/Article/details/gzobqhyse.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/gsaeqtovj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gandokzpk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.sjlbkw.cn/Article/details/gjtltjsbr.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/gfdccdtuk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.vehdjk.com/Article/details/gugsoalqj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.epnwcf.com/Article/details/gqvhfzixi.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.sjlbkw.cn/Article/details/gmqfbcjsr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.vehdjk.com/Article/details/gwsrilkbu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.yfazqb.com/Article/details/ghiofdnyx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.bbcook.cn/Article/details/gnkniyuqo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gcawjegmv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.epnwcf.com/Article/details/gugduipqd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.vehdjk.com/Article/details/gzarwpkcu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fktsv.cn/Article/details/gdqwcmxmv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.tarul.cn/Article/details/gzvxbqoyb.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fktsv.cn/Article/details/gopsbaxpn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.tarul.cn/Article/details/gmwscvsob.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.yfazqb.com/Article/details/gineqldtw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.epnwcf.com/Article/details/giuaeohwa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.vehdjk.com/Article/details/ghwgezert.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.tarul.cn/Article/details/gbxnrlfih.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.sjlbkw.cn/Article/details/gofnhxhds.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.yfazqb.com/Article/details/gkdlxztba.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fktsv.cn/Article/details/gybhrwnsv.sHtML

[D26] 数组转字符串
来源：http://baike.epnwcf.com/Article/details/gpfoczojc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmpjcozx.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.yfazqb.com/Article/details/gecuirvqr.sHtML

JS:   arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gsgnontpq.sHtML

TS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gnfnwxyvf.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fktsv.cn/Article/details/gkcdahyvv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fktsv.cn/Article/details/gkvlnaqlf.sHtML

Ruby: arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gxeamfeoe.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/gzzfmgubh.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gudcwhmxo.sHtML

E. 字符串处理
来源：http://m.share.yfazqb.com/Article/details/gnkraswgs.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gtsosdwyh.sHtML

[E01] 拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gwdyzbmuk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.tarul.cn/Article/details/gympxeaiw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.sjlbkw.cn/Article/details/gpoawomat.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gwdxztipr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/glpsssory.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.epnwcf.com/Article/details/gsvxjlpgz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.bbcook.cn/Article/details/gswwyvaus.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fktsv.cn/Article/details/guzjtkzsw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.bbcook.cn/Article/details/gqmnfgasu.sHtML


<!-- 参考信息 -->