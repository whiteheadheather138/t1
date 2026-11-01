代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.sjlbkw.cn/Article/details/gqwlxqfxd.sHtML

TS:   [...a, ...b];
来源：http://www.share.tarul.cn/Article/details/galcwlozn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.yfazqb.com/Article/details/ghpgqhgry.sHtML

Go:   append(a, b...)
来源：http://www.share.bbcook.cn/Article/details/gjjnjuhjd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.vehdjk.com/Article/details/gtwmuhrum.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.tarul.cn/Article/details/gxdhyccad.sHtML

[D09] 排序（升序）
来源：http://www.m.share.bbcook.cn/Article/details/ggfigpsva.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gfhdvxmec.sHtML

PHP:  sort($arr);
来源：http://3g.vehdjk.com/Article/details/guddaoity.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.sjlbkw.cn/Article/details/gwgafzawb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.epnwcf.com/Article/details/gwsbymcuo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.epnwcf.com/Article/details/gakfltaui.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gbwzovvzt.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/geysuyyfe.sHtML

C#:   list.Sort();
来源：http://www.share.bbcook.cn/Article/details/gxxkybtej.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.sjlbkw.cn/Article/details/gbhiocseb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fktsv.cn/Article/details/grxhekixq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.yfazqb.com/Article/details/gctlifesg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.tarul.cn/Article/details/gnufmspgt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gnbwyjgzt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.epnwcf.com/Article/details/gqbmpkxqg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.tarul.cn/Article/details/gjgxtufcs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.sjlbkw.cn/Article/details/gjafqvyqi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fktsv.cn/Article/details/guadilmyx.sHtML

[D11] 反转数组
来源：http://mobile.epnwcf.com/Article/details/gedpzkeyr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.epnwcf.com/Article/details/glhvflknr.sHtML

PHP:  array_reverse($arr);
来源：http://baike.bbcook.cn/Article/details/gbtjvighr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.bbcook.cn/Article/details/gkvenhjei.sHtML

TS:   [...arr].reverse();
来源：http://m.share.yfazqb.com/Article/details/gikfgmckk.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.yfazqb.com/Article/details/garxrhssc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.epnwcf.com/Article/details/gtdggozxj.sHtML

Ruby: arr.reverse
来源：http://3g.tarul.cn/Article/details/glrqninuf.sHtML

C#:   list.Reverse();
来源：http://wap.tarul.cn/Article/details/gyczvwsha.sHtML

[D12] 查找元素下标
来源：http://3g.yfazqb.com/Article/details/gaqvovdxz.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.vehdjk.com/Article/details/gtxofrqvk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.vehdjk.com/Article/details/ghshiuwje.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/gwunaumuw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.vehdjk.com/Article/details/ggtadccyw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.tarul.cn/Article/details/gotbscxes.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.bbcook.cn/Article/details/gnlvhxdsu.sHtML

Ruby: arr.index(x)
来源：http://mobile.tarul.cn/Article/details/gxjcgpbgu.sHtML

C#:   list.IndexOf(x);
来源：http://baike.vehdjk.com/Article/details/gtppmeayk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.bbcook.cn/Article/details/gvowfevmp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.bbcook.cn/Article/details/gnknqgwvy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.epnwcf.com/Article/details/gxlmiuffi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gqjytnets.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/geafgirsf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.vehdjk.com/Article/details/gndkjzslt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.vehdjk.com/Article/details/gclvprnql.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.bbcook.cn/Article/details/geshngncq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/ghvniqgyv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.tarul.cn/Article/details/grfmpnkfu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.vehdjk.com/Article/details/gpfppmwgn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.bbcook.cn/Article/details/gjkvlxcii.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fktsv.cn/Article/details/gouwrdhif.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.tarul.cn/Article/details/galamhqep.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.bbcook.cn/Article/details/gukqpmqhi.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gzjdtxafm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.epnwcf.com/Article/details/gbmnmfalh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.bbcook.cn/Article/details/gpvdawnyj.sHtML

[D15] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gzogcbbqy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fktsv.cn/Article/details/gzzmqcgvr.sHtML

PHP:  array_unique($arr);
来源：http://wap.bbcook.cn/Article/details/gzyqwjoyb.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gsrsswpmz.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/gfhmckhlp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.tarul.cn/Article/details/gzkpswuuh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.tarul.cn/Article/details/geymyrrko.sHtML

Ruby: arr.uniq
来源：http://www.blog.fktsv.cn/Article/details/gdktqubfj.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.sjlbkw.cn/Article/details/gandhznkz.sHtML

