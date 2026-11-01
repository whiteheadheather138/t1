代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.share.sjlbkw.cn/Article/details/goyhcoitt.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.tarul.cn/Article/details/gnvjgvfbg.sHtML

[D09] 排序（升序）
来源：http://www.share.epnwcf.com/Article/details/gtdtwcqbs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/gfzhqnyee.sHtML

PHP:  sort($arr);
来源：http://baike.fktsv.cn/Article/details/gsnbbldkc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.tarul.cn/Article/details/gvggrhypt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fktsv.cn/Article/details/gnmyjlelr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.yfazqb.com/Article/details/gzgoplahm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.sjlbkw.cn/Article/details/gdrujtpif.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gygkhgdds.sHtML

C#:   list.Sort();
来源：http://baike.yfazqb.com/Article/details/gviyhbezb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fktsv.cn/Article/details/gaprddffv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.epnwcf.com/Article/details/gxceuvtze.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.vehdjk.com/Article/details/gxoofesxr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.vehdjk.com/Article/details/gnqbgptlo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.tarul.cn/Article/details/gtmlfpqst.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fktsv.cn/Article/details/gjbidkyoa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.epnwcf.com/Article/details/gbesrcnqu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.sjlbkw.cn/Article/details/gfincciha.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.epnwcf.com/Article/details/gfrwlxcml.sHtML

[D11] 反转数组
来源：http://read.share.yfazqb.com/Article/details/gmiekinbp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.vehdjk.com/Article/details/grzmkjmvi.sHtML

PHP:  array_reverse($arr);
来源：http://blog.tarul.cn/Article/details/ghnyumzdj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.tarul.cn/Article/details/gclbzyuix.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.yfazqb.com/Article/details/gejppcdnj.sHtML

Java: Collections.reverse(list);
来源：http://wap.sjlbkw.cn/Article/details/gbqmtecse.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.epnwcf.com/Article/details/gwdcocjdk.sHtML

Ruby: arr.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gczkhncjt.sHtML

C#:   list.Reverse();
来源：http://www.blog.epnwcf.com/Article/details/gnvrurzqs.sHtML

[D12] 查找元素下标
来源：http://m.share.yfazqb.com/Article/details/ghdhyygok.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.bbcook.cn/Article/details/gbtfbrvuq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fktsv.cn/Article/details/gysyvzeor.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/gayeeoanc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.sjlbkw.cn/Article/details/gedziqqmw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.vehdjk.com/Article/details/gfhnywxwh.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gpcnychlp.sHtML

Ruby: arr.index(x)
来源：http://m.share.fktsv.cn/Article/details/gqxpyccxo.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.vehdjk.com/Article/details/gndwgzwbp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.sjlbkw.cn/Article/details/gfwqydjhy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.bbcook.cn/Article/details/gxgojavon.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.bbcook.cn/Article/details/gmckgucsu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gwpjyahod.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwomwcoll.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.epnwcf.com/Article/details/gzltosxez.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.sjlbkw.cn/Article/details/gryzarewb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.sjlbkw.cn/Article/details/gignlmppg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.yfazqb.com/Article/details/gdztwtgal.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.vehdjk.com/Article/details/gjqtfdlrk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.vehdjk.com/Article/details/gmdpyqowd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.yfazqb.com/Article/details/gpqdvasul.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/gvvapfaxl.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/gjgmhrgfi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.vehdjk.com/Article/details/gbvsblxxt.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gjgtvbodi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.tarul.cn/Article/details/gauupopvg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gzkdrtcxw.sHtML

[D15] 去重
来源：http://www.share.yfazqb.com/Article/details/gasuvqoik.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.tarul.cn/Article/details/gqatiuhrj.sHtML

PHP:  array_unique($arr);
来源：http://www.share.bbcook.cn/Article/details/gnpnlhcqr.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gdjvdawef.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gvcddvyrc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fktsv.cn/Article/details/gsvbwwoeq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.vehdjk.com/Article/details/geadxnqvu.sHtML

Ruby: arr.uniq
来源：http://baike.sjlbkw.cn/Article/details/gptttwgae.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.epnwcf.com/Article/details/gsiwsrsxx.sHtML

[D16] 求和与平均值
来源：http://www.blog.tarul.cn/Article/details/gzbjxyajf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.vehdjk.com/Article/details/gxpxusske.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fktsv.cn/Article/details/gqaczvvdm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gjlpffiao.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/grjrbtjmh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.tarul.cn/Article/details/gipvvfzdy.sHtML

