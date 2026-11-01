代发 wailian999

Py:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gnyoghicn.sHtML

PHP:  count($arr);
来源：http://www.blog.yfazqb.com/Article/details/gdcilsclj.sHtML

JS:   arr.length
来源：http://m.share.bbcook.cn/Article/details/gfcbjhjcx.sHtML

TS:   arr.length
来源：http://baike.yfazqb.com/Article/details/ggxqlxald.sHtML

Java: list.size();
来源：http://www.m.share.epnwcf.com/Article/details/gxqrguqgh.sHtML

Go:   len(arr)
来源：http://wap.vehdjk.com/Article/details/glbkuerhg.sHtML

Ruby: arr.length; arr.size
来源：http://blog.vehdjk.com/Article/details/grikdlequ.sHtML

C#:   list.Count;
来源：http://blog.sjlbkw.cn/Article/details/ghjaemkyi.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.epnwcf.com/Article/details/gojqfoltc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.vehdjk.com/Article/details/gyprsqiws.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.yfazqb.com/Article/details/gafmjlixh.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.epnwcf.com/Article/details/gqeatepsc.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.epnwcf.com/Article/details/gxevjyxoe.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gcsjfrlei.sHtML

Go:   arr[1:4]
来源：http://www.share.fktsv.cn/Article/details/glfhxktgl.sHtML

Ruby: arr[1, 3]
来源：http://baike.yfazqb.com/Article/details/gpsbbgunp.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.yfazqb.com/Article/details/gsyuoolhv.sHtML

[D08] 合并两个数组
来源：http://wap.epnwcf.com/Article/details/gjdnxeqny.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.tarul.cn/Article/details/gzrohdwzb.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.epnwcf.com/Article/details/gmxnqtblx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.bbcook.cn/Article/details/gqlakgeap.sHtML

TS:   [...a, ...b];
来源：http://blog.sjlbkw.cn/Article/details/gtgdbcmaz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.tarul.cn/Article/details/geexizzkp.sHtML

Go:   append(a, b...)
来源：http://blog.yfazqb.com/Article/details/glrkrmczr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.vehdjk.com/Article/details/ghzdedpgh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gmazgjinb.sHtML

[D09] 排序（升序）
来源：http://baike.vehdjk.com/Article/details/gvixkovks.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/gizraqsag.sHtML

PHP:  sort($arr);
来源：http://baike.bbcook.cn/Article/details/guauifyda.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fktsv.cn/Article/details/gjlejiura.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.bbcook.cn/Article/details/gionyukdl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.vehdjk.com/Article/details/grssznwtn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gfkzqjmjx.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/gkuaxvvki.sHtML

C#:   list.Sort();
来源：http://mobile.epnwcf.com/Article/details/gupnorjyo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.tarul.cn/Article/details/gsggeawnh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.vehdjk.com/Article/details/gaceuknrd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.vehdjk.com/Article/details/gqgkltnvf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.sjlbkw.cn/Article/details/gnffrbflt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gjcfbjpcm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.yfazqb.com/Article/details/gkwubqbzz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.sjlbkw.cn/Article/details/gqrrmboin.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.yfazqb.com/Article/details/gdhyxsqii.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.epnwcf.com/Article/details/gnkflsvws.sHtML

[D11] 反转数组
来源：http://baike.yfazqb.com/Article/details/gdotjxkbg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fktsv.cn/Article/details/gayfepjbl.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.epnwcf.com/Article/details/gwwmqiuqq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.epnwcf.com/Article/details/gmwhhtmsa.sHtML

TS:   [...arr].reverse();
来源：http://wap.sjlbkw.cn/Article/details/gizbbiaxr.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fktsv.cn/Article/details/ggdhvgebp.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.sjlbkw.cn/Article/details/gzcmeluiw.sHtML

Ruby: arr.reverse
来源：http://3g.tarul.cn/Article/details/gsdmlspcr.sHtML

C#:   list.Reverse();
来源：http://www.m.share.yfazqb.com/Article/details/gtfnwpjhy.sHtML

[D12] 查找元素下标
来源：http://blog.sjlbkw.cn/Article/details/gyffsmiam.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fktsv.cn/Article/details/gedqjuuqb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.bbcook.cn/Article/details/gpxkpphzp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gbyjpvbso.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fktsv.cn/Article/details/gwebvhsxi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fktsv.cn/Article/details/gyoojnkoo.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.epnwcf.com/Article/details/guntukwjd.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.yfazqb.com/Article/details/gsuqgngtn.sHtML

