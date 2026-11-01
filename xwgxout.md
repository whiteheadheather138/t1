代发 wailian999

Java: list.size();
来源：http://www.m.share.vehdjk.com/Article/details/gmdjstzzz.sHtML

Go:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/gfwuvvdgv.sHtML

Ruby: arr.length; arr.size
来源：http://3g.epnwcf.com/Article/details/gdjukehjt.sHtML

C#:   list.Count;
来源：http://www.share.fktsv.cn/Article/details/gsgavuyxl.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.yfazqb.com/Article/details/gyklwjvqb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.bbcook.cn/Article/details/gnitgwnyw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fktsv.cn/Article/details/gvqhfcweo.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gncadoeun.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/ggacdsjzr.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/ghakvpnsm.sHtML

Go:   arr[1:4]
来源：http://baike.vehdjk.com/Article/details/gicgnyjpv.sHtML

Ruby: arr[1, 3]
来源：http://read.share.vehdjk.com/Article/details/gppcmrhzd.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fktsv.cn/Article/details/glvbkcsps.sHtML

[D08] 合并两个数组
来源：http://www.blog.sjlbkw.cn/Article/details/gcsgtyccf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.vehdjk.com/Article/details/gancjgcsk.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.epnwcf.com/Article/details/gegqzwyef.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.vehdjk.com/Article/details/gmeqdluqz.sHtML

TS:   [...a, ...b];
来源：http://read.share.bbcook.cn/Article/details/gcuhtqzde.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.yfazqb.com/Article/details/gckjwbffh.sHtML

Go:   append(a, b...)
来源：http://3g.epnwcf.com/Article/details/gvjwhyjfd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.sjlbkw.cn/Article/details/glkcikvgc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gdbltiqzm.sHtML

[D09] 排序（升序）
来源：http://read.share.vehdjk.com/Article/details/geneonbnz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/gicjcsbjg.sHtML

PHP:  sort($arr);
来源：http://read.share.bbcook.cn/Article/details/gyvcwvbmq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.bbcook.cn/Article/details/gqhiokkll.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fktsv.cn/Article/details/gcabbjibu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.tarul.cn/Article/details/gwooavjgh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gixgvjuki.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/gtillczuf.sHtML

C#:   list.Sort();
来源：http://www.m.share.vehdjk.com/Article/details/gozsmjrqh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.yfazqb.com/Article/details/gbmyqwzep.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.tarul.cn/Article/details/gychygmxc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.bbcook.cn/Article/details/gbggnbovi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gztrfcwfd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gvgiidekr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.bbcook.cn/Article/details/gtuyekgnq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.epnwcf.com/Article/details/gvgtdbdxi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.epnwcf.com/Article/details/gtynkynyd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.bbcook.cn/Article/details/gyiozrnkz.sHtML

[D11] 反转数组
来源：http://wap.tarul.cn/Article/details/gjclwipgb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.yfazqb.com/Article/details/gtmxgtsju.sHtML

PHP:  array_reverse($arr);
来源：http://wap.vehdjk.com/Article/details/gpteoxidz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fktsv.cn/Article/details/gonukvlwn.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.bbcook.cn/Article/details/gftccxuhc.sHtML

Java: Collections.reverse(list);
来源：http://3g.epnwcf.com/Article/details/gkvjrfgbt.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.yfazqb.com/Article/details/gpiucwfex.sHtML

Ruby: arr.reverse
来源：http://mobile.bbcook.cn/Article/details/ghjizejio.sHtML

C#:   list.Reverse();
来源：http://read.share.fktsv.cn/Article/details/gwcjymcgv.sHtML

[D12] 查找元素下标
来源：http://3g.epnwcf.com/Article/details/gbhcewalw.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.yfazqb.com/Article/details/gyatbkbgm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.sjlbkw.cn/Article/details/gsovomufe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gjjmyhvji.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/gpmurwxyg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.epnwcf.com/Article/details/gbvfrvgfq.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/grbxfolif.sHtML

Ruby: arr.index(x)
来源：http://www.share.vehdjk.com/Article/details/ghcyuyhrj.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/gazfsfqdr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.epnwcf.com/Article/details/gnbjumqwp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.tarul.cn/Article/details/gscmpkbxq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.bbcook.cn/Article/details/gtufvqasj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/ggfdhqmgy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gvwmflzex.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/gjjcwvqgb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.sjlbkw.cn/Article/details/gkwxjaumo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.bbcook.cn/Article/details/gcamngwmt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gmhbcofay.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.yfazqb.com/Article/details/gstdiqutk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.vehdjk.com/Article/details/gcybtwyek.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.bbcook.cn/Article/details/grzfddhca.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gfeyyykkj.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/gmqkmulfz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gngpdjzbd.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gvhchhish.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fktsv.cn/Article/details/gnqeltvek.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fktsv.cn/Article/details/gubszsobz.sHtML

