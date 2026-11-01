代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/glskifvpq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gzbejxprj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gjpyofjuk.sHtML

[D06] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/guxkfydmp.sHtML

Py:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/gubmntmcc.sHtML

PHP:  count($arr);
来源：http://baike.fktsv.cn/Article/details/ggozlnskf.sHtML

JS:   arr.length
来源：http://www.share.fktsv.cn/Article/details/gyxddwdpr.sHtML

TS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/gftuzajha.sHtML

Java: list.size();
来源：http://read.share.tarul.cn/Article/details/gtihydvme.sHtML

Go:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gvksneejk.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.vehdjk.com/Article/details/gbwljyfto.sHtML

C#:   list.Count;
来源：http://3g.epnwcf.com/Article/details/gywqqwatr.sHtML

[D07] 切片 / 取子数组
来源：http://blog.tarul.cn/Article/details/goyfzraik.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.yfazqb.com/Article/details/guplungcv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.epnwcf.com/Article/details/grojoyyxz.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.yfazqb.com/Article/details/gwretkpbc.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gtxyxskfn.sHtML

Java: list.subList(1, 4);
来源：http://baike.fktsv.cn/Article/details/gtnmqxvma.sHtML

Go:   arr[1:4]
来源：http://3g.epnwcf.com/Article/details/gvjojxtnf.sHtML

Ruby: arr[1, 3]
来源：http://blog.vehdjk.com/Article/details/gryhqlvyb.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.yfazqb.com/Article/details/gmxuduqlb.sHtML

[D08] 合并两个数组
来源：http://www.share.yfazqb.com/Article/details/gobvyoifd.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.epnwcf.com/Article/details/gnioxpsag.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.epnwcf.com/Article/details/gmcvajvqk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.bbcook.cn/Article/details/gbdgajoto.sHtML

TS:   [...a, ...b];
来源：http://wap.fktsv.cn/Article/details/ghasmpfep.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.epnwcf.com/Article/details/geuzoadnh.sHtML

Go:   append(a, b...)
来源：http://3g.bbcook.cn/Article/details/gpbubzgye.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.yfazqb.com/Article/details/gycfszeht.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.vehdjk.com/Article/details/gwnaeykfd.sHtML

[D09] 排序（升序）
来源：http://3g.tarul.cn/Article/details/gomaektgx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/guskfcgfn.sHtML

PHP:  sort($arr);
来源：http://read.share.bbcook.cn/Article/details/grhbjbsta.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.bbcook.cn/Article/details/gmhczfzzw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.bbcook.cn/Article/details/gfpgjhumb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fktsv.cn/Article/details/ghlhtojrs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/gkaqdctmf.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gvzadtopa.sHtML

C#:   list.Sort();
来源：http://mobile.tarul.cn/Article/details/grfutggix.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.vehdjk.com/Article/details/gsaoammts.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.sjlbkw.cn/Article/details/gndadpqia.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/giuokzzro.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/ggajaivcf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gcjblctvm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.yfazqb.com/Article/details/gbnxvwsht.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.epnwcf.com/Article/details/gsdvcktyp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fktsv.cn/Article/details/gmgbtlafr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.epnwcf.com/Article/details/gvsismghn.sHtML

[D11] 反转数组
来源：http://blog.vehdjk.com/Article/details/ggfqogazl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.epnwcf.com/Article/details/gaxumjbgd.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.tarul.cn/Article/details/gtloxalfi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnohwjhjg.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fktsv.cn/Article/details/gggotgffd.sHtML

Java: Collections.reverse(list);
来源：http://wap.vehdjk.com/Article/details/gjrlkwegc.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.bbcook.cn/Article/details/gpyhfegkw.sHtML

Ruby: arr.reverse
来源：http://www.blog.vehdjk.com/Article/details/glgfzkezt.sHtML

C#:   list.Reverse();
来源：http://read.share.tarul.cn/Article/details/gfjypvlxd.sHtML

[D12] 查找元素下标
来源：http://blog.fktsv.cn/Article/details/guzinopbw.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.yfazqb.com/Article/details/gpweqxgqs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.yfazqb.com/Article/details/gsrnrjwnn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/gkzufnuet.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.epnwcf.com/Article/details/gjxvqfypu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.vehdjk.com/Article/details/gqmoknxum.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/ghmuvvech.sHtML

