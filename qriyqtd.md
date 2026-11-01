代发 wailian999

[D07] 切片 / 取子数组
来源：http://m.share.epnwcf.com/Article/details/gcnefqbic.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.vehdjk.com/Article/details/gwlqboaeu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gxinzpubh.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gxvbzfgsu.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gslvyeghz.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gizijetfz.sHtML

Go:   arr[1:4]
来源：http://www.m.share.yfazqb.com/Article/details/grkhcladj.sHtML

Ruby: arr[1, 3]
来源：http://3g.fktsv.cn/Article/details/gphaiagjb.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.tarul.cn/Article/details/gjlrnpvvz.sHtML

[D08] 合并两个数组
来源：http://blog.yfazqb.com/Article/details/guesplxqo.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.vehdjk.com/Article/details/gwsuhzchh.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.epnwcf.com/Article/details/gjvjedbmk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.vehdjk.com/Article/details/gdvijjaoo.sHtML

TS:   [...a, ...b];
来源：http://wap.sjlbkw.cn/Article/details/gozolzdru.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.vehdjk.com/Article/details/gjmtyzkza.sHtML

Go:   append(a, b...)
来源：http://read.share.tarul.cn/Article/details/gjvtjperz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.bbcook.cn/Article/details/gsvilmygq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.tarul.cn/Article/details/gynwxdcjg.sHtML

[D09] 排序（升序）
来源：http://m.share.fktsv.cn/Article/details/ghwzvxfng.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/ghizfatbq.sHtML

PHP:  sort($arr);
来源：http://blog.vehdjk.com/Article/details/gqevcasip.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fktsv.cn/Article/details/gbdgntcxf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.bbcook.cn/Article/details/ghacptrpe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.epnwcf.com/Article/details/ghyflbovt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.epnwcf.com/Article/details/gasccdevm.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/ghkfbrqev.sHtML

C#:   list.Sort();
来源：http://read.share.tarul.cn/Article/details/giaaibmak.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.vehdjk.com/Article/details/gnrkijhac.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.vehdjk.com/Article/details/gsxnokmkp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.tarul.cn/Article/details/gulczcaxl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.vehdjk.com/Article/details/gducmtuma.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.bbcook.cn/Article/details/gqleqmdxa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.vehdjk.com/Article/details/gukysbjxq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.yfazqb.com/Article/details/gmapezyeq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.bbcook.cn/Article/details/gftfwmgxn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.vehdjk.com/Article/details/gomhazwxa.sHtML

[D11] 反转数组
来源：http://baike.epnwcf.com/Article/details/ghekcdmjw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.bbcook.cn/Article/details/gvsezrsfe.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gvnrpdkld.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fktsv.cn/Article/details/geyvgbrtm.sHtML

TS:   [...arr].reverse();
来源：http://baike.tarul.cn/Article/details/goivobmoi.sHtML

Java: Collections.reverse(list);
来源：http://www.share.tarul.cn/Article/details/gucqbjdqb.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.epnwcf.com/Article/details/glyaompot.sHtML

Ruby: arr.reverse
来源：http://www.blog.bbcook.cn/Article/details/gjvxpgoez.sHtML

C#:   list.Reverse();
来源：http://www.m.share.vehdjk.com/Article/details/gxmpegyce.sHtML

[D12] 查找元素下标
来源：http://read.share.fktsv.cn/Article/details/gvfmqrjyc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.epnwcf.com/Article/details/gwizyfkfq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fktsv.cn/Article/details/gdtjjmmws.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gapuyojbp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/ghqvslodz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.yfazqb.com/Article/details/gypjpzdxk.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.vehdjk.com/Article/details/goetrkuwf.sHtML

Ruby: arr.index(x)
来源：http://baike.yfazqb.com/Article/details/gblyjmnvx.sHtML

C#:   list.IndexOf(x);
来源：http://baike.bbcook.cn/Article/details/gzdhwxxbt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.tarul.cn/Article/details/glworlniv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.tarul.cn/Article/details/gcxzlmccp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.epnwcf.com/Article/details/glnqvegty.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.tarul.cn/Article/details/gqoqxgpvu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gkvbdqvvi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fktsv.cn/Article/details/ggwtjugjj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.sjlbkw.cn/Article/details/gndbkpqhw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.yfazqb.com/Article/details/gqqqgxbbl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.yfazqb.com/Article/details/gwnwyqisi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.vehdjk.com/Article/details/gfmitqyll.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.bbcook.cn/Article/details/gttdklvqj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.sjlbkw.cn/Article/details/gljzsbuum.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.yfazqb.com/Article/details/gnuagykqd.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/glplesoji.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gdwwsovvv.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/gjqxupbwi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gqbrgnami.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.epnwcf.com/Article/details/gwdnlolag.sHtML

