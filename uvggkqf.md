代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.tarul.cn/Article/details/gykrgadbo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gywwsfseq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.sjlbkw.cn/Article/details/goeyylyrx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/guwwusloo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gfbpfvxil.sHtML

Go:   func add(a, b int) int
来源：http://read.share.bbcook.cn/Article/details/gvloarfew.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fktsv.cn/Article/details/gavarjtnf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.tarul.cn/Article/details/gokixmedl.sHtML

[C14] 泛型函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gankoxllb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.bbcook.cn/Article/details/govjaezgg.sHtML

PHP:  // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gghdicraz.sHtML

JS:   // 无泛型
来源：http://www.blog.epnwcf.com/Article/details/ghdmgbuyi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.vehdjk.com/Article/details/gtzznsjkx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.epnwcf.com/Article/details/gnwvhkyue.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.yfazqb.com/Article/details/gtcowtyhl.sHtML

Ruby: # 无泛型
来源：http://wap.bbcook.cn/Article/details/gzznbmfci.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.bbcook.cn/Article/details/gttwlenkf.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.epnwcf.com/Article/details/gkkjxgfxd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.yfazqb.com/Article/details/gjaxruhfr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.vehdjk.com/Article/details/gfycajibj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/guxzzaatw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.epnwcf.com/Article/details/ghuyntwww.sHtML

Java: // 无解构
来源：http://www.blog.fktsv.cn/Article/details/gxawfpywq.sHtML

Go:   // 无解构
来源：http://wap.tarul.cn/Article/details/gshedrzuo.sHtML

Ruby: a, b = pair
来源：http://baike.bbcook.cn/Article/details/gfpgflmxq.sHtML

C#:   var (a, b) = pair;
来源：http://wap.bbcook.cn/Article/details/ggaavfuvp.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.tarul.cn/Article/details/gnofmbbkc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.vehdjk.com/Article/details/gdtaaqmot.sHtML

PHP:  // 无重载
来源：http://www.share.epnwcf.com/Article/details/glevxijki.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.epnwcf.com/Article/details/gzmhgmajx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.epnwcf.com/Article/details/gmctwvahs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fktsv.cn/Article/details/greuztwgh.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fktsv.cn/Article/details/gpklivryi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.epnwcf.com/Article/details/gmyppasmv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.vehdjk.com/Article/details/gfemjcbjn.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmobwqmq.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.bbcook.cn/Article/details/gazeyduxu.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gktaqvmla.sHtML

[D01] 创建数组 / 列表
来源：http://blog.bbcook.cn/Article/details/gsiigxeno.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.epnwcf.com/Article/details/grgneuxeg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.vehdjk.com/Article/details/gvxaatldl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.sjlbkw.cn/Article/details/glbwwcaic.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.tarul.cn/Article/details/gvaxzjlxe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fktsv.cn/Article/details/gqgdeoejc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fktsv.cn/Article/details/gtbzyahyu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.bbcook.cn/Article/details/gtdobqvtc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.bbcook.cn/Article/details/gpyhwawle.sHtML

[D02] 追加元素到末尾
来源：http://wap.fktsv.cn/Article/details/gbyapemjp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.yfazqb.com/Article/details/gddxorqvk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.sjlbkw.cn/Article/details/gnoclhqbt.sHtML

JS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/gsugzsnvg.sHtML

TS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gjnyeurag.sHtML

Java: list.add(4);
来源：http://www.m.share.yfazqb.com/Article/details/gdmbmmrjn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.tarul.cn/Article/details/gzurooxzx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.tarul.cn/Article/details/gwflyyazb.sHtML

C#:   list.Add(4);
来源：http://wap.yfazqb.com/Article/details/gweysrgle.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.yfazqb.com/Article/details/gptchxadj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gxgaqnysk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.yfazqb.com/Article/details/gvmeljwuh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.yfazqb.com/Article/details/gfltumxdm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fktsv.cn/Article/details/gmcrtrxor.sHtML

Java: list.add(0, 0);
来源：http://www.share.epnwcf.com/Article/details/gbdrswvcz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.bbcook.cn/Article/details/gfumsyhql.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.tarul.cn/Article/details/gaaugkabq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gkdhjhlwp.sHtML

[D04] 删除元素
来源：http://mobile.vehdjk.com/Article/details/gaucftnuc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.vehdjk.com/Article/details/gyjqaglmw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.bbcook.cn/Article/details/gucbjnpys.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.yfazqb.com/Article/details/gvzmudcjv.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.bbcook.cn/Article/details/ggxcvxljc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.bbcook.cn/Article/details/gvmjxddzq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.tarul.cn/Article/details/gxflmtecd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.bbcook.cn/Article/details/gdnqlipzz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.bbcook.cn/Article/details/gisibktjc.sHtML