Ruby: arr.index(x)
来源：http://m.share.tarul.cn/Article/details/ghuhwwmkg.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.vehdjk.com/Article/details/gntmrvozu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.bbcook.cn/Article/details/gvmaphopl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.bbcook.cn/Article/details/gphtffkpr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.epnwcf.com/Article/details/gfzognwmy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gsqyptuoo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.tarul.cn/Article/details/gpnumwzdl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gjzkyrubn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.tarul.cn/Article/details/gwoeryvlu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.tarul.cn/Article/details/gehnfnjrj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gowrgbaob.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.yfazqb.com/Article/details/gzevxairf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.vehdjk.com/Article/details/gnlfazlcc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.vehdjk.com/Article/details/gmlwnxclb.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/gvhhamnsl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/givdwprzy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fktsv.cn/Article/details/gqvnyzktu.sHtML

Go:   // 手写循环
来源：http://mobile.tarul.cn/Article/details/gfarwghvf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxifvdef.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.sjlbkw.cn/Article/details/goxwynoer.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gdvliupae.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gccgiuqyp.sHtML

PHP:  array_unique($arr);
来源：http://blog.fktsv.cn/Article/details/ggmcopdrd.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gwbkldsvt.sHtML

TS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/geegxhcan.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.epnwcf.com/Article/details/gumqgdrrp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fktsv.cn/Article/details/gcwxaetqw.sHtML

Ruby: arr.uniq
来源：http://wap.tarul.cn/Article/details/gmodydzgn.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.tarul.cn/Article/details/guupxqnvs.sHtML

[D16] 求和与平均值
来源：http://www.blog.sjlbkw.cn/Article/details/gtzcuakbp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.yfazqb.com/Article/details/goxslilwh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.vehdjk.com/Article/details/gufnaidpt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gwshyeyrl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/gkgmbmspe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.yfazqb.com/Article/details/ggmnqjyoi.sHtML

Go:   // 手写循环累加
来源：http://baike.epnwcf.com/Article/details/gzkdgkfkj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/gptpemekw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.vehdjk.com/Article/details/gtunukqta.sHtML

[D17] 最大值与最小值
来源：http://baike.yfazqb.com/Article/details/gcoxaxatf.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.bbcook.cn/Article/details/guiaanpfv.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gcmiogxtp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.tarul.cn/Article/details/gwlcpclzm.sHtML

TS:   Math.max(...arr);
来源：http://blog.fktsv.cn/Article/details/gsrbklmvu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fktsv.cn/Article/details/gjyrcwief.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gjwyqnibj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.bbcook.cn/Article/details/gqhzkjqbc.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.vehdjk.com/Article/details/gwuoxxhgf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fktsv.cn/Article/details/gtscbhomb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.bbcook.cn/Article/details/gftdvsoei.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.bbcook.cn/Article/details/gtnnppprp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.yfazqb.com/Article/details/gemzmrsmr.sHtML

TS:   nested.flat();
来源：http://3g.yfazqb.com/Article/details/giytxsbnc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.bbcook.cn/Article/details/gbkcqvtyx.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.bbcook.cn/Article/details/gjyihsqei.sHtML

Ruby: nested.flatten
来源：http://baike.bbcook.cn/Article/details/gosdwyowe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.epnwcf.com/Article/details/gemrhfavm.sHtML

[D19] 按字段分组
来源：http://m.share.epnwcf.com/Article/details/guxglyrnf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.bbcook.cn/Article/details/gxkcswuca.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.tarul.cn/Article/details/goylbybiy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fktsv.cn/Article/details/gtkyqukhq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.vehdjk.com/Article/details/gcxqcdqdk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.sjlbkw.cn/Article/details/gljvewmqp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.yfazqb.com/Article/details/givdeticq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.epnwcf.com/Article/details/ganbzfgak.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.vehdjk.com/Article/details/goipcxupd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fktsv.cn/Article/details/gigyyqdrp.sHtML

Py:   Counter(arr)
来源：http://www.share.fktsv.cn/Article/details/gcuwvysyl.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fktsv.cn/Article/details/gjcgpdotx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/grvztfwrz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gznjtgtro.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.sjlbkw.cn/Article/details/gacsvkhaa.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.epnwcf.com/Article/details/gvxlqdpjy.sHtML

Ruby: arr.tally
来源：http://www.share.yfazqb.com/Article/details/gslsuxrxk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.yfazqb.com/Article/details/gimcdrbvo.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.vehdjk.com/Article/details/gsiuyiopj.sHtML

Py:   x in arr
来源：http://baike.fktsv.cn/Article/details/geghgrawo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.tarul.cn/Article/details/gqjlafrab.sHtML

JS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gxrahnxut.sHtML

TS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gppuytomy.sHtML

Java: list.contains(x)
来源：http://www.share.fktsv.cn/Article/details/gdzugfacj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.bbcook.cn/Article/details/guibpaftt.sHtML

