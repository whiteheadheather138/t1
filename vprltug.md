代发 wailian999

Java: list.size();
来源：http://blog.bbcook.cn/Article/details/gasnmadns.sHtML

Go:   len(arr)
来源：http://wap.vehdjk.com/Article/details/gbyztlsrx.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.yfazqb.com/Article/details/gwzwgqwug.sHtML

C#:   list.Count;
来源：http://read.share.fktsv.cn/Article/details/gyzdcvelm.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.yfazqb.com/Article/details/gecvcqgli.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.bbcook.cn/Article/details/gepbzfipz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.yfazqb.com/Article/details/gonrtbdga.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/gsfrkuzhc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.bbcook.cn/Article/details/gqbspzvwj.sHtML

Java: list.subList(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gsbvduvbi.sHtML

Go:   arr[1:4]
来源：http://www.share.vehdjk.com/Article/details/gtrnqgibw.sHtML

Ruby: arr[1, 3]
来源：http://baike.epnwcf.com/Article/details/glnzjmegu.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/ggubzvkxu.sHtML

[D08] 合并两个数组
来源：http://www.blog.epnwcf.com/Article/details/gjmrwuexd.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.yfazqb.com/Article/details/gxgwzkbep.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.bbcook.cn/Article/details/gmfgbuowy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.tarul.cn/Article/details/ghpyarbjh.sHtML

TS:   [...a, ...b];
来源：http://m.share.yfazqb.com/Article/details/ggrjzxqbc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.yfazqb.com/Article/details/gcpqcenvn.sHtML

Go:   append(a, b...)
来源：http://www.blog.epnwcf.com/Article/details/glocmlekp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fktsv.cn/Article/details/gqttxabyy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/glahmdmcg.sHtML

[D09] 排序（升序）
来源：http://www.m.share.bbcook.cn/Article/details/gnnnkdbya.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gwbesrwpc.sHtML

PHP:  sort($arr);
来源：http://blog.epnwcf.com/Article/details/gungxymle.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.sjlbkw.cn/Article/details/gmfmnvuuu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.sjlbkw.cn/Article/details/gwodberpp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.bbcook.cn/Article/details/gjypzdeuf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gotgjrbpg.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/gtgfzhpcp.sHtML

C#:   list.Sort();
来源：http://www.m.share.fktsv.cn/Article/details/gshvwwzoi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.vehdjk.com/Article/details/gkuzdxyqz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.sjlbkw.cn/Article/details/gidfuylpd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.epnwcf.com/Article/details/gapjrckmh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gwjaihdei.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.sjlbkw.cn/Article/details/gngknlcxi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.yfazqb.com/Article/details/gdflfdubp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.vehdjk.com/Article/details/ghhsjqmrf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.yfazqb.com/Article/details/guemawslh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.vehdjk.com/Article/details/gtxqmaasu.sHtML

[D11] 反转数组
来源：http://read.share.epnwcf.com/Article/details/ggfphwrnc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.epnwcf.com/Article/details/gmjjsigne.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.yfazqb.com/Article/details/grlfmlwnx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.bbcook.cn/Article/details/gpauqihit.sHtML

TS:   [...arr].reverse();
来源：http://3g.yfazqb.com/Article/details/gwheieljd.sHtML

Java: Collections.reverse(list);
来源：http://wap.fktsv.cn/Article/details/gbeivvyoi.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.yfazqb.com/Article/details/gsoussssn.sHtML

Ruby: arr.reverse
来源：http://baike.sjlbkw.cn/Article/details/gcjhitgwj.sHtML

C#:   list.Reverse();
来源：http://wap.yfazqb.com/Article/details/gybmrxhqe.sHtML

[D12] 查找元素下标
来源：http://mobile.bbcook.cn/Article/details/gnhsxbfqh.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.tarul.cn/Article/details/gxjiqbdwb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.yfazqb.com/Article/details/glrvnsvqi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/gjbzseqgf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/gssgqqetb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fktsv.cn/Article/details/gwaiksyac.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gysfkanlg.sHtML

Ruby: arr.index(x)
来源：http://blog.yfazqb.com/Article/details/gmmtrxjht.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.yfazqb.com/Article/details/gejqdlbsy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.sjlbkw.cn/Article/details/gjowgzwao.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gbxgtuyvi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.bbcook.cn/Article/details/grmwepeea.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gbcolkhjt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.epnwcf.com/Article/details/gaffdhhxz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gflntcrgw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.sjlbkw.cn/Article/details/gwccfltqe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fktsv.cn/Article/details/gbibnxllu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gnfrnanby.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.yfazqb.com/Article/details/gjiycvxma.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.bbcook.cn/Article/details/gfqdwjdbn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.tarul.cn/Article/details/gawogynch.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/getyobcar.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fktsv.cn/Article/details/gwwiutdyd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.yfazqb.com/Article/details/grxtzmner.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gyzmlujfg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gpppjnawq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gzdqxphax.sHtML

[D15] 去重
来源：http://m.share.fktsv.cn/Article/details/gezcccufg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/gjemejqym.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.bbcook.cn/Article/details/gqazshiyz.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/geysctxfc.sHtML

TS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gecgxezdl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.sjlbkw.cn/Article/details/gjqvxqpzo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.yfazqb.com/Article/details/gdznocavc.sHtML

Ruby: arr.uniq
来源：http://www.share.epnwcf.com/Article/details/gocjyjopg.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.tarul.cn/Article/details/gzqlydeop.sHtML

[D16] 求和与平均值
来源：http://baike.vehdjk.com/Article/details/gfhaphfnp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gawesgtbq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.yfazqb.com/Article/details/gvhwapjdl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.epnwcf.com/Article/details/ghuuvkwmb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/gqkbyahlv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fktsv.cn/Article/details/grrrcwfpg.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.yfazqb.com/Article/details/gpboijhtg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.yfazqb.com/Article/details/gmsameipf.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/gyderpdmn.sHtML

[D17] 最大值与最小值
来源：http://blog.bbcook.cn/Article/details/gcvzbetks.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.yfazqb.com/Article/details/gbdekxhee.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.tarul.cn/Article/details/goqedmxjy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.epnwcf.com/Article/details/gjauvagwb.sHtML

TS:   Math.max(...arr);
来源：http://m.share.epnwcf.com/Article/details/gldjyzfnq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.sjlbkw.cn/Article/details/gwzqeptvr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.epnwcf.com/Article/details/gldtfdcuv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fktsv.cn/Article/details/gxoyckwdu.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.epnwcf.com/Article/details/gyjwjgcwz.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.epnwcf.com/Article/details/gyfrxdqmz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.yfazqb.com/Article/details/ggjnrlgph.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/gjfiyhoqz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.sjlbkw.cn/Article/details/gjkhzaggk.sHtML

TS:   nested.flat();
来源：http://www.share.epnwcf.com/Article/details/gmgcsyzao.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.bbcook.cn/Article/details/gohwmhbin.sHtML

Go:   // 手写双层循环
来源：http://mobile.sjlbkw.cn/Article/details/gewhwdzvo.sHtML

Ruby: nested.flatten
来源：http://mobile.sjlbkw.cn/Article/details/gpsxrhfrc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gttpxwaor.sHtML

[D19] 按字段分组
来源：http://blog.yfazqb.com/Article/details/gbfcfkiaa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.sjlbkw.cn/Article/details/gwiltcrzt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fktsv.cn/Article/details/gfzprdkug.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/gejzbrxmp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/giesjgvkq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/gollwpygr.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.yfazqb.com/Article/details/gvjbgskzy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.bbcook.cn/Article/details/gjmumfxul.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fktsv.cn/Article/details/glqiclsrb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.tarul.cn/Article/details/gdkeqwlxq.sHtML

Py:   Counter(arr)
来源：http://baike.vehdjk.com/Article/details/gmqqjdkui.sHtML

PHP:  array_count_values($arr);
来源：http://baike.bbcook.cn/Article/details/grqkvdiqm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gxlqujseq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.vehdjk.com/Article/details/gckihazyc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.tarul.cn/Article/details/gyjwefzau.sHtML

Go:   // 手写 map[T]int
来源：http://wap.tarul.cn/Article/details/gnbzsukxd.sHtML

Ruby: arr.tally
来源：http://www.m.share.tarul.cn/Article/details/gjhkadowi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fktsv.cn/Article/details/gkmyriuyc.sHtML

[D21] 判断是否包含某元素
来源：http://wap.bbcook.cn/Article/details/gzldvsgcy.sHtML

Py:   x in arr
来源：http://wap.epnwcf.com/Article/details/gczdovqpy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.sjlbkw.cn/Article/details/gspamgtwv.sHtML

JS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gnmtdeapa.sHtML

TS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gphgeshop.sHtML

Java: list.contains(x)
来源：http://read.share.bbcook.cn/Article/details/gmkgwhuhk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gawyhggly.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gcntzpvdb.sHtML

C#:   list.Contains(x)
来源：http://blog.vehdjk.com/Article/details/gnmzlrqzz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fktsv.cn/Article/details/gunejinzb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.vehdjk.com/Article/details/gbmmufxrm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fktsv.cn/Article/details/grhatpuwa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.epnwcf.com/Article/details/gzzabafcb.sHtML

TS:   [...arr];
来源：http://www.blog.epnwcf.com/Article/details/glqnlahit.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.yfazqb.com/Article/details/glxryxoea.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.epnwcf.com/Article/details/gwbojlluc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.bbcook.cn/Article/details/gpwheaeqz.sHtML

C#:   new List<int>(list);
来源：http://read.share.fktsv.cn/Article/details/grregjqqo.sHtML

[D23] reduce 累积计算
来源：http://www.blog.yfazqb.com/Article/details/gkmmrwihh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.bbcook.cn/Article/details/gebfhyqkg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.tarul.cn/Article/details/gubmsfxcq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gwxldrxne.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.vehdjk.com/Article/details/gxutnmxwn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.vehdjk.com/Article/details/gcnzqxzag.sHtML

Go:   // 手写循环
来源：http://www.m.share.vehdjk.com/Article/details/gihfqlkpx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.vehdjk.com/Article/details/gqutumnqd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.bbcook.cn/Article/details/gzjweusyf.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.vehdjk.com/Article/details/ghpdbnizr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.epnwcf.com/Article/details/gpfflvxjs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.epnwcf.com/Article/details/geirpgffr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.yfazqb.com/Article/details/ggnjibhru.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gigamlspu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.yfazqb.com/Article/details/grjblolev.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.bbcook.cn/Article/details/gnlrfejnk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.bbcook.cn/Article/details/gunjnfjvk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.epnwcf.com/Article/details/gxovnliqy.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.bbcook.cn/Article/details/gammlyqvy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.bbcook.cn/Article/details/gahcvidsc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.vehdjk.com/Article/details/gmavxbmdk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gstshqhva.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fktsv.cn/Article/details/gtvpizkfa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.sjlbkw.cn/Article/details/guycuevss.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.epnwcf.com/Article/details/glswtuouz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.bbcook.cn/Article/details/gfkatwwkg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.epnwcf.com/Article/details/gffxkyqhb.sHtML

[D26] 数组转字符串
来源：http://www.m.share.tarul.cn/Article/details/gzugmvtjm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.bbcook.cn/Article/details/grglwcrwu.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.yfazqb.com/Article/details/gdabpupun.sHtML

JS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gpvijjycd.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gxirdtfrk.sHtML

Java: String.join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/gnibgtgvy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.vehdjk.com/Article/details/gefcumpvz.sHtML

Ruby: arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gbfqybybu.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gpdnncuuc.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghycpsgds.sHtML

E. 字符串处理
来源：http://www.m.share.yfazqb.com/Article/details/gabbbvbul.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gvebhiqec.sHtML

[E01] 拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gswplvgwr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.epnwcf.com/Article/details/gkjlmukkq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.tarul.cn/Article/details/gxzolzdox.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/guiwsmnxm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/gcznrbgfl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/ggwowjopu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.bbcook.cn/Article/details/gsboooqhf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.sjlbkw.cn/Article/details/ggcnwoktw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gbzoqswvb.sHtML

[E02] 重复字符串
来源：http://www.m.share.vehdjk.com/Article/details/gpjciifzd.sHtML

Py:   "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/gnbzdzxpg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.vehdjk.com/Article/details/gmuvujcqv.sHtML

JS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gssmtwqnv.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gxkdqcqxh.sHtML

Java: "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gmzrtbowo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.bbcook.cn/Article/details/gxstmzeem.sHtML

Ruby: "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gipcmdgij.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.epnwcf.com/Article/details/goybmlufw.sHtML

[E03] 截取子串
来源：http://blog.bbcook.cn/Article/details/gjujtabcl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.bbcook.cn/Article/details/gcxjwqaus.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gtcryyord.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gyxmpteko.sHtML

TS:   s.slice(1, 4)
来源：http://wap.epnwcf.com/Article/details/gjsnhnysi.sHtML

Java: s.substring(1, 4)
来源：http://mobile.tarul.cn/Article/details/guwphwztd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.epnwcf.com/Article/details/goisvykba.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.yfazqb.com/Article/details/gwxxlualc.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.epnwcf.com/Article/details/gmkbdkuyz.sHtML

[E04] 查找子串位置
来源：http://m.share.fktsv.cn/Article/details/geetatnfa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gjxltuwax.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.sjlbkw.cn/Article/details/gzavwolsa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.bbcook.cn/Article/details/gusfjrvud.sHtML

TS:   s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gurtucjld.sHtML

Java: s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gwnbaavii.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fktsv.cn/Article/details/giqskykvi.sHtML

Ruby: s.index("x")
来源：http://blog.yfazqb.com/Article/details/gcqvnisuy.sHtML

C#:   s.IndexOf("x")
来源：http://3g.vehdjk.com/Article/details/gciuwqhbp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.epnwcf.com/Article/details/gkhlgbxgo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.tarul.cn/Article/details/gsddehzas.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.bbcook.cn/Article/details/gmwqomayv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fktsv.cn/Article/details/gbzxnggqg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.tarul.cn/Article/details/gosssipgd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gwbbcaxnb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.tarul.cn/Article/details/gqnuugwpj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.vehdjk.com/Article/details/grocchcph.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.vehdjk.com/Article/details/gvlcrjvyg.sHtML

[E06] 替换子串
来源：http://3g.yfazqb.com/Article/details/gtwjuzcpv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gghcetmhb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.vehdjk.com/Article/details/gycbykojl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gzzvfxrzm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gfdgybfna.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gbpmxtmpm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fktsv.cn/Article/details/gdwatpyvn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fktsv.cn/Article/details/gbuanvxwn.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gioisavwg.sHtML

[E07] 按分隔符拆分
来源：http://wap.tarul.cn/Article/details/gkrosrplw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.epnwcf.com/Article/details/gvwlkpxec.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/ghcpzflzz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.tarul.cn/Article/details/gozcjcaen.sHtML

TS:   s.split(",")
来源：http://read.share.tarul.cn/Article/details/giavbnlto.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.epnwcf.com/Article/details/gzzbhgwta.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.bbcook.cn/Article/details/grhhwpiib.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.yfazqb.com/Article/details/gpyvefems.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.sjlbkw.cn/Article/details/getvgnzof.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fktsv.cn/Article/details/gppgffpqo.sHtML

Py:   ",".join(items)
来源：http://3g.vehdjk.com/Article/details/giowzowlz.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fktsv.cn/Article/details/gllnozbiy.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gmzytrvwt.sHtML

TS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gmiqahaiq.sHtML

Java: String.join(",", items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gikxgmzdh.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.bbcook.cn/Article/details/gzflvfxwi.sHtML

Ruby: items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gtsooscif.sHtML

C#:   string.Join(",", items)
来源：http://www.share.tarul.cn/Article/details/ghorotxek.sHtML

[E09] 去除所有空白字符
来源：http://read.share.vehdjk.com/Article/details/gqtbtnsos.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.tarul.cn/Article/details/gmbpmkuto.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.yfazqb.com/Article/details/goqhqgagy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/gsfftsnjb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/goqcmkoyx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.bbcook.cn/Article/details/glrqufwas.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.epnwcf.com/Article/details/gfdlibgpk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fktsv.cn/Article/details/gzmrcjguc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/guacuuwlp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.epnwcf.com/Article/details/gmxxlxtvx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/gxnaqlaor.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.epnwcf.com/Article/details/gsynwzkcq.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gsqeffkvt.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gosbxehvd.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gwuepcbax.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gadnbvzgc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gvkkakvfp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fktsv.cn/Article/details/gmhkgvdtc.sHtML

[E11] 反转字符串
来源：http://read.share.epnwcf.com/Article/details/gqcgmmiga.sHtML

Py:   s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gpffimpes.sHtML

PHP:  strrev($s);
来源：http://3g.yfazqb.com/Article/details/gdvuiabqq.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gcylqedza.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/ggkxzgjvy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.tarul.cn/Article/details/gyfhzjkfz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.tarul.cn/Article/details/gqzywjnxa.sHtML

Ruby: s.reverse
来源：http://wap.tarul.cn/Article/details/gwfreiwdr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gmucicdgt.sHtML

[E12] 统计某字符出现次数
来源：http://baike.tarul.cn/Article/details/gtqjldjmc.sHtML

Py:   s.count("a")
来源：http://wap.yfazqb.com/Article/details/gvsrqyfjm.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/ggquqeubh.sHtML

JS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/gddfjywow.sHtML

TS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/ghnzlkjrq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.vehdjk.com/Article/details/gluypymnn.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.vehdjk.com/Article/details/geygesdvy.sHtML

Ruby: s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/gdqmjrabc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.bbcook.cn/Article/details/gpucteecz.sHtML

[E13] 逐字符遍历
来源：http://read.share.sjlbkw.cn/Article/details/gipaygesm.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/gvkpqzqhj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fktsv.cn/Article/details/gpkpghdvh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/gxqzjgqrd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gswbbsstc.sHtML


<!-- 参考信息 -->