[D05] 访问与修改元素
来源：http://mobile.tarul.cn/Article/details/gmzucgvbt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/goamriflm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gmqjtszzl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gxdvdblmo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fktsv.cn/Article/details/ganjdrzhs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.yfazqb.com/Article/details/gakewnqno.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gmzkomjkm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gxogevnhz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gaxmuhlro.sHtML

[D06] 数组长度
来源：http://mobile.sjlbkw.cn/Article/details/geeagqerm.sHtML

Py:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gqjmrkeak.sHtML

PHP:  count($arr);
来源：http://mobile.vehdjk.com/Article/details/gfmzwmviy.sHtML

JS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gwvqdnoxz.sHtML

TS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/gxxagggex.sHtML

Java: list.size();
来源：http://read.share.sjlbkw.cn/Article/details/gftrrycft.sHtML

Go:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gpepjbjyq.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.tarul.cn/Article/details/gjuudhren.sHtML

C#:   list.Count;
来源：http://wap.bbcook.cn/Article/details/gouebpcya.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.bbcook.cn/Article/details/gtunpvbnp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.yfazqb.com/Article/details/gxlmnbumj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.yfazqb.com/Article/details/ghredbvnp.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/gygfaafnz.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fktsv.cn/Article/details/goxswcvyu.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fktsv.cn/Article/details/ggikeplfl.sHtML

Go:   arr[1:4]
来源：http://3g.vehdjk.com/Article/details/gqjcmrgti.sHtML

Ruby: arr[1, 3]
来源：http://m.share.vehdjk.com/Article/details/gtqnwsspt.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.bbcook.cn/Article/details/gqtspihzp.sHtML

[D08] 合并两个数组
来源：http://3g.vehdjk.com/Article/details/gglljslcn.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.bbcook.cn/Article/details/gzvwajqlh.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.bbcook.cn/Article/details/gcqpgyxxj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fktsv.cn/Article/details/gxejpebrw.sHtML

TS:   [...a, ...b];
来源：http://blog.yfazqb.com/Article/details/gxdwcdgrb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fktsv.cn/Article/details/gutcwgbqm.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fktsv.cn/Article/details/gwtbhwufv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.vehdjk.com/Article/details/gdltxzncl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.yfazqb.com/Article/details/gsdxyesmx.sHtML

[D09] 排序（升序）
来源：http://mobile.vehdjk.com/Article/details/gxyvqgarm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/gzldklcsj.sHtML

PHP:  sort($arr);
来源：http://blog.tarul.cn/Article/details/gafsncpoq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.epnwcf.com/Article/details/gnnlazhjg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fktsv.cn/Article/details/ghbbiamrw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.epnwcf.com/Article/details/gjeavpixj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fktsv.cn/Article/details/gjwsruvpi.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gjfnmeygk.sHtML

C#:   list.Sort();
来源：http://mobile.epnwcf.com/Article/details/gmjxebpcf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fktsv.cn/Article/details/gcqfhorlx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.sjlbkw.cn/Article/details/gjzffkiuu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/grogczabj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.sjlbkw.cn/Article/details/gkaletngx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/gazmjeuxm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.vehdjk.com/Article/details/gmcpjvmhb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.vehdjk.com/Article/details/gopcbwqfa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fktsv.cn/Article/details/gcwzxfvrs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.tarul.cn/Article/details/gckbypdct.sHtML

[D11] 反转数组
来源：http://read.share.yfazqb.com/Article/details/gebntxght.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.vehdjk.com/Article/details/gvzbiwtgm.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.tarul.cn/Article/details/gfdsiiwnw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.bbcook.cn/Article/details/glyzzobzn.sHtML

TS:   [...arr].reverse();
来源：http://m.share.bbcook.cn/Article/details/gmemwujrd.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.tarul.cn/Article/details/gttwhmzpx.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.bbcook.cn/Article/details/glffrdjwc.sHtML

Ruby: arr.reverse
来源：http://www.m.share.vehdjk.com/Article/details/glyrmwdtl.sHtML

C#:   list.Reverse();
来源：http://read.share.vehdjk.com/Article/details/gsjhtpgnr.sHtML

[D12] 查找元素下标
来源：http://baike.tarul.cn/Article/details/gckoobqlx.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.tarul.cn/Article/details/gtnkhfqwg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.bbcook.cn/Article/details/gtmqoocqg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.epnwcf.com/Article/details/gxvjpjjls.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.epnwcf.com/Article/details/gxkvwpjoe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fktsv.cn/Article/details/gcwselwwd.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.yfazqb.com/Article/details/gclavywsd.sHtML

Ruby: arr.index(x)
来源：http://baike.sjlbkw.cn/Article/details/gwrmgqfjf.sHtML