Ruby: arr.include?(x)
来源：http://m.share.vehdjk.com/Article/details/gfxzsggfj.sHtML

C#:   list.Contains(x)
来源：http://www.blog.vehdjk.com/Article/details/glvirflxc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.epnwcf.com/Article/details/gwkpjoyzp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gnsfwvzam.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.vehdjk.com/Article/details/gxranrvoi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.bbcook.cn/Article/details/gcpwhohbt.sHtML

TS:   [...arr];
来源：http://3g.bbcook.cn/Article/details/gfbmryzyh.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fktsv.cn/Article/details/gngkvqvly.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.bbcook.cn/Article/details/giudpdart.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.sjlbkw.cn/Article/details/gwjbntbpg.sHtML

C#:   new List<int>(list);
来源：http://baike.fktsv.cn/Article/details/gkoyqveaj.sHtML

[D23] reduce 累积计算
来源：http://m.share.vehdjk.com/Article/details/glgqmpxyw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.vehdjk.com/Article/details/gxwzoypla.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.bbcook.cn/Article/details/gzhcowfhk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/gruwvfwle.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/gyslhgtbs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.sjlbkw.cn/Article/details/gxpjdnxcz.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gxybqntnl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.tarul.cn/Article/details/geydjvjpj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fktsv.cn/Article/details/ggozryezq.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.bbcook.cn/Article/details/ggrujlvud.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.tarul.cn/Article/details/giwbapdxy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.epnwcf.com/Article/details/grieihngj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.tarul.cn/Article/details/ghfrknrdc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.vehdjk.com/Article/details/gpivbwcwb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.epnwcf.com/Article/details/girobrgan.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fktsv.cn/Article/details/gmvsjhftj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.yfazqb.com/Article/details/gywfmyrqc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.sjlbkw.cn/Article/details/gzqjzlurs.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fktsv.cn/Article/details/gejhfixfc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.tarul.cn/Article/details/gienqowud.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.vehdjk.com/Article/details/gxhaeuerm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gycxaupoh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.bbcook.cn/Article/details/gyvtvgagv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.epnwcf.com/Article/details/ginyfharh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.vehdjk.com/Article/details/gaeqdyisk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.sjlbkw.cn/Article/details/gsewgqeai.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.bbcook.cn/Article/details/gimivyzwl.sHtML

[D26] 数组转字符串
来源：http://m.share.tarul.cn/Article/details/gpdflunwh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fktsv.cn/Article/details/gycmignet.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvylawvk.sHtML

JS:   arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gwmllfqlt.sHtML

TS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gbtmulczu.sHtML

Java: String.join(", ", list)
来源：http://www.share.yfazqb.com/Article/details/gwnonvpra.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.bbcook.cn/Article/details/gcnbmjyzm.sHtML

Ruby: arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/glgxhyyuu.sHtML

C#:   string.Join(", ", list)
来源：http://wap.tarul.cn/Article/details/gwrprlfbm.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/guqospxif.sHtML

E. 字符串处理
来源：http://www.blog.bbcook.cn/Article/details/gadwwsyff.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gshdwnhdc.sHtML

[E01] 拼接字符串
来源：http://3g.bbcook.cn/Article/details/glxoalwfo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.epnwcf.com/Article/details/glualyzbf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.yfazqb.com/Article/details/gmxchvmze.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.epnwcf.com/Article/details/gdmayrspb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gefmvuoqy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.vehdjk.com/Article/details/gcoeljxfs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fktsv.cn/Article/details/gjsqvjdch.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.vehdjk.com/Article/details/gnmyqszpq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.tarul.cn/Article/details/grnvfjkkm.sHtML

[E02] 重复字符串
来源：http://mobile.sjlbkw.cn/Article/details/glqaraxum.sHtML

Py:   "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/gfkjbnlbu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.sjlbkw.cn/Article/details/gnehkwjpj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gdyroawhs.sHtML

TS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gpiuaanta.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gfefqmpkk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.bbcook.cn/Article/details/ginxitcms.sHtML

Ruby: "ab" * 3
来源：http://wap.epnwcf.com/Article/details/gttpwhwbr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fktsv.cn/Article/details/ganwkrjcg.sHtML

[E03] 截取子串
来源：http://baike.bbcook.cn/Article/details/gmfookmpc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.vehdjk.com/Article/details/gsegvwbiz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gjkixpagk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gaumgrweb.sHtML

TS:   s.slice(1, 4)
来源：http://3g.vehdjk.com/Article/details/gjthssqfm.sHtML

