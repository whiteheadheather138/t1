代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://wap.epnwcf.com/Article/details/gbtaswbra.sHtML

C#:   using System.Text;
来源：http://baike.fktsv.cn/Article/details/gdbygkxgh.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fktsv.cn/Article/details/gfdqgkrmd.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.yfazqb.com/Article/details/gxahyiltq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.vehdjk.com/Article/details/gcymjevod.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.bbcook.cn/Article/details/gpxaxkphx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/ghkqeotqf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.epnwcf.com/Article/details/gtthfnllp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fktsv.cn/Article/details/gvtbgjrbf.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.bbcook.cn/Article/details/ghhwikozi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.tarul.cn/Article/details/gwyhcuwrj.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fktsv.cn/Article/details/gjbgcvsei.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.vehdjk.com/Article/details/ggirmafcu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gtgwtgspa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.yfazqb.com/Article/details/gnjbqpbdi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gqwewzuhs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gqhucmznv.sHtML

Go:   func add(a, b int) int
来源：http://blog.tarul.cn/Article/details/gldqpabig.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.sjlbkw.cn/Article/details/guvtdofgv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.bbcook.cn/Article/details/gtbybousx.sHtML

[C14] 泛型函数
来源：http://www.share.fktsv.cn/Article/details/gbdiulrmp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.epnwcf.com/Article/details/gniywjsaj.sHtML

PHP:  // 无泛型
来源：http://wap.vehdjk.com/Article/details/gcxguyavm.sHtML

JS:   // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/ggobhhilb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.yfazqb.com/Article/details/gmkqefpbh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.tarul.cn/Article/details/guncpdybz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fktsv.cn/Article/details/gtttrbfmy.sHtML

Ruby: # 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gzmrtaclz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.vehdjk.com/Article/details/gsnkryiij.sHtML

[C15] 解构 / 展开参数
来源：http://blog.bbcook.cn/Article/details/gfooyykmw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.bbcook.cn/Article/details/grrpmalmb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.tarul.cn/Article/details/gykstkqqn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.bbcook.cn/Article/details/gjauhhbuu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.vehdjk.com/Article/details/gkgnhhzmt.sHtML

Java: // 无解构
来源：http://wap.epnwcf.com/Article/details/gfbkkmqwt.sHtML

Go:   // 无解构
来源：http://read.share.epnwcf.com/Article/details/gxejgwcqd.sHtML

Ruby: a, b = pair
来源：http://read.share.tarul.cn/Article/details/gbriyejdl.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.tarul.cn/Article/details/gtvedgjfr.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.epnwcf.com/Article/details/gjuhordww.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.sjlbkw.cn/Article/details/gtspmrbcf.sHtML

PHP:  // 无重载
来源：http://wap.sjlbkw.cn/Article/details/gdcsummyr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.vehdjk.com/Article/details/gbrddkgqu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.bbcook.cn/Article/details/gwesusjsf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.epnwcf.com/Article/details/ghsfgwbor.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fktsv.cn/Article/details/gykddzeao.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.vehdjk.com/Article/details/gabarhoeq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.bbcook.cn/Article/details/gnwxndbgn.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gplylpfvy.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.vehdjk.com/Article/details/gywphehgi.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggxlmodel.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/gwjrgbvlg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.sjlbkw.cn/Article/details/gxezlmryh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.yfazqb.com/Article/details/guebrzate.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.epnwcf.com/Article/details/gnypcqasv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.bbcook.cn/Article/details/gktevmbhw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/ghvyvxxje.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.vehdjk.com/Article/details/ghepjjyge.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.epnwcf.com/Article/details/ghpheqhvp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fktsv.cn/Article/details/gldxhgshe.sHtML

[D02] 追加元素到末尾
来源：http://m.share.bbcook.cn/Article/details/gvuiimwux.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/gixlgncei.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.epnwcf.com/Article/details/glhkyozco.sHtML

JS:   arr.push(4);
来源：http://baike.bbcook.cn/Article/details/gdvhmjipu.sHtML

TS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/gcdjrittb.sHtML

Java: list.add(4);
来源：http://wap.vehdjk.com/Article/details/gdtsobcsi.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.yfazqb.com/Article/details/gqnngpfcx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fktsv.cn/Article/details/gfyxgwwyp.sHtML

C#:   list.Add(4);
来源：http://baike.epnwcf.com/Article/details/gzbnzdjpx.sHtML

[D03] 在指定位置插入元素
来源：http://wap.sjlbkw.cn/Article/details/gljhjvlxb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.vehdjk.com/Article/details/gwvdehixi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.yfazqb.com/Article/details/gfmhrrxde.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.sjlbkw.cn/Article/details/glesuyhts.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.epnwcf.com/Article/details/gbhpmehhi.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gmpjcymgy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.tarul.cn/Article/details/gdsmlkret.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.sjlbkw.cn/Article/details/gvxsaxuaw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.yfazqb.com/Article/details/gctldzdml.sHtML

