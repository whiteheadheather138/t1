代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/gmtsemszx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gdqjtphvm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.tarul.cn/Article/details/gayrljztz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.bbcook.cn/Article/details/gnizhhonh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gpdyjuwhe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gjvpcuofw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gqwmnzvob.sHtML

[D06] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gnoczsyap.sHtML

Py:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gwlmwwrnf.sHtML

PHP:  count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gvexbhswv.sHtML

JS:   arr.length
来源：http://www.share.tarul.cn/Article/details/glhzifbyj.sHtML

TS:   arr.length
来源：http://baike.tarul.cn/Article/details/gqldwmpku.sHtML

Java: list.size();
来源：http://read.share.sjlbkw.cn/Article/details/gmghtjxxf.sHtML

Go:   len(arr)
来源：http://baike.vehdjk.com/Article/details/gemmxwwbz.sHtML

Ruby: arr.length; arr.size
来源：http://3g.bbcook.cn/Article/details/gtzrsvgyy.sHtML

C#:   list.Count;
来源：http://m.share.sjlbkw.cn/Article/details/gdshxnpzs.sHtML

[D07] 切片 / 取子数组
来源：http://baike.tarul.cn/Article/details/gdiwyctzs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fktsv.cn/Article/details/gyuxlmoll.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.vehdjk.com/Article/details/gywnseogj.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gfbvhvmvx.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gmvwnbisg.sHtML

