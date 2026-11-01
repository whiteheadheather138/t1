代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.blog.yfazqb.com/Article/details/gaqywujzc.sHtML

[D08] 合并两个数组
来源：http://3g.epnwcf.com/Article/details/gwovzzpxx.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.tarul.cn/Article/details/geirdvwlt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.epnwcf.com/Article/details/giuyxzcew.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.yfazqb.com/Article/details/gfkmzwxxn.sHtML

TS:   [...a, ...b];
来源：http://blog.tarul.cn/Article/details/gvgkjnjrg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fktsv.cn/Article/details/glajkbpep.sHtML

Go:   append(a, b...)
来源：http://read.share.sjlbkw.cn/Article/details/gmiuwgwmg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.epnwcf.com/Article/details/gomehpqrj.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.yfazqb.com/Article/details/gmoudgunt.sHtML

[D09] 排序（升序）
来源：http://baike.fktsv.cn/Article/details/gndkptcyl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gznejogdt.sHtML

PHP:  sort($arr);
来源：http://baike.sjlbkw.cn/Article/details/gpredrrgn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fktsv.cn/Article/details/getfwfpoq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.vehdjk.com/Article/details/gvpmpfoqv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.epnwcf.com/Article/details/gfqmxwwyd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gbqvdlbwe.sHtML

Ruby: arr.sort
来源：http://baike.yfazqb.com/Article/details/gvatqonkz.sHtML

C#:   list.Sort();
来源：http://www.blog.sjlbkw.cn/Article/details/gmalplhpv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.vehdjk.com/Article/details/gpqkcmqfx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.vehdjk.com/Article/details/gwxajxkid.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.bbcook.cn/Article/details/gpvegueml.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.epnwcf.com/Article/details/gecvjoylu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.yfazqb.com/Article/details/gxhsfacpd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.sjlbkw.cn/Article/details/gdhmvwnpl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.sjlbkw.cn/Article/details/gaonmotyo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.epnwcf.com/Article/details/gmehrodhe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.tarul.cn/Article/details/ghczmobwy.sHtML

[D11] 反转数组
来源：http://wap.vehdjk.com/Article/details/gcdhhmmbq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/ggcbuqqgo.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gclhlicfr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.epnwcf.com/Article/details/goyfyrfza.sHtML

TS:   [...arr].reverse();
来源：http://www.share.sjlbkw.cn/Article/details/ggmiimopr.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fktsv.cn/Article/details/gokelrenv.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.yfazqb.com/Article/details/gshzxxdze.sHtML

Ruby: arr.reverse
来源：http://mobile.fktsv.cn/Article/details/ghfmfqqwl.sHtML

C#:   list.Reverse();
来源：http://mobile.yfazqb.com/Article/details/ggmdmoyjz.sHtML

[D12] 查找元素下标
来源：http://mobile.bbcook.cn/Article/details/gangizqjp.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.bbcook.cn/Article/details/greqddjfk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gircwxqwq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.yfazqb.com/Article/details/gjmiwhrvg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/grgltafvn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.epnwcf.com/Article/details/gyjzciita.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gboqbbkah.sHtML

Ruby: arr.index(x)
来源：http://m.share.sjlbkw.cn/Article/details/guvdcbpkg.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.vehdjk.com/Article/details/gkzmgqxqz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.epnwcf.com/Article/details/gvirtvmnw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.vehdjk.com/Article/details/giglthtlv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.yfazqb.com/Article/details/goeprgnkh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/ggnqtxqiu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/gzigjkyql.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fktsv.cn/Article/details/ganzaowca.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.bbcook.cn/Article/details/gjtaqhrdx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.bbcook.cn/Article/details/guacqvcul.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.bbcook.cn/Article/details/grkmragwv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.epnwcf.com/Article/details/gmalzhupr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.epnwcf.com/Article/details/gbwhmvjbs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fktsv.cn/Article/details/gwbrsfxnr.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/gjmikuacl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gfurnmnpn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gghtsqpyl.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/gngsrtrei.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.bbcook.cn/Article/details/gcpjnjiix.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gfqnktdtb.sHtML

[D15] 去重
来源：http://baike.yfazqb.com/Article/details/gaqzpfkel.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/gzwfsyqas.sHtML

PHP:  array_unique($arr);
来源：http://wap.sjlbkw.cn/Article/details/gwjcyskrl.sHtML

JS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/geezcxpde.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gyazqblyv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.vehdjk.com/Article/details/gxgmwruiw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fktsv.cn/Article/details/gysoitegt.sHtML

Ruby: arr.uniq
来源：http://wap.bbcook.cn/Article/details/guvjgomby.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.epnwcf.com/Article/details/gvafhvepw.sHtML