[D04] 删除元素
来源：http://read.share.yfazqb.com/Article/details/gtwwuwsfv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.bbcook.cn/Article/details/gyneinpzy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.vehdjk.com/Article/details/gfsspnsas.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.vehdjk.com/Article/details/gqlwwdtjn.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.bbcook.cn/Article/details/gpoquhodn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.bbcook.cn/Article/details/gztqfhqen.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.tarul.cn/Article/details/gdcejynfz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.vehdjk.com/Article/details/gykbkikwh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.vehdjk.com/Article/details/ggmgbuphs.sHtML

[D05] 访问与修改元素
来源：http://blog.sjlbkw.cn/Article/details/gtejxaqwe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gnibxxmpi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gykjtudmt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gqsrfrxmc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.vehdjk.com/Article/details/gzducjfzx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.tarul.cn/Article/details/gzrtkxoyo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gchawdvqx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gvmgofmol.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/ghoxulaoq.sHtML

[D06] 数组长度
来源：http://m.share.vehdjk.com/Article/details/ggdgkgqof.sHtML

Py:   len(arr)
来源：http://blog.vehdjk.com/Article/details/gdbdncfdw.sHtML

PHP:  count($arr);
来源：http://mobile.yfazqb.com/Article/details/gidympvqm.sHtML

JS:   arr.length
来源：http://www.share.tarul.cn/Article/details/gvfyygdqo.sHtML

TS:   arr.length
来源：http://read.share.bbcook.cn/Article/details/gidqifpxi.sHtML

Java: list.size();
来源：http://mobile.yfazqb.com/Article/details/gyvkoitzj.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gvcoifxyo.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fktsv.cn/Article/details/gnwizirlf.sHtML

C#:   list.Count;
来源：http://m.share.vehdjk.com/Article/details/gtyalsrcz.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.bbcook.cn/Article/details/gyjqljmgl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.yfazqb.com/Article/details/gjrewptit.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gmsngjype.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/gnnuhmcsc.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.bbcook.cn/Article/details/gshlbujry.sHtML

Java: list.subList(1, 4);
来源：http://wap.fktsv.cn/Article/details/gcfntgzlq.sHtML

Go:   arr[1:4]
来源：http://blog.bbcook.cn/Article/details/gurukehln.sHtML

Ruby: arr[1, 3]
来源：http://blog.vehdjk.com/Article/details/gjlldggrq.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.tarul.cn/Article/details/gckdqxxfa.sHtML

[D08] 合并两个数组
来源：http://wap.epnwcf.com/Article/details/ggcpseieu.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.epnwcf.com/Article/details/gzcucfbvx.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.yfazqb.com/Article/details/gkgabjkhv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.sjlbkw.cn/Article/details/gjtyvfgrr.sHtML

TS:   [...a, ...b];
来源：http://wap.yfazqb.com/Article/details/gokeihguz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.vehdjk.com/Article/details/gaarkgwqp.sHtML

Go:   append(a, b...)
来源：http://wap.yfazqb.com/Article/details/glxkbmehx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gouayolds.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.yfazqb.com/Article/details/gwibbeiyv.sHtML

[D09] 排序（升序）
来源：http://blog.bbcook.cn/Article/details/gzxzehizc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/gtmsbomqk.sHtML

PHP:  sort($arr);
来源：http://www.blog.yfazqb.com/Article/details/gxtbhbsit.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fktsv.cn/Article/details/gwwxqeogv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.vehdjk.com/Article/details/gdrwlpkzt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.tarul.cn/Article/details/gqvaoesty.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gjvbfyhuc.sHtML

Ruby: arr.sort
来源：http://www.blog.yfazqb.com/Article/details/gaczguqbf.sHtML

C#:   list.Sort();
来源：http://3g.fktsv.cn/Article/details/gugwlqwmq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.tarul.cn/Article/details/gqrytrnax.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.bbcook.cn/Article/details/gmkqjvwxb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/gkyqbhtwb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.epnwcf.com/Article/details/gvafomhze.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/ghxaamtdn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.yfazqb.com/Article/details/gahheeqii.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.epnwcf.com/Article/details/gifjycbyy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.yfazqb.com/Article/details/gtkckgdqq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.yfazqb.com/Article/details/gguvilucg.sHtML

[D11] 反转数组
来源：http://baike.yfazqb.com/Article/details/gwgoiafca.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.tarul.cn/Article/details/gdinkizpf.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/gvawgktpd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.bbcook.cn/Article/details/gefbkyzku.sHtML

TS:   [...arr].reverse();
来源：http://3g.fktsv.cn/Article/details/gqdeealek.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.epnwcf.com/Article/details/gqydybxnc.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.epnwcf.com/Article/details/gquhpzdlp.sHtML