[D15] 去重
来源：http://m.share.vehdjk.com/Article/details/gexgpeojh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/ggvkxhtif.sHtML

PHP:  array_unique($arr);
来源：http://mobile.vehdjk.com/Article/details/goeyzhlem.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gvcyfrhly.sHtML

TS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/gbwvwhlbe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.bbcook.cn/Article/details/glzigstaa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.yfazqb.com/Article/details/gpclfmtif.sHtML

Ruby: arr.uniq
来源：http://3g.vehdjk.com/Article/details/gdkvhendv.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.epnwcf.com/Article/details/gwjyikfra.sHtML

[D16] 求和与平均值
来源：http://wap.bbcook.cn/Article/details/gvpsjdycn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.vehdjk.com/Article/details/gmhwgcxru.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fktsv.cn/Article/details/ghwikevio.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fktsv.cn/Article/details/guryvhaiy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/gmdxmmzph.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.vehdjk.com/Article/details/gfjhnjiyy.sHtML

Go:   // 手写循环累加
来源：http://www.share.bbcook.cn/Article/details/gemwqjqsk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fktsv.cn/Article/details/gjtbxwcva.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.bbcook.cn/Article/details/gdplcdvxw.sHtML

[D17] 最大值与最小值
来源：http://blog.epnwcf.com/Article/details/gxmpdjlcm.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.bbcook.cn/Article/details/gcvyyszcd.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.sjlbkw.cn/Article/details/gdmgigyfv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcolbucye.sHtML

TS:   Math.max(...arr);
来源：http://blog.bbcook.cn/Article/details/gfevziwsj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.bbcook.cn/Article/details/gevmgfyfn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.epnwcf.com/Article/details/gleihqlxc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.tarul.cn/Article/details/ggxgybrqu.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.tarul.cn/Article/details/gveoktdtx.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.sjlbkw.cn/Article/details/ggbyytomg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.bbcook.cn/Article/details/glfcayfln.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.bbcook.cn/Article/details/gntzyugmi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.epnwcf.com/Article/details/gsfksghoa.sHtML

TS:   nested.flat();
来源：http://www.blog.yfazqb.com/Article/details/gywiiklqh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.epnwcf.com/Article/details/gygoewuur.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gstuelbrv.sHtML

Ruby: nested.flatten
来源：http://baike.epnwcf.com/Article/details/gsgfmnabw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.tarul.cn/Article/details/gxvggigym.sHtML

[D19] 按字段分组
来源：http://read.share.yfazqb.com/Article/details/glssotukf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.bbcook.cn/Article/details/gxophnaid.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.tarul.cn/Article/details/gramzupbb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.bbcook.cn/Article/details/gtxfqcrvi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.tarul.cn/Article/details/gyzlrwmsl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.tarul.cn/Article/details/guwsyehsd.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.epnwcf.com/Article/details/gtinpwmks.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fktsv.cn/Article/details/ggjikydtf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.sjlbkw.cn/Article/details/gykzqqzvq.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.tarul.cn/Article/details/gidfxycih.sHtML

Py:   Counter(arr)
来源：http://blog.sjlbkw.cn/Article/details/gbxtuzcus.sHtML

PHP:  array_count_values($arr);
来源：http://wap.yfazqb.com/Article/details/gqxjwthpn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gqliyezjm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.vehdjk.com/Article/details/gzpotgzne.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.tarul.cn/Article/details/gkecyyexz.sHtML

Go:   // 手写 map[T]int
来源：http://baike.yfazqb.com/Article/details/ghwhddozr.sHtML

Ruby: arr.tally
来源：http://read.share.vehdjk.com/Article/details/gshqhztzi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.bbcook.cn/Article/details/gcphplzqx.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fktsv.cn/Article/details/gxgtwnuoc.sHtML

Py:   x in arr
来源：http://www.share.yfazqb.com/Article/details/gmpwegglm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/gfysroyfg.sHtML

JS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gwrauhxjv.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmutbtja.sHtML

Java: list.contains(x)
来源：http://wap.bbcook.cn/Article/details/gplynigkv.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/ghqagcnut.sHtML

Ruby: arr.include?(x)
来源：http://blog.tarul.cn/Article/details/gyqqzxfbw.sHtML