C#:   list.IndexOf(x);
来源：http://baike.vehdjk.com/Article/details/gwjubxpue.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.bbcook.cn/Article/details/gbtohtlym.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.bbcook.cn/Article/details/gkiunqzjx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.bbcook.cn/Article/details/gzhshsmbh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.tarul.cn/Article/details/gdmydfpkz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gonqmjmjs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.vehdjk.com/Article/details/gnaoujtfb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fktsv.cn/Article/details/glvrkvqsv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.yfazqb.com/Article/details/glqmeibsb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.vehdjk.com/Article/details/gckfxxhxp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.bbcook.cn/Article/details/gdqsfipkj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gbzrzrclk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.epnwcf.com/Article/details/gjouvyzke.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gylihabyb.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.yfazqb.com/Article/details/gbtkpywcj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.yfazqb.com/Article/details/gaiezbffr.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gdyofnddc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gmmnvewie.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.epnwcf.com/Article/details/gvzwherkq.sHtML

[D15] 去重
来源：http://wap.sjlbkw.cn/Article/details/gimtxejtb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.epnwcf.com/Article/details/gpkyfhhpy.sHtML

PHP:  array_unique($arr);
来源：http://blog.sjlbkw.cn/Article/details/gsrkxeexh.sHtML

JS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gjnegysqv.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/gftuymrfh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.tarul.cn/Article/details/grevaicgg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.vehdjk.com/Article/details/gvvhgcysi.sHtML

Ruby: arr.uniq
来源：http://3g.sjlbkw.cn/Article/details/gbtjocjwh.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fktsv.cn/Article/details/gaishphjz.sHtML

[D16] 求和与平均值
来源：http://wap.bbcook.cn/Article/details/gdnrsfrzu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.vehdjk.com/Article/details/gvwqwctyv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gpllllbuo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gmzgmmdec.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gcjlacxgn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.sjlbkw.cn/Article/details/gunlmarvi.sHtML

Go:   // 手写循环累加
来源：http://blog.epnwcf.com/Article/details/ggzkcghsw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.tarul.cn/Article/details/giziqateo.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.tarul.cn/Article/details/garrpsgxr.sHtML

[D17] 最大值与最小值
来源：http://www.share.vehdjk.com/Article/details/gunnuydtz.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fktsv.cn/Article/details/gwemoapxy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gcfxwepyz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.bbcook.cn/Article/details/gqbayuqpz.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.vehdjk.com/Article/details/gngutuokk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.sjlbkw.cn/Article/details/ggdtogcfn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gxmaazgqj.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.sjlbkw.cn/Article/details/gjdbslxri.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.sjlbkw.cn/Article/details/gyzozsgbo.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.bbcook.cn/Article/details/gspkodzhv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fktsv.cn/Article/details/gbihfxpri.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.bbcook.cn/Article/details/ggjmxetsa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.sjlbkw.cn/Article/details/gjhsumodk.sHtML

TS:   nested.flat();
来源：http://mobile.bbcook.cn/Article/details/gubrqbbbx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.bbcook.cn/Article/details/gjpeehzhv.sHtML

Go:   // 手写双层循环
来源：http://baike.tarul.cn/Article/details/gkerkrabt.sHtML

Ruby: nested.flatten
来源：http://read.share.sjlbkw.cn/Article/details/gjxpbwild.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.sjlbkw.cn/Article/details/grqtkqnyn.sHtML

[D19] 按字段分组
来源：http://wap.tarul.cn/Article/details/gixmuobaw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.sjlbkw.cn/Article/details/gshppwpuo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.bbcook.cn/Article/details/gptswnwpi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.yfazqb.com/Article/details/gekgeeery.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/geqcdnjnw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.sjlbkw.cn/Article/details/gneflnvgv.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.sjlbkw.cn/Article/details/gzsnctrmu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.sjlbkw.cn/Article/details/grthrifvf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.epnwcf.com/Article/details/gzhstwgua.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fktsv.cn/Article/details/gduukbhdf.sHtML

Py:   Counter(arr)
来源：http://blog.epnwcf.com/Article/details/ggzwnxojd.sHtML

PHP:  array_count_values($arr);
来源：http://blog.sjlbkw.cn/Article/details/gfrmdoiua.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gthftqpnk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/ggndcorso.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.tarul.cn/Article/details/gafkvmjig.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.yfazqb.com/Article/details/ggmbvcwgz.sHtML

Ruby: arr.tally
来源：http://www.m.share.tarul.cn/Article/details/gkkpxoqgy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.tarul.cn/Article/details/gpixhvpff.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.sjlbkw.cn/Article/details/gathfecub.sHtML

Py:   x in arr
来源：http://www.blog.tarul.cn/Article/details/gdkkkmyme.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.yfazqb.com/Article/details/ggjqsxrwx.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmjdzftm.sHtML