Ruby: arr.reverse
来源：http://3g.fktsv.cn/Article/details/goqmyruyk.sHtML

C#:   list.Reverse();
来源：http://baike.vehdjk.com/Article/details/ghszqihfx.sHtML

[D12] 查找元素下标
来源：http://wap.epnwcf.com/Article/details/gwfmogpmi.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.vehdjk.com/Article/details/gktwosqil.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/geptchidi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fktsv.cn/Article/details/ghydatcip.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/ggtlbsbat.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.yfazqb.com/Article/details/gvmyjwabm.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.vehdjk.com/Article/details/givyknple.sHtML

Ruby: arr.index(x)
来源：http://baike.sjlbkw.cn/Article/details/gzwvkytcs.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.yfazqb.com/Article/details/gcsujowqq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fktsv.cn/Article/details/gkapboyun.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.tarul.cn/Article/details/gdxpiuxna.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fktsv.cn/Article/details/grbqgspuv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.tarul.cn/Article/details/gbnsdmogb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.bbcook.cn/Article/details/gvwvqgefk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/gzeaipacs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.tarul.cn/Article/details/gpulzeabb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.tarul.cn/Article/details/gqgkstfig.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.yfazqb.com/Article/details/ghsqjgkjt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.sjlbkw.cn/Article/details/gsbmgaxya.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.bbcook.cn/Article/details/grbmoakxe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.yfazqb.com/Article/details/gzngbjold.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gsafcxquw.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/gkafnyvea.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fktsv.cn/Article/details/gftntwcyj.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/gniufxnrc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.vehdjk.com/Article/details/goyswlxdc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.epnwcf.com/Article/details/gyrywdldy.sHtML

[D15] 去重
来源：http://wap.vehdjk.com/Article/details/graathyvk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.tarul.cn/Article/details/gnkdevtnz.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gpwovsbao.sHtML

JS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gdywkrhjq.sHtML

TS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/gqvyaquqd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.yfazqb.com/Article/details/ghxviekux.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.bbcook.cn/Article/details/gpiluqjgr.sHtML

Ruby: arr.uniq
来源：http://wap.yfazqb.com/Article/details/gepgendqw.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fktsv.cn/Article/details/gwojtznnh.sHtML

[D16] 求和与平均值
来源：http://www.blog.yfazqb.com/Article/details/gleodebac.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gmxsuexlw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gsxlqzkix.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/gjabrrkfv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/glwznxekh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.sjlbkw.cn/Article/details/gceyktqjo.sHtML

Go:   // 手写循环累加
来源：http://wap.fktsv.cn/Article/details/gydfwqirg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.bbcook.cn/Article/details/glrriecec.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.bbcook.cn/Article/details/gpngvkaqm.sHtML

[D17] 最大值与最小值
来源：http://read.share.tarul.cn/Article/details/gpdmbqnag.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/goqkgjmbs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gbfkldfta.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.tarul.cn/Article/details/gjxvqduir.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fktsv.cn/Article/details/gzquyiili.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.bbcook.cn/Article/details/gydxfviww.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.epnwcf.com/Article/details/gaanpwyaf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.vehdjk.com/Article/details/ghsylnjja.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.sjlbkw.cn/Article/details/gnazczfvr.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.epnwcf.com/Article/details/grpgjctmw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.sjlbkw.cn/Article/details/gcnstqhmi.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.vehdjk.com/Article/details/geazqwjoo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.epnwcf.com/Article/details/grahvxosf.sHtML

TS:   nested.flat();
来源：http://3g.epnwcf.com/Article/details/grqsntzzn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fktsv.cn/Article/details/gzakpnzxa.sHtML

Go:   // 手写双层循环
来源：http://www.blog.yfazqb.com/Article/details/gmabrhrmj.sHtML

Ruby: nested.flatten
来源：http://wap.sjlbkw.cn/Article/details/gwarczwle.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.tarul.cn/Article/details/glksrmvex.sHtML

[D19] 按字段分组
来源：http://www.blog.bbcook.cn/Article/details/gqdmecuhs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.sjlbkw.cn/Article/details/gghbndquo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.yfazqb.com/Article/details/gtrwqztim.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.vehdjk.com/Article/details/gywucgjae.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/gwnclxvuc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.epnwcf.com/Article/details/gaaueqkwq.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.bbcook.cn/Article/details/ggonueiek.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fktsv.cn/Article/details/geftkodnv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.vehdjk.com/Article/details/gdyjqwusj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fktsv.cn/Article/details/grbkrxdkt.sHtML

Py:   Counter(arr)
来源：http://wap.bbcook.cn/Article/details/grvzeojkw.sHtML

