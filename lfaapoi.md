代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.yfazqb.com/Article/details/gtfszawhx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.sjlbkw.cn/Article/details/gdjyhheef.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gjvkbmets.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/gbshwikhq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.bbcook.cn/Article/details/ggmxmrqcm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.bbcook.cn/Article/details/gykzhrcat.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.bbcook.cn/Article/details/gwyphbcdc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.epnwcf.com/Article/details/ghkmphnzi.sHtML

[D11] 反转数组
来源：http://wap.fktsv.cn/Article/details/gqnvbhmuj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.vehdjk.com/Article/details/gnewmpcxh.sHtML

PHP:  array_reverse($arr);
来源：http://wap.sjlbkw.cn/Article/details/gxkmoognd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.sjlbkw.cn/Article/details/gnuurtpsp.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fktsv.cn/Article/details/gguoxgeik.sHtML

Java: Collections.reverse(list);
来源：http://baike.fktsv.cn/Article/details/giwvihxsi.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.epnwcf.com/Article/details/gtfbwncuo.sHtML

Ruby: arr.reverse
来源：http://mobile.yfazqb.com/Article/details/gfdzmctlb.sHtML

C#:   list.Reverse();
来源：http://blog.sjlbkw.cn/Article/details/gkaioxcpr.sHtML

[D12] 查找元素下标
来源：http://www.m.share.bbcook.cn/Article/details/gozpsdfoc.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.tarul.cn/Article/details/gmamtxxhc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.yfazqb.com/Article/details/glazhpzme.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.yfazqb.com/Article/details/gfnaclycu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gvsnxlvjc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fktsv.cn/Article/details/gmateihfs.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.tarul.cn/Article/details/gkemxuuia.sHtML

Ruby: arr.index(x)
来源：http://m.share.bbcook.cn/Article/details/gsujepgyz.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fktsv.cn/Article/details/gqzfjljqm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.epnwcf.com/Article/details/gzckmqmng.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.yfazqb.com/Article/details/gfdmarfss.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.epnwcf.com/Article/details/gtftqimpq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gwlwxdpfr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/gqwkcraro.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fktsv.cn/Article/details/gqiximodz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.bbcook.cn/Article/details/gvtnvqset.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.yfazqb.com/Article/details/goqfljrkf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gttvuaxoy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fktsv.cn/Article/details/gfidbhzhp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.vehdjk.com/Article/details/gnlayddkl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fktsv.cn/Article/details/gmkzlguvp.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/gypnfeomx.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/gvjclrnkl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.vehdjk.com/Article/details/gggqzdkzh.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/gzsuyjsuc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.yfazqb.com/Article/details/gdxxrliod.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.tarul.cn/Article/details/gbhdwauur.sHtML

[D15] 去重
来源：http://baike.epnwcf.com/Article/details/grattyxjx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/geojsvwgb.sHtML

