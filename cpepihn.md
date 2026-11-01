代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fktsv.cn/Article/details/gujqwdlcz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/gvsfiajsz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.sjlbkw.cn/Article/details/gwcjhelqe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.vehdjk.com/Article/details/gcrbzfdwt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.epnwcf.com/Article/details/gkcgmhbaz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fktsv.cn/Article/details/gnhqcmksh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.vehdjk.com/Article/details/gdsdpobhs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.epnwcf.com/Article/details/garurodwx.sHtML

[D11] 反转数组
来源：http://www.share.sjlbkw.cn/Article/details/giwflsqsr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.tarul.cn/Article/details/gmigaazdp.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.bbcook.cn/Article/details/gfdjmstwv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.tarul.cn/Article/details/gsymlyhie.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fktsv.cn/Article/details/givqqsyzw.sHtML

Java: Collections.reverse(list);
来源：http://3g.vehdjk.com/Article/details/gcoavqbmn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.yfazqb.com/Article/details/goiectxam.sHtML

Ruby: arr.reverse
来源：http://read.share.fktsv.cn/Article/details/gktoohuik.sHtML

C#:   list.Reverse();
来源：http://read.share.vehdjk.com/Article/details/genjhimwj.sHtML

[D12] 查找元素下标
来源：http://wap.vehdjk.com/Article/details/glwbeofcx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.epnwcf.com/Article/details/gnaylsuis.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.yfazqb.com/Article/details/gdqvixqsn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gmmaahdjd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gvzscvyvu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fktsv.cn/Article/details/gkacxmkvw.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.vehdjk.com/Article/details/ghaipwjei.sHtML

Ruby: arr.index(x)
来源：http://www.blog.tarul.cn/Article/details/gtkwfjndg.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.yfazqb.com/Article/details/gqykskygk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.yfazqb.com/Article/details/gxgqwabke.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.bbcook.cn/Article/details/grufovrjb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.yfazqb.com/Article/details/glqipfacq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.epnwcf.com/Article/details/gurrdhoyt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/gdcrzhhus.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gxnyawscd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.vehdjk.com/Article/details/geuknqmgw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.epnwcf.com/Article/details/geoseybes.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.bbcook.cn/Article/details/golmnxdwo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.bbcook.cn/Article/details/grngfinwm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.bbcook.cn/Article/details/gzbzquxeb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.sjlbkw.cn/Article/details/gnkxjrucd.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.vehdjk.com/Article/details/glynjgvpb.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/gunqeldzd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/gtnmxiovi.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gygzkgeah.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.yfazqb.com/Article/details/gvafeuwky.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gisdvkheo.sHtML

[D15] 去重
来源：http://www.m.share.fktsv.cn/Article/details/gtczpdwej.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.tarul.cn/Article/details/gfnjlkmre.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fktsv.cn/Article/details/gepiebwzb.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gwdukpntt.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/grseanjdt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.tarul.cn/Article/details/gsxyketlm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.vehdjk.com/Article/details/gfwmijwlj.sHtML

Ruby: arr.uniq
来源：http://baike.tarul.cn/Article/details/gfgqcqjkp.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.sjlbkw.cn/Article/details/gpmpmmzzk.sHtML

[D16] 求和与平均值
来源：http://blog.sjlbkw.cn/Article/details/gjbqfglez.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gtvuzsozk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.tarul.cn/Article/details/gvzinehub.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gyrovigxr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/grdmxorol.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.tarul.cn/Article/details/gagrxwzlx.sHtML

Go:   // 手写循环累加
来源：http://baike.yfazqb.com/Article/details/gieazwowo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.sjlbkw.cn/Article/details/ginitnbrt.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fktsv.cn/Article/details/gheirrctd.sHtML

[D17] 最大值与最小值
来源：http://baike.tarul.cn/Article/details/gxggvxcer.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.epnwcf.com/Article/details/gaikzzzjn.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.vehdjk.com/Article/details/guoprhnok.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.vehdjk.com/Article/details/gozdolgjn.sHtML

TS:   Math.max(...arr);
来源：http://3g.sjlbkw.cn/Article/details/gbfyqeeqd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.bbcook.cn/Article/details/gpbvmtfop.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.bbcook.cn/Article/details/gwbsfealh.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.sjlbkw.cn/Article/details/grqcmcvix.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.epnwcf.com/Article/details/gddkynuzp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.tarul.cn/Article/details/gvwlfirrs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fktsv.cn/Article/details/gdkgfvcwc.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.bbcook.cn/Article/details/garzsfwmn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.tarul.cn/Article/details/galmdisia.sHtML