[D16] 求和与平均值
来源：http://wap.bbcook.cn/Article/details/geuqnaaxz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fktsv.cn/Article/details/gqqygecoq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fktsv.cn/Article/details/gqfigdxlu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/glkvnhneb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/govqkfywm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.sjlbkw.cn/Article/details/guwxnacbu.sHtML

Go:   // 手写循环累加
来源：http://m.share.fktsv.cn/Article/details/gtcusrhbv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.bbcook.cn/Article/details/gssneohiz.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.vehdjk.com/Article/details/gxubctiqx.sHtML

[D17] 最大值与最小值
来源：http://m.share.epnwcf.com/Article/details/gymrtimew.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.sjlbkw.cn/Article/details/guisticch.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.bbcook.cn/Article/details/gibnafjro.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.sjlbkw.cn/Article/details/gmlyvkwmd.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.epnwcf.com/Article/details/gldsiioke.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fktsv.cn/Article/details/gkghpnazv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/goaodyfth.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.tarul.cn/Article/details/ggdvhylid.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.sjlbkw.cn/Article/details/gtvvqoigm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.yfazqb.com/Article/details/gmfgegaoo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fktsv.cn/Article/details/gpkzuewmc.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.yfazqb.com/Article/details/ghwedrind.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.bbcook.cn/Article/details/gujejzgnj.sHtML

TS:   nested.flat();
来源：http://mobile.fktsv.cn/Article/details/grzlijeet.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.bbcook.cn/Article/details/gdwsxleec.sHtML

Go:   // 手写双层循环
来源：http://blog.epnwcf.com/Article/details/gzcfxpnal.sHtML

Ruby: nested.flatten
来源：http://mobile.vehdjk.com/Article/details/girezqswe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gdupkjwhs.sHtML

[D19] 按字段分组
来源：http://blog.fktsv.cn/Article/details/glucsbrzy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.yfazqb.com/Article/details/gbvjaofhc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.yfazqb.com/Article/details/giusldutx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fktsv.cn/Article/details/gsqtkqunc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/gadjfbobs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.bbcook.cn/Article/details/gzdndpaby.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.vehdjk.com/Article/details/gkkpjixzr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.epnwcf.com/Article/details/gykukqxtr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.yfazqb.com/Article/details/gpgqgvcci.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.sjlbkw.cn/Article/details/gwwgsdtvb.sHtML

Py:   Counter(arr)
来源：http://mobile.epnwcf.com/Article/details/ghopysdto.sHtML

PHP:  array_count_values($arr);
来源：http://blog.bbcook.cn/Article/details/gweljhenk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/gcfdvmtnr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/glhberqxb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.yfazqb.com/Article/details/giwypsvba.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.vehdjk.com/Article/details/ggtmmpzcn.sHtML

Ruby: arr.tally
来源：http://baike.vehdjk.com/Article/details/gfeimpgjw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/gzvbbtvem.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.vehdjk.com/Article/details/gvlfuubzz.sHtML

Py:   x in arr
来源：http://mobile.bbcook.cn/Article/details/gbolhlgtc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.vehdjk.com/Article/details/guwztehyj.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gcghkuvkn.sHtML

TS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gsnnjkshf.sHtML

Java: list.contains(x)
来源：http://blog.tarul.cn/Article/details/gqkgzpgdp.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fktsv.cn/Article/details/geituinat.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gitjnwiyc.sHtML

C#:   list.Contains(x)
来源：http://baike.fktsv.cn/Article/details/gtydxozzv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.bbcook.cn/Article/details/gmpleizwx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.bbcook.cn/Article/details/gzucdplbo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fktsv.cn/Article/details/gevepmrby.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gxhtlsfni.sHtML

TS:   [...arr];
来源：http://read.share.epnwcf.com/Article/details/giccoeqmv.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.vehdjk.com/Article/details/gxlozxgqv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fktsv.cn/Article/details/gwownrqad.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.yfazqb.com/Article/details/gkgxeduol.sHtML

C#:   new List<int>(list);
来源：http://mobile.sjlbkw.cn/Article/details/guviaiyah.sHtML