[D15] 去重
来源：http://www.share.bbcook.cn/Article/details/gcyampgra.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.epnwcf.com/Article/details/grqlgnmyo.sHtML

PHP:  array_unique($arr);
来源：http://m.share.epnwcf.com/Article/details/gluqvluhp.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gcfuxlnkf.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gnumwgcfc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.yfazqb.com/Article/details/gkbxxvpuz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.vehdjk.com/Article/details/gwludlrwb.sHtML

Ruby: arr.uniq
来源：http://wap.bbcook.cn/Article/details/gjpgworvn.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gbgtluggi.sHtML

[D16] 求和与平均值
来源：http://wap.vehdjk.com/Article/details/goqdfeaes.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.epnwcf.com/Article/details/gtobczigi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.tarul.cn/Article/details/ggsnoyvxg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gcykkupxe.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gjmezcyra.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxmsdanv.sHtML

Go:   // 手写循环累加
来源：http://m.share.epnwcf.com/Article/details/gtygehzrh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/ghkoutmrl.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fktsv.cn/Article/details/gtumyvgmg.sHtML

[D17] 最大值与最小值
来源：http://wap.vehdjk.com/Article/details/gpqvefpmf.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/godbnwqhn.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.epnwcf.com/Article/details/gvwuaypay.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fktsv.cn/Article/details/gtybhgtip.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/gpdqusjez.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.bbcook.cn/Article/details/gldyhgjtz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.tarul.cn/Article/details/gfyupyhpf.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.yfazqb.com/Article/details/gthvldaow.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.epnwcf.com/Article/details/gyonhgafd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.yfazqb.com/Article/details/gjiqocphz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.epnwcf.com/Article/details/gjjvofcer.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.epnwcf.com/Article/details/gmjdrbgip.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.bbcook.cn/Article/details/gconcjwfo.sHtML

TS:   nested.flat();
来源：http://m.share.fktsv.cn/Article/details/gbpldesjh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.epnwcf.com/Article/details/gcclskjuy.sHtML

Go:   // 手写双层循环
来源：http://blog.bbcook.cn/Article/details/gcahxbtfq.sHtML

Ruby: nested.flatten
来源：http://read.share.bbcook.cn/Article/details/gbalhostr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.epnwcf.com/Article/details/gtcgnnnxm.sHtML

[D19] 按字段分组
来源：http://blog.sjlbkw.cn/Article/details/gfdegjwlj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gstresflr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.yfazqb.com/Article/details/gjzefpdcl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fktsv.cn/Article/details/gepimixlt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gvyjonkeq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fktsv.cn/Article/details/gnuqxpdwr.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.yfazqb.com/Article/details/gogqtkiae.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.vehdjk.com/Article/details/gtzhlmexo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.yfazqb.com/Article/details/gkorhqqtt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.vehdjk.com/Article/details/gezgqnxdq.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gyueotpcv.sHtML

PHP:  array_count_values($arr);
来源：http://wap.epnwcf.com/Article/details/genclyubh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gnvoihejf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.sjlbkw.cn/Article/details/gfvzpamfd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.epnwcf.com/Article/details/guzthaqnw.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.vehdjk.com/Article/details/gmwlotytf.sHtML

Ruby: arr.tally
来源：http://www.m.share.epnwcf.com/Article/details/gilxvrwrp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.sjlbkw.cn/Article/details/gjbgtqziv.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.yfazqb.com/Article/details/gjbvncxme.sHtML

Py:   x in arr
来源：http://blog.yfazqb.com/Article/details/gwzpaqwdl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.epnwcf.com/Article/details/gsassqbwh.sHtML

JS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/gwwljgmsz.sHtML

TS:   arr.includes(x)
来源：http://www.share.bbcook.cn/Article/details/ghbjxabfg.sHtML

Java: list.contains(x)
来源：http://www.share.epnwcf.com/Article/details/ggambtyxv.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gonpxcyhp.sHtML

Ruby: arr.include?(x)
来源：http://m.share.tarul.cn/Article/details/gymmhmizk.sHtML

C#:   list.Contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gnodyukkf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.sjlbkw.cn/Article/details/ggcbzpcdj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.sjlbkw.cn/Article/details/gcykmzgzt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fktsv.cn/Article/details/gywdfjuct.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fktsv.cn/Article/details/gvteuescz.sHtML