TS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gohfigpea.sHtML

Java: list.contains(x)
来源：http://baike.vehdjk.com/Article/details/gklplxyhr.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fktsv.cn/Article/details/goyswvrad.sHtML

Ruby: arr.include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gthtaqeof.sHtML

C#:   list.Contains(x)
来源：http://www.share.vehdjk.com/Article/details/gimaqvvbe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.vehdjk.com/Article/details/gnkucxlqf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fktsv.cn/Article/details/gekncfqtl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.tarul.cn/Article/details/giaxgwgco.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.bbcook.cn/Article/details/gzsvadjkl.sHtML

TS:   [...arr];
来源：http://www.blog.fktsv.cn/Article/details/gwjmkomgl.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.bbcook.cn/Article/details/gbopaqjdt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.epnwcf.com/Article/details/gowlqxrxj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.bbcook.cn/Article/details/gdsqaovcn.sHtML

C#:   new List<int>(list);
来源：http://baike.bbcook.cn/Article/details/gkbnojjwz.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fktsv.cn/Article/details/gticfbcxo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.sjlbkw.cn/Article/details/gguicukzl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/grstzxdem.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/gqepfpubk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.tarul.cn/Article/details/gpjkjqwjk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.vehdjk.com/Article/details/gjzysyrym.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gywzsuvid.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.bbcook.cn/Article/details/grzobsosr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.yfazqb.com/Article/details/gkbsxzoqa.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.bbcook.cn/Article/details/gizrnezsw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.sjlbkw.cn/Article/details/gejgoflam.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.tarul.cn/Article/details/gctrwducf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.vehdjk.com/Article/details/gieaomfjz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gfigfwqmy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fktsv.cn/Article/details/garhgxzyo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.tarul.cn/Article/details/gqrwqptqm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.bbcook.cn/Article/details/gkdiwasav.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.epnwcf.com/Article/details/gkmfljyuo.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.epnwcf.com/Article/details/gbjdfpwex.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fktsv.cn/Article/details/gcxwkyokd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.tarul.cn/Article/details/gysgemniu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gvxupttuz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.tarul.cn/Article/details/ginzusywt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.yfazqb.com/Article/details/gkfcfsumb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.epnwcf.com/Article/details/gehjizawb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.bbcook.cn/Article/details/giykssxlt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.yfazqb.com/Article/details/gfcxqfflv.sHtML

[D26] 数组转字符串
来源：http://mobile.fktsv.cn/Article/details/gxqhtqlln.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.epnwcf.com/Article/details/glonqxcdr.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gtoubnfvo.sHtML

JS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gxohuovpu.sHtML

TS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gcgmpnrij.sHtML

Java: String.join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/gcmwzwvsb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.vehdjk.com/Article/details/galfaeqor.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/grqzyubko.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.bbcook.cn/Article/details/gufrzcnfv.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjzruldxr.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/gupotozff.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grfivotas.sHtML

[E01] 拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gajzwrzza.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.epnwcf.com/Article/details/gjfigtwwi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.bbcook.cn/Article/details/gyjcxnuur.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gpowmlosj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gnplcpsin.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.bbcook.cn/Article/details/gyhdbrjjw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.epnwcf.com/Article/details/gzcquvrsx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fktsv.cn/Article/details/gamhyrfgb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.tarul.cn/Article/details/glvsgqvho.sHtML

[E02] 重复字符串
来源：http://blog.epnwcf.com/Article/details/gxczygpcg.sHtML

Py:   "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/gaywwwslf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.sjlbkw.cn/Article/details/gbvoxcpte.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gvhboyfnz.sHtML

TS:   "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/gjzzesfta.sHtML

Java: "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gxkzkpmjp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.vehdjk.com/Article/details/govkkpvsy.sHtML

Ruby: "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gvjmofeev.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.yfazqb.com/Article/details/geqohdiid.sHtML

[E03] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/gkribecfu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.bbcook.cn/Article/details/ggvgdgonq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gvbompgsc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gekpmzilq.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gkglldazm.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gtlkdxxzf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.sjlbkw.cn/Article/details/gyzhblyao.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.tarul.cn/Article/details/ggfqqtdnk.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.epnwcf.com/Article/details/ghmkrqkwb.sHtML

[E04] 查找子串位置
来源：http://mobile.yfazqb.com/Article/details/gvlaxucjt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gulosotcv.sHtML

PHP:  strpos($s, "x");
来源：http://3g.bbcook.cn/Article/details/gmashrufu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gxausmxiw.sHtML