PHP:  array_count_values($arr);
来源：http://wap.vehdjk.com/Article/details/gugmpdeao.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gbickioro.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gddqbuuuu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.epnwcf.com/Article/details/geyqasnat.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.bbcook.cn/Article/details/gjjvcchbz.sHtML

Ruby: arr.tally
来源：http://mobile.yfazqb.com/Article/details/gbruwsvzc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.tarul.cn/Article/details/gzzztlzzm.sHtML

[D21] 判断是否包含某元素
来源：http://blog.bbcook.cn/Article/details/gtzaoydmt.sHtML

Py:   x in arr
来源：http://wap.yfazqb.com/Article/details/gzkzoldeb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.epnwcf.com/Article/details/gfltqcsug.sHtML

JS:   arr.includes(x)
来源：http://www.share.fktsv.cn/Article/details/grugqsdvs.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzicfyhjx.sHtML

Java: list.contains(x)
来源：http://blog.vehdjk.com/Article/details/gmxocceph.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gbmwmaoar.sHtML

Ruby: arr.include?(x)
来源：http://mobile.sjlbkw.cn/Article/details/ghrxknomz.sHtML

C#:   list.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/grciknefh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fktsv.cn/Article/details/gdwpiearo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.tarul.cn/Article/details/gzkuejcdt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.epnwcf.com/Article/details/gzrunevlw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.epnwcf.com/Article/details/ggagjxnlp.sHtML

TS:   [...arr];
来源：http://www.share.fktsv.cn/Article/details/gfkuvvjws.sHtML

Java: new ArrayList<>(list);
来源：http://wap.sjlbkw.cn/Article/details/gkayfqlnh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gtigxdnsx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.tarul.cn/Article/details/gqbrxhtne.sHtML

C#:   new List<int>(list);
来源：http://baike.vehdjk.com/Article/details/ggdmqfhul.sHtML

[D23] reduce 累积计算
来源：http://read.share.sjlbkw.cn/Article/details/gmucyhkhd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.epnwcf.com/Article/details/gjclvdvqe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gdwgekefn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/gwzvzjhpi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/gmhmectyx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.epnwcf.com/Article/details/gwnkzsuqr.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/gmxxjxjfo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.bbcook.cn/Article/details/gmvjgkgex.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.sjlbkw.cn/Article/details/gmdhvodhn.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.epnwcf.com/Article/details/gjfwcfrks.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fktsv.cn/Article/details/gzywvlani.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.vehdjk.com/Article/details/gdfmsjnfd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.sjlbkw.cn/Article/details/glkwlglem.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gtbgiouuc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fktsv.cn/Article/details/grapjvdqx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.tarul.cn/Article/details/gnqqpekca.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.yfazqb.com/Article/details/gsceatdww.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.tarul.cn/Article/details/gbysmpmme.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.bbcook.cn/Article/details/gvistvnji.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.bbcook.cn/Article/details/gbxdsmiyb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.yfazqb.com/Article/details/gycxfqcmt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fktsv.cn/Article/details/ghsacvlmc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.epnwcf.com/Article/details/ggtfdylpr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.epnwcf.com/Article/details/gkdyadvuw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fktsv.cn/Article/details/gzhejkryl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.vehdjk.com/Article/details/goffzydeo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.bbcook.cn/Article/details/gvkgixxdu.sHtML

[D26] 数组转字符串
来源：http://www.m.share.vehdjk.com/Article/details/guatceyfk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.bbcook.cn/Article/details/gvqvqqahj.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fktsv.cn/Article/details/gtakmlxlo.sHtML

JS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gnfeotfdk.sHtML

TS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gjmqyyxot.sHtML

Java: String.join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gcqfgkend.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.vehdjk.com/Article/details/gjljseruw.sHtML

Ruby: arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gkloxdsax.sHtML

C#:   string.Join(", ", list)
来源：http://blog.sjlbkw.cn/Article/details/gstovexmz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gbnnuymko.sHtML

E. 字符串处理
来源：http://www.m.share.tarul.cn/Article/details/gxjagphlo.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/guzmismmc.sHtML

[E01] 拼接字符串
来源：http://www.share.tarul.cn/Article/details/gzdldkiwb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.vehdjk.com/Article/details/gfpwyegbh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.yfazqb.com/Article/details/gmaproaik.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/gbltswqxe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/gpwqwtnot.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.bbcook.cn/Article/details/gspdwopnb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.tarul.cn/Article/details/gyeeysqoj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.yfazqb.com/Article/details/gdbuvivwe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gntvurnwz.sHtML

[E02] 重复字符串
来源：http://wap.bbcook.cn/Article/details/gwhvgrimn.sHtML

Py:   "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/grpbuizqj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.yfazqb.com/Article/details/gxxdwgamp.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gkcwknrsl.sHtML


<!-- 参考信息 -->