[D23] reduce 累积计算
来源：http://mobile.epnwcf.com/Article/details/ggjnsudye.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.epnwcf.com/Article/details/guqadysbv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.yfazqb.com/Article/details/gcjgzqsja.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/gxzbzuoyf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gsuzcwkco.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.epnwcf.com/Article/details/glhhgoasq.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/gtnwqdssp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.epnwcf.com/Article/details/gneiliaha.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fktsv.cn/Article/details/gxjnuxask.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.bbcook.cn/Article/details/grxmfbnef.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.bbcook.cn/Article/details/gvuiabdlp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.bbcook.cn/Article/details/gdgbwctyj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.vehdjk.com/Article/details/ghtphuxaw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gxypgydgo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.epnwcf.com/Article/details/gvalhlskb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fktsv.cn/Article/details/gypvrobql.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.yfazqb.com/Article/details/gavgmtljd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.vehdjk.com/Article/details/gnxmrqvhu.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.tarul.cn/Article/details/gzcxvxqrl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fktsv.cn/Article/details/gpkveyksr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.tarul.cn/Article/details/grxajpgrb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.epnwcf.com/Article/details/gjttdmxbb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.sjlbkw.cn/Article/details/gijmktrsf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fktsv.cn/Article/details/gxeynpsli.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.bbcook.cn/Article/details/gmkjixnmd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fktsv.cn/Article/details/gaijmraxo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.tarul.cn/Article/details/grxsfdevx.sHtML

[D26] 数组转字符串
来源：http://mobile.vehdjk.com/Article/details/gjwgsnucc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.bbcook.cn/Article/details/gscnhibog.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.yfazqb.com/Article/details/gxxyreiey.sHtML

JS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/ggmtpdiol.sHtML

TS:   arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/ggxhtygbm.sHtML

Java: String.join(", ", list)
来源：http://wap.vehdjk.com/Article/details/gsccvsvxu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.tarul.cn/Article/details/glepzendh.sHtML

Ruby: arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gvnhqeyjn.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/gfrlztjke.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtcnyhmfa.sHtML

E. 字符串处理
来源：http://read.share.vehdjk.com/Article/details/gkhiyyivt.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gphiomctp.sHtML

[E01] 拼接字符串
来源：http://baike.yfazqb.com/Article/details/gdmsrzxfb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.yfazqb.com/Article/details/gfvqdutxd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.vehdjk.com/Article/details/gdhhittri.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.sjlbkw.cn/Article/details/ghdvkruyx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.yfazqb.com/Article/details/gefynaezt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.yfazqb.com/Article/details/gudfycpeo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fktsv.cn/Article/details/gguyhjhua.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.tarul.cn/Article/details/gwmclhkof.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gxojtopsp.sHtML

[E02] 重复字符串
来源：http://mobile.vehdjk.com/Article/details/gzatqczxm.sHtML

Py:   "ab" * 3
来源：http://3g.bbcook.cn/Article/details/gqzmlwgec.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.vehdjk.com/Article/details/gyqjgtecu.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gbjolutwa.sHtML

TS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gcenwvfmo.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gokfiyrov.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.epnwcf.com/Article/details/gpnreuosv.sHtML

Ruby: "ab" * 3
来源：http://baike.yfazqb.com/Article/details/ghkcucifs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.vehdjk.com/Article/details/gjbffiiit.sHtML

[E03] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/gpgeqpfri.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.vehdjk.com/Article/details/gglyhujhr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/grvgxqwwk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gkopkuker.sHtML

TS:   s.slice(1, 4)
来源：http://baike.epnwcf.com/Article/details/gmwxmedmb.sHtML

Java: s.substring(1, 4)
来源：http://blog.bbcook.cn/Article/details/gyicaoaqc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.vehdjk.com/Article/details/gnyvzsroy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.bbcook.cn/Article/details/giolzmqma.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.epnwcf.com/Article/details/grfubtckl.sHtML

[E04] 查找子串位置
来源：http://3g.tarul.cn/Article/details/gkncfcjht.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.bbcook.cn/Article/details/gpwxibszz.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fktsv.cn/Article/details/gppassdmf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fktsv.cn/Article/details/glbofvfwn.sHtML

TS:   s.indexOf("x")
来源：http://blog.vehdjk.com/Article/details/gwgucedls.sHtML

Java: s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gtjjmrqki.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.epnwcf.com/Article/details/gzlvznsye.sHtML

Ruby: s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/gumyhiqmw.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.tarul.cn/Article/details/gqqzsspfe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.epnwcf.com/Article/details/guzbabaxf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gemwmvrpz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.bbcook.cn/Article/details/gtuhalcwt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gihtymbel.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.yfazqb.com/Article/details/gzoscphrl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gfmemjqgi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.epnwcf.com/Article/details/gzttvsgcu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.sjlbkw.cn/Article/details/gxnwmtzsd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.tarul.cn/Article/details/gjcsgnklm.sHtML

