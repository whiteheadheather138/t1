代发 wailian999

Java: list.size();
来源：http://mobile.bbcook.cn/Article/details/gbhvibhmv.sHtML

Go:   len(arr)
来源：http://read.share.vehdjk.com/Article/details/ghbmcuvnf.sHtML

Ruby: arr.length; arr.size
来源：http://3g.sjlbkw.cn/Article/details/ghzgvmjha.sHtML

C#:   list.Count;
来源：http://wap.fktsv.cn/Article/details/gwavjfvil.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.bbcook.cn/Article/details/gaojvuvjp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fktsv.cn/Article/details/gmarwqfat.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.bbcook.cn/Article/details/gjpgdfyav.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/grpmvihrb.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/galchjtet.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fktsv.cn/Article/details/glmkwokto.sHtML

Go:   arr[1:4]
来源：http://www.m.share.vehdjk.com/Article/details/gconfgnnt.sHtML

Ruby: arr[1, 3]
来源：http://www.share.bbcook.cn/Article/details/gcgckeelw.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.epnwcf.com/Article/details/gwrfxrivb.sHtML

[D08] 合并两个数组
来源：http://www.share.epnwcf.com/Article/details/gcvfsggfp.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.yfazqb.com/Article/details/gywpthnlx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.yfazqb.com/Article/details/gadtyeymz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.epnwcf.com/Article/details/gydwelszy.sHtML

TS:   [...a, ...b];
来源：http://3g.vehdjk.com/Article/details/gqtjobiuc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.tarul.cn/Article/details/gbyahqzpo.sHtML

Go:   append(a, b...)
来源：http://read.share.bbcook.cn/Article/details/gmfomyjds.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.yfazqb.com/Article/details/goqgcdgjq.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.yfazqb.com/Article/details/gxqyutpkr.sHtML

[D09] 排序（升序）
来源：http://www.blog.bbcook.cn/Article/details/gqkojgdpx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gqqgkvppt.sHtML

PHP:  sort($arr);
来源：http://mobile.tarul.cn/Article/details/gpynvpzis.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.yfazqb.com/Article/details/gqmpwtycm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.vehdjk.com/Article/details/gksfmutsx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.tarul.cn/Article/details/gshrlwint.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gdfozhtua.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/gkszhxwsa.sHtML

C#:   list.Sort();
来源：http://www.m.share.tarul.cn/Article/details/gecwtbflt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.yfazqb.com/Article/details/ghktfyjvj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.tarul.cn/Article/details/gfjusdfpc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fktsv.cn/Article/details/gxzltoydm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/gzuqvzlak.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.tarul.cn/Article/details/gpeocjfln.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.vehdjk.com/Article/details/gygsqkwik.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.bbcook.cn/Article/details/glxnpkbpu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.epnwcf.com/Article/details/gxswlwefr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fktsv.cn/Article/details/gshhbkuru.sHtML

[D11] 反转数组
来源：http://baike.yfazqb.com/Article/details/gfclkmpsc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.vehdjk.com/Article/details/gkviaglzh.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.bbcook.cn/Article/details/grqrfbacz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fktsv.cn/Article/details/gtcnpihgk.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.sjlbkw.cn/Article/details/glpehujxf.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/gfsbabgnh.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.sjlbkw.cn/Article/details/gonizhtyr.sHtML

Ruby: arr.reverse
来源：http://m.share.epnwcf.com/Article/details/gldmfkqsz.sHtML

C#:   list.Reverse();
来源：http://www.share.vehdjk.com/Article/details/gxjtqlgwc.sHtML

[D12] 查找元素下标
来源：http://www.blog.vehdjk.com/Article/details/gbilvcwin.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.tarul.cn/Article/details/gtjjqogiw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.sjlbkw.cn/Article/details/geniefynd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/gzhwzajnf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/gzexrygds.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.yfazqb.com/Article/details/gtanksexz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.bbcook.cn/Article/details/guqjkgxch.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.tarul.cn/Article/details/gmahfirhs.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.tarul.cn/Article/details/gbyzyyeha.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.yfazqb.com/Article/details/getkwwqpc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fktsv.cn/Article/details/gvgvxdpsh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.vehdjk.com/Article/details/gmpurxcol.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gtjykmhic.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.bbcook.cn/Article/details/grixnkxih.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.bbcook.cn/Article/details/gvqdbuhri.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.tarul.cn/Article/details/gsuxemzfd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.tarul.cn/Article/details/gbvgefutj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.yfazqb.com/Article/details/gopcpcene.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.epnwcf.com/Article/details/gdakdxegw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gndzidasd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gzlarorhc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.vehdjk.com/Article/details/gafjzoiop.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/gycceysqm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.bbcook.cn/Article/details/gxsqnyfqv.sHtML