[D16] 求和与平均值
来源：http://mobile.bbcook.cn/Article/details/gbgwozpmf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.tarul.cn/Article/details/gwtkfhhxl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gfcrqipuh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/gjrctaqut.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.bbcook.cn/Article/details/gwugtmjrq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.bbcook.cn/Article/details/gvtiwfgsf.sHtML

Go:   // 手写循环累加
来源：http://m.share.tarul.cn/Article/details/gzwtgamkp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.bbcook.cn/Article/details/gsqibktce.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.yfazqb.com/Article/details/galcabkpu.sHtML

[D17] 最大值与最小值
来源：http://blog.bbcook.cn/Article/details/gryicgvyz.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/glntbozhv.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fktsv.cn/Article/details/gdruayosh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.tarul.cn/Article/details/gqnubvefg.sHtML

TS:   Math.max(...arr);
来源：http://wap.bbcook.cn/Article/details/gwsmhuvbv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.vehdjk.com/Article/details/ggwcfnddg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.bbcook.cn/Article/details/gzojyesve.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.bbcook.cn/Article/details/goiferhju.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fktsv.cn/Article/details/gnsjtizqw.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.tarul.cn/Article/details/gtnmaxuam.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.vehdjk.com/Article/details/gelmfagox.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.epnwcf.com/Article/details/gxvmcdmgi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.vehdjk.com/Article/details/ggvuggked.sHtML

TS:   nested.flat();
来源：http://3g.sjlbkw.cn/Article/details/gengdxpvo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.yfazqb.com/Article/details/ghjowewjw.sHtML

Go:   // 手写双层循环
来源：http://3g.yfazqb.com/Article/details/gvipjqdzr.sHtML

Ruby: nested.flatten
来源：http://www.blog.tarul.cn/Article/details/gygannftx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gktzqxiif.sHtML

[D19] 按字段分组
来源：http://blog.bbcook.cn/Article/details/ggccpfgae.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.tarul.cn/Article/details/ggwpebwos.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.yfazqb.com/Article/details/gqfpuybhs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.yfazqb.com/Article/details/gcztgfnsp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/ggsqgbyqn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.bbcook.cn/Article/details/glgqjxkjc.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.tarul.cn/Article/details/gnrrsyayq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.epnwcf.com/Article/details/gddaqluba.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.vehdjk.com/Article/details/gwzdokjte.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.yfazqb.com/Article/details/godhtlscf.sHtML

Py:   Counter(arr)
来源：http://wap.tarul.cn/Article/details/gkbgozozf.sHtML

PHP:  array_count_values($arr);
来源：http://blog.yfazqb.com/Article/details/gwdoqqdyb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fktsv.cn/Article/details/gpgyztpab.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gmajipsxi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fktsv.cn/Article/details/gcgvrucdf.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.sjlbkw.cn/Article/details/gjkybbhbw.sHtML

Ruby: arr.tally
来源：http://baike.sjlbkw.cn/Article/details/gmxfrwjgr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.tarul.cn/Article/details/gpdpdehsd.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.yfazqb.com/Article/details/gugapjine.sHtML

Py:   x in arr
来源：http://www.blog.bbcook.cn/Article/details/gvvlcthzl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.bbcook.cn/Article/details/gheoinnvw.sHtML

JS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gztqtlcca.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gkeddjims.sHtML

Java: list.contains(x)
来源：http://3g.fktsv.cn/Article/details/gevqzbhrb.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.epnwcf.com/Article/details/glhydanqk.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gcvhlxoxc.sHtML

C#:   list.Contains(x)
来源：http://wap.vehdjk.com/Article/details/gjdvywkwr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fktsv.cn/Article/details/gonzkhkth.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.tarul.cn/Article/details/gauhovhnz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.vehdjk.com/Article/details/gkvkzdylw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.epnwcf.com/Article/details/gudlzhcju.sHtML

TS:   [...arr];
来源：http://www.share.bbcook.cn/Article/details/gxbhpsffl.sHtML

Java: new ArrayList<>(list);
来源：http://wap.yfazqb.com/Article/details/gtllkralc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.sjlbkw.cn/Article/details/gjycbmaef.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.sjlbkw.cn/Article/details/gnevjyuma.sHtML

C#:   new List<int>(list);
来源：http://mobile.fktsv.cn/Article/details/gwigbgyid.sHtML

