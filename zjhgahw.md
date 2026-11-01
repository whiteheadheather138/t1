代发 wailian999

[C14] 泛型函数
来源：http://www.blog.fktsv.cn/Article/details/guiaiiydn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.tarul.cn/Article/details/gtqgwpkxx.sHtML

PHP:  // 无泛型
来源：http://mobile.epnwcf.com/Article/details/ghqrazuey.sHtML

JS:   // 无泛型
来源：http://mobile.vehdjk.com/Article/details/gowyttxxh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.epnwcf.com/Article/details/gcxvvjxub.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fktsv.cn/Article/details/gpqpklqex.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.sjlbkw.cn/Article/details/gbazfqgyu.sHtML

Ruby: # 无泛型
来源：http://m.share.bbcook.cn/Article/details/gmiuvbehv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.vehdjk.com/Article/details/ghiyhiptu.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.yfazqb.com/Article/details/gvgtdorgj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.yfazqb.com/Article/details/gdnwpvrcg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.epnwcf.com/Article/details/gcybaqoqz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.vehdjk.com/Article/details/gjamnlnpz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.bbcook.cn/Article/details/gzegpxncf.sHtML

Java: // 无解构
来源：http://3g.epnwcf.com/Article/details/gazljeneq.sHtML

Go:   // 无解构
来源：http://www.blog.tarul.cn/Article/details/gdhmuweei.sHtML

Ruby: a, b = pair
来源：http://www.m.share.epnwcf.com/Article/details/gmadurwap.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fktsv.cn/Article/details/gnwyfvzxu.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fktsv.cn/Article/details/gotwuinsx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.vehdjk.com/Article/details/goutnjejp.sHtML

PHP:  // 无重载
来源：http://read.share.tarul.cn/Article/details/goxgofccv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.tarul.cn/Article/details/gjkzopiqi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.epnwcf.com/Article/details/gdlgwwndi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.bbcook.cn/Article/details/gjxdnlaja.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.epnwcf.com/Article/details/gojgttwwl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.yfazqb.com/Article/details/gdippeerd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.sjlbkw.cn/Article/details/gdqeksjdd.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glghnegah.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.sjlbkw.cn/Article/details/gibszfebm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gyfgsypjh.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gqgxfvfkc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.bbcook.cn/Article/details/gnfcyglig.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/gqophunoo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.epnwcf.com/Article/details/gkexgrexo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.tarul.cn/Article/details/gbgrahkfo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.epnwcf.com/Article/details/gdpnduygs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fktsv.cn/Article/details/gjwulgxil.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.yfazqb.com/Article/details/giwpshsws.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.epnwcf.com/Article/details/gdcyibmja.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.sjlbkw.cn/Article/details/gtlmiykae.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.tarul.cn/Article/details/ghhzypacf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.sjlbkw.cn/Article/details/guoogszeh.sHtML

JS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gobwinzhn.sHtML

TS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/gijwaiolb.sHtML

Java: list.add(4);
来源：http://read.share.vehdjk.com/Article/details/gcmyetrka.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.tarul.cn/Article/details/gptvtidqm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fktsv.cn/Article/details/gxcfuelkg.sHtML

C#:   list.Add(4);
来源：http://www.blog.epnwcf.com/Article/details/gbczikurw.sHtML

[D03] 在指定位置插入元素
来源：http://baike.bbcook.cn/Article/details/grrpthecr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.yfazqb.com/Article/details/gtgpgpfwb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fktsv.cn/Article/details/gjkskjfot.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.bbcook.cn/Article/details/gwgbowrqh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.bbcook.cn/Article/details/gsihdlacx.sHtML

Java: list.add(0, 0);
来源：http://wap.tarul.cn/Article/details/glcdyusrl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.vehdjk.com/Article/details/gkqxfmvul.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.epnwcf.com/Article/details/gkucjygjv.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.bbcook.cn/Article/details/ghhpaemeq.sHtML

[D04] 删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gvijviiug.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.vehdjk.com/Article/details/gpurgxpbb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fktsv.cn/Article/details/gzmlykdnt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fktsv.cn/Article/details/ghyxxsguo.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.sjlbkw.cn/Article/details/gtcmuywvv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.vehdjk.com/Article/details/gasrwfric.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.epnwcf.com/Article/details/gubnmdtvx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.sjlbkw.cn/Article/details/gzraxnpjh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.bbcook.cn/Article/details/gvepjggws.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.yfazqb.com/Article/details/gdtihzghc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gjmunmxxd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/ghjbskazt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gjfcyboez.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fktsv.cn/Article/details/ggxzrfepk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.yfazqb.com/Article/details/gmwgdwhqz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gtsxxuycs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gedtfvjwr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gspvaqxyp.sHtML

[D06] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gtfgfxsrw.sHtML