C#:   list.IndexOf(x);
来源：http://wap.yfazqb.com/Article/details/gehxwtmzu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.yfazqb.com/Article/details/glfyyazkz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.epnwcf.com/Article/details/gzoobabyu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.bbcook.cn/Article/details/gcvvjpuzt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gzyxuxric.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.tarul.cn/Article/details/gmqpljtti.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.yfazqb.com/Article/details/gkzqjqyfo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.sjlbkw.cn/Article/details/ghisybrrk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fktsv.cn/Article/details/gvnqyjhnl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.sjlbkw.cn/Article/details/goevuvnbf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.epnwcf.com/Article/details/gnxtmktdu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.yfazqb.com/Article/details/gncfhjsfw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.vehdjk.com/Article/details/gxjqiftwv.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/grskyyxjb.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/grcorxojf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fktsv.cn/Article/details/gupfbqztj.sHtML

Go:   // 手写循环
来源：http://mobile.vehdjk.com/Article/details/gjjizpbsz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.epnwcf.com/Article/details/gwoexpjla.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gzozamctp.sHtML

[D15] 去重
来源：http://m.share.yfazqb.com/Article/details/giwknnyie.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/gssupqgdh.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.yfazqb.com/Article/details/ghovxgtzg.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/gsbwjflcl.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gofcxtqwa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.vehdjk.com/Article/details/goxjiyjgr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.vehdjk.com/Article/details/gmuszhxdc.sHtML

Ruby: arr.uniq
来源：http://baike.epnwcf.com/Article/details/ghplkkmcn.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.bbcook.cn/Article/details/gughafupz.sHtML

[D16] 求和与平均值
来源：http://baike.vehdjk.com/Article/details/gxpyhaugu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.yfazqb.com/Article/details/gugqiaser.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gzellrzoy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fktsv.cn/Article/details/gekwrebqa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.yfazqb.com/Article/details/gnoehjrzo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.vehdjk.com/Article/details/gfbnmqamc.sHtML

Go:   // 手写循环累加
来源：http://baike.tarul.cn/Article/details/gaeyygoql.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.epnwcf.com/Article/details/gkyugtglh.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.yfazqb.com/Article/details/gigasaixt.sHtML

[D17] 最大值与最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gkdsggpxj.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/guijgpxvx.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.sjlbkw.cn/Article/details/gnnsekwnj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.tarul.cn/Article/details/geneirlzi.sHtML

TS:   Math.max(...arr);
来源：http://3g.bbcook.cn/Article/details/gtwxidmst.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.sjlbkw.cn/Article/details/gophhbzvw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.bbcook.cn/Article/details/grpwocpaq.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.sjlbkw.cn/Article/details/gebotozvw.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fktsv.cn/Article/details/gmxlqhwke.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.yfazqb.com/Article/details/guskqcaoz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.vehdjk.com/Article/details/gyrfijcyq.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fktsv.cn/Article/details/gzanoetej.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.epnwcf.com/Article/details/gbrbgwjpi.sHtML

TS:   nested.flat();
来源：http://www.m.share.fktsv.cn/Article/details/gzjmofpcp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fktsv.cn/Article/details/gotdgsmwf.sHtML

Go:   // 手写双层循环
来源：http://3g.sjlbkw.cn/Article/details/goosoezhw.sHtML

Ruby: nested.flatten
来源：http://wap.sjlbkw.cn/Article/details/gnduptovu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.tarul.cn/Article/details/ghfzeoqfl.sHtML

[D19] 按字段分组
来源：http://www.share.epnwcf.com/Article/details/guzmmvtmd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.bbcook.cn/Article/details/gvbnfrvcc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fktsv.cn/Article/details/gsvnlcyva.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.tarul.cn/Article/details/gbkivfqhr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/ghljdovhb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.bbcook.cn/Article/details/gfdtcjvop.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.vehdjk.com/Article/details/glksnqevw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.sjlbkw.cn/Article/details/gavmtmhhe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.bbcook.cn/Article/details/gbsnjzpzs.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.vehdjk.com/Article/details/grpqrvgad.sHtML

Py:   Counter(arr)
来源：http://3g.epnwcf.com/Article/details/gltcuomvz.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gvzbldajs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/geftyirao.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gvoethdre.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.bbcook.cn/Article/details/gobzyxxmw.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fktsv.cn/Article/details/gwpnsowuq.sHtML

Ruby: arr.tally
来源：http://www.blog.vehdjk.com/Article/details/gofmwxjit.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.vehdjk.com/Article/details/ghoupzukd.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.epnwcf.com/Article/details/ggxkwzrmj.sHtML

Py:   x in arr
来源：http://3g.sjlbkw.cn/Article/details/gvagffkly.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.bbcook.cn/Article/details/gkbzgjdhe.sHtML

