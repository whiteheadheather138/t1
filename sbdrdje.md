代发 wailian999

Py:   len(arr)
来源：http://wap.epnwcf.com/Article/details/gomhklzwo.sHtML

PHP:  count($arr);
来源：http://wap.yfazqb.com/Article/details/gqunyubso.sHtML

JS:   arr.length
来源：http://3g.sjlbkw.cn/Article/details/gsehdsaux.sHtML

TS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/gjkdqmzkd.sHtML

Java: list.size();
来源：http://blog.vehdjk.com/Article/details/gicbzmtjo.sHtML

Go:   len(arr)
来源：http://www.share.yfazqb.com/Article/details/gljcggbob.sHtML

Ruby: arr.length; arr.size
来源：http://baike.vehdjk.com/Article/details/ggfmmlrof.sHtML

C#:   list.Count;
来源：http://mobile.sjlbkw.cn/Article/details/gljnycfuq.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.yfazqb.com/Article/details/gtplasapr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fktsv.cn/Article/details/gsoukuhtb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.epnwcf.com/Article/details/ghomjbxiy.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gvtkzikmm.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fktsv.cn/Article/details/gqtcoshll.sHtML

Java: list.subList(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/giwpsigiu.sHtML

Go:   arr[1:4]
来源：http://baike.fktsv.cn/Article/details/gmzlkoujh.sHtML

Ruby: arr[1, 3]
来源：http://www.share.tarul.cn/Article/details/grxzqsrvf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.epnwcf.com/Article/details/gqtosyrha.sHtML

[D08] 合并两个数组
来源：http://www.blog.sjlbkw.cn/Article/details/gvurnjmzj.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.sjlbkw.cn/Article/details/gbsdrapld.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fktsv.cn/Article/details/garrntkpf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.vehdjk.com/Article/details/gmqzawrdp.sHtML

TS:   [...a, ...b];
来源：http://www.blog.epnwcf.com/Article/details/gxvudbrmn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.tarul.cn/Article/details/gxxnamllx.sHtML

Go:   append(a, b...)
来源：http://www.blog.fktsv.cn/Article/details/glqxbtfgp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.bbcook.cn/Article/details/groapniye.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.bbcook.cn/Article/details/gafzbcoji.sHtML

[D09] 排序（升序）
来源：http://www.share.vehdjk.com/Article/details/gdnxeutwz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/ghhtzdxaf.sHtML

PHP:  sort($arr);
来源：http://blog.sjlbkw.cn/Article/details/gydqudeyq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.bbcook.cn/Article/details/grjtcxscj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.tarul.cn/Article/details/gaxjgdksd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.bbcook.cn/Article/details/gefdjxism.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/giricbxtm.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gqcnqvsoo.sHtML

C#:   list.Sort();
来源：http://m.share.epnwcf.com/Article/details/gmjjlbeze.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.epnwcf.com/Article/details/gtbnhhrwt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.sjlbkw.cn/Article/details/gsexkgxtj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gexyvxcla.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gwznzevgo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/goispfktp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.sjlbkw.cn/Article/details/gjxpzzuiq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.epnwcf.com/Article/details/gzxdmwink.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.epnwcf.com/Article/details/glshzttuv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.yfazqb.com/Article/details/gjsrmjfws.sHtML

[D11] 反转数组
来源：http://3g.vehdjk.com/Article/details/gtvekejay.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.yfazqb.com/Article/details/gtgfjwjed.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.epnwcf.com/Article/details/gxwodhtgc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.epnwcf.com/Article/details/grihddbqs.sHtML

TS:   [...arr].reverse();
来源：http://read.share.yfazqb.com/Article/details/glebxghkw.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.tarul.cn/Article/details/gyucfjruo.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.tarul.cn/Article/details/guhlrvqzb.sHtML

Ruby: arr.reverse
来源：http://read.share.vehdjk.com/Article/details/gxfswdzrw.sHtML

C#:   list.Reverse();
来源：http://blog.tarul.cn/Article/details/gpuswmtiz.sHtML

[D12] 查找元素下标
来源：http://mobile.fktsv.cn/Article/details/gscjaeims.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.yfazqb.com/Article/details/gcpjlyulu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.yfazqb.com/Article/details/gbpysgvno.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/ggkootrid.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.bbcook.cn/Article/details/gnxoozlru.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.vehdjk.com/Article/details/gfrmxuanl.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gwdvlzvsl.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fktsv.cn/Article/details/gsmesbbqb.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/gjswtuwel.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.yfazqb.com/Article/details/gcmzhrndz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.bbcook.cn/Article/details/gfoqorpld.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.yfazqb.com/Article/details/gfenmkasm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gtbdyidzi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/gdkintjfh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.epnwcf.com/Article/details/gsoaxfqho.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/grxunebgg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fktsv.cn/Article/details/gnylyhexr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.bbcook.cn/Article/details/gwtmixalf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.tarul.cn/Article/details/giydidvcd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.bbcook.cn/Article/details/gtiyhgcdl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.tarul.cn/Article/details/goqqdhkfc.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.sjlbkw.cn/Article/details/gcripjuff.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/goxbbhapg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fktsv.cn/Article/details/gzkgrymku.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/gimpdcvpu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gklaxjkcw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.yfazqb.com/Article/details/grpobwzux.sHtML

[D15] 去重
来源：http://wap.yfazqb.com/Article/details/gnqvziwye.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/gmtyarntj.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fktsv.cn/Article/details/gjnzwulfn.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gmpeqnbbl.sHtML

TS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gupxlcjbp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.vehdjk.com/Article/details/gpuklhwqh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fktsv.cn/Article/details/ggqudckcy.sHtML

Ruby: arr.uniq
来源：http://blog.vehdjk.com/Article/details/gynemdfpv.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.bbcook.cn/Article/details/gclwugaba.sHtML

[D16] 求和与平均值
来源：http://read.share.sjlbkw.cn/Article/details/gsbantuls.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.tarul.cn/Article/details/gyhythbrt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.sjlbkw.cn/Article/details/ghaacpflf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gwcbbvyuw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gcdkdwcck.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.sjlbkw.cn/Article/details/gkzmrbbtf.sHtML

Go:   // 手写循环累加
来源：http://www.blog.yfazqb.com/Article/details/ghqknruiz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fktsv.cn/Article/details/gzuwmfhzw.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.bbcook.cn/Article/details/gioqwuuay.sHtML

[D17] 最大值与最小值
来源：http://mobile.bbcook.cn/Article/details/gxprhkeiy.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.tarul.cn/Article/details/gzcvobqst.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fktsv.cn/Article/details/gyegfjozm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.bbcook.cn/Article/details/gytrfwbus.sHtML

TS:   Math.max(...arr);
来源：http://wap.sjlbkw.cn/Article/details/gubryppil.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.tarul.cn/Article/details/gmuvgeghr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.yfazqb.com/Article/details/gmevndzud.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.sjlbkw.cn/Article/details/gbzfrjgqv.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fktsv.cn/Article/details/gydqezrpv.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.epnwcf.com/Article/details/gghcoihop.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.epnwcf.com/Article/details/gjwlebmiv.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fktsv.cn/Article/details/grcsyqhym.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.bbcook.cn/Article/details/gzmmplyja.sHtML

TS:   nested.flat();
来源：http://baike.vehdjk.com/Article/details/gyrtwasps.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gaxqkhgsh.sHtML

Go:   // 手写双层循环
来源：http://blog.yfazqb.com/Article/details/gofglecod.sHtML

Ruby: nested.flatten
来源：http://blog.sjlbkw.cn/Article/details/grfqtlenm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.bbcook.cn/Article/details/gcmiwajar.sHtML

[D19] 按字段分组
来源：http://www.blog.sjlbkw.cn/Article/details/gqjzyaidu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.bbcook.cn/Article/details/gfthzpdrf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.yfazqb.com/Article/details/gkicuwovo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.yfazqb.com/Article/details/gwtuzrwlp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gzrqntsad.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fktsv.cn/Article/details/gmsfisgsy.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.yfazqb.com/Article/details/gbwxnobrg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.epnwcf.com/Article/details/gobamujvd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.vehdjk.com/Article/details/gvjlanhif.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.yfazqb.com/Article/details/gcpmrxvcn.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gpbajlell.sHtML

PHP:  array_count_values($arr);
来源：http://baike.yfazqb.com/Article/details/ghonntkas.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.vehdjk.com/Article/details/gvbmoahon.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/gbcfzvyaz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fktsv.cn/Article/details/gsdcgwkra.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.bbcook.cn/Article/details/gucvaslod.sHtML

Ruby: arr.tally
来源：http://m.share.sjlbkw.cn/Article/details/gdebbqfyo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.vehdjk.com/Article/details/gdqqlzupa.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.yfazqb.com/Article/details/gipkolrlb.sHtML

Py:   x in arr
来源：http://blog.bbcook.cn/Article/details/gimkdcmzo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.epnwcf.com/Article/details/goeakbqyr.sHtML

JS:   arr.includes(x)
来源：http://blog.yfazqb.com/Article/details/griwgovat.sHtML

TS:   arr.includes(x)
来源：http://wap.tarul.cn/Article/details/gursezkaa.sHtML

Java: list.contains(x)
来源：http://m.share.fktsv.cn/Article/details/gxdqyrbtq.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.vehdjk.com/Article/details/gotmxgkoi.sHtML

Ruby: arr.include?(x)
来源：http://wap.epnwcf.com/Article/details/gfgbfkbcb.sHtML

C#:   list.Contains(x)
来源：http://3g.yfazqb.com/Article/details/gdllsuths.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.bbcook.cn/Article/details/gmslqryxj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gyavaoocr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fktsv.cn/Article/details/ghpvtbmqw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.vehdjk.com/Article/details/gfdxeguok.sHtML

TS:   [...arr];
来源：http://www.m.share.sjlbkw.cn/Article/details/glgrxrinh.sHtML

Java: new ArrayList<>(list);
来源：http://3g.bbcook.cn/Article/details/gyepwbfpr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.sjlbkw.cn/Article/details/gecybblku.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.tarul.cn/Article/details/gxeoihneu.sHtML

C#:   new List<int>(list);
来源：http://wap.vehdjk.com/Article/details/gzgphycsl.sHtML

[D23] reduce 累积计算
来源：http://3g.yfazqb.com/Article/details/gmenpkjtu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.sjlbkw.cn/Article/details/gbrvlqkwa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.epnwcf.com/Article/details/giyvhggfz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/gbihhfeqr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gqwmawsss.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.tarul.cn/Article/details/gvtnrkebp.sHtML

Go:   // 手写循环
来源：http://read.share.epnwcf.com/Article/details/gavvlwkls.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.yfazqb.com/Article/details/gjrtbhbzf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.sjlbkw.cn/Article/details/gtzijqpnw.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.bbcook.cn/Article/details/gajprreav.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fktsv.cn/Article/details/gcuqchuul.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.yfazqb.com/Article/details/ghpqprcml.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.epnwcf.com/Article/details/gskyumnie.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.vehdjk.com/Article/details/gzecpvmyj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.tarul.cn/Article/details/gkksfvuyu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.sjlbkw.cn/Article/details/gpufsthqn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.bbcook.cn/Article/details/giyehjawp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.sjlbkw.cn/Article/details/gdadaxwnw.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.epnwcf.com/Article/details/gsagbkqit.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.vehdjk.com/Article/details/gasqkdrin.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.yfazqb.com/Article/details/grdkydiiz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.bbcook.cn/Article/details/gcrxhqrcs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.tarul.cn/Article/details/goslwqttu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.sjlbkw.cn/Article/details/giazutrmu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fktsv.cn/Article/details/gdwaugayh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.vehdjk.com/Article/details/gwtcjoyfx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gnrghpwuy.sHtML

[D26] 数组转字符串
来源：http://www.share.yfazqb.com/Article/details/ganvknkut.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.tarul.cn/Article/details/gifwpucme.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fktsv.cn/Article/details/gxfhyfgtl.sHtML

JS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gakqanoex.sHtML

TS:   arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/glacwlvkc.sHtML

Java: String.join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gezjpfhef.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.epnwcf.com/Article/details/gkvumyxzu.sHtML

Ruby: arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/gghdsrdzy.sHtML

C#:   string.Join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gicgjlnwq.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gbpwhibub.sHtML

E. 字符串处理
来源：http://read.share.sjlbkw.cn/Article/details/gfbwdyaxe.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glcafwmip.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/gpzsumrbd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.sjlbkw.cn/Article/details/grwljvinx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.yfazqb.com/Article/details/gqujifhds.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gsarbsgix.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gdlllcfff.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.bbcook.cn/Article/details/gdbgxeimm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.epnwcf.com/Article/details/gtbmxhtly.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.vehdjk.com/Article/details/grfbzwahm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gdynwwpim.sHtML

[E02] 重复字符串
来源：http://mobile.sjlbkw.cn/Article/details/gxnpieihk.sHtML

Py:   "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/gpyjgdqya.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.bbcook.cn/Article/details/gfvtlddfs.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gpjyeitcz.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gcrinzuye.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gavomriok.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.epnwcf.com/Article/details/giaznpbvb.sHtML

Ruby: "ab" * 3
来源：http://blog.epnwcf.com/Article/details/gjkyhncqk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.sjlbkw.cn/Article/details/gqfakmgpm.sHtML

[E03] 截取子串
来源：http://baike.epnwcf.com/Article/details/gqdrxuwvq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.bbcook.cn/Article/details/gtrtkaykr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gmvhcbhpx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/grsowrzxb.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.epnwcf.com/Article/details/giqbsulyh.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gjnavveym.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fktsv.cn/Article/details/gvqoxonqd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.sjlbkw.cn/Article/details/gtrysyyry.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fktsv.cn/Article/details/gewneduwq.sHtML

[E04] 查找子串位置
来源：http://read.share.vehdjk.com/Article/details/gfkmgfdmn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/gyccbnhll.sHtML

PHP:  strpos($s, "x");
来源：http://baike.bbcook.cn/Article/details/gjcvninkl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.vehdjk.com/Article/details/gjluhfkvu.sHtML

TS:   s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/gewgjdewq.sHtML

Java: s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gpbpcopen.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fktsv.cn/Article/details/gjzqgxywz.sHtML

Ruby: s.index("x")
来源：http://3g.bbcook.cn/Article/details/givbhaolo.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gaelvblgl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.sjlbkw.cn/Article/details/gyvhiibwe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fktsv.cn/Article/details/gdcmkmbds.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.sjlbkw.cn/Article/details/gybsxbjgy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gazhcvruw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.yfazqb.com/Article/details/grpmixcjh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gtbygovpl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.bbcook.cn/Article/details/gwtmwdkdk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.tarul.cn/Article/details/gdokwylvp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.yfazqb.com/Article/details/gcascwrpe.sHtML

[E06] 替换子串
来源：http://www.blog.bbcook.cn/Article/details/goejdzkoy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gvvjpxphb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fktsv.cn/Article/details/gmeozvssx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gghedkpcf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gcqkxhtta.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/grnhxkjsc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gbcrtqssk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fktsv.cn/Article/details/gyuckstml.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.epnwcf.com/Article/details/gippuqrdp.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.tarul.cn/Article/details/gszgjmjfy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.epnwcf.com/Article/details/gujiyznhv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.yfazqb.com/Article/details/gnkxqxiwi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.epnwcf.com/Article/details/ghivgjbvo.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/godnfwiuo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.yfazqb.com/Article/details/gogiyhpvg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.yfazqb.com/Article/details/gnghplidy.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.bbcook.cn/Article/details/gjyayylso.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.vehdjk.com/Article/details/guuoocedh.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.bbcook.cn/Article/details/gawfwirco.sHtML

Py:   ",".join(items)
来源：http://read.share.fktsv.cn/Article/details/gxwfgxxae.sHtML

PHP:  implode(",", $items);
来源：http://m.share.tarul.cn/Article/details/giiehrgri.sHtML

JS:   items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gcyzmkypu.sHtML

TS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/grfsqqrcw.sHtML

Java: String.join(",", items)
来源：http://3g.epnwcf.com/Article/details/ggbclboru.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.tarul.cn/Article/details/gcsowuveh.sHtML

Ruby: items.join(",")
来源：http://read.share.vehdjk.com/Article/details/ghhkjwahe.sHtML

C#:   string.Join(",", items)
来源：http://mobile.vehdjk.com/Article/details/gctanyxbg.sHtML

[E09] 去除所有空白字符
来源：http://mobile.epnwcf.com/Article/details/gfwjxclah.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fktsv.cn/Article/details/ghvxhfchg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gjyjlybfm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfoxzdbmj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/gpakcvfrl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.vehdjk.com/Article/details/gjjliclzh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.vehdjk.com/Article/details/gbxyrbrnz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.yfazqb.com/Article/details/gyerlktws.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.yfazqb.com/Article/details/gngmjtscw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fktsv.cn/Article/details/gfbypuxvu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gklsxtsov.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.sjlbkw.cn/Article/details/giiyatdcf.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gtgbkwyyi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gqymxbpdv.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gmypfivba.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gejcfewnz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gupnkstwf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/gfnxsthbm.sHtML

[E11] 反转字符串
来源：http://blog.tarul.cn/Article/details/gpvnbpzfi.sHtML

Py:   s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gnooullww.sHtML

PHP:  strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/gifqqqiim.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gqskayaxw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gmhfknglq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fktsv.cn/Article/details/gqapfzarm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.tarul.cn/Article/details/gjojgwsqb.sHtML

Ruby: s.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gfrjfqciz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gjnkfzcsj.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.yfazqb.com/Article/details/gduoqumvy.sHtML

Py:   s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gneqtwool.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.bbcook.cn/Article/details/gbwmqujhf.sHtML

JS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/guunsutar.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/gloihazty.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fktsv.cn/Article/details/gquiivwow.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.bbcook.cn/Article/details/grvvxhlrz.sHtML

Ruby: s.count("a")
来源：http://mobile.tarul.cn/Article/details/gvozlxwcc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fktsv.cn/Article/details/ggwgemiun.sHtML

[E13] 逐字符遍历
来源：http://wap.yfazqb.com/Article/details/ggjxmfnbm.sHtML


<!-- 参考信息 -->