代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/grybkyqhd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.vehdjk.com/Article/details/glcyrvfbi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gooolnrbz.sHtML

[D06] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gyfgoaamz.sHtML

Py:   len(arr)
来源：http://blog.fktsv.cn/Article/details/gljoybwpz.sHtML

PHP:  count($arr);
来源：http://mobile.tarul.cn/Article/details/gfelhghzn.sHtML

JS:   arr.length
来源：http://blog.bbcook.cn/Article/details/gqfngslrj.sHtML

TS:   arr.length
来源：http://baike.epnwcf.com/Article/details/gqhhzsjpi.sHtML

Java: list.size();
来源：http://wap.yfazqb.com/Article/details/gyxpnabcm.sHtML

Go:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/grzmvutvs.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.bbcook.cn/Article/details/gfnbzouho.sHtML

C#:   list.Count;
来源：http://mobile.sjlbkw.cn/Article/details/gptztuzbs.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fktsv.cn/Article/details/gylpocnzo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.sjlbkw.cn/Article/details/glsuuvrma.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.tarul.cn/Article/details/glanxyemf.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gzsfldmni.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gohvoytnt.sHtML

Java: list.subList(1, 4);
来源：http://wap.vehdjk.com/Article/details/gupfmgibh.sHtML

Go:   arr[1:4]
来源：http://read.share.sjlbkw.cn/Article/details/gezpomjaf.sHtML

Ruby: arr[1, 3]
来源：http://read.share.tarul.cn/Article/details/gbjcqzjus.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.yfazqb.com/Article/details/ggozsckfx.sHtML

[D08] 合并两个数组
来源：http://www.blog.fktsv.cn/Article/details/gpvoshjni.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.epnwcf.com/Article/details/giribjkrm.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fktsv.cn/Article/details/gvynwsieq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.tarul.cn/Article/details/gertaxzks.sHtML

TS:   [...a, ...b];
来源：http://wap.epnwcf.com/Article/details/gzrulpxiv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fktsv.cn/Article/details/gblnalgfa.sHtML

Go:   append(a, b...)
来源：http://www.share.vehdjk.com/Article/details/gmenbirsc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.epnwcf.com/Article/details/gpekdbglk.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.bbcook.cn/Article/details/gwtdnlfsa.sHtML

[D09] 排序（升序）
来源：http://www.blog.epnwcf.com/Article/details/gxpazekgy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/gtphdzrws.sHtML

PHP:  sort($arr);
来源：http://www.share.bbcook.cn/Article/details/gexgbwkgi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.tarul.cn/Article/details/gaklogfat.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.epnwcf.com/Article/details/gflovgaza.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.vehdjk.com/Article/details/gybysgcnw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.vehdjk.com/Article/details/glkjllhrk.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/grjgzidma.sHtML

C#:   list.Sort();
来源：http://baike.fktsv.cn/Article/details/geufeixef.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.yfazqb.com/Article/details/gvqatziwa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.tarul.cn/Article/details/guyuitqat.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/gzroieuqo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.yfazqb.com/Article/details/grmnchxeu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/gbcjvthrj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.vehdjk.com/Article/details/gpjxhblpk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fktsv.cn/Article/details/gxxtmefqv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.epnwcf.com/Article/details/gppmjlqvc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.vehdjk.com/Article/details/gujhgopra.sHtML

[D11] 反转数组
来源：http://blog.bbcook.cn/Article/details/grntsxqsd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fktsv.cn/Article/details/gqedevkjn.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.epnwcf.com/Article/details/gdlsbywpg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.bbcook.cn/Article/details/glrnmsxfh.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.sjlbkw.cn/Article/details/gtstdwcao.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fktsv.cn/Article/details/ghrllduqz.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.epnwcf.com/Article/details/gkkprhzzs.sHtML

Ruby: arr.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gaqwtjhow.sHtML

C#:   list.Reverse();
来源：http://mobile.sjlbkw.cn/Article/details/gvelaqkmz.sHtML

[D12] 查找元素下标
来源：http://wap.tarul.cn/Article/details/ghoazdwje.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fktsv.cn/Article/details/glcvaufxp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.yfazqb.com/Article/details/gakcbmull.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gaojetedo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.vehdjk.com/Article/details/gspwzvqqo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fktsv.cn/Article/details/gasiqcduz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gohmtwfgv.sHtML

Ruby: arr.index(x)
来源：http://mobile.yfazqb.com/Article/details/gnutqjvwk.sHtML

C#:   list.IndexOf(x);
来源：http://baike.vehdjk.com/Article/details/gjgtxldvz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fktsv.cn/Article/details/gujqokwvh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.bbcook.cn/Article/details/gyttxercj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.epnwcf.com/Article/details/gsaftwaca.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/gzcuodhlm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/gbesveonr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fktsv.cn/Article/details/gfurszmxc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.sjlbkw.cn/Article/details/gfhgcumhp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.tarul.cn/Article/details/grvrfjvym.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.tarul.cn/Article/details/gvjjwhhyq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.vehdjk.com/Article/details/gxkljzdgm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.bbcook.cn/Article/details/gdirnqkxr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/geaidplqg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.bbcook.cn/Article/details/glsmagkgx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.vehdjk.com/Article/details/gfgahgjlv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.bbcook.cn/Article/details/gumjsoowc.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/guotngkrr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gizxejune.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.vehdjk.com/Article/details/gryknhbte.sHtML

[D15] 去重
来源：http://blog.bbcook.cn/Article/details/gqirxkhxy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fktsv.cn/Article/details/glnfkjars.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gytyvveri.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gkowcpiqs.sHtML

TS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gpgwadvfr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.epnwcf.com/Article/details/grsegarlw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.bbcook.cn/Article/details/gnhwipsns.sHtML

Ruby: arr.uniq
来源：http://m.share.vehdjk.com/Article/details/gexfdqkla.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fktsv.cn/Article/details/grlcwoenr.sHtML

[D16] 求和与平均值
来源：http://mobile.sjlbkw.cn/Article/details/ggqrvzojk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gnfxjdsrl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/galmldazm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.yfazqb.com/Article/details/gjnsxkdrr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gtzrmlxlt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.epnwcf.com/Article/details/guatxridt.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.yfazqb.com/Article/details/gzdjgvgwt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/gldwcisgw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.epnwcf.com/Article/details/gobqsjwcr.sHtML

[D17] 最大值与最小值
来源：http://blog.yfazqb.com/Article/details/gmffmqkex.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fktsv.cn/Article/details/guazvurul.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gvalhayjm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.bbcook.cn/Article/details/gziphjafg.sHtML

TS:   Math.max(...arr);
来源：http://read.share.yfazqb.com/Article/details/ginlhrpmd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.sjlbkw.cn/Article/details/gjkhrkjjd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fktsv.cn/Article/details/gpoqjxcll.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.sjlbkw.cn/Article/details/gjowxwmbf.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.sjlbkw.cn/Article/details/guyjjidxd.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.tarul.cn/Article/details/gnqgifyfm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.epnwcf.com/Article/details/gbduviovo.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.bbcook.cn/Article/details/gfkbnuxcq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.sjlbkw.cn/Article/details/gfbevfdgy.sHtML

TS:   nested.flat();
来源：http://wap.bbcook.cn/Article/details/goitfsjyt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.bbcook.cn/Article/details/gmnmythcf.sHtML

Go:   // 手写双层循环
来源：http://mobile.bbcook.cn/Article/details/gvudxljqu.sHtML

Ruby: nested.flatten
来源：http://www.m.share.bbcook.cn/Article/details/gbovfqekj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gktvtdqct.sHtML

[D19] 按字段分组
来源：http://3g.bbcook.cn/Article/details/gsnngxpjy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fktsv.cn/Article/details/gnngrcwzq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.vehdjk.com/Article/details/guuixaixq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.epnwcf.com/Article/details/gnwfswieq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/gbabcxfvb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.yfazqb.com/Article/details/gnburrfdr.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.tarul.cn/Article/details/goglfrynd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.epnwcf.com/Article/details/ggrclpxal.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fktsv.cn/Article/details/gyfxvvyjb.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.vehdjk.com/Article/details/ggajgzvjx.sHtML

Py:   Counter(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gzfjbmcae.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.tarul.cn/Article/details/gdsgxqsrs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gskwtoxgw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/glofuoeza.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.yfazqb.com/Article/details/gqotuagxb.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.vehdjk.com/Article/details/gxozkcgvt.sHtML

Ruby: arr.tally
来源：http://blog.epnwcf.com/Article/details/gzetwxlrs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/gmdrjsrqi.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.vehdjk.com/Article/details/gzscyjglq.sHtML

Py:   x in arr
来源：http://read.share.bbcook.cn/Article/details/grlbaappy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.epnwcf.com/Article/details/gytrrfqqo.sHtML

JS:   arr.includes(x)
来源：http://read.share.fktsv.cn/Article/details/gglizqoob.sHtML

TS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gegrmshua.sHtML

Java: list.contains(x)
来源：http://read.share.vehdjk.com/Article/details/gevxeojra.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.bbcook.cn/Article/details/gkwwyropy.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.tarul.cn/Article/details/gfnxyhhpw.sHtML

C#:   list.Contains(x)
来源：http://wap.vehdjk.com/Article/details/gcrpnrcce.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.bbcook.cn/Article/details/ghblxwgvm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.bbcook.cn/Article/details/gxqdfhfoh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.epnwcf.com/Article/details/gbiqumubh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.yfazqb.com/Article/details/gxbmpfccj.sHtML

TS:   [...arr];
来源：http://www.share.tarul.cn/Article/details/ggfmkjdex.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.bbcook.cn/Article/details/gxckixnbb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.tarul.cn/Article/details/ggguukybn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.sjlbkw.cn/Article/details/ghcdobmgi.sHtML

C#:   new List<int>(list);
来源：http://blog.sjlbkw.cn/Article/details/ggfjnmkak.sHtML

[D23] reduce 累积计算
来源：http://wap.bbcook.cn/Article/details/gjqgvrpbo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.vehdjk.com/Article/details/gjrwyoxyg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.epnwcf.com/Article/details/gcbikoezj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gmahldtsm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gxvjluexf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fktsv.cn/Article/details/giufrwepr.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/gdgdshgut.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.bbcook.cn/Article/details/gwrtcojmw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.sjlbkw.cn/Article/details/gisjejrps.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.vehdjk.com/Article/details/gwbqylddx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.bbcook.cn/Article/details/gjphcmlnb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.yfazqb.com/Article/details/gkqchrncw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gkbyznket.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fktsv.cn/Article/details/gjsmoomvw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.sjlbkw.cn/Article/details/glbhjznse.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.tarul.cn/Article/details/gzkdpwmxb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fktsv.cn/Article/details/gvwmafpsr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.epnwcf.com/Article/details/guaxgocuv.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.epnwcf.com/Article/details/gpbgdyeyz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.bbcook.cn/Article/details/gsgetvule.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.tarul.cn/Article/details/gplzgkjvz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.epnwcf.com/Article/details/gvbvjskmx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.yfazqb.com/Article/details/glyvrxsko.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.bbcook.cn/Article/details/gvrcdhhfb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.vehdjk.com/Article/details/gxemygcsi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.tarul.cn/Article/details/gustgddhr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.yfazqb.com/Article/details/gdoftlxgr.sHtML

[D26] 数组转字符串
来源：http://m.share.fktsv.cn/Article/details/guducpcre.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fktsv.cn/Article/details/ghhlffoiq.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.tarul.cn/Article/details/gvjfraklc.sHtML

JS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gdrmhvqad.sHtML

TS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gkmbtmwnl.sHtML

Java: String.join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gjccwbrtu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.sjlbkw.cn/Article/details/gkmdvphdu.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gdfrfjtcn.sHtML

C#:   string.Join(", ", list)
来源：http://wap.vehdjk.com/Article/details/gdifxocbk.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gxjuetuuc.sHtML

E. 字符串处理
来源：http://wap.tarul.cn/Article/details/guljwaulk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gmljlfoqk.sHtML

[E01] 拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gbboqbkey.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.yfazqb.com/Article/details/gmxxztzjg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.vehdjk.com/Article/details/ghhzafopt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gjpviqxmo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.sjlbkw.cn/Article/details/glzwtlcej.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.yfazqb.com/Article/details/gxzsoxqhd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.sjlbkw.cn/Article/details/gvdttawsz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fktsv.cn/Article/details/gkmpuypgh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.epnwcf.com/Article/details/guhxwpgma.sHtML

[E02] 重复字符串
来源：http://baike.epnwcf.com/Article/details/ggiyvxbdj.sHtML

Py:   "ab" * 3
来源：http://blog.sjlbkw.cn/Article/details/gebxtzkes.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.sjlbkw.cn/Article/details/ghvxbrhcx.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/goyquwgsx.sHtML

TS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gsdmejupp.sHtML

Java: "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gwpohbayl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.vehdjk.com/Article/details/ggkrbbcjm.sHtML

Ruby: "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gytjoevcm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.yfazqb.com/Article/details/gnouwkujf.sHtML

[E03] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gbopczvvu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.epnwcf.com/Article/details/gbkjtyzat.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/guomoizdf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gscgxoyze.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fktsv.cn/Article/details/glbejusii.sHtML

Java: s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gipdgiztb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.bbcook.cn/Article/details/gicavryms.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.vehdjk.com/Article/details/gwkyqeeck.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fktsv.cn/Article/details/gxcbzhvik.sHtML

[E04] 查找子串位置
来源：http://wap.yfazqb.com/Article/details/gitmgksnh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.bbcook.cn/Article/details/gwmpybshm.sHtML

PHP:  strpos($s, "x");
来源：http://baike.yfazqb.com/Article/details/ghusierpo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.sjlbkw.cn/Article/details/govmgwanm.sHtML

TS:   s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/glszdvidh.sHtML

Java: s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/glchyaatf.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.vehdjk.com/Article/details/gcnddpqwl.sHtML

Ruby: s.index("x")
来源：http://baike.fktsv.cn/Article/details/gtimcuziq.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.epnwcf.com/Article/details/ggfyihqox.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.epnwcf.com/Article/details/gkfqjsncy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.epnwcf.com/Article/details/gtxvmgpuw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.vehdjk.com/Article/details/glwgndamm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.yfazqb.com/Article/details/gujtdllbm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.vehdjk.com/Article/details/gcuqgjiof.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.bbcook.cn/Article/details/gjemntgeq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.sjlbkw.cn/Article/details/gbhuaouis.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.yfazqb.com/Article/details/ghpupnkit.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gggbcjxoa.sHtML

[E06] 替换子串
来源：http://www.blog.tarul.cn/Article/details/gclkzlqyn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gjzvmmkea.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.yfazqb.com/Article/details/gwahnnqyf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gkiacvllh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/ghbgacqht.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gekgljujz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/gwmttwgjl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gzrxoyofp.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.epnwcf.com/Article/details/giskhgzjx.sHtML

[E07] 按分隔符拆分
来源：http://3g.fktsv.cn/Article/details/gvlgdpwzv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fktsv.cn/Article/details/grrqjnahw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gulgfmgti.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.bbcook.cn/Article/details/gqtunofkg.sHtML

TS:   s.split(",")
来源：http://baike.fktsv.cn/Article/details/gyqlggijp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.epnwcf.com/Article/details/gbyajcapy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.epnwcf.com/Article/details/gksjbbtjf.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.tarul.cn/Article/details/gamevxxqe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.tarul.cn/Article/details/ghjjtngwv.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.sjlbkw.cn/Article/details/gwuqxnwhc.sHtML

Py:   ",".join(items)
来源：http://read.share.bbcook.cn/Article/details/ghcomknuo.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fktsv.cn/Article/details/gszqqbbcz.sHtML

JS:   items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gpfaygevu.sHtML

TS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gjcylcncp.sHtML

Java: String.join(",", items)
来源：http://wap.yfazqb.com/Article/details/gbrvmpahg.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fktsv.cn/Article/details/gzkpnjjvg.sHtML

Ruby: items.join(",")
来源：http://blog.vehdjk.com/Article/details/gwyeneylh.sHtML

C#:   string.Join(",", items)
来源：http://blog.vehdjk.com/Article/details/gfrybuoim.sHtML

[E09] 去除所有空白字符
来源：http://mobile.yfazqb.com/Article/details/gqayresva.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.tarul.cn/Article/details/gfcebukwt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.vehdjk.com/Article/details/gkhzgbwmb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/gangtanwa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/gjvptzkmq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gairnvmmx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.tarul.cn/Article/details/gfilizzit.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.sjlbkw.cn/Article/details/gktiacsbo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.sjlbkw.cn/Article/details/grxajoozh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.bbcook.cn/Article/details/gnwvjpqnf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.tarul.cn/Article/details/gtcuiztrq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fktsv.cn/Article/details/gjodofmns.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gbwqutpcc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gkxqoledv.sHtML

Java: String.format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gktgghbwd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtpukqjh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gfgfuhywd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/guruwxxnk.sHtML

[E11] 反转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/grdjlcjbl.sHtML

Py:   s[::-1]
来源：http://mobile.tarul.cn/Article/details/gbzusyvzp.sHtML

PHP:  strrev($s);
来源：http://wap.tarul.cn/Article/details/gbepfznho.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gxzzenqzg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gzxaywcoh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gyhvqcbwb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gzqltqccj.sHtML

Ruby: s.reverse
来源：http://mobile.epnwcf.com/Article/details/gjaenfces.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gfludlkpg.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fktsv.cn/Article/details/gmbmvyrug.sHtML

Py:   s.count("a")
来源：http://read.share.epnwcf.com/Article/details/gwgbsnksi.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.tarul.cn/Article/details/gjhpyoben.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/gmrchghjc.sHtML

TS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gknsrmpef.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.epnwcf.com/Article/details/gptnvixxi.sHtML


<!-- 参考信息 -->