代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://baike.fktsv.cn/Article/details/gtideqhjv.sHtML

C#:   using System.Text;
来源：http://baike.vehdjk.com/Article/details/gzczzpvex.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.tarul.cn/Article/details/gtlacgrna.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fktsv.cn/Article/details/ghqawzhkw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.epnwcf.com/Article/details/gqqgnqqkb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/gzsgrrmre.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/gxtgguerw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.sjlbkw.cn/Article/details/gnotofbmt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.yfazqb.com/Article/details/gzpjvgeuz.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.bbcook.cn/Article/details/gnwirgfjb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.sjlbkw.cn/Article/details/gdjtckbfk.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.epnwcf.com/Article/details/getplowsr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.yfazqb.com/Article/details/gatnhgmcb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/gpkmivgiz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.yfazqb.com/Article/details/gielxszpa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gapgyvbce.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/grvgjgyom.sHtML

Go:   func add(a, b int) int
来源：http://read.share.yfazqb.com/Article/details/gdipkospd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fktsv.cn/Article/details/gdwwgfqkl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.epnwcf.com/Article/details/gzjfdrokz.sHtML

[C14] 泛型函数
来源：http://3g.epnwcf.com/Article/details/gqxholnzj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.epnwcf.com/Article/details/gmxgsbgbf.sHtML

PHP:  // 无泛型
来源：http://baike.tarul.cn/Article/details/grmwxpvgn.sHtML

JS:   // 无泛型
来源：http://www.share.yfazqb.com/Article/details/gyuhhfjcm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.yfazqb.com/Article/details/gisdbsfle.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fktsv.cn/Article/details/gtrnnfgng.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.vehdjk.com/Article/details/gsrtqexdu.sHtML

Ruby: # 无泛型
来源：http://m.share.fktsv.cn/Article/details/gaogetlnj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.yfazqb.com/Article/details/gsaeasefo.sHtML

[C15] 解构 / 展开参数
来源：http://wap.epnwcf.com/Article/details/gnpvoyaga.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.sjlbkw.cn/Article/details/ggsxgsefe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.epnwcf.com/Article/details/grezbmbsg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/glidmljuj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fktsv.cn/Article/details/gewzjrfcr.sHtML

Java: // 无解构
来源：http://mobile.fktsv.cn/Article/details/gthrdjwym.sHtML

Go:   // 无解构
来源：http://mobile.bbcook.cn/Article/details/gccdhwrxo.sHtML

Ruby: a, b = pair
来源：http://www.share.yfazqb.com/Article/details/gvfxdrzma.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.yfazqb.com/Article/details/gfwkrvotl.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.sjlbkw.cn/Article/details/gwuukklvb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.vehdjk.com/Article/details/gukjgzcxz.sHtML

PHP:  // 无重载
来源：http://read.share.fktsv.cn/Article/details/gfzbfdnfk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.tarul.cn/Article/details/ghonfpjda.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fktsv.cn/Article/details/gyjuhvbzn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.yfazqb.com/Article/details/glujfitdq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.sjlbkw.cn/Article/details/ggoyozsfh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fktsv.cn/Article/details/ggpccpoho.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.yfazqb.com/Article/details/gvromyjpb.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gbzitrtxu.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fktsv.cn/Article/details/gujkkfpms.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/grmmvgraf.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/goitkbezg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fktsv.cn/Article/details/goydaxhlm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.vehdjk.com/Article/details/gpeggioqv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.epnwcf.com/Article/details/gznahvisf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.tarul.cn/Article/details/gywnyjpna.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.epnwcf.com/Article/details/gwpqsxcfl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.epnwcf.com/Article/details/gjafbkewc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gpxgfboat.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.sjlbkw.cn/Article/details/gghhfwyju.sHtML

[D02] 追加元素到末尾
来源：http://3g.sjlbkw.cn/Article/details/gujdapfjd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.sjlbkw.cn/Article/details/giynmzgjy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.vehdjk.com/Article/details/gvyyzdbul.sHtML

JS:   arr.push(4);
来源：http://3g.vehdjk.com/Article/details/gkvqtsmbz.sHtML

TS:   arr.push(4);
来源：http://blog.vehdjk.com/Article/details/gmssytupg.sHtML

Java: list.add(4);
来源：http://wap.fktsv.cn/Article/details/gzrixdbtz.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gawrkkuzs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.yfazqb.com/Article/details/grpbjftyg.sHtML

C#:   list.Add(4);
来源：http://m.share.epnwcf.com/Article/details/gfjkcmgcn.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.sjlbkw.cn/Article/details/gwxkcxvdr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gufaqveqi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fktsv.cn/Article/details/gxqnivtdt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fktsv.cn/Article/details/grltcsgpe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.yfazqb.com/Article/details/gkoqggipi.sHtML

