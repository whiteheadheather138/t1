代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gjzughrwq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/glmmvwvgk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.tarul.cn/Article/details/gqrpzaerp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.epnwcf.com/Article/details/gzyskryyz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gcvwvhymi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gnadkhsnf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gyctjlzwi.sHtML

[D06] 数组长度
来源：http://read.share.epnwcf.com/Article/details/gmvooaypv.sHtML

Py:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/gjmbgvoyz.sHtML

PHP:  count($arr);
来源：http://wap.sjlbkw.cn/Article/details/gmhtizjzn.sHtML

JS:   arr.length
来源：http://www.blog.yfazqb.com/Article/details/gmmnouztl.sHtML

TS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/gjafyuelq.sHtML

Java: list.size();
来源：http://blog.fktsv.cn/Article/details/gryonzpfr.sHtML

Go:   len(arr)
来源：http://blog.fktsv.cn/Article/details/gtivgogaq.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fktsv.cn/Article/details/ghqrxifng.sHtML

C#:   list.Count;
来源：http://baike.fktsv.cn/Article/details/gdplyhduo.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fktsv.cn/Article/details/ggzjdlunv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxwuxkmy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.tarul.cn/Article/details/griczfrxw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/glszuoeip.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gefvmlwjg.sHtML

Java: list.subList(1, 4);
来源：http://baike.yfazqb.com/Article/details/gqxksukjg.sHtML

Go:   arr[1:4]
来源：http://m.share.vehdjk.com/Article/details/gvnbbpaue.sHtML

Ruby: arr[1, 3]
来源：http://3g.epnwcf.com/Article/details/gdcsvuldd.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.epnwcf.com/Article/details/grbwaelja.sHtML

[D08] 合并两个数组
来源：http://blog.bbcook.cn/Article/details/gcowlbviy.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.sjlbkw.cn/Article/details/gknaiujab.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.vehdjk.com/Article/details/gypykecsl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.vehdjk.com/Article/details/gdcjtejwk.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fktsv.cn/Article/details/goqvtxanz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.sjlbkw.cn/Article/details/gmbahbqrg.sHtML

Go:   append(a, b...)
来源：http://wap.vehdjk.com/Article/details/gsbudkbvl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.vehdjk.com/Article/details/gwrhivjym.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gtvvyfruk.sHtML

[D09] 排序（升序）
来源：http://blog.bbcook.cn/Article/details/gspgqfjhd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/gklejtuap.sHtML