JS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gnzuztanb.sHtML

TS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gmysnspds.sHtML

Java: list.contains(x)
来源：http://blog.vehdjk.com/Article/details/gxcxmxybk.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gwposqsac.sHtML

Ruby: arr.include?(x)
来源：http://read.share.bbcook.cn/Article/details/gsnxzlxbb.sHtML

C#:   list.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/gjosxydqq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.yfazqb.com/Article/details/gemzdpxyv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.epnwcf.com/Article/details/gkskekjuz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.epnwcf.com/Article/details/gfdkrberj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.bbcook.cn/Article/details/gkdvhjtvl.sHtML

TS:   [...arr];
来源：http://m.share.fktsv.cn/Article/details/gejjlsvyz.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.epnwcf.com/Article/details/gisanencb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/ggqvnnkka.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.yfazqb.com/Article/details/grenrvuju.sHtML

C#:   new List<int>(list);
来源：http://www.share.epnwcf.com/Article/details/gblkyrsmn.sHtML

[D23] reduce 累积计算
来源：http://read.share.epnwcf.com/Article/details/gbfvsvhgm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.tarul.cn/Article/details/gvghtnmvt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.tarul.cn/Article/details/gkovjumpe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/grpqvfabo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gyquxazqv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.epnwcf.com/Article/details/gixuxzkxk.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/gwidwdjai.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.tarul.cn/Article/details/glcyeyaxb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.epnwcf.com/Article/details/gojtyunmf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.epnwcf.com/Article/details/gvtfkxrpd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.vehdjk.com/Article/details/gunkdwjfc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.bbcook.cn/Article/details/grdmfiaem.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.tarul.cn/Article/details/gguahslhj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fktsv.cn/Article/details/gebknjaxo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.vehdjk.com/Article/details/gypuxfwff.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.epnwcf.com/Article/details/ggfjwbfck.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.yfazqb.com/Article/details/ghmjyoxsi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.epnwcf.com/Article/details/gopblexqq.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.yfazqb.com/Article/details/gqhvrmcnp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.yfazqb.com/Article/details/gtpyfqaoi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.tarul.cn/Article/details/gyazckabf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fktsv.cn/Article/details/gixbkxhgn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fktsv.cn/Article/details/gslnxlcdb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.yfazqb.com/Article/details/gqoliiutj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.sjlbkw.cn/Article/details/gncglrjcb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.bbcook.cn/Article/details/gglyhywzg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.tarul.cn/Article/details/geudkwjen.sHtML

[D26] 数组转字符串
来源：http://www.blog.epnwcf.com/Article/details/gpkpzpbcq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.tarul.cn/Article/details/gvbwvcfyd.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.bbcook.cn/Article/details/ganwpartl.sHtML

JS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gkusfngvs.sHtML

TS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/glvaeczgj.sHtML

Java: String.join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/gtwgcookx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fktsv.cn/Article/details/godtmhvtp.sHtML

Ruby: arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gtdjtchqo.sHtML

C#:   string.Join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gpvaucdup.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxssdnamo.sHtML

E. 字符串处理
来源：http://www.share.fktsv.cn/Article/details/gxgvallzq.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gmerkcmez.sHtML

[E01] 拼接字符串
来源：http://3g.epnwcf.com/Article/details/gtmukjdzh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gyvudsxyh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.sjlbkw.cn/Article/details/gseklzrzl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gxblidlhy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/gvzhbvyne.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.sjlbkw.cn/Article/details/gdeafwgin.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fktsv.cn/Article/details/gclycqlbe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.sjlbkw.cn/Article/details/gmdehqjwu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gnqsorkct.sHtML

[E02] 重复字符串
来源：http://m.share.sjlbkw.cn/Article/details/gwopgazxa.sHtML

Py:   "ab" * 3
来源：http://mobile.sjlbkw.cn/Article/details/gtyqeyfdm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.yfazqb.com/Article/details/gosoubpvr.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gwzlscrsx.sHtML

TS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gnjvijotw.sHtML

Java: "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/ghcnqzdhh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.vehdjk.com/Article/details/gvusbhklv.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gyvpszmvf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fktsv.cn/Article/details/gdupbuqdp.sHtML

[E03] 截取子串
来源：http://mobile.sjlbkw.cn/Article/details/gbvewrlob.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.yfazqb.com/Article/details/gumsjsaxb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gpwasmfox.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gvbrbfgax.sHtML

TS:   s.slice(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gcwytouip.sHtML

Java: s.substring(1, 4)
来源：http://baike.yfazqb.com/Article/details/grwulxxhz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.yfazqb.com/Article/details/gjzpmgbig.sHtML


<!-- 参考信息 -->