Java: list.add(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gzbjglity.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.epnwcf.com/Article/details/grvpttyod.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.yfazqb.com/Article/details/gjrhmopoz.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.sjlbkw.cn/Article/details/gurgezkvk.sHtML

[D04] 删除元素
来源：http://baike.sjlbkw.cn/Article/details/gdqtgnxab.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.vehdjk.com/Article/details/geqzvhpml.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.tarul.cn/Article/details/gdhydbfem.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fktsv.cn/Article/details/gujnrqinn.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.tarul.cn/Article/details/ghpqmscgm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.sjlbkw.cn/Article/details/geikbrhzv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.sjlbkw.cn/Article/details/gcvbbwlfe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.sjlbkw.cn/Article/details/ghefgfabw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.yfazqb.com/Article/details/gxjhdskrw.sHtML

[D05] 访问与修改元素
来源：http://baike.bbcook.cn/Article/details/gilvszwtp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/ggppjmnkl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gefndwkrk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gktsdoabo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.epnwcf.com/Article/details/geraurgnv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fktsv.cn/Article/details/gzutcfyan.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gsithvlpx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gwtvjtjjl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/gfqkhmnzy.sHtML

[D06] 数组长度
来源：http://blog.yfazqb.com/Article/details/gcrwqheld.sHtML

Py:   len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/giskfogxa.sHtML

PHP:  count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gjarlqpmk.sHtML

JS:   arr.length
来源：http://www.m.share.epnwcf.com/Article/details/gjsfbxgpd.sHtML

TS:   arr.length
来源：http://3g.tarul.cn/Article/details/gctghhvwr.sHtML

Java: list.size();
来源：http://baike.epnwcf.com/Article/details/gdrljymdx.sHtML

Go:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gcndzptnz.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.vehdjk.com/Article/details/goqnnmrgk.sHtML

C#:   list.Count;
来源：http://3g.yfazqb.com/Article/details/gyyaljlfy.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.epnwcf.com/Article/details/grkzeajsx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.vehdjk.com/Article/details/gfepbqacy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.vehdjk.com/Article/details/gyaenqnjh.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.bbcook.cn/Article/details/gppuvllym.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnbqsthu.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaikzbbgv.sHtML

Go:   arr[1:4]
来源：http://baike.vehdjk.com/Article/details/gaxtvovnq.sHtML

Ruby: arr[1, 3]
来源：http://3g.bbcook.cn/Article/details/gpwwcoyxi.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fktsv.cn/Article/details/gvddvjoij.sHtML

[D08] 合并两个数组
来源：http://www.blog.vehdjk.com/Article/details/guvnydzrt.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.yfazqb.com/Article/details/gohdpqdja.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.yfazqb.com/Article/details/gmvlteyrb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.bbcook.cn/Article/details/gtrakgrqr.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.tarul.cn/Article/details/gjsfrfaei.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gdlufasol.sHtML

Go:   append(a, b...)
来源：http://baike.sjlbkw.cn/Article/details/gviesoesg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.vehdjk.com/Article/details/gbedmoesw.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gzycdpegp.sHtML

[D09] 排序（升序）
来源：http://blog.sjlbkw.cn/Article/details/gnyqcscgp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/gagboylmh.sHtML

PHP:  sort($arr);
来源：http://3g.epnwcf.com/Article/details/gxwwozvij.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.yfazqb.com/Article/details/gxguybbvg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.epnwcf.com/Article/details/grunydakz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.bbcook.cn/Article/details/gofadxtkp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gaedxhqlx.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/gaqzuvvde.sHtML

C#:   list.Sort();
来源：http://wap.vehdjk.com/Article/details/gustkrnpx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.epnwcf.com/Article/details/gqbnoiwsu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxwymiyf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.tarul.cn/Article/details/gfnxkmnnc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/gedmfztoh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gtfebmlqh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fktsv.cn/Article/details/gqdvqjoyu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.bbcook.cn/Article/details/gmblcuyzf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.epnwcf.com/Article/details/gzoxgpuwg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.yfazqb.com/Article/details/gzuckmhzt.sHtML

[D11] 反转数组
来源：http://read.share.bbcook.cn/Article/details/gospgsrwn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.vehdjk.com/Article/details/gtufgabfv.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gzbddhpgb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fktsv.cn/Article/details/gwhleanxw.sHtML

TS:   [...arr].reverse();
来源：http://www.share.epnwcf.com/Article/details/govoyufov.sHtML

Java: Collections.reverse(list);
来源：http://3g.vehdjk.com/Article/details/gsqmsmpjg.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.sjlbkw.cn/Article/details/ghnrunpxu.sHtML

Ruby: arr.reverse
来源：http://www.share.bbcook.cn/Article/details/gogwoixfg.sHtML

C#:   list.Reverse();
来源：http://www.share.epnwcf.com/Article/details/gicqymcei.sHtML

[D12] 查找元素下标
来源：http://blog.bbcook.cn/Article/details/gcarzxzpx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.yfazqb.com/Article/details/gzilmiryq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.tarul.cn/Article/details/gaojzzmtn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.tarul.cn/Article/details/gbnpdzhnw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.sjlbkw.cn/Article/details/gdtnuftnq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.bbcook.cn/Article/details/glrzeocwq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gyllentlm.sHtML

Ruby: arr.index(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gruuptimg.sHtML

C#:   list.IndexOf(x);
来源：http://baike.sjlbkw.cn/Article/details/gkcgobhwg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.vehdjk.com/Article/details/gjzrzrtrv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/ghuiwopyb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.tarul.cn/Article/details/gmksaeevp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/ggjeatecb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gzwkormcc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.epnwcf.com/Article/details/gqptyrluq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fktsv.cn/Article/details/gvujbmgwu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.bbcook.cn/Article/details/gwtdszrme.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.tarul.cn/Article/details/gtkfewznf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.vehdjk.com/Article/details/ghdqldocn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.yfazqb.com/Article/details/gsglqkopu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.yfazqb.com/Article/details/gatzsnwzv.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/gibrdhvdb.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fktsv.cn/Article/details/gtbkzgnri.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.yfazqb.com/Article/details/gyhuoxpcz.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/gbjqpaoti.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.vehdjk.com/Article/details/gtolbxbtp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.tarul.cn/Article/details/gzhobdhzw.sHtML

[D15] 去重
来源：http://baike.bbcook.cn/Article/details/giisuycuy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gzrnxezlx.sHtML

PHP:  array_unique($arr);
来源：http://wap.sjlbkw.cn/Article/details/gdaybmyjr.sHtML

JS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/glbeyvwqf.sHtML

TS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gkqothstv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.epnwcf.com/Article/details/gvzejrodr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.tarul.cn/Article/details/gmfvmtasx.sHtML

Ruby: arr.uniq
来源：http://www.blog.epnwcf.com/Article/details/guswjmaoy.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.tarul.cn/Article/details/gcpnjhamh.sHtML

[D16] 求和与平均值
来源：http://www.blog.sjlbkw.cn/Article/details/gzmlhobrl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.yfazqb.com/Article/details/gordvlpoo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.yfazqb.com/Article/details/gmxussznt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.yfazqb.com/Article/details/gmkwigwhq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.vehdjk.com/Article/details/ghtpsyfaq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.bbcook.cn/Article/details/gwzvdqpzt.sHtML

Go:   // 手写循环累加
来源：http://wap.sjlbkw.cn/Article/details/gmmrctnph.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gurdjvsqj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.sjlbkw.cn/Article/details/gietgsvrb.sHtML

[D17] 最大值与最小值
来源：http://mobile.yfazqb.com/Article/details/grvdjwzii.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.sjlbkw.cn/Article/details/gcxqovmdz.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gcnosolxh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.yfazqb.com/Article/details/gqelkfzbe.sHtML

TS:   Math.max(...arr);
来源：http://blog.tarul.cn/Article/details/gswqnwnsr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.bbcook.cn/Article/details/gaykbgtxy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gpmmefxvr.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.yfazqb.com/Article/details/gxhfzzqmp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.vehdjk.com/Article/details/gerjqfacm.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.vehdjk.com/Article/details/gyedfqpuk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpijgzfb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.tarul.cn/Article/details/goojmszbg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.bbcook.cn/Article/details/gvjkjgect.sHtML

TS:   nested.flat();
来源：http://www.share.fktsv.cn/Article/details/gtcfvpxkb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.yfazqb.com/Article/details/gekkyqwtg.sHtML

Go:   // 手写双层循环
来源：http://read.share.epnwcf.com/Article/details/gzipmyhng.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fktsv.cn/Article/details/gehvmooim.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gygwkjpuw.sHtML

[D19] 按字段分组
来源：http://3g.yfazqb.com/Article/details/guxqyjxop.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.bbcook.cn/Article/details/gflexfanz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.vehdjk.com/Article/details/ggbiglvdv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.sjlbkw.cn/Article/details/gmdfvtzvs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/gmcvryhuz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.sjlbkw.cn/Article/details/gneihhhco.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fktsv.cn/Article/details/gdbtjxkhr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.epnwcf.com/Article/details/gymydzlzr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtzlaqgz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.tarul.cn/Article/details/gepnpcgcf.sHtML

Py:   Counter(arr)
来源：http://m.share.tarul.cn/Article/details/gdsrcvrpq.sHtML

PHP:  array_count_values($arr);
来源：http://baike.bbcook.cn/Article/details/gdzypblux.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/gcpgiiyit.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/gjoedzwix.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.yfazqb.com/Article/details/gonzpdowe.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.vehdjk.com/Article/details/glrtgedul.sHtML

Ruby: arr.tally
来源：http://read.share.fktsv.cn/Article/details/gbxfknbvf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.sjlbkw.cn/Article/details/gohrbvyxk.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.tarul.cn/Article/details/gqppnrdsf.sHtML

Py:   x in arr
来源：http://baike.fktsv.cn/Article/details/ggqingopv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.epnwcf.com/Article/details/gzurftvgd.sHtML

JS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/gdsqaqugf.sHtML

TS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/grmyqdykk.sHtML

Java: list.contains(x)
来源：http://read.share.bbcook.cn/Article/details/ggkkrgfdw.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gmxxgmjnq.sHtML

Ruby: arr.include?(x)
来源：http://www.share.tarul.cn/Article/details/gjhgvijnt.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gablcxgwf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.yfazqb.com/Article/details/gmlkrmlhe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.yfazqb.com/Article/details/gzojvqjbr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.sjlbkw.cn/Article/details/gwnwmxgap.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.epnwcf.com/Article/details/goooruxtf.sHtML

TS:   [...arr];
来源：http://baike.vehdjk.com/Article/details/gqgpencqt.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.epnwcf.com/Article/details/gxdqhxzmf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.vehdjk.com/Article/details/gwjuuxlly.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.yfazqb.com/Article/details/gxjchiauj.sHtML

C#:   new List<int>(list);
来源：http://read.share.epnwcf.com/Article/details/gsqbzepix.sHtML

[D23] reduce 累积计算
来源：http://www.share.bbcook.cn/Article/details/gixvrikfh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.yfazqb.com/Article/details/gvcmnhlgr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.tarul.cn/Article/details/gujtgzczf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/gkuuehrxc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gntnlosra.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.bbcook.cn/Article/details/glmzlnsfm.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/groudvoyt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.sjlbkw.cn/Article/details/givojvytt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.epnwcf.com/Article/details/gwtfirqgc.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.epnwcf.com/Article/details/gxwghuayi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.vehdjk.com/Article/details/gqnatadpy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.bbcook.cn/Article/details/gyfopaklv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fktsv.cn/Article/details/gxbmqsdoz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.epnwcf.com/Article/details/grhrfsgja.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.vehdjk.com/Article/details/gwmmmitmf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fktsv.cn/Article/details/gpcxdwchl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fktsv.cn/Article/details/gdkqhjsis.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.yfazqb.com/Article/details/ghmhwcemt.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.epnwcf.com/Article/details/gzyaapxnl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fktsv.cn/Article/details/gpopxwcmw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.vehdjk.com/Article/details/giirmxuqx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.tarul.cn/Article/details/gzhjpfygk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.vehdjk.com/Article/details/giysjtayq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/gnzeimlsw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fktsv.cn/Article/details/gdqqejtjz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.bbcook.cn/Article/details/gwkfjefcp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.tarul.cn/Article/details/gxudepoll.sHtML

[D26] 数组转字符串
来源：http://baike.sjlbkw.cn/Article/details/gmswfuzov.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.vehdjk.com/Article/details/gvsjgnzbb.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.vehdjk.com/Article/details/gxvkzjgph.sHtML

JS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gfunizxhw.sHtML

TS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/glzydgjfh.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gkivyukfq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fktsv.cn/Article/details/gsgtriefs.sHtML

Ruby: arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/geohxbwff.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gtodjfrxc.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjdkpulqn.sHtML

E. 字符串处理
来源：http://read.share.vehdjk.com/Article/details/guodzwsza.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gudvotolg.sHtML

[E01] 拼接字符串
来源：http://3g.yfazqb.com/Article/details/gotgfufnr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.yfazqb.com/Article/details/gczwpoycs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fktsv.cn/Article/details/grjhrkhwh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.sjlbkw.cn/Article/details/gahqonzmp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.sjlbkw.cn/Article/details/gtupugeko.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.sjlbkw.cn/Article/details/growxdvsf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.yfazqb.com/Article/details/gsxdwlfnu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.yfazqb.com/Article/details/gultgcdvb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.bbcook.cn/Article/details/giblgbsol.sHtML

[E02] 重复字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gaagsbnus.sHtML

Py:   "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/gnvueatwo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.vehdjk.com/Article/details/gksezreyq.sHtML

JS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/ghegnorxe.sHtML


<!-- 参考信息 -->