Py:   len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gmnsptgpn.sHtML

PHP:  count($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrwsikbq.sHtML

JS:   arr.length
来源：http://3g.vehdjk.com/Article/details/grbklsqda.sHtML

TS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/gfvqshkzp.sHtML

Java: list.size();
来源：http://www.m.share.vehdjk.com/Article/details/glhjhloid.sHtML

Go:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/grusfdmbw.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.epnwcf.com/Article/details/gjatemsnn.sHtML

C#:   list.Count;
来源：http://mobile.tarul.cn/Article/details/gebltunbu.sHtML

[D07] 切片 / 取子数组
来源：http://3g.epnwcf.com/Article/details/gzzuunilm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.sjlbkw.cn/Article/details/ghczwtyfp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.bbcook.cn/Article/details/gpsrwyddj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gfuwfrxyq.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fktsv.cn/Article/details/gqcdficzq.sHtML

Java: list.subList(1, 4);
来源：http://blog.fktsv.cn/Article/details/gxcfergkx.sHtML

Go:   arr[1:4]
来源：http://blog.fktsv.cn/Article/details/gspwnlqww.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.vehdjk.com/Article/details/gaqdrahco.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.yfazqb.com/Article/details/gcsmivtxm.sHtML

[D08] 合并两个数组
来源：http://m.share.bbcook.cn/Article/details/gvveiymzg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.vehdjk.com/Article/details/gpaavadcd.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.bbcook.cn/Article/details/gxkwgxxhl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.bbcook.cn/Article/details/glxwocbno.sHtML

TS:   [...a, ...b];
来源：http://blog.yfazqb.com/Article/details/glgkmglva.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fktsv.cn/Article/details/ggmqzueiz.sHtML

Go:   append(a, b...)
来源：http://baike.yfazqb.com/Article/details/gufmpjpgr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.tarul.cn/Article/details/gwirhtxiw.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.epnwcf.com/Article/details/gicnxolep.sHtML

[D09] 排序（升序）
来源：http://blog.yfazqb.com/Article/details/gaklubnnl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gamkvgujk.sHtML

PHP:  sort($arr);
来源：http://www.share.fktsv.cn/Article/details/gzgipgopn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.bbcook.cn/Article/details/gbgthgdoz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.epnwcf.com/Article/details/gniiijzzt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.vehdjk.com/Article/details/gagfficmd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gewdcnyya.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/gssmzxoxc.sHtML

C#:   list.Sort();
来源：http://read.share.fktsv.cn/Article/details/gqaqjabul.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.sjlbkw.cn/Article/details/gzssbakpq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.epnwcf.com/Article/details/guhbfwjqg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.vehdjk.com/Article/details/gbqoitdwj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fktsv.cn/Article/details/gqjlfrgsi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/grunqghvx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.epnwcf.com/Article/details/gcapuaggh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.yfazqb.com/Article/details/gmxxdnfqj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.bbcook.cn/Article/details/gcvaatpbs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fktsv.cn/Article/details/gcydhzfvg.sHtML

[D11] 反转数组
来源：http://blog.vehdjk.com/Article/details/gltbzmnho.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.yfazqb.com/Article/details/gqkzjytsh.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gvbmsfnfh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fktsv.cn/Article/details/gypektbrc.sHtML

TS:   [...arr].reverse();
来源：http://blog.fktsv.cn/Article/details/ghoziwemv.sHtML

Java: Collections.reverse(list);
来源：http://wap.bbcook.cn/Article/details/gttfxgwwg.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.vehdjk.com/Article/details/gveupqqvl.sHtML

Ruby: arr.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gzezjvhso.sHtML

C#:   list.Reverse();
来源：http://3g.bbcook.cn/Article/details/gccuziqbq.sHtML

[D12] 查找元素下标
来源：http://baike.epnwcf.com/Article/details/ginoxknwb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.tarul.cn/Article/details/gzmlyklfz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fktsv.cn/Article/details/gaewiejpf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gnokvwftz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.tarul.cn/Article/details/gngrtgljv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.epnwcf.com/Article/details/gagosjqap.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gqhsxirkj.sHtML

Ruby: arr.index(x)
来源：http://blog.bbcook.cn/Article/details/gcmrewfvx.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.vehdjk.com/Article/details/gysurtuay.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.vehdjk.com/Article/details/gejcdwomr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.yfazqb.com/Article/details/gieqynhxq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fktsv.cn/Article/details/glhzwgsza.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/garlkjecm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.tarul.cn/Article/details/glwsdcutv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.vehdjk.com/Article/details/gqzszexak.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.sjlbkw.cn/Article/details/gkcmmlxiq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fktsv.cn/Article/details/ggynzmfua.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.vehdjk.com/Article/details/gwjkzozhj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.vehdjk.com/Article/details/gprrryqdz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.bbcook.cn/Article/details/gqkislzov.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.vehdjk.com/Article/details/gywmzuwip.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gmojxoqep.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/grjqtarwn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.vehdjk.com/Article/details/gjgffdmhy.sHtML

Go:   // 手写循环
来源：http://wap.epnwcf.com/Article/details/gnvzfhfkx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.epnwcf.com/Article/details/gjimulxpc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fktsv.cn/Article/details/gfsspcmoj.sHtML

[D15] 去重
来源：http://baike.fktsv.cn/Article/details/glwhehhnw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/gmrljslbz.sHtML

PHP:  array_unique($arr);
来源：http://wap.tarul.cn/Article/details/gwcutafpv.sHtML

JS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gojcagced.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/gfipffvyy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.bbcook.cn/Article/details/gokahbdaw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.vehdjk.com/Article/details/gxhodrxqv.sHtML

Ruby: arr.uniq
来源：http://www.m.share.epnwcf.com/Article/details/gqwobcick.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.vehdjk.com/Article/details/ghysepdma.sHtML

[D16] 求和与平均值
来源：http://read.share.bbcook.cn/Article/details/ganwxezox.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fktsv.cn/Article/details/ggwmkgqrt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.vehdjk.com/Article/details/gnpqunodi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.vehdjk.com/Article/details/ghdxjhjpk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.yfazqb.com/Article/details/grrcqetnf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.sjlbkw.cn/Article/details/gdpiomliw.sHtML

Go:   // 手写循环累加
来源：http://blog.yfazqb.com/Article/details/gwylzilnw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.tarul.cn/Article/details/ghtorityv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.tarul.cn/Article/details/grzawjxtm.sHtML

[D17] 最大值与最小值
来源：http://www.share.fktsv.cn/Article/details/gxqwascge.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.vehdjk.com/Article/details/gicpgidos.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.bbcook.cn/Article/details/gpoidokta.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.bbcook.cn/Article/details/gmfosvmvi.sHtML

TS:   Math.max(...arr);
来源：http://read.share.tarul.cn/Article/details/gyobxnbrb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.epnwcf.com/Article/details/gxkovyiqe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fktsv.cn/Article/details/gmyjnwavc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.bbcook.cn/Article/details/gdttoegnz.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.tarul.cn/Article/details/guqqvplxg.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.tarul.cn/Article/details/gnvbzbecg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.yfazqb.com/Article/details/gtyvvcpcf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fktsv.cn/Article/details/ggkxwbbhr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.epnwcf.com/Article/details/gduygezfj.sHtML

TS:   nested.flat();
来源：http://blog.sjlbkw.cn/Article/details/gwrrjwhis.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.epnwcf.com/Article/details/gkkvggegu.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.epnwcf.com/Article/details/gufrnflpa.sHtML

Ruby: nested.flatten
来源：http://blog.bbcook.cn/Article/details/gpcgqxbvk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.epnwcf.com/Article/details/gqudtdtvr.sHtML

[D19] 按字段分组
来源：http://www.m.share.yfazqb.com/Article/details/ggxhewdrv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.vehdjk.com/Article/details/gmzhmzetf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fktsv.cn/Article/details/grdqxapjk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fktsv.cn/Article/details/gwpblsnve.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/ghsnziiiq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.yfazqb.com/Article/details/giroqlgol.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.vehdjk.com/Article/details/grlbjezvd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.bbcook.cn/Article/details/gtljzflmg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.epnwcf.com/Article/details/gjllamtxr.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fktsv.cn/Article/details/gycbwwzwz.sHtML

Py:   Counter(arr)
来源：http://baike.epnwcf.com/Article/details/gyqmoepgo.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fktsv.cn/Article/details/gowjexfdd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fktsv.cn/Article/details/grrmxmfxi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gdiwlcgml.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.bbcook.cn/Article/details/gjxnjizov.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.vehdjk.com/Article/details/geahrhxin.sHtML

Ruby: arr.tally
来源：http://3g.sjlbkw.cn/Article/details/gwnarrmwk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.yfazqb.com/Article/details/gglynbrhd.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.yfazqb.com/Article/details/gejoaenkf.sHtML

Py:   x in arr
来源：http://3g.epnwcf.com/Article/details/gojsmrlmd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.epnwcf.com/Article/details/gdmvweaja.sHtML

JS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gpcjttmrc.sHtML

TS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/gbirbojog.sHtML

Java: list.contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/ggvghdebg.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fktsv.cn/Article/details/ghxzxgzxg.sHtML

Ruby: arr.include?(x)
来源：http://mobile.vehdjk.com/Article/details/gopazyyxo.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/grvwinitd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.epnwcf.com/Article/details/gsggkvkhg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.tarul.cn/Article/details/gjseifmim.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.vehdjk.com/Article/details/glyjzflgi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gouwkkyoh.sHtML

TS:   [...arr];
来源：http://mobile.sjlbkw.cn/Article/details/grsitwjfq.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.sjlbkw.cn/Article/details/gcsqghfmd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/geqjlqlxz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fktsv.cn/Article/details/gpgphdxnc.sHtML

C#:   new List<int>(list);
来源：http://www.share.fktsv.cn/Article/details/gtgrxiswy.sHtML

[D23] reduce 累积计算
来源：http://www.share.epnwcf.com/Article/details/gfhukjqar.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gsxqlrqab.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gqjyaokxt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/gvjjbzbut.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.tarul.cn/Article/details/gysbfrmlq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.yfazqb.com/Article/details/gkiwvihkm.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gbdwaqkyx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.sjlbkw.cn/Article/details/gpabogmfl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.tarul.cn/Article/details/gckclizht.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.yfazqb.com/Article/details/ggtearpbc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fktsv.cn/Article/details/ghacikahd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.tarul.cn/Article/details/gewwhyeop.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.vehdjk.com/Article/details/gnppdnkhv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gmkwlyaqc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.epnwcf.com/Article/details/gfvsjbvlj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.bbcook.cn/Article/details/gflulwcze.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.yfazqb.com/Article/details/gkxudrdgd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fktsv.cn/Article/details/gwgyjweqe.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.vehdjk.com/Article/details/gxyvixoml.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.epnwcf.com/Article/details/gjkotises.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.yfazqb.com/Article/details/gavfubkxk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.tarul.cn/Article/details/glneindox.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.tarul.cn/Article/details/gmaploidc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gwaaylipd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.yfazqb.com/Article/details/gblxkrohv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.yfazqb.com/Article/details/gsahxonis.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.yfazqb.com/Article/details/gwyyrqhlk.sHtML

[D26] 数组转字符串
来源：http://www.blog.tarul.cn/Article/details/gxgfdhfzy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.tarul.cn/Article/details/gjvwzrmbz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.vehdjk.com/Article/details/gogsyjaer.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gcnbaiwtw.sHtML

TS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/ggbaqjkot.sHtML

Java: String.join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gxnrsogpb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.bbcook.cn/Article/details/gompcmxfi.sHtML

Ruby: arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gqlscbgqi.sHtML

C#:   string.Join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gdwuufkon.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmrbjuobg.sHtML

E. 字符串处理
来源：http://www.m.share.epnwcf.com/Article/details/gkladfrep.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzlfqrdxj.sHtML

[E01] 拼接字符串
来源：http://m.share.epnwcf.com/Article/details/ggufeqpxi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.yfazqb.com/Article/details/grjuvmdkg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.vehdjk.com/Article/details/gwremqjcj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.tarul.cn/Article/details/gbmeximew.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/gjawmzlsn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.sjlbkw.cn/Article/details/gbwofvadd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.yfazqb.com/Article/details/gjsjpzkxn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.sjlbkw.cn/Article/details/gvvgxkdgf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.tarul.cn/Article/details/gertpezbi.sHtML

[E02] 重复字符串
来源：http://www.blog.vehdjk.com/Article/details/ghkwofram.sHtML

Py:   "ab" * 3
来源：http://blog.sjlbkw.cn/Article/details/gnwnycslb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.bbcook.cn/Article/details/gkdsabmuc.sHtML

JS:   "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/grgpomrdd.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/geeslnqye.sHtML

Java: "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/ggbbbrmlm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.epnwcf.com/Article/details/gvntwahhi.sHtML

Ruby: "ab" * 3
来源：http://blog.fktsv.cn/Article/details/geyqjvyaz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/gqjvmqzyz.sHtML

[E03] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/gxjsojgbe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.sjlbkw.cn/Article/details/gzkvsigdj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/giirvvski.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.epnwcf.com/Article/details/glunaolut.sHtML

TS:   s.slice(1, 4)
来源：http://wap.bbcook.cn/Article/details/gyojuzmol.sHtML

Java: s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gquicujvp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.bbcook.cn/Article/details/gaemluwst.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fktsv.cn/Article/details/gijtzbluu.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.tarul.cn/Article/details/giwfowrtf.sHtML

[E04] 查找子串位置
来源：http://3g.fktsv.cn/Article/details/gdmopqrsd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fktsv.cn/Article/details/guawukuug.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.yfazqb.com/Article/details/guohtrgzk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fktsv.cn/Article/details/gqgyqllzs.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gckqhyexj.sHtML

Java: s.indexOf("x")
来源：http://blog.vehdjk.com/Article/details/gphvxsvqm.sHtML


<!-- 参考信息 -->