TS:   nested.flat();
来源：http://baike.vehdjk.com/Article/details/gjixheapj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fktsv.cn/Article/details/gurswmfkn.sHtML

Go:   // 手写双层循环
来源：http://m.share.yfazqb.com/Article/details/gsuxvnygo.sHtML

Ruby: nested.flatten
来源：http://wap.yfazqb.com/Article/details/ghumhlcod.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.vehdjk.com/Article/details/gyuozdvuj.sHtML

[D19] 按字段分组
来源：http://www.blog.tarul.cn/Article/details/gliombzxf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.tarul.cn/Article/details/ggvxfdfit.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.vehdjk.com/Article/details/glhgpxzdv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.yfazqb.com/Article/details/gvuutklid.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.bbcook.cn/Article/details/gmicsvpwc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.sjlbkw.cn/Article/details/gviifbmyl.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.vehdjk.com/Article/details/gzjpbcrzz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fktsv.cn/Article/details/gkflvfywc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.tarul.cn/Article/details/gmtoapizv.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.epnwcf.com/Article/details/gnnyyrain.sHtML

Py:   Counter(arr)
来源：http://3g.epnwcf.com/Article/details/gnuwehqkh.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fktsv.cn/Article/details/gvraxavhy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.vehdjk.com/Article/details/gervwwcso.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/gxkvfzimt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.tarul.cn/Article/details/ggbrlzepd.sHtML

Go:   // 手写 map[T]int
来源：http://blog.bbcook.cn/Article/details/gkcqjoftu.sHtML

Ruby: arr.tally
来源：http://www.m.share.yfazqb.com/Article/details/giywtqpnj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.sjlbkw.cn/Article/details/gboirlpja.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fktsv.cn/Article/details/gqsvqstas.sHtML

Py:   x in arr
来源：http://baike.tarul.cn/Article/details/gorhhmvfv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.vehdjk.com/Article/details/gteqnhwfe.sHtML

JS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/gckzqppon.sHtML

TS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gmdgopnuw.sHtML

Java: list.contains(x)
来源：http://blog.yfazqb.com/Article/details/gskwfzuom.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gbqmsvshp.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gwkczpjsw.sHtML

C#:   list.Contains(x)
来源：http://blog.yfazqb.com/Article/details/gilnpkfqr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.bbcook.cn/Article/details/gspcsqtmm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.bbcook.cn/Article/details/gdfayilpr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fktsv.cn/Article/details/gribxwimx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.tarul.cn/Article/details/gpgdanthw.sHtML

TS:   [...arr];
来源：http://m.share.sjlbkw.cn/Article/details/gaokwdvzn.sHtML

Java: new ArrayList<>(list);
来源：http://3g.tarul.cn/Article/details/gihaebtzy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.yfazqb.com/Article/details/gmjfsxqkp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.epnwcf.com/Article/details/gzlvgpfvb.sHtML

C#:   new List<int>(list);
来源：http://3g.tarul.cn/Article/details/gcyiziyvo.sHtML

[D23] reduce 累积计算
来源：http://3g.sjlbkw.cn/Article/details/gaknnbeez.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.epnwcf.com/Article/details/gsenojstd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gdbukeocq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/ggqamkmbi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gccocqcjt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.epnwcf.com/Article/details/ggdgbkwbb.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/gtiruzjbm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fktsv.cn/Article/details/gtrqynqws.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fktsv.cn/Article/details/glfhgimkg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fktsv.cn/Article/details/gnnfpmuip.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.bbcook.cn/Article/details/gkcruddwy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.epnwcf.com/Article/details/gfirgzfyt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gqogakgqi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gulqhhnct.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.sjlbkw.cn/Article/details/gudzcwrqb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.vehdjk.com/Article/details/gcoadlyyv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.tarul.cn/Article/details/gedhqtyyx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.vehdjk.com/Article/details/gvwtwhqur.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.vehdjk.com/Article/details/gbjgcatff.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.yfazqb.com/Article/details/gszfbdfpe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.bbcook.cn/Article/details/gexchpqug.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.tarul.cn/Article/details/gxxaalflz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.tarul.cn/Article/details/ghmgnjjrb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gejauvpzm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fktsv.cn/Article/details/gafultykj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.epnwcf.com/Article/details/gsnfdmaly.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.bbcook.cn/Article/details/geggfrgdl.sHtML