[D23] reduce 累积计算
来源：http://wap.sjlbkw.cn/Article/details/glzuqvslr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwusvarbf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fktsv.cn/Article/details/gzmtmrcds.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gojgansyt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gmkcluzgs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fktsv.cn/Article/details/gxiiajcbj.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gmeznsjaa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.yfazqb.com/Article/details/glkdhmjtf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.tarul.cn/Article/details/gmujuihaw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fktsv.cn/Article/details/ghdadrcdo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.yfazqb.com/Article/details/gjegylqfs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.epnwcf.com/Article/details/ghwnijfxe.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.tarul.cn/Article/details/grisqbvvt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.vehdjk.com/Article/details/ggaeqelej.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.yfazqb.com/Article/details/gfhusehrb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.tarul.cn/Article/details/grqwsifri.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.epnwcf.com/Article/details/gicgiwqdm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.bbcook.cn/Article/details/grnpjokxb.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fktsv.cn/Article/details/gagsgowib.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.tarul.cn/Article/details/gvhkpoply.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.vehdjk.com/Article/details/gdpxnaffv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fktsv.cn/Article/details/gjetpydnw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.bbcook.cn/Article/details/gnaydptxo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.yfazqb.com/Article/details/garnrscic.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.vehdjk.com/Article/details/gybamname.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnftdwhl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.sjlbkw.cn/Article/details/glgzmkwjb.sHtML

[D26] 数组转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gjzwdmufy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fktsv.cn/Article/details/gluprtciq.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.tarul.cn/Article/details/gmatprnsp.sHtML

JS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/grevzqfit.sHtML

TS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/ghnqxwrgi.sHtML

Java: String.join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/guidxrouu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.epnwcf.com/Article/details/grbudwlnz.sHtML

Ruby: arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gyanrmubb.sHtML

C#:   string.Join(", ", list)
来源：http://blog.sjlbkw.cn/Article/details/gycsvtvjg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvoncuuoj.sHtML

E. 字符串处理
来源：http://www.m.share.vehdjk.com/Article/details/gnhbbjqtr.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghhrbtkbd.sHtML

[E01] 拼接字符串
来源：http://baike.tarul.cn/Article/details/gzwfiptmz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.yfazqb.com/Article/details/glwmpgcsn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.epnwcf.com/Article/details/glkeyqqeq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.yfazqb.com/Article/details/gzngwwurw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gbsjemcyr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fktsv.cn/Article/details/gcemtyxmr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.yfazqb.com/Article/details/gvcvglyjl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fktsv.cn/Article/details/gprhxowzq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.yfazqb.com/Article/details/gywmpeich.sHtML

[E02] 重复字符串
来源：http://www.share.yfazqb.com/Article/details/grgbngutf.sHtML

Py:   "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/ggnaxomlq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.vehdjk.com/Article/details/gbkumpkkp.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gqvxcrqyz.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gbardzcni.sHtML

Java: "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gnsluqxku.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fktsv.cn/Article/details/gijzadsjv.sHtML

Ruby: "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/gujwzamws.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fktsv.cn/Article/details/gcorogqmi.sHtML

[E03] 截取子串
来源：http://m.share.tarul.cn/Article/details/gycjhcsvd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.vehdjk.com/Article/details/gydbsoekz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gkqvjbzed.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.tarul.cn/Article/details/gqrlwkdik.sHtML

TS:   s.slice(1, 4)
来源：http://baike.epnwcf.com/Article/details/gyaxbende.sHtML

Java: s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gfyujxkeo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.epnwcf.com/Article/details/gmyxbyigg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.yfazqb.com/Article/details/gikxbwmkh.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.epnwcf.com/Article/details/gtjuxamhi.sHtML

[E04] 查找子串位置
来源：http://read.share.bbcook.cn/Article/details/gdqxzwwit.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gpfdnzwfk.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaemyecq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.epnwcf.com/Article/details/gyzkumbls.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gjqfnhdgs.sHtML

Java: s.indexOf("x")
来源：http://blog.vehdjk.com/Article/details/gigkjufty.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.bbcook.cn/Article/details/grgtrsrxg.sHtML

Ruby: s.index("x")
来源：http://3g.fktsv.cn/Article/details/grzelubjj.sHtML

C#:   s.IndexOf("x")
来源：http://baike.bbcook.cn/Article/details/gxasijhqt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.bbcook.cn/Article/details/gdbfuuror.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gkhbbrcwi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.tarul.cn/Article/details/gqtfdjplu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gfofhevwa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.epnwcf.com/Article/details/ggxrgfhdc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.tarul.cn/Article/details/gnyomwvwb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.tarul.cn/Article/details/gpjfcrzrk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.yfazqb.com/Article/details/gffhgqdbi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gfgvteoti.sHtML