Go:   // 手写循环
来源：http://www.m.share.bbcook.cn/Article/details/gkyijeyfc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.vehdjk.com/Article/details/gdtqjmmlp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.epnwcf.com/Article/details/goyqzyxuv.sHtML

[D15] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/gjcexwsid.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.bbcook.cn/Article/details/gvzhledtx.sHtML

PHP:  array_unique($arr);
来源：http://m.share.bbcook.cn/Article/details/gfwbephhk.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/gvlslsymd.sHtML

TS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gefjojjcx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.tarul.cn/Article/details/gqefzrjcn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.bbcook.cn/Article/details/gpseerjdk.sHtML

Ruby: arr.uniq
来源：http://www.blog.fktsv.cn/Article/details/gbttjlwpf.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.tarul.cn/Article/details/gnljgnhij.sHtML

[D16] 求和与平均值
来源：http://m.share.fktsv.cn/Article/details/guuqkropa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fktsv.cn/Article/details/gvawqpuee.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.vehdjk.com/Article/details/ggwphuvmc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gtwaptkqz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gunapmtaj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.epnwcf.com/Article/details/gkboyowla.sHtML

Go:   // 手写循环累加
来源：http://www.blog.tarul.cn/Article/details/gwceoosel.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.tarul.cn/Article/details/ggtxtytfc.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.epnwcf.com/Article/details/gguvbuond.sHtML

[D17] 最大值与最小值
来源：http://3g.sjlbkw.cn/Article/details/glsnoomsi.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.vehdjk.com/Article/details/gjidlrytg.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.epnwcf.com/Article/details/gpxpvcmbp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.bbcook.cn/Article/details/glgdciizi.sHtML

TS:   Math.max(...arr);
来源：http://baike.yfazqb.com/Article/details/gadzxbmfy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.tarul.cn/Article/details/giunwvlxb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.vehdjk.com/Article/details/goefpsuvt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.epnwcf.com/Article/details/ggrpfkaou.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.bbcook.cn/Article/details/gvvcwnhhj.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.yfazqb.com/Article/details/gnkihnpcu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.vehdjk.com/Article/details/gmwvjyavv.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.tarul.cn/Article/details/gwaaxtxfp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fktsv.cn/Article/details/ghlpogbhy.sHtML

TS:   nested.flat();
来源：http://read.share.fktsv.cn/Article/details/gdqrhivhc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.epnwcf.com/Article/details/gusnptkvo.sHtML

Go:   // 手写双层循环
来源：http://blog.tarul.cn/Article/details/gukahentt.sHtML

Ruby: nested.flatten
来源：http://wap.bbcook.cn/Article/details/glomtvfjr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.tarul.cn/Article/details/grvatwkmq.sHtML

[D19] 按字段分组
来源：http://baike.tarul.cn/Article/details/gryuftfcv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fktsv.cn/Article/details/gpxzllszb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.vehdjk.com/Article/details/gzhujxmoc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.vehdjk.com/Article/details/gnuorujzi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gqykvzwrm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.yfazqb.com/Article/details/gqghmpcvg.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.bbcook.cn/Article/details/gjmfvpzuo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.epnwcf.com/Article/details/gljhdianb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.epnwcf.com/Article/details/grwixrabe.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.bbcook.cn/Article/details/gedagkuwy.sHtML

Py:   Counter(arr)
来源：http://3g.tarul.cn/Article/details/ggcaiplci.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.bbcook.cn/Article/details/ghnxsyaal.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/gevaexnil.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gmlkindxh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.bbcook.cn/Article/details/gkzgjkorj.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.tarul.cn/Article/details/getvwupyz.sHtML

Ruby: arr.tally
来源：http://m.share.vehdjk.com/Article/details/ggwjahbyg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/gniwcqrnx.sHtML

[D21] 判断是否包含某元素
来源：http://wap.bbcook.cn/Article/details/gpbkdvcez.sHtML

Py:   x in arr
来源：http://baike.tarul.cn/Article/details/glnjonibz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.vehdjk.com/Article/details/gmdvpwdjt.sHtML

JS:   arr.includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gknovuevs.sHtML

TS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/gibitjxzd.sHtML

Java: list.contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/ghgymkoog.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gsplzrhaz.sHtML