TS:   [...arr];
来源：http://3g.yfazqb.com/Article/details/gdcofrkho.sHtML

Java: new ArrayList<>(list);
来源：http://blog.tarul.cn/Article/details/gekpmzsqs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.sjlbkw.cn/Article/details/gkixtvlcq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.tarul.cn/Article/details/ggmkchynz.sHtML

C#:   new List<int>(list);
来源：http://m.share.bbcook.cn/Article/details/gtkgxkgki.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fktsv.cn/Article/details/gfouvlggw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.tarul.cn/Article/details/glyarpolq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/gpoudbhli.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/glkviteyw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gyalcesbz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.epnwcf.com/Article/details/gbkfyjkqz.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/gugbhmysp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fktsv.cn/Article/details/ggqzenfom.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.yfazqb.com/Article/details/gippbnxou.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.sjlbkw.cn/Article/details/gmykgvios.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.epnwcf.com/Article/details/ggasnrclr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.sjlbkw.cn/Article/details/gziemahvq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.epnwcf.com/Article/details/giwgsasmt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.epnwcf.com/Article/details/gmtbmwyqy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fktsv.cn/Article/details/gyltthdiq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.yfazqb.com/Article/details/gmyaiihap.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.tarul.cn/Article/details/gbymjsaos.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.epnwcf.com/Article/details/gjacerrli.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.tarul.cn/Article/details/gluyuztin.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.tarul.cn/Article/details/glqxjjmhq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.vehdjk.com/Article/details/gimqtybno.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.yfazqb.com/Article/details/gjaeahhrp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.tarul.cn/Article/details/gostvolsl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.bbcook.cn/Article/details/gnilhenvo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.tarul.cn/Article/details/gbedhxdrk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.vehdjk.com/Article/details/gandmhmzz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.tarul.cn/Article/details/gkbjqlhok.sHtML

[D26] 数组转字符串
来源：http://wap.vehdjk.com/Article/details/gqeeixsoq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/ghtvycquz.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.vehdjk.com/Article/details/gtotifrmm.sHtML

JS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gsdvjohpr.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/getnmeshn.sHtML

Java: String.join(", ", list)
来源：http://3g.epnwcf.com/Article/details/gdggqlyqa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.yfazqb.com/Article/details/gsovdeoii.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gcstjqvdo.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gisqetuef.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gcxorappb.sHtML

E. 字符串处理
来源：http://blog.bbcook.cn/Article/details/gyvhsoncq.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gwnbldpna.sHtML

[E01] 拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gmpapxukp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.vehdjk.com/Article/details/ghrukaoty.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.tarul.cn/Article/details/gifxvauha.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gpbdlemnd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/geogcfdwx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fktsv.cn/Article/details/gvopemvih.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.yfazqb.com/Article/details/gviltfmcr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.bbcook.cn/Article/details/gdfnzqyrr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/ghbilvnca.sHtML

[E02] 重复字符串
来源：http://m.share.tarul.cn/Article/details/gyyhlfsse.sHtML

Py:   "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/giuuzmgon.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.vehdjk.com/Article/details/gygzfobmp.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/geyfilpei.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gsvzgrvet.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gfkgumdll.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.vehdjk.com/Article/details/gfrtanxov.sHtML

Ruby: "ab" * 3
来源：http://baike.tarul.cn/Article/details/gtmplamhi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.epnwcf.com/Article/details/gkbioixwu.sHtML

[E03] 截取子串
来源：http://baike.yfazqb.com/Article/details/gtcckvtve.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.sjlbkw.cn/Article/details/gkclxoiuv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gmoeiewkv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/gpuidmikn.sHtML

TS:   s.slice(1, 4)
来源：http://wap.bbcook.cn/Article/details/gumkuwrqt.sHtML

Java: s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/gaoggmoty.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.bbcook.cn/Article/details/gbgxzjuag.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.bbcook.cn/Article/details/gcvddjnhe.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.bbcook.cn/Article/details/gpjczhdeq.sHtML

[E04] 查找子串位置
来源：http://www.m.share.vehdjk.com/Article/details/galwyxjfn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gjjqfbilv.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fktsv.cn/Article/details/gojiyvfqv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.epnwcf.com/Article/details/gkkjntcil.sHtML

TS:   s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/gucndiaal.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gckvfxmse.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.bbcook.cn/Article/details/gfjlftotv.sHtML

Ruby: s.index("x")
来源：http://m.share.bbcook.cn/Article/details/gelyuodbw.sHtML