[D26] 数组转字符串
来源：http://baike.sjlbkw.cn/Article/details/gvnwblscc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.tarul.cn/Article/details/gqlpuyxkk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.tarul.cn/Article/details/gtuuzcrbj.sHtML

JS:   arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gxrdwdduh.sHtML

TS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/glqpeshvt.sHtML

Java: String.join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/gwwrpblpk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.vehdjk.com/Article/details/gmezgapmx.sHtML

Ruby: arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gmjvdqlnt.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.bbcook.cn/Article/details/gvapfdsns.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gfjofycah.sHtML

E. 字符串处理
来源：http://baike.sjlbkw.cn/Article/details/gmhhuqblw.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gijzlfpev.sHtML

[E01] 拼接字符串
来源：http://mobile.tarul.cn/Article/details/gbofeieti.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.vehdjk.com/Article/details/gqtfbvqyw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gezyincqb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.tarul.cn/Article/details/gaezfsbsj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.yfazqb.com/Article/details/gkfzjcqnw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.yfazqb.com/Article/details/gwmwmmhpz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.sjlbkw.cn/Article/details/guhdxxmlm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fktsv.cn/Article/details/gshejojhz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gbhsvuvxd.sHtML

[E02] 重复字符串
来源：http://www.share.fktsv.cn/Article/details/gsbwvntwo.sHtML

Py:   "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gmpeaytfb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.sjlbkw.cn/Article/details/gajboyewv.sHtML

JS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/giheavcbe.sHtML

TS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gtugadajw.sHtML

Java: "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gbzicymti.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.epnwcf.com/Article/details/ganhjuyrh.sHtML

Ruby: "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gvfljerby.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fktsv.cn/Article/details/grkmwmept.sHtML

[E03] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/gqjjlaamk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fktsv.cn/Article/details/getdhgezq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gatqbgypl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gblwecrhj.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gylbanhfa.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/grrvvjhud.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.vehdjk.com/Article/details/gflfzdoid.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.yfazqb.com/Article/details/gjkgqnopz.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fktsv.cn/Article/details/gqfsqvklw.sHtML

[E04] 查找子串位置
来源：http://read.share.tarul.cn/Article/details/gjbzrclka.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fktsv.cn/Article/details/gwpyqxwcw.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnufaurt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.yfazqb.com/Article/details/gznxeqfgc.sHtML

TS:   s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/galyewiyu.sHtML

Java: s.indexOf("x")
来源：http://read.share.bbcook.cn/Article/details/gflkxzmuy.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.sjlbkw.cn/Article/details/gpdczdarh.sHtML

Ruby: s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/gslqvvxcc.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gbusbtcwp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fktsv.cn/Article/details/gqodnmtru.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.bbcook.cn/Article/details/gxjoyykxs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.epnwcf.com/Article/details/gpfoxkkrp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/gygvvtvei.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.yfazqb.com/Article/details/gyxkpidms.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gravmxdny.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.yfazqb.com/Article/details/gwjsuljzz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.bbcook.cn/Article/details/gppanfzgj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gdkxqmbsx.sHtML

[E06] 替换子串
来源：http://3g.sjlbkw.cn/Article/details/govhsbncx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/gqkiycytd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.epnwcf.com/Article/details/gcmtxqmsa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gusjankwj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gpppzcxsk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/geyvsyvrw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gzaigdlbd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fktsv.cn/Article/details/gaznlyeak.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.vehdjk.com/Article/details/gtuntjnvx.sHtML

[E07] 按分隔符拆分
来源：http://mobile.epnwcf.com/Article/details/gwyumljhi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.tarul.cn/Article/details/gqzooskhy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fktsv.cn/Article/details/ghitbygqk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fktsv.cn/Article/details/grdtpguxz.sHtML

TS:   s.split(",")
来源：http://baike.fktsv.cn/Article/details/gjbwrrilv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.tarul.cn/Article/details/gqdywbzxv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.vehdjk.com/Article/details/gnrxnaamq.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fktsv.cn/Article/details/gaykgwlzt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.epnwcf.com/Article/details/gpaoypouj.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fktsv.cn/Article/details/gysjwdacq.sHtML

Py:   ",".join(items)
来源：http://mobile.vehdjk.com/Article/details/gayzrznqo.sHtML

PHP:  implode(",", $items);
来源：http://baike.sjlbkw.cn/Article/details/gianhoyee.sHtML

JS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gcstpelnd.sHtML

TS:   items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gqgkablbt.sHtML

