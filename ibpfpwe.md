代发 wailian999

TS:   arr.slice(1, 4);
来源：http://baike.tarul.cn/Article/details/gkzgkoumw.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gjuxwkhal.sHtML

Go:   arr[1:4]
来源：http://baike.fktsv.cn/Article/details/ggcleewhh.sHtML

Ruby: arr[1, 3]
来源：http://3g.epnwcf.com/Article/details/gzgqslpqt.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gunezmkcz.sHtML

[D08] 合并两个数组
来源：http://www.m.share.epnwcf.com/Article/details/gbpjkmyoq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.tarul.cn/Article/details/gpsarsqxh.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.vehdjk.com/Article/details/giwsmeocc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.sjlbkw.cn/Article/details/gifghnvaz.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fktsv.cn/Article/details/giwtwbrta.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.bbcook.cn/Article/details/gbgurdlew.sHtML

Go:   append(a, b...)
来源：http://baike.vehdjk.com/Article/details/gsyjplgrp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.vehdjk.com/Article/details/gmrdzsxmz.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.vehdjk.com/Article/details/grvqzuwxc.sHtML

[D09] 排序（升序）
来源：http://wap.bbcook.cn/Article/details/gcyhxbhqz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/ggkhrchoz.sHtML

PHP:  sort($arr);
来源：http://wap.tarul.cn/Article/details/ggvgwifjb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.epnwcf.com/Article/details/gfehaxbfl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fktsv.cn/Article/details/gttcyalbj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.tarul.cn/Article/details/ghjyqrxps.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gwymjpzab.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/geubstbhm.sHtML

C#:   list.Sort();
来源：http://www.m.share.tarul.cn/Article/details/glzvygjgi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.bbcook.cn/Article/details/gfnknsmpx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.yfazqb.com/Article/details/gguvsnsae.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fktsv.cn/Article/details/gsxrdeank.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/gemkvosmh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/glrnpkviw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.epnwcf.com/Article/details/gmvxizfup.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.tarul.cn/Article/details/ggqcsnfzt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.vehdjk.com/Article/details/gseivmfnb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.vehdjk.com/Article/details/glpkaries.sHtML

[D11] 反转数组
来源：http://m.share.vehdjk.com/Article/details/gpenxcahb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.vehdjk.com/Article/details/gcxbpejrj.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.tarul.cn/Article/details/gxfwgorgu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.epnwcf.com/Article/details/gtwaogwyt.sHtML

TS:   [...arr].reverse();
来源：http://read.share.vehdjk.com/Article/details/gqrdzdrhl.sHtML

Java: Collections.reverse(list);
来源：http://read.share.bbcook.cn/Article/details/gywnokckw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fktsv.cn/Article/details/gancmffzq.sHtML

Ruby: arr.reverse
来源：http://mobile.tarul.cn/Article/details/gyobgvnfw.sHtML

C#:   list.Reverse();
来源：http://www.share.epnwcf.com/Article/details/gzausvltr.sHtML

[D12] 查找元素下标
来源：http://blog.bbcook.cn/Article/details/gnzcdnmiw.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.tarul.cn/Article/details/ghnwsjhuu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.sjlbkw.cn/Article/details/gkkdputsv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.sjlbkw.cn/Article/details/gwyfolhqj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.bbcook.cn/Article/details/ghlawuvei.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.epnwcf.com/Article/details/geqyzbphc.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gyublmznz.sHtML

Ruby: arr.index(x)
来源：http://baike.sjlbkw.cn/Article/details/grktpokxq.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.bbcook.cn/Article/details/gglibxqug.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fktsv.cn/Article/details/gssabjdvn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.bbcook.cn/Article/details/gpqnntxiw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.vehdjk.com/Article/details/ghxpskajx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/grzwxtmwi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/gdnthkpuo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fktsv.cn/Article/details/gvbmncsgj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fktsv.cn/Article/details/gsgvwnvqu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.epnwcf.com/Article/details/gfibwanok.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gkmfngjrc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.epnwcf.com/Article/details/gcrjrlgua.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fktsv.cn/Article/details/gqkscxbbc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fktsv.cn/Article/details/gwotcnhke.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gppghxxik.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/gtmtfujvo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.epnwcf.com/Article/details/giseaazbr.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gvjbhiwvb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.tarul.cn/Article/details/giesylxnu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/glykswsum.sHtML

