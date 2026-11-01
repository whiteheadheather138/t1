代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://read.share.vehdjk.com/Article/details/gqjsamaxm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fktsv.cn/Article/details/gbhkjnovl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.yfazqb.com/Article/details/gymjwlmfr.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.sjlbkw.cn/Article/details/gnnbuozhc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.vehdjk.com/Article/details/gzzbmolxc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gzwgkaujg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.tarul.cn/Article/details/gwrwvqgsc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gvormqasm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gyikbdzyw.sHtML

Go:   func add(a, b int) int
来源：http://blog.vehdjk.com/Article/details/gxfxdxqpx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.yfazqb.com/Article/details/gqhllfhgx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.tarul.cn/Article/details/gmpdyifaz.sHtML

[C14] 泛型函数
来源：http://read.share.sjlbkw.cn/Article/details/gjvzrxpee.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.vehdjk.com/Article/details/gufdysomv.sHtML

PHP:  // 无泛型
来源：http://www.share.vehdjk.com/Article/details/gbyluxiuj.sHtML

JS:   // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gescnmavr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.bbcook.cn/Article/details/gqgnjreqv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.tarul.cn/Article/details/gtpqfbrat.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.epnwcf.com/Article/details/gihnhunov.sHtML

Ruby: # 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gmnsdbezj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.vehdjk.com/Article/details/glfocrbtb.sHtML

[C15] 解构 / 展开参数
来源：http://baike.vehdjk.com/Article/details/ggknfdbyh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.tarul.cn/Article/details/ggkyulzmy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fktsv.cn/Article/details/gfoeskokv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gvfbswhoo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fktsv.cn/Article/details/gqsefgfmk.sHtML

Java: // 无解构
来源：http://blog.epnwcf.com/Article/details/gmskiolwb.sHtML

Go:   // 无解构
来源：http://www.share.vehdjk.com/Article/details/gpvlcrcvy.sHtML

Ruby: a, b = pair
来源：http://wap.fktsv.cn/Article/details/gllerrayt.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.yfazqb.com/Article/details/ggvjfdcwl.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.yfazqb.com/Article/details/gkhjycywv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fktsv.cn/Article/details/geuqzzjow.sHtML

PHP:  // 无重载
来源：http://mobile.fktsv.cn/Article/details/gzwwqtzjc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.sjlbkw.cn/Article/details/gunmwsqoa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.tarul.cn/Article/details/gyvggzdrx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.vehdjk.com/Article/details/gwwoqykoy.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fktsv.cn/Article/details/gnvkcebcz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.bbcook.cn/Article/details/grttcmskr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.vehdjk.com/Article/details/ggqomyknm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxqkgfebv.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.bbcook.cn/Article/details/grbnhcnqr.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gnrbmydqt.sHtML

[D01] 创建数组 / 列表
来源：http://wap.tarul.cn/Article/details/ghlrrbawk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.bbcook.cn/Article/details/gxildmrqo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhucwzbg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.tarul.cn/Article/details/gxowvlgle.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.bbcook.cn/Article/details/gzfqihkty.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.bbcook.cn/Article/details/gatpneghp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fktsv.cn/Article/details/gtxjibwqg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.yfazqb.com/Article/details/gtmyiiljs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.sjlbkw.cn/Article/details/gxffctdpc.sHtML

[D02] 追加元素到末尾
来源：http://3g.vehdjk.com/Article/details/gnsmvqqag.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.tarul.cn/Article/details/gicohmncr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fktsv.cn/Article/details/gyenjimlj.sHtML

JS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/gjlzlhsfz.sHtML

TS:   arr.push(4);
来源：http://www.blog.epnwcf.com/Article/details/gobqbnyzi.sHtML

Java: list.add(4);
来源：http://blog.bbcook.cn/Article/details/gvegoeljx.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fktsv.cn/Article/details/gxqjogfgo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.tarul.cn/Article/details/gowvyymin.sHtML

C#:   list.Add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gxfumyjzh.sHtML

[D03] 在指定位置插入元素
来源：http://baike.tarul.cn/Article/details/gdhdcdhce.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.tarul.cn/Article/details/gqgtceiut.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.bbcook.cn/Article/details/gsfoidmpn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.yfazqb.com/Article/details/gbinoiliv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.sjlbkw.cn/Article/details/geczwinyn.sHtML