PHP:  array_unique($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gunouogxz.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/genvrzojy.sHtML

TS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gbiqkfkbf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.bbcook.cn/Article/details/gpfkwjrer.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.tarul.cn/Article/details/gihgftjcs.sHtML

Ruby: arr.uniq
来源：http://www.blog.tarul.cn/Article/details/gidgsapqa.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fktsv.cn/Article/details/gjrulypmc.sHtML

[D16] 求和与平均值
来源：http://baike.sjlbkw.cn/Article/details/gtgtunlhe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fktsv.cn/Article/details/gnkmwxnhx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fktsv.cn/Article/details/gzaqpponb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/glwpflflj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gfohxziqw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.tarul.cn/Article/details/gldovtzyt.sHtML

Go:   // 手写循环累加
来源：http://www.blog.yfazqb.com/Article/details/gxfduobde.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/gnqggiqys.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.epnwcf.com/Article/details/gfghyekea.sHtML

[D17] 最大值与最小值
来源：http://www.blog.tarul.cn/Article/details/gondwwqot.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.tarul.cn/Article/details/gupjsbguz.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.tarul.cn/Article/details/ghzrvdkvg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fktsv.cn/Article/details/gxvnmsypj.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gavwwxnlo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.yfazqb.com/Article/details/gogwqbdqp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fktsv.cn/Article/details/gubcqfrss.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.epnwcf.com/Article/details/gtsinsdye.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fktsv.cn/Article/details/ggktmoytx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.vehdjk.com/Article/details/gvdiueggj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.yfazqb.com/Article/details/gxrjswvvy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fktsv.cn/Article/details/gonrlgzqx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.sjlbkw.cn/Article/details/gmgyngopc.sHtML

TS:   nested.flat();
来源：http://www.blog.bbcook.cn/Article/details/gaaeouddj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.tarul.cn/Article/details/gpiupoeze.sHtML

Go:   // 手写双层循环
来源：http://3g.vehdjk.com/Article/details/gvidpujuc.sHtML

Ruby: nested.flatten
来源：http://blog.yfazqb.com/Article/details/geebjemda.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.tarul.cn/Article/details/gjhhmbmik.sHtML

[D19] 按字段分组
来源：http://wap.yfazqb.com/Article/details/gktfesaiw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.yfazqb.com/Article/details/gjrwxxgyn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.bbcook.cn/Article/details/gdpsgheyt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.vehdjk.com/Article/details/gpgovclba.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.vehdjk.com/Article/details/gbddlenkk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fktsv.cn/Article/details/gqdjdidfv.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.tarul.cn/Article/details/gtgazimfd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.sjlbkw.cn/Article/details/gzkledvyk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.epnwcf.com/Article/details/glrorysvl.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.vehdjk.com/Article/details/gpsopolrv.sHtML

Py:   Counter(arr)
来源：http://blog.yfazqb.com/Article/details/gccmlnbxt.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fktsv.cn/Article/details/gxtqybbyy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.yfazqb.com/Article/details/gmmmdjrzz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.tarul.cn/Article/details/gyuhmeqec.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.sjlbkw.cn/Article/details/gaapltkgs.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.epnwcf.com/Article/details/ghxnkrqxf.sHtML

Ruby: arr.tally
来源：http://m.share.bbcook.cn/Article/details/gpqdtgyub.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.bbcook.cn/Article/details/gjephngxm.sHtML

[D21] 判断是否包含某元素
来源：http://blog.yfazqb.com/Article/details/gqvuqdtij.sHtML

Py:   x in arr
来源：http://wap.vehdjk.com/Article/details/gcrolryvl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fktsv.cn/Article/details/gygjqadty.sHtML

JS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gzubuvrzh.sHtML

TS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/gupkapcof.sHtML

Java: list.contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gwlnpynkr.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gqvncituj.sHtML

Ruby: arr.include?(x)
来源：http://read.share.vehdjk.com/Article/details/gxffjgdkv.sHtML

C#:   list.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gjznrhwfn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.tarul.cn/Article/details/gybqehbrf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.tarul.cn/Article/details/gqyznmovj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.sjlbkw.cn/Article/details/gufroclfd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.bbcook.cn/Article/details/gazupujap.sHtML

TS:   [...arr];
来源：http://mobile.tarul.cn/Article/details/grrddxlyj.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gcsjgiboq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fktsv.cn/Article/details/gsaqydyhm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.tarul.cn/Article/details/gxsgabgtx.sHtML

C#:   new List<int>(list);
来源：http://mobile.yfazqb.com/Article/details/guicndnat.sHtML

[D23] reduce 累积计算
来源：http://www.share.sjlbkw.cn/Article/details/gdpegejal.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gyddplcta.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.tarul.cn/Article/details/gfjmdkwcb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gxugkwykd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gegfwcghn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.vehdjk.com/Article/details/gsabrhszy.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/gkuvtaltd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.epnwcf.com/Article/details/gzbnriujv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fktsv.cn/Article/details/gpsfmrrin.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.epnwcf.com/Article/details/gigrnegob.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.vehdjk.com/Article/details/gnulnwtxm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gtmkiqqom.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.bbcook.cn/Article/details/gcmbvfgwl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gkqvadohb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.tarul.cn/Article/details/gmhjehnlr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.vehdjk.com/Article/details/glqcjokjb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.yfazqb.com/Article/details/gyoudpbtj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.yfazqb.com/Article/details/grjzjlwnq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.yfazqb.com/Article/details/gjqliazxw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.tarul.cn/Article/details/gbvbdiuup.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.sjlbkw.cn/Article/details/grkpldzqz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.vehdjk.com/Article/details/gvrpfymcw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.vehdjk.com/Article/details/guufvymqs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gmrgywrrl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.bbcook.cn/Article/details/glsmhrrme.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.tarul.cn/Article/details/gptouitlj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.bbcook.cn/Article/details/gwtuvzcpg.sHtML

[D26] 数组转字符串
来源：http://www.share.yfazqb.com/Article/details/gpdmjlrne.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.bbcook.cn/Article/details/gxvpzkgsw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fktsv.cn/Article/details/gqjpsnrwr.sHtML

JS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gtugqnpsw.sHtML

TS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gypibwuaf.sHtML

Java: String.join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/gjeuhayky.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fktsv.cn/Article/details/gellqgdiq.sHtML

Ruby: arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/gidfdgmah.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gyltghovm.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gdchqzdac.sHtML

E. 字符串处理
来源：http://blog.fktsv.cn/Article/details/gdkarizdp.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gkhndosfq.sHtML

[E01] 拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gbisvfuwk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.bbcook.cn/Article/details/guwrerlfn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.sjlbkw.cn/Article/details/gbrkpjxrh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gwztapyjl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.bbcook.cn/Article/details/gqvmqjucy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.vehdjk.com/Article/details/grhjifvdx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.vehdjk.com/Article/details/ghsvehuzy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.epnwcf.com/Article/details/genmieboj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gzqvodilh.sHtML

[E02] 重复字符串
来源：http://baike.fktsv.cn/Article/details/gqqoistip.sHtML

Py:   "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gecfpeckp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.tarul.cn/Article/details/gvwztswbe.sHtML

JS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gfgicafoh.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gmbhdrgej.sHtML

Java: "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gehagtmqg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgctwfgk.sHtML

Ruby: "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/guzlzizef.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.vehdjk.com/Article/details/gkopnavra.sHtML

[E03] 截取子串
来源：http://www.share.sjlbkw.cn/Article/details/guyovzmom.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fktsv.cn/Article/details/gbbpidlzt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gaefusbyb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/guwjprhht.sHtML

TS:   s.slice(1, 4)
来源：http://wap.bbcook.cn/Article/details/gofhdmmnd.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gatpnlwqp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.epnwcf.com/Article/details/gshmxbtin.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.tarul.cn/Article/details/ghagcbnlb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.tarul.cn/Article/details/gthndxqib.sHtML

[E04] 查找子串位置
来源：http://read.share.sjlbkw.cn/Article/details/grusgxjux.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gksvonnub.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fktsv.cn/Article/details/gtprrjaiu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrqcbcjb.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gevhlmrsj.sHtML

Java: s.indexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gfgpfmyvl.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.sjlbkw.cn/Article/details/gldxemsag.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/guzehjqbw.sHtML

C#:   s.IndexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gojuwzkib.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.bbcook.cn/Article/details/galpzebdw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.vehdjk.com/Article/details/gzuyoxnie.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fktsv.cn/Article/details/gsncnyalf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gjvfulelj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.bbcook.cn/Article/details/glgyktvhs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fktsv.cn/Article/details/glxstbdql.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.vehdjk.com/Article/details/gurguqxjk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fktsv.cn/Article/details/gzejtfhjy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/gifvcmkhm.sHtML

[E06] 替换子串
来源：http://read.share.sjlbkw.cn/Article/details/gtlttijek.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gxpalmicv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.epnwcf.com/Article/details/gryeyrogm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gvkgbxlfp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gyvdwsuzr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gyhzrxbap.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gdngcddhm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gswlkdytu.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gpiqzlhzw.sHtML

[E07] 按分隔符拆分
来源：http://blog.vehdjk.com/Article/details/gibzqaguo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fktsv.cn/Article/details/gvzhsldjw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fktsv.cn/Article/details/ghyhhbhqp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/gxmqgsmot.sHtML

TS:   s.split(",")
来源：http://wap.bbcook.cn/Article/details/gypwaigln.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fktsv.cn/Article/details/glnlfahmv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.epnwcf.com/Article/details/gzcfrozgs.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.vehdjk.com/Article/details/glirvkyzv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.vehdjk.com/Article/details/gizjzbxna.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.epnwcf.com/Article/details/gvyshsswm.sHtML

Py:   ",".join(items)
来源：http://3g.epnwcf.com/Article/details/gxliksdet.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fktsv.cn/Article/details/gobilenjx.sHtML

JS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gfcrndlkp.sHtML

TS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gniyjmjjp.sHtML

Java: String.join(",", items)
来源：http://blog.epnwcf.com/Article/details/gygzkoxna.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.sjlbkw.cn/Article/details/gsbxwbxnf.sHtML

Ruby: items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gkdiekcem.sHtML

C#:   string.Join(",", items)
来源：http://baike.vehdjk.com/Article/details/gzexbrpeb.sHtML

[E09] 去除所有空白字符
来源：http://www.share.epnwcf.com/Article/details/gbrzbxzxc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fktsv.cn/Article/details/gvvuzwbzs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/gwafgxhjl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.tarul.cn/Article/details/gbrtrqskw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gineumhjb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gurypwasr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.bbcook.cn/Article/details/garbjhjdw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.vehdjk.com/Article/details/gypcwkxnu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.epnwcf.com/Article/details/ggzcrckda.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcvgykuc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/gdaubfsig.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fktsv.cn/Article/details/gslusqqre.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gzyqnklhx.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/guybvachn.sHtML

Java: String.format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gnpqcfdgz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gwdeljodg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gruztpsol.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/gufxytfuh.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/gbblmmwpl.sHtML

Py:   s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gzkybrusf.sHtML

PHP:  strrev($s);
来源：http://mobile.fktsv.cn/Article/details/ganeshudx.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gyaijgnoc.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/ggnkdllkx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fktsv.cn/Article/details/gaphnbdvy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.sjlbkw.cn/Article/details/gpvaqbuim.sHtML

Ruby: s.reverse
来源：http://read.share.vehdjk.com/Article/details/ggcmgoncx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.epnwcf.com/Article/details/gxmclzvna.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.yfazqb.com/Article/details/gvyudvtjz.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/gimmucwsx.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.epnwcf.com/Article/details/gmairxcpy.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/gtoelgfze.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.bbcook.cn/Article/details/gugizdzun.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.sjlbkw.cn/Article/details/gdgcwbtiu.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.epnwcf.com/Article/details/gomqkzbqm.sHtML

Ruby: s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gflhjjigo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fktsv.cn/Article/details/gucexkfgd.sHtML

[E13] 逐字符遍历
来源：http://read.share.tarul.cn/Article/details/gvgudlcnt.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/gqwgpueno.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.tarul.cn/Article/details/gadyaafpq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gkgswkfnw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/glezcfnoy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.tarul.cn/Article/details/ggsgeeyfc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fktsv.cn/Article/details/gzwjahcqv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.bbcook.cn/Article/details/ggiymxfou.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/grqzacpwn.sHtML

[E14] URL 编码与 Base64
来源：http://baike.sjlbkw.cn/Article/details/gyypmxmux.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.epnwcf.com/Article/details/grpkkhbdd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.tarul.cn/Article/details/gevowhlak.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.sjlbkw.cn/Article/details/gszzndxpd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.tarul.cn/Article/details/gjftrakdx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gnseavdhw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.bbcook.cn/Article/details/gtwemzpqo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.epnwcf.com/Article/details/gyacltipg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fktsv.cn/Article/details/gbmrakbpy.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.sjlbkw.cn/Article/details/gsayvvimz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.sjlbkw.cn/Article/details/gdbtbvgdb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gzjgtfcmg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.epnwcf.com/Article/details/guukyufko.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.sjlbkw.cn/Article/details/gqdidqbgj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.yfazqb.com/Article/details/ggkygxntz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gwavvxhid.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.yfazqb.com/Article/details/gdzorgmmo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.tarul.cn/Article/details/gdhcvycbc.sHtML

[E16] 数字千分位
来源：http://3g.yfazqb.com/Article/details/gcozvzjvj.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fktsv.cn/Article/details/gwmkmnuvj.sHtML

PHP:  number_format(1234567);
来源：http://3g.sjlbkw.cn/Article/details/gjfbkzfwi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/ghoomxvka.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gzdtjavjw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fktsv.cn/Article/details/gcqfqpagd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.epnwcf.com/Article/details/geualemuo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.epnwcf.com/Article/details/gvacglpme.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fktsv.cn/Article/details/gwbwlxrsq.sHtML

[E17] 首字母大写
来源：http://m.share.vehdjk.com/Article/details/gmmyvftvs.sHtML


<!-- 参考信息 -->