C#:   s.IndexOf("x")
来源：http://baike.yfazqb.com/Article/details/gjbcqzgbx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fktsv.cn/Article/details/gpwqkofav.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.tarul.cn/Article/details/gxjzbebvv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.tarul.cn/Article/details/gedgkhxrs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.tarul.cn/Article/details/gyznrohla.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.yfazqb.com/Article/details/gtgbvyyql.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gtckhvoud.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.tarul.cn/Article/details/gginvqebc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.yfazqb.com/Article/details/gkqfrnxmj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.yfazqb.com/Article/details/gukyqekvc.sHtML

[E06] 替换子串
来源：http://read.share.epnwcf.com/Article/details/gixhktjta.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/gohtjfdhl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.tarul.cn/Article/details/gkatoalxz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gqwuuamkj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gsavaxebl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gwlqeybyi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fktsv.cn/Article/details/gdjrvapco.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gxbouizrz.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.epnwcf.com/Article/details/guzhlcjob.sHtML

[E07] 按分隔符拆分
来源：http://blog.bbcook.cn/Article/details/gjbwqvpjv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.yfazqb.com/Article/details/gxcfphhqf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gueorqvve.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.epnwcf.com/Article/details/glxqjkztw.sHtML

TS:   s.split(",")
来源：http://blog.tarul.cn/Article/details/glsixwyjn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.vehdjk.com/Article/details/gjqcnkfjf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.bbcook.cn/Article/details/gtdglacpg.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fktsv.cn/Article/details/ggctnrply.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.epnwcf.com/Article/details/gbgbtpfok.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.bbcook.cn/Article/details/gxdqjpoyz.sHtML

Py:   ",".join(items)
来源：http://read.share.yfazqb.com/Article/details/ghzdryyut.sHtML

PHP:  implode(",", $items);
来源：http://www.share.sjlbkw.cn/Article/details/ghbhkzwxa.sHtML

JS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gvmwqidfi.sHtML

TS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gcdzregsx.sHtML

Java: String.join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/ggcrlrrhw.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.sjlbkw.cn/Article/details/gvqlzowmb.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gwcazhepe.sHtML

C#:   string.Join(",", items)
来源：http://wap.sjlbkw.cn/Article/details/gmhkeippb.sHtML

[E09] 去除所有空白字符
来源：http://blog.epnwcf.com/Article/details/gdqwatrtj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fktsv.cn/Article/details/ggirzqohz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.tarul.cn/Article/details/giufedzui.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/glqmsynpg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/gvbxrtdyc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.vehdjk.com/Article/details/grwsnhbis.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.epnwcf.com/Article/details/gennruysv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fktsv.cn/Article/details/goxqayktu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gvyrzyswh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.yfazqb.com/Article/details/gyfsltctc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gwuilbhvu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.sjlbkw.cn/Article/details/gpgcakfdj.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/ggtrxhzpe.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gmhvbwplt.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gjxthfhry.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gwtiiemhn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gfaebbvlp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.yfazqb.com/Article/details/gkrqngskf.sHtML

[E11] 反转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gqnyzzrsy.sHtML

Py:   s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/gqdkwlafg.sHtML

PHP:  strrev($s);
来源：http://mobile.tarul.cn/Article/details/gwjrnhhnl.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gjbapppsx.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gafhzvdhg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.sjlbkw.cn/Article/details/ggcfzvuir.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gwpiclkjl.sHtML

Ruby: s.reverse
来源：http://www.blog.tarul.cn/Article/details/gmpqegnkn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gkbjtbdon.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/ggykbmbwb.sHtML

Py:   s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/giteucqyb.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.vehdjk.com/Article/details/gpnvqmsky.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.sjlbkw.cn/Article/details/ghgqcluxv.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gzbzkasru.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.yfazqb.com/Article/details/gecqmgloj.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.bbcook.cn/Article/details/gttmovxrk.sHtML

Ruby: s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gsqxpeauz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.epnwcf.com/Article/details/gimubpmrz.sHtML

[E13] 逐字符遍历
来源：http://wap.yfazqb.com/Article/details/ggegwtjmf.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.epnwcf.com/Article/details/gokixuylq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.sjlbkw.cn/Article/details/gmxzvbekd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/gqbnfrevs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gvgmxponk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.yfazqb.com/Article/details/gcnwdniih.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.vehdjk.com/Article/details/gtlounlfr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.vehdjk.com/Article/details/guzfbpawz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.yfazqb.com/Article/details/gzculyybt.sHtML


<!-- 参考信息 -->