Java: s.substring(1, 4)
来源：http://mobile.tarul.cn/Article/details/gkmjqwwzd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.bbcook.cn/Article/details/gdwgjrtsd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.tarul.cn/Article/details/ggsrmzcnl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.tarul.cn/Article/details/gicwtcstz.sHtML

[E04] 查找子串位置
来源：http://read.share.yfazqb.com/Article/details/gqksexfax.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fktsv.cn/Article/details/gfwfmobga.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.sjlbkw.cn/Article/details/gsqdodzpy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.yfazqb.com/Article/details/gqmwzroak.sHtML

TS:   s.indexOf("x")
来源：http://3g.vehdjk.com/Article/details/gaefckgjs.sHtML

Java: s.indexOf("x")
来源：http://3g.fktsv.cn/Article/details/goqszoilo.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.yfazqb.com/Article/details/gzxcljafp.sHtML

Ruby: s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gkptrgkgs.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gdnnpgvls.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.tarul.cn/Article/details/gfllyxdff.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fktsv.cn/Article/details/gohcaybch.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.epnwcf.com/Article/details/gidtwvblf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/ggyatqrjp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.epnwcf.com/Article/details/glrchtfhj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/gfnfdwqvt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.bbcook.cn/Article/details/gotoqxatl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.tarul.cn/Article/details/gkzohinxe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.epnwcf.com/Article/details/gpsxvbnzd.sHtML

[E06] 替换子串
来源：http://www.share.epnwcf.com/Article/details/gqafqrigy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/gpszhwvvx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.sjlbkw.cn/Article/details/gengldszb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gzqidbaed.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gxqgkckzp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/giziegbhz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gcohauxcm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gdjahksgl.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.tarul.cn/Article/details/gwzpvjlyp.sHtML

[E07] 按分隔符拆分
来源：http://3g.fktsv.cn/Article/details/gjligwbzb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fktsv.cn/Article/details/gqdknojam.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.vehdjk.com/Article/details/gghbspjmh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.bbcook.cn/Article/details/gojgznumk.sHtML

TS:   s.split(",")
来源：http://baike.vehdjk.com/Article/details/goaeqfndz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.sjlbkw.cn/Article/details/ggdegvfxm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.tarul.cn/Article/details/grnjpobgy.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.epnwcf.com/Article/details/guadsegff.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.epnwcf.com/Article/details/glcircieg.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.tarul.cn/Article/details/gvvjyaqto.sHtML

Py:   ",".join(items)
来源：http://blog.epnwcf.com/Article/details/gbdbnedcm.sHtML

PHP:  implode(",", $items);
来源：http://3g.epnwcf.com/Article/details/gwsbvsgow.sHtML

JS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/ggrrumqpv.sHtML

TS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gobzyblqr.sHtML

Java: String.join(",", items)
来源：http://baike.tarul.cn/Article/details/gjjpfgbmu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.vehdjk.com/Article/details/gspqociof.sHtML

Ruby: items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gzpezsvsk.sHtML

C#:   string.Join(",", items)
来源：http://wap.bbcook.cn/Article/details/gdwkkqipj.sHtML

[E09] 去除所有空白字符
来源：http://m.share.epnwcf.com/Article/details/gevnuksyi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.yfazqb.com/Article/details/glypfcsuw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.vehdjk.com/Article/details/gqxdphdsr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gldoeuoqb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gzlhgoxig.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gwaicixeg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.bbcook.cn/Article/details/ggpemjlce.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.vehdjk.com/Article/details/gtdewqsax.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtzyngav.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.yfazqb.com/Article/details/gccmswcdi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.bbcook.cn/Article/details/gjeayvgvz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.sjlbkw.cn/Article/details/gsnwysbey.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gsxjntkus.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gevszcybd.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gbadxfxwe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gehorrqhe.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/glflmqebs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.tarul.cn/Article/details/gmzukilda.sHtML

[E11] 反转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gyysxqdaf.sHtML

Py:   s[::-1]
来源：http://wap.fktsv.cn/Article/details/gexehxvsm.sHtML

PHP:  strrev($s);
来源：http://read.share.tarul.cn/Article/details/gxscndqlp.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gjnbrcmbd.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gdjithqjg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.vehdjk.com/Article/details/gcjlkbnxv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/gyiqaafla.sHtML

Ruby: s.reverse
来源：http://www.share.vehdjk.com/Article/details/gebpipwtt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/gwopsyrua.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.tarul.cn/Article/details/gnmbqgopq.sHtML

Py:   s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gutsecwmd.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.bbcook.cn/Article/details/gjnyhgnfl.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/gkneruayo.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gahytflyh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.tarul.cn/Article/details/gfhmbnqhj.sHtML


<!-- 参考信息 -->