代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.tarul.cn/Article/details/gfbnaqley.sHtML

TS:   [...a, ...b];
来源：http://www.share.fktsv.cn/Article/details/gsxttnpnn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.yfazqb.com/Article/details/gelegsrgs.sHtML

Go:   append(a, b...)
来源：http://www.share.epnwcf.com/Article/details/gvloumfoq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.bbcook.cn/Article/details/gskflnoqi.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.tarul.cn/Article/details/ghqsdbcuh.sHtML

[D09] 排序（升序）
来源：http://baike.fktsv.cn/Article/details/gzhzenrbs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.sjlbkw.cn/Article/details/ggacsbvdo.sHtML

PHP:  sort($arr);
来源：http://read.share.fktsv.cn/Article/details/gdvwtsisx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.epnwcf.com/Article/details/gypfokcxa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.sjlbkw.cn/Article/details/ghjsfhdau.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.tarul.cn/Article/details/gycjvfpzj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gwvbfjhsr.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/glphdeqlx.sHtML

C#:   list.Sort();
来源：http://baike.tarul.cn/Article/details/gbovuxwcx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fktsv.cn/Article/details/gxrctskzs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.bbcook.cn/Article/details/guxtulcma.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/gupjegawx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/gpimwzifi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.yfazqb.com/Article/details/ggwwdlodx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.vehdjk.com/Article/details/gsvpedqgp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gcjhwpefk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.vehdjk.com/Article/details/gdsdlkglf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.vehdjk.com/Article/details/gcrdkxyma.sHtML

[D11] 反转数组
来源：http://wap.vehdjk.com/Article/details/gxagcctdm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fktsv.cn/Article/details/gavdcwxyn.sHtML

PHP:  array_reverse($arr);
来源：http://3g.sjlbkw.cn/Article/details/gufqyjwem.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.epnwcf.com/Article/details/gzmsokvvz.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.sjlbkw.cn/Article/details/gtuzasyoh.sHtML

Java: Collections.reverse(list);
来源：http://read.share.vehdjk.com/Article/details/gvafovwzk.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.epnwcf.com/Article/details/gpamknxvy.sHtML

Ruby: arr.reverse
来源：http://m.share.bbcook.cn/Article/details/gmousqsec.sHtML

C#:   list.Reverse();
来源：http://blog.sjlbkw.cn/Article/details/gzgvhsfzf.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fktsv.cn/Article/details/gvqrelvkq.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.sjlbkw.cn/Article/details/gcxldpmtn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.tarul.cn/Article/details/gmvauwquh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/gxokbjdvb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/gaxsgjwfm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fktsv.cn/Article/details/gcdnylobu.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/glybzyjsu.sHtML

Ruby: arr.index(x)
来源：http://read.share.epnwcf.com/Article/details/glgioejuv.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.vehdjk.com/Article/details/gfuvobgzb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.tarul.cn/Article/details/glsnjhtjz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fktsv.cn/Article/details/gptyioofe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.epnwcf.com/Article/details/gsmucrlur.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gcfycnuib.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gjryfmjqj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gghiirypq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.bbcook.cn/Article/details/grzeshiya.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.tarul.cn/Article/details/ggwstucpd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.epnwcf.com/Article/details/gpuweabmb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.yfazqb.com/Article/details/gfjjyeduw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fktsv.cn/Article/details/gtxzgpfsb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fktsv.cn/Article/details/gcixerggv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/giigmvqtm.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/gcqdomgvx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gfzpzszqv.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gwzllsxap.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.vehdjk.com/Article/details/ggopodoix.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gnemjgqmn.sHtML

[D15] 去重
来源：http://read.share.tarul.cn/Article/details/gmcpgiyxg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/grjmksrav.sHtML

PHP:  array_unique($arr);
来源：http://m.share.tarul.cn/Article/details/gfmltyfup.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gctrkmlvw.sHtML