C#:   list.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/geukyzdzl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fktsv.cn/Article/details/gkkxmlzti.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/gnotxzljy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.bbcook.cn/Article/details/gposfzdeb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.bbcook.cn/Article/details/gatqdddcx.sHtML

TS:   [...arr];
来源：http://mobile.bbcook.cn/Article/details/gettesofd.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.epnwcf.com/Article/details/gwyyjglmo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.bbcook.cn/Article/details/gqlxcguwo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.sjlbkw.cn/Article/details/gljdnoknb.sHtML

C#:   new List<int>(list);
来源：http://blog.sjlbkw.cn/Article/details/gaoixlfjs.sHtML

[D23] reduce 累积计算
来源：http://wap.tarul.cn/Article/details/gilpsrblp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.yfazqb.com/Article/details/gvqppgxwa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gizojhnwy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/ggjdrcoqy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gygfevmmz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.sjlbkw.cn/Article/details/gtbmpmgju.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/gmkdkrejk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.yfazqb.com/Article/details/gsytzylkh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fktsv.cn/Article/details/gslcvtzmt.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.yfazqb.com/Article/details/gprxeotnx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.yfazqb.com/Article/details/gxyvmcacn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.bbcook.cn/Article/details/gwrgelsdl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fktsv.cn/Article/details/gxgboliim.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.epnwcf.com/Article/details/gibbaleaw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.bbcook.cn/Article/details/gybfwxtax.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.yfazqb.com/Article/details/gfuvqqdzg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.tarul.cn/Article/details/gyvhayett.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.vehdjk.com/Article/details/gjhixheck.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.vehdjk.com/Article/details/gltcmvbmy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/gawlppocd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.tarul.cn/Article/details/gfscyoiol.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.sjlbkw.cn/Article/details/gearahdth.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.epnwcf.com/Article/details/gixzspvzh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.epnwcf.com/Article/details/gribfmxdt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.tarul.cn/Article/details/gllensbnw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.vehdjk.com/Article/details/gvdqzccrp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.epnwcf.com/Article/details/giqrptfwg.sHtML

[D26] 数组转字符串
来源：http://www.blog.yfazqb.com/Article/details/gezwqyfoh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.tarul.cn/Article/details/grirrwsfh.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.epnwcf.com/Article/details/gmobjqctn.sHtML

JS:   arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gpqpsmbrr.sHtML

TS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gkshgyggz.sHtML

Java: String.join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gizdrvupb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.yfazqb.com/Article/details/gbenkownw.sHtML

Ruby: arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/getqkcbcq.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gyabkgbtr.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/grqqdjkcw.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/gaaxoewvo.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gsahsewuy.sHtML

[E01] 拼接字符串
来源：http://blog.vehdjk.com/Article/details/glpmwubsp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.epnwcf.com/Article/details/ghevjmozl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.bbcook.cn/Article/details/glcovfwgy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/gcgepxbrk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gyhjbzgje.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/glkcqvvvc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.vehdjk.com/Article/details/gprahtyvo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.tarul.cn/Article/details/gifghofos.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gzuhqljcf.sHtML

[E02] 重复字符串
来源：http://mobile.sjlbkw.cn/Article/details/gyuabgjni.sHtML

Py:   "ab" * 3
来源：http://blog.tarul.cn/Article/details/gjqmdcbey.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.tarul.cn/Article/details/gfkvzpjmo.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gltickytz.sHtML

TS:   "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/gkobcfzac.sHtML

Java: "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gogvumhus.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.sjlbkw.cn/Article/details/gceimtjau.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.epnwcf.com/Article/details/ginwnhdtc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.epnwcf.com/Article/details/gqcwfsflm.sHtML

[E03] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/gasqnoclg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.yfazqb.com/Article/details/gwgtkyjjk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gwntkcvap.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/grvthncpq.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gpbdxoprd.sHtML

Java: s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gcualqlhu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.yfazqb.com/Article/details/gxlvuwluc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.epnwcf.com/Article/details/gypmcnbta.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.sjlbkw.cn/Article/details/gftwptzzc.sHtML

[E04] 查找子串位置
来源：http://mobile.bbcook.cn/Article/details/gkvxokqhr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gsyajrdiy.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fktsv.cn/Article/details/gsbjhttri.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfvfxtrd.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gfdcgagjy.sHtML

Java: s.indexOf("x")
来源：http://m.share.vehdjk.com/Article/details/goywzcack.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.sjlbkw.cn/Article/details/gppztmmhv.sHtML