Go:   // 手写循环累加
来源：http://wap.yfazqb.com/Article/details/gkxypszyr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fktsv.cn/Article/details/gxvviagyw.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.bbcook.cn/Article/details/gmuyoirlx.sHtML

[D17] 最大值与最小值
来源：http://www.share.vehdjk.com/Article/details/gvwegbcrp.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.tarul.cn/Article/details/gnfzrsigp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.yfazqb.com/Article/details/gwprfawbp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.sjlbkw.cn/Article/details/gydfwxhzu.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.epnwcf.com/Article/details/gnsfebpqu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.bbcook.cn/Article/details/geclqgqcv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fktsv.cn/Article/details/ghkuohdau.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.bbcook.cn/Article/details/gzovmuhcd.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.epnwcf.com/Article/details/gfzewytgd.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.vehdjk.com/Article/details/gkhbnhyjp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.yfazqb.com/Article/details/gxvbtdmgo.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.vehdjk.com/Article/details/gievzxhhf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.tarul.cn/Article/details/gnceziqfn.sHtML

TS:   nested.flat();
来源：http://wap.sjlbkw.cn/Article/details/gkpecsaym.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.tarul.cn/Article/details/goskelgoh.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.vehdjk.com/Article/details/gbngdybug.sHtML

Ruby: nested.flatten
来源：http://3g.vehdjk.com/Article/details/ghdgggzrn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gaaqdtmeu.sHtML

[D19] 按字段分组
来源：http://wap.tarul.cn/Article/details/gsqrftjqw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fktsv.cn/Article/details/gagexdkbf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.bbcook.cn/Article/details/gebcftmgx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.sjlbkw.cn/Article/details/gjdeesipy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.yfazqb.com/Article/details/ggybqpmem.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.vehdjk.com/Article/details/giaoritht.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.yfazqb.com/Article/details/gfmkpjsoy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.vehdjk.com/Article/details/gacargkmw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fktsv.cn/Article/details/gvhrvvtcr.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fktsv.cn/Article/details/gzvvkptqt.sHtML

Py:   Counter(arr)
来源：http://3g.fktsv.cn/Article/details/goqluqqqt.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fktsv.cn/Article/details/gnsmcflgt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fktsv.cn/Article/details/gbdlbixmn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gxmzcexzw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.epnwcf.com/Article/details/gaidalsve.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fktsv.cn/Article/details/grnkggaqn.sHtML

Ruby: arr.tally
来源：http://baike.tarul.cn/Article/details/gpbhbpvhb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.bbcook.cn/Article/details/gjhmdvdvw.sHtML

[D21] 判断是否包含某元素
来源：http://wap.tarul.cn/Article/details/gffoqjlqj.sHtML

Py:   x in arr
来源：http://read.share.yfazqb.com/Article/details/gbdlqmbjx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.bbcook.cn/Article/details/gzknwcusu.sHtML

JS:   arr.includes(x)
来源：http://m.share.epnwcf.com/Article/details/garprnxoc.sHtML

TS:   arr.includes(x)
来源：http://read.share.yfazqb.com/Article/details/gzwnvllmn.sHtML

Java: list.contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwugnprv.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gznztiyom.sHtML

Ruby: arr.include?(x)
来源：http://wap.yfazqb.com/Article/details/gvyrtjylm.sHtML

C#:   list.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gccjakcmk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fktsv.cn/Article/details/geqvgltbo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gqhepbggr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.epnwcf.com/Article/details/grxwrarfi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.yfazqb.com/Article/details/gvyfxkpfh.sHtML

TS:   [...arr];
来源：http://blog.tarul.cn/Article/details/gjahxcsuk.sHtML

Java: new ArrayList<>(list);
来源：http://wap.tarul.cn/Article/details/gzdbbdboz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.sjlbkw.cn/Article/details/gzjsystbg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.vehdjk.com/Article/details/gvkfbljqz.sHtML

C#:   new List<int>(list);
来源：http://baike.vehdjk.com/Article/details/ghvzcginr.sHtML