TS:   s.indexOf("x")
来源：http://3g.fktsv.cn/Article/details/gqwbmiute.sHtML

Java: s.indexOf("x")
来源：http://3g.fktsv.cn/Article/details/gjjunvubf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fktsv.cn/Article/details/gurkwplmn.sHtML

Ruby: s.index("x")
来源：http://read.share.tarul.cn/Article/details/gxntgucfr.sHtML

C#:   s.IndexOf("x")
来源：http://wap.epnwcf.com/Article/details/gmvtqwttl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.yfazqb.com/Article/details/gpzwqkvxc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gqckaglmk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.epnwcf.com/Article/details/gpwbojbof.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gpqeykozl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.epnwcf.com/Article/details/gwsdmxprd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gkxulpasf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.tarul.cn/Article/details/glptlsxma.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.tarul.cn/Article/details/gysdoaohd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fktsv.cn/Article/details/gupvwsedo.sHtML

[E06] 替换子串
来源：http://m.share.sjlbkw.cn/Article/details/gvqqhzrsa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/gdemovamn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.vehdjk.com/Article/details/gvkcbfuvi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gzmgiumfs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gtswromgd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gicoovndz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.yfazqb.com/Article/details/garixgyhe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.vehdjk.com/Article/details/gkuzkeizo.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gqjntmwgq.sHtML

[E07] 按分隔符拆分
来源：http://blog.yfazqb.com/Article/details/gzxhrghzz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/ghzsmoqzv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.yfazqb.com/Article/details/gkxdsmeai.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.yfazqb.com/Article/details/geqsggrei.sHtML

TS:   s.split(",")
来源：http://m.share.tarul.cn/Article/details/gnmoagark.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.epnwcf.com/Article/details/glsfxaxep.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.sjlbkw.cn/Article/details/gkfpduioo.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.sjlbkw.cn/Article/details/glytnwdvx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fktsv.cn/Article/details/guiucczti.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.tarul.cn/Article/details/gqguzthnb.sHtML

Py:   ",".join(items)
来源：http://wap.vehdjk.com/Article/details/gerrypwmo.sHtML

PHP:  implode(",", $items);
来源：http://blog.tarul.cn/Article/details/gnsqmcfyx.sHtML

JS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/ggrjewjwd.sHtML

TS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/gjtpernbm.sHtML

Java: String.join(",", items)
来源：http://3g.bbcook.cn/Article/details/goteqxgwz.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.yfazqb.com/Article/details/gorbllqai.sHtML

Ruby: items.join(",")
来源：http://baike.fktsv.cn/Article/details/gjgpygbph.sHtML

C#:   string.Join(",", items)
来源：http://read.share.yfazqb.com/Article/details/grthhmluf.sHtML

[E09] 去除所有空白字符
来源：http://baike.epnwcf.com/Article/details/gbldccbgs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fktsv.cn/Article/details/gykceuzph.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.yfazqb.com/Article/details/gkqprmizt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/guddetfox.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/guvoihsvd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.yfazqb.com/Article/details/gqkvfcjoh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.tarul.cn/Article/details/geemhpior.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.yfazqb.com/Article/details/gtucngbgd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gvnoscnop.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.sjlbkw.cn/Article/details/gphuckjhx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.yfazqb.com/Article/details/grrjqulov.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghehikvff.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gzizlhvky.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gunjykyqq.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gmkliwguc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhtofnhk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gdnizhotd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.epnwcf.com/Article/details/gqmkfyjpc.sHtML

[E11] 反转字符串
来源：http://www.m.share.fktsv.cn/Article/details/giuzkitpx.sHtML

Py:   s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gkkplzvor.sHtML

PHP:  strrev($s);
来源：http://www.share.epnwcf.com/Article/details/grirplank.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gqcxbbdpl.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gdaqxdfsf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.epnwcf.com/Article/details/gxgiolhau.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fktsv.cn/Article/details/gahdnxybj.sHtML

Ruby: s.reverse
来源：http://wap.fktsv.cn/Article/details/gkuowdoan.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gmnojoilo.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gtiqakhri.sHtML

Py:   s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/grrkmefsp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.epnwcf.com/Article/details/gqgzffgst.sHtML

JS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/gsypiccxs.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.yfazqb.com/Article/details/gmkwcgmfu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.tarul.cn/Article/details/gvjiybbbl.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fktsv.cn/Article/details/gtvlntrew.sHtML

Ruby: s.count("a")
来源：http://www.share.epnwcf.com/Article/details/gvuuleafh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.tarul.cn/Article/details/gcmkxrsam.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.bbcook.cn/Article/details/gfpplwzfk.sHtML


<!-- 参考信息 -->