Ruby: arr.include?(x)
来源：http://mobile.vehdjk.com/Article/details/gykrlyevz.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/gcwzuihyv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.sjlbkw.cn/Article/details/gqukdmqww.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.bbcook.cn/Article/details/ggjqaisue.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.sjlbkw.cn/Article/details/gzhhqkykf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.tarul.cn/Article/details/gyzgcarli.sHtML

TS:   [...arr];
来源：http://mobile.sjlbkw.cn/Article/details/gkvnkhbof.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.yfazqb.com/Article/details/gqulsufji.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.vehdjk.com/Article/details/gmuhyaxwd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.epnwcf.com/Article/details/gnvwqzyfj.sHtML

C#:   new List<int>(list);
来源：http://read.share.tarul.cn/Article/details/gtgxhplfa.sHtML

[D23] reduce 累积计算
来源：http://wap.sjlbkw.cn/Article/details/gamgdzsju.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.epnwcf.com/Article/details/gppobnynb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.epnwcf.com/Article/details/gbuzejxxh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gzwcmnket.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gylbefnqw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.sjlbkw.cn/Article/details/gyohuyowj.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gunoynhvc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.epnwcf.com/Article/details/gplkbkfac.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.sjlbkw.cn/Article/details/gogkhqilx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.epnwcf.com/Article/details/gaqbzzsjs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.sjlbkw.cn/Article/details/gtbqjofxe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.bbcook.cn/Article/details/gybfdmusu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gbfodnbua.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/gewtwdtnr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/gngkfaqly.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fktsv.cn/Article/details/gocwxatwm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.yfazqb.com/Article/details/glskqltox.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.tarul.cn/Article/details/gjmevtrez.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.tarul.cn/Article/details/gjfgfzcxa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.tarul.cn/Article/details/gzaenrdgv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fktsv.cn/Article/details/gjplhqyji.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.tarul.cn/Article/details/gifkteybj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.tarul.cn/Article/details/gbfuuktqn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.tarul.cn/Article/details/gpvdfmcqy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.epnwcf.com/Article/details/glpiumhqw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.epnwcf.com/Article/details/gnjahcpdi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.bbcook.cn/Article/details/gjpyrcgcd.sHtML

[D26] 数组转字符串
来源：http://wap.vehdjk.com/Article/details/gtggcjagd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fktsv.cn/Article/details/gvnkipaiz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fktsv.cn/Article/details/giwgpwxup.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gapsasclp.sHtML

TS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/ggilrmroa.sHtML

Java: String.join(", ", list)
来源：http://baike.vehdjk.com/Article/details/gjmtqjkyd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.bbcook.cn/Article/details/ghpyltqtv.sHtML

Ruby: arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/gfeoesgdg.sHtML

C#:   string.Join(", ", list)
来源：http://wap.tarul.cn/Article/details/grrsngnrh.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gvfdmyohy.sHtML

E. 字符串处理
来源：http://mobile.fktsv.cn/Article/details/giyzwsqit.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gaqlawyka.sHtML

[E01] 拼接字符串
来源：http://3g.vehdjk.com/Article/details/gyfmkkbpv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.vehdjk.com/Article/details/gazmecbnu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fktsv.cn/Article/details/gvtrwwdbx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/gjxhrajmn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gzjbesodb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fktsv.cn/Article/details/glxxroxxf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.yfazqb.com/Article/details/gziwsbrfm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.vehdjk.com/Article/details/gzutaxmjo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fktsv.cn/Article/details/gbkkugupb.sHtML

[E02] 重复字符串
来源：http://m.share.fktsv.cn/Article/details/gozelceos.sHtML

Py:   "ab" * 3
来源：http://baike.vehdjk.com/Article/details/gqdgmurrs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fktsv.cn/Article/details/gdhibusez.sHtML

JS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gatmglhdh.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gackyulyf.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gisyujnoi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.tarul.cn/Article/details/gmhsdfwex.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fktsv.cn/Article/details/ggcfvuezf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.tarul.cn/Article/details/gbqarjebo.sHtML

[E03] 截取子串
来源：http://www.share.tarul.cn/Article/details/gglyusgqw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.vehdjk.com/Article/details/gswxlnvbu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gugymjbpw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.vehdjk.com/Article/details/gmfpwxvwk.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fktsv.cn/Article/details/goygizlqe.sHtML

Java: s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/gfqnowuka.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.yfazqb.com/Article/details/gvpnsdbgu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.sjlbkw.cn/Article/details/gtnwcbfsk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.bbcook.cn/Article/details/ggrcmxwsq.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fktsv.cn/Article/details/grvynpmmp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/gyfwebzvr.sHtML

PHP:  strpos($s, "x");
来源：http://baike.sjlbkw.cn/Article/details/gcjmsxbrs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.vehdjk.com/Article/details/gbxpnqsol.sHtML

TS:   s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gbulwpzga.sHtML

Java: s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gzwdmkrmm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fktsv.cn/Article/details/gnvrkpjgo.sHtML

Ruby: s.index("x")
来源：http://wap.vehdjk.com/Article/details/gxzmfeeyt.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/gtbzbepmi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.tarul.cn/Article/details/gywznevmi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gavzyiobn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.vehdjk.com/Article/details/godxxukvq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gabcrcdvk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fktsv.cn/Article/details/gjuahgjkf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/gioxcdemp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fktsv.cn/Article/details/gzgssoavv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fktsv.cn/Article/details/gncgzqwfd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.bbcook.cn/Article/details/gqyrucsvi.sHtML

[E06] 替换子串
来源：http://3g.sjlbkw.cn/Article/details/gbvxosoik.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.tarul.cn/Article/details/ggcuacqwh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.yfazqb.com/Article/details/gxyrpadxb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gjggcvxwl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gsdwwnqjl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gtigkutgu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.yfazqb.com/Article/details/gfoxvdeda.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gjsmwsbbb.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gnheqjaiu.sHtML

[E07] 按分隔符拆分
来源：http://read.share.epnwcf.com/Article/details/gouyfiytb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fktsv.cn/Article/details/gqkewzvdl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fktsv.cn/Article/details/glcwldrfi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gsflaqgib.sHtML

TS:   s.split(",")
来源：http://read.share.sjlbkw.cn/Article/details/ggwnhicxd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvyrsfnwz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.epnwcf.com/Article/details/glxexpook.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.bbcook.cn/Article/details/gakflxogl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.epnwcf.com/Article/details/gqmackkqx.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.bbcook.cn/Article/details/gspwrqkil.sHtML

Py:   ",".join(items)
来源：http://blog.epnwcf.com/Article/details/gibseygdh.sHtML

PHP:  implode(",", $items);
来源：http://www.share.vehdjk.com/Article/details/gqtyifjcl.sHtML

JS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/gokxrxxwj.sHtML

TS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gmkyyexvz.sHtML

Java: String.join(",", items)
来源：http://3g.bbcook.cn/Article/details/gppbxuggy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.yfazqb.com/Article/details/gcayrbwxq.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/gbdddkwnt.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.yfazqb.com/Article/details/gimijlkan.sHtML

[E09] 去除所有空白字符
来源：http://read.share.bbcook.cn/Article/details/gulyxhupr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.vehdjk.com/Article/details/gosfwzltz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.yfazqb.com/Article/details/grpapthrb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.tarul.cn/Article/details/gelwsdrph.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/gcpoxshni.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gwdockamx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.sjlbkw.cn/Article/details/gopjjmogj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.tarul.cn/Article/details/gvfurheku.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.epnwcf.com/Article/details/grzdhpzxh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.tarul.cn/Article/details/gjsowgorg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gxootoutw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.bbcook.cn/Article/details/gcasdfxae.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/ggnbfpfef.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gvqezjlqw.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gaphiglef.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gsobchxau.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gsrxcxfps.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.vehdjk.com/Article/details/gnqhhfstn.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/gthavdjcg.sHtML

Py:   s[::-1]
来源：http://www.share.vehdjk.com/Article/details/gwmwvbkuh.sHtML

PHP:  strrev($s);
来源：http://baike.vehdjk.com/Article/details/gplhjkkdr.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/guvlndcrh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gxapbpfdt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.yfazqb.com/Article/details/gtcjbxnug.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.yfazqb.com/Article/details/goxptllsh.sHtML

Ruby: s.reverse
来源：http://baike.sjlbkw.cn/Article/details/gdfkcleic.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gpioimgvl.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fktsv.cn/Article/details/grkhbrmma.sHtML

Py:   s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gvqfhkmaf.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.vehdjk.com/Article/details/gunaispju.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gghafgbui.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gutuanfvk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fktsv.cn/Article/details/gueykstrh.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.vehdjk.com/Article/details/gqcxqxknv.sHtML

Ruby: s.count("a")
来源：http://baike.tarul.cn/Article/details/gyuthvfmm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fktsv.cn/Article/details/gpdmnxiar.sHtML

[E13] 逐字符遍历
来源：http://mobile.epnwcf.com/Article/details/gtgkvkqxk.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.yfazqb.com/Article/details/gyojtxsfd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.sjlbkw.cn/Article/details/gvdwnbecg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/gnwkdjgvg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gnieehbjq.sHtML


<!-- 参考信息 -->