[D15] 去重
来源：http://www.m.share.yfazqb.com/Article/details/gzcivgmol.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.sjlbkw.cn/Article/details/gwtzummuu.sHtML

PHP:  array_unique($arr);
来源：http://baike.sjlbkw.cn/Article/details/gxazhyydq.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/guxdrqnwa.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/grbtnpfmk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.bbcook.cn/Article/details/gvbnzhvsk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdukswod.sHtML

Ruby: arr.uniq
来源：http://read.share.bbcook.cn/Article/details/gnkayndem.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.yfazqb.com/Article/details/gusgzszsj.sHtML

[D16] 求和与平均值
来源：http://read.share.tarul.cn/Article/details/gbdkypiyr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.yfazqb.com/Article/details/guwrabfqf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/ghtuntkhf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/gqgxlgdip.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gdsfvnnmc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.tarul.cn/Article/details/gkthdxiuj.sHtML

Go:   // 手写循环累加
来源：http://baike.epnwcf.com/Article/details/gdjiygqut.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.bbcook.cn/Article/details/goyeqzyis.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.yfazqb.com/Article/details/gdferrgri.sHtML

[D17] 最大值与最小值
来源：http://m.share.sjlbkw.cn/Article/details/gmsnczreo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gfqzpgiyx.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gjchzvabm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.vehdjk.com/Article/details/gxiexjubt.sHtML

TS:   Math.max(...arr);
来源：http://mobile.yfazqb.com/Article/details/gngqrrsod.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.sjlbkw.cn/Article/details/gmhbegdqg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.tarul.cn/Article/details/gcfpfuitx.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.yfazqb.com/Article/details/gjqdndolm.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.bbcook.cn/Article/details/grvefkjsr.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.vehdjk.com/Article/details/gnvnifgzr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.bbcook.cn/Article/details/ggpxcavxo.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.epnwcf.com/Article/details/gthscepvf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.tarul.cn/Article/details/gjyozkant.sHtML

TS:   nested.flat();
来源：http://m.share.bbcook.cn/Article/details/gbukfjzhs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.yfazqb.com/Article/details/gjcfeyywr.sHtML

Go:   // 手写双层循环
来源：http://www.share.bbcook.cn/Article/details/gjyybseti.sHtML

Ruby: nested.flatten
来源：http://baike.epnwcf.com/Article/details/grspuboab.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gbqozjfoi.sHtML

[D19] 按字段分组
来源：http://blog.epnwcf.com/Article/details/gozbphepf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.yfazqb.com/Article/details/glgchiaks.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.tarul.cn/Article/details/gygpinytg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.yfazqb.com/Article/details/gedjvbvjg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/gmsqgvypw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.yfazqb.com/Article/details/gypmqnixt.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.vehdjk.com/Article/details/grtdhouvs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.tarul.cn/Article/details/gtznbqpps.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.sjlbkw.cn/Article/details/gyjradpji.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.yfazqb.com/Article/details/govclqvfo.sHtML

Py:   Counter(arr)
来源：http://read.share.epnwcf.com/Article/details/gwazhivdb.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.bbcook.cn/Article/details/ghpqmhxzp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gueuhqymb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.vehdjk.com/Article/details/gocvjyplf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.sjlbkw.cn/Article/details/ggvbsjvjj.sHtML

Go:   // 手写 map[T]int
来源：http://baike.bbcook.cn/Article/details/gaebionun.sHtML

Ruby: arr.tally
来源：http://read.share.fktsv.cn/Article/details/gjjdmaqge.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.tarul.cn/Article/details/gyjcnquiu.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.vehdjk.com/Article/details/glhploaam.sHtML

Py:   x in arr
来源：http://mobile.yfazqb.com/Article/details/grkrdwygd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.bbcook.cn/Article/details/gjlohszhl.sHtML

JS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/gzhvnxxew.sHtML

TS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/gesjmrdtm.sHtML

Java: list.contains(x)
来源：http://blog.tarul.cn/Article/details/gxmoxpmyi.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gzlfjhmsv.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gcyjzvvds.sHtML

C#:   list.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gzkegalef.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.yfazqb.com/Article/details/gmzjpobex.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fktsv.cn/Article/details/gmojcbmhk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.yfazqb.com/Article/details/gvcxeogbf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.tarul.cn/Article/details/gobdjayhk.sHtML

TS:   [...arr];
来源：http://read.share.bbcook.cn/Article/details/gbkkdmsji.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fktsv.cn/Article/details/ggxibvpat.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.epnwcf.com/Article/details/gsvmjuyet.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.sjlbkw.cn/Article/details/gmufcyirs.sHtML