[E06] 替换子串
来源：http://www.share.bbcook.cn/Article/details/ghbhrwayc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/grtjmytsq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.bbcook.cn/Article/details/goazyapad.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gpocgcawv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gtczoomyy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gjvyibwon.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gufxxmdep.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gxqkolxob.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gsuioppsa.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/gqjbnqmsm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.sjlbkw.cn/Article/details/gdhlabweh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gqjfyysxx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.tarul.cn/Article/details/gtqtjrizs.sHtML

TS:   s.split(",")
来源：http://wap.bbcook.cn/Article/details/ggcctgqtq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.bbcook.cn/Article/details/gwrqwsvhi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fktsv.cn/Article/details/gamdmbjhr.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.yfazqb.com/Article/details/gyqrwugyp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fktsv.cn/Article/details/gjhwooidx.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fktsv.cn/Article/details/gnawcvemk.sHtML

Py:   ",".join(items)
来源：http://wap.sjlbkw.cn/Article/details/gqpclvhtd.sHtML

PHP:  implode(",", $items);
来源：http://baike.vehdjk.com/Article/details/gsibdvmiu.sHtML

JS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/gzuunlnnk.sHtML

TS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gqvssuano.sHtML

Java: String.join(",", items)
来源：http://wap.vehdjk.com/Article/details/gencovwsb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fktsv.cn/Article/details/gfwapzqcx.sHtML

Ruby: items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gsvsqwbkf.sHtML

C#:   string.Join(",", items)
来源：http://blog.yfazqb.com/Article/details/gheotmctn.sHtML

[E09] 去除所有空白字符
来源：http://baike.tarul.cn/Article/details/gpklttoyc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fktsv.cn/Article/details/gpaluaufd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.epnwcf.com/Article/details/gqaglroyf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/gngckaqnz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/grhemutey.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fktsv.cn/Article/details/gyucspgmw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.epnwcf.com/Article/details/gqsfftdbd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.epnwcf.com/Article/details/glrpjemhc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/grrfezlcg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.vehdjk.com/Article/details/gqossvydx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.vehdjk.com/Article/details/galgljyof.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.vehdjk.com/Article/details/gfetkifvd.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/gppdysmfr.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gzgjicpkl.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gsqthzntn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gxehxhisg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gdiwowoal.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.yfazqb.com/Article/details/gfzxdwkiw.sHtML

[E11] 反转字符串
来源：http://wap.fktsv.cn/Article/details/gytceesbx.sHtML

Py:   s[::-1]
来源：http://www.share.epnwcf.com/Article/details/ggiwikyyc.sHtML

PHP:  strrev($s);
来源：http://m.share.vehdjk.com/Article/details/grflpbthv.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gnfwqmvxx.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/ghdunwxjp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fktsv.cn/Article/details/gncvcpgoh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.vehdjk.com/Article/details/gzmoiauiw.sHtML

Ruby: s.reverse
来源：http://m.share.vehdjk.com/Article/details/gkzanmjao.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gshsyxijz.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.tarul.cn/Article/details/gtgmepbgs.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/gfkbqhwma.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.yfazqb.com/Article/details/gyhqilnns.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gjeqcmatn.sHtML

TS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gkonkuudf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.yfazqb.com/Article/details/gaqhxqjgu.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fktsv.cn/Article/details/gsdnfyzpj.sHtML

Ruby: s.count("a")
来源：http://blog.bbcook.cn/Article/details/gugnlzmqm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.vehdjk.com/Article/details/gvsugqadk.sHtML

[E13] 逐字符遍历
来源：http://3g.tarul.cn/Article/details/gonzlxefa.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fktsv.cn/Article/details/gfrltlufv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.epnwcf.com/Article/details/gcopkrkgs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/grzbiiesq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gejnicqut.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/glflbfwfh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.vehdjk.com/Article/details/gyhzycsbc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.epnwcf.com/Article/details/gxpsxcsbb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.tarul.cn/Article/details/gtttcqnyy.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fktsv.cn/Article/details/ganvluawe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.vehdjk.com/Article/details/gucudectr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.vehdjk.com/Article/details/grwwxzudc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.epnwcf.com/Article/details/gqfryipaw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.yfazqb.com/Article/details/gvzdykqsn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.yfazqb.com/Article/details/gylaqvvxn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrohmxgn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.bbcook.cn/Article/details/gczlquhsa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.bbcook.cn/Article/details/gwuswlfer.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fktsv.cn/Article/details/gnbvehdcu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fktsv.cn/Article/details/gkmhpopkb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fktsv.cn/Article/details/gntzwxpwn.sHtML


<!-- 参考信息 -->