[E06] 替换子串
来源：http://baike.yfazqb.com/Article/details/galylluix.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/gxwisduoq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.yfazqb.com/Article/details/gsplhqvwj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gestkuqby.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gzyrivlcg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gdzpklxqn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gmxpqqfia.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gpbrklusq.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gsnhhhafb.sHtML

[E07] 按分隔符拆分
来源：http://blog.epnwcf.com/Article/details/gpephipow.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.bbcook.cn/Article/details/glvvkrwae.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.bbcook.cn/Article/details/gupmufmlw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fktsv.cn/Article/details/gqssrviil.sHtML

TS:   s.split(",")
来源：http://blog.epnwcf.com/Article/details/gmcqgmhte.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.yfazqb.com/Article/details/gsiamslfh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.epnwcf.com/Article/details/gfoknqncj.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.yfazqb.com/Article/details/gfpyxzmrd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.bbcook.cn/Article/details/gggkjicbe.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.bbcook.cn/Article/details/gyjiggyap.sHtML

Py:   ",".join(items)
来源：http://m.share.fktsv.cn/Article/details/gphpujuvs.sHtML

PHP:  implode(",", $items);
来源：http://blog.fktsv.cn/Article/details/giyipijtz.sHtML

JS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/gkmgwnbse.sHtML

TS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gflxzxwpe.sHtML

Java: String.join(",", items)
来源：http://baike.yfazqb.com/Article/details/gefjgyunt.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.epnwcf.com/Article/details/gpbwneukv.sHtML

Ruby: items.join(",")
来源：http://3g.vehdjk.com/Article/details/gbtpjbayq.sHtML

C#:   string.Join(",", items)
来源：http://wap.yfazqb.com/Article/details/gitimwcqf.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.tarul.cn/Article/details/gyrjrmuor.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.yfazqb.com/Article/details/gifvcggev.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.vehdjk.com/Article/details/gkvtzmaos.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/ggpyimizp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gteomsdoy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.yfazqb.com/Article/details/gqxvjacnv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.bbcook.cn/Article/details/gopvxpusr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fktsv.cn/Article/details/gkdeuegco.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.vehdjk.com/Article/details/grjrmhkgk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.yfazqb.com/Article/details/gibjgkbpq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gajbibibt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fktsv.cn/Article/details/gynhpfrsu.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/ginethtms.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gvaiguoso.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gzwwoqdlw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gyqlzrukv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/grjlrtbrf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.sjlbkw.cn/Article/details/ghbpxvprr.sHtML

[E11] 反转字符串
来源：http://blog.fktsv.cn/Article/details/gshdthkof.sHtML

Py:   s[::-1]
来源：http://baike.tarul.cn/Article/details/gbegggzpo.sHtML

PHP:  strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gdxsklwwl.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gpndtivup.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gueqiqcak.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gxgqnkqvc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.epnwcf.com/Article/details/gidwmsskn.sHtML

Ruby: s.reverse
来源：http://mobile.yfazqb.com/Article/details/ggegxvpev.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/goexweoqp.sHtML

[E12] 统计某字符出现次数
来源：http://wap.tarul.cn/Article/details/gyenbcqta.sHtML

Py:   s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gxhducxzy.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.vehdjk.com/Article/details/gcmgkbsos.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/glfnkvcdo.sHtML

TS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gkkajnbtf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.epnwcf.com/Article/details/ginmjuxnf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fktsv.cn/Article/details/gdonqlcfl.sHtML

Ruby: s.count("a")
来源：http://blog.fktsv.cn/Article/details/gxajddmhy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fktsv.cn/Article/details/galmkqbzp.sHtML

[E13] 逐字符遍历
来源：http://wap.sjlbkw.cn/Article/details/gmgehdlfy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.tarul.cn/Article/details/gwrqiuywj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fktsv.cn/Article/details/gkdelbdbv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.tarul.cn/Article/details/gjrorsspz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gimpffnfk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.epnwcf.com/Article/details/ggbzxgfek.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.bbcook.cn/Article/details/gjtrfreqj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fktsv.cn/Article/details/gdwfvmmfj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.yfazqb.com/Article/details/gmfjcegji.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.epnwcf.com/Article/details/gzxqlmkzi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.epnwcf.com/Article/details/gghlxaurg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.epnwcf.com/Article/details/gcidxxfay.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.vehdjk.com/Article/details/gkxstmpwb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.bbcook.cn/Article/details/gmrzpovga.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fktsv.cn/Article/details/grqpkhufo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.sjlbkw.cn/Article/details/gzfzwlfup.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.vehdjk.com/Article/details/geofszfhv.sHtML


<!-- 参考信息 -->