C#:   new List<int>(list);
来源：http://www.share.fktsv.cn/Article/details/gzgpdanwc.sHtML

[D23] reduce 累积计算
来源：http://baike.vehdjk.com/Article/details/gkzjbflsp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.tarul.cn/Article/details/gbglthkoo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.vehdjk.com/Article/details/gvmaybnnk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/gcvvnqkcw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/gnhipadka.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.tarul.cn/Article/details/gwjeikuom.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/gsokngznu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.tarul.cn/Article/details/gefgsvidq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fktsv.cn/Article/details/ghxmikwkl.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.epnwcf.com/Article/details/gyjxnavzj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.epnwcf.com/Article/details/glsnglsyt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.sjlbkw.cn/Article/details/gbuehixss.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.yfazqb.com/Article/details/gqxeefvqg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.tarul.cn/Article/details/gziruyggl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fktsv.cn/Article/details/gwprgopal.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.vehdjk.com/Article/details/gtbsfkwwz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.bbcook.cn/Article/details/gsspshdfz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.vehdjk.com/Article/details/gcyvuxryf.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.yfazqb.com/Article/details/gfnxbgypo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fktsv.cn/Article/details/gwhtzjdeu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.tarul.cn/Article/details/gferdllrk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.yfazqb.com/Article/details/gdklkmtbl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.vehdjk.com/Article/details/gwahylpoy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.epnwcf.com/Article/details/gbwpikkfy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fktsv.cn/Article/details/govrxtanf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.tarul.cn/Article/details/gpiorjxop.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gklkpjney.sHtML

[D26] 数组转字符串
来源：http://blog.yfazqb.com/Article/details/gzllpdjru.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.tarul.cn/Article/details/gdinwezke.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gycylgrgg.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gdtjpvgkm.sHtML

TS:   arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gacunvcej.sHtML

Java: String.join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/giiorgave.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.yfazqb.com/Article/details/gioebvkob.sHtML

Ruby: arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gjeigpsrs.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/gbbkwxgdl.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gjomlnkcf.sHtML

E. 字符串处理
来源：http://wap.fktsv.cn/Article/details/ghtrjytmt.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gubvbbdzo.sHtML

[E01] 拼接字符串
来源：http://wap.bbcook.cn/Article/details/gjvrbjzdg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.yfazqb.com/Article/details/gcvioefzc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.epnwcf.com/Article/details/gjkmemmqw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/gfpukwmct.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/ghrtduzfi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.epnwcf.com/Article/details/gjgozntla.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.sjlbkw.cn/Article/details/gjbdimvet.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.tarul.cn/Article/details/gxccaabjq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.epnwcf.com/Article/details/gnfzyswnq.sHtML

[E02] 重复字符串
来源：http://www.share.yfazqb.com/Article/details/gdtmbxtji.sHtML

Py:   "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gbwytfvul.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fktsv.cn/Article/details/gxjzjrktd.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gffjvahiw.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gldggpdzj.sHtML

Java: "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/grzvrasbo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.sjlbkw.cn/Article/details/gxaufzmgq.sHtML

Ruby: "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gjlbitdcm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.bbcook.cn/Article/details/gtthmvigy.sHtML

[E03] 截取子串
来源：http://wap.tarul.cn/Article/details/ghadkofqr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.sjlbkw.cn/Article/details/gdvrgmsfw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gmpxwclrd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gmcniovbi.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gjpcanpfr.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gdanuraux.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/glsquybmb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.vehdjk.com/Article/details/gyyrwatgd.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fktsv.cn/Article/details/grkciivsb.sHtML

[E04] 查找子串位置
来源：http://wap.vehdjk.com/Article/details/giasvvhhj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.tarul.cn/Article/details/gzvolbxki.sHtML

PHP:  strpos($s, "x");
来源：http://3g.sjlbkw.cn/Article/details/gzviiqmea.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.vehdjk.com/Article/details/gvymrsahx.sHtML

TS:   s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gwramculy.sHtML

Java: s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gpmlrkfqo.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.bbcook.cn/Article/details/gzexpvoxh.sHtML

Ruby: s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gxwltjwdp.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gyrliktxa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.yfazqb.com/Article/details/grenhxfac.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/gxvedsdff.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fktsv.cn/Article/details/gjgwyxjih.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.vehdjk.com/Article/details/gfktvovtz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.bbcook.cn/Article/details/gkuaizowl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gmctlaoqj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.vehdjk.com/Article/details/guatbufim.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.sjlbkw.cn/Article/details/ggnayrkwv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.tarul.cn/Article/details/gsknllhms.sHtML