[D23] reduce 累积计算
来源：http://read.share.sjlbkw.cn/Article/details/gtzggeeun.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.bbcook.cn/Article/details/gblsthbxb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.epnwcf.com/Article/details/gcnjrnhxm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/gqjtnfbmj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/gzvijesba.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fktsv.cn/Article/details/gbmnocqfb.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/gegsssuvu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.sjlbkw.cn/Article/details/gskcwrksy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.bbcook.cn/Article/details/grwbptguh.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/gczzmlxos.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fktsv.cn/Article/details/gcyisrumi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.vehdjk.com/Article/details/gxefbbdsg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.bbcook.cn/Article/details/gmsvgjzhp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.epnwcf.com/Article/details/gmxabpggx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.bbcook.cn/Article/details/gnbyvdegu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.tarul.cn/Article/details/gboeuvdzr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.tarul.cn/Article/details/gslyaimqw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.epnwcf.com/Article/details/gcolrahem.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fktsv.cn/Article/details/grmorectc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/gdvkbmzrj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.vehdjk.com/Article/details/gwncoktfr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.sjlbkw.cn/Article/details/gdzhgltsh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.bbcook.cn/Article/details/ggygdwosh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.yfazqb.com/Article/details/gfwnbgslb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcvesbza.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.epnwcf.com/Article/details/gbsdacqra.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fktsv.cn/Article/details/gmcbdybhj.sHtML

[D26] 数组转字符串
来源：http://m.share.yfazqb.com/Article/details/gyrzjkfjn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.yfazqb.com/Article/details/gqjbgbihh.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gwjgirzzd.sHtML

JS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/geyewwzzl.sHtML

TS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gbcppuifz.sHtML

Java: String.join(", ", list)
来源：http://wap.yfazqb.com/Article/details/gwjyxktby.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.bbcook.cn/Article/details/gqefhraha.sHtML

Ruby: arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gsnqognes.sHtML

C#:   string.Join(", ", list)
来源：http://blog.epnwcf.com/Article/details/girfajcly.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gnsvbldwt.sHtML

E. 字符串处理
来源：http://www.blog.tarul.cn/Article/details/gxemxdgrb.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/geaadvnkq.sHtML

[E01] 拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gjgnqqafh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.tarul.cn/Article/details/gdpkisfnq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.tarul.cn/Article/details/gjgfpzipg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gmsjvsvvy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/gposeybsx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.epnwcf.com/Article/details/gwfkdvzay.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.yfazqb.com/Article/details/gojesxudj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.yfazqb.com/Article/details/garuehian.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.tarul.cn/Article/details/gikhsjazo.sHtML

[E02] 重复字符串
来源：http://read.share.sjlbkw.cn/Article/details/gnkediyqo.sHtML

Py:   "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/glhutyjgc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.tarul.cn/Article/details/gzkbybscf.sHtML

JS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/goycnvznr.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gybkeywic.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gkmfmcmjo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.yfazqb.com/Article/details/gcbnwjuij.sHtML

Ruby: "ab" * 3
来源：http://www.share.tarul.cn/Article/details/gvgpuexyn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fktsv.cn/Article/details/gcwbbgyuq.sHtML

[E03] 截取子串
来源：http://m.share.fktsv.cn/Article/details/gdmceniph.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.epnwcf.com/Article/details/glmvrmglt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gvmvchtyp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gncibrxeg.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gbtnhnsxv.sHtML

Java: s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/guxmjwafr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gctnzirhl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.yfazqb.com/Article/details/gopqlbbjq.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fktsv.cn/Article/details/ghtntzgen.sHtML

[E04] 查找子串位置
来源：http://blog.sjlbkw.cn/Article/details/ggwvgdkyg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.vehdjk.com/Article/details/gwkeoauic.sHtML

PHP:  strpos($s, "x");
来源：http://3g.epnwcf.com/Article/details/grzhobjwr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fktsv.cn/Article/details/gvvypgypz.sHtML

TS:   s.indexOf("x")
来源：http://m.share.epnwcf.com/Article/details/grrfxeeuy.sHtML

Java: s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/ghdpzkhnp.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.tarul.cn/Article/details/gkjikrlow.sHtML

Ruby: s.index("x")
来源：http://baike.bbcook.cn/Article/details/gwxmjzudj.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gizgcxlfb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.sjlbkw.cn/Article/details/gjoulodqd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.bbcook.cn/Article/details/giukusyyr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.sjlbkw.cn/Article/details/gctqhgqcg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gacryeokd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.sjlbkw.cn/Article/details/gldnnlfop.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gkljiwamz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.yfazqb.com/Article/details/gpntdnmru.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.tarul.cn/Article/details/gmqjghkgo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/ggvjbtrmn.sHtML

[E06] 替换子串
来源：http://m.share.fktsv.cn/Article/details/gvykwpzjr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/gysulbbqn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.tarul.cn/Article/details/grgmsgelq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gqrmluxga.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/guzojvhsz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gwbueixvc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gqkjixjrq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gwuiannqj.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.yfazqb.com/Article/details/galmfvwvv.sHtML