Ruby: s.index("x")
来源：http://blog.epnwcf.com/Article/details/gxpcecgbw.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gqzidqirk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.bbcook.cn/Article/details/gijhjmbzr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fktsv.cn/Article/details/gwaiwnpsw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.epnwcf.com/Article/details/galihritl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/gpzsjvssf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.epnwcf.com/Article/details/gtxpejyli.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gvlpgxoie.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.vehdjk.com/Article/details/godooahhx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.tarul.cn/Article/details/gvcnjicqi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gyhodbxle.sHtML

[E06] 替换子串
来源：http://www.m.share.vehdjk.com/Article/details/glhdwqtfy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/gdipwdfxj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fktsv.cn/Article/details/gmzlfsgvn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gyxinwnbd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gkxiqjfls.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gkjevwyis.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/gvffznvhf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.tarul.cn/Article/details/gjilbebtu.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.epnwcf.com/Article/details/gwegwlbob.sHtML

[E07] 按分隔符拆分
来源：http://mobile.vehdjk.com/Article/details/gljperqfr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.sjlbkw.cn/Article/details/gsdggiggp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gggnnxoqc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.tarul.cn/Article/details/gnjvetkeg.sHtML

TS:   s.split(",")
来源：http://mobile.sjlbkw.cn/Article/details/gthknrkdo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.epnwcf.com/Article/details/guvrrwuke.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.sjlbkw.cn/Article/details/gzpubegue.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.vehdjk.com/Article/details/gbnbehpay.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fktsv.cn/Article/details/giuwbeltk.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.epnwcf.com/Article/details/gvotuzvca.sHtML

Py:   ",".join(items)
来源：http://blog.sjlbkw.cn/Article/details/grxpfwwtp.sHtML

PHP:  implode(",", $items);
来源：http://wap.bbcook.cn/Article/details/gmcawqfrz.sHtML

JS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/grjeeqlvh.sHtML

TS:   items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gpkvraeoy.sHtML

Java: String.join(",", items)
来源：http://www.blog.yfazqb.com/Article/details/guroopqop.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fktsv.cn/Article/details/ghcdhgmgj.sHtML

Ruby: items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gejijyhtf.sHtML

C#:   string.Join(",", items)
来源：http://3g.epnwcf.com/Article/details/gefdlbnbb.sHtML

[E09] 去除所有空白字符
来源：http://wap.fktsv.cn/Article/details/gmlgqloqn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.yfazqb.com/Article/details/gvffuuvcn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.bbcook.cn/Article/details/gfbfmndvv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.vehdjk.com/Article/details/gndzromoc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/goomhjyci.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fktsv.cn/Article/details/gyxidldyx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.yfazqb.com/Article/details/gxvscdval.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.tarul.cn/Article/details/gsiapogir.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fktsv.cn/Article/details/gkycezksj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.tarul.cn/Article/details/gyrjakepn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gnpupykzi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.epnwcf.com/Article/details/gewncvjva.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/ggiinmssy.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gakwjqvsf.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/geoajmpux.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gykodzzyi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gvmhnudqo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.vehdjk.com/Article/details/gzhaaucch.sHtML

[E11] 反转字符串
来源：http://www.share.bbcook.cn/Article/details/gvfcoyxmt.sHtML

Py:   s[::-1]
来源：http://baike.epnwcf.com/Article/details/gbdljnvfs.sHtML

PHP:  strrev($s);
来源：http://baike.epnwcf.com/Article/details/gyxrkuvdw.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gtorjritv.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/grbgtboqd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.bbcook.cn/Article/details/gboljxxrr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fktsv.cn/Article/details/gkewzcxmc.sHtML

Ruby: s.reverse
来源：http://3g.sjlbkw.cn/Article/details/ghausnzvw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/gvgtdgugy.sHtML

[E12] 统计某字符出现次数
来源：http://3g.yfazqb.com/Article/details/guepqytiq.sHtML

Py:   s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gphoslhav.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.epnwcf.com/Article/details/giqwtvlai.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gaqeksnav.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gyhymnufd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.sjlbkw.cn/Article/details/gjidfhqqa.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.epnwcf.com/Article/details/gcfwjxasf.sHtML

Ruby: s.count("a")
来源：http://read.share.tarul.cn/Article/details/gxuumnoqf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.epnwcf.com/Article/details/gcibjhzvh.sHtML

[E13] 逐字符遍历
来源：http://www.blog.vehdjk.com/Article/details/gvtdbxnjx.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.sjlbkw.cn/Article/details/gzxlciyoz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.tarul.cn/Article/details/goqfownbq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gfrrzpfos.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gwlwiluks.sHtML


<!-- 参考信息 -->