[E06] 替换子串
来源：http://www.blog.fktsv.cn/Article/details/gfgkjzwhh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gikaxcrsa.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fktsv.cn/Article/details/gmvqgigqc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/goxahrevt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gpytliire.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gzwpiribp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdfpixur.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fktsv.cn/Article/details/gkeuytsxn.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gauzvookz.sHtML

[E07] 按分隔符拆分
来源：http://baike.bbcook.cn/Article/details/ghyxdrstp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.epnwcf.com/Article/details/gxwgbvkrm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gezmellcc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfmacklq.sHtML

TS:   s.split(",")
来源：http://read.share.fktsv.cn/Article/details/gahlpilcz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.tarul.cn/Article/details/gxfcwjcsb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.yfazqb.com/Article/details/gnupixrlj.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.yfazqb.com/Article/details/gufpvngci.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.yfazqb.com/Article/details/gddvwuhwa.sHtML

[E08] 数组按分隔符合并
来源：http://wap.bbcook.cn/Article/details/gyfpwxnhd.sHtML

Py:   ",".join(items)
来源：http://www.share.epnwcf.com/Article/details/gawkdplrb.sHtML

PHP:  implode(",", $items);
来源：http://wap.bbcook.cn/Article/details/gurvywpxd.sHtML

JS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/gyorddvaf.sHtML

TS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gmtratndn.sHtML

Java: String.join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/gruuswbtg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.sjlbkw.cn/Article/details/gmrfdhliz.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gaouaiqnu.sHtML

C#:   string.Join(",", items)
来源：http://m.share.bbcook.cn/Article/details/golagrjds.sHtML

[E09] 去除所有空白字符
来源：http://wap.tarul.cn/Article/details/gobcuqtmt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.yfazqb.com/Article/details/gobjjomyl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fktsv.cn/Article/details/gfwcjcvpm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/gceescpgb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/gjlhpfqsz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gmtjzsbaw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.bbcook.cn/Article/details/gijrcxgkv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.bbcook.cn/Article/details/gvaemyuux.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.vehdjk.com/Article/details/grjgsjumv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.bbcook.cn/Article/details/guurobwzu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fktsv.cn/Article/details/gowluypzr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.tarul.cn/Article/details/gitwntirb.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gqkguakef.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gdmsvniie.sHtML

Java: String.format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gjrglyskr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gunsyxhsn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gruzispnx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.tarul.cn/Article/details/gbyxewllt.sHtML

[E11] 反转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsurigzb.sHtML

Py:   s[::-1]
来源：http://baike.vehdjk.com/Article/details/gotrbhtqf.sHtML

PHP:  strrev($s);
来源：http://m.share.fktsv.cn/Article/details/gpxvwvmmb.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gnppfmgfc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbgigiak.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.bbcook.cn/Article/details/gsogogjkm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gjlromeoj.sHtML

Ruby: s.reverse
来源：http://mobile.epnwcf.com/Article/details/gsnjqbyyg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gmtccrupf.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gicnrufpq.sHtML

Py:   s.count("a")
来源：http://wap.bbcook.cn/Article/details/gwkjcyldn.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.bbcook.cn/Article/details/ggbncpjqy.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/gadfnaqom.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/gybxbxdqs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.sjlbkw.cn/Article/details/gzekftnhe.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.yfazqb.com/Article/details/gptlfyplo.sHtML

Ruby: s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gryohnpwh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fktsv.cn/Article/details/gfzkjkaui.sHtML

[E13] 逐字符遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gcebwbltt.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.epnwcf.com/Article/details/gwqkqkcjz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.epnwcf.com/Article/details/glybxbedo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/gttefpuoa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/grvytxgzq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.bbcook.cn/Article/details/gsclavbbt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.vehdjk.com/Article/details/gntbcebdi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.vehdjk.com/Article/details/gjyvrffmh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.bbcook.cn/Article/details/giqshbbvj.sHtML

[E14] URL 编码与 Base64
来源：http://3g.tarul.cn/Article/details/gyzupaivb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/grsmbmcpa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.bbcook.cn/Article/details/gxqiwwanl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.bbcook.cn/Article/details/gwqsdxnob.sHtML


<!-- 参考信息 -->