Java: String.join(",", items)
来源：http://m.share.vehdjk.com/Article/details/gqcfjvgtp.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.yfazqb.com/Article/details/gvchybwtq.sHtML

Ruby: items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gpxlbmcyj.sHtML

C#:   string.Join(",", items)
来源：http://3g.yfazqb.com/Article/details/gsvswiqyp.sHtML

[E09] 去除所有空白字符
来源：http://baike.tarul.cn/Article/details/grnxuuqtu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.epnwcf.com/Article/details/goqnfyuzw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gyvxqhecf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/geqipfaap.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/gfvsdrnia.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.yfazqb.com/Article/details/gwdstutez.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fktsv.cn/Article/details/gevslhqex.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.vehdjk.com/Article/details/gxysvzbcv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gfeiglhxd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.bbcook.cn/Article/details/gxcntzifg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gntzrrddf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.tarul.cn/Article/details/gzbcphzmo.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gsyggcihe.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/goigfphsg.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gjpejjugx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gmifxnapw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gphqyimfy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.sjlbkw.cn/Article/details/gucjhiyrf.sHtML

[E11] 反转字符串
来源：http://m.share.yfazqb.com/Article/details/gethwbjnu.sHtML

Py:   s[::-1]
来源：http://www.share.fktsv.cn/Article/details/gxwpgccca.sHtML

PHP:  strrev($s);
来源：http://3g.vehdjk.com/Article/details/gptgieiju.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gxbjtuftm.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gothrlksy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.tarul.cn/Article/details/gehnrrmtu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.vehdjk.com/Article/details/gtwgtotsp.sHtML

Ruby: s.reverse
来源：http://blog.epnwcf.com/Article/details/gtcwoyjfo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/ggidzfysv.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.tarul.cn/Article/details/glqyvpkmk.sHtML

Py:   s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gtfraksck.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.sjlbkw.cn/Article/details/gppcjwzpw.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/geozsqepf.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/gvodlyfzm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.epnwcf.com/Article/details/goeimjlls.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fktsv.cn/Article/details/gvizlowep.sHtML

Ruby: s.count("a")
来源：http://m.share.tarul.cn/Article/details/gkbnfnzbl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.yfazqb.com/Article/details/gxhhvrppz.sHtML

[E13] 逐字符遍历
来源：http://www.share.sjlbkw.cn/Article/details/gxsxfezmn.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.vehdjk.com/Article/details/gzaylpywz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.tarul.cn/Article/details/gnrcdhoez.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gookeqbsk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gphkxfqxf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.tarul.cn/Article/details/gyqfzmzol.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.sjlbkw.cn/Article/details/gzhdjmdos.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.sjlbkw.cn/Article/details/gyyzqmifx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/gubnphnsg.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.yfazqb.com/Article/details/grkkifldi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.vehdjk.com/Article/details/gbiqxkgvf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.sjlbkw.cn/Article/details/gleyvrpqf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.bbcook.cn/Article/details/gwtnsnpxr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.vehdjk.com/Article/details/gijnhsxck.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.bbcook.cn/Article/details/gtqkqnyrc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.tarul.cn/Article/details/giwdkqhwt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.sjlbkw.cn/Article/details/genvcrgym.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.tarul.cn/Article/details/gjfniiozq.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.tarul.cn/Article/details/gxcozvxoo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.yfazqb.com/Article/details/gitopoici.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gwpyaolzj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.bbcook.cn/Article/details/gjuuevopl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fktsv.cn/Article/details/gequnxttw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fktsv.cn/Article/details/gdlnumtfi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.sjlbkw.cn/Article/details/gyvtkfxoc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.vehdjk.com/Article/details/gjpbmhohp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.vehdjk.com/Article/details/gsshmfcdl.sHtML

[E16] 数字千分位
来源：http://www.m.share.fktsv.cn/Article/details/gztxpuxil.sHtML

Py:   f"{1234567:,}"
来源：http://blog.yfazqb.com/Article/details/gpfwcjavu.sHtML

PHP:  number_format(1234567);
来源：http://wap.sjlbkw.cn/Article/details/gzhllbaul.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/gmicqntff.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gnggshmue.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.tarul.cn/Article/details/glumdgiln.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fktsv.cn/Article/details/gabuwjthw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.bbcook.cn/Article/details/grfbtybyw.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.sjlbkw.cn/Article/details/gymdnfrgm.sHtML

[E17] 首字母大写
来源：http://blog.bbcook.cn/Article/details/gxqeavjiw.sHtML


<!-- 参考信息 -->