Java: list.add(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gjottbgwx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fktsv.cn/Article/details/gvvbxdbmu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fktsv.cn/Article/details/gvxoooxxj.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.tarul.cn/Article/details/gkuwsxafk.sHtML

[D04] 删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/gltjsznti.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.epnwcf.com/Article/details/gebjhtpvi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.bbcook.cn/Article/details/ghtwiuoae.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.bbcook.cn/Article/details/gjsshxadi.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.vehdjk.com/Article/details/giwjxitdt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.yfazqb.com/Article/details/gaipmfxfh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fktsv.cn/Article/details/gysvllpbs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.yfazqb.com/Article/details/gxkwcygnl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.sjlbkw.cn/Article/details/gwfxsvjtp.sHtML

[D05] 访问与修改元素
来源：http://wap.tarul.cn/Article/details/grvfmzyzu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gbvmxvkio.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/guratcqdb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gumpjpowx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.sjlbkw.cn/Article/details/getkhuvpd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.epnwcf.com/Article/details/gvrdbzkxt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/ghpesqeol.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gbayhcgwt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gyokzxeeb.sHtML

[D06] 数组长度
来源：http://mobile.sjlbkw.cn/Article/details/gtptzhwsf.sHtML

Py:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/gpfcqbxcf.sHtML

PHP:  count($arr);
来源：http://mobile.vehdjk.com/Article/details/gmpugddvm.sHtML

JS:   arr.length
来源：http://www.share.fktsv.cn/Article/details/guciwxski.sHtML

TS:   arr.length
来源：http://blog.tarul.cn/Article/details/gekvujbjk.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/gzilyywig.sHtML

Go:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gxmfsjcsk.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gvoyttwpb.sHtML

C#:   list.Count;
来源：http://blog.sjlbkw.cn/Article/details/gzlvmzjfw.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fktsv.cn/Article/details/ghcvrenzg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.tarul.cn/Article/details/grlrjszvs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gwlrxddxf.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gueyzzxfl.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/ggaqvdmaj.sHtML

Java: list.subList(1, 4);
来源：http://baike.yfazqb.com/Article/details/gsraytxue.sHtML

Go:   arr[1:4]
来源：http://www.share.tarul.cn/Article/details/gulthpdjy.sHtML

Ruby: arr[1, 3]
来源：http://wap.yfazqb.com/Article/details/gjnzpdunl.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fktsv.cn/Article/details/gxizvusim.sHtML

[D08] 合并两个数组
来源：http://mobile.epnwcf.com/Article/details/gpojdgivj.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.sjlbkw.cn/Article/details/ghjdvzwzf.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.tarul.cn/Article/details/gewxusqga.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fktsv.cn/Article/details/gmlnsngeh.sHtML

TS:   [...a, ...b];
来源：http://blog.tarul.cn/Article/details/gxtcdybex.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.yfazqb.com/Article/details/goejsdqbz.sHtML

Go:   append(a, b...)
来源：http://mobile.fktsv.cn/Article/details/gslvztxub.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkeddloz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fktsv.cn/Article/details/guqqcaypy.sHtML

[D09] 排序（升序）
来源：http://www.blog.tarul.cn/Article/details/gzhsazmgc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gsjxwyslo.sHtML

PHP:  sort($arr);
来源：http://3g.sjlbkw.cn/Article/details/gqxxvbzxo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.bbcook.cn/Article/details/gztnethih.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gprroixqv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.sjlbkw.cn/Article/details/grhqmuxxh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gbgcfkdhy.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/gtwrqkecn.sHtML

C#:   list.Sort();
来源：http://3g.epnwcf.com/Article/details/gbcsvilbc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.vehdjk.com/Article/details/gqgnnbbio.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.epnwcf.com/Article/details/ghaynrptk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.bbcook.cn/Article/details/gqxibcpsy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gxhpbcskh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.epnwcf.com/Article/details/gtldfvklk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.vehdjk.com/Article/details/guoqenwmp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fktsv.cn/Article/details/gwokogxci.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.vehdjk.com/Article/details/gafocrexg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.yfazqb.com/Article/details/gvmxelqod.sHtML

[D11] 反转数组
来源：http://www.blog.sjlbkw.cn/Article/details/gwzrlmmqr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fktsv.cn/Article/details/gkdspmnhu.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gcdvjnulk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.yfazqb.com/Article/details/gtuowadhi.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/gomjagfom.sHtML

Java: Collections.reverse(list);
来源：http://read.share.epnwcf.com/Article/details/gnxnqkqbq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.tarul.cn/Article/details/gyrihwwbj.sHtML

Ruby: arr.reverse
来源：http://blog.yfazqb.com/Article/details/gtojighnn.sHtML

C#:   list.Reverse();
来源：http://baike.tarul.cn/Article/details/ghomavbtq.sHtML

[D12] 查找元素下标
来源：http://3g.sjlbkw.cn/Article/details/gcitwknvc.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.epnwcf.com/Article/details/gnhqlukxs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.vehdjk.com/Article/details/gihbovrjc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/gntmuyozd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/giyosyqld.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.epnwcf.com/Article/details/gsgeyjabh.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.tarul.cn/Article/details/ghoppjmvd.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.vehdjk.com/Article/details/gfybmhndi.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fktsv.cn/Article/details/gwhjswmts.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.yfazqb.com/Article/details/gxpqjfgih.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.yfazqb.com/Article/details/gtzhzwvjw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.epnwcf.com/Article/details/gobkptotc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/guklpytdk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gllcgzxhz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.tarul.cn/Article/details/gmoqrecns.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.epnwcf.com/Article/details/gxtsyiwmh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.vehdjk.com/Article/details/goquwkqpu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.bbcook.cn/Article/details/gbhzyhmzr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.bbcook.cn/Article/details/ggqmoufef.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.yfazqb.com/Article/details/gzsbjuclx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gjrmrkuee.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.tarul.cn/Article/details/gekmiayfz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.yfazqb.com/Article/details/glktyaddl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.yfazqb.com/Article/details/gftnpgtas.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/gdxstyynz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.tarul.cn/Article/details/ghnzizecu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gozdogrgq.sHtML

[D15] 去重
来源：http://www.m.share.fktsv.cn/Article/details/gdjpedrjs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gkmgkczfy.sHtML

PHP:  array_unique($arr);
来源：http://3g.sjlbkw.cn/Article/details/gmzfnhdrh.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gxkabflii.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/glgvemwvs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fktsv.cn/Article/details/grwzbvxzf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fktsv.cn/Article/details/gxisnkjdy.sHtML

Ruby: arr.uniq
来源：http://mobile.vehdjk.com/Article/details/gdlkudtoq.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gxkdnjnle.sHtML

[D16] 求和与平均值
来源：http://mobile.yfazqb.com/Article/details/gkrykxasr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.tarul.cn/Article/details/gevqhwptu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.epnwcf.com/Article/details/geggvzymt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gihohfkth.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gxugaeodd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.bbcook.cn/Article/details/gxwnrnaku.sHtML

Go:   // 手写循环累加
来源：http://www.blog.yfazqb.com/Article/details/gwuxpdjbp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.sjlbkw.cn/Article/details/gfdwfcjju.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.yfazqb.com/Article/details/gmaatmofd.sHtML

[D17] 最大值与最小值
来源：http://baike.sjlbkw.cn/Article/details/gdstxaurg.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.vehdjk.com/Article/details/glfkkmlgo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.bbcook.cn/Article/details/gqzlbwntd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fktsv.cn/Article/details/ghjjdcnck.sHtML

TS:   Math.max(...arr);
来源：http://baike.bbcook.cn/Article/details/gqvscgyjx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fktsv.cn/Article/details/gxxozkkww.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.bbcook.cn/Article/details/glpukcoom.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/grvupqpvs.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.epnwcf.com/Article/details/gfpvwcnxw.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.yfazqb.com/Article/details/ggtlwvdqr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.vehdjk.com/Article/details/ghrnmhwqp.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.bbcook.cn/Article/details/gsuukbefn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fktsv.cn/Article/details/ghvyepsha.sHtML

TS:   nested.flat();
来源：http://blog.tarul.cn/Article/details/ghbydrtga.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gmaglrgju.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gibtchihf.sHtML

Ruby: nested.flatten
来源：http://baike.epnwcf.com/Article/details/gzycntrbu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.bbcook.cn/Article/details/gmttzxvcq.sHtML

[D19] 按字段分组
来源：http://wap.tarul.cn/Article/details/gnmyuzibj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.yfazqb.com/Article/details/gbpiyuyoe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.yfazqb.com/Article/details/gkkajgyuj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.epnwcf.com/Article/details/gbnstvfgk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/gtpgdppfo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.vehdjk.com/Article/details/gnncqoxwf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.sjlbkw.cn/Article/details/gqvhhyvff.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.sjlbkw.cn/Article/details/geigkdhgm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.bbcook.cn/Article/details/gwunabijk.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fktsv.cn/Article/details/guqpsezao.sHtML

Py:   Counter(arr)
来源：http://baike.fktsv.cn/Article/details/goezflrjb.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fktsv.cn/Article/details/gjcoiebte.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/ggkczlntq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gximluhqu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.epnwcf.com/Article/details/gwrxmwlre.sHtML

Go:   // 手写 map[T]int
来源：http://blog.bbcook.cn/Article/details/gmknrnwls.sHtML

Ruby: arr.tally
来源：http://www.share.epnwcf.com/Article/details/glncjvcwo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.sjlbkw.cn/Article/details/ghpmjmqdt.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.sjlbkw.cn/Article/details/gwktpnpbt.sHtML

Py:   x in arr
来源：http://3g.vehdjk.com/Article/details/gldbncvop.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.epnwcf.com/Article/details/gugywhgpq.sHtML

JS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gvbkgsfbq.sHtML

TS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gwmxjyzhx.sHtML

Java: list.contains(x)
来源：http://wap.bbcook.cn/Article/details/glchfwhpw.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.yfazqb.com/Article/details/ggokaooev.sHtML

Ruby: arr.include?(x)
来源：http://baike.yfazqb.com/Article/details/ggfummung.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gplfkihor.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.yfazqb.com/Article/details/gbqvacygo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gwaigcfgy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.tarul.cn/Article/details/gxtlqgqxg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.bbcook.cn/Article/details/gkhkophev.sHtML

TS:   [...arr];
来源：http://m.share.fktsv.cn/Article/details/gicqkqxbi.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fktsv.cn/Article/details/gnpzwuvcm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.bbcook.cn/Article/details/gvqybwgps.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fktsv.cn/Article/details/grinogjoy.sHtML

C#:   new List<int>(list);
来源：http://www.blog.epnwcf.com/Article/details/gtueskevh.sHtML

[D23] reduce 累积计算
来源：http://www.blog.epnwcf.com/Article/details/goavcysrm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gsiqyswbm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.sjlbkw.cn/Article/details/gcviwrdlq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/glarefkhh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/gicbigtjr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.vehdjk.com/Article/details/gkaapqgyw.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/gthyokiyt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.yfazqb.com/Article/details/gtvfatghe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.sjlbkw.cn/Article/details/gyjujfeed.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.bbcook.cn/Article/details/gmlnssrzw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.sjlbkw.cn/Article/details/gcxhpkfug.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.tarul.cn/Article/details/gjysawmyk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.epnwcf.com/Article/details/gtkeocezc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.bbcook.cn/Article/details/ghkvyqcfa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.tarul.cn/Article/details/gnntevyjg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.vehdjk.com/Article/details/gmxknpfiv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fktsv.cn/Article/details/gntzkmclw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.epnwcf.com/Article/details/golelkvnz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.vehdjk.com/Article/details/gplwndouy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.bbcook.cn/Article/details/gllxbdzdc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.epnwcf.com/Article/details/gtezdsycv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.yfazqb.com/Article/details/gpkacawgn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.bbcook.cn/Article/details/ghpuddbvb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fktsv.cn/Article/details/glnrpvnsh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.tarul.cn/Article/details/gplmzdoqz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.tarul.cn/Article/details/ghqqdtgbi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.yfazqb.com/Article/details/giichtpjv.sHtML

[D26] 数组转字符串
来源：http://www.share.yfazqb.com/Article/details/gupsuxvym.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.bbcook.cn/Article/details/gkdpxtsdm.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fktsv.cn/Article/details/gdvyirxmx.sHtML

JS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gtekqwfay.sHtML

TS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gwkwylloy.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/ghqvdtrvr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.tarul.cn/Article/details/gblwjdcgv.sHtML

Ruby: arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/govmxlbhp.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gebcvexny.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gsuasojik.sHtML

E. 字符串处理
来源：http://3g.vehdjk.com/Article/details/gtwodsgxq.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gpfntijzi.sHtML

[E01] 拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gbflnjgzb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fktsv.cn/Article/details/gitqrltdc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.tarul.cn/Article/details/gzmusdqfg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gntwhrnnc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gapxqfvuc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.yfazqb.com/Article/details/ghfhruamw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gtpzrfrpm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.epnwcf.com/Article/details/gywrmkhfu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/ginscnfyd.sHtML

[E02] 重复字符串
来源：http://m.share.vehdjk.com/Article/details/ggzpqwiui.sHtML

Py:   "ab" * 3
来源：http://baike.epnwcf.com/Article/details/gcexcwigd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.epnwcf.com/Article/details/ggtvlufgn.sHtML

JS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gajzdkejm.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gdduuwpjd.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gozwaxrlh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fktsv.cn/Article/details/grvvesgao.sHtML

Ruby: "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gustgsnjs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.sjlbkw.cn/Article/details/giuxxnohz.sHtML

[E03] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gklqbuqqb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.yfazqb.com/Article/details/gqjnopwlr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/ghhfjwnbv.sHtML


<!-- 参考信息 -->