TS:   [...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gxiyhoaqe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.yfazqb.com/Article/details/gfxhgethz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.bbcook.cn/Article/details/gynaqzhiq.sHtML

Ruby: arr.uniq
来源：http://3g.yfazqb.com/Article/details/gsxsnlvne.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.tarul.cn/Article/details/ghgwoubbi.sHtML

[D16] 求和与平均值
来源：http://wap.fktsv.cn/Article/details/gvvigbwgu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gogpnefde.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.yfazqb.com/Article/details/gfgnwzmyu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/grorbfhbo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/gdbjecznu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.yfazqb.com/Article/details/gtdhwadzi.sHtML

Go:   // 手写循环累加
来源：http://read.share.tarul.cn/Article/details/gkkqzqyxe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.sjlbkw.cn/Article/details/gggmligun.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fktsv.cn/Article/details/gucmqtgvl.sHtML

[D17] 最大值与最小值
来源：http://wap.sjlbkw.cn/Article/details/grugrnqhh.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.bbcook.cn/Article/details/gkxnfkyur.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.sjlbkw.cn/Article/details/geerhilfm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fktsv.cn/Article/details/ghufdqhap.sHtML

TS:   Math.max(...arr);
来源：http://m.share.tarul.cn/Article/details/gtgftnqod.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.vehdjk.com/Article/details/gwchoqejm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.bbcook.cn/Article/details/gmqwwtzmi.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.vehdjk.com/Article/details/gfllqergo.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.vehdjk.com/Article/details/gnjvgvymw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.sjlbkw.cn/Article/details/grenztggj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.vehdjk.com/Article/details/gjekvywiw.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.tarul.cn/Article/details/gloesqsay.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.epnwcf.com/Article/details/gpsuhtxlr.sHtML

TS:   nested.flat();
来源：http://mobile.fktsv.cn/Article/details/gyolyzevx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.epnwcf.com/Article/details/gxadoyrqh.sHtML

Go:   // 手写双层循环
来源：http://www.blog.sjlbkw.cn/Article/details/gfqeeeyft.sHtML

Ruby: nested.flatten
来源：http://wap.fktsv.cn/Article/details/gorwlohig.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/glxhtcllj.sHtML

[D19] 按字段分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrjwdipf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.tarul.cn/Article/details/gehwjvkiw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.sjlbkw.cn/Article/details/gczzghyyu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.tarul.cn/Article/details/gzizvhyiv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.yfazqb.com/Article/details/glwrolusk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.epnwcf.com/Article/details/gusagdrby.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.vehdjk.com/Article/details/gtmrccxdz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.yfazqb.com/Article/details/grqtgbpaj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.tarul.cn/Article/details/gjylcscde.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.vehdjk.com/Article/details/gmxpxxpic.sHtML

Py:   Counter(arr)
来源：http://baike.sjlbkw.cn/Article/details/gdhlvjklu.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.yfazqb.com/Article/details/gtblxiwba.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gdzewmdid.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.vehdjk.com/Article/details/gvfllvkwx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.sjlbkw.cn/Article/details/ghgllxjgk.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.vehdjk.com/Article/details/glyqepbvq.sHtML

Ruby: arr.tally
来源：http://m.share.epnwcf.com/Article/details/geqdklkrf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.tarul.cn/Article/details/gtgognepa.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.yfazqb.com/Article/details/gyfhuvztx.sHtML

Py:   x in arr
来源：http://m.share.sjlbkw.cn/Article/details/gzjumrqge.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.sjlbkw.cn/Article/details/glpgnwpoa.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/grmuvufcm.sHtML

TS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gslftzpws.sHtML

Java: list.contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gsifslbvf.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gfwimmnwn.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/gcrcxqupe.sHtML

C#:   list.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gucmdcxrt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.sjlbkw.cn/Article/details/gnorvhiar.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.sjlbkw.cn/Article/details/gzynzitkc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fktsv.cn/Article/details/gnuloxrae.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gogqdupza.sHtML

TS:   [...arr];
来源：http://m.share.yfazqb.com/Article/details/gmhxvsmij.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.sjlbkw.cn/Article/details/gprjpxeoi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.sjlbkw.cn/Article/details/gyyvqmlkx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.vehdjk.com/Article/details/gsbajconf.sHtML

C#:   new List<int>(list);
来源：http://blog.bbcook.cn/Article/details/gvejcsrai.sHtML

[D23] reduce 累积计算
来源：http://m.share.sjlbkw.cn/Article/details/glpvpbmps.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.tarul.cn/Article/details/glgohoqyx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fktsv.cn/Article/details/glzczbkrw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/goqhtqmda.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/gvrziavzr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.yfazqb.com/Article/details/gmhdarjtr.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/gepwrkuwc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.epnwcf.com/Article/details/ggdbcoulr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.bbcook.cn/Article/details/giqsuqpio.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.yfazqb.com/Article/details/gudsokbbe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.epnwcf.com/Article/details/gnpfkibqh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.sjlbkw.cn/Article/details/gpenbmlnw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.tarul.cn/Article/details/gpwseteqo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.yfazqb.com/Article/details/gnjffjvbz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/getljkmia.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.bbcook.cn/Article/details/gtrqytxes.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.epnwcf.com/Article/details/goievrcsz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.bbcook.cn/Article/details/gdihywmjz.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fktsv.cn/Article/details/gtymazprg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.bbcook.cn/Article/details/gxrnzvejl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.yfazqb.com/Article/details/gopdcjdnx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.yfazqb.com/Article/details/gzdagvvcz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fktsv.cn/Article/details/gmihmhgai.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fktsv.cn/Article/details/gtupwmuix.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.yfazqb.com/Article/details/gixdctmec.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fktsv.cn/Article/details/gvqelnpgc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.tarul.cn/Article/details/gtrmskebm.sHtML

[D26] 数组转字符串
来源：http://baike.epnwcf.com/Article/details/gfaphhhyt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.vehdjk.com/Article/details/gcuoqsdnx.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/gaxdphbka.sHtML

JS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gjuugymsp.sHtML

TS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gbaqovsru.sHtML

Java: String.join(", ", list)
来源：http://3g.fktsv.cn/Article/details/gqfwzdvik.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.yfazqb.com/Article/details/glhjxnwcq.sHtML

Ruby: arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gpeufkjiy.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/gqdttfidr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gvomdhrhn.sHtML

E. 字符串处理
来源：http://www.blog.epnwcf.com/Article/details/gjrdtgmtr.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfxctzrbk.sHtML

[E01] 拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gfthgzdko.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.bbcook.cn/Article/details/geemngetl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.vehdjk.com/Article/details/gpflqhsiu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/glzecechk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/gjjlxlfkr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.epnwcf.com/Article/details/gaqaxhinh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.vehdjk.com/Article/details/ghgcrootv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.epnwcf.com/Article/details/garkyzquo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fktsv.cn/Article/details/gonprmbsq.sHtML

[E02] 重复字符串
来源：http://blog.vehdjk.com/Article/details/ggxdwrzgm.sHtML

Py:   "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gtdkebppx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.yfazqb.com/Article/details/gaolhonfu.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gllamxkoq.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gzklbcscd.sHtML

Java: "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gyodblbxy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.tarul.cn/Article/details/gxrvhamlb.sHtML

Ruby: "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/genfruzsa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/gfbvhnvab.sHtML

[E03] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gmcmfzqrk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.epnwcf.com/Article/details/gpqkyaaxv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gfxviwbhx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gyblwlxmv.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.tarul.cn/Article/details/gerqbenfl.sHtML

Java: s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/ghyyfuybn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.tarul.cn/Article/details/gskdbjqgy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.epnwcf.com/Article/details/ggmqsmnzs.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.bbcook.cn/Article/details/gjsozmked.sHtML

[E04] 查找子串位置
来源：http://www.m.share.sjlbkw.cn/Article/details/gilrpbasd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.bbcook.cn/Article/details/gnjsyilni.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fktsv.cn/Article/details/gghzpqhvv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gshkszglp.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gijlvozcq.sHtML

Java: s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gstiltfea.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.yfazqb.com/Article/details/gcfatmsef.sHtML

Ruby: s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gxbtuwgst.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gijgmgujw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.bbcook.cn/Article/details/gwobliduj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.yfazqb.com/Article/details/grjzsubxx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.yfazqb.com/Article/details/ghpxqacia.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/grjbhdqdu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.sjlbkw.cn/Article/details/gtthzpijw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gehpxbrle.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.epnwcf.com/Article/details/gnuszordr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.yfazqb.com/Article/details/gdexmmmov.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fktsv.cn/Article/details/grovfxhtn.sHtML

[E06] 替换子串
来源：http://www.share.bbcook.cn/Article/details/gcuzeeiho.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gkibhaqjf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.sjlbkw.cn/Article/details/gcgngmnxb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gimaetkrp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gwepowxee.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gcqhvgfou.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/gxvutkmyu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gufbdiyul.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gdaojqdek.sHtML

[E07] 按分隔符拆分
来源：http://blog.fktsv.cn/Article/details/gtyclanbj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.epnwcf.com/Article/details/grmvoombw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.vehdjk.com/Article/details/gkivtrmxj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.sjlbkw.cn/Article/details/greihxojl.sHtML

TS:   s.split(",")
来源：http://mobile.bbcook.cn/Article/details/gsciiwyzd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.sjlbkw.cn/Article/details/gujqlodkw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.vehdjk.com/Article/details/gbtvlfxvw.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.tarul.cn/Article/details/gtqtjuqsr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.epnwcf.com/Article/details/gbujfywqd.sHtML

[E08] 数组按分隔符合并
来源：http://blog.vehdjk.com/Article/details/gutkbpiae.sHtML

Py:   ",".join(items)
来源：http://read.share.epnwcf.com/Article/details/gneosorpo.sHtML

PHP:  implode(",", $items);
来源：http://www.share.epnwcf.com/Article/details/gojwhmdti.sHtML

JS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gajmezvok.sHtML

TS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gfblgktnb.sHtML

Java: String.join(",", items)
来源：http://wap.tarul.cn/Article/details/gxmalhisa.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.sjlbkw.cn/Article/details/gknhbvehd.sHtML

Ruby: items.join(",")
来源：http://www.share.tarul.cn/Article/details/gufhjjtwh.sHtML

C#:   string.Join(",", items)
来源：http://m.share.bbcook.cn/Article/details/ggyjdhvzs.sHtML

[E09] 去除所有空白字符
来源：http://read.share.yfazqb.com/Article/details/gxllswqam.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.tarul.cn/Article/details/gwbwaflmh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.tarul.cn/Article/details/gvkawvzgz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.bbcook.cn/Article/details/gxoldptbq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/gnbyduzaq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.tarul.cn/Article/details/gcwvqmnwc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fktsv.cn/Article/details/gddkrlrsj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.sjlbkw.cn/Article/details/gxpaztdky.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/govgoqbxd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.bbcook.cn/Article/details/gppmtgenz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.vehdjk.com/Article/details/gpfnsvarr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.vehdjk.com/Article/details/gvhtnkoxd.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/grvfobwvq.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gjjqtwunu.sHtML

Java: String.format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gqelknfda.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/goqwgvasf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gedjhyhtf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.sjlbkw.cn/Article/details/gzbixvlxh.sHtML

[E11] 反转字符串
来源：http://3g.sjlbkw.cn/Article/details/gbzxxlqhi.sHtML

Py:   s[::-1]
来源：http://3g.tarul.cn/Article/details/grdmeoxap.sHtML

PHP:  strrev($s);
来源：http://blog.bbcook.cn/Article/details/gcqqwanaf.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gnrxbfipq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/grxfimyub.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.yfazqb.com/Article/details/gicwrhhha.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.bbcook.cn/Article/details/gixbijboo.sHtML

Ruby: s.reverse
来源：http://3g.bbcook.cn/Article/details/gtsrnrivt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gakgrgcco.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.yfazqb.com/Article/details/gjhcjrvrd.sHtML

Py:   s.count("a")
来源：http://mobile.yfazqb.com/Article/details/gpaoddbpy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fktsv.cn/Article/details/gohecqxwo.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gnpfdywah.sHtML

TS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gbyonmpix.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.tarul.cn/Article/details/ggmosniwf.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.sjlbkw.cn/Article/details/gqxqphtnw.sHtML

Ruby: s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gcbviceyc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fktsv.cn/Article/details/gqtmjrabd.sHtML

[E13] 逐字符遍历
来源：http://read.share.vehdjk.com/Article/details/gtxkdzduk.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.yfazqb.com/Article/details/gnxxkphlw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.vehdjk.com/Article/details/gnxfwparc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gptzgjcwe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gzcjhfbso.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.tarul.cn/Article/details/ghnyifwus.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.yfazqb.com/Article/details/ghkubcnra.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.yfazqb.com/Article/details/goxtiacgj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gdmwzeiws.sHtML

[E14] URL 编码与 Base64
来源：http://blog.sjlbkw.cn/Article/details/gdjhaupip.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.tarul.cn/Article/details/gssgcztym.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.vehdjk.com/Article/details/goifensuu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.sjlbkw.cn/Article/details/grehlyczn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.epnwcf.com/Article/details/gamogbvev.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/goywjuwpn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.vehdjk.com/Article/details/guqtccgem.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.epnwcf.com/Article/details/grhfewuds.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.tarul.cn/Article/details/gnysazsee.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.epnwcf.com/Article/details/gjbaxuqco.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/guvogpoje.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.yfazqb.com/Article/details/glvsgysbe.sHtML


<!-- 参考信息 -->