Java: list.subList(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gxgmkfexr.sHtML

Go:   arr[1:4]
来源：http://m.share.bbcook.cn/Article/details/gmldpylsh.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.tarul.cn/Article/details/gangyksmy.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gtnrhlgli.sHtML

[D08] 合并两个数组
来源：http://blog.epnwcf.com/Article/details/gstzircex.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.vehdjk.com/Article/details/gpxltcnmx.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.tarul.cn/Article/details/gxrvewlxu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.yfazqb.com/Article/details/gexdhbvep.sHtML

TS:   [...a, ...b];
来源：http://www.share.sjlbkw.cn/Article/details/gfowtdytp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gatjyihix.sHtML

Go:   append(a, b...)
来源：http://baike.fktsv.cn/Article/details/gfeohqyln.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.bbcook.cn/Article/details/gtavbowxv.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fktsv.cn/Article/details/gfsjwmrsw.sHtML

[D09] 排序（升序）
来源：http://wap.bbcook.cn/Article/details/gaqqfuzet.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gcjyrticb.sHtML

PHP:  sort($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gyzuzizzd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.tarul.cn/Article/details/gtnhoystm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.tarul.cn/Article/details/gxpllerzm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.vehdjk.com/Article/details/ggazskobs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gpndipaag.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/glarapoxn.sHtML

C#:   list.Sort();
来源：http://wap.fktsv.cn/Article/details/gkfggqauq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fktsv.cn/Article/details/gmkczziko.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.yfazqb.com/Article/details/gbadfcsgd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.epnwcf.com/Article/details/gghafmqdl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.sjlbkw.cn/Article/details/gqwmhksvn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gltbcckhp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.tarul.cn/Article/details/gqjggzqow.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.yfazqb.com/Article/details/gzbtablfz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fktsv.cn/Article/details/glshtzpwj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.yfazqb.com/Article/details/ghaabtarj.sHtML

[D11] 反转数组
来源：http://blog.bbcook.cn/Article/details/gemmkcuyw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.bbcook.cn/Article/details/gebflsash.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fktsv.cn/Article/details/gvugzianh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.tarul.cn/Article/details/grketfsdz.sHtML

TS:   [...arr].reverse();
来源：http://3g.epnwcf.com/Article/details/ghuayeixq.sHtML

Java: Collections.reverse(list);
来源：http://3g.vehdjk.com/Article/details/gmdtaewkr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.vehdjk.com/Article/details/guiixwhqs.sHtML

Ruby: arr.reverse
来源：http://read.share.yfazqb.com/Article/details/gueowoopp.sHtML

C#:   list.Reverse();
来源：http://mobile.yfazqb.com/Article/details/gbtnltacz.sHtML

[D12] 查找元素下标
来源：http://wap.epnwcf.com/Article/details/gtguozbdr.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.yfazqb.com/Article/details/gheaofxhk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gzfsxhunu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.bbcook.cn/Article/details/gzqrnrqgn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/gixngfrbg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.epnwcf.com/Article/details/gvgkjoqrk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/giqzaacoo.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.yfazqb.com/Article/details/gftkjxwow.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fktsv.cn/Article/details/gdxrksskc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fktsv.cn/Article/details/gjpkigzef.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.vehdjk.com/Article/details/gkzhjvlhq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.yfazqb.com/Article/details/gfrtbwoiq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/glxrcpypa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.bbcook.cn/Article/details/gsxjqxjgn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gywoqrhsh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.vehdjk.com/Article/details/gdupqtkub.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.bbcook.cn/Article/details/ganddmkmv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fktsv.cn/Article/details/ghmsbygcs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.tarul.cn/Article/details/gqwiwdvsw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.epnwcf.com/Article/details/gftgvpalj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gseifdiqo.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/gcnnlmrpk.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gkhnjmhvt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.yfazqb.com/Article/details/grxjtlgpo.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/glgmerubu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gluhchnih.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.yfazqb.com/Article/details/gbdzzqbtn.sHtML

[D15] 去重
来源：http://www.m.share.yfazqb.com/Article/details/gftkagkiw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gpxiverum.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.epnwcf.com/Article/details/gfhrawubz.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/glwpwvzgj.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.epnwcf.com/Article/details/gskrfgjho.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.sjlbkw.cn/Article/details/ghyeiaevw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.yfazqb.com/Article/details/gnerkudwi.sHtML

Ruby: arr.uniq
来源：http://mobile.sjlbkw.cn/Article/details/gnfowfsnv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.vehdjk.com/Article/details/gerxkukdx.sHtML

[D16] 求和与平均值
来源：http://wap.epnwcf.com/Article/details/gqoswxtwo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.epnwcf.com/Article/details/gjftspwuc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fktsv.cn/Article/details/gyjoveqmo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/gelbtedhq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.yfazqb.com/Article/details/goivsojfn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.epnwcf.com/Article/details/gzbwvgfev.sHtML

Go:   // 手写循环累加
来源：http://mobile.tarul.cn/Article/details/godcvqtva.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/gfttlxknr.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.sjlbkw.cn/Article/details/gizdoiwrd.sHtML

[D17] 最大值与最小值
来源：http://read.share.epnwcf.com/Article/details/gvlsetcpo.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.tarul.cn/Article/details/ginpatarn.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.bbcook.cn/Article/details/gdorydbcd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.tarul.cn/Article/details/gkkczjoyp.sHtML

TS:   Math.max(...arr);
来源：http://3g.sjlbkw.cn/Article/details/gskkhdzax.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fktsv.cn/Article/details/gelpdfsyf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.bbcook.cn/Article/details/gjkpfwdbs.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.bbcook.cn/Article/details/ggiguhqor.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fktsv.cn/Article/details/gvqzccrrh.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.yfazqb.com/Article/details/gfadnuxyx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.yfazqb.com/Article/details/gjjytgzaw.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fktsv.cn/Article/details/gbosjoctm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.epnwcf.com/Article/details/ghkrwespr.sHtML

TS:   nested.flat();
来源：http://m.share.vehdjk.com/Article/details/grrozrphp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.bbcook.cn/Article/details/gjcgldymq.sHtML

Go:   // 手写双层循环
来源：http://mobile.vehdjk.com/Article/details/gpcsqlfrj.sHtML

Ruby: nested.flatten
来源：http://www.share.sjlbkw.cn/Article/details/gygogbsjd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.sjlbkw.cn/Article/details/grcrkfrlk.sHtML

[D19] 按字段分组
来源：http://blog.tarul.cn/Article/details/gknpneksp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fktsv.cn/Article/details/gyrlabixn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.yfazqb.com/Article/details/gkoviyncr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.yfazqb.com/Article/details/ggrcqvzgj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.sjlbkw.cn/Article/details/gusproazm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.bbcook.cn/Article/details/gkuhfnpto.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.tarul.cn/Article/details/gdegejktw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fktsv.cn/Article/details/gmaprfyxo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.yfazqb.com/Article/details/gvrwtsrgy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.yfazqb.com/Article/details/gbgloypuq.sHtML

Py:   Counter(arr)
来源：http://3g.vehdjk.com/Article/details/gyerkhnqb.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.vehdjk.com/Article/details/gesaxswfd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.bbcook.cn/Article/details/gjzpuaeel.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.epnwcf.com/Article/details/gvvryarwi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fktsv.cn/Article/details/gmlbnqvcp.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.yfazqb.com/Article/details/gxnfnsqst.sHtML

Ruby: arr.tally
来源：http://m.share.sjlbkw.cn/Article/details/gyfalncdy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.vehdjk.com/Article/details/geqhmsayn.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.bbcook.cn/Article/details/ggbtqftpq.sHtML

Py:   x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gxtueqlnc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/gzgkvrvsf.sHtML

JS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gvawvuwxs.sHtML

TS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gwidtzzyc.sHtML

Java: list.contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gbhezsfwx.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.vehdjk.com/Article/details/ggznbtclj.sHtML

Ruby: arr.include?(x)
来源：http://blog.epnwcf.com/Article/details/gryyaatst.sHtML

C#:   list.Contains(x)
来源：http://wap.bbcook.cn/Article/details/guwtrnxja.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.vehdjk.com/Article/details/gqvaqpvma.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gotpwdrta.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.sjlbkw.cn/Article/details/gapqsggps.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.yfazqb.com/Article/details/gajprigrn.sHtML

TS:   [...arr];
来源：http://m.share.bbcook.cn/Article/details/gyqdcgdmq.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.yfazqb.com/Article/details/giaywqswi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.tarul.cn/Article/details/gnpshnyjr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.sjlbkw.cn/Article/details/ggslpcyxz.sHtML

C#:   new List<int>(list);
来源：http://read.share.tarul.cn/Article/details/gknpibiib.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.epnwcf.com/Article/details/gbjdkudrb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.bbcook.cn/Article/details/gqnnjppsm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.tarul.cn/Article/details/geilwceun.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.epnwcf.com/Article/details/gxdwmwrdj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.vehdjk.com/Article/details/giinqtwgz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.tarul.cn/Article/details/gogjisdip.sHtML

Go:   // 手写循环
来源：http://www.share.fktsv.cn/Article/details/gyzrfpiut.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.sjlbkw.cn/Article/details/gsfwlkxfo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.sjlbkw.cn/Article/details/gpmuxnkpo.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.epnwcf.com/Article/details/gfmjzvlln.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.sjlbkw.cn/Article/details/glyuhypvd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.bbcook.cn/Article/details/gayesokcl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gtpfgfevb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gpckcyuhy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gogwvhepi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.epnwcf.com/Article/details/ghzltoshc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.vehdjk.com/Article/details/godkbqufj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.vehdjk.com/Article/details/gwmreeegi.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/girgbjxss.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.sjlbkw.cn/Article/details/gwpojxovw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.vehdjk.com/Article/details/grvayhtjg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.epnwcf.com/Article/details/gzvtluxic.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fktsv.cn/Article/details/gzstbfale.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.epnwcf.com/Article/details/gzexxxrhq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fktsv.cn/Article/details/gtahanvos.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.tarul.cn/Article/details/gkfgdmjna.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.tarul.cn/Article/details/gfznvupvp.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/gsuppojts.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gemwtmtrt.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fktsv.cn/Article/details/gocrierck.sHtML

JS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/giqffgrux.sHtML

TS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gbygluudw.sHtML

Java: String.join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gpusnfyzk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.bbcook.cn/Article/details/gfhelroye.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gyklfcghd.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/grildwkbz.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjonqhltq.sHtML

E. 字符串处理
来源：http://wap.sjlbkw.cn/Article/details/gemkvwnyx.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtledlqfv.sHtML

[E01] 拼接字符串
来源：http://baike.fktsv.cn/Article/details/grhcirfid.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.bbcook.cn/Article/details/gpxoxugca.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.bbcook.cn/Article/details/gisevmicg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gfikfkvtf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/ghczkzkvb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.yfazqb.com/Article/details/gbuukmfna.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.bbcook.cn/Article/details/gyyxlnwea.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fktsv.cn/Article/details/glwiwestf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gtdsdlshc.sHtML

[E02] 重复字符串
来源：http://baike.fktsv.cn/Article/details/gfdipqghy.sHtML

Py:   "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/gvkjxvjpd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.yfazqb.com/Article/details/gpkxlzgow.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gefzjykay.sHtML

TS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gtlktevjw.sHtML

Java: "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gwdtlsttv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.epnwcf.com/Article/details/gvyqahmpv.sHtML

Ruby: "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gvzmyjpsz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.epnwcf.com/Article/details/gkljettty.sHtML

[E03] 截取子串
来源：http://3g.vehdjk.com/Article/details/gacpkkjtt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.sjlbkw.cn/Article/details/gygbitdoy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gcsjmhekw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gabhrrgcs.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.tarul.cn/Article/details/gmjwdlhyp.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxgbfpds.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.tarul.cn/Article/details/gjcjtcgnb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.vehdjk.com/Article/details/gtjwmdbye.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gnjrxzdmy.sHtML

[E04] 查找子串位置
来源：http://blog.bbcook.cn/Article/details/gnvxlqcul.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.tarul.cn/Article/details/guwhwovmk.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.sjlbkw.cn/Article/details/gjybjfxre.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.sjlbkw.cn/Article/details/gzsqmjzdr.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/ghdcanpqt.sHtML

Java: s.indexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gvuhoheug.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.bbcook.cn/Article/details/gnkyvgdyb.sHtML

Ruby: s.index("x")
来源：http://www.share.vehdjk.com/Article/details/ghnpqvurj.sHtML

C#:   s.IndexOf("x")
来源：http://baike.vehdjk.com/Article/details/gtjsilvvw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.bbcook.cn/Article/details/gtljorjax.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.bbcook.cn/Article/details/guqgvvvyd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fktsv.cn/Article/details/gdpbjcfph.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.epnwcf.com/Article/details/glrtsutgl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.yfazqb.com/Article/details/gnxrbtbuj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gdbcyzgwo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.tarul.cn/Article/details/gytrrzhfe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.bbcook.cn/Article/details/gatziyqfc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gceruqxgj.sHtML

[E06] 替换子串
来源：http://blog.fktsv.cn/Article/details/gwklmbxoo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fktsv.cn/Article/details/gkzdecvef.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.tarul.cn/Article/details/gmfxxdjgo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gyqrafejq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gxzjajcho.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gwiwizfjq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.tarul.cn/Article/details/giufljmql.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gaeofnujt.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.vehdjk.com/Article/details/gtpdmxfmd.sHtML

[E07] 按分隔符拆分
来源：http://blog.fktsv.cn/Article/details/gmxwxejvl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.yfazqb.com/Article/details/gndiukkeo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gdphkohij.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.tarul.cn/Article/details/gdfbsgiwh.sHtML

TS:   s.split(",")
来源：http://www.share.vehdjk.com/Article/details/gxmwroyts.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.sjlbkw.cn/Article/details/gpdsqynql.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.sjlbkw.cn/Article/details/gmobyafph.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.vehdjk.com/Article/details/gupwkthrx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.tarul.cn/Article/details/gnskiwqtn.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.tarul.cn/Article/details/gmxbhepix.sHtML

Py:   ",".join(items)
来源：http://m.share.tarul.cn/Article/details/gugshwqpa.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.sjlbkw.cn/Article/details/gufhdsokm.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gralksrba.sHtML

TS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gtvmejqbu.sHtML

Java: String.join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gbafkjfqw.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.tarul.cn/Article/details/gpvglmdns.sHtML

Ruby: items.join(",")
来源：http://wap.vehdjk.com/Article/details/grzovndpk.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/ggvncymsx.sHtML

[E09] 去除所有空白字符
来源：http://read.share.epnwcf.com/Article/details/gudfdcwkc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.bbcook.cn/Article/details/gcpvckxya.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.tarul.cn/Article/details/gviaqlyaf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/glphgfjbh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.bbcook.cn/Article/details/gbcoeizbd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gloewnenx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.sjlbkw.cn/Article/details/gtzsiocfo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.yfazqb.com/Article/details/gmcmfsspu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.tarul.cn/Article/details/gkmijlyge.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/garqtzknr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.epnwcf.com/Article/details/ggamfugsn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.epnwcf.com/Article/details/gjrhzzubs.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/ggbxhldpp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gaoqbekaq.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gwsuywbeb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gedeqdimu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gvuxxhfzb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/gsujmkydx.sHtML

[E11] 反转字符串
来源：http://wap.sjlbkw.cn/Article/details/ggljtichm.sHtML

Py:   s[::-1]
来源：http://3g.bbcook.cn/Article/details/gpzecydcf.sHtML

PHP:  strrev($s);
来源：http://wap.tarul.cn/Article/details/gapymonvn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gbesoadmv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gwukkfnxx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.sjlbkw.cn/Article/details/gdgremwdc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.epnwcf.com/Article/details/gxygbdmrn.sHtML

Ruby: s.reverse
来源：http://3g.bbcook.cn/Article/details/gwcsogeth.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.epnwcf.com/Article/details/geiwhprwi.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fktsv.cn/Article/details/gvzlilinr.sHtML

Py:   s.count("a")
来源：http://wap.epnwcf.com/Article/details/gjjhwdcbr.sHtML


<!-- 参考信息 -->