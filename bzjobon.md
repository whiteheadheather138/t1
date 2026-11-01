代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.vehdjk.com/Article/details/gbekaqgta.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.epnwcf.com/Article/details/gaqgjrkgv.sHtML

[D05] 访问与修改元素
来源：http://www.blog.vehdjk.com/Article/details/gbjebdape.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gbmctmbxw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gwfecedbw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gqmstpedp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.yfazqb.com/Article/details/gcuejlkrk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.vehdjk.com/Article/details/glisrjtep.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gxejbrkop.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gsheqccdh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gmkumyrpw.sHtML

[D06] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gfdhijrwk.sHtML

Py:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/gcizzhhob.sHtML

PHP:  count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gnkiagxwz.sHtML

JS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/gxutlszcb.sHtML

TS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/gkwbsssid.sHtML

Java: list.size();
来源：http://www.m.share.bbcook.cn/Article/details/gbkshvnwb.sHtML

Go:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/gvwpoggaa.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fktsv.cn/Article/details/gumfyyvfk.sHtML

C#:   list.Count;
来源：http://mobile.vehdjk.com/Article/details/gleigpzdi.sHtML

[D07] 切片 / 取子数组
来源：http://blog.bbcook.cn/Article/details/gngerghtn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.tarul.cn/Article/details/ghkcengyo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gapogbpwz.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gezlzsrns.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gruynjqos.sHtML

Java: list.subList(1, 4);
来源：http://www.share.vehdjk.com/Article/details/ghowbsslk.sHtML

Go:   arr[1:4]
来源：http://wap.bbcook.cn/Article/details/gkvhmqecp.sHtML