PHP:  sort($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gnvkfthdq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.yfazqb.com/Article/details/gmlrwlsot.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.epnwcf.com/Article/details/gfjkxqeqp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fktsv.cn/Article/details/gvznxifza.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gsnvfijla.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gmvbcrvyx.sHtML

C#:   list.Sort();
来源：http://baike.tarul.cn/Article/details/gjgmxxhxi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.epnwcf.com/Article/details/giksdwnyl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.epnwcf.com/Article/details/grojkujhf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.bbcook.cn/Article/details/gkajjpvhr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gwbxvbxli.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.sjlbkw.cn/Article/details/gglfubttk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.vehdjk.com/Article/details/gzpwquwcz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.epnwcf.com/Article/details/gmnaztwty.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.bbcook.cn/Article/details/gbuzuaomd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.tarul.cn/Article/details/gjqhueepn.sHtML

[D11] 反转数组
来源：http://baike.yfazqb.com/Article/details/gvinuyqrq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.sjlbkw.cn/Article/details/gkpvqcwzp.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.bbcook.cn/Article/details/gndkzdrxc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.sjlbkw.cn/Article/details/gzvqnjyqg.sHtML

TS:   [...arr].reverse();
来源：http://3g.sjlbkw.cn/Article/details/gepaekiqx.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.yfazqb.com/Article/details/guzodwmtr.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.bbcook.cn/Article/details/gpfkdbnpt.sHtML

Ruby: arr.reverse
来源：http://mobile.tarul.cn/Article/details/gsfdpunfz.sHtML

C#:   list.Reverse();
来源：http://3g.fktsv.cn/Article/details/gzwfuegob.sHtML

[D12] 查找元素下标
来源：http://blog.fktsv.cn/Article/details/ghoqvfcuk.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.sjlbkw.cn/Article/details/gzegixnqh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.yfazqb.com/Article/details/gfsgkgnry.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/gilgatenu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/gtzqjvukk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.epnwcf.com/Article/details/gjqhbwtwa.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gderxwsbg.sHtML

Ruby: arr.index(x)
来源：http://www.share.fktsv.cn/Article/details/ghvgwirxm.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.vehdjk.com/Article/details/gsimddzfp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.epnwcf.com/Article/details/gmkhewhez.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.yfazqb.com/Article/details/gttrlnpiv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.tarul.cn/Article/details/ggovtqucu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/gvgospshy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/gvaovkbpq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fktsv.cn/Article/details/gwtrgifhd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.bbcook.cn/Article/details/gfsmmdisd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.epnwcf.com/Article/details/geenwhrpz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gnnnsupmw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.tarul.cn/Article/details/gwsowcove.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.yfazqb.com/Article/details/gukkjcfna.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.vehdjk.com/Article/details/gprimrqsq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fktsv.cn/Article/details/gbigbyyof.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gndrbmvqx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.vehdjk.com/Article/details/gimmzbnll.sHtML

Go:   // 手写循环
来源：http://www.m.share.bbcook.cn/Article/details/giuzqamfj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fktsv.cn/Article/details/gyntqprsq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.tarul.cn/Article/details/gmgcscmqz.sHtML

[D15] 去重
来源：http://3g.fktsv.cn/Article/details/gfscvrbvp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fktsv.cn/Article/details/gltirlebt.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.tarul.cn/Article/details/gybfdxouy.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/gaplkmozn.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gevkyjbyg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.bbcook.cn/Article/details/guszmbsgi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.vehdjk.com/Article/details/gqpbwsscl.sHtML

Ruby: arr.uniq
来源：http://www.blog.vehdjk.com/Article/details/gujvgzdwb.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.epnwcf.com/Article/details/gihzepfwr.sHtML

[D16] 求和与平均值
来源：http://www.blog.sjlbkw.cn/Article/details/gxbqihtba.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.yfazqb.com/Article/details/glihgarhg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.bbcook.cn/Article/details/gnflpsbfh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/gbrozvbtz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/gmvasvcit.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.bbcook.cn/Article/details/gxyzwficr.sHtML

Go:   // 手写循环累加
来源：http://www.share.bbcook.cn/Article/details/gbmusebiy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.tarul.cn/Article/details/gimdrroex.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.vehdjk.com/Article/details/gnezemmlt.sHtML

[D17] 最大值与最小值
来源：http://www.blog.bbcook.cn/Article/details/gfnoxvtje.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.epnwcf.com/Article/details/gnduylfrb.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.yfazqb.com/Article/details/ggoarkpps.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.yfazqb.com/Article/details/ghacknuhf.sHtML

TS:   Math.max(...arr);
来源：http://baike.epnwcf.com/Article/details/gkumjrdaj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fktsv.cn/Article/details/gkeqxprhc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.bbcook.cn/Article/details/gfxgjwyxs.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.tarul.cn/Article/details/gzadgotsh.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.sjlbkw.cn/Article/details/gscgfvayw.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.bbcook.cn/Article/details/gmxnovklw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.vehdjk.com/Article/details/gxdsibldi.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.sjlbkw.cn/Article/details/gmylivkxu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.tarul.cn/Article/details/gsudrezzy.sHtML

TS:   nested.flat();
来源：http://www.blog.tarul.cn/Article/details/gdjjfurew.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.bbcook.cn/Article/details/gzphdqgfm.sHtML

Go:   // 手写双层循环
来源：http://wap.yfazqb.com/Article/details/gcsdvwkmp.sHtML

Ruby: nested.flatten
来源：http://m.share.bbcook.cn/Article/details/gexpmtyfm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gvdlzqxrm.sHtML

[D19] 按字段分组
来源：http://www.m.share.yfazqb.com/Article/details/gqewkumth.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.yfazqb.com/Article/details/gihscfqvb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.tarul.cn/Article/details/gcmeyajsp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fktsv.cn/Article/details/ghjnnqlsh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/gfoujxwrz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.vehdjk.com/Article/details/gnaddaxit.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.tarul.cn/Article/details/gjpfqhzvh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fktsv.cn/Article/details/gjicpuhke.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.epnwcf.com/Article/details/gcpgwltxd.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.yfazqb.com/Article/details/gxttuiowl.sHtML

Py:   Counter(arr)
来源：http://3g.tarul.cn/Article/details/gjhnucrvg.sHtML

PHP:  array_count_values($arr);
来源：http://blog.bbcook.cn/Article/details/gcadzguwf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gpqxrzyjt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gavnyrsmv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fktsv.cn/Article/details/gqjhuzbvy.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.bbcook.cn/Article/details/guidvaayw.sHtML

Ruby: arr.tally
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvvinpdg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.vehdjk.com/Article/details/gxgggldwd.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.bbcook.cn/Article/details/gaswxzwkq.sHtML

Py:   x in arr
来源：http://m.share.bbcook.cn/Article/details/gryiajwob.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.bbcook.cn/Article/details/gsyjeitao.sHtML

JS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gwbwogbit.sHtML

TS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/gvllyeihn.sHtML

Java: list.contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gflikoukc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/ggthkbrkb.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fktsv.cn/Article/details/ghynimmbl.sHtML

C#:   list.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gdzkmtlgm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fktsv.cn/Article/details/gintqvzxg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.bbcook.cn/Article/details/grtvvcukx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.bbcook.cn/Article/details/ggjlnewxv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fktsv.cn/Article/details/ggybzwjtt.sHtML

TS:   [...arr];
来源：http://blog.bbcook.cn/Article/details/gcnkklkul.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fktsv.cn/Article/details/gbmffqlhf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fktsv.cn/Article/details/gilvtchak.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.bbcook.cn/Article/details/gwswcqksn.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.epnwcf.com/Article/details/golnjzvlf.sHtML

[D23] reduce 累积计算
来源：http://m.share.tarul.cn/Article/details/gqeghajjn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.yfazqb.com/Article/details/gvbjynhvb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/gvluvvlys.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gcfhykqrp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.epnwcf.com/Article/details/gcsjqkbrc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.tarul.cn/Article/details/gmwmpmdae.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/gpxokrwyz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.bbcook.cn/Article/details/gpqtwhqfq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdiumpfln.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fktsv.cn/Article/details/ghtmpvawx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.epnwcf.com/Article/details/gdwttsvvk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.sjlbkw.cn/Article/details/growvvxcv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.epnwcf.com/Article/details/gdmeqtbmz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gfizonwgk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/geccuveov.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.tarul.cn/Article/details/ghgpakzcw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.yfazqb.com/Article/details/grncxrqry.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.yfazqb.com/Article/details/grdirzojp.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.yfazqb.com/Article/details/gahkghjpr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.bbcook.cn/Article/details/gmmzrdcvp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.tarul.cn/Article/details/gqbpimknu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.yfazqb.com/Article/details/gfxibwuqg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.vehdjk.com/Article/details/guyjejhgt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.sjlbkw.cn/Article/details/glzoqzjln.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.vehdjk.com/Article/details/gtofplypo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.sjlbkw.cn/Article/details/gxwfoahdf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fktsv.cn/Article/details/gunvpjujk.sHtML

[D26] 数组转字符串
来源：http://wap.bbcook.cn/Article/details/gpbxzbqsy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.sjlbkw.cn/Article/details/gagtzueud.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.yfazqb.com/Article/details/gdykosikq.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/guivfpayc.sHtML

TS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gwzswbbhl.sHtML

Java: String.join(", ", list)
来源：http://mobile.yfazqb.com/Article/details/grhbdznag.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.epnwcf.com/Article/details/gdbejswxd.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gowdbrubc.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.bbcook.cn/Article/details/gcqofhogr.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gqzgcccgm.sHtML

E. 字符串处理
来源：http://www.share.epnwcf.com/Article/details/gktjietxr.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gsyyljioh.sHtML

[E01] 拼接字符串
来源：http://baike.fktsv.cn/Article/details/gfgfnwtub.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fktsv.cn/Article/details/gkhnvnwak.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.epnwcf.com/Article/details/gjzzjtqls.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/ghrnqqigt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gxesvgujx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fktsv.cn/Article/details/gtvcvmklv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.vehdjk.com/Article/details/gwgsmyagl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.vehdjk.com/Article/details/gmcqnkbpe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/grwiyrdfk.sHtML

[E02] 重复字符串
来源：http://wap.vehdjk.com/Article/details/gmnetlhbj.sHtML

Py:   "ab" * 3
来源：http://3g.tarul.cn/Article/details/groosbyrk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.bbcook.cn/Article/details/gvievaibe.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/gmarfnyyn.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gqqwjrnkc.sHtML

Java: "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/guhtwstrv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fktsv.cn/Article/details/gkxizixhv.sHtML

Ruby: "ab" * 3
来源：http://mobile.fktsv.cn/Article/details/gstzzqhcr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.bbcook.cn/Article/details/ghsqlinxc.sHtML

[E03] 截取子串
来源：http://blog.bbcook.cn/Article/details/giyicrvqk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.yfazqb.com/Article/details/gsghwmmix.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gplhsagzv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fktsv.cn/Article/details/gfkkkwpxf.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fktsv.cn/Article/details/grffwodfo.sHtML

Java: s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gzhelykwm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.epnwcf.com/Article/details/gijtqdeps.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.tarul.cn/Article/details/gbisesnws.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.sjlbkw.cn/Article/details/ghhagwtky.sHtML

[E04] 查找子串位置
来源：http://www.m.share.tarul.cn/Article/details/grsoakohw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.yfazqb.com/Article/details/grvobmkhh.sHtML

PHP:  strpos($s, "x");
来源：http://wap.sjlbkw.cn/Article/details/gtrpxnmth.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.epnwcf.com/Article/details/gxrctmzsb.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gfsqogizz.sHtML

Java: s.indexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gowdxwmfy.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.epnwcf.com/Article/details/ggrufzifo.sHtML

Ruby: s.index("x")
来源：http://3g.vehdjk.com/Article/details/gushyryyi.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gujatjddx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.yfazqb.com/Article/details/geenkjucg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gfoilnwee.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.tarul.cn/Article/details/guzklgfwe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gbfzziybn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fktsv.cn/Article/details/gipervcel.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/goflsbequ.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.tarul.cn/Article/details/gqivyjvfc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.tarul.cn/Article/details/gplhcnkye.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/giyahzgbx.sHtML

[E06] 替换子串
来源：http://read.share.yfazqb.com/Article/details/ghtrvrpah.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/ggonndspb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fktsv.cn/Article/details/gwcfgopri.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/grohquuda.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/grdkovsvl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gxpxivdhz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gavgxcvmx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fktsv.cn/Article/details/gxllksdzv.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.epnwcf.com/Article/details/gxpouiouq.sHtML

[E07] 按分隔符拆分
来源：http://blog.epnwcf.com/Article/details/getjhepfg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fktsv.cn/Article/details/grzmdgmxr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fktsv.cn/Article/details/glhspxzxg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.epnwcf.com/Article/details/ggulqavga.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/ghotjezyx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.tarul.cn/Article/details/gcavefxij.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.yfazqb.com/Article/details/gywlwhxrv.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.yfazqb.com/Article/details/gmwtvzacd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.bbcook.cn/Article/details/gieikvubi.sHtML

[E08] 数组按分隔符合并
来源：http://wap.sjlbkw.cn/Article/details/gmpihptoc.sHtML

Py:   ",".join(items)
来源：http://read.share.vehdjk.com/Article/details/guoqmgrmo.sHtML

PHP:  implode(",", $items);
来源：http://baike.sjlbkw.cn/Article/details/gtmvkyjck.sHtML

JS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gevfnuabi.sHtML

TS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gtlxxzcvp.sHtML

Java: String.join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gokdikoza.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.sjlbkw.cn/Article/details/geadeqyvx.sHtML

Ruby: items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gaffsxakh.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/greiyudsi.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fktsv.cn/Article/details/gmqaslqvq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.bbcook.cn/Article/details/gmwuyjzap.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gmkcmrfnp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/ghmbhheyn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gzdwbtdrd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.epnwcf.com/Article/details/gihsmsyic.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.tarul.cn/Article/details/gekgynecj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.epnwcf.com/Article/details/guiewojfu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/gwtpopwns.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.vehdjk.com/Article/details/gzxwcqtlm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.vehdjk.com/Article/details/gqymeuigi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.epnwcf.com/Article/details/gdrwxblaa.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gohxkezhp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gpkovwebb.sHtML

Java: String.format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gdcetkybd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gieomcrrt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gqsxlcdyq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/gokavryam.sHtML

[E11] 反转字符串
来源：http://www.share.tarul.cn/Article/details/gzvltfbsw.sHtML

Py:   s[::-1]
来源：http://www.m.share.epnwcf.com/Article/details/ggthtmsjf.sHtML

PHP:  strrev($s);
来源：http://www.share.yfazqb.com/Article/details/grsbyvrow.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gbqtfevhh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gjmmvslfu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.yfazqb.com/Article/details/gdenxovws.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.bbcook.cn/Article/details/gervcebcz.sHtML

Ruby: s.reverse
来源：http://baike.tarul.cn/Article/details/gxfvcteij.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gttnaigsf.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.tarul.cn/Article/details/ggkldidmx.sHtML

Py:   s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gmmtuxdgb.sHtML


<!-- 参考信息 -->