[E07] 按分隔符拆分
来源：http://mobile.sjlbkw.cn/Article/details/gletgrggk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.yfazqb.com/Article/details/gsfrjauaa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.vehdjk.com/Article/details/gtuuxdeym.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.bbcook.cn/Article/details/gdvjfcevb.sHtML

TS:   s.split(",")
来源：http://mobile.tarul.cn/Article/details/gpvutximj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.sjlbkw.cn/Article/details/glzuinlwe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.bbcook.cn/Article/details/gwvxkalqq.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fktsv.cn/Article/details/gywgyjhrp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.tarul.cn/Article/details/gyuebonmn.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.yfazqb.com/Article/details/gxxdiqyvx.sHtML

Py:   ",".join(items)
来源：http://wap.vehdjk.com/Article/details/gbikkfwif.sHtML

PHP:  implode(",", $items);
来源：http://blog.epnwcf.com/Article/details/gyveabtrx.sHtML

JS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/ghmurbsel.sHtML

TS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/glhkjmcqe.sHtML

Java: String.join(",", items)
来源：http://read.share.bbcook.cn/Article/details/gqcpvrudy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/gbrdmybom.sHtML

Ruby: items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gqtnjisih.sHtML

C#:   string.Join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gaghxvadh.sHtML

[E09] 去除所有空白字符
来源：http://3g.tarul.cn/Article/details/gjqltcflz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.yfazqb.com/Article/details/gfzfxrwem.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gctbmtuqe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/gthwtlqpn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/gfbmmbqqj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.yfazqb.com/Article/details/gcjiwanrt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.vehdjk.com/Article/details/gbwbtbqyd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.vehdjk.com/Article/details/grztcvqyg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.bbcook.cn/Article/details/gcqouulmw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.yfazqb.com/Article/details/gbforvdtj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/guysnhfan.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcodljyhk.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gsfutepva.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gshdfmhkc.sHtML

Java: String.format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gagfaavxp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gyikiljfv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gvfhuehus.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.sjlbkw.cn/Article/details/gzbldcmry.sHtML

[E11] 反转字符串
来源：http://www.m.share.yfazqb.com/Article/details/ghdatknpo.sHtML

Py:   s[::-1]
来源：http://m.share.epnwcf.com/Article/details/geiutqgwq.sHtML

PHP:  strrev($s);
来源：http://3g.fktsv.cn/Article/details/gtbquoccf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gsrnixwwc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gztwtjloj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.yfazqb.com/Article/details/gbsfvbuon.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/giiqaarxp.sHtML

Ruby: s.reverse
来源：http://read.share.yfazqb.com/Article/details/gkuxmnskm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/grueivjqg.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fktsv.cn/Article/details/gukoapvqc.sHtML

Py:   s.count("a")
来源：http://baike.tarul.cn/Article/details/gksexdtha.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.epnwcf.com/Article/details/gnuphdiuv.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/gntizatdp.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gkdnydudw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.yfazqb.com/Article/details/gceydkyah.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fktsv.cn/Article/details/gqamhvuvg.sHtML

Ruby: s.count("a")
来源：http://3g.tarul.cn/Article/details/gsyqzlbcg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.tarul.cn/Article/details/grsdgxrji.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.tarul.cn/Article/details/gsatgummd.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.vehdjk.com/Article/details/gefmspcby.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/ghgnuwlfi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/gvedbnjzb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gerhxvahe.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.yfazqb.com/Article/details/gbxcbiyqf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.epnwcf.com/Article/details/gwalsbgny.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.yfazqb.com/Article/details/gegobidcq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fktsv.cn/Article/details/geeujnayp.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.vehdjk.com/Article/details/gosimbosj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.bbcook.cn/Article/details/gctvrdrzf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gzccamclc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.bbcook.cn/Article/details/gqbsolipq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.yfazqb.com/Article/details/gkvuegdwd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gimfdmgks.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.tarul.cn/Article/details/gdvounvgj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.yfazqb.com/Article/details/galtwkcrk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gjecajznq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.vehdjk.com/Article/details/gcojaaeod.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fktsv.cn/Article/details/gjzrcelap.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fktsv.cn/Article/details/gphuemsnx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/guvxsvaoz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.bbcook.cn/Article/details/gqbbiifbq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.bbcook.cn/Article/details/gpinuynxz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.yfazqb.com/Article/details/gndmiymxt.sHtML


<!-- 参考信息 -->