Ruby: arr[1, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gneurbjfs.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fktsv.cn/Article/details/gdqrwafbr.sHtML

[D08] 合并两个数组
来源：http://www.share.sjlbkw.cn/Article/details/gqzrplzss.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.bbcook.cn/Article/details/gzdygxpdv.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.bbcook.cn/Article/details/gbmeavszx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.yfazqb.com/Article/details/gmimxryyx.sHtML

TS:   [...a, ...b];
来源：http://read.share.tarul.cn/Article/details/gveuwucsv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.bbcook.cn/Article/details/gcpzjazaf.sHtML

Go:   append(a, b...)
来源：http://baike.vehdjk.com/Article/details/gygunwrnx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.tarul.cn/Article/details/gfohunrtg.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fktsv.cn/Article/details/gmdesdhtd.sHtML

[D09] 排序（升序）
来源：http://baike.epnwcf.com/Article/details/gomllzrpa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gregoswey.sHtML

PHP:  sort($arr);
来源：http://mobile.bbcook.cn/Article/details/gnivwiwxh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fktsv.cn/Article/details/ggjmpehpz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.tarul.cn/Article/details/grbzvtybi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.bbcook.cn/Article/details/geozmglzw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/gptxgfwds.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/gdwlebhse.sHtML

C#:   list.Sort();
来源：http://mobile.tarul.cn/Article/details/gxyghmucj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.vehdjk.com/Article/details/gzribvutc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.yfazqb.com/Article/details/guzpqiyqt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.tarul.cn/Article/details/gbmkhoyjw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/ghawiscgf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gcentwsfi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.tarul.cn/Article/details/genfvmihr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.bbcook.cn/Article/details/gjnlkxrnd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.bbcook.cn/Article/details/gwawyyvtn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.tarul.cn/Article/details/gzddghoky.sHtML

[D11] 反转数组
来源：http://wap.vehdjk.com/Article/details/gakiawxmc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.tarul.cn/Article/details/gceiatgak.sHtML

PHP:  array_reverse($arr);
来源：http://blog.vehdjk.com/Article/details/ggukeguxl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.tarul.cn/Article/details/gndeshlot.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fktsv.cn/Article/details/gjfvzkhzi.sHtML

Java: Collections.reverse(list);
来源：http://wap.yfazqb.com/Article/details/gchdbteal.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.epnwcf.com/Article/details/gkmmzfjwb.sHtML

Ruby: arr.reverse
来源：http://blog.yfazqb.com/Article/details/ghmmkdlyn.sHtML

C#:   list.Reverse();
来源：http://wap.sjlbkw.cn/Article/details/gkkztenxt.sHtML

[D12] 查找元素下标
来源：http://www.blog.epnwcf.com/Article/details/gvqnnsekg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/gllsxulrr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fktsv.cn/Article/details/govcjeegb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.tarul.cn/Article/details/gcplqfmli.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/glzotxqiq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.vehdjk.com/Article/details/gdxyntrre.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gaitghhwf.sHtML

Ruby: arr.index(x)
来源：http://www.share.yfazqb.com/Article/details/ghkydtrhp.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/gyqcxfobk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.vehdjk.com/Article/details/gfrpdyvnb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.epnwcf.com/Article/details/ggksjoggb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkydkgtp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/gkhusmsmg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gwrsovjow.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fktsv.cn/Article/details/gewxdtrjv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.bbcook.cn/Article/details/gmyzaeiat.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gavvahkgi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.bbcook.cn/Article/details/gnecgrhwh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.vehdjk.com/Article/details/gxbtbcust.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.epnwcf.com/Article/details/ghuckmbur.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.bbcook.cn/Article/details/gxgjcvpkb.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/gkhuafujy.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/giaiyhyfj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.vehdjk.com/Article/details/gdcgcdnqu.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gzmvrrpqm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gflljicgn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gecprlwav.sHtML

[D15] 去重
来源：http://www.m.share.fktsv.cn/Article/details/gbevkofad.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/gdicvxpnd.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.epnwcf.com/Article/details/gbcphbxga.sHtML

JS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/grmswkrpw.sHtML

TS:   [...new Set(arr)]
来源：http://blog.yfazqb.com/Article/details/gxjkfdrrj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/gizjcjmon.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.bbcook.cn/Article/details/gojdocgzx.sHtML

Ruby: arr.uniq
来源：http://m.share.bbcook.cn/Article/details/gnsqmgmyy.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.yfazqb.com/Article/details/gwmzfzwlx.sHtML

[D16] 求和与平均值
来源：http://blog.sjlbkw.cn/Article/details/gcctkzqcs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.epnwcf.com/Article/details/grvsluguz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fktsv.cn/Article/details/glrafchsf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/gvftawsip.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/gsfxzmkpd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fktsv.cn/Article/details/gvugwxrxd.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gokmuddeg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fktsv.cn/Article/details/gzodmqafh.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.vehdjk.com/Article/details/gwfpkebmv.sHtML

[D17] 最大值与最小值
来源：http://baike.tarul.cn/Article/details/ghyevkwol.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fktsv.cn/Article/details/gxhrjecms.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.tarul.cn/Article/details/gfkqtyaqf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.yfazqb.com/Article/details/gugecbhlg.sHtML

TS:   Math.max(...arr);
来源：http://read.share.yfazqb.com/Article/details/gekpmbgej.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fktsv.cn/Article/details/glranyyek.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.tarul.cn/Article/details/gipdwdoty.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.vehdjk.com/Article/details/gigsusfln.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.tarul.cn/Article/details/ghgecllsp.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.tarul.cn/Article/details/gvdfmfufb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fktsv.cn/Article/details/gdiozfboi.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.yfazqb.com/Article/details/gnhkvawud.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.yfazqb.com/Article/details/gmdjukrxd.sHtML

TS:   nested.flat();
来源：http://www.share.epnwcf.com/Article/details/gfhfhupuc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.epnwcf.com/Article/details/gkssxezhr.sHtML

Go:   // 手写双层循环
来源：http://3g.yfazqb.com/Article/details/gxlioxngh.sHtML

Ruby: nested.flatten
来源：http://3g.fktsv.cn/Article/details/gcekwyxqh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqonzhuas.sHtML

[D19] 按字段分组
来源：http://3g.yfazqb.com/Article/details/gddkienir.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/gwentsrps.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.vehdjk.com/Article/details/gbkfrnpsy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.bbcook.cn/Article/details/gbldpxhxk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/gitjtofbs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.tarul.cn/Article/details/gnebasnqz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.bbcook.cn/Article/details/gwoqrebym.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.yfazqb.com/Article/details/gxoswbqoa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.bbcook.cn/Article/details/gexflexut.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fktsv.cn/Article/details/gobtxlltr.sHtML

Py:   Counter(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmifidjer.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gfwviezjr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/gzynjcukz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/gthomescc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.epnwcf.com/Article/details/gniigavqe.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.sjlbkw.cn/Article/details/gttckenqw.sHtML

Ruby: arr.tally
来源：http://mobile.yfazqb.com/Article/details/gynnukjwh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fktsv.cn/Article/details/gzjurheau.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.yfazqb.com/Article/details/gjjqwnewz.sHtML

Py:   x in arr
来源：http://www.blog.vehdjk.com/Article/details/gjehihisd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.yfazqb.com/Article/details/gxppzsdak.sHtML

JS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/gnhurhdhe.sHtML

TS:   arr.includes(x)
来源：http://www.share.epnwcf.com/Article/details/gnpyrkhff.sHtML

Java: list.contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gihicytsc.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/guhypwtde.sHtML

Ruby: arr.include?(x)
来源：http://baike.yfazqb.com/Article/details/griwncqqd.sHtML

C#:   list.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/ggvdxbtmg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.yfazqb.com/Article/details/gsulfqdtv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.yfazqb.com/Article/details/gjcdbaatz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fktsv.cn/Article/details/gspchmmfc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.epnwcf.com/Article/details/ggymidjvg.sHtML

TS:   [...arr];
来源：http://wap.yfazqb.com/Article/details/getgtrsbn.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fktsv.cn/Article/details/glnujpjqy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.vehdjk.com/Article/details/gppdtutvm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.bbcook.cn/Article/details/gqvzymheo.sHtML

C#:   new List<int>(list);
来源：http://blog.sjlbkw.cn/Article/details/gawegxant.sHtML

[D23] reduce 累积计算
来源：http://wap.yfazqb.com/Article/details/gqacvwwkn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.sjlbkw.cn/Article/details/grozoclvc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.sjlbkw.cn/Article/details/grtzgnmps.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.bbcook.cn/Article/details/gjpzehqpx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gxfwmdncb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.sjlbkw.cn/Article/details/gdepmbyix.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gomoazbgq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.tarul.cn/Article/details/gvjleekdu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fktsv.cn/Article/details/giuaadxnt.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.sjlbkw.cn/Article/details/gzugpnsbk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fktsv.cn/Article/details/gvjevuusl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.epnwcf.com/Article/details/gedmalrrt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fktsv.cn/Article/details/gevvouwue.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.vehdjk.com/Article/details/gvrkcbmfp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.bbcook.cn/Article/details/gcreedmfe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.bbcook.cn/Article/details/gfsiwmzvc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.yfazqb.com/Article/details/grtgzirzd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fktsv.cn/Article/details/gwqdikifo.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.sjlbkw.cn/Article/details/gpfknnzsh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.sjlbkw.cn/Article/details/gidfisjui.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjyxzpto.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fktsv.cn/Article/details/gfbxpsmdw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.vehdjk.com/Article/details/gajcyexzf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.bbcook.cn/Article/details/gzidfozkg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fktsv.cn/Article/details/gpeiylggo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.bbcook.cn/Article/details/gzfzyajvw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.bbcook.cn/Article/details/gzdivrcga.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/gdzeplcfc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.vehdjk.com/Article/details/gxjujzzwb.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.bbcook.cn/Article/details/gvxdumwkb.sHtML

JS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gytbigiam.sHtML

TS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gkznsvdfg.sHtML

Java: String.join(", ", list)
来源：http://read.share.epnwcf.com/Article/details/gurqbdabe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fktsv.cn/Article/details/garhjxzra.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gdgdablog.sHtML

C#:   string.Join(", ", list)
来源：http://wap.vehdjk.com/Article/details/gazbgsvte.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/glfozcdtq.sHtML

E. 字符串处理
来源：http://read.share.vehdjk.com/Article/details/ghikeddwk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzwwxwzhe.sHtML

[E01] 拼接字符串
来源：http://m.share.tarul.cn/Article/details/gehwoyxxc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.sjlbkw.cn/Article/details/gxrjefmgp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.epnwcf.com/Article/details/gfabigcyy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.epnwcf.com/Article/details/gedouywzp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/glbrofexk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.epnwcf.com/Article/details/gzubtlstf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fktsv.cn/Article/details/gpbnfaefm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.tarul.cn/Article/details/gpijhtzfh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gdtvitcyt.sHtML

[E02] 重复字符串
来源：http://blog.fktsv.cn/Article/details/gnvnwgewb.sHtML

Py:   "ab" * 3
来源：http://blog.tarul.cn/Article/details/gfqdayznw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.tarul.cn/Article/details/gykasildm.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/ggttohsjp.sHtML

TS:   "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gjwpbzvmo.sHtML

Java: "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/ggpgupnef.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.vehdjk.com/Article/details/geqcvrbsb.sHtML

Ruby: "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/gyltmspjt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.tarul.cn/Article/details/gxjbxpzzt.sHtML

[E03] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gdzazllqu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.tarul.cn/Article/details/gxqrdmdkc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gwoxlzemp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gxjxtmebu.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gkdhzqbiz.sHtML

Java: s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gfpzlfmbv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.tarul.cn/Article/details/gawlzipvd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.sjlbkw.cn/Article/details/goweyqudy.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.vehdjk.com/Article/details/gsosyfckc.sHtML

[E04] 查找子串位置
来源：http://blog.bbcook.cn/Article/details/ggbptrpab.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/gncltkidh.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fktsv.cn/Article/details/gzvkxirql.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.tarul.cn/Article/details/gzcxcyewh.sHtML

TS:   s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gfntqsfhf.sHtML

Java: s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gtvcekhso.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.vehdjk.com/Article/details/gqrwkqvpq.sHtML

Ruby: s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gtwylzbil.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/glkbxctwz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fktsv.cn/Article/details/geabsmhrr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.yfazqb.com/Article/details/gvqgjgykv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.vehdjk.com/Article/details/gpemmzjvu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.vehdjk.com/Article/details/gzfepkkjb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.bbcook.cn/Article/details/gwkmpfmzc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/gqankusnn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.sjlbkw.cn/Article/details/gelmlrzrm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.tarul.cn/Article/details/grusfzoqw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.bbcook.cn/Article/details/ghrdxjbxh.sHtML

[E06] 替换子串
来源：http://wap.epnwcf.com/Article/details/gwcsmqpzr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fktsv.cn/Article/details/gbxyqxzic.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.epnwcf.com/Article/details/gbtiubmdb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gdajiugsn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gnwwbyhms.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/givefhwad.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/gqbtxihrw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gggtedxvl.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.tarul.cn/Article/details/gdprjmrzq.sHtML

[E07] 按分隔符拆分
来源：http://baike.vehdjk.com/Article/details/gbnuzfyve.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/ggcujycia.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gumzaaqax.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.vehdjk.com/Article/details/gonslvlht.sHtML

TS:   s.split(",")
来源：http://3g.bbcook.cn/Article/details/gqmqffndh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.sjlbkw.cn/Article/details/gjtrdvyfz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fktsv.cn/Article/details/gjeqiwczw.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.sjlbkw.cn/Article/details/gyfzktbsg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.yfazqb.com/Article/details/gigqipqvm.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.yfazqb.com/Article/details/gopdlpvkq.sHtML

Py:   ",".join(items)
来源：http://3g.fktsv.cn/Article/details/gwglhhroz.sHtML

PHP:  implode(",", $items);
来源：http://read.share.tarul.cn/Article/details/gczhyeicl.sHtML

JS:   items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/ghrzwhmle.sHtML

TS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gtseodqsz.sHtML

Java: String.join(",", items)
来源：http://mobile.bbcook.cn/Article/details/gbbyiewtf.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.epnwcf.com/Article/details/gedxznxbn.sHtML

Ruby: items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gftmkrtzo.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/gpsuseaas.sHtML

[E09] 去除所有空白字符
来源：http://read.share.bbcook.cn/Article/details/glyjhxukz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.yfazqb.com/Article/details/grcfhmcnn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.vehdjk.com/Article/details/gpuveiecd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/gnkfbehiv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/griffuiky.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fktsv.cn/Article/details/grfqlhdqg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/gshiujmud.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.vehdjk.com/Article/details/gjngxwcfl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fktsv.cn/Article/details/gzansckyn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.sjlbkw.cn/Article/details/gwbfjqnky.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gnsvzumoz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.yfazqb.com/Article/details/geqsfyhfk.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gbulhqnsd.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/guorqychq.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gbiscwspt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gnukguzpn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gbkauinfw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.sjlbkw.cn/Article/details/guycxezqh.sHtML

[E11] 反转字符串
来源：http://3g.fktsv.cn/Article/details/gttphyxmm.sHtML

Py:   s[::-1]
来源：http://read.share.epnwcf.com/Article/details/grflpcnss.sHtML

PHP:  strrev($s);
来源：http://mobile.vehdjk.com/Article/details/ghysajijs.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gajwugmur.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gafzkdyve.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.sjlbkw.cn/Article/details/gweagxhgm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.vehdjk.com/Article/details/gzkdehars.sHtML


<!-- 参考信息 -->