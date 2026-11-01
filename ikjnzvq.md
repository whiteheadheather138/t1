代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/geoeiymim.sHtML

Java: list.subList(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gokvzgorl.sHtML

Go:   arr[1:4]
来源：http://mobile.bbcook.cn/Article/details/goepyzjcg.sHtML

Ruby: arr[1, 3]
来源：http://www.share.epnwcf.com/Article/details/girkmtuck.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fktsv.cn/Article/details/glcdivakb.sHtML

[D08] 合并两个数组
来源：http://m.share.epnwcf.com/Article/details/gtpjmkoer.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.bbcook.cn/Article/details/gfraqrpca.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvoqmchl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.epnwcf.com/Article/details/gjndiwlgo.sHtML

TS:   [...a, ...b];
来源：http://wap.yfazqb.com/Article/details/gmnuljrbz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.tarul.cn/Article/details/gkhclnycc.sHtML

Go:   append(a, b...)
来源：http://www.blog.yfazqb.com/Article/details/ghxpphscu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.yfazqb.com/Article/details/guvwgndup.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gingonuxp.sHtML

[D09] 排序（升序）
来源：http://blog.epnwcf.com/Article/details/gzuwlwalo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/geqxwinto.sHtML

PHP:  sort($arr);
来源：http://www.share.sjlbkw.cn/Article/details/ghxdapviy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.sjlbkw.cn/Article/details/gsosyalpv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gyvcrktam.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fktsv.cn/Article/details/gozyhvrek.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/gfywcqmov.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/geuvucons.sHtML

C#:   list.Sort();
来源：http://mobile.epnwcf.com/Article/details/ggfkdjjbv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fktsv.cn/Article/details/gpiexhgte.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.vehdjk.com/Article/details/gemtaltvu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/gngtcsjtr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/glwdrxwic.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gwbgjopbo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.bbcook.cn/Article/details/gwytfdqxh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.bbcook.cn/Article/details/grmekmtni.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.tarul.cn/Article/details/gzpnpoevc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.bbcook.cn/Article/details/gxmcpbyeq.sHtML

[D11] 反转数组
来源：http://www.share.sjlbkw.cn/Article/details/ggoomtxjn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.yfazqb.com/Article/details/gfklzxdmr.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.vehdjk.com/Article/details/gxhyolrrf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fktsv.cn/Article/details/gpkttbrxb.sHtML

TS:   [...arr].reverse();
来源：http://wap.sjlbkw.cn/Article/details/gkharuscv.sHtML

Java: Collections.reverse(list);
来源：http://baike.yfazqb.com/Article/details/gbfcyiwzv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.vehdjk.com/Article/details/gvnwzwqtd.sHtML

Ruby: arr.reverse
来源：http://baike.fktsv.cn/Article/details/gsfzpucvm.sHtML

C#:   list.Reverse();
来源：http://blog.bbcook.cn/Article/details/gmfjodtnd.sHtML

[D12] 查找元素下标
来源：http://www.share.epnwcf.com/Article/details/gizevzdof.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.tarul.cn/Article/details/gtofkorpo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fktsv.cn/Article/details/gfikrrspr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.epnwcf.com/Article/details/gdugophpl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/gtcsmcuzi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fktsv.cn/Article/details/gnqasmngt.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fktsv.cn/Article/details/gjjyaaqbn.sHtML

Ruby: arr.index(x)
来源：http://mobile.vehdjk.com/Article/details/gyenxefdo.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.vehdjk.com/Article/details/ggeiamejh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.epnwcf.com/Article/details/gupsiuovj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.tarul.cn/Article/details/gwzyhlbjf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.epnwcf.com/Article/details/gcemvixtz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gjjhnwkqe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gbwxtvslv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.tarul.cn/Article/details/grymevusf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.bbcook.cn/Article/details/goaqtnrgv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdxcdwny.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gzxqttiwd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.epnwcf.com/Article/details/gogphhiyz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.epnwcf.com/Article/details/glxbkjbnq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.bbcook.cn/Article/details/ggkzhaole.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gjwejywii.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/ggjxlkohh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/ghislgmxw.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/gbpgxlodw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.yfazqb.com/Article/details/giewzyxsx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gjibfhkrj.sHtML

[D15] 去重
来源：http://www.blog.tarul.cn/Article/details/gdgzrqzjr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/ghvuwtsal.sHtML

PHP:  array_unique($arr);
来源：http://wap.fktsv.cn/Article/details/gkfpfdnrq.sHtML

JS:   [...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/ghhypwdnh.sHtML

TS:   [...new Set(arr)]
来源：http://blog.yfazqb.com/Article/details/gbsgyrxof.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.sjlbkw.cn/Article/details/gwcshwkaa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.tarul.cn/Article/details/gzqvrosvr.sHtML

Ruby: arr.uniq
来源：http://baike.yfazqb.com/Article/details/geaeshjhd.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fktsv.cn/Article/details/gwxjqsvri.sHtML

[D16] 求和与平均值
来源：http://mobile.tarul.cn/Article/details/gylkgrkqn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gvonogbqa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fktsv.cn/Article/details/gkgihcdbw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gorphucej.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gdoxmwxsx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.bbcook.cn/Article/details/gbmgqwykp.sHtML

Go:   // 手写循环累加
来源：http://blog.sjlbkw.cn/Article/details/gjjgcabcd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fktsv.cn/Article/details/gkvcbqzhn.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/gdccgrrta.sHtML

[D17] 最大值与最小值
来源：http://m.share.epnwcf.com/Article/details/gqjwrundr.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fktsv.cn/Article/details/gyildernh.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.yfazqb.com/Article/details/ggsmzijwp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.yfazqb.com/Article/details/ghvfdqqml.sHtML

TS:   Math.max(...arr);
来源：http://wap.yfazqb.com/Article/details/gijzecogp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.vehdjk.com/Article/details/gydrojbyq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.bbcook.cn/Article/details/gpzsfnjaf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fktsv.cn/Article/details/geocqqwqg.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.yfazqb.com/Article/details/glwobxqzz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fktsv.cn/Article/details/gxcqirmcw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.tarul.cn/Article/details/gqtfqibwv.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/grgoupxsq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.bbcook.cn/Article/details/grrxtzkjm.sHtML

TS:   nested.flat();
来源：http://m.share.fktsv.cn/Article/details/giwpaizyr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.bbcook.cn/Article/details/gbhuwsltp.sHtML

Go:   // 手写双层循环
来源：http://mobile.tarul.cn/Article/details/gzunruppe.sHtML

Ruby: nested.flatten
来源：http://blog.yfazqb.com/Article/details/gcxguazsb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gdrfsuloo.sHtML

[D19] 按字段分组
来源：http://m.share.epnwcf.com/Article/details/gvmmuwczy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fktsv.cn/Article/details/goztbqazg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.tarul.cn/Article/details/gexidpckq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.sjlbkw.cn/Article/details/gixjjurim.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gwtpndmlw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fktsv.cn/Article/details/gkurqqnrf.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.vehdjk.com/Article/details/gerdpzawf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.epnwcf.com/Article/details/gykespseo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.sjlbkw.cn/Article/details/gpkbakmrq.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fktsv.cn/Article/details/gavwkuquq.sHtML

Py:   Counter(arr)
来源：http://mobile.epnwcf.com/Article/details/gzpklfrba.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.vehdjk.com/Article/details/gybumvatu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/geuuirmrr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.yfazqb.com/Article/details/gbaizvgzw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.vehdjk.com/Article/details/gvlbfbjal.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fktsv.cn/Article/details/gzuioarev.sHtML

Ruby: arr.tally
来源：http://wap.vehdjk.com/Article/details/gnbtktnpv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.yfazqb.com/Article/details/gwkpawbmi.sHtML

[D21] 判断是否包含某元素
来源：http://baike.tarul.cn/Article/details/grxhcvmih.sHtML

Py:   x in arr
来源：http://read.share.fktsv.cn/Article/details/glnyvgfol.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.vehdjk.com/Article/details/gieeolzbh.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gxjkkcdny.sHtML

TS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/gthhqvngc.sHtML

Java: list.contains(x)
来源：http://www.share.fktsv.cn/Article/details/gpvmfwdll.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.yfazqb.com/Article/details/gwtxgzcdq.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.bbcook.cn/Article/details/guewftrvo.sHtML

C#:   list.Contains(x)
来源：http://blog.fktsv.cn/Article/details/gqepmmosx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.vehdjk.com/Article/details/gqyrcgumf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.yfazqb.com/Article/details/gafhhaaws.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.bbcook.cn/Article/details/gwbbqpsxf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.tarul.cn/Article/details/gfwqevokk.sHtML

TS:   [...arr];
来源：http://mobile.yfazqb.com/Article/details/ggscdrwsr.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.yfazqb.com/Article/details/gsbqyzdwv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.epnwcf.com/Article/details/gcymdnukc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.epnwcf.com/Article/details/glvvfosfd.sHtML

C#:   new List<int>(list);
来源：http://baike.bbcook.cn/Article/details/gtwvaqxkr.sHtML

[D23] reduce 累积计算
来源：http://3g.sjlbkw.cn/Article/details/gwiksjiyv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.yfazqb.com/Article/details/gcsnzdzle.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.tarul.cn/Article/details/gazceeyjz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/gmmuqtnyb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/girljqggq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fktsv.cn/Article/details/gxurmkljm.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/gfuerleil.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.epnwcf.com/Article/details/gtufhjvmd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fktsv.cn/Article/details/gwzbhzqoz.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fktsv.cn/Article/details/gtsqbusdc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.vehdjk.com/Article/details/gkfqgiyxw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.sjlbkw.cn/Article/details/gzkptjurp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.tarul.cn/Article/details/gzqcfdfpc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gismwxxdt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.yfazqb.com/Article/details/gyecvtpth.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fktsv.cn/Article/details/gwcqjydkr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.sjlbkw.cn/Article/details/gytmqivug.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fktsv.cn/Article/details/gmaphdyjt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.yfazqb.com/Article/details/gtqzvafgo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.yfazqb.com/Article/details/gemnvymlh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.epnwcf.com/Article/details/gghefkhua.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fktsv.cn/Article/details/gjtpkxygi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fktsv.cn/Article/details/gdooycckk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fktsv.cn/Article/details/gvwdfbnel.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gmsrdtbke.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.yfazqb.com/Article/details/gjorfjisj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fktsv.cn/Article/details/guniirmkk.sHtML

[D26] 数组转字符串
来源：http://mobile.bbcook.cn/Article/details/gvmufzikc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fktsv.cn/Article/details/gtkindbkb.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.epnwcf.com/Article/details/gtzwemcuy.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/greeejulu.sHtML

TS:   arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gsexdwlsh.sHtML

Java: String.join(", ", list)
来源：http://mobile.fktsv.cn/Article/details/gbynigxyx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.bbcook.cn/Article/details/gacmeftzx.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gckastpkq.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.yfazqb.com/Article/details/gpaqxqgae.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/grcoxiewf.sHtML

E. 字符串处理
来源：http://3g.bbcook.cn/Article/details/gmowmupit.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gohgukzos.sHtML

[E01] 拼接字符串
来源：http://read.share.epnwcf.com/Article/details/ggnyhqjsn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.tarul.cn/Article/details/gzsfpbupl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.vehdjk.com/Article/details/gpfpsxpcn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.sjlbkw.cn/Article/details/gnwkrrxeo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.sjlbkw.cn/Article/details/gxznutmkt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.yfazqb.com/Article/details/gmjhtpfxr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fktsv.cn/Article/details/gaoytviue.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.vehdjk.com/Article/details/gjqjzvwus.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gzljgycoc.sHtML

[E02] 重复字符串
来源：http://wap.epnwcf.com/Article/details/gouqmveru.sHtML

Py:   "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/glwagphip.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.vehdjk.com/Article/details/goneskvjo.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/glpscbdlm.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/ggheicdif.sHtML

Java: "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gkjtsspnk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.yfazqb.com/Article/details/gcdlvlbhd.sHtML

Ruby: "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gsasofgae.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.epnwcf.com/Article/details/giskljqju.sHtML

[E03] 截取子串
来源：http://m.share.epnwcf.com/Article/details/glbaufmlg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.bbcook.cn/Article/details/gnfprjomd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gorfcocwo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.vehdjk.com/Article/details/gkoyzgrne.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gfhzfndxs.sHtML

Java: s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/ggwomvqaq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.tarul.cn/Article/details/ggtoybayr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.epnwcf.com/Article/details/gqxkvphhf.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.bbcook.cn/Article/details/ghkahfyfb.sHtML

[E04] 查找子串位置
来源：http://baike.bbcook.cn/Article/details/gyyzkgmhy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/givzjoqly.sHtML

PHP:  strpos($s, "x");
来源：http://wap.epnwcf.com/Article/details/gmvaucmzz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fktsv.cn/Article/details/gvfarpivu.sHtML

TS:   s.indexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gxqcezozd.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/ghjtjflsz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.vehdjk.com/Article/details/gxlafygoc.sHtML

Ruby: s.index("x")
来源：http://read.share.epnwcf.com/Article/details/gtcmgqjsm.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/glxrywljo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.yfazqb.com/Article/details/gtznppisi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.sjlbkw.cn/Article/details/gtnnhzjht.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fktsv.cn/Article/details/gzqyjhuwp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.epnwcf.com/Article/details/gufqaeibv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.vehdjk.com/Article/details/gfkjwmvrz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.yfazqb.com/Article/details/glzelvrab.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.vehdjk.com/Article/details/gvifznqrb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.tarul.cn/Article/details/gmaltfsdf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.bbcook.cn/Article/details/gflfbunai.sHtML

[E06] 替换子串
来源：http://www.m.share.yfazqb.com/Article/details/geyszxazk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gqnjoqsdk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.yfazqb.com/Article/details/gwecbgcbh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gbtizeqvm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gpqsttlzc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gbrghkbei.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gmeoehcfe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.bbcook.cn/Article/details/glzzkmztf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gfsnxnczy.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/gzyfepite.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.sjlbkw.cn/Article/details/gvkbqdaku.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.bbcook.cn/Article/details/ggkizpeth.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.bbcook.cn/Article/details/gekqyjlik.sHtML

TS:   s.split(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqixrczy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.epnwcf.com/Article/details/gwtfhqayx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fktsv.cn/Article/details/gucqadgmj.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fktsv.cn/Article/details/gtbcucbdn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.epnwcf.com/Article/details/gpuwinhwo.sHtML

[E08] 数组按分隔符合并
来源：http://baike.epnwcf.com/Article/details/gezbsaqeu.sHtML

Py:   ",".join(items)
来源：http://3g.yfazqb.com/Article/details/gexgfyjqw.sHtML

PHP:  implode(",", $items);
来源：http://www.share.tarul.cn/Article/details/gmshaztym.sHtML

JS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gkpygjnxz.sHtML

TS:   items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gdprxlyeb.sHtML

Java: String.join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gxbejtpyk.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.bbcook.cn/Article/details/gunoozoab.sHtML

Ruby: items.join(",")
来源：http://baike.epnwcf.com/Article/details/gtkikdjyu.sHtML

C#:   string.Join(",", items)
来源：http://wap.epnwcf.com/Article/details/gvkiesgkr.sHtML

[E09] 去除所有空白字符
来源：http://www.share.yfazqb.com/Article/details/gcutnqxdh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.yfazqb.com/Article/details/gndpolqxt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.bbcook.cn/Article/details/gtkxbnwey.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/goteomhjg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/gtzqjdxen.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fktsv.cn/Article/details/gcjjgtptd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.tarul.cn/Article/details/gsvhvcgbf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.yfazqb.com/Article/details/gyseidgav.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.epnwcf.com/Article/details/gtvudjszi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fktsv.cn/Article/details/gsxfqtaoi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gqvzmpbkt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.vehdjk.com/Article/details/gzbkddbca.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gnszuhazl.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gypnpmgfj.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/grpkesqkv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gvcscyfgo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gvfgdntjb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fktsv.cn/Article/details/geqblfbbs.sHtML

[E11] 反转字符串
来源：http://blog.tarul.cn/Article/details/grpagmueo.sHtML

Py:   s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gknnlrtda.sHtML

PHP:  strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/geqljmjcz.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/giltugzga.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gkgndonov.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gljknprup.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.epnwcf.com/Article/details/gwrixezix.sHtML

Ruby: s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gndljjwuy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gbtjrlvqb.sHtML

[E12] 统计某字符出现次数
来源：http://wap.tarul.cn/Article/details/ghplrecuq.sHtML

Py:   s.count("a")
来源：http://3g.vehdjk.com/Article/details/ghxnqekev.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.vehdjk.com/Article/details/guwngxdwo.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.bbcook.cn/Article/details/gtnpyxsia.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gublcijxr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.epnwcf.com/Article/details/gcgsemiuc.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.tarul.cn/Article/details/gmsadbhyo.sHtML

Ruby: s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gtrfavwfe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fktsv.cn/Article/details/gndovcxsh.sHtML

[E13] 逐字符遍历
来源：http://mobile.tarul.cn/Article/details/gcqvatpdr.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/gydajlxff.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.tarul.cn/Article/details/gfhsqahdr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gzuctcoyx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/ggkugraha.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/giyzfitls.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.bbcook.cn/Article/details/gqalidqfx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.vehdjk.com/Article/details/gldbcfldw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gdjpfyrxz.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.yfazqb.com/Article/details/gluvhatnk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.vehdjk.com/Article/details/gtynwksxo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.yfazqb.com/Article/details/gpwzssvih.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.sjlbkw.cn/Article/details/grpqaywyb.sHtML


<!-- 参考信息 -->