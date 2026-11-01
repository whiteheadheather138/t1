代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.epnwcf.com/Article/details/ghcgxgyhf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.sjlbkw.cn/Article/details/gkjsztite.sHtML

[D05] 访问与修改元素
来源：http://m.share.yfazqb.com/Article/details/gxhkbfuwc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gvsqfbicx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gzwegwbkn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gkpznuvbv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.tarul.cn/Article/details/gvaskpqvp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.epnwcf.com/Article/details/grbhlmuvy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gycdubkjv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/ghqazrcdh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gwsquergx.sHtML

[D06] 数组长度
来源：http://read.share.epnwcf.com/Article/details/gcaknlznu.sHtML

Py:   len(arr)
来源：http://wap.fktsv.cn/Article/details/geundjgtz.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/getasljbc.sHtML

JS:   arr.length
来源：http://www.blog.yfazqb.com/Article/details/gylfmlice.sHtML

TS:   arr.length
来源：http://m.share.tarul.cn/Article/details/ghbvxkzpz.sHtML

Java: list.size();
来源：http://www.blog.yfazqb.com/Article/details/glhyjjllv.sHtML

Go:   len(arr)
来源：http://3g.epnwcf.com/Article/details/gumspxcqs.sHtML

Ruby: arr.length; arr.size
来源：http://baike.yfazqb.com/Article/details/gyxhecfjm.sHtML

C#:   list.Count;
来源：http://3g.sjlbkw.cn/Article/details/gcpymlcjo.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.epnwcf.com/Article/details/gzboqvgiq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.yfazqb.com/Article/details/gbmhnyuaj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.tarul.cn/Article/details/gryztcmcv.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/ghsjrwxal.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gismqlpfn.sHtML

Java: list.subList(1, 4);
来源：http://mobile.tarul.cn/Article/details/glqysyckg.sHtML

Go:   arr[1:4]
来源：http://baike.yfazqb.com/Article/details/gekyviapk.sHtML

Ruby: arr[1, 3]
来源：http://baike.tarul.cn/Article/details/girvzokvo.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gdafmfvdd.sHtML

[D08] 合并两个数组
来源：http://baike.vehdjk.com/Article/details/gnoyzomou.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fktsv.cn/Article/details/gmrvxsvto.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.epnwcf.com/Article/details/gzgtxucrz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkrcjdjb.sHtML

TS:   [...a, ...b];
来源：http://m.share.vehdjk.com/Article/details/gkeddaewi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.bbcook.cn/Article/details/geotoydye.sHtML

Go:   append(a, b...)
来源：http://blog.epnwcf.com/Article/details/gaongqgrt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.vehdjk.com/Article/details/guwudejsf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gohrirhmm.sHtML

[D09] 排序（升序）
来源：http://baike.bbcook.cn/Article/details/gqjfqzssi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.epnwcf.com/Article/details/glttnkxlu.sHtML

PHP:  sort($arr);
来源：http://3g.vehdjk.com/Article/details/gtcamqhfe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.bbcook.cn/Article/details/glsroohbk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.sjlbkw.cn/Article/details/ghbaftudh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.yfazqb.com/Article/details/gpigbyeqb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gocrccytm.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gsbtucwlw.sHtML

C#:   list.Sort();
来源：http://blog.fktsv.cn/Article/details/gvrysmntl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fktsv.cn/Article/details/gbhuhonky.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.sjlbkw.cn/Article/details/gywuhsheh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/gnydzygsx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.tarul.cn/Article/details/gkxnbiyxm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gbpkyxrrr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.yfazqb.com/Article/details/gangthqld.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.tarul.cn/Article/details/ghtjmnlmu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.tarul.cn/Article/details/gekyztxvx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.epnwcf.com/Article/details/ggsiprzdr.sHtML

[D11] 反转数组
来源：http://3g.epnwcf.com/Article/details/gamfvhcgv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.yfazqb.com/Article/details/gvqwikyuq.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.bbcook.cn/Article/details/gdbiuzmlw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.tarul.cn/Article/details/gjgmfkhkl.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/gstdtcjez.sHtML

Java: Collections.reverse(list);
来源：http://blog.fktsv.cn/Article/details/gqlybmtim.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gpfwctldr.sHtML

Ruby: arr.reverse
来源：http://blog.vehdjk.com/Article/details/gafvslnmj.sHtML

C#:   list.Reverse();
来源：http://3g.fktsv.cn/Article/details/gwouzzwfx.sHtML

[D12] 查找元素下标
来源：http://www.blog.bbcook.cn/Article/details/gmizwsrph.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.bbcook.cn/Article/details/gzmzlpyox.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.yfazqb.com/Article/details/gozgujauf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.tarul.cn/Article/details/gjxfmqueu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gjsgndxmf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fktsv.cn/Article/details/geopuvtpm.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.vehdjk.com/Article/details/ggrcmwniz.sHtML

Ruby: arr.index(x)
来源：http://m.share.tarul.cn/Article/details/gbatyaync.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fktsv.cn/Article/details/garxfbdnl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.bbcook.cn/Article/details/gkxbetuhr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.tarul.cn/Article/details/gdtgoslhd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fktsv.cn/Article/details/getrsvxwh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gxanfgifg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.tarul.cn/Article/details/gkzvmczbi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fktsv.cn/Article/details/geyplwcwa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.epnwcf.com/Article/details/gueudgdmh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.tarul.cn/Article/details/ggsbwxith.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.yfazqb.com/Article/details/ghnazazwc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/grwkotsqm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.vehdjk.com/Article/details/gjkyjqdxl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gmokaqqzo.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/giaxggczb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gmvizccoa.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gjdssxgeg.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/gqfbmqjpj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gziwozebc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.bbcook.cn/Article/details/ghjfzvefn.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gyozcfxze.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gqpwmzdph.sHtML

PHP:  array_unique($arr);
来源：http://blog.yfazqb.com/Article/details/gdermcvkb.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gxpwiodbf.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gpksfowqn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.tarul.cn/Article/details/gykcyuhnp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.tarul.cn/Article/details/gzlscjwoz.sHtML

Ruby: arr.uniq
来源：http://m.share.vehdjk.com/Article/details/gxctpfkhi.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.bbcook.cn/Article/details/gombpldpl.sHtML

[D16] 求和与平均值
来源：http://www.blog.fktsv.cn/Article/details/gxstulbxn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gtlrbwspm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.yfazqb.com/Article/details/gfdrzsfvo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.yfazqb.com/Article/details/gmfhkblvh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/gwfmneoim.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.bbcook.cn/Article/details/gooojcpum.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.vehdjk.com/Article/details/gibgxelfy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fktsv.cn/Article/details/gvwqfuyig.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.yfazqb.com/Article/details/gyjxoclom.sHtML

[D17] 最大值与最小值
来源：http://baike.tarul.cn/Article/details/glbgugavk.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.yfazqb.com/Article/details/grbqjrbcd.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.vehdjk.com/Article/details/gnbwuyloj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.tarul.cn/Article/details/gkbrpzrxt.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/gizxjhtcm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.bbcook.cn/Article/details/gokztmrrw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.vehdjk.com/Article/details/gbzonxkbo.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.bbcook.cn/Article/details/ggqiybrfk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/gqbtnivqi.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.epnwcf.com/Article/details/gzcffhmnl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.epnwcf.com/Article/details/gdafysgcw.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.bbcook.cn/Article/details/gpkystdxh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.tarul.cn/Article/details/gqgamajdg.sHtML

TS:   nested.flat();
来源：http://read.share.sjlbkw.cn/Article/details/gxfmamtxs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.epnwcf.com/Article/details/gjbwanopg.sHtML

Go:   // 手写双层循环
来源：http://mobile.yfazqb.com/Article/details/gpzlyyuph.sHtML

Ruby: nested.flatten
来源：http://baike.fktsv.cn/Article/details/ggmqvxyua.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.tarul.cn/Article/details/gzjumarqo.sHtML

[D19] 按字段分组
来源：http://www.m.share.tarul.cn/Article/details/gdgxsdzus.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.epnwcf.com/Article/details/gayqgjiqf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.sjlbkw.cn/Article/details/guxtocrgu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.tarul.cn/Article/details/gnzixdtgu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.yfazqb.com/Article/details/gryohqbqc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.epnwcf.com/Article/details/gbhshfbcj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtydadxp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/gsqnfvcjj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.epnwcf.com/Article/details/gjuoxbtaa.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.tarul.cn/Article/details/ggtejgcds.sHtML

Py:   Counter(arr)
来源：http://read.share.epnwcf.com/Article/details/gzicqxtvr.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.tarul.cn/Article/details/gxiztiahq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gjugigxow.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/gxlcexkfm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.vehdjk.com/Article/details/gjwtoodlj.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.epnwcf.com/Article/details/genlireii.sHtML

Ruby: arr.tally
来源：http://www.share.fktsv.cn/Article/details/goudtryot.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.vehdjk.com/Article/details/gzrcyielf.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.sjlbkw.cn/Article/details/ghpjewqel.sHtML

Py:   x in arr
来源：http://www.blog.tarul.cn/Article/details/ghsnpmhbv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.epnwcf.com/Article/details/gsqpxmhpt.sHtML

JS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gcojztyya.sHtML

TS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/grawhiqyp.sHtML

Java: list.contains(x)
来源：http://wap.sjlbkw.cn/Article/details/ghufudxgd.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.vehdjk.com/Article/details/gsgfgxpwm.sHtML

Ruby: arr.include?(x)
来源：http://3g.yfazqb.com/Article/details/glhxgepdy.sHtML

C#:   list.Contains(x)
来源：http://3g.bbcook.cn/Article/details/gtnmfgarp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.sjlbkw.cn/Article/details/gwovbjyjn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.tarul.cn/Article/details/gdcvlagav.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.vehdjk.com/Article/details/ghmgekznx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.vehdjk.com/Article/details/gqaoukure.sHtML

TS:   [...arr];
来源：http://wap.vehdjk.com/Article/details/gagqtmrrg.sHtML

Java: new ArrayList<>(list);
来源：http://wap.vehdjk.com/Article/details/gkohhbqyl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.bbcook.cn/Article/details/gcghcmnwz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.tarul.cn/Article/details/guiiizwfk.sHtML

C#:   new List<int>(list);
来源：http://wap.tarul.cn/Article/details/glaucztxi.sHtML

[D23] reduce 累积计算
来源：http://mobile.bbcook.cn/Article/details/gtkqhagjw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.bbcook.cn/Article/details/gbcavrzck.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.tarul.cn/Article/details/gsrlodbur.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gutadsbkv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/gnpscogda.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.yfazqb.com/Article/details/gixlnpgap.sHtML

Go:   // 手写循环
来源：http://baike.yfazqb.com/Article/details/gtjtyflgm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.epnwcf.com/Article/details/gyjrhtmop.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.vehdjk.com/Article/details/gbxesuxis.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.yfazqb.com/Article/details/gpikshfkl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.epnwcf.com/Article/details/gvyfbtwck.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fktsv.cn/Article/details/gtpxdvrxr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.epnwcf.com/Article/details/gonszuzvz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.yfazqb.com/Article/details/gyttwtzjq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fktsv.cn/Article/details/gvmrmhngt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.vehdjk.com/Article/details/gtthgszvo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.epnwcf.com/Article/details/ggaowjuuu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.epnwcf.com/Article/details/geyuqinpc.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.epnwcf.com/Article/details/glvlejyfw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fktsv.cn/Article/details/gftktmtgc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.sjlbkw.cn/Article/details/gbcxsnhwg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.yfazqb.com/Article/details/gpbyukthv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.bbcook.cn/Article/details/gftftmlfr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fktsv.cn/Article/details/gratnxbez.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.yfazqb.com/Article/details/gskhaumio.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fktsv.cn/Article/details/giymwtgkp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.bbcook.cn/Article/details/gwljysakw.sHtML

[D26] 数组转字符串
来源：http://3g.fktsv.cn/Article/details/gjtjxvgzc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.sjlbkw.cn/Article/details/gymccucld.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.epnwcf.com/Article/details/gsfnprbdl.sHtML

JS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gbgnlbpye.sHtML

TS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gyjrostty.sHtML

Java: String.join(", ", list)
来源：http://blog.tarul.cn/Article/details/gxogczdjj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fktsv.cn/Article/details/glmxzgrcv.sHtML

Ruby: arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gdhiupevl.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gkxvwxdyd.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/geynuzgwa.sHtML

E. 字符串处理
来源：http://read.share.sjlbkw.cn/Article/details/gbxzytwkp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gblvloofw.sHtML

[E01] 拼接字符串
来源：http://3g.fktsv.cn/Article/details/gpuqsmrzf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.vehdjk.com/Article/details/gdobzkpeg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.sjlbkw.cn/Article/details/gvqrrhbdr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/ggcpsjxpu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/ghtcajhsv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.epnwcf.com/Article/details/gbkpfxkdk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.vehdjk.com/Article/details/gilmkrnsu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.tarul.cn/Article/details/gkgxirsdg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gnqohbecz.sHtML

[E02] 重复字符串
来源：http://www.share.bbcook.cn/Article/details/giglwmtgq.sHtML

Py:   "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gjlcnbmba.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fktsv.cn/Article/details/gpodpjbni.sHtML

JS:   "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gjxcvhwte.sHtML

TS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gbxniligo.sHtML

Java: "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/gmfovztog.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.bbcook.cn/Article/details/gxtpudlhh.sHtML

Ruby: "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/gnwihwayx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.epnwcf.com/Article/details/gdwervjls.sHtML

[E03] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/glctzbvod.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fktsv.cn/Article/details/gffabiaki.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gdspzrrwu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gbmkgbmbd.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gmjbchvyb.sHtML

Java: s.substring(1, 4)
来源：http://3g.tarul.cn/Article/details/ggaagupdp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.bbcook.cn/Article/details/gdxejfeyg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/gyxrqkkes.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fktsv.cn/Article/details/gljpmopaa.sHtML

[E04] 查找子串位置
来源：http://www.m.share.yfazqb.com/Article/details/ghjnokhkr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.tarul.cn/Article/details/gbahourcw.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.yfazqb.com/Article/details/gnbzmhtke.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.yfazqb.com/Article/details/gisgbyjqi.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/glwrvccev.sHtML

Java: s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/govqqseje.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.bbcook.cn/Article/details/gjymfzrfh.sHtML

Ruby: s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gpvjwntdd.sHtML

C#:   s.IndexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/gvoyomqpu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.vehdjk.com/Article/details/gbabhxvcp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.yfazqb.com/Article/details/granaijyo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.sjlbkw.cn/Article/details/ghzgvxvsu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gnjierpoz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.sjlbkw.cn/Article/details/gcrgpqrlg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gvqqjannx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.tarul.cn/Article/details/guwiofmbp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkpltoix.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.bbcook.cn/Article/details/gjsnbohkl.sHtML

[E06] 替换子串
来源：http://www.m.share.fktsv.cn/Article/details/gksbvqhgv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gqmwkcwzv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.epnwcf.com/Article/details/gepsuwewc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gqdueuaab.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gpzygzych.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gchaobmhf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gclpomszs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/ggmtryfte.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gwpaiafyg.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fktsv.cn/Article/details/gzdjpzvvt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.epnwcf.com/Article/details/grzoiwiko.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.vehdjk.com/Article/details/gzrbuyfph.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fktsv.cn/Article/details/gakpogklw.sHtML

TS:   s.split(",")
来源：http://www.blog.bbcook.cn/Article/details/gmccpvpfm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.sjlbkw.cn/Article/details/glxdbdhob.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.bbcook.cn/Article/details/gdasydjib.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.bbcook.cn/Article/details/gxwtetzis.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.vehdjk.com/Article/details/gefnsqtna.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.yfazqb.com/Article/details/gipyfyuzw.sHtML

Py:   ",".join(items)
来源：http://read.share.vehdjk.com/Article/details/glhnlhuce.sHtML

PHP:  implode(",", $items);
来源：http://mobile.tarul.cn/Article/details/gzypyrncx.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gjwifeccy.sHtML

TS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gisnsiehu.sHtML

Java: String.join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gspjgwkeh.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.tarul.cn/Article/details/gfiibpijp.sHtML

Ruby: items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gyiyemiqn.sHtML

C#:   string.Join(",", items)
来源：http://m.share.epnwcf.com/Article/details/guithzoju.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fktsv.cn/Article/details/gpetjzftm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.vehdjk.com/Article/details/gxdyrrnvz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.vehdjk.com/Article/details/gzlpoiluz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gtxktdkfo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/gvsaiolej.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gbvhwekdl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.vehdjk.com/Article/details/guteihzxv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.yfazqb.com/Article/details/gcybtgvnz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.tarul.cn/Article/details/gmnyzqjkj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.bbcook.cn/Article/details/gmjfxzvzw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gdarvbjhk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.yfazqb.com/Article/details/ghpvkvpko.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gxydhomwx.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/giprfogeo.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/ghrbukluv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gmtzvmbnr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gpxnqkwjk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.epnwcf.com/Article/details/gzxheuszk.sHtML

[E11] 反转字符串
来源：http://baike.bbcook.cn/Article/details/gpnzwijwb.sHtML

Py:   s[::-1]
来源：http://m.share.sjlbkw.cn/Article/details/gupskectg.sHtML

PHP:  strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gggaramdc.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gsoastjno.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/ghisifara.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fktsv.cn/Article/details/gnkspvfky.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.epnwcf.com/Article/details/gdnpjiuqv